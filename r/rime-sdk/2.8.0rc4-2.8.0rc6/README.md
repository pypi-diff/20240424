# Comparing `tmp/rime_sdk-2.8.0rc4.tar.gz` & `tmp/rime_sdk-2.8.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rime_sdk-2.8.0rc4.tar", last modified: Wed Apr 10 21:01:22 2024, max compression
+gzip compressed data, was "rime_sdk-2.8.0rc6.tar", last modified: Thu Apr 18 17:21:20 2024, max compression
```

## Comparing `rime_sdk-2.8.0rc4.tar` & `rime_sdk-2.8.0rc6.tar`

### file list

```diff
@@ -1,585 +1,590 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-10 21:01:22.520005 rime_sdk-2.8.0rc4/
--rw-r--r--   0 runner    (1001) runner    (1001)      566 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/LICENSE
--rw-r--r--   0 runner    (1001) runner    (1001)     1275 2024-04-10 21:01:22.520005 rime_sdk-2.8.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      984 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/README.md
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-10 21:01:22.496005 rime_sdk-2.8.0rc4/rime_sdk/
--rw-r--r--   0 runner    (1001) runner    (1001)     1490 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2268 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/authenticator.py
--rw-r--r--   0 runner    (1001) runner    (1001)    71496 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/client.py
--rw-r--r--   0 runner    (1001) runner    (1001)    23353 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/continuous_test.py
--rw-r--r--   0 runner    (1001) runner    (1001)    12282 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/data_collector.py
--rw-r--r--   0 runner    (1001) runner    (1001)      883 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/detection_event.py
--rw-r--r--   0 runner    (1001) runner    (1001)    25061 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/generative_firewall.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3453 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/generative_model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4892 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/image_builder.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-10 21:01:22.496005 rime_sdk-2.8.0rc4/rime_sdk/internal/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/internal/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18350 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/internal/config_parser.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1004 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/internal/constants.py
--rw-r--r--   0 runner    (1001) runner    (1001)      667 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/internal/decorators.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9740 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/internal/file_upload.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1973 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/internal/rest_error_handler.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9361 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/internal/swagger_parser.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2577 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/internal/swagger_utils.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1081 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/internal/test_helpers.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2681 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/internal/throttle_queue.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3570 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/internal/utils.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18764 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/job.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5042 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/monitor.py
--rw-r--r--   0 runner    (1001) runner    (1001)   107184 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/project.py
--rw-r--r--   0 runner    (1001) runner    (1001)    38328 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/registry.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4396 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/schedule.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-10 21:01:22.496005 rime_sdk-2.8.0rc4/rime_sdk/swagger/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-10 21:01:22.496005 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/
--rw-r--r--   0 runner    (1001) runner    (1001)    59356 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-10 21:01:22.496005 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/
--rw-r--r--   0 runner    (1001) runner    (1001)     2411 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)    46640 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5851 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/config_validator_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18207 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    25430 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/data_collector_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11733 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/detection_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    23108 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    17931 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    27750 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/file_upload_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    24169 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/firewall_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    23787 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/firewall_instance_manager_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    22695 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    15262 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/generative_model_testing_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    28916 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/image_registry_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    27170 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/integration_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    27728 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/job_reader_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    21865 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    14474 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/model_testing_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    35026 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    19932 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    74338 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/project_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    57883 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/registry_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    77856 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/results_reader_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4167 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/rime_info_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18249 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/schedule_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    40655 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/user_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    25780 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/validation_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    46472 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    25179 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8845 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-10 21:01:22.520005 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/
--rw-r--r--   0 runner    (1001) runner    (1001)    56846 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4210 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4369 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body1.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4328 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6669 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5483 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5103 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/config_generation_category_config_generation_service_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3706 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/config_generation_profiling_config_generation_service_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3725 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/config_generation_test_suite_config_generation_service_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3435 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8968 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3552 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4503 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3582 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2551 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6687 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
--rw-r--r--   0 runner    (1001) runner    (1001)    17329 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/crossplanetask_cross_plane_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3362 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8011 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4630 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2674 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2695 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7390 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4396 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3292 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6273 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13500 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8080 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4925 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5748 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2705 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5806 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)    14085 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8545 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3410 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)    15539 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4273 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2728 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/detection_event_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2587 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4205 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/detection_resolution.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7745 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2744 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2719 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2670 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4176 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10779 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10808 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_file_security_report.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7556 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_package_url.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7459 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3304 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata_license.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3285 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/fileserver_check_object_exists_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/fileserver_delete_object_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3294 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/fileserver_get_read_object_presigned_link_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3310 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/fileserver_get_upload_object_presigned_link_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3232 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/fileserver_list_objects_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9982 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5075 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3149 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10070 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5158 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6961 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/firewallinstance_firewall_instance_firewall_instance_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2822 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/flagged_substring_request_body_component.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4455 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generative_testing_result_example.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3382 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generative_testing_result_standard_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4502 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3679 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5387 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_custom_pii_entity.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4675 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_denial_of_service_rule_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2722 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6459 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2844 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5781 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3291 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2896 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_tokenizer.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6773 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_flagged_substring.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3517 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_effective_config_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3686 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_instance_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11464 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_individual_rules_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4144 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3934 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_rule_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3740 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_list_firewall_instances_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8681 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_off_topic_rule_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4848 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4877 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_rule_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3752 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_entity_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3712 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3487 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_v2_rule_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9562 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_output.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2808 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_sensitivity.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3447 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_detection_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5128 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_unknown_external_source_rule_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3869 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_update_firewall_instance_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5046 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4841 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)    12694 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2667 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_request_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5869 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7850 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativetesting_model_connection_spec.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4012 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativetesting_objective_sub_category.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3664 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3408 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4422 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4103 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2821 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2770 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3403 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3161 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2808 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4550 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5064 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3344 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/job_data_generative_model_test.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3915 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/job_data_scan.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4710 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4752 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/language_detection_details_language_substring.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4794 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4426 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4187 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_file_scan_results_request_file_scan_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4033 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6007 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5102 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5050 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4570 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3633 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6549 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4842 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4373 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3722 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5728 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5076 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3993 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4508 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2674 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13205 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/model_model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3523 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4142 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2745 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2515 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6262 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4125 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3518 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4963 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)    12705 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2665 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4511 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2667 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3520 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_transform.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2728 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4020 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5602 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3275 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9399 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/notification_notification.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2774 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2644 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/notification_object_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3594 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4781 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6823 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/pii_detection_details_flagged_entity.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4341 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4384 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_activate_schedule_for_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2563 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11026 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3279 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2607 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_deactivate_schedule_for_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2547 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3288 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3190 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4530 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9270 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10536 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)    12754 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5306 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5738 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3739 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_owner_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)    19393 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_project.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2693 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_project_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5013 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_project_with_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2579 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4180 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_schedule_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3279 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2571 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4380 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4765 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2715 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/protobuf_any.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2574 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6648 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_connection_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3375 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4050 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4143 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6599 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)    20609 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_params.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2624 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3454 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4688 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_generative_language_model_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5621 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4998 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4224 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_metadata.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6051 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_model_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3453 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3654 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_open_ai_chat_completion_model_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4161 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_pred_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5645 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2728 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13267 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3218 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5797 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/repo_metadata_reputation.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5037 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2753 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2559 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8702 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_agent.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5337 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_agent_desired_state.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2745 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8524 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2775 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_attack_objective.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2519 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6159 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13366 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2860 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_config_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4337 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3505 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3389 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4997 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6566 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4077 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6407 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3976 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3303 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3478 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3486 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7059 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3324 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6750 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3842 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3407 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3481 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4086 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3371 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7230 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3177 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5393 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_schedule_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3324 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_schedule_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5936 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3212 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7061 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3352 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2559 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2535 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2539 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2551 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3371 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2559 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2539 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_schedule_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2567 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5159 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_detailed_upgrade_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2563 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4600 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6332 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6606 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3344 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3130 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_float_list.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3160 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3462 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3357 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4523 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6063 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3231 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4115 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3631 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3396 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3501 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_file_scan_result_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3265 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3181 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3457 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3122 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3266 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3394 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3365 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3303 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5967 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6275 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3208 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8929 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3381 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3406 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3288 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8541 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4079 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_schedule_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3292 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8955 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_time_series_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4877 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_upgrade_for_agent_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3110 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3147 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4256 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4226 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4316 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3284 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2519 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4368 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3108 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_int_list.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4063 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6446 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_data.py
--rw-r--r--   0 runner    (1001) runner    (1001)    14784 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2865 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2617 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_view.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2611 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_language.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2904 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2770 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5439 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2672 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4968 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4995 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3283 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4835 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11090 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5364 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4580 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5385 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5847 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4070 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7152 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5064 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4682 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3431 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4796 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5011 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5555 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5033 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4139 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3335 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5758 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2535 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4727 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3583 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4904 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3855 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
--rw-r--r--   0 runner    (1001) runner    (1001)    12972 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2701 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_managed_image_package_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2784 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3900 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_model_card.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3127 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_model_task.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4059 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4134 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3697 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_named_double.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2620 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_order.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4197 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3415 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4616 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4108 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3320 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4337 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3678 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2575 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2535 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2567 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2691 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2666 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3126 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3976 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_search_spec.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2654 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_severity.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5062 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3831 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3226 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5586 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3178 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3194 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5016 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3304 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4870 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3288 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5859 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3336 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3390 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4438 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2547 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3108 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_str_list.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3289 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2741 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3134 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3854 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4448 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_table_column.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2768 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5133 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2718 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9660 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3423 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4811 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2869 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2652 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3911 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2698 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_token_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3172 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_toxicity_threat_category.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5196 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3289 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3481 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3327 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3255 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3425 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3289 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_schedule_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2591 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_upgrade_status_for_agent_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2567 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2523 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2531 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_upgrade_agent_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3156 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_upgrade_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4875 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5335 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_role.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3886 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6815 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3106 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_uuid.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7431 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_workspace.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7167 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7715 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2841 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4741 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4096 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/role_users_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4673 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4098 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4401 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4797 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6378 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4295 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_activate_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4319 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_deactivate_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6026 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/schedule_schedule.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6508 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/schedules_schedule_schedule_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6690 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2948 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/schemafilescanning_package_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5053 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4051 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5310 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4156 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2790 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3993 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2803 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4121 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4121 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4136 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7276 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6259 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4371 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4136 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4187 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10280 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6416 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
--rw-r--r--   0 runner    (1001) runner    (1001)    12809 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4278 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5610 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3485 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9333 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4444 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2764 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6759 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3436 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3799 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_category_results_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3538 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3641 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3358 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5680 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5790 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3496 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5835 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5553 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5086 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5530 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3520 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3382 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6503 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
--rw-r--r--   0 runner    (1001) runner    (1001)    16800 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7005 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13296 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5304 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13655 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4663 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
--rw-r--r--   0 runner    (1001) runner    (1001)    19373 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11743 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4077 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3410 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/user_private_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2634 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/user_role.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7844 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/user_user_detail.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3815 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4140 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4196 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8329 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4326 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13843 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11044 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10263 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4396 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8198 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8401 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5364 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5380 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body1.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4825 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/validate_request_input.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3641 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/validate_request_output.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5905 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5093 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5189 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4338 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4533 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13063 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/rest.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5257 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/test_batch.py
--rw-r--r--   0 runner    (1001) runner    (1001)    17414 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/rime_sdk/test_run.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-10 21:01:22.496005 rime_sdk-2.8.0rc4/rime_sdk.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)     1275 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)    40275 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       80 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) runner    (1001)      161 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        9 2024-04-10 21:01:22.000000 rime_sdk-2.8.0rc4/rime_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-04-10 21:01:22.520005 rime_sdk-2.8.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) runner    (1001)     3903 2024-04-10 21:00:21.000000 rime_sdk-2.8.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 17:21:20.224007 rime_sdk-2.8.0rc6/
+-rw-r--r--   0 runner    (1001) runner    (1001)      566 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/LICENSE
+-rw-r--r--   0 runner    (1001) runner    (1001)     1275 2024-04-18 17:21:20.224007 rime_sdk-2.8.0rc6/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      984 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/README.md
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 17:21:20.196007 rime_sdk-2.8.0rc6/rime_sdk/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1490 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2268 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/authenticator.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    71496 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/client.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    23353 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/continuous_test.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12282 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/data_collector.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      883 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/detection_event.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    25617 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/generative_firewall.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3315 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/generative_model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4892 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/image_builder.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 17:21:20.196007 rime_sdk-2.8.0rc6/rime_sdk/internal/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/internal/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18386 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/internal/config_parser.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1004 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/internal/constants.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      667 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/internal/decorators.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9740 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/internal/file_upload.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1973 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/internal/rest_error_handler.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9361 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/internal/swagger_parser.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2577 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/internal/swagger_utils.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1081 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/internal/test_helpers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2681 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/internal/throttle_queue.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3570 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/internal/utils.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18764 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5042 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/monitor.py
+-rw-r--r--   0 runner    (1001) runner    (1001)   107184 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    38328 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/registry.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4396 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/schedule.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 17:21:20.196007 rime_sdk-2.8.0rc6/rime_sdk/swagger/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 17:21:20.196007 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/
+-rw-r--r--   0 runner    (1001) runner    (1001)    60015 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 17:21:20.200008 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/
+-rw-r--r--   0 runner    (1001) runner    (1001)     2411 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    46640 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5851 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/config_validator_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18207 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    25430 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/data_collector_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11733 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/detection_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    23108 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13964 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    27750 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/file_upload_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    24169 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/firewall_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    23787 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/firewall_instance_manager_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    22695 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    15676 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/generative_model_testing_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    28916 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/image_registry_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    27170 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/integration_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    27728 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/job_reader_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    21865 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18441 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/model_testing_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    35026 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    19932 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    74338 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/project_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    57883 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/registry_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    77856 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/results_reader_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4167 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/rime_info_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18249 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/schedule_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    40655 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/user_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    25780 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/validation_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    46472 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    25179 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8845 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 17:21:20.224007 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/
+-rw-r--r--   0 runner    (1001) runner    (1001)    57505 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4210 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4369 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body1.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3366 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/apigenerativefirewall_standard_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4328 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6669 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5483 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5103 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/config_generation_category_config_generation_service_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3706 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/config_generation_profiling_config_generation_service_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3725 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/config_generation_test_suite_config_generation_service_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3435 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8968 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3552 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4503 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3582 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2551 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6687 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    17329 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/crossplanetask_cross_plane_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3362 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8011 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4630 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2674 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2695 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7390 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4396 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3292 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6273 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13500 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8080 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4925 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5748 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2705 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5806 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    14085 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8545 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3410 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    15539 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4273 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2728 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_event_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2587 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4205 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_resolution.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7745 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2744 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2719 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2670 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4176 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10779 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10808 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_file_security_report.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7556 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_package_url.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7459 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3304 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata_license.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3285 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/fileserver_check_object_exists_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/fileserver_delete_object_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3294 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/fileserver_get_read_object_presigned_link_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3310 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/fileserver_get_upload_object_presigned_link_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3232 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/fileserver_list_objects_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9982 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5075 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3149 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10070 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5158 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6961 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewallinstance_firewall_instance_firewall_instance_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2822 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/flagged_substring_request_body_component.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4455 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generative_testing_result_example.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4502 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3679 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5387 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_custom_pii_entity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4675 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_denial_of_service_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2722 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6459 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2844 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5781 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3291 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2896 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_tokenizer.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6773 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_flagged_substring.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3517 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_effective_config_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3686 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_instance_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11464 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_individual_rules_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4144 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3934 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3740 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_list_firewall_instances_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8681 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_off_topic_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4848 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4877 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3752 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_entity_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3712 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3487 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_v2_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11874 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_output.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2808 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_sensitivity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3447 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_detection_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5128 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_unknown_external_source_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3869 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_update_firewall_instance_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5046 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7846 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13957 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3518 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result_standard_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2667 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_request_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5869 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4012 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_objective_sub_category.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9383 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3408 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4422 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4103 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2821 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2770 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3403 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3206 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2808 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4550 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5064 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4141 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/job_data_generative_model_test.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3915 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/job_data_scan.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4710 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4752 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/language_detection_details_language_substring.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4794 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4426 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4187 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_file_scan_results_request_file_scan_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4033 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6007 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5102 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5050 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4570 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3633 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6549 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4842 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4373 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3722 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5728 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5076 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3993 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4508 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2674 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13223 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/model_model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3523 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4142 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2745 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2515 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6262 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4125 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3518 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4963 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12705 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2665 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4511 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2667 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3520 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_transform.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2728 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4020 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5602 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3275 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9399 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_notification.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2774 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2644 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_object_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3594 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4781 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6823 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/pii_detection_details_flagged_entity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4341 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4384 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_activate_schedule_for_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2563 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11026 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3279 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2607 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_deactivate_schedule_for_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2547 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3288 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3190 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4530 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9270 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10554 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12754 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5306 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5738 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3739 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_owner_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    19393 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2693 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_project_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5013 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_project_with_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2579 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4180 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_schedule_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3279 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2571 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4380 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4765 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2715 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/protobuf_any.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2574 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6648 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_connection_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3375 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4050 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4143 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6599 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    20609 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_params.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2624 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3454 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4688 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_generative_language_model_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5621 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4998 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4224 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_metadata.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3453 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3654 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_open_ai_chat_completion_model_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4161 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_pred_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5645 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2728 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13267 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3218 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5797 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/repo_metadata_reputation.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5037 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2753 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2559 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8702 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5337 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent_desired_state.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2745 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8524 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2775 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_attack_objective.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2519 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6159 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13366 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2860 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_config_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4337 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3505 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3389 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4997 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6566 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4077 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6407 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3976 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3303 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3478 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3486 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7059 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3324 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6750 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3842 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3407 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3481 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4086 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3371 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7230 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3177 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5393 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_schedule_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3324 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_schedule_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5936 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3212 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7061 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3352 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2559 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2535 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2539 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2551 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3371 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2559 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2539 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_schedule_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2567 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5159 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_detailed_upgrade_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2563 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4600 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6332 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6606 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3344 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3130 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_float_list.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3469 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_generative_model_test_progress.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3160 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3462 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3357 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4523 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6063 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3231 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4115 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3631 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3396 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3501 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_file_scan_result_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3265 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3181 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3457 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3122 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3266 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3394 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3365 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3303 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5967 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6275 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3208 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8929 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3381 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3406 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3288 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8541 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4079 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_schedule_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3292 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8955 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_time_series_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4877 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_upgrade_for_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3110 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3147 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4256 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4226 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4316 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3284 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2519 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4368 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3108 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_int_list.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4063 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6446 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_data.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    14784 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2865 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2617 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_view.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2611 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_language.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2904 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2770 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5439 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2672 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4968 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4995 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3283 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4835 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11090 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5364 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4580 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5385 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5847 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4070 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7152 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5064 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4682 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3431 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4796 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5011 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5555 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5033 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4139 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3335 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5758 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2535 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4727 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3583 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4904 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3855 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12972 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2701 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image_package_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2784 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3900 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_card.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3127 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_task.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4059 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4134 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3697 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_named_double.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2620 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_order.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4197 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3415 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4616 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4108 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3320 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4337 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3678 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2575 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2535 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2567 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2691 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2666 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3126 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3976 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_search_spec.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2654 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_severity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5062 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3831 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3226 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5586 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3178 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3194 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5016 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3304 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4870 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3288 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5859 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3336 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3390 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4438 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2547 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3108 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_str_list.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3289 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2741 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3134 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3854 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4448 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_table_column.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2768 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5133 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2718 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9660 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3423 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4811 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2869 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2652 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3911 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2698 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_token_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3172 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_toxicity_threat_category.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5196 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3289 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3481 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3327 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3255 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3425 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3289 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_schedule_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2591 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_upgrade_status_for_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2567 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2523 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2531 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_upgrade_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3156 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_upgrade_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4875 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5335 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_role.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3886 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6815 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3106 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_uuid.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7431 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_workspace.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7167 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7715 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2841 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4741 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4096 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/role_users_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4673 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3900 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rule_output_rule_evaluation_metadata.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3469 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rule_output_rule_evaluation_metadata_model_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4098 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4401 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4797 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6378 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4295 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_activate_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4319 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_deactivate_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6026 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schedule_schedule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6508 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schedules_schedule_schedule_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6690 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2948 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemafilescanning_package_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5053 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4051 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5310 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6171 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemaregistry_model_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4156 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2790 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3993 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2803 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4121 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4121 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4136 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7276 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6259 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4371 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4136 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4187 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10280 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6416 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12809 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4278 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5610 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3485 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9333 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4444 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2764 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6759 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3436 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3799 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_category_results_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3538 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3641 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3358 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5680 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5790 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3496 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5835 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5553 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5086 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5530 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3520 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3382 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6503 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    16800 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7005 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13296 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5304 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13655 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4663 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    19373 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11743 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4077 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3410 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/user_private_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2634 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/user_role.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7844 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/user_user_detail.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3815 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4140 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4196 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8329 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4326 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13843 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11044 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10263 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4396 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8198 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8401 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5364 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5380 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body1.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4825 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validate_request_input.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3641 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validate_request_output.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10037 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validate_response_processed_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5992 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validate_response_product_metadata.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5905 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5093 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5189 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4338 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4533 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13063 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/rest.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5257 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/test_batch.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    17414 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/test_run.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 17:21:20.196007 rime_sdk-2.8.0rc6/rime_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1275 2024-04-18 17:21:20.000000 rime_sdk-2.8.0rc6/rime_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)    40697 2024-04-18 17:21:20.000000 rime_sdk-2.8.0rc6/rime_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-04-18 17:21:20.000000 rime_sdk-2.8.0rc6/rime_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       80 2024-04-18 17:21:20.000000 rime_sdk-2.8.0rc6/rime_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)      161 2024-04-18 17:21:20.000000 rime_sdk-2.8.0rc6/rime_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        9 2024-04-18 17:21:20.000000 rime_sdk-2.8.0rc6/rime_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-04-18 17:21:20.224007 rime_sdk-2.8.0rc6/setup.cfg
+-rw-r--r--   0 runner    (1001) runner    (1001)     3903 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/setup.py
```

### Comparing `rime_sdk-2.8.0rc4/LICENSE` & `rime_sdk-2.8.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/PKG-INFO` & `rime_sdk-2.8.0rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime_sdk
-Version: 2.8.0rc4
+Version: 2.8.0rc6
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.8.0rc4/README.md` & `rime_sdk-2.8.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/__init__.py` & `rime_sdk-2.8.0rc6/rime_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/authenticator.py` & `rime_sdk-2.8.0rc6/rime_sdk/authenticator.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/client.py` & `rime_sdk-2.8.0rc6/rime_sdk/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1492,17 +1492,17 @@
             req.run_time_info.custom_image = RuntimeinfoCustomImageType(
                 managed_image_name=rime_managed_image
             )
 
         Client._throttler.throttle(
             throttling_msg="Your request is throttled to limit # of file scans."
         )
-        api = swagger_client.FileScanningApi(self._api_client)
+        api = swagger_client.ModelTestingApi(self._api_client)
         with RESTErrorHandler():
-            response = api.file_scanning_start_file_scan(body=req)
+            response = api.model_testing_start_file_scan(body=req)
             job: RimeJobMetadata = response.job
             return FileScanJob(self._api_client, job.job_id)
 
     def get_file_scan_result(
         self,
         file_scan_id: str,
     ) -> dict:
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/continuous_test.py` & `rime_sdk-2.8.0rc6/rime_sdk/continuous_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/data_collector.py` & `rime_sdk-2.8.0rc6/rime_sdk/data_collector.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/detection_event.py` & `rime_sdk-2.8.0rc6/rime_sdk/detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/generative_firewall.py` & `rime_sdk-2.8.0rc6/rime_sdk/generative_firewall.py`

 * *Files 1% similar despite different names*

```diff
@@ -477,18 +477,26 @@
         self._api_client = ApiClient(configuration)
         # Prevent race condition in pool.close() triggered by swagger generated code
         atexit.register(self._api_client.pool.close)
         # Sets the timeout and hardcoded retries parameter for the api client.
         self._api_client.rest_client.pool_manager.connection_pool_kw[
             "timeout"
         ] = channel_timeout
+        # Configure the retries against the firewall cluster.
+        # Due to NGINX refresh issues breaking connections, we want to allow
+        # retries on `read` errors on all idempotent HTTP methods.
+        # The current implementation of PATCH with gRPC-gateway proto field
+        # masks is idempotent, so it can be safely retried.
+        # Note: the Retry will only retry on read errors if the HTTP method
+        # belongs to one of the configured `allowed_methods`.
         self._api_client.rest_client.pool_manager.connection_pool_kw["retries"] = Retry(
             read=3,
             status=3,
             status_forcelist=RETRY_HTTP_STATUS,
+            allowed_methods=Retry.DEFAULT_ALLOWED_METHODS.union(["PATCH"]),
             backoff_factor=0.5,
         )
         self._instance_manager_client = FirewallInstanceManagerApi(self._api_client)
 
     def login(self, email: str, system_account: bool = False) -> None:
         """Login to obtain an auth token.
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/generative_model.py` & `rime_sdk-2.8.0rc6/rime_sdk/generative_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from rime_sdk.internal.rest_error_handler import RESTErrorHandler
 from rime_sdk.job import GenerativeModelTestJob
 from rime_sdk.swagger.swagger_client import (
     ApiClient,
     GenerativeModelTestingApi,
     GenerativetestingGenerativeTestingResult,
     GenerativetestingGetGenerativeModelTestResultsResponse,
-    GenerativetestingModelConnectionSpec,
     GenerativetestingStartGenerativeModelTestRequest,
     GenerativetestingStartGenerativeModelTestResponse,
 )
 
 
 class GenerativeModel:
     """The interface to the Generative Model Testing API."""
@@ -40,20 +39,18 @@
             endpoint_payload_template: The endpoint payload template to use.
             response_json_path: The response JSON path to use.
 
         Returns:
             GenerativeModelTestJob: The Generative Model Test Job.
         """
         request = GenerativetestingStartGenerativeModelTestRequest(
-            connection_spec=GenerativetestingModelConnectionSpec(
-                url=url,
-                http_headers=http_headers,
-                endpoint_payload_template=endpoint_payload_template,
-                response_json_path=response_json_path,
-            )
+            url=url,
+            http_headers=http_headers,
+            endpoint_payload_template=endpoint_payload_template,
+            response_json_path=response_json_path,
         )
         with RESTErrorHandler():
             res: GenerativetestingStartGenerativeModelTestResponse = (
                 GenerativeModelTestingApi(
                     self._api_client
                 ).generative_model_testing_start_generative_model_test(body=request)
             )
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/image_builder.py` & `rime_sdk-2.8.0rc6/rime_sdk/image_builder.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/internal/config_parser.py` & `rime_sdk-2.8.0rc6/rime_sdk/internal/config_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     RegistryDataCollectorInfo,
     RegistryDataFileInfo,
     RegistryDataInfo,
     RegistryDataLoadingInfo,
     RegistryDataParams,
     RegistryHuggingFaceDataInfo,
     RegistryHuggingFaceModelInfo,
-    RegistryModelInfo,
     RegistryModelPathInfo,
     RegistryPredictionParams,
     RegistryPredInfo,
     RimeUUID,
+    SchemaregistryModelInfo,
 )
 
 DEFAULT_DO_SAMPLING = True
 CONNECTION_INFO_TYPE_SWAGGER = Union[
     RegistryDataFileInfo,
     RegistryDataLoadingInfo,
     RegistryDataCollectorInfo,
@@ -328,54 +328,54 @@
     return RegistryDataInfo(
         data_params=data_params,
         connection_info=connection_info,
     )
 
 
 @validate_types
-def convert_model_info_to_swagger(model_config: dict) -> RegistryModelInfo:
+def convert_model_info_to_swagger(model_config: dict) -> SchemaregistryModelInfo:
     """Convert a dictionary to model info swagger message."""
     _config = deepcopy(model_config)
-    valid_model_infos = list(RegistryModelInfo.swagger_types)
+    valid_model_infos = list(SchemaregistryModelInfo.swagger_types)
     if len(_config) != 1:
         raise ValueError(
             "Must specify exactly one valid model_info type in config. "
             f"Valid model_info types are: {valid_model_infos}. "
             f"Got: {list(_config)}."
         )
     model_type, model_info = next(iter(_config.items()))
     if not isinstance(model_info, dict):
         raise ValueError(
             f"model_info must be a dictionary. Got: {type(model_info)}."
             f"\nFull config: {model_config}"
         )
     try:
         if model_type == "model_path":
-            model_info_swagger = RegistryModelInfo(
+            model_info_swagger = SchemaregistryModelInfo(
                 model_path=RegistryModelPathInfo(path=model_info.pop("path"))
             )
         elif model_type == "hugging_face":
             model_uri = model_info.pop("model_uri")
             config_d = model_info.pop("kwargs", {})
             if isinstance(config_d, dict):
                 config_str = json.dumps(config_d)
             elif isinstance(config_d, str):
                 config_str = config_d
             else:
                 raise ValueError(
                     f"Invalid type for `kwargs` in hugging_face model_info."
                     f" Expected `dict` or json `str`. Got: {type(config_d)}"
                 )
-            model_info_swagger = RegistryModelInfo(
+            model_info_swagger = SchemaregistryModelInfo(
                 hugging_face=RegistryHuggingFaceModelInfo(
                     model_uri=model_uri, kwargs=config_str
                 )
             )
         elif model_type == "generative_language_model":
-            model_info_swagger = RegistryModelInfo(
+            model_info_swagger = SchemaregistryModelInfo(
                 generative_language_model=RegistryGenerativeLanguageModelInfo(
                     model_path=model_info.pop("model_path"),
                     system_prompt=model_info.pop("system_prompt", ""),
                 )
             )
         else:
             raise ValueError(
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/internal/constants.py` & `rime_sdk-2.8.0rc6/rime_sdk/internal/constants.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/internal/decorators.py` & `rime_sdk-2.8.0rc6/rime_sdk/internal/decorators.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/internal/file_upload.py` & `rime_sdk-2.8.0rc6/rime_sdk/internal/file_upload.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/internal/rest_error_handler.py` & `rime_sdk-2.8.0rc6/rime_sdk/internal/rest_error_handler.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/internal/swagger_parser.py` & `rime_sdk-2.8.0rc6/rime_sdk/internal/swagger_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/internal/swagger_utils.py` & `rime_sdk-2.8.0rc6/rime_sdk/internal/swagger_utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/internal/test_helpers.py` & `rime_sdk-2.8.0rc6/rime_sdk/internal/test_helpers.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/internal/throttle_queue.py` & `rime_sdk-2.8.0rc6/rime_sdk/internal/throttle_queue.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/internal/utils.py` & `rime_sdk-2.8.0rc6/rime_sdk/internal/utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/job.py` & `rime_sdk-2.8.0rc6/rime_sdk/job.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/monitor.py` & `rime_sdk-2.8.0rc6/rime_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/project.py` & `rime_sdk-2.8.0rc6/rime_sdk/project.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/registry.py` & `rime_sdk-2.8.0rc6/rime_sdk/registry.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/schedule.py` & `rime_sdk-2.8.0rc6/rime_sdk/schedule.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/__init__.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 from rime_sdk.swagger.swagger_client.api.workspace_service_api import WorkspaceServiceApi
 # import ApiClient
 from rime_sdk.swagger.swagger_client.api_client import ApiClient
 from rime_sdk.swagger.swagger_client.configuration import Configuration
 # import models into sdk package
 from rime_sdk.swagger.swagger_client.models.agent_id_uuid_upgrade_body import AgentIdUuidUpgradeBody
 from rime_sdk.swagger.swagger_client.models.agent_id_uuid_upgrade_body1 import AgentIdUuidUpgradeBody1
+from rime_sdk.swagger.swagger_client.models.apigenerativefirewall_standard_info import ApigenerativefirewallStandardInfo
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_category_test_identifier import ArtifactIdentifierCategoryTestIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_subset_test_metric_identifier import ArtifactIdentifierSubsetTestMetricIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_test_case_metric_identifier import ArtifactIdentifierTestCaseMetricIdentifier
 from rime_sdk.swagger.swagger_client.models.config_generation_category_config_generation_service_response import ConfigGenerationCategoryConfigGenerationServiceResponse
 from rime_sdk.swagger.swagger_client.models.config_generation_profiling_config_generation_service_response import ConfigGenerationProfilingConfigGenerationServiceResponse
 from rime_sdk.swagger.swagger_client.models.config_generation_test_suite_config_generation_service_response import ConfigGenerationTestSuiteConfigGenerationServiceResponse
 from rime_sdk.swagger.swagger_client.models.configvalidator_config_type_body import ConfigvalidatorConfigTypeBody
@@ -104,15 +105,14 @@
 from rime_sdk.swagger.swagger_client.models.firewall_firewall_firewall_id_uuid_body import FirewallFirewallFirewallIdUuidBody
 from rime_sdk.swagger.swagger_client.models.firewall_latest_run_info import FirewallLatestRunInfo
 from rime_sdk.swagger.swagger_client.models.firewall_scheduled_ct_info import FirewallScheduledCTInfo
 from rime_sdk.swagger.swagger_client.models.firewall_test_category_severity import FirewallTestCategorySeverity
 from rime_sdk.swagger.swagger_client.models.firewallinstance_firewall_instance_firewall_instance_id_uuid_body import FirewallinstanceFirewallInstanceFirewallInstanceIdUuidBody
 from rime_sdk.swagger.swagger_client.models.flagged_substring_request_body_component import FlaggedSubstringRequestBodyComponent
 from rime_sdk.swagger.swagger_client.models.generative_testing_result_example import GenerativeTestingResultExample
-from rime_sdk.swagger.swagger_client.models.generative_testing_result_standard_info import GenerativeTestingResultStandardInfo
 from rime_sdk.swagger.swagger_client.models.generativefirewall_create_firewall_instance_request import GenerativefirewallCreateFirewallInstanceRequest
 from rime_sdk.swagger.swagger_client.models.generativefirewall_create_firewall_instance_response import GenerativefirewallCreateFirewallInstanceResponse
 from rime_sdk.swagger.swagger_client.models.generativefirewall_custom_pii_entity import GenerativefirewallCustomPiiEntity
 from rime_sdk.swagger.swagger_client.models.generativefirewall_denial_of_service_rule_config import GenerativefirewallDenialOfServiceRuleConfig
 from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_action import GenerativefirewallFirewallAction
 from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_instance_info import GenerativefirewallFirewallInstanceInfo
 from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_instance_status import GenerativefirewallFirewallInstanceStatus
@@ -136,17 +136,17 @@
 from rime_sdk.swagger.swagger_client.models.generativefirewall_rule_sensitivity import GenerativefirewallRuleSensitivity
 from rime_sdk.swagger.swagger_client.models.generativefirewall_toxicity_detection_details import GenerativefirewallToxicityDetectionDetails
 from rime_sdk.swagger.swagger_client.models.generativefirewall_unknown_external_source_rule_config import GenerativefirewallUnknownExternalSourceRuleConfig
 from rime_sdk.swagger.swagger_client.models.generativefirewall_update_firewall_instance_response import GenerativefirewallUpdateFirewallInstanceResponse
 from rime_sdk.swagger.swagger_client.models.generativefirewall_validate_request import GenerativefirewallValidateRequest
 from rime_sdk.swagger.swagger_client.models.generativefirewall_validate_response import GenerativefirewallValidateResponse
 from rime_sdk.swagger.swagger_client.models.generativetesting_generative_testing_result import GenerativetestingGenerativeTestingResult
+from rime_sdk.swagger.swagger_client.models.generativetesting_generative_testing_result_standard_info import GenerativetestingGenerativeTestingResultStandardInfo
 from rime_sdk.swagger.swagger_client.models.generativetesting_get_generative_model_test_results_request_query import GenerativetestingGetGenerativeModelTestResultsRequestQuery
 from rime_sdk.swagger.swagger_client.models.generativetesting_get_generative_model_test_results_response import GenerativetestingGetGenerativeModelTestResultsResponse
-from rime_sdk.swagger.swagger_client.models.generativetesting_model_connection_spec import GenerativetestingModelConnectionSpec
 from rime_sdk.swagger.swagger_client.models.generativetesting_objective_sub_category import GenerativetestingObjectiveSubCategory
 from rime_sdk.swagger.swagger_client.models.generativetesting_start_generative_model_test_request import GenerativetestingStartGenerativeModelTestRequest
 from rime_sdk.swagger.swagger_client.models.generativetesting_start_generative_model_test_response import GenerativetestingStartGenerativeModelTestResponse
 from rime_sdk.swagger.swagger_client.models.googlerpc_status import GooglerpcStatus
 from rime_sdk.swagger.swagger_client.models.heartbeat_agent_id_uuid_body import HeartbeatAgentIdUuidBody
 from rime_sdk.swagger.swagger_client.models.image_reference_reference_type import ImageReferenceReferenceType
 from rime_sdk.swagger.swagger_client.models.integration_integration_level import IntegrationIntegrationLevel
@@ -238,15 +238,14 @@
 from rime_sdk.swagger.swagger_client.models.registry_data_params import RegistryDataParams
 from rime_sdk.swagger.swagger_client.models.registry_data_type import RegistryDataType
 from rime_sdk.swagger.swagger_client.models.registry_databricks_info import RegistryDatabricksInfo
 from rime_sdk.swagger.swagger_client.models.registry_generative_language_model_info import RegistryGenerativeLanguageModelInfo
 from rime_sdk.swagger.swagger_client.models.registry_hugging_face_data_info import RegistryHuggingFaceDataInfo
 from rime_sdk.swagger.swagger_client.models.registry_hugging_face_model_info import RegistryHuggingFaceModelInfo
 from rime_sdk.swagger.swagger_client.models.registry_metadata import RegistryMetadata
-from rime_sdk.swagger.swagger_client.models.registry_model_info import RegistryModelInfo
 from rime_sdk.swagger.swagger_client.models.registry_model_path_info import RegistryModelPathInfo
 from rime_sdk.swagger.swagger_client.models.registry_open_ai_chat_completion_model_info import RegistryOpenAIChatCompletionModelInfo
 from rime_sdk.swagger.swagger_client.models.registry_pred_info import RegistryPredInfo
 from rime_sdk.swagger.swagger_client.models.registry_prediction_params import RegistryPredictionParams
 from rime_sdk.swagger.swagger_client.models.registry_validity_status import RegistryValidityStatus
 from rime_sdk.swagger.swagger_client.models.registryprediction_prediction import RegistrypredictionPrediction
 from rime_sdk.swagger.swagger_client.models.rename_test_run_id_body import RenameTestRunIdBody
@@ -304,14 +303,15 @@
 from rime_sdk.swagger.swagger_client.models.rime_detailed_upgrade_status import RimeDetailedUpgradeStatus
 from rime_sdk.swagger.swagger_client.models.rime_ensure_image_existence_response import RimeEnsureImageExistenceResponse
 from rime_sdk.swagger.swagger_client.models.rime_failing_row import RimeFailingRow
 from rime_sdk.swagger.swagger_client.models.rime_failing_rows_result import RimeFailingRowsResult
 from rime_sdk.swagger.swagger_client.models.rime_feature_flags import RimeFeatureFlags
 from rime_sdk.swagger.swagger_client.models.rime_feature_type import RimeFeatureType
 from rime_sdk.swagger.swagger_client.models.rime_float_list import RimeFloatList
+from rime_sdk.swagger.swagger_client.models.rime_generative_model_test_progress import RimeGenerativeModelTestProgress
 from rime_sdk.swagger.swagger_client.models.rime_get_agent_response import RimeGetAgentResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_customer_managed_key_response import RimeGetCustomerManagedKeyResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_datapoints_response import RimeGetDatapointsResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_dataset_file_upload_url_request import RimeGetDatasetFileUploadURLRequest
 from rime_sdk.swagger.swagger_client.models.rime_get_dataset_file_upload_url_response import RimeGetDatasetFileUploadURLResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_dataset_response import RimeGetDatasetResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_enabled_feature_response import RimeGetEnabledFeatureResponse
@@ -465,27 +465,30 @@
 from rime_sdk.swagger.swagger_client.models.rime_workspace import RimeWorkspace
 from rime_sdk.swagger.swagger_client.models.rime_workspace_write_mask import RimeWorkspaceWriteMask
 from rime_sdk.swagger.swagger_client.models.rischemaintegration_integration import RischemaintegrationIntegration
 from rime_sdk.swagger.swagger_client.models.riskscore_risk_category_type import RiskscoreRiskCategoryType
 from rime_sdk.swagger.swagger_client.models.riskscore_risk_score import RiskscoreRiskScore
 from rime_sdk.swagger.swagger_client.models.role_users_body import RoleUsersBody
 from rime_sdk.swagger.swagger_client.models.role_workspace_body import RoleWorkspaceBody
+from rime_sdk.swagger.swagger_client.models.rule_output_rule_evaluation_metadata import RuleOutputRuleEvaluationMetadata
+from rime_sdk.swagger.swagger_client.models.rule_output_rule_evaluation_metadata_model_info import RuleOutputRuleEvaluationMetadataModelInfo
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_custom_image import RuntimeinfoCustomImage
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_custom_image_type import RuntimeinfoCustomImageType
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_resource_request import RuntimeinfoResourceRequest
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_run_time_info import RuntimeinfoRunTimeInfo
 from rime_sdk.swagger.swagger_client.models.schedule_id_uuid_activate_body import ScheduleIdUuidActivateBody
 from rime_sdk.swagger.swagger_client.models.schedule_id_uuid_deactivate_body import ScheduleIdUuidDeactivateBody
 from rime_sdk.swagger.swagger_client.models.schedule_schedule import ScheduleSchedule
 from rime_sdk.swagger.swagger_client.models.schedules_schedule_schedule_id_uuid_body import SchedulesScheduleScheduleIdUuidBody
 from rime_sdk.swagger.swagger_client.models.schemadatacollector_prediction import SchemadatacollectorPrediction
 from rime_sdk.swagger.swagger_client.models.schemafilescanning_package_type import SchemafilescanningPackageType
 from rime_sdk.swagger.swagger_client.models.schemaintegration_integration_variable import SchemaintegrationIntegrationVariable
 from rime_sdk.swagger.swagger_client.models.schemamonitor_config import SchemamonitorConfig
 from rime_sdk.swagger.swagger_client.models.schemanotification_config import SchemanotificationConfig
+from rime_sdk.swagger.swagger_client.models.schemaregistry_model_info import SchemaregistryModelInfo
 from rime_sdk.swagger.swagger_client.models.security_event_details_flagged_datapoint import SecurityEventDetailsFlaggedDatapoint
 from rime_sdk.swagger.swagger_client.models.security_event_details_security_event_type import SecurityEventDetailsSecurityEventType
 from rime_sdk.swagger.swagger_client.models.statedb_archived_job_logs import StatedbArchivedJobLogs
 from rime_sdk.swagger.swagger_client.models.statedb_job_status import StatedbJobStatus
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_datapoints_response import StreamResultOfRimeGetDatapointsResponse
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_latest_logs_response import StreamResultOfRimeGetLatestLogsResponse
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_predictions_response import StreamResultOfRimeGetPredictionsResponse
@@ -542,12 +545,14 @@
 from rime_sdk.swagger.swagger_client.models.v1projectsproject_id_uuidroleusersuser_user_id_uuid_user import V1projectsprojectIdUuidroleusersuserUserIdUuidUser
 from rime_sdk.swagger.swagger_client.models.v1usersuser_id_uuid_user import V1usersuserIdUuidUser
 from rime_sdk.swagger.swagger_client.models.v1workspaceworkspace_workspace_id_uuid_workspace import V1workspaceworkspaceWorkspaceIdUuidWorkspace
 from rime_sdk.swagger.swagger_client.models.validate_firewall_instance_id_uuid_body import ValidateFirewallInstanceIdUuidBody
 from rime_sdk.swagger.swagger_client.models.validate_firewall_instance_id_uuid_body1 import ValidateFirewallInstanceIdUuidBody1
 from rime_sdk.swagger.swagger_client.models.validate_request_input import ValidateRequestInput
 from rime_sdk.swagger.swagger_client.models.validate_request_output import ValidateRequestOutput
+from rime_sdk.swagger.swagger_client.models.validate_response_processed_request import ValidateResponseProcessedRequest
+from rime_sdk.swagger.swagger_client.models.validate_response_product_metadata import ValidateResponseProductMetadata
 from rime_sdk.swagger.swagger_client.models.validation_validate_dataset_response import ValidationValidateDatasetResponse
 from rime_sdk.swagger.swagger_client.models.validation_validate_model_response import ValidationValidateModelResponse
 from rime_sdk.swagger.swagger_client.models.validation_validate_predictions_response import ValidationValidatePredictionsResponse
 from rime_sdk.swagger.swagger_client.models.workspace_id_uuid_users_body import WorkspaceIdUuidUsersBody
 from rime_sdk.swagger.swagger_client.models.workspace_workspace_workspace_id_uuid_body import WorkspaceWorkspaceWorkspaceIdUuidBody
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/__init__.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/agent_manager_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/agent_manager_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/config_validator_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/config_validator_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/data_collector_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/data_collector_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/detection_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/detection_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/feature_flag_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/feature_flag_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/file_scanning_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/file_scanning_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -320,106 +320,7 @@
             response_type='RimeListFileScanResultsResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
-
-    def file_scanning_start_file_scan(self, body, **kwargs):  # noqa: E501
-        """StartFileScan  # noqa: E501
-
-        Starts a File Scan for the specified model.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.file_scanning_start_file_scan(body, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param RimeStartFileScanRequest body: (required)
-        :return: RimeStartFileScanResponse
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.file_scanning_start_file_scan_with_http_info(body, **kwargs)  # noqa: E501
-        else:
-            (data) = self.file_scanning_start_file_scan_with_http_info(body, **kwargs)  # noqa: E501
-            return data
-
-    def file_scanning_start_file_scan_with_http_info(self, body, **kwargs):  # noqa: E501
-        """StartFileScan  # noqa: E501
-
-        Starts a File Scan for the specified model.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.file_scanning_start_file_scan_with_http_info(body, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param RimeStartFileScanRequest body: (required)
-        :return: RimeStartFileScanResponse
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        all_params = ['body']  # noqa: E501
-        all_params.append('async_req')
-        all_params.append('_return_http_data_only')
-        all_params.append('_preload_content')
-        all_params.append('_request_timeout')
-
-        params = locals()
-        for key, val in six.iteritems(params['kwargs']):
-            if key not in all_params:
-                raise TypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method file_scanning_start_file_scan" % key
-                )
-            params[key] = val
-        del params['kwargs']
-        # verify the required parameter 'body' is set
-        if ('body' not in params or
-                params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `file_scanning_start_file_scan`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        if 'body' in params:
-            body_params = params['body']
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['X-Firewall-Api-Key', 'X-Firewall-Auth-Token', 'rime-api-key']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/v1-beta/file-scans', 'POST',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='RimeStartFileScanResponse',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=params.get('async_req'),
-            _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
-            _request_timeout=params.get('_request_timeout'),
-            collection_formats=collection_formats)
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/file_upload_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/file_upload_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/firewall_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/firewall_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/firewall_instance_manager_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/firewall_instance_manager_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/firewall_service_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/firewall_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/generative_model_testing_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/generative_model_testing_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,49 +28,49 @@
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def generative_model_testing_get_generative_model_test_results(self, **kwargs):  # noqa: E501
+    def generative_model_testing_get_generative_model_test_results(self, job_id_uuid, **kwargs):  # noqa: E501
         """GetGenerativeModelTestResults  # noqa: E501
 
         Retrieve the results of a generative model testing for a successful job. This is a paginated API.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.generative_model_testing_get_generative_model_test_results(async_req=True)
+        >>> thread = api.generative_model_testing_get_generative_model_test_results(job_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str job_id_uuid: Unique object ID.
+        :param str job_id_uuid: Unique object ID. (required)
         :param str page_token: A token representing one page from the list returned by a GetGenerativeModelTestResults API. The GetGenerativeModelTestResults API returns a page_token when there is more than one page of results.
         :param str page_size: The maximum number of objects to return in a single page.  Maximum page size is 1000.
         :return: GenerativetestingGetGenerativeModelTestResultsResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.generative_model_testing_get_generative_model_test_results_with_http_info(**kwargs)  # noqa: E501
+            return self.generative_model_testing_get_generative_model_test_results_with_http_info(job_id_uuid, **kwargs)  # noqa: E501
         else:
-            (data) = self.generative_model_testing_get_generative_model_test_results_with_http_info(**kwargs)  # noqa: E501
+            (data) = self.generative_model_testing_get_generative_model_test_results_with_http_info(job_id_uuid, **kwargs)  # noqa: E501
             return data
 
-    def generative_model_testing_get_generative_model_test_results_with_http_info(self, **kwargs):  # noqa: E501
+    def generative_model_testing_get_generative_model_test_results_with_http_info(self, job_id_uuid, **kwargs):  # noqa: E501
         """GetGenerativeModelTestResults  # noqa: E501
 
         Retrieve the results of a generative model testing for a successful job. This is a paginated API.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.generative_model_testing_get_generative_model_test_results_with_http_info(async_req=True)
+        >>> thread = api.generative_model_testing_get_generative_model_test_results_with_http_info(job_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str job_id_uuid: Unique object ID.
+        :param str job_id_uuid: Unique object ID. (required)
         :param str page_token: A token representing one page from the list returned by a GetGenerativeModelTestResults API. The GetGenerativeModelTestResults API returns a page_token when there is more than one page of results.
         :param str page_size: The maximum number of objects to return in a single page.  Maximum page size is 1000.
         :return: GenerativetestingGetGenerativeModelTestResultsResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
@@ -85,22 +85,26 @@
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method generative_model_testing_get_generative_model_test_results" % key
                 )
             params[key] = val
         del params['kwargs']
+        # verify the required parameter 'job_id_uuid' is set
+        if ('job_id_uuid' not in params or
+                params['job_id_uuid'] is None):
+            raise ValueError("Missing the required parameter `job_id_uuid` when calling `generative_model_testing_get_generative_model_test_results`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
+        if 'job_id_uuid' in params:
+            path_params['jobId.uuid'] = params['job_id_uuid']  # noqa: E501
 
         query_params = []
-        if 'job_id_uuid' in params:
-            query_params.append(('jobId.uuid', params['job_id_uuid']))  # noqa: E501
         if 'page_token' in params:
             query_params.append(('pageToken', params['page_token']))  # noqa: E501
         if 'page_size' in params:
             query_params.append(('pageSize', params['page_size']))  # noqa: E501
 
         header_params = {}
 
@@ -112,15 +116,15 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['X-Firewall-Api-Key', 'X-Firewall-Auth-Token', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1-beta/generative/testing/result', 'GET',
+            '/v1-beta/generative/testing/{jobId.uuid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='GenerativetestingGetGenerativeModelTestResultsResponse',  # noqa: E501
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/image_registry_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/image_registry_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/integration_service_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/integration_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/job_reader_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/job_reader_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/model_card_service_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/model_card_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/model_testing_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/model_testing_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -230,14 +230,113 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def model_testing_start_file_scan(self, body, **kwargs):  # noqa: E501
+        """StartFileScan  # noqa: E501
+
+        Starts a File Scan for the specified model.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.model_testing_start_file_scan(body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param RimeStartFileScanRequest body: (required)
+        :return: RimeStartFileScanResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.model_testing_start_file_scan_with_http_info(body, **kwargs)  # noqa: E501
+        else:
+            (data) = self.model_testing_start_file_scan_with_http_info(body, **kwargs)  # noqa: E501
+            return data
+
+    def model_testing_start_file_scan_with_http_info(self, body, **kwargs):  # noqa: E501
+        """StartFileScan  # noqa: E501
+
+        Starts a File Scan for the specified model.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.model_testing_start_file_scan_with_http_info(body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param RimeStartFileScanRequest body: (required)
+        :return: RimeStartFileScanResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['body']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method model_testing_start_file_scan" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'body' is set
+        if ('body' not in params or
+                params['body'] is None):
+            raise ValueError("Missing the required parameter `body` when calling `model_testing_start_file_scan`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in params:
+            body_params = params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['X-Firewall-Api-Key', 'X-Firewall-Auth-Token', 'rime-api-key']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/v1-beta/file-scans', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RimeStartFileScanResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def model_testing_start_stress_test(self, body, project_id_uuid, **kwargs):  # noqa: E501
         """StartStressTest  # noqa: E501
 
         Starts a Stress Test and returns a Job object containing metadata for the Test Run.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.model_testing_start_stress_test(body, project_id_uuid, async_req=True)
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/monitor_service_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/monitor_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/notification_setting_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/notification_setting_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/project_service_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/project_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/registry_service_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/registry_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/results_reader_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/results_reader_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/rime_info_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/rime_info_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/schedule_service_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/schedule_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/user_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/validation_service_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/validation_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api/workspace_service_api.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/workspace_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/api_client.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/configuration.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/__init__.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 """
 
 from __future__ import absolute_import
 
 # import models into model package
 from rime_sdk.swagger.swagger_client.models.agent_id_uuid_upgrade_body import AgentIdUuidUpgradeBody
 from rime_sdk.swagger.swagger_client.models.agent_id_uuid_upgrade_body1 import AgentIdUuidUpgradeBody1
+from rime_sdk.swagger.swagger_client.models.apigenerativefirewall_standard_info import ApigenerativefirewallStandardInfo
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_category_test_identifier import ArtifactIdentifierCategoryTestIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_subset_test_metric_identifier import ArtifactIdentifierSubsetTestMetricIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_test_case_metric_identifier import ArtifactIdentifierTestCaseMetricIdentifier
 from rime_sdk.swagger.swagger_client.models.config_generation_category_config_generation_service_response import ConfigGenerationCategoryConfigGenerationServiceResponse
 from rime_sdk.swagger.swagger_client.models.config_generation_profiling_config_generation_service_response import ConfigGenerationProfilingConfigGenerationServiceResponse
 from rime_sdk.swagger.swagger_client.models.config_generation_test_suite_config_generation_service_response import ConfigGenerationTestSuiteConfigGenerationServiceResponse
 from rime_sdk.swagger.swagger_client.models.configvalidator_config_type_body import ConfigvalidatorConfigTypeBody
@@ -72,15 +73,14 @@
 from rime_sdk.swagger.swagger_client.models.firewall_firewall_firewall_id_uuid_body import FirewallFirewallFirewallIdUuidBody
 from rime_sdk.swagger.swagger_client.models.firewall_latest_run_info import FirewallLatestRunInfo
 from rime_sdk.swagger.swagger_client.models.firewall_scheduled_ct_info import FirewallScheduledCTInfo
 from rime_sdk.swagger.swagger_client.models.firewall_test_category_severity import FirewallTestCategorySeverity
 from rime_sdk.swagger.swagger_client.models.firewallinstance_firewall_instance_firewall_instance_id_uuid_body import FirewallinstanceFirewallInstanceFirewallInstanceIdUuidBody
 from rime_sdk.swagger.swagger_client.models.flagged_substring_request_body_component import FlaggedSubstringRequestBodyComponent
 from rime_sdk.swagger.swagger_client.models.generative_testing_result_example import GenerativeTestingResultExample
-from rime_sdk.swagger.swagger_client.models.generative_testing_result_standard_info import GenerativeTestingResultStandardInfo
 from rime_sdk.swagger.swagger_client.models.generativefirewall_create_firewall_instance_request import GenerativefirewallCreateFirewallInstanceRequest
 from rime_sdk.swagger.swagger_client.models.generativefirewall_create_firewall_instance_response import GenerativefirewallCreateFirewallInstanceResponse
 from rime_sdk.swagger.swagger_client.models.generativefirewall_custom_pii_entity import GenerativefirewallCustomPiiEntity
 from rime_sdk.swagger.swagger_client.models.generativefirewall_denial_of_service_rule_config import GenerativefirewallDenialOfServiceRuleConfig
 from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_action import GenerativefirewallFirewallAction
 from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_instance_info import GenerativefirewallFirewallInstanceInfo
 from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_instance_status import GenerativefirewallFirewallInstanceStatus
@@ -104,17 +104,17 @@
 from rime_sdk.swagger.swagger_client.models.generativefirewall_rule_sensitivity import GenerativefirewallRuleSensitivity
 from rime_sdk.swagger.swagger_client.models.generativefirewall_toxicity_detection_details import GenerativefirewallToxicityDetectionDetails
 from rime_sdk.swagger.swagger_client.models.generativefirewall_unknown_external_source_rule_config import GenerativefirewallUnknownExternalSourceRuleConfig
 from rime_sdk.swagger.swagger_client.models.generativefirewall_update_firewall_instance_response import GenerativefirewallUpdateFirewallInstanceResponse
 from rime_sdk.swagger.swagger_client.models.generativefirewall_validate_request import GenerativefirewallValidateRequest
 from rime_sdk.swagger.swagger_client.models.generativefirewall_validate_response import GenerativefirewallValidateResponse
 from rime_sdk.swagger.swagger_client.models.generativetesting_generative_testing_result import GenerativetestingGenerativeTestingResult
+from rime_sdk.swagger.swagger_client.models.generativetesting_generative_testing_result_standard_info import GenerativetestingGenerativeTestingResultStandardInfo
 from rime_sdk.swagger.swagger_client.models.generativetesting_get_generative_model_test_results_request_query import GenerativetestingGetGenerativeModelTestResultsRequestQuery
 from rime_sdk.swagger.swagger_client.models.generativetesting_get_generative_model_test_results_response import GenerativetestingGetGenerativeModelTestResultsResponse
-from rime_sdk.swagger.swagger_client.models.generativetesting_model_connection_spec import GenerativetestingModelConnectionSpec
 from rime_sdk.swagger.swagger_client.models.generativetesting_objective_sub_category import GenerativetestingObjectiveSubCategory
 from rime_sdk.swagger.swagger_client.models.generativetesting_start_generative_model_test_request import GenerativetestingStartGenerativeModelTestRequest
 from rime_sdk.swagger.swagger_client.models.generativetesting_start_generative_model_test_response import GenerativetestingStartGenerativeModelTestResponse
 from rime_sdk.swagger.swagger_client.models.googlerpc_status import GooglerpcStatus
 from rime_sdk.swagger.swagger_client.models.heartbeat_agent_id_uuid_body import HeartbeatAgentIdUuidBody
 from rime_sdk.swagger.swagger_client.models.image_reference_reference_type import ImageReferenceReferenceType
 from rime_sdk.swagger.swagger_client.models.integration_integration_level import IntegrationIntegrationLevel
@@ -206,15 +206,14 @@
 from rime_sdk.swagger.swagger_client.models.registry_data_params import RegistryDataParams
 from rime_sdk.swagger.swagger_client.models.registry_data_type import RegistryDataType
 from rime_sdk.swagger.swagger_client.models.registry_databricks_info import RegistryDatabricksInfo
 from rime_sdk.swagger.swagger_client.models.registry_generative_language_model_info import RegistryGenerativeLanguageModelInfo
 from rime_sdk.swagger.swagger_client.models.registry_hugging_face_data_info import RegistryHuggingFaceDataInfo
 from rime_sdk.swagger.swagger_client.models.registry_hugging_face_model_info import RegistryHuggingFaceModelInfo
 from rime_sdk.swagger.swagger_client.models.registry_metadata import RegistryMetadata
-from rime_sdk.swagger.swagger_client.models.registry_model_info import RegistryModelInfo
 from rime_sdk.swagger.swagger_client.models.registry_model_path_info import RegistryModelPathInfo
 from rime_sdk.swagger.swagger_client.models.registry_open_ai_chat_completion_model_info import RegistryOpenAIChatCompletionModelInfo
 from rime_sdk.swagger.swagger_client.models.registry_pred_info import RegistryPredInfo
 from rime_sdk.swagger.swagger_client.models.registry_prediction_params import RegistryPredictionParams
 from rime_sdk.swagger.swagger_client.models.registry_validity_status import RegistryValidityStatus
 from rime_sdk.swagger.swagger_client.models.registryprediction_prediction import RegistrypredictionPrediction
 from rime_sdk.swagger.swagger_client.models.rename_test_run_id_body import RenameTestRunIdBody
@@ -272,14 +271,15 @@
 from rime_sdk.swagger.swagger_client.models.rime_detailed_upgrade_status import RimeDetailedUpgradeStatus
 from rime_sdk.swagger.swagger_client.models.rime_ensure_image_existence_response import RimeEnsureImageExistenceResponse
 from rime_sdk.swagger.swagger_client.models.rime_failing_row import RimeFailingRow
 from rime_sdk.swagger.swagger_client.models.rime_failing_rows_result import RimeFailingRowsResult
 from rime_sdk.swagger.swagger_client.models.rime_feature_flags import RimeFeatureFlags
 from rime_sdk.swagger.swagger_client.models.rime_feature_type import RimeFeatureType
 from rime_sdk.swagger.swagger_client.models.rime_float_list import RimeFloatList
+from rime_sdk.swagger.swagger_client.models.rime_generative_model_test_progress import RimeGenerativeModelTestProgress
 from rime_sdk.swagger.swagger_client.models.rime_get_agent_response import RimeGetAgentResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_customer_managed_key_response import RimeGetCustomerManagedKeyResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_datapoints_response import RimeGetDatapointsResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_dataset_file_upload_url_request import RimeGetDatasetFileUploadURLRequest
 from rime_sdk.swagger.swagger_client.models.rime_get_dataset_file_upload_url_response import RimeGetDatasetFileUploadURLResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_dataset_response import RimeGetDatasetResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_enabled_feature_response import RimeGetEnabledFeatureResponse
@@ -433,27 +433,30 @@
 from rime_sdk.swagger.swagger_client.models.rime_workspace import RimeWorkspace
 from rime_sdk.swagger.swagger_client.models.rime_workspace_write_mask import RimeWorkspaceWriteMask
 from rime_sdk.swagger.swagger_client.models.rischemaintegration_integration import RischemaintegrationIntegration
 from rime_sdk.swagger.swagger_client.models.riskscore_risk_category_type import RiskscoreRiskCategoryType
 from rime_sdk.swagger.swagger_client.models.riskscore_risk_score import RiskscoreRiskScore
 from rime_sdk.swagger.swagger_client.models.role_users_body import RoleUsersBody
 from rime_sdk.swagger.swagger_client.models.role_workspace_body import RoleWorkspaceBody
+from rime_sdk.swagger.swagger_client.models.rule_output_rule_evaluation_metadata import RuleOutputRuleEvaluationMetadata
+from rime_sdk.swagger.swagger_client.models.rule_output_rule_evaluation_metadata_model_info import RuleOutputRuleEvaluationMetadataModelInfo
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_custom_image import RuntimeinfoCustomImage
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_custom_image_type import RuntimeinfoCustomImageType
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_resource_request import RuntimeinfoResourceRequest
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_run_time_info import RuntimeinfoRunTimeInfo
 from rime_sdk.swagger.swagger_client.models.schedule_id_uuid_activate_body import ScheduleIdUuidActivateBody
 from rime_sdk.swagger.swagger_client.models.schedule_id_uuid_deactivate_body import ScheduleIdUuidDeactivateBody
 from rime_sdk.swagger.swagger_client.models.schedule_schedule import ScheduleSchedule
 from rime_sdk.swagger.swagger_client.models.schedules_schedule_schedule_id_uuid_body import SchedulesScheduleScheduleIdUuidBody
 from rime_sdk.swagger.swagger_client.models.schemadatacollector_prediction import SchemadatacollectorPrediction
 from rime_sdk.swagger.swagger_client.models.schemafilescanning_package_type import SchemafilescanningPackageType
 from rime_sdk.swagger.swagger_client.models.schemaintegration_integration_variable import SchemaintegrationIntegrationVariable
 from rime_sdk.swagger.swagger_client.models.schemamonitor_config import SchemamonitorConfig
 from rime_sdk.swagger.swagger_client.models.schemanotification_config import SchemanotificationConfig
+from rime_sdk.swagger.swagger_client.models.schemaregistry_model_info import SchemaregistryModelInfo
 from rime_sdk.swagger.swagger_client.models.security_event_details_flagged_datapoint import SecurityEventDetailsFlaggedDatapoint
 from rime_sdk.swagger.swagger_client.models.security_event_details_security_event_type import SecurityEventDetailsSecurityEventType
 from rime_sdk.swagger.swagger_client.models.statedb_archived_job_logs import StatedbArchivedJobLogs
 from rime_sdk.swagger.swagger_client.models.statedb_job_status import StatedbJobStatus
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_datapoints_response import StreamResultOfRimeGetDatapointsResponse
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_latest_logs_response import StreamResultOfRimeGetLatestLogsResponse
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_predictions_response import StreamResultOfRimeGetPredictionsResponse
@@ -510,12 +513,14 @@
 from rime_sdk.swagger.swagger_client.models.v1projectsproject_id_uuidroleusersuser_user_id_uuid_user import V1projectsprojectIdUuidroleusersuserUserIdUuidUser
 from rime_sdk.swagger.swagger_client.models.v1usersuser_id_uuid_user import V1usersuserIdUuidUser
 from rime_sdk.swagger.swagger_client.models.v1workspaceworkspace_workspace_id_uuid_workspace import V1workspaceworkspaceWorkspaceIdUuidWorkspace
 from rime_sdk.swagger.swagger_client.models.validate_firewall_instance_id_uuid_body import ValidateFirewallInstanceIdUuidBody
 from rime_sdk.swagger.swagger_client.models.validate_firewall_instance_id_uuid_body1 import ValidateFirewallInstanceIdUuidBody1
 from rime_sdk.swagger.swagger_client.models.validate_request_input import ValidateRequestInput
 from rime_sdk.swagger.swagger_client.models.validate_request_output import ValidateRequestOutput
+from rime_sdk.swagger.swagger_client.models.validate_response_processed_request import ValidateResponseProcessedRequest
+from rime_sdk.swagger.swagger_client.models.validate_response_product_metadata import ValidateResponseProductMetadata
 from rime_sdk.swagger.swagger_client.models.validation_validate_dataset_response import ValidationValidateDatasetResponse
 from rime_sdk.swagger.swagger_client.models.validation_validate_model_response import ValidationValidateModelResponse
 from rime_sdk.swagger.swagger_client.models.validation_validate_predictions_response import ValidationValidatePredictionsResponse
 from rime_sdk.swagger.swagger_client.models.workspace_id_uuid_users_body import WorkspaceIdUuidUsersBody
 from rime_sdk.swagger.swagger_client.models.workspace_workspace_workspace_id_uuid_body import WorkspaceWorkspaceWorkspaceIdUuidBody
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body1.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body1.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/config_generation_category_config_generation_service_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/config_generation_category_config_generation_service_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/config_generation_profiling_config_generation_service_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/config_generation_profiling_config_generation_service_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/config_generation_test_suite_config_generation_service_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/config_generation_test_suite_config_generation_service_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/crossplanetask_cross_plane_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/crossplanetask_cross_plane_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/dataset_dataset.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/dataset_dataset.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/detection_detection_event.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/detection_event_detail.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_event_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/detection_event_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/detection_resolution.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_resolution.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_file_security_report.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_file_security_report.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_package_url.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_package_url.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata_license.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata_license.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/fileserver_check_object_exists_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/fileserver_check_object_exists_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/fileserver_delete_object_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/fileserver_delete_object_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/fileserver_get_read_object_presigned_link_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/fileserver_get_read_object_presigned_link_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/fileserver_get_upload_object_presigned_link_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/fileserver_get_upload_object_presigned_link_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/fileserver_list_objects_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/fileserver_list_objects_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/firewall_firewall.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewall_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/firewallinstance_firewall_instance_firewall_instance_id_uuid_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewallinstance_firewall_instance_firewall_instance_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/flagged_substring_request_body_component.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/flagged_substring_request_body_component.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generative_testing_result_example.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generative_testing_result_example.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generative_testing_result_standard_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result_standard_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class GenerativeTestingResultStandardInfo(object):
+class GenerativetestingGenerativeTestingResultStandardInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -32,36 +32,36 @@
     }
 
     attribute_map = {
         'description': 'description'
     }
 
     def __init__(self, description=None):  # noqa: E501
-        """GenerativeTestingResultStandardInfo - a model defined in Swagger"""  # noqa: E501
+        """GenerativetestingGenerativeTestingResultStandardInfo - a model defined in Swagger"""  # noqa: E501
         self._description = None
         self.discriminator = None
         if description is not None:
             self.description = description
 
     @property
     def description(self):
-        """Gets the description of this GenerativeTestingResultStandardInfo.  # noqa: E501
+        """Gets the description of this GenerativetestingGenerativeTestingResultStandardInfo.  # noqa: E501
 
 
-        :return: The description of this GenerativeTestingResultStandardInfo.  # noqa: E501
+        :return: The description of this GenerativetestingGenerativeTestingResultStandardInfo.  # noqa: E501
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
-        """Sets the description of this GenerativeTestingResultStandardInfo.
+        """Sets the description of this GenerativetestingGenerativeTestingResultStandardInfo.
 
 
-        :param description: The description of this GenerativeTestingResultStandardInfo.  # noqa: E501
+        :param description: The description of this GenerativetestingGenerativeTestingResultStandardInfo.  # noqa: E501
         :type: str
         """
 
         self._description = description
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(GenerativeTestingResultStandardInfo, dict):
+        if issubclass(GenerativetestingGenerativeTestingResultStandardInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, GenerativeTestingResultStandardInfo):
+        if not isinstance(other, GenerativetestingGenerativeTestingResultStandardInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_custom_pii_entity.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_custom_pii_entity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_denial_of_service_rule_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_denial_of_service_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_status.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_tokenizer.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_flagged_substring.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_flagged_substring.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_effective_config_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_effective_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_instance_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_instance_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_individual_rules_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_individual_rules_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_details.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_rule_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_list_firewall_instances_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_list_firewall_instances_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_off_topic_rule_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_off_topic_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_details.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_rule_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_entity_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_entity_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_details.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_v2_rule_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_v2_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_sensitivity.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_detection_details.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_detection_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_unknown_external_source_rule_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_unknown_external_source_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_update_firewall_instance_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_update_firewall_instance_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,91 +11,115 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class GenerativefirewallValidateResponse(object):
+class RimeListAgentsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'input_results': 'dict(str, GenerativefirewallRuleOutput)',
-        'output_results': 'dict(str, GenerativefirewallRuleOutput)'
+        'agents': 'list[RimeAgent]',
+        'next_page_token': 'str',
+        'has_more': 'bool'
     }
 
     attribute_map = {
-        'input_results': 'inputResults',
-        'output_results': 'outputResults'
+        'agents': 'agents',
+        'next_page_token': 'nextPageToken',
+        'has_more': 'hasMore'
     }
 
-    def __init__(self, input_results=None, output_results=None):  # noqa: E501
-        """GenerativefirewallValidateResponse - a model defined in Swagger"""  # noqa: E501
-        self._input_results = None
-        self._output_results = None
+    def __init__(self, agents=None, next_page_token=None, has_more=None):  # noqa: E501
+        """RimeListAgentsResponse - a model defined in Swagger"""  # noqa: E501
+        self._agents = None
+        self._next_page_token = None
+        self._has_more = None
         self.discriminator = None
-        if input_results is not None:
-            self.input_results = input_results
-        if output_results is not None:
-            self.output_results = output_results
+        if agents is not None:
+            self.agents = agents
+        if next_page_token is not None:
+            self.next_page_token = next_page_token
+        if has_more is not None:
+            self.has_more = has_more
 
     @property
-    def input_results(self):
-        """Gets the input_results of this GenerativefirewallValidateResponse.  # noqa: E501
+    def agents(self):
+        """Gets the agents of this RimeListAgentsResponse.  # noqa: E501
 
-        Results of the firewall for user input. The key is a rule name.  # noqa: E501
 
-        :return: The input_results of this GenerativefirewallValidateResponse.  # noqa: E501
-        :rtype: dict(str, GenerativefirewallRuleOutput)
+        :return: The agents of this RimeListAgentsResponse.  # noqa: E501
+        :rtype: list[RimeAgent]
         """
-        return self._input_results
+        return self._agents
 
-    @input_results.setter
-    def input_results(self, input_results):
-        """Sets the input_results of this GenerativefirewallValidateResponse.
+    @agents.setter
+    def agents(self, agents):
+        """Sets the agents of this RimeListAgentsResponse.
 
-        Results of the firewall for user input. The key is a rule name.  # noqa: E501
 
-        :param input_results: The input_results of this GenerativefirewallValidateResponse.  # noqa: E501
-        :type: dict(str, GenerativefirewallRuleOutput)
+        :param agents: The agents of this RimeListAgentsResponse.  # noqa: E501
+        :type: list[RimeAgent]
         """
 
-        self._input_results = input_results
+        self._agents = agents
 
     @property
-    def output_results(self):
-        """Gets the output_results of this GenerativefirewallValidateResponse.  # noqa: E501
+    def next_page_token(self):
+        """Gets the next_page_token of this RimeListAgentsResponse.  # noqa: E501
 
-        Results of the firewall for model output. The key is a rule name.  # noqa: E501
+        Use this page token in your next ListAgents call to access to the next page of results.  # noqa: E501
 
-        :return: The output_results of this GenerativefirewallValidateResponse.  # noqa: E501
-        :rtype: dict(str, GenerativefirewallRuleOutput)
+        :return: The next_page_token of this RimeListAgentsResponse.  # noqa: E501
+        :rtype: str
         """
-        return self._output_results
+        return self._next_page_token
 
-    @output_results.setter
-    def output_results(self, output_results):
-        """Sets the output_results of this GenerativefirewallValidateResponse.
+    @next_page_token.setter
+    def next_page_token(self, next_page_token):
+        """Sets the next_page_token of this RimeListAgentsResponse.
 
-        Results of the firewall for model output. The key is a rule name.  # noqa: E501
+        Use this page token in your next ListAgents call to access to the next page of results.  # noqa: E501
 
-        :param output_results: The output_results of this GenerativefirewallValidateResponse.  # noqa: E501
-        :type: dict(str, GenerativefirewallRuleOutput)
+        :param next_page_token: The next_page_token of this RimeListAgentsResponse.  # noqa: E501
+        :type: str
         """
 
-        self._output_results = output_results
+        self._next_page_token = next_page_token
+
+    @property
+    def has_more(self):
+        """Gets the has_more of this RimeListAgentsResponse.  # noqa: E501
+
+
+        :return: The has_more of this RimeListAgentsResponse.  # noqa: E501
+        :rtype: bool
+        """
+        return self._has_more
+
+    @has_more.setter
+    def has_more(self, has_more):
+        """Sets the has_more of this RimeListAgentsResponse.
+
+
+        :param has_more: The has_more of this RimeListAgentsResponse.  # noqa: E501
+        :type: bool
+        """
+
+        self._has_more = has_more
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -110,15 +134,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(GenerativefirewallValidateResponse, dict):
+        if issubclass(RimeListAgentsResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -126,15 +150,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, GenerativefirewallValidateResponse):
+        if not isinstance(other, RimeListAgentsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,44 +31,47 @@
         'id': 'RimeUUID',
         'job_id': 'RimeUUID',
         'attack_technique': 'str',
         'attack_objective': 'RimeAttackObjective',
         'objective_sub_category': 'GenerativetestingObjectiveSubCategory',
         'failing_examples': 'list[GenerativeTestingResultExample]',
         'severity': 'RimeSeverity',
-        'owasp_standards': 'list[GenerativeTestingResultStandardInfo]',
-        'nist_standards': 'list[GenerativeTestingResultStandardInfo]',
-        'mitre_standards': 'list[GenerativeTestingResultStandardInfo]'
+        'owasp_standards': 'list[GenerativetestingGenerativeTestingResultStandardInfo]',
+        'nist_standards': 'list[GenerativetestingGenerativeTestingResultStandardInfo]',
+        'mitre_standards': 'list[GenerativetestingGenerativeTestingResultStandardInfo]',
+        'attacks_attempted': 'str'
     }
 
     attribute_map = {
         'id': 'id',
         'job_id': 'jobId',
         'attack_technique': 'attackTechnique',
         'attack_objective': 'attackObjective',
         'objective_sub_category': 'objectiveSubCategory',
         'failing_examples': 'failingExamples',
         'severity': 'severity',
         'owasp_standards': 'owaspStandards',
         'nist_standards': 'nistStandards',
-        'mitre_standards': 'mitreStandards'
+        'mitre_standards': 'mitreStandards',
+        'attacks_attempted': 'attacksAttempted'
     }
 
-    def __init__(self, id=None, job_id=None, attack_technique=None, attack_objective=None, objective_sub_category=None, failing_examples=None, severity=None, owasp_standards=None, nist_standards=None, mitre_standards=None):  # noqa: E501
+    def __init__(self, id=None, job_id=None, attack_technique=None, attack_objective=None, objective_sub_category=None, failing_examples=None, severity=None, owasp_standards=None, nist_standards=None, mitre_standards=None, attacks_attempted=None):  # noqa: E501
         """GenerativetestingGenerativeTestingResult - a model defined in Swagger"""  # noqa: E501
         self._id = None
         self._job_id = None
         self._attack_technique = None
         self._attack_objective = None
         self._objective_sub_category = None
         self._failing_examples = None
         self._severity = None
         self._owasp_standards = None
         self._nist_standards = None
         self._mitre_standards = None
+        self._attacks_attempted = None
         self.discriminator = None
         if id is not None:
             self.id = id
         if job_id is not None:
             self.job_id = job_id
         if attack_technique is not None:
             self.attack_technique = attack_technique
@@ -82,14 +85,16 @@
             self.severity = severity
         if owasp_standards is not None:
             self.owasp_standards = owasp_standards
         if nist_standards is not None:
             self.nist_standards = nist_standards
         if mitre_standards is not None:
             self.mitre_standards = mitre_standards
+        if attacks_attempted is not None:
+            self.attacks_attempted = attacks_attempted
 
     @property
     def id(self):
         """Gets the id of this GenerativetestingGenerativeTestingResult.  # noqa: E501
 
 
         :return: The id of this GenerativetestingGenerativeTestingResult.  # noqa: E501
@@ -241,72 +246,95 @@
     @property
     def owasp_standards(self):
         """Gets the owasp_standards of this GenerativetestingGenerativeTestingResult.  # noqa: E501
 
         Containers describing the various AI risk standards associated with this batch of attack examples.  # noqa: E501
 
         :return: The owasp_standards of this GenerativetestingGenerativeTestingResult.  # noqa: E501
-        :rtype: list[GenerativeTestingResultStandardInfo]
+        :rtype: list[GenerativetestingGenerativeTestingResultStandardInfo]
         """
         return self._owasp_standards
 
     @owasp_standards.setter
     def owasp_standards(self, owasp_standards):
         """Sets the owasp_standards of this GenerativetestingGenerativeTestingResult.
 
         Containers describing the various AI risk standards associated with this batch of attack examples.  # noqa: E501
 
         :param owasp_standards: The owasp_standards of this GenerativetestingGenerativeTestingResult.  # noqa: E501
-        :type: list[GenerativeTestingResultStandardInfo]
+        :type: list[GenerativetestingGenerativeTestingResultStandardInfo]
         """
 
         self._owasp_standards = owasp_standards
 
     @property
     def nist_standards(self):
         """Gets the nist_standards of this GenerativetestingGenerativeTestingResult.  # noqa: E501
 
 
         :return: The nist_standards of this GenerativetestingGenerativeTestingResult.  # noqa: E501
-        :rtype: list[GenerativeTestingResultStandardInfo]
+        :rtype: list[GenerativetestingGenerativeTestingResultStandardInfo]
         """
         return self._nist_standards
 
     @nist_standards.setter
     def nist_standards(self, nist_standards):
         """Sets the nist_standards of this GenerativetestingGenerativeTestingResult.
 
 
         :param nist_standards: The nist_standards of this GenerativetestingGenerativeTestingResult.  # noqa: E501
-        :type: list[GenerativeTestingResultStandardInfo]
+        :type: list[GenerativetestingGenerativeTestingResultStandardInfo]
         """
 
         self._nist_standards = nist_standards
 
     @property
     def mitre_standards(self):
         """Gets the mitre_standards of this GenerativetestingGenerativeTestingResult.  # noqa: E501
 
 
         :return: The mitre_standards of this GenerativetestingGenerativeTestingResult.  # noqa: E501
-        :rtype: list[GenerativeTestingResultStandardInfo]
+        :rtype: list[GenerativetestingGenerativeTestingResultStandardInfo]
         """
         return self._mitre_standards
 
     @mitre_standards.setter
     def mitre_standards(self, mitre_standards):
         """Sets the mitre_standards of this GenerativetestingGenerativeTestingResult.
 
 
         :param mitre_standards: The mitre_standards of this GenerativetestingGenerativeTestingResult.  # noqa: E501
-        :type: list[GenerativeTestingResultStandardInfo]
+        :type: list[GenerativetestingGenerativeTestingResultStandardInfo]
         """
 
         self._mitre_standards = mitre_standards
 
+    @property
+    def attacks_attempted(self):
+        """Gets the attacks_attempted of this GenerativetestingGenerativeTestingResult.  # noqa: E501
+
+        The number of attacks prompts attempted for these results.  # noqa: E501
+
+        :return: The attacks_attempted of this GenerativetestingGenerativeTestingResult.  # noqa: E501
+        :rtype: str
+        """
+        return self._attacks_attempted
+
+    @attacks_attempted.setter
+    def attacks_attempted(self, attacks_attempted):
+        """Sets the attacks_attempted of this GenerativetestingGenerativeTestingResult.
+
+        The number of attacks prompts attempted for these results.  # noqa: E501
+
+        :param attacks_attempted: The attacks_attempted of this GenerativetestingGenerativeTestingResult.  # noqa: E501
+        :type: str
+        """
+
+        self._attacks_attempted = attacks_attempted
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_request_query.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativetesting_objective_sub_category.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_objective_sub_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_pred_info.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,61 +11,87 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class GenerativetestingStartGenerativeModelTestRequest(object):
+class RegistryPredInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'connection_spec': 'GenerativetestingModelConnectionSpec'
+        'connection_info': 'RegistryConnectionInfo',
+        'pred_params': 'RegistryPredictionParams'
     }
 
     attribute_map = {
-        'connection_spec': 'connectionSpec'
+        'connection_info': 'connectionInfo',
+        'pred_params': 'predParams'
     }
 
-    def __init__(self, connection_spec=None):  # noqa: E501
-        """GenerativetestingStartGenerativeModelTestRequest - a model defined in Swagger"""  # noqa: E501
-        self._connection_spec = None
+    def __init__(self, connection_info=None, pred_params=None):  # noqa: E501
+        """RegistryPredInfo - a model defined in Swagger"""  # noqa: E501
+        self._connection_info = None
+        self._pred_params = None
         self.discriminator = None
-        if connection_spec is not None:
-            self.connection_spec = connection_spec
+        if connection_info is not None:
+            self.connection_info = connection_info
+        if pred_params is not None:
+            self.pred_params = pred_params
 
     @property
-    def connection_spec(self):
-        """Gets the connection_spec of this GenerativetestingStartGenerativeModelTestRequest.  # noqa: E501
+    def connection_info(self):
+        """Gets the connection_info of this RegistryPredInfo.  # noqa: E501
 
 
-        :return: The connection_spec of this GenerativetestingStartGenerativeModelTestRequest.  # noqa: E501
-        :rtype: GenerativetestingModelConnectionSpec
+        :return: The connection_info of this RegistryPredInfo.  # noqa: E501
+        :rtype: RegistryConnectionInfo
         """
-        return self._connection_spec
+        return self._connection_info
 
-    @connection_spec.setter
-    def connection_spec(self, connection_spec):
-        """Sets the connection_spec of this GenerativetestingStartGenerativeModelTestRequest.
+    @connection_info.setter
+    def connection_info(self, connection_info):
+        """Sets the connection_info of this RegistryPredInfo.
 
 
-        :param connection_spec: The connection_spec of this GenerativetestingStartGenerativeModelTestRequest.  # noqa: E501
-        :type: GenerativetestingModelConnectionSpec
+        :param connection_info: The connection_info of this RegistryPredInfo.  # noqa: E501
+        :type: RegistryConnectionInfo
         """
 
-        self._connection_spec = connection_spec
+        self._connection_info = connection_info
+
+    @property
+    def pred_params(self):
+        """Gets the pred_params of this RegistryPredInfo.  # noqa: E501
+
+
+        :return: The pred_params of this RegistryPredInfo.  # noqa: E501
+        :rtype: RegistryPredictionParams
+        """
+        return self._pred_params
+
+    @pred_params.setter
+    def pred_params(self, pred_params):
+        """Sets the pred_params of this RegistryPredInfo.
+
+
+        :param pred_params: The pred_params of this RegistryPredInfo.  # noqa: E501
+        :type: RegistryPredictionParams
+        """
+
+        self._pred_params = pred_params
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(GenerativetestingStartGenerativeModelTestRequest, dict):
+        if issubclass(RegistryPredInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, GenerativetestingStartGenerativeModelTestRequest):
+        if not isinstance(other, RegistryPredInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/googlerpc_status.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/integration_integration_level.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/integration_integration_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     AWS_ROLE_ARN = "INTEGRATION_TYPE_AWS_ROLE_ARN"
     HUGGINGFACE = "INTEGRATION_TYPE_HUGGINGFACE"
     GCS = "INTEGRATION_TYPE_GCS"
     AZURE_CLIENT_SECRET = "INTEGRATION_TYPE_AZURE_CLIENT_SECRET"
     AZURE_WORKLOAD_IDENTITY = "INTEGRATION_TYPE_AZURE_WORKLOAD_IDENTITY"
     INTERNAL_OPENAI_API_KEY = "INTEGRATION_TYPE_INTERNAL_OPENAI_API_KEY"
     OPENAI_API = "INTEGRATION_TYPE_OPENAI_API"
+    HTTP_AUTH = "INTEGRATION_TYPE_HTTP_AUTH"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/job_data_generative_model_test.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,61 +11,35 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class JobDataGenerativeModelTest(object):
+class RimeListUsersRequestQuery(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'workspace_id': 'RimeUUID'
     }
 
     attribute_map = {
-        'workspace_id': 'workspaceId'
     }
 
-    def __init__(self, workspace_id=None):  # noqa: E501
-        """JobDataGenerativeModelTest - a model defined in Swagger"""  # noqa: E501
-        self._workspace_id = None
+    def __init__(self):  # noqa: E501
+        """RimeListUsersRequestQuery - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
-        if workspace_id is not None:
-            self.workspace_id = workspace_id
-
-    @property
-    def workspace_id(self):
-        """Gets the workspace_id of this JobDataGenerativeModelTest.  # noqa: E501
-
-
-        :return: The workspace_id of this JobDataGenerativeModelTest.  # noqa: E501
-        :rtype: RimeUUID
-        """
-        return self._workspace_id
-
-    @workspace_id.setter
-    def workspace_id(self, workspace_id):
-        """Sets the workspace_id of this JobDataGenerativeModelTest.
-
-
-        :param workspace_id: The workspace_id of this JobDataGenerativeModelTest.  # noqa: E501
-        :type: RimeUUID
-        """
-
-        self._workspace_id = workspace_id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(JobDataGenerativeModelTest, dict):
+        if issubclass(RimeListUsersRequestQuery, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, JobDataGenerativeModelTest):
+        if not isinstance(other, RimeListUsersRequestQuery):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/job_data_scan.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/job_data_scan.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/language_detection_details_language_substring.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/language_detection_details_language_substring.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_file_scan_results_request_file_scan_query.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_file_scan_results_request_file_scan_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/model_model.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/model_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         'name': 'str',
         'model_id': 'RimeUUID',
         'project_ids': 'list[RimeUUID]',
         'creator_id': 'RimeUUID',
         'creation_time': 'datetime',
         'external_id': 'str',
         'user_metadata': 'RegistryMetadata',
-        'model_info': 'RegistryModelInfo',
+        'model_info': 'SchemaregistryModelInfo',
         'validity_status': 'RegistryValidityStatus',
         'integration_id': 'RimeUUID',
         'model_endpoint_integration_id': 'RimeUUID',
         'validity_status_message': 'str'
     }
 
     attribute_map = {
@@ -252,25 +252,25 @@
 
     @property
     def model_info(self):
         """Gets the model_info of this ModelModel.  # noqa: E501
 
 
         :return: The model_info of this ModelModel.  # noqa: E501
-        :rtype: RegistryModelInfo
+        :rtype: SchemaregistryModelInfo
         """
         return self._model_info
 
     @model_info.setter
     def model_info(self, model_info):
         """Sets the model_info of this ModelModel.
 
 
         :param model_info: The model_info of this ModelModel.  # noqa: E501
-        :type: RegistryModelInfo
+        :type: SchemaregistryModelInfo
         """
 
         self._model_info = model_info
 
     @property
     def validity_status(self):
         """Gets the validity_status of this ModelModel.  # noqa: E501
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_monitor.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_threshold.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_threshold.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitor_transform.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_transform.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/notification_digest_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_digest_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/notification_notification.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_notification.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/notification_notification_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_notification_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/notification_object_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_object_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/pii_detection_details_flagged_entity.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/pii_detection_details_flagged_entity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_activate_schedule_for_project_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_activate_schedule_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_create_project_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_create_project_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_create_project_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_create_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_deactivate_schedule_for_project_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_deactivate_schedule_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_get_project_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_get_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'project_id': 'object',
         'name': 'str',
         'metadata': 'RegistryMetadata',
         'external_id': 'str',
-        'model_info': 'RegistryModelInfo',
+        'model_info': 'SchemaregistryModelInfo',
         'integration_id': 'RimeUUID',
         'skip_validation': 'bool',
         'agent_id': 'RimeUUID',
         'model_endpoint_integration_id': 'RimeUUID'
     }
 
     attribute_map = {
@@ -175,25 +175,25 @@
 
     @property
     def model_info(self):
         """Gets the model_info of this ProjectIdUuidModelBody.  # noqa: E501
 
 
         :return: The model_info of this ProjectIdUuidModelBody.  # noqa: E501
-        :rtype: RegistryModelInfo
+        :rtype: SchemaregistryModelInfo
         """
         return self._model_info
 
     @model_info.setter
     def model_info(self, model_info):
         """Sets the model_info of this ProjectIdUuidModelBody.
 
 
         :param model_info: The model_info of this ProjectIdUuidModelBody.  # noqa: E501
-        :type: RegistryModelInfo
+        :type: SchemaregistryModelInfo
         """
 
         self._model_info = model_info
 
     @property
     def integration_id(self):
         """Gets the integration_id of this ProjectIdUuidModelBody.  # noqa: E501
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_owner_details.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_project.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_project.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_project_status.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_project_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_project_with_details.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_project_with_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_schedule_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_schedule_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_update_project_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_update_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/protobuf_any.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_connection_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_connection_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_params.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_generative_language_model_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_generative_language_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_metadata.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_model_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemaregistry_model_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RegistryModelInfo(object):
+class SchemaregistryModelInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -38,15 +38,15 @@
         'model_path': 'modelPath',
         'hugging_face': 'huggingFace',
         'generative_language_model': 'generativeLanguageModel',
         'openai_chat': 'openaiChat'
     }
 
     def __init__(self, model_path=None, hugging_face=None, generative_language_model=None, openai_chat=None):  # noqa: E501
-        """RegistryModelInfo - a model defined in Swagger"""  # noqa: E501
+        """SchemaregistryModelInfo - a model defined in Swagger"""  # noqa: E501
         self._model_path = None
         self._hugging_face = None
         self._generative_language_model = None
         self._openai_chat = None
         self.discriminator = None
         if model_path is not None:
             self.model_path = model_path
@@ -55,91 +55,91 @@
         if generative_language_model is not None:
             self.generative_language_model = generative_language_model
         if openai_chat is not None:
             self.openai_chat = openai_chat
 
     @property
     def model_path(self):
-        """Gets the model_path of this RegistryModelInfo.  # noqa: E501
+        """Gets the model_path of this SchemaregistryModelInfo.  # noqa: E501
 
 
-        :return: The model_path of this RegistryModelInfo.  # noqa: E501
+        :return: The model_path of this SchemaregistryModelInfo.  # noqa: E501
         :rtype: RegistryModelPathInfo
         """
         return self._model_path
 
     @model_path.setter
     def model_path(self, model_path):
-        """Sets the model_path of this RegistryModelInfo.
+        """Sets the model_path of this SchemaregistryModelInfo.
 
 
-        :param model_path: The model_path of this RegistryModelInfo.  # noqa: E501
+        :param model_path: The model_path of this SchemaregistryModelInfo.  # noqa: E501
         :type: RegistryModelPathInfo
         """
 
         self._model_path = model_path
 
     @property
     def hugging_face(self):
-        """Gets the hugging_face of this RegistryModelInfo.  # noqa: E501
+        """Gets the hugging_face of this SchemaregistryModelInfo.  # noqa: E501
 
 
-        :return: The hugging_face of this RegistryModelInfo.  # noqa: E501
+        :return: The hugging_face of this SchemaregistryModelInfo.  # noqa: E501
         :rtype: RegistryHuggingFaceModelInfo
         """
         return self._hugging_face
 
     @hugging_face.setter
     def hugging_face(self, hugging_face):
-        """Sets the hugging_face of this RegistryModelInfo.
+        """Sets the hugging_face of this SchemaregistryModelInfo.
 
 
-        :param hugging_face: The hugging_face of this RegistryModelInfo.  # noqa: E501
+        :param hugging_face: The hugging_face of this SchemaregistryModelInfo.  # noqa: E501
         :type: RegistryHuggingFaceModelInfo
         """
 
         self._hugging_face = hugging_face
 
     @property
     def generative_language_model(self):
-        """Gets the generative_language_model of this RegistryModelInfo.  # noqa: E501
+        """Gets the generative_language_model of this SchemaregistryModelInfo.  # noqa: E501
 
 
-        :return: The generative_language_model of this RegistryModelInfo.  # noqa: E501
+        :return: The generative_language_model of this SchemaregistryModelInfo.  # noqa: E501
         :rtype: RegistryGenerativeLanguageModelInfo
         """
         return self._generative_language_model
 
     @generative_language_model.setter
     def generative_language_model(self, generative_language_model):
-        """Sets the generative_language_model of this RegistryModelInfo.
+        """Sets the generative_language_model of this SchemaregistryModelInfo.
 
 
-        :param generative_language_model: The generative_language_model of this RegistryModelInfo.  # noqa: E501
+        :param generative_language_model: The generative_language_model of this SchemaregistryModelInfo.  # noqa: E501
         :type: RegistryGenerativeLanguageModelInfo
         """
 
         self._generative_language_model = generative_language_model
 
     @property
     def openai_chat(self):
-        """Gets the openai_chat of this RegistryModelInfo.  # noqa: E501
+        """Gets the openai_chat of this SchemaregistryModelInfo.  # noqa: E501
 
 
-        :return: The openai_chat of this RegistryModelInfo.  # noqa: E501
+        :return: The openai_chat of this SchemaregistryModelInfo.  # noqa: E501
         :rtype: RegistryOpenAIChatCompletionModelInfo
         """
         return self._openai_chat
 
     @openai_chat.setter
     def openai_chat(self, openai_chat):
-        """Sets the openai_chat of this RegistryModelInfo.
+        """Sets the openai_chat of this SchemaregistryModelInfo.
 
 
-        :param openai_chat: The openai_chat of this RegistryModelInfo.  # noqa: E501
+        :param openai_chat: The openai_chat of this SchemaregistryModelInfo.  # noqa: E501
         :type: RegistryOpenAIChatCompletionModelInfo
         """
 
         self._openai_chat = openai_chat
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -158,15 +158,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RegistryModelInfo, dict):
+        if issubclass(SchemaregistryModelInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -174,15 +174,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RegistryModelInfo):
+        if not isinstance(other, SchemaregistryModelInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_open_ai_chat_completion_model_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_open_ai_chat_completion_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_pred_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,87 +11,90 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RegistryPredInfo(object):
+class RimeStorePredictionsRequestPrediction(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'connection_info': 'RegistryConnectionInfo',
-        'pred_params': 'RegistryPredictionParams'
+        'datapoint_id': 'RimeUUID',
+        'prediction': 'str'
     }
 
     attribute_map = {
-        'connection_info': 'connectionInfo',
-        'pred_params': 'predParams'
+        'datapoint_id': 'datapointId',
+        'prediction': 'prediction'
     }
 
-    def __init__(self, connection_info=None, pred_params=None):  # noqa: E501
-        """RegistryPredInfo - a model defined in Swagger"""  # noqa: E501
-        self._connection_info = None
-        self._pred_params = None
+    def __init__(self, datapoint_id=None, prediction=None):  # noqa: E501
+        """RimeStorePredictionsRequestPrediction - a model defined in Swagger"""  # noqa: E501
+        self._datapoint_id = None
+        self._prediction = None
         self.discriminator = None
-        if connection_info is not None:
-            self.connection_info = connection_info
-        if pred_params is not None:
-            self.pred_params = pred_params
+        if datapoint_id is not None:
+            self.datapoint_id = datapoint_id
+        self.prediction = prediction
 
     @property
-    def connection_info(self):
-        """Gets the connection_info of this RegistryPredInfo.  # noqa: E501
+    def datapoint_id(self):
+        """Gets the datapoint_id of this RimeStorePredictionsRequestPrediction.  # noqa: E501
 
 
-        :return: The connection_info of this RegistryPredInfo.  # noqa: E501
-        :rtype: RegistryConnectionInfo
+        :return: The datapoint_id of this RimeStorePredictionsRequestPrediction.  # noqa: E501
+        :rtype: RimeUUID
         """
-        return self._connection_info
+        return self._datapoint_id
 
-    @connection_info.setter
-    def connection_info(self, connection_info):
-        """Sets the connection_info of this RegistryPredInfo.
+    @datapoint_id.setter
+    def datapoint_id(self, datapoint_id):
+        """Sets the datapoint_id of this RimeStorePredictionsRequestPrediction.
 
 
-        :param connection_info: The connection_info of this RegistryPredInfo.  # noqa: E501
-        :type: RegistryConnectionInfo
+        :param datapoint_id: The datapoint_id of this RimeStorePredictionsRequestPrediction.  # noqa: E501
+        :type: RimeUUID
         """
 
-        self._connection_info = connection_info
+        self._datapoint_id = datapoint_id
 
     @property
-    def pred_params(self):
-        """Gets the pred_params of this RegistryPredInfo.  # noqa: E501
+    def prediction(self):
+        """Gets the prediction of this RimeStorePredictionsRequestPrediction.  # noqa: E501
 
+        A JSON-encoded prediction dictionary.  # noqa: E501
 
-        :return: The pred_params of this RegistryPredInfo.  # noqa: E501
-        :rtype: RegistryPredictionParams
+        :return: The prediction of this RimeStorePredictionsRequestPrediction.  # noqa: E501
+        :rtype: str
         """
-        return self._pred_params
+        return self._prediction
 
-    @pred_params.setter
-    def pred_params(self, pred_params):
-        """Sets the pred_params of this RegistryPredInfo.
+    @prediction.setter
+    def prediction(self, prediction):
+        """Sets the prediction of this RimeStorePredictionsRequestPrediction.
 
+        A JSON-encoded prediction dictionary.  # noqa: E501
 
-        :param pred_params: The pred_params of this RegistryPredInfo.  # noqa: E501
-        :type: RegistryPredictionParams
+        :param prediction: The prediction of this RimeStorePredictionsRequestPrediction.  # noqa: E501
+        :type: str
         """
+        if prediction is None:
+            raise ValueError("Invalid value for `prediction`, must not be `None`")  # noqa: E501
 
-        self._pred_params = pred_params
+        self._prediction = prediction
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +109,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RegistryPredInfo, dict):
+        if issubclass(RimeStorePredictionsRequestPrediction, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +125,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RegistryPredInfo):
+        if not isinstance(other, RimeStorePredictionsRequestPrediction):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registry_validity_status.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_validity_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/repo_metadata_reputation.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/repo_metadata_reputation.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_actor_role.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_actor_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_agent.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_agent_desired_state.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent_desired_state.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_agent_status.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_attack_objective.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_attack_objective.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_category_metric.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_category_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_config_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_config_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_schedule_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_schedule_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_schedule_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_schedule_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_schedule_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_schedule_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_detailed_upgrade_status.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_detailed_upgrade_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_failing_row.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_failing_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_feature_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_feature_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_float_list.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_float_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_file_scan_result_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_file_scan_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_schedule_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_schedule_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_time_series_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_time_series_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_upgrade_for_agent_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_upgrade_for_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_image_reference.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_image_reference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_int_list.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_int_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_integration_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_integration_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_data.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_data.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_view.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_view.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_language.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_language.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_license_feature.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_license_feature.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_license_limit.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_license_limit.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_limit_status.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_limit_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,111 +11,109 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeListAgentsResponse(object):
+class RimeListModelsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'agents': 'list[RimeAgent]',
+        'models': 'list[RimeModelWithOwnerDetails]',
         'next_page_token': 'str',
         'has_more': 'bool'
     }
 
     attribute_map = {
-        'agents': 'agents',
+        'models': 'models',
         'next_page_token': 'nextPageToken',
         'has_more': 'hasMore'
     }
 
-    def __init__(self, agents=None, next_page_token=None, has_more=None):  # noqa: E501
-        """RimeListAgentsResponse - a model defined in Swagger"""  # noqa: E501
-        self._agents = None
+    def __init__(self, models=None, next_page_token=None, has_more=None):  # noqa: E501
+        """RimeListModelsResponse - a model defined in Swagger"""  # noqa: E501
+        self._models = None
         self._next_page_token = None
         self._has_more = None
         self.discriminator = None
-        if agents is not None:
-            self.agents = agents
+        if models is not None:
+            self.models = models
         if next_page_token is not None:
             self.next_page_token = next_page_token
         if has_more is not None:
             self.has_more = has_more
 
     @property
-    def agents(self):
-        """Gets the agents of this RimeListAgentsResponse.  # noqa: E501
+    def models(self):
+        """Gets the models of this RimeListModelsResponse.  # noqa: E501
 
 
-        :return: The agents of this RimeListAgentsResponse.  # noqa: E501
-        :rtype: list[RimeAgent]
+        :return: The models of this RimeListModelsResponse.  # noqa: E501
+        :rtype: list[RimeModelWithOwnerDetails]
         """
-        return self._agents
+        return self._models
 
-    @agents.setter
-    def agents(self, agents):
-        """Sets the agents of this RimeListAgentsResponse.
+    @models.setter
+    def models(self, models):
+        """Sets the models of this RimeListModelsResponse.
 
 
-        :param agents: The agents of this RimeListAgentsResponse.  # noqa: E501
-        :type: list[RimeAgent]
+        :param models: The models of this RimeListModelsResponse.  # noqa: E501
+        :type: list[RimeModelWithOwnerDetails]
         """
 
-        self._agents = agents
+        self._models = models
 
     @property
     def next_page_token(self):
-        """Gets the next_page_token of this RimeListAgentsResponse.  # noqa: E501
+        """Gets the next_page_token of this RimeListModelsResponse.  # noqa: E501
 
-        Use this page token in your next ListAgents call to access to the next page of results.  # noqa: E501
 
-        :return: The next_page_token of this RimeListAgentsResponse.  # noqa: E501
+        :return: The next_page_token of this RimeListModelsResponse.  # noqa: E501
         :rtype: str
         """
         return self._next_page_token
 
     @next_page_token.setter
     def next_page_token(self, next_page_token):
-        """Sets the next_page_token of this RimeListAgentsResponse.
+        """Sets the next_page_token of this RimeListModelsResponse.
 
-        Use this page token in your next ListAgents call to access to the next page of results.  # noqa: E501
 
-        :param next_page_token: The next_page_token of this RimeListAgentsResponse.  # noqa: E501
+        :param next_page_token: The next_page_token of this RimeListModelsResponse.  # noqa: E501
         :type: str
         """
 
         self._next_page_token = next_page_token
 
     @property
     def has_more(self):
-        """Gets the has_more of this RimeListAgentsResponse.  # noqa: E501
+        """Gets the has_more of this RimeListModelsResponse.  # noqa: E501
 
 
-        :return: The has_more of this RimeListAgentsResponse.  # noqa: E501
+        :return: The has_more of this RimeListModelsResponse.  # noqa: E501
         :rtype: bool
         """
         return self._has_more
 
     @has_more.setter
     def has_more(self, has_more):
-        """Sets the has_more of this RimeListAgentsResponse.
+        """Sets the has_more of this RimeListModelsResponse.
 
 
-        :param has_more: The has_more of this RimeListAgentsResponse.  # noqa: E501
+        :param has_more: The has_more of this RimeListModelsResponse.  # noqa: E501
         :type: bool
         """
 
         self._has_more = has_more
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -134,15 +132,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeListAgentsResponse, dict):
+        if issubclass(RimeListModelsResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -150,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeListAgentsResponse):
+        if not isinstance(other, RimeListModelsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,109 +11,109 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeListModelsResponse(object):
+class RimeListWorkspacesResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'models': 'list[RimeModelWithOwnerDetails]',
+        'workspaces': 'list[RimeWorkspace]',
         'next_page_token': 'str',
         'has_more': 'bool'
     }
 
     attribute_map = {
-        'models': 'models',
+        'workspaces': 'workspaces',
         'next_page_token': 'nextPageToken',
         'has_more': 'hasMore'
     }
 
-    def __init__(self, models=None, next_page_token=None, has_more=None):  # noqa: E501
-        """RimeListModelsResponse - a model defined in Swagger"""  # noqa: E501
-        self._models = None
+    def __init__(self, workspaces=None, next_page_token=None, has_more=None):  # noqa: E501
+        """RimeListWorkspacesResponse - a model defined in Swagger"""  # noqa: E501
+        self._workspaces = None
         self._next_page_token = None
         self._has_more = None
         self.discriminator = None
-        if models is not None:
-            self.models = models
+        if workspaces is not None:
+            self.workspaces = workspaces
         if next_page_token is not None:
             self.next_page_token = next_page_token
         if has_more is not None:
             self.has_more = has_more
 
     @property
-    def models(self):
-        """Gets the models of this RimeListModelsResponse.  # noqa: E501
+    def workspaces(self):
+        """Gets the workspaces of this RimeListWorkspacesResponse.  # noqa: E501
 
 
-        :return: The models of this RimeListModelsResponse.  # noqa: E501
-        :rtype: list[RimeModelWithOwnerDetails]
+        :return: The workspaces of this RimeListWorkspacesResponse.  # noqa: E501
+        :rtype: list[RimeWorkspace]
         """
-        return self._models
+        return self._workspaces
 
-    @models.setter
-    def models(self, models):
-        """Sets the models of this RimeListModelsResponse.
+    @workspaces.setter
+    def workspaces(self, workspaces):
+        """Sets the workspaces of this RimeListWorkspacesResponse.
 
 
-        :param models: The models of this RimeListModelsResponse.  # noqa: E501
-        :type: list[RimeModelWithOwnerDetails]
+        :param workspaces: The workspaces of this RimeListWorkspacesResponse.  # noqa: E501
+        :type: list[RimeWorkspace]
         """
 
-        self._models = models
+        self._workspaces = workspaces
 
     @property
     def next_page_token(self):
-        """Gets the next_page_token of this RimeListModelsResponse.  # noqa: E501
+        """Gets the next_page_token of this RimeListWorkspacesResponse.  # noqa: E501
 
 
-        :return: The next_page_token of this RimeListModelsResponse.  # noqa: E501
+        :return: The next_page_token of this RimeListWorkspacesResponse.  # noqa: E501
         :rtype: str
         """
         return self._next_page_token
 
     @next_page_token.setter
     def next_page_token(self, next_page_token):
-        """Sets the next_page_token of this RimeListModelsResponse.
+        """Sets the next_page_token of this RimeListWorkspacesResponse.
 
 
-        :param next_page_token: The next_page_token of this RimeListModelsResponse.  # noqa: E501
+        :param next_page_token: The next_page_token of this RimeListWorkspacesResponse.  # noqa: E501
         :type: str
         """
 
         self._next_page_token = next_page_token
 
     @property
     def has_more(self):
-        """Gets the has_more of this RimeListModelsResponse.  # noqa: E501
+        """Gets the has_more of this RimeListWorkspacesResponse.  # noqa: E501
 
 
-        :return: The has_more of this RimeListModelsResponse.  # noqa: E501
+        :return: The has_more of this RimeListWorkspacesResponse.  # noqa: E501
         :rtype: bool
         """
         return self._has_more
 
     @has_more.setter
     def has_more(self, has_more):
-        """Sets the has_more of this RimeListModelsResponse.
+        """Sets the has_more of this RimeListWorkspacesResponse.
 
 
-        :param has_more: The has_more of this RimeListModelsResponse.  # noqa: E501
+        :param has_more: The has_more of this RimeListWorkspacesResponse.  # noqa: E501
         :type: bool
         """
 
         self._has_more = has_more
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -132,15 +132,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeListModelsResponse, dict):
+        if issubclass(RimeListWorkspacesResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -148,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeListModelsResponse):
+        if not isinstance(other, RimeListWorkspacesResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeListUsersRequestQuery(object):
+class RimeSendRIEmailResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeListUsersRequestQuery - a model defined in Swagger"""  # noqa: E501
+        """RimeSendRIEmailResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeListUsersRequestQuery, dict):
+        if issubclass(RimeSendRIEmailResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeListUsersRequestQuery):
+        if not isinstance(other, RimeSendRIEmailResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,109 +11,115 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeListWorkspacesResponse(object):
+class TestrunresultListTestRunsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'workspaces': 'list[RimeWorkspace]',
+        'test_runs': 'list[TestrunresultTestRunDetail]',
         'next_page_token': 'str',
         'has_more': 'bool'
     }
 
     attribute_map = {
-        'workspaces': 'workspaces',
+        'test_runs': 'testRuns',
         'next_page_token': 'nextPageToken',
         'has_more': 'hasMore'
     }
 
-    def __init__(self, workspaces=None, next_page_token=None, has_more=None):  # noqa: E501
-        """RimeListWorkspacesResponse - a model defined in Swagger"""  # noqa: E501
-        self._workspaces = None
+    def __init__(self, test_runs=None, next_page_token=None, has_more=None):  # noqa: E501
+        """TestrunresultListTestRunsResponse - a model defined in Swagger"""  # noqa: E501
+        self._test_runs = None
         self._next_page_token = None
         self._has_more = None
         self.discriminator = None
-        if workspaces is not None:
-            self.workspaces = workspaces
+        if test_runs is not None:
+            self.test_runs = test_runs
         if next_page_token is not None:
             self.next_page_token = next_page_token
         if has_more is not None:
             self.has_more = has_more
 
     @property
-    def workspaces(self):
-        """Gets the workspaces of this RimeListWorkspacesResponse.  # noqa: E501
+    def test_runs(self):
+        """Gets the test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
 
+        The details of the test runs.  # noqa: E501
 
-        :return: The workspaces of this RimeListWorkspacesResponse.  # noqa: E501
-        :rtype: list[RimeWorkspace]
+        :return: The test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
+        :rtype: list[TestrunresultTestRunDetail]
         """
-        return self._workspaces
+        return self._test_runs
 
-    @workspaces.setter
-    def workspaces(self, workspaces):
-        """Sets the workspaces of this RimeListWorkspacesResponse.
+    @test_runs.setter
+    def test_runs(self, test_runs):
+        """Sets the test_runs of this TestrunresultListTestRunsResponse.
 
+        The details of the test runs.  # noqa: E501
 
-        :param workspaces: The workspaces of this RimeListWorkspacesResponse.  # noqa: E501
-        :type: list[RimeWorkspace]
+        :param test_runs: The test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
+        :type: list[TestrunresultTestRunDetail]
         """
 
-        self._workspaces = workspaces
+        self._test_runs = test_runs
 
     @property
     def next_page_token(self):
-        """Gets the next_page_token of this RimeListWorkspacesResponse.  # noqa: E501
+        """Gets the next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
 
+        A token representing the next page from the list returned by a ListTestRuns query.  # noqa: E501
 
-        :return: The next_page_token of this RimeListWorkspacesResponse.  # noqa: E501
+        :return: The next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
         :rtype: str
         """
         return self._next_page_token
 
     @next_page_token.setter
     def next_page_token(self, next_page_token):
-        """Sets the next_page_token of this RimeListWorkspacesResponse.
+        """Sets the next_page_token of this TestrunresultListTestRunsResponse.
 
+        A token representing the next page from the list returned by a ListTestRuns query.  # noqa: E501
 
-        :param next_page_token: The next_page_token of this RimeListWorkspacesResponse.  # noqa: E501
+        :param next_page_token: The next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
         :type: str
         """
 
         self._next_page_token = next_page_token
 
     @property
     def has_more(self):
-        """Gets the has_more of this RimeListWorkspacesResponse.  # noqa: E501
+        """Gets the has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
 
+        A Boolean that specifies whether there are more test runs to return.  # noqa: E501
 
-        :return: The has_more of this RimeListWorkspacesResponse.  # noqa: E501
+        :return: The has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
         :rtype: bool
         """
         return self._has_more
 
     @has_more.setter
     def has_more(self, has_more):
-        """Sets the has_more of this RimeListWorkspacesResponse.
+        """Sets the has_more of this TestrunresultListTestRunsResponse.
 
+        A Boolean that specifies whether there are more test runs to return.  # noqa: E501
 
-        :param has_more: The has_more of this RimeListWorkspacesResponse.  # noqa: E501
+        :param has_more: The has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
         :type: bool
         """
 
         self._has_more = has_more
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -132,15 +138,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeListWorkspacesResponse, dict):
+        if issubclass(TestrunresultListTestRunsResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -148,15 +154,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeListWorkspacesResponse):
+        if not isinstance(other, TestrunresultListTestRunsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_managed_image.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_managed_image_package_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image_package_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_model_card.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_model_task.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_task.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_named_double.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_named_double.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_order.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_order.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_safe_url.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_safe_url.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_search_spec.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_search_spec.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeSendRIEmailResponse(object):
+class RimeStorePredictionsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeSendRIEmailResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeStorePredictionsResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeSendRIEmailResponse, dict):
+        if issubclass(RimeStorePredictionsResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeSendRIEmailResponse):
+        if not isinstance(other, RimeStorePredictionsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_severity.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,90 +11,113 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeStorePredictionsRequestPrediction(object):
+class TestrunresultListTestRunsRequestQuery(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'datapoint_id': 'RimeUUID',
-        'prediction': 'str'
+        'project_id': 'RimeUUID',
+        'testing_type': 'RimeTestType',
+        'schedule_id': 'RimeUUID'
     }
 
     attribute_map = {
-        'datapoint_id': 'datapointId',
-        'prediction': 'prediction'
+        'project_id': 'projectId',
+        'testing_type': 'testingType',
+        'schedule_id': 'scheduleId'
     }
 
-    def __init__(self, datapoint_id=None, prediction=None):  # noqa: E501
-        """RimeStorePredictionsRequestPrediction - a model defined in Swagger"""  # noqa: E501
-        self._datapoint_id = None
-        self._prediction = None
+    def __init__(self, project_id=None, testing_type=None, schedule_id=None):  # noqa: E501
+        """TestrunresultListTestRunsRequestQuery - a model defined in Swagger"""  # noqa: E501
+        self._project_id = None
+        self._testing_type = None
+        self._schedule_id = None
         self.discriminator = None
-        if datapoint_id is not None:
-            self.datapoint_id = datapoint_id
-        self.prediction = prediction
+        if project_id is not None:
+            self.project_id = project_id
+        if testing_type is not None:
+            self.testing_type = testing_type
+        if schedule_id is not None:
+            self.schedule_id = schedule_id
 
     @property
-    def datapoint_id(self):
-        """Gets the datapoint_id of this RimeStorePredictionsRequestPrediction.  # noqa: E501
+    def project_id(self):
+        """Gets the project_id of this TestrunresultListTestRunsRequestQuery.  # noqa: E501
 
 
-        :return: The datapoint_id of this RimeStorePredictionsRequestPrediction.  # noqa: E501
+        :return: The project_id of this TestrunresultListTestRunsRequestQuery.  # noqa: E501
         :rtype: RimeUUID
         """
-        return self._datapoint_id
+        return self._project_id
 
-    @datapoint_id.setter
-    def datapoint_id(self, datapoint_id):
-        """Sets the datapoint_id of this RimeStorePredictionsRequestPrediction.
+    @project_id.setter
+    def project_id(self, project_id):
+        """Sets the project_id of this TestrunresultListTestRunsRequestQuery.
 
 
-        :param datapoint_id: The datapoint_id of this RimeStorePredictionsRequestPrediction.  # noqa: E501
+        :param project_id: The project_id of this TestrunresultListTestRunsRequestQuery.  # noqa: E501
         :type: RimeUUID
         """
 
-        self._datapoint_id = datapoint_id
+        self._project_id = project_id
 
     @property
-    def prediction(self):
-        """Gets the prediction of this RimeStorePredictionsRequestPrediction.  # noqa: E501
+    def testing_type(self):
+        """Gets the testing_type of this TestrunresultListTestRunsRequestQuery.  # noqa: E501
 
-        A JSON-encoded prediction dictionary.  # noqa: E501
 
-        :return: The prediction of this RimeStorePredictionsRequestPrediction.  # noqa: E501
-        :rtype: str
+        :return: The testing_type of this TestrunresultListTestRunsRequestQuery.  # noqa: E501
+        :rtype: RimeTestType
         """
-        return self._prediction
+        return self._testing_type
 
-    @prediction.setter
-    def prediction(self, prediction):
-        """Sets the prediction of this RimeStorePredictionsRequestPrediction.
+    @testing_type.setter
+    def testing_type(self, testing_type):
+        """Sets the testing_type of this TestrunresultListTestRunsRequestQuery.
 
-        A JSON-encoded prediction dictionary.  # noqa: E501
 
-        :param prediction: The prediction of this RimeStorePredictionsRequestPrediction.  # noqa: E501
-        :type: str
+        :param testing_type: The testing_type of this TestrunresultListTestRunsRequestQuery.  # noqa: E501
+        :type: RimeTestType
         """
-        if prediction is None:
-            raise ValueError("Invalid value for `prediction`, must not be `None`")  # noqa: E501
 
-        self._prediction = prediction
+        self._testing_type = testing_type
+
+    @property
+    def schedule_id(self):
+        """Gets the schedule_id of this TestrunresultListTestRunsRequestQuery.  # noqa: E501
+
+
+        :return: The schedule_id of this TestrunresultListTestRunsRequestQuery.  # noqa: E501
+        :rtype: RimeUUID
+        """
+        return self._schedule_id
+
+    @schedule_id.setter
+    def schedule_id(self, schedule_id):
+        """Sets the schedule_id of this TestrunresultListTestRunsRequestQuery.
+
+
+        :param schedule_id: The schedule_id of this TestrunresultListTestRunsRequestQuery.  # noqa: E501
+        :type: RimeUUID
+        """
+
+        self._schedule_id = schedule_id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -109,15 +132,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeStorePredictionsRequestPrediction, dict):
+        if issubclass(TestrunresultListTestRunsRequestQuery, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -125,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeStorePredictionsRequestPrediction):
+        if not isinstance(other, TestrunresultListTestRunsRequestQuery):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_str_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,35 +11,61 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeStorePredictionsResponse(object):
+class RimeStrList(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'values': 'list[str]'
     }
 
     attribute_map = {
+        'values': 'values'
     }
 
-    def __init__(self):  # noqa: E501
-        """RimeStorePredictionsResponse - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, values=None):  # noqa: E501
+        """RimeStrList - a model defined in Swagger"""  # noqa: E501
+        self._values = None
         self.discriminator = None
+        if values is not None:
+            self.values = values
+
+    @property
+    def values(self):
+        """Gets the values of this RimeStrList.  # noqa: E501
+
+
+        :return: The values of this RimeStrList.  # noqa: E501
+        :rtype: list[str]
+        """
+        return self._values
+
+    @values.setter
+    def values(self, values):
+        """Sets the values of this RimeStrList.
+
+
+        :param values: The values of this RimeStrList.  # noqa: E501
+        :type: list[str]
+        """
+
+        self._values = values
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -54,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeStorePredictionsResponse, dict):
+        if issubclass(RimeStrList, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeStorePredictionsResponse):
+        if not isinstance(other, RimeStrList):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_str_list.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,61 +11,41 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeStrList(object):
+class RimeTestType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
+
+    """
+    allowed enum values
+    """
+    STRESS_TESTING_UNSPECIFIED = "TEST_TYPE_STRESS_TESTING_UNSPECIFIED"
+    CONTINUOUS_TESTING = "TEST_TYPE_CONTINUOUS_TESTING"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'values': 'list[str]'
     }
 
     attribute_map = {
-        'values': 'values'
     }
 
-    def __init__(self, values=None):  # noqa: E501
-        """RimeStrList - a model defined in Swagger"""  # noqa: E501
-        self._values = None
+    def __init__(self):  # noqa: E501
+        """RimeTestType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
-        if values is not None:
-            self.values = values
-
-    @property
-    def values(self):
-        """Gets the values of this RimeStrList.  # noqa: E501
-
-
-        :return: The values of this RimeStrList.  # noqa: E501
-        :rtype: list[str]
-        """
-        return self._values
-
-    @values.setter
-    def values(self, values):
-        """Sets the values of this RimeStrList.
-
-
-        :param values: The values of this RimeStrList.  # noqa: E501
-        :type: list[str]
-        """
-
-        self._values = values
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +60,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeStrList, dict):
+        if issubclass(RimeTestType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +76,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeStrList):
+        if not isinstance(other, RimeTestType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_subject_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_subject_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_suggestion.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_suggestion.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_table_column.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_table_column.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_metric.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/user_role.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,40 +11,42 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeTestType(object):
+class UserRole(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    STRESS_TESTING_UNSPECIFIED = "TEST_TYPE_STRESS_TESTING_UNSPECIFIED"
-    CONTINUOUS_TESTING = "TEST_TYPE_CONTINUOUS_TESTING"
+    UNSPECIFIED = "ROLE_UNSPECIFIED"
+    ADMIN = "ROLE_ADMIN"
+    TRIAL_USER = "ROLE_TRIAL_USER"
+    SUPPORT = "ROLE_SUPPORT"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeTestType - a model defined in Swagger"""  # noqa: E501
+        """UserRole - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -60,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeTestType, dict):
+        if issubclass(UserRole, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -76,15 +78,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeTestType):
+        if not isinstance(other, UserRole):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_time_interval.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_time_interval.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_token_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_token_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_toxicity_threat_category.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_toxicity_threat_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_schedule_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_schedule_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_upgrade_status_for_agent_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_upgrade_status_for_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_upgrade_agent_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_upgrade_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_upgrade_status.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_upgrade_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_role.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_uuid.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_uuid.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_workspace.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/role_users_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/role_users_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/role_workspace_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/role_workspace_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_activate_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_activate_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_deactivate_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_deactivate_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/schedule_schedule.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schedule_schedule.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/schedules_schedule_schedule_id_uuid_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schedules_schedule_schedule_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/schemafilescanning_package_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemafilescanning_package_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/schemanotification_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemanotification_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/statedb_job_status.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/statedb_job_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_category_results_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_category_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,119 +11,117 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunresultListTestRunsResponse(object):
+class TestrunresultTestCaseDisplay(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'test_runs': 'list[TestrunresultTestRunDetail]',
-        'next_page_token': 'str',
-        'has_more': 'bool'
+        'table_info': 'str',
+        'details': 'str',
+        'details_layout': 'list[str]'
     }
 
     attribute_map = {
-        'test_runs': 'testRuns',
-        'next_page_token': 'nextPageToken',
-        'has_more': 'hasMore'
+        'table_info': 'tableInfo',
+        'details': 'details',
+        'details_layout': 'detailsLayout'
     }
 
-    def __init__(self, test_runs=None, next_page_token=None, has_more=None):  # noqa: E501
-        """TestrunresultListTestRunsResponse - a model defined in Swagger"""  # noqa: E501
-        self._test_runs = None
-        self._next_page_token = None
-        self._has_more = None
+    def __init__(self, table_info=None, details=None, details_layout=None):  # noqa: E501
+        """TestrunresultTestCaseDisplay - a model defined in Swagger"""  # noqa: E501
+        self._table_info = None
+        self._details = None
+        self._details_layout = None
         self.discriminator = None
-        if test_runs is not None:
-            self.test_runs = test_runs
-        if next_page_token is not None:
-            self.next_page_token = next_page_token
-        if has_more is not None:
-            self.has_more = has_more
+        if table_info is not None:
+            self.table_info = table_info
+        if details is not None:
+            self.details = details
+        if details_layout is not None:
+            self.details_layout = details_layout
 
     @property
-    def test_runs(self):
-        """Gets the test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
+    def table_info(self):
+        """Gets the table_info of this TestrunresultTestCaseDisplay.  # noqa: E501
 
-        The details of the test runs.  # noqa: E501
+        Table info contains information for displaying the test case in a table in the FE.  # noqa: E501
 
-        :return: The test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
-        :rtype: list[TestrunresultTestRunDetail]
+        :return: The table_info of this TestrunresultTestCaseDisplay.  # noqa: E501
+        :rtype: str
         """
-        return self._test_runs
+        return self._table_info
 
-    @test_runs.setter
-    def test_runs(self, test_runs):
-        """Sets the test_runs of this TestrunresultListTestRunsResponse.
+    @table_info.setter
+    def table_info(self, table_info):
+        """Sets the table_info of this TestrunresultTestCaseDisplay.
 
-        The details of the test runs.  # noqa: E501
+        Table info contains information for displaying the test case in a table in the FE.  # noqa: E501
 
-        :param test_runs: The test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
-        :type: list[TestrunresultTestRunDetail]
+        :param table_info: The table_info of this TestrunresultTestCaseDisplay.  # noqa: E501
+        :type: str
         """
 
-        self._test_runs = test_runs
+        self._table_info = table_info
 
     @property
-    def next_page_token(self):
-        """Gets the next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
+    def details(self):
+        """Gets the details of this TestrunresultTestCaseDisplay.  # noqa: E501
 
-        A token representing the next page from the list returned by a ListTestRuns query.  # noqa: E501
+        Details includes ML-specified details for the test case. This can include graphs, HTML, etc.  # noqa: E501
 
-        :return: The next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
+        :return: The details of this TestrunresultTestCaseDisplay.  # noqa: E501
         :rtype: str
         """
-        return self._next_page_token
+        return self._details
 
-    @next_page_token.setter
-    def next_page_token(self, next_page_token):
-        """Sets the next_page_token of this TestrunresultListTestRunsResponse.
+    @details.setter
+    def details(self, details):
+        """Sets the details of this TestrunresultTestCaseDisplay.
 
-        A token representing the next page from the list returned by a ListTestRuns query.  # noqa: E501
+        Details includes ML-specified details for the test case. This can include graphs, HTML, etc.  # noqa: E501
 
-        :param next_page_token: The next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
+        :param details: The details of this TestrunresultTestCaseDisplay.  # noqa: E501
         :type: str
         """
 
-        self._next_page_token = next_page_token
+        self._details = details
 
     @property
-    def has_more(self):
-        """Gets the has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
+    def details_layout(self):
+        """Gets the details_layout of this TestrunresultTestCaseDisplay.  # noqa: E501
 
-        A Boolean that specifies whether there are more test runs to return.  # noqa: E501
 
-        :return: The has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
-        :rtype: bool
+        :return: The details_layout of this TestrunresultTestCaseDisplay.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._has_more
+        return self._details_layout
 
-    @has_more.setter
-    def has_more(self, has_more):
-        """Sets the has_more of this TestrunresultListTestRunsResponse.
+    @details_layout.setter
+    def details_layout(self, details_layout):
+        """Sets the details_layout of this TestrunresultTestCaseDisplay.
 
-        A Boolean that specifies whether there are more test runs to return.  # noqa: E501
 
-        :param has_more: The has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
-        :type: bool
+        :param details_layout: The details_layout of this TestrunresultTestCaseDisplay.  # noqa: E501
+        :type: list[str]
         """
 
-        self._has_more = has_more
+        self._details_layout = details_layout
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -138,15 +136,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunresultListTestRunsResponse, dict):
+        if issubclass(TestrunresultTestCaseDisplay, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -154,15 +152,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunresultListTestRunsResponse):
+        if not isinstance(other, TestrunresultTestCaseDisplay):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,117 +11,113 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunresultTestCaseDisplay(object):
+class ValidationValidateModelResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'table_info': 'str',
-        'details': 'str',
-        'details_layout': 'list[str]'
+        'is_valid': 'bool',
+        'error_message': 'str',
+        'validation_status': 'RegistryValidityStatus'
     }
 
     attribute_map = {
-        'table_info': 'tableInfo',
-        'details': 'details',
-        'details_layout': 'detailsLayout'
+        'is_valid': 'isValid',
+        'error_message': 'errorMessage',
+        'validation_status': 'validationStatus'
     }
 
-    def __init__(self, table_info=None, details=None, details_layout=None):  # noqa: E501
-        """TestrunresultTestCaseDisplay - a model defined in Swagger"""  # noqa: E501
-        self._table_info = None
-        self._details = None
-        self._details_layout = None
+    def __init__(self, is_valid=None, error_message=None, validation_status=None):  # noqa: E501
+        """ValidationValidateModelResponse - a model defined in Swagger"""  # noqa: E501
+        self._is_valid = None
+        self._error_message = None
+        self._validation_status = None
         self.discriminator = None
-        if table_info is not None:
-            self.table_info = table_info
-        if details is not None:
-            self.details = details
-        if details_layout is not None:
-            self.details_layout = details_layout
+        if is_valid is not None:
+            self.is_valid = is_valid
+        if error_message is not None:
+            self.error_message = error_message
+        if validation_status is not None:
+            self.validation_status = validation_status
 
     @property
-    def table_info(self):
-        """Gets the table_info of this TestrunresultTestCaseDisplay.  # noqa: E501
+    def is_valid(self):
+        """Gets the is_valid of this ValidationValidateModelResponse.  # noqa: E501
 
-        Table info contains information for displaying the test case in a table in the FE.  # noqa: E501
 
-        :return: The table_info of this TestrunresultTestCaseDisplay.  # noqa: E501
-        :rtype: str
+        :return: The is_valid of this ValidationValidateModelResponse.  # noqa: E501
+        :rtype: bool
         """
-        return self._table_info
+        return self._is_valid
 
-    @table_info.setter
-    def table_info(self, table_info):
-        """Sets the table_info of this TestrunresultTestCaseDisplay.
+    @is_valid.setter
+    def is_valid(self, is_valid):
+        """Sets the is_valid of this ValidationValidateModelResponse.
 
-        Table info contains information for displaying the test case in a table in the FE.  # noqa: E501
 
-        :param table_info: The table_info of this TestrunresultTestCaseDisplay.  # noqa: E501
-        :type: str
+        :param is_valid: The is_valid of this ValidationValidateModelResponse.  # noqa: E501
+        :type: bool
         """
 
-        self._table_info = table_info
+        self._is_valid = is_valid
 
     @property
-    def details(self):
-        """Gets the details of this TestrunresultTestCaseDisplay.  # noqa: E501
+    def error_message(self):
+        """Gets the error_message of this ValidationValidateModelResponse.  # noqa: E501
 
-        Details includes ML-specified details for the test case. This can include graphs, HTML, etc.  # noqa: E501
 
-        :return: The details of this TestrunresultTestCaseDisplay.  # noqa: E501
+        :return: The error_message of this ValidationValidateModelResponse.  # noqa: E501
         :rtype: str
         """
-        return self._details
+        return self._error_message
 
-    @details.setter
-    def details(self, details):
-        """Sets the details of this TestrunresultTestCaseDisplay.
+    @error_message.setter
+    def error_message(self, error_message):
+        """Sets the error_message of this ValidationValidateModelResponse.
 
-        Details includes ML-specified details for the test case. This can include graphs, HTML, etc.  # noqa: E501
 
-        :param details: The details of this TestrunresultTestCaseDisplay.  # noqa: E501
+        :param error_message: The error_message of this ValidationValidateModelResponse.  # noqa: E501
         :type: str
         """
 
-        self._details = details
+        self._error_message = error_message
 
     @property
-    def details_layout(self):
-        """Gets the details_layout of this TestrunresultTestCaseDisplay.  # noqa: E501
+    def validation_status(self):
+        """Gets the validation_status of this ValidationValidateModelResponse.  # noqa: E501
 
 
-        :return: The details_layout of this TestrunresultTestCaseDisplay.  # noqa: E501
-        :rtype: list[str]
+        :return: The validation_status of this ValidationValidateModelResponse.  # noqa: E501
+        :rtype: RegistryValidityStatus
         """
-        return self._details_layout
+        return self._validation_status
 
-    @details_layout.setter
-    def details_layout(self, details_layout):
-        """Sets the details_layout of this TestrunresultTestCaseDisplay.
+    @validation_status.setter
+    def validation_status(self, validation_status):
+        """Sets the validation_status of this ValidationValidateModelResponse.
 
 
-        :param details_layout: The details_layout of this TestrunresultTestCaseDisplay.  # noqa: E501
-        :type: list[str]
+        :param validation_status: The validation_status of this ValidationValidateModelResponse.  # noqa: E501
+        :type: RegistryValidityStatus
         """
 
-        self._details_layout = details_layout
+        self._validation_status = validation_status
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -136,15 +132,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunresultTestCaseDisplay, dict):
+        if issubclass(ValidationValidateModelResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -152,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunresultTestCaseDisplay):
+        if not isinstance(other, ValidationValidateModelResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/user_private_info.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/user_private_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/user_role.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,43 +11,87 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UserRole(object):
+class UsersUserIdUuidBody(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
-
-    """
-    allowed enum values
-    """
-    UNSPECIFIED = "ROLE_UNSPECIFIED"
-    ADMIN = "ROLE_ADMIN"
-    TRIAL_USER = "ROLE_TRIAL_USER"
-    SUPPORT = "ROLE_SUPPORT"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'user': 'V1usersuserIdUuidUser',
+        'mask': 'RimeUserWriteMask'
     }
 
     attribute_map = {
+        'user': 'user',
+        'mask': 'mask'
     }
 
-    def __init__(self):  # noqa: E501
-        """UserRole - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, user=None, mask=None):  # noqa: E501
+        """UsersUserIdUuidBody - a model defined in Swagger"""  # noqa: E501
+        self._user = None
+        self._mask = None
         self.discriminator = None
+        if user is not None:
+            self.user = user
+        if mask is not None:
+            self.mask = mask
+
+    @property
+    def user(self):
+        """Gets the user of this UsersUserIdUuidBody.  # noqa: E501
+
+
+        :return: The user of this UsersUserIdUuidBody.  # noqa: E501
+        :rtype: V1usersuserIdUuidUser
+        """
+        return self._user
+
+    @user.setter
+    def user(self, user):
+        """Sets the user of this UsersUserIdUuidBody.
+
+
+        :param user: The user of this UsersUserIdUuidBody.  # noqa: E501
+        :type: V1usersuserIdUuidUser
+        """
+
+        self._user = user
+
+    @property
+    def mask(self):
+        """Gets the mask of this UsersUserIdUuidBody.  # noqa: E501
+
+
+        :return: The mask of this UsersUserIdUuidBody.  # noqa: E501
+        :rtype: RimeUserWriteMask
+        """
+        return self._mask
+
+    @mask.setter
+    def mask(self, mask):
+        """Sets the mask of this UsersUserIdUuidBody.
+
+
+        :param mask: The mask of this UsersUserIdUuidBody.  # noqa: E501
+        :type: RimeUserWriteMask
+        """
+
+        self._mask = mask
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -62,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UserRole, dict):
+        if issubclass(UsersUserIdUuidBody, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UserRole):
+        if not isinstance(other, UsersUserIdUuidBody):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/user_user_detail.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/user_user_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,87 +11,89 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UsersUserIdUuidBody(object):
+class UsersUserUserIdUuidBody1(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'user': 'V1usersuserIdUuidUser',
-        'mask': 'RimeUserWriteMask'
+        'workspace_id': 'object',
+        'user': 'V1projectsprojectIdUuidroleusersuserUserIdUuidUser'
     }
 
     attribute_map = {
-        'user': 'user',
-        'mask': 'mask'
+        'workspace_id': 'workspaceId',
+        'user': 'user'
     }
 
-    def __init__(self, user=None, mask=None):  # noqa: E501
-        """UsersUserIdUuidBody - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, workspace_id=None, user=None):  # noqa: E501
+        """UsersUserUserIdUuidBody1 - a model defined in Swagger"""  # noqa: E501
+        self._workspace_id = None
         self._user = None
-        self._mask = None
         self.discriminator = None
+        if workspace_id is not None:
+            self.workspace_id = workspace_id
         if user is not None:
             self.user = user
-        if mask is not None:
-            self.mask = mask
 
     @property
-    def user(self):
-        """Gets the user of this UsersUserIdUuidBody.  # noqa: E501
+    def workspace_id(self):
+        """Gets the workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
 
+        Unique ID of an object in RIME.  # noqa: E501
 
-        :return: The user of this UsersUserIdUuidBody.  # noqa: E501
-        :rtype: V1usersuserIdUuidUser
+        :return: The workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :rtype: object
         """
-        return self._user
+        return self._workspace_id
 
-    @user.setter
-    def user(self, user):
-        """Sets the user of this UsersUserIdUuidBody.
+    @workspace_id.setter
+    def workspace_id(self, workspace_id):
+        """Sets the workspace_id of this UsersUserUserIdUuidBody1.
 
+        Unique ID of an object in RIME.  # noqa: E501
 
-        :param user: The user of this UsersUserIdUuidBody.  # noqa: E501
-        :type: V1usersuserIdUuidUser
+        :param workspace_id: The workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :type: object
         """
 
-        self._user = user
+        self._workspace_id = workspace_id
 
     @property
-    def mask(self):
-        """Gets the mask of this UsersUserIdUuidBody.  # noqa: E501
+    def user(self):
+        """Gets the user of this UsersUserUserIdUuidBody1.  # noqa: E501
 
 
-        :return: The mask of this UsersUserIdUuidBody.  # noqa: E501
-        :rtype: RimeUserWriteMask
+        :return: The user of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :rtype: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
         """
-        return self._mask
+        return self._user
 
-    @mask.setter
-    def mask(self, mask):
-        """Sets the mask of this UsersUserIdUuidBody.
+    @user.setter
+    def user(self, user):
+        """Sets the user of this UsersUserUserIdUuidBody1.
 
 
-        :param mask: The mask of this UsersUserIdUuidBody.  # noqa: E501
-        :type: RimeUserWriteMask
+        :param user: The user of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :type: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
         """
 
-        self._mask = mask
+        self._user = user
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UsersUserIdUuidBody, dict):
+        if issubclass(UsersUserUserIdUuidBody1, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UsersUserIdUuidBody):
+        if not isinstance(other, UsersUserUserIdUuidBody1):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,89 +11,89 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UsersUserUserIdUuidBody1(object):
+class V1projectsprojectIdUuidroleusersuserUserIdUuidUser(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'workspace_id': 'object',
-        'user': 'V1projectsprojectIdUuidroleusersuserUserIdUuidUser'
+        'user_id': 'object',
+        'user_role': 'RimeActorRole'
     }
 
     attribute_map = {
-        'workspace_id': 'workspaceId',
-        'user': 'user'
+        'user_id': 'userId',
+        'user_role': 'userRole'
     }
 
-    def __init__(self, workspace_id=None, user=None):  # noqa: E501
-        """UsersUserUserIdUuidBody1 - a model defined in Swagger"""  # noqa: E501
-        self._workspace_id = None
-        self._user = None
+    def __init__(self, user_id=None, user_role=None):  # noqa: E501
+        """V1projectsprojectIdUuidroleusersuserUserIdUuidUser - a model defined in Swagger"""  # noqa: E501
+        self._user_id = None
+        self._user_role = None
         self.discriminator = None
-        if workspace_id is not None:
-            self.workspace_id = workspace_id
-        if user is not None:
-            self.user = user
+        if user_id is not None:
+            self.user_id = user_id
+        if user_role is not None:
+            self.user_role = user_role
 
     @property
-    def workspace_id(self):
-        """Gets the workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
+    def user_id(self):
+        """Gets the user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
 
         Unique ID of an object in RIME.  # noqa: E501
 
-        :return: The workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :return: The user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
         :rtype: object
         """
-        return self._workspace_id
+        return self._user_id
 
-    @workspace_id.setter
-    def workspace_id(self, workspace_id):
-        """Sets the workspace_id of this UsersUserUserIdUuidBody1.
+    @user_id.setter
+    def user_id(self, user_id):
+        """Sets the user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.
 
         Unique ID of an object in RIME.  # noqa: E501
 
-        :param workspace_id: The workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :param user_id: The user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
         :type: object
         """
 
-        self._workspace_id = workspace_id
+        self._user_id = user_id
 
     @property
-    def user(self):
-        """Gets the user of this UsersUserUserIdUuidBody1.  # noqa: E501
+    def user_role(self):
+        """Gets the user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
 
 
-        :return: The user of this UsersUserUserIdUuidBody1.  # noqa: E501
-        :rtype: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
+        :return: The user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
+        :rtype: RimeActorRole
         """
-        return self._user
+        return self._user_role
 
-    @user.setter
-    def user(self, user):
-        """Sets the user of this UsersUserUserIdUuidBody1.
+    @user_role.setter
+    def user_role(self, user_role):
+        """Sets the user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.
 
 
-        :param user: The user of this UsersUserUserIdUuidBody1.  # noqa: E501
-        :type: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
+        :param user_role: The user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
+        :type: RimeActorRole
         """
 
-        self._user = user
+        self._user_role = user_role
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -108,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UsersUserUserIdUuidBody1, dict):
+        if issubclass(V1projectsprojectIdUuidroleusersuserUserIdUuidUser, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -124,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UsersUserUserIdUuidBody1):
+        if not isinstance(other, V1projectsprojectIdUuidroleusersuserUserIdUuidUser):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body1.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body1.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/validate_request_input.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validate_request_input.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/validate_request_output.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validate_request_output.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ValidationValidateModelResponse(object):
+class ValidationValidatePredictionsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -36,84 +36,84 @@
     attribute_map = {
         'is_valid': 'isValid',
         'error_message': 'errorMessage',
         'validation_status': 'validationStatus'
     }
 
     def __init__(self, is_valid=None, error_message=None, validation_status=None):  # noqa: E501
-        """ValidationValidateModelResponse - a model defined in Swagger"""  # noqa: E501
+        """ValidationValidatePredictionsResponse - a model defined in Swagger"""  # noqa: E501
         self._is_valid = None
         self._error_message = None
         self._validation_status = None
         self.discriminator = None
         if is_valid is not None:
             self.is_valid = is_valid
         if error_message is not None:
             self.error_message = error_message
         if validation_status is not None:
             self.validation_status = validation_status
 
     @property
     def is_valid(self):
-        """Gets the is_valid of this ValidationValidateModelResponse.  # noqa: E501
+        """Gets the is_valid of this ValidationValidatePredictionsResponse.  # noqa: E501
 
 
-        :return: The is_valid of this ValidationValidateModelResponse.  # noqa: E501
+        :return: The is_valid of this ValidationValidatePredictionsResponse.  # noqa: E501
         :rtype: bool
         """
         return self._is_valid
 
     @is_valid.setter
     def is_valid(self, is_valid):
-        """Sets the is_valid of this ValidationValidateModelResponse.
+        """Sets the is_valid of this ValidationValidatePredictionsResponse.
 
 
-        :param is_valid: The is_valid of this ValidationValidateModelResponse.  # noqa: E501
+        :param is_valid: The is_valid of this ValidationValidatePredictionsResponse.  # noqa: E501
         :type: bool
         """
 
         self._is_valid = is_valid
 
     @property
     def error_message(self):
-        """Gets the error_message of this ValidationValidateModelResponse.  # noqa: E501
+        """Gets the error_message of this ValidationValidatePredictionsResponse.  # noqa: E501
 
 
-        :return: The error_message of this ValidationValidateModelResponse.  # noqa: E501
+        :return: The error_message of this ValidationValidatePredictionsResponse.  # noqa: E501
         :rtype: str
         """
         return self._error_message
 
     @error_message.setter
     def error_message(self, error_message):
-        """Sets the error_message of this ValidationValidateModelResponse.
+        """Sets the error_message of this ValidationValidatePredictionsResponse.
 
 
-        :param error_message: The error_message of this ValidationValidateModelResponse.  # noqa: E501
+        :param error_message: The error_message of this ValidationValidatePredictionsResponse.  # noqa: E501
         :type: str
         """
 
         self._error_message = error_message
 
     @property
     def validation_status(self):
-        """Gets the validation_status of this ValidationValidateModelResponse.  # noqa: E501
+        """Gets the validation_status of this ValidationValidatePredictionsResponse.  # noqa: E501
 
 
-        :return: The validation_status of this ValidationValidateModelResponse.  # noqa: E501
+        :return: The validation_status of this ValidationValidatePredictionsResponse.  # noqa: E501
         :rtype: RegistryValidityStatus
         """
         return self._validation_status
 
     @validation_status.setter
     def validation_status(self, validation_status):
-        """Sets the validation_status of this ValidationValidateModelResponse.
+        """Sets the validation_status of this ValidationValidatePredictionsResponse.
 
 
-        :param validation_status: The validation_status of this ValidationValidateModelResponse.  # noqa: E501
+        :param validation_status: The validation_status of this ValidationValidatePredictionsResponse.  # noqa: E501
         :type: RegistryValidityStatus
         """
 
         self._validation_status = validation_status
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -132,15 +132,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ValidationValidateModelResponse, dict):
+        if issubclass(ValidationValidatePredictionsResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -148,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ValidationValidateModelResponse):
+        if not isinstance(other, ValidationValidatePredictionsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/swagger/swagger_client/rest.py` & `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/test_batch.py` & `rime_sdk-2.8.0rc6/rime_sdk/test_batch.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk/test_run.py` & `rime_sdk-2.8.0rc6/rime_sdk/test_run.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc4/rime_sdk.egg-info/PKG-INFO` & `rime_sdk-2.8.0rc6/rime_sdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime-sdk
-Version: 2.8.0rc4
+Version: 2.8.0rc6
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.8.0rc4/rime_sdk.egg-info/SOURCES.txt` & `rime_sdk-2.8.0rc6/rime_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 rime_sdk/swagger/swagger_client/api/schedule_service_api.py
 rime_sdk/swagger/swagger_client/api/user_api.py
 rime_sdk/swagger/swagger_client/api/validation_service_api.py
 rime_sdk/swagger/swagger_client/api/workspace_service_api.py
 rime_sdk/swagger/swagger_client/models/__init__.py
 rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body.py
 rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body1.py
+rime_sdk/swagger/swagger_client/models/apigenerativefirewall_standard_info.py
 rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
 rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
 rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
 rime_sdk/swagger/swagger_client/models/config_generation_category_config_generation_service_response.py
 rime_sdk/swagger/swagger_client/models/config_generation_profiling_config_generation_service_response.py
 rime_sdk/swagger/swagger_client/models/config_generation_test_suite_config_generation_service_response.py
 rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
@@ -126,15 +127,14 @@
 rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
 rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
 rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
 rime_sdk/swagger/swagger_client/models/firewallinstance_firewall_instance_firewall_instance_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/flagged_substring_request_body_component.py
 rime_sdk/swagger/swagger_client/models/generative_testing_result_example.py
-rime_sdk/swagger/swagger_client/models/generative_testing_result_standard_info.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_request.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_response.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_custom_pii_entity.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_denial_of_service_rule_config.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_info.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_status.py
@@ -158,17 +158,17 @@
 rime_sdk/swagger/swagger_client/models/generativefirewall_rule_sensitivity.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_detection_details.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_unknown_external_source_rule_config.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_update_firewall_instance_response.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_validate_response.py
 rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result.py
+rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result_standard_info.py
 rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_request_query.py
 rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_response.py
-rime_sdk/swagger/swagger_client/models/generativetesting_model_connection_spec.py
 rime_sdk/swagger/swagger_client/models/generativetesting_objective_sub_category.py
 rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_request.py
 rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_response.py
 rime_sdk/swagger/swagger_client/models/googlerpc_status.py
 rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
 rime_sdk/swagger/swagger_client/models/integration_integration_level.py
@@ -260,15 +260,14 @@
 rime_sdk/swagger/swagger_client/models/registry_data_params.py
 rime_sdk/swagger/swagger_client/models/registry_data_type.py
 rime_sdk/swagger/swagger_client/models/registry_databricks_info.py
 rime_sdk/swagger/swagger_client/models/registry_generative_language_model_info.py
 rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
 rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
 rime_sdk/swagger/swagger_client/models/registry_metadata.py
-rime_sdk/swagger/swagger_client/models/registry_model_info.py
 rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
 rime_sdk/swagger/swagger_client/models/registry_open_ai_chat_completion_model_info.py
 rime_sdk/swagger/swagger_client/models/registry_pred_info.py
 rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
 rime_sdk/swagger/swagger_client/models/registry_validity_status.py
 rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
 rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
@@ -326,14 +325,15 @@
 rime_sdk/swagger/swagger_client/models/rime_detailed_upgrade_status.py
 rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
 rime_sdk/swagger/swagger_client/models/rime_failing_row.py
 rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
 rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
 rime_sdk/swagger/swagger_client/models/rime_feature_type.py
 rime_sdk/swagger/swagger_client/models/rime_float_list.py
+rime_sdk/swagger/swagger_client/models/rime_generative_model_test_progress.py
 rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_request.py
 rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
@@ -487,27 +487,30 @@
 rime_sdk/swagger/swagger_client/models/rime_workspace.py
 rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
 rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py
 rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
 rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
 rime_sdk/swagger/swagger_client/models/role_users_body.py
 rime_sdk/swagger/swagger_client/models/role_workspace_body.py
+rime_sdk/swagger/swagger_client/models/rule_output_rule_evaluation_metadata.py
+rime_sdk/swagger/swagger_client/models/rule_output_rule_evaluation_metadata_model_info.py
 rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
 rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
 rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
 rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
 rime_sdk/swagger/swagger_client/models/schedule_id_uuid_activate_body.py
 rime_sdk/swagger/swagger_client/models/schedule_id_uuid_deactivate_body.py
 rime_sdk/swagger/swagger_client/models/schedule_schedule.py
 rime_sdk/swagger/swagger_client/models/schedules_schedule_schedule_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
 rime_sdk/swagger/swagger_client/models/schemafilescanning_package_type.py
 rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
 rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
 rime_sdk/swagger/swagger_client/models/schemanotification_config.py
+rime_sdk/swagger/swagger_client/models/schemaregistry_model_info.py
 rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
 rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
 rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
 rime_sdk/swagger/swagger_client/models/statedb_job_status.py
 rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
 rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
 rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
@@ -564,12 +567,14 @@
 rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
 rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
 rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
 rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body1.py
 rime_sdk/swagger/swagger_client/models/validate_request_input.py
 rime_sdk/swagger/swagger_client/models/validate_request_output.py
+rime_sdk/swagger/swagger_client/models/validate_response_processed_request.py
+rime_sdk/swagger/swagger_client/models/validate_response_product_metadata.py
 rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py
 rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py
 rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py
 rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
 rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
```

### Comparing `rime_sdk-2.8.0rc4/setup.py` & `rime_sdk-2.8.0rc6/setup.py`

 * *Files identical despite different names*

