# Comparing `tmp/rime_sdk-2.8.0rc6.tar.gz` & `tmp/rime_sdk-2.8.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rime_sdk-2.8.0rc6.tar", last modified: Thu Apr 18 17:21:20 2024, max compression
+gzip compressed data, was "rime_sdk-2.8.0rc7.tar", last modified: Wed Apr 24 05:55:42 2024, max compression
```

## Comparing `rime_sdk-2.8.0rc6.tar` & `rime_sdk-2.8.0rc7.tar`

### file list

```diff
@@ -1,590 +1,600 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 17:21:20.224007 rime_sdk-2.8.0rc6/
--rw-r--r--   0 runner    (1001) runner    (1001)      566 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/LICENSE
--rw-r--r--   0 runner    (1001) runner    (1001)     1275 2024-04-18 17:21:20.224007 rime_sdk-2.8.0rc6/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      984 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/README.md
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 17:21:20.196007 rime_sdk-2.8.0rc6/rime_sdk/
--rw-r--r--   0 runner    (1001) runner    (1001)     1490 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2268 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/authenticator.py
--rw-r--r--   0 runner    (1001) runner    (1001)    71496 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/client.py
--rw-r--r--   0 runner    (1001) runner    (1001)    23353 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/continuous_test.py
--rw-r--r--   0 runner    (1001) runner    (1001)    12282 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/data_collector.py
--rw-r--r--   0 runner    (1001) runner    (1001)      883 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/detection_event.py
--rw-r--r--   0 runner    (1001) runner    (1001)    25617 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/generative_firewall.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3315 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/generative_model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4892 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/image_builder.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 17:21:20.196007 rime_sdk-2.8.0rc6/rime_sdk/internal/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/internal/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18386 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/internal/config_parser.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1004 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/internal/constants.py
--rw-r--r--   0 runner    (1001) runner    (1001)      667 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/internal/decorators.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9740 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/internal/file_upload.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1973 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/internal/rest_error_handler.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9361 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/internal/swagger_parser.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2577 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/internal/swagger_utils.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1081 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/internal/test_helpers.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2681 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/internal/throttle_queue.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3570 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/internal/utils.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18764 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/job.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5042 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/monitor.py
--rw-r--r--   0 runner    (1001) runner    (1001)   107184 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/project.py
--rw-r--r--   0 runner    (1001) runner    (1001)    38328 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/registry.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4396 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/schedule.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 17:21:20.196007 rime_sdk-2.8.0rc6/rime_sdk/swagger/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 17:21:20.196007 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/
--rw-r--r--   0 runner    (1001) runner    (1001)    60015 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 17:21:20.200008 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/
--rw-r--r--   0 runner    (1001) runner    (1001)     2411 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)    46640 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5851 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/config_validator_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18207 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    25430 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/data_collector_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11733 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/detection_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    23108 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13964 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    27750 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/file_upload_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    24169 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/firewall_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    23787 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/firewall_instance_manager_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    22695 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    15676 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/generative_model_testing_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    28916 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/image_registry_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    27170 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/integration_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    27728 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/job_reader_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    21865 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18441 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/model_testing_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    35026 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    19932 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    74338 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/project_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    57883 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/registry_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    77856 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/results_reader_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4167 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/rime_info_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18249 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/schedule_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    40655 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/user_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    25780 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/validation_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    46472 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    25179 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8845 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 17:21:20.224007 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/
--rw-r--r--   0 runner    (1001) runner    (1001)    57505 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4210 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4369 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body1.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3366 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/apigenerativefirewall_standard_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4328 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6669 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5483 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5103 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/config_generation_category_config_generation_service_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3706 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/config_generation_profiling_config_generation_service_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3725 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/config_generation_test_suite_config_generation_service_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3435 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8968 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3552 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4503 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3582 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2551 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6687 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
--rw-r--r--   0 runner    (1001) runner    (1001)    17329 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/crossplanetask_cross_plane_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3362 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8011 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4630 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2674 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2695 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7390 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4396 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3292 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6273 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13500 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8080 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4925 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5748 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2705 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5806 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)    14085 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8545 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3410 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)    15539 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4273 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2728 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_event_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2587 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4205 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_resolution.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7745 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2744 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2719 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2670 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4176 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10779 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10808 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_file_security_report.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7556 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_package_url.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7459 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3304 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata_license.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3285 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/fileserver_check_object_exists_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/fileserver_delete_object_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3294 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/fileserver_get_read_object_presigned_link_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3310 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/fileserver_get_upload_object_presigned_link_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3232 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/fileserver_list_objects_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9982 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5075 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3149 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10070 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5158 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6961 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewallinstance_firewall_instance_firewall_instance_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2822 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/flagged_substring_request_body_component.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4455 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generative_testing_result_example.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4502 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3679 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5387 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_custom_pii_entity.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4675 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_denial_of_service_rule_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2722 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6459 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2844 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5781 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3291 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2896 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_tokenizer.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6773 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_flagged_substring.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3517 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_effective_config_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3686 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_instance_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11464 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_individual_rules_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4144 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3934 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_rule_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3740 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_list_firewall_instances_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8681 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_off_topic_rule_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4848 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4877 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_rule_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3752 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_entity_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3712 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3487 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_v2_rule_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11874 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_output.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2808 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_sensitivity.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3447 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_detection_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5128 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_unknown_external_source_rule_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3869 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_update_firewall_instance_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5046 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7846 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13957 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3518 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result_standard_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2667 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_request_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5869 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4012 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_objective_sub_category.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9383 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3408 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4422 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4103 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2821 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2770 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3403 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3206 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2808 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4550 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5064 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4141 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/job_data_generative_model_test.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3915 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/job_data_scan.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4710 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4752 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/language_detection_details_language_substring.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4794 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4426 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4187 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_file_scan_results_request_file_scan_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4033 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6007 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5102 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5050 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4570 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3633 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6549 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4842 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4373 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3722 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5728 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5076 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3993 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4508 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2674 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13223 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/model_model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3523 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4142 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2745 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2515 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6262 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4125 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3518 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4963 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)    12705 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2665 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4511 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2667 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3520 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_transform.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2728 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4020 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5602 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3275 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9399 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_notification.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2774 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2644 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_object_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3594 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4781 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6823 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/pii_detection_details_flagged_entity.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4341 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4384 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_activate_schedule_for_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2563 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11026 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3279 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2607 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_deactivate_schedule_for_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2547 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3288 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3190 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4530 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9270 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10554 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)    12754 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5306 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5738 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3739 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_owner_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)    19393 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_project.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2693 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_project_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5013 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_project_with_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2579 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4180 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_schedule_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3279 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2571 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4380 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4765 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2715 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/protobuf_any.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2574 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6648 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_connection_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3375 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4050 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4143 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6599 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)    20609 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_params.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2624 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3454 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4688 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_generative_language_model_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5621 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4998 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4224 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_metadata.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3453 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3654 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_open_ai_chat_completion_model_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4161 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_pred_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5645 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2728 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13267 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3218 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5797 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/repo_metadata_reputation.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5037 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2753 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2559 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8702 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5337 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent_desired_state.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2745 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8524 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2775 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_attack_objective.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2519 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6159 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13366 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2860 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_config_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4337 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3505 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3389 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4997 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6566 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4077 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6407 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3976 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3303 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3478 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3486 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7059 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3324 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6750 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3842 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3407 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3481 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4086 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3371 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7230 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3177 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5393 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_schedule_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3324 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_schedule_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5936 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3212 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7061 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3352 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2559 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2535 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2539 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2551 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3371 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2559 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2539 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_schedule_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2567 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5159 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_detailed_upgrade_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2563 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4600 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6332 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6606 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3344 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3130 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_float_list.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3469 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_generative_model_test_progress.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3160 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3462 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3357 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4523 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6063 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3231 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4115 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3631 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3396 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3501 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_file_scan_result_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3265 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3181 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3457 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3122 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3266 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3394 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3365 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3303 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5967 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6275 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3208 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8929 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3381 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3406 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3288 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8541 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4079 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_schedule_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3292 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8955 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_time_series_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4877 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_upgrade_for_agent_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3110 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3147 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4256 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4226 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4316 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3284 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2519 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4368 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3108 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_int_list.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4063 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6446 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_data.py
--rw-r--r--   0 runner    (1001) runner    (1001)    14784 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2865 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2617 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_view.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2611 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_language.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2904 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2770 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5439 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2672 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4968 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4995 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3283 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4835 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11090 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5364 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4580 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5385 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5847 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4070 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7152 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5064 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4682 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3431 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4796 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5011 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5555 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5033 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4139 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3335 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5758 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2535 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4727 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3583 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4904 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3855 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
--rw-r--r--   0 runner    (1001) runner    (1001)    12972 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2701 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image_package_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2784 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3900 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_card.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3127 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_task.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4059 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4134 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3697 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_named_double.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2620 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_order.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4197 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3415 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4616 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4108 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3320 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4337 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3678 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2575 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2535 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2567 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2691 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2666 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3126 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3976 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_search_spec.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2654 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_severity.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5062 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3831 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3226 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5586 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3178 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3194 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5016 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3304 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4870 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3288 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5859 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3336 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3390 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4438 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2547 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3108 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_str_list.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3289 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2741 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3134 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3854 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4448 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_table_column.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2768 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5133 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2718 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9660 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3423 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4811 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2869 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2652 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3911 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2698 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_token_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3172 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_toxicity_threat_category.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5196 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3289 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3481 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3327 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3255 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3425 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3289 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_schedule_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2591 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_upgrade_status_for_agent_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2567 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2523 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2531 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_upgrade_agent_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3156 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_upgrade_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4875 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5335 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_role.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3886 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6815 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3106 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_uuid.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7431 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_workspace.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7167 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7715 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2841 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4741 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4096 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/role_users_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4673 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3900 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rule_output_rule_evaluation_metadata.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3469 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rule_output_rule_evaluation_metadata_model_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4098 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4401 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4797 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6378 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4295 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_activate_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4319 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_deactivate_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6026 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schedule_schedule.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6508 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schedules_schedule_schedule_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6690 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2948 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemafilescanning_package_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5053 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4051 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5310 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6171 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemaregistry_model_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4156 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2790 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3993 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2803 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4121 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4121 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4136 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7276 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6259 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4371 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4136 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4187 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10280 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6416 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
--rw-r--r--   0 runner    (1001) runner    (1001)    12809 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4278 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5610 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3485 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9333 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4444 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2764 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6759 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3436 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3799 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_category_results_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3538 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3641 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3358 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5680 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5790 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3496 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5835 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5553 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5086 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5530 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3520 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3382 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6503 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
--rw-r--r--   0 runner    (1001) runner    (1001)    16800 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7005 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13296 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5304 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13655 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4663 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
--rw-r--r--   0 runner    (1001) runner    (1001)    19373 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11743 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4077 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3410 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/user_private_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2634 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/user_role.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7844 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/user_user_detail.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3815 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4140 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4196 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8329 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4326 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13843 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11044 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10263 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4396 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8198 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8401 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5364 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5380 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body1.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4825 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validate_request_input.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3641 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validate_request_output.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10037 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validate_response_processed_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5992 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validate_response_product_metadata.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5905 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5093 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5189 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4338 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4533 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13063 2024-04-18 17:21:19.000000 rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/rest.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5257 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/test_batch.py
--rw-r--r--   0 runner    (1001) runner    (1001)    17414 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/rime_sdk/test_run.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 17:21:20.196007 rime_sdk-2.8.0rc6/rime_sdk.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)     1275 2024-04-18 17:21:20.000000 rime_sdk-2.8.0rc6/rime_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)    40697 2024-04-18 17:21:20.000000 rime_sdk-2.8.0rc6/rime_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-04-18 17:21:20.000000 rime_sdk-2.8.0rc6/rime_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       80 2024-04-18 17:21:20.000000 rime_sdk-2.8.0rc6/rime_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) runner    (1001)      161 2024-04-18 17:21:20.000000 rime_sdk-2.8.0rc6/rime_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        9 2024-04-18 17:21:20.000000 rime_sdk-2.8.0rc6/rime_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-04-18 17:21:20.224007 rime_sdk-2.8.0rc6/setup.cfg
--rw-r--r--   0 runner    (1001) runner    (1001)     3903 2024-04-18 17:19:44.000000 rime_sdk-2.8.0rc6/setup.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-24 05:55:42.516008 rime_sdk-2.8.0rc7/
+-rw-r--r--   0 runner    (1001) runner    (1001)      566 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/LICENSE
+-rw-r--r--   0 runner    (1001) runner    (1001)     1275 2024-04-24 05:55:42.516008 rime_sdk-2.8.0rc7/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      984 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/README.md
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-24 05:55:42.480008 rime_sdk-2.8.0rc7/rime_sdk/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1490 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2268 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/authenticator.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    71496 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/client.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    23353 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/continuous_test.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12282 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/data_collector.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      883 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/detection_event.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    25623 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/generative_firewall.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3437 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/generative_model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4892 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/image_builder.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-24 05:55:42.484007 rime_sdk-2.8.0rc7/rime_sdk/internal/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/internal/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18386 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/internal/config_parser.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1004 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/internal/constants.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      667 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/internal/decorators.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9740 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/internal/file_upload.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1973 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/internal/rest_error_handler.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9361 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/internal/swagger_parser.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2577 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/internal/swagger_utils.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1081 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/internal/test_helpers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2681 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/internal/throttle_queue.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3570 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/internal/utils.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18764 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5042 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/monitor.py
+-rw-r--r--   0 runner    (1001) runner    (1001)   107184 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    38328 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/registry.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4396 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/schedule.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-24 05:55:42.484007 rime_sdk-2.8.0rc7/rime_sdk/swagger/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-24 05:55:42.484007 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/
+-rw-r--r--   0 runner    (1001) runner    (1001)    61236 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-24 05:55:42.484007 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/
+-rw-r--r--   0 runner    (1001) runner    (1001)     2411 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    60690 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5851 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/config_validator_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18207 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    25430 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/data_collector_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11733 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/detection_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    23108 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13964 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    27750 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/file_upload_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    24169 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/firewall_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    23796 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/firewall_instance_manager_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    22695 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    15676 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/generative_model_testing_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    28916 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/image_registry_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    27170 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/integration_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    27728 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/job_reader_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    21865 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18441 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/model_testing_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    35026 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    19932 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    74338 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/project_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    57883 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/registry_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    77856 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/results_reader_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4167 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/rime_info_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18249 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/schedule_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    40655 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/user_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    25780 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/validation_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    46472 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    25179 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8845 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-24 05:55:42.516008 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/
+-rw-r--r--   0 runner    (1001) runner    (1001)    58726 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4210 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4369 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body1.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3764 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/apigenerativefirewall_list_firewall_instances_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3366 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/apigenerativefirewall_standard_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4328 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6669 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5483 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5103 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/config_generation_category_config_generation_service_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3706 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/config_generation_profiling_config_generation_service_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3725 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/config_generation_test_suite_config_generation_service_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3435 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8968 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3552 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4503 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3582 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2551 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6687 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    17329 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/crossplanetask_cross_plane_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3362 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8011 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4630 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2674 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2695 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7390 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4396 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3292 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6273 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13500 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8080 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4925 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5748 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2705 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5806 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    14085 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8545 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3410 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    15539 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4273 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2728 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/detection_event_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2587 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4205 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/detection_resolution.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7745 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2744 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2719 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2670 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4176 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10779 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10808 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_file_security_report.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7556 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_package_url.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7459 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3304 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata_license.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3285 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/fileserver_check_object_exists_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/fileserver_delete_object_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3294 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/fileserver_get_read_object_presigned_link_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3310 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/fileserver_get_upload_object_presigned_link_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3232 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/fileserver_list_objects_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9982 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5075 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3149 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10070 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5158 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7816 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/firewallinstance_firewall_instance_firewall_instance_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2822 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/flagged_substring_request_body_component.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4455 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generative_testing_result_example.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4502 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3679 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5387 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_custom_pii_entity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4675 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_denial_of_service_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2722 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7234 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2844 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5781 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3291 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2896 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_tokenizer.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6773 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_flagged_substring.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3517 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_effective_config_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3686 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_instance_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13926 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_individual_rules_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4144 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3934 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8681 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_off_topic_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4848 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4877 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3752 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_entity_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4895 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5039 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_v2_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2924 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_false_positive_rate.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11874 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_output.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2808 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_sensitivity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3447 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_detection_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3934 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5128 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_unknown_external_source_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3869 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_update_firewall_instance_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5046 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7846 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    14746 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3518 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result_standard_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2667 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_request_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5869 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4012 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativetesting_objective_sub_category.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10258 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3408 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3157 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativetesting_threat.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4422 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4103 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2821 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2770 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3403 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3206 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2808 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4550 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5064 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4774 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/job_data_generative_model_test.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3915 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/job_data_scan.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4710 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4752 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/language_detection_details_language_substring.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5481 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4426 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4187 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_file_scan_results_request_file_scan_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3771 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_firewall_instances_request_list_firewall_instances_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4033 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6007 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5102 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5050 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4570 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3633 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6549 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4842 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4373 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3722 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5728 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5076 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3993 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4508 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2674 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13223 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/model_model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3523 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4142 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2745 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2515 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6262 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4125 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3518 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4963 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12705 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2665 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4511 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2667 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3520 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_transform.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2728 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4020 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5602 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3275 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9399 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/notification_notification.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2774 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2644 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/notification_object_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3594 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4781 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6823 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/pii_detection_details_flagged_entity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4341 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4384 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_activate_schedule_for_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2563 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11026 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3279 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2607 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_deactivate_schedule_for_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2547 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3288 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3190 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4530 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9270 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10554 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12754 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5306 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5738 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3739 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_owner_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    19393 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2693 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_project_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5013 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_project_with_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2579 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4180 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_schedule_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3279 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2571 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4380 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4765 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2715 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/protobuf_any.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2574 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6648 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_connection_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3375 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4050 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4143 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_data_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6599 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    20609 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_data_params.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2624 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_data_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3454 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4688 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_generative_language_model_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5621 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4998 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4224 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_metadata.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3453 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3654 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_open_ai_chat_completion_model_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4161 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_pred_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5645 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2728 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13267 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3218 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5797 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/repo_metadata_reputation.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5037 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2753 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2559 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9297 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_agent.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5337 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_agent_desired_state.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2745 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2606 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_agent_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8524 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2775 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_attack_objective.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2519 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6159 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13366 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2860 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_config_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4337 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3505 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3389 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4997 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6566 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4077 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6407 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3976 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3303 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3478 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3486 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3314 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_firewall_agent_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4200 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_firewall_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7059 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3324 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6750 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3842 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3407 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3481 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4086 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3371 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7230 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3177 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5393 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_schedule_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3324 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_schedule_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5936 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3212 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7061 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3352 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2559 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2535 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2539 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2551 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3371 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2559 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2539 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_schedule_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2567 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5159 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_detailed_upgrade_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2563 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4600 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6332 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6606 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3344 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3130 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_float_list.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3469 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_generative_model_test_progress.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3160 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3462 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3357 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4523 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6063 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3231 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4115 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3631 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3396 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3501 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_file_scan_result_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3265 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3181 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3457 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3122 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3266 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3394 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3365 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3303 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5967 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6275 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3208 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8929 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3381 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3406 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3288 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8541 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4079 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_schedule_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3292 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8955 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_time_series_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4877 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_upgrade_for_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3110 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3147 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4256 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4226 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4316 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3284 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2519 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4368 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3108 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_int_list.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4063 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6446 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_data.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    14784 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2865 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2617 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_view.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2611 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_language.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2904 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2770 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5439 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2672 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4968 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4995 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3283 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4835 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11090 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5364 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4580 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5385 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5366 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_firewall_instances_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5847 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4070 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7152 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5064 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4682 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3431 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4796 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5011 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5555 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5033 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4139 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3335 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5758 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2535 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4727 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3583 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4904 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3855 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12972 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2701 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_managed_image_package_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2784 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3900 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_model_card.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3127 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_model_task.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4059 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4134 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3697 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_named_double.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2620 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_order.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4197 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3415 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4616 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4108 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3464 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_firewall_agent_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3623 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_firewall_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3320 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4337 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3678 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2575 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2535 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2567 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2691 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2666 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3126 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3976 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_search_spec.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2654 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_severity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5062 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3831 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3226 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5586 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3178 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3194 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5016 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3304 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4870 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3288 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5859 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3336 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3390 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4438 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2547 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3108 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_str_list.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3289 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2741 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3134 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3854 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4448 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_table_column.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2768 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5133 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2718 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9660 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3423 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4811 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2869 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2652 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3911 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2698 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_token_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3172 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_toxicity_threat_category.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5196 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3289 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3481 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3327 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3255 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3425 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3289 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_schedule_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2591 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_upgrade_status_for_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2567 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2523 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2531 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_upgrade_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3156 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_upgrade_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4875 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5335 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_role.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3886 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6815 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3106 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_uuid.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7431 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_workspace.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7167 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7715 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2841 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4741 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4096 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/role_users_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4673 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3900 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rule_output_rule_evaluation_metadata.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3469 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rule_output_rule_evaluation_metadata_model_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4098 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4401 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4797 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6378 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4295 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_activate_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4319 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_deactivate_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6026 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/schedule_schedule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6508 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/schedules_schedule_schedule_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6690 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2948 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/schemafilescanning_package_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5053 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4051 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5310 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6171 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/schemaregistry_model_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4156 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2790 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3993 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2803 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4121 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4121 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4136 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7276 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6259 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4371 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4136 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4187 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10280 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6416 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12809 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4278 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5610 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3485 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9333 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4444 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2764 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6759 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3436 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3799 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_category_results_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3538 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3641 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3358 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5680 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5790 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3496 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5835 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5553 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5086 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5530 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3520 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3382 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6503 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    16800 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7005 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13296 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5304 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13655 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4663 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    19373 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11743 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4077 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3410 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/user_private_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2634 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/user_role.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7844 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/user_user_detail.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3815 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4140 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4196 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8329 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4326 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13843 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11044 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10263 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4396 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8198 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8401 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5364 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5380 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body1.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4825 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/validate_request_input.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3641 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/validate_request_output.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9852 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/validate_response_processed_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5992 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/validate_response_product_metadata.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5905 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5093 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5189 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4338 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4533 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13063 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/rest.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5257 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/test_batch.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    17414 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/rime_sdk/test_run.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-24 05:55:42.480008 rime_sdk-2.8.0rc7/rime_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1275 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)    41491 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       80 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)      161 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        9 2024-04-24 05:55:42.000000 rime_sdk-2.8.0rc7/rime_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-04-24 05:55:42.516008 rime_sdk-2.8.0rc7/setup.cfg
+-rw-r--r--   0 runner    (1001) runner    (1001)     3903 2024-04-24 05:54:00.000000 rime_sdk-2.8.0rc7/setup.py
```

### Comparing `rime_sdk-2.8.0rc6/LICENSE` & `rime_sdk-2.8.0rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/PKG-INFO` & `rime_sdk-2.8.0rc7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime_sdk
-Version: 2.8.0rc6
+Version: 2.8.0rc7
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.8.0rc6/README.md` & `rime_sdk-2.8.0rc7/README.md`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/__init__.py` & `rime_sdk-2.8.0rc7/rime_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/authenticator.py` & `rime_sdk-2.8.0rc7/rime_sdk/authenticator.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/client.py` & `rime_sdk-2.8.0rc7/rime_sdk/client.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/continuous_test.py` & `rime_sdk-2.8.0rc7/rime_sdk/continuous_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/data_collector.py` & `rime_sdk-2.8.0rc7/rime_sdk/data_collector.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/detection_event.py` & `rime_sdk-2.8.0rc7/rime_sdk/detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/generative_firewall.py` & `rime_sdk-2.8.0rc7/rime_sdk/generative_firewall.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 
 from rime_sdk.authenticator import Authenticator
 from rime_sdk.client import RETRY_HTTP_STATUS
 from rime_sdk.internal.rest_error_handler import RESTErrorHandler
 from rime_sdk.internal.utils import is_positive_number, remove_null_values_from_dict
 from rime_sdk.swagger.swagger_client import (
     ApiClient,
+    ApigenerativefirewallListFirewallInstancesResponse,
     Configuration,
     FirewallApi,
     FirewallinstanceFirewallInstanceFirewallInstanceIdUuidBody,
     FirewallInstanceManagerApi,
     GenerativefirewallCreateFirewallInstanceRequest,
     GenerativefirewallCreateFirewallInstanceResponse,
     GenerativefirewallFirewallInstanceInfo,
     GenerativefirewallFirewallInstanceStatus,
     GenerativefirewallFirewallRuleConfig,
     GenerativefirewallGetFirewallEffectiveConfigResponse,
     GenerativefirewallGetFirewallInstanceResponse,
-    GenerativefirewallListFirewallInstancesResponse,
     GenerativefirewallValidateRequest,
     ValidateRequestInput,
     ValidateRequestOutput,
 )
 from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_rule_type import (
     GenerativefirewallFirewallRuleType,
 )
@@ -518,15 +518,15 @@
             self._api_client.configuration.api_key[
                 "X-Firewall-Auth-Token"
             ] = file1.read()
 
     def list_firewall_instances(self) -> Iterable[FirewallInstance]:
         """List the FirewallInstances for the given cluster."""
         with RESTErrorHandler():
-            res: GenerativefirewallListFirewallInstancesResponse = (
+            res: ApigenerativefirewallListFirewallInstancesResponse = (
                 self._instance_manager_client.firewall_instance_manager_list_firewall_instances()
             )
             firewall_instances: List[
                 GenerativefirewallFirewallInstanceInfo
             ] = res.firewall_instances
             for fwinfo in firewall_instances:
                 yield FirewallInstance(
```

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/generative_model.py` & `rime_sdk-2.8.0rc7/rime_sdk/generative_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,31 +26,34 @@
 
     def start_test(
         self,
         url: str,
         endpoint_payload_template: str,
         response_json_path: str,
         http_headers: Optional[dict] = None,
+        name: Optional[str] = None,
     ) -> GenerativeModelTestJob:
         """Start a Generative Model Test.
 
         Args:
             url: The URL to test.
             http_headers: The HTTP headers to use.
             endpoint_payload_template: The endpoint payload template to use.
             response_json_path: The response JSON path to use.
+            name: A name to identify your generative test run.
 
         Returns:
             GenerativeModelTestJob: The Generative Model Test Job.
         """
         request = GenerativetestingStartGenerativeModelTestRequest(
             url=url,
             http_headers=http_headers,
             endpoint_payload_template=endpoint_payload_template,
             response_json_path=response_json_path,
+            name=name,
         )
         with RESTErrorHandler():
             res: GenerativetestingStartGenerativeModelTestResponse = (
                 GenerativeModelTestingApi(
                     self._api_client
                 ).generative_model_testing_start_generative_model_test(body=request)
             )
```

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/image_builder.py` & `rime_sdk-2.8.0rc7/rime_sdk/image_builder.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/internal/config_parser.py` & `rime_sdk-2.8.0rc7/rime_sdk/internal/config_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/internal/constants.py` & `rime_sdk-2.8.0rc7/rime_sdk/internal/constants.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/internal/decorators.py` & `rime_sdk-2.8.0rc7/rime_sdk/internal/decorators.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/internal/file_upload.py` & `rime_sdk-2.8.0rc7/rime_sdk/internal/file_upload.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/internal/rest_error_handler.py` & `rime_sdk-2.8.0rc7/rime_sdk/internal/rest_error_handler.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/internal/swagger_parser.py` & `rime_sdk-2.8.0rc7/rime_sdk/internal/swagger_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/internal/swagger_utils.py` & `rime_sdk-2.8.0rc7/rime_sdk/internal/swagger_utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/internal/test_helpers.py` & `rime_sdk-2.8.0rc7/rime_sdk/internal/test_helpers.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/internal/throttle_queue.py` & `rime_sdk-2.8.0rc7/rime_sdk/internal/throttle_queue.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/internal/utils.py` & `rime_sdk-2.8.0rc7/rime_sdk/internal/utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/job.py` & `rime_sdk-2.8.0rc7/rime_sdk/job.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/monitor.py` & `rime_sdk-2.8.0rc7/rime_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/project.py` & `rime_sdk-2.8.0rc7/rime_sdk/project.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/registry.py` & `rime_sdk-2.8.0rc7/rime_sdk/registry.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/schedule.py` & `rime_sdk-2.8.0rc7/rime_sdk/schedule.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/__init__.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 from rime_sdk.swagger.swagger_client.api.workspace_service_api import WorkspaceServiceApi
 # import ApiClient
 from rime_sdk.swagger.swagger_client.api_client import ApiClient
 from rime_sdk.swagger.swagger_client.configuration import Configuration
 # import models into sdk package
 from rime_sdk.swagger.swagger_client.models.agent_id_uuid_upgrade_body import AgentIdUuidUpgradeBody
 from rime_sdk.swagger.swagger_client.models.agent_id_uuid_upgrade_body1 import AgentIdUuidUpgradeBody1
+from rime_sdk.swagger.swagger_client.models.apigenerativefirewall_list_firewall_instances_response import ApigenerativefirewallListFirewallInstancesResponse
 from rime_sdk.swagger.swagger_client.models.apigenerativefirewall_standard_info import ApigenerativefirewallStandardInfo
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_category_test_identifier import ArtifactIdentifierCategoryTestIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_subset_test_metric_identifier import ArtifactIdentifierSubsetTestMetricIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_test_case_metric_identifier import ArtifactIdentifierTestCaseMetricIdentifier
 from rime_sdk.swagger.swagger_client.models.config_generation_category_config_generation_service_response import ConfigGenerationCategoryConfigGenerationServiceResponse
 from rime_sdk.swagger.swagger_client.models.config_generation_profiling_config_generation_service_response import ConfigGenerationProfilingConfigGenerationServiceResponse
 from rime_sdk.swagger.swagger_client.models.config_generation_test_suite_config_generation_service_response import ConfigGenerationTestSuiteConfigGenerationServiceResponse
@@ -121,35 +122,37 @@
 from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_tokenizer import GenerativefirewallFirewallTokenizer
 from rime_sdk.swagger.swagger_client.models.generativefirewall_flagged_substring import GenerativefirewallFlaggedSubstring
 from rime_sdk.swagger.swagger_client.models.generativefirewall_get_firewall_effective_config_response import GenerativefirewallGetFirewallEffectiveConfigResponse
 from rime_sdk.swagger.swagger_client.models.generativefirewall_get_firewall_instance_response import GenerativefirewallGetFirewallInstanceResponse
 from rime_sdk.swagger.swagger_client.models.generativefirewall_individual_rules_config import GenerativefirewallIndividualRulesConfig
 from rime_sdk.swagger.swagger_client.models.generativefirewall_language_detection_details import GenerativefirewallLanguageDetectionDetails
 from rime_sdk.swagger.swagger_client.models.generativefirewall_language_detection_rule_config import GenerativefirewallLanguageDetectionRuleConfig
-from rime_sdk.swagger.swagger_client.models.generativefirewall_list_firewall_instances_response import GenerativefirewallListFirewallInstancesResponse
 from rime_sdk.swagger.swagger_client.models.generativefirewall_off_topic_rule_config import GenerativefirewallOffTopicRuleConfig
 from rime_sdk.swagger.swagger_client.models.generativefirewall_pii_detection_details import GenerativefirewallPiiDetectionDetails
 from rime_sdk.swagger.swagger_client.models.generativefirewall_pii_detection_rule_config import GenerativefirewallPiiDetectionRuleConfig
 from rime_sdk.swagger.swagger_client.models.generativefirewall_pii_entity_type import GenerativefirewallPiiEntityType
 from rime_sdk.swagger.swagger_client.models.generativefirewall_prompt_injection_details import GenerativefirewallPromptInjectionDetails
 from rime_sdk.swagger.swagger_client.models.generativefirewall_prompt_injection_v2_rule_config import GenerativefirewallPromptInjectionV2RuleConfig
+from rime_sdk.swagger.swagger_client.models.generativefirewall_rule_false_positive_rate import GenerativefirewallRuleFalsePositiveRate
 from rime_sdk.swagger.swagger_client.models.generativefirewall_rule_output import GenerativefirewallRuleOutput
 from rime_sdk.swagger.swagger_client.models.generativefirewall_rule_sensitivity import GenerativefirewallRuleSensitivity
 from rime_sdk.swagger.swagger_client.models.generativefirewall_toxicity_detection_details import GenerativefirewallToxicityDetectionDetails
+from rime_sdk.swagger.swagger_client.models.generativefirewall_toxicity_rule_config import GenerativefirewallToxicityRuleConfig
 from rime_sdk.swagger.swagger_client.models.generativefirewall_unknown_external_source_rule_config import GenerativefirewallUnknownExternalSourceRuleConfig
 from rime_sdk.swagger.swagger_client.models.generativefirewall_update_firewall_instance_response import GenerativefirewallUpdateFirewallInstanceResponse
 from rime_sdk.swagger.swagger_client.models.generativefirewall_validate_request import GenerativefirewallValidateRequest
 from rime_sdk.swagger.swagger_client.models.generativefirewall_validate_response import GenerativefirewallValidateResponse
 from rime_sdk.swagger.swagger_client.models.generativetesting_generative_testing_result import GenerativetestingGenerativeTestingResult
 from rime_sdk.swagger.swagger_client.models.generativetesting_generative_testing_result_standard_info import GenerativetestingGenerativeTestingResultStandardInfo
 from rime_sdk.swagger.swagger_client.models.generativetesting_get_generative_model_test_results_request_query import GenerativetestingGetGenerativeModelTestResultsRequestQuery
 from rime_sdk.swagger.swagger_client.models.generativetesting_get_generative_model_test_results_response import GenerativetestingGetGenerativeModelTestResultsResponse
 from rime_sdk.swagger.swagger_client.models.generativetesting_objective_sub_category import GenerativetestingObjectiveSubCategory
 from rime_sdk.swagger.swagger_client.models.generativetesting_start_generative_model_test_request import GenerativetestingStartGenerativeModelTestRequest
 from rime_sdk.swagger.swagger_client.models.generativetesting_start_generative_model_test_response import GenerativetestingStartGenerativeModelTestResponse
+from rime_sdk.swagger.swagger_client.models.generativetesting_threat import GenerativetestingThreat
 from rime_sdk.swagger.swagger_client.models.googlerpc_status import GooglerpcStatus
 from rime_sdk.swagger.swagger_client.models.heartbeat_agent_id_uuid_body import HeartbeatAgentIdUuidBody
 from rime_sdk.swagger.swagger_client.models.image_reference_reference_type import ImageReferenceReferenceType
 from rime_sdk.swagger.swagger_client.models.integration_integration_level import IntegrationIntegrationLevel
 from rime_sdk.swagger.swagger_client.models.integration_integration_schema import IntegrationIntegrationSchema
 from rime_sdk.swagger.swagger_client.models.integration_integration_type import IntegrationIntegrationType
 from rime_sdk.swagger.swagger_client.models.integration_variable_sensitivity import IntegrationVariableSensitivity
@@ -158,14 +161,15 @@
 from rime_sdk.swagger.swagger_client.models.job_data_generative_model_test import JobDataGenerativeModelTest
 from rime_sdk.swagger.swagger_client.models.job_data_scan import JobDataScan
 from rime_sdk.swagger.swagger_client.models.job_data_stress_test import JobDataStressTest
 from rime_sdk.swagger.swagger_client.models.language_detection_details_language_substring import LanguageDetectionDetailsLanguageSubstring
 from rime_sdk.swagger.swagger_client.models.list_agents_request_list_agents_query import ListAgentsRequestListAgentsQuery
 from rime_sdk.swagger.swagger_client.models.list_datasets_request_datasets_query import ListDatasetsRequestDatasetsQuery
 from rime_sdk.swagger.swagger_client.models.list_file_scan_results_request_file_scan_query import ListFileScanResultsRequestFileScanQuery
+from rime_sdk.swagger.swagger_client.models.list_firewall_instances_request_list_firewall_instances_query import ListFirewallInstancesRequestListFirewallInstancesQuery
 from rime_sdk.swagger.swagger_client.models.list_images_request_pip_library_filter import ListImagesRequestPipLibraryFilter
 from rime_sdk.swagger.swagger_client.models.list_metric_identifiers_response_aggregated_metric import ListMetricIdentifiersResponseAggregatedMetric
 from rime_sdk.swagger.swagger_client.models.list_metric_identifiers_response_feature_metric_without_subsets import ListMetricIdentifiersResponseFeatureMetricWithoutSubsets
 from rime_sdk.swagger.swagger_client.models.list_metric_identifiers_response_feature_metrics import ListMetricIdentifiersResponseFeatureMetrics
 from rime_sdk.swagger.swagger_client.models.list_metric_identifiers_response_subset_metric import ListMetricIdentifiersResponseSubsetMetric
 from rime_sdk.swagger.swagger_client.models.list_metric_identifiers_response_subset_metrics import ListMetricIdentifiersResponseSubsetMetrics
 from rime_sdk.swagger.swagger_client.models.list_models_request_model_query import ListModelsRequestModelQuery
@@ -253,14 +257,15 @@
 from rime_sdk.swagger.swagger_client.models.resetpassword_user_id_uuid_body import ResetpasswordUserIdUuidBody
 from rime_sdk.swagger.swagger_client.models.rime_api_token_info import RimeAPITokenInfo
 from rime_sdk.swagger.swagger_client.models.rime_actor_role import RimeActorRole
 from rime_sdk.swagger.swagger_client.models.rime_add_users_to_workspace_response import RimeAddUsersToWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_agent import RimeAgent
 from rime_sdk.swagger.swagger_client.models.rime_agent_desired_state import RimeAgentDesiredState
 from rime_sdk.swagger.swagger_client.models.rime_agent_status import RimeAgentStatus
+from rime_sdk.swagger.swagger_client.models.rime_agent_type import RimeAgentType
 from rime_sdk.swagger.swagger_client.models.rime_attack_objective import RimeAttackObjective
 from rime_sdk.swagger.swagger_client.models.rime_cancel_job_response import RimeCancelJobResponse
 from rime_sdk.swagger.swagger_client.models.rime_category_metric import RimeCategoryMetric
 from rime_sdk.swagger.swagger_client.models.rime_category_test_result import RimeCategoryTestResult
 from rime_sdk.swagger.swagger_client.models.rime_config_type import RimeConfigType
 from rime_sdk.swagger.swagger_client.models.rime_configure_integration_request_integration_variable import RimeConfigureIntegrationRequestIntegrationVariable
 from rime_sdk.swagger.swagger_client.models.rime_configure_integration_response import RimeConfigureIntegrationResponse
@@ -269,14 +274,16 @@
 from rime_sdk.swagger.swagger_client.models.rime_create_api_token_request import RimeCreateAPITokenRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_api_token_response import RimeCreateAPITokenResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_agent_request import RimeCreateAgentRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_agent_response import RimeCreateAgentResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_custom_monitor_response import RimeCreateCustomMonitorResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_customer_managed_key_request import RimeCreateCustomerManagedKeyRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_customer_managed_key_response import RimeCreateCustomerManagedKeyResponse
+from rime_sdk.swagger.swagger_client.models.rime_create_firewall_agent_request import RimeCreateFirewallAgentRequest
+from rime_sdk.swagger.swagger_client.models.rime_create_firewall_agent_response import RimeCreateFirewallAgentResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_firewall_request import RimeCreateFirewallRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_firewall_response import RimeCreateFirewallResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_image_request import RimeCreateImageRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_image_response import RimeCreateImageResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_integration_request import RimeCreateIntegrationRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_integration_response import RimeCreateIntegrationResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_model_card_request import RimeCreateModelCardRequest
@@ -361,14 +368,15 @@
 from rime_sdk.swagger.swagger_client.models.rime_list_agents_response import RimeListAgentsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_current_user_roles_response import RimeListCurrentUserRolesResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_datasets_response import RimeListDatasetsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_detection_events_request_query import RimeListDetectionEventsRequestQuery
 from rime_sdk.swagger.swagger_client.models.rime_list_detection_events_response import RimeListDetectionEventsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_enabled_features_response import RimeListEnabledFeaturesResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_file_scan_results_response import RimeListFileScanResultsResponse
+from rime_sdk.swagger.swagger_client.models.rime_list_firewall_instances_response import RimeListFirewallInstancesResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_images_request import RimeListImagesRequest
 from rime_sdk.swagger.swagger_client.models.rime_list_images_response import RimeListImagesResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_jobs_for_project_request_query import RimeListJobsForProjectRequestQuery
 from rime_sdk.swagger.swagger_client.models.rime_list_jobs_for_project_response import RimeListJobsForProjectResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_metric_identifiers_response import RimeListMetricIdentifiersResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_model_cards_response import RimeListModelCardsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_models_response import RimeListModelsResponse
@@ -395,14 +403,16 @@
 from rime_sdk.swagger.swagger_client.models.rime_order import RimeOrder
 from rime_sdk.swagger.swagger_client.models.rime_parent_role_subject_role_pair import RimeParentRoleSubjectRolePair
 from rime_sdk.swagger.swagger_client.models.rime_ri_email_recipient import RimeRIEmailRecipient
 from rime_sdk.swagger.swagger_client.models.rime_ri_plan import RimeRIPlan
 from rime_sdk.swagger.swagger_client.models.rime_register_data_stream_response import RimeRegisterDataStreamResponse
 from rime_sdk.swagger.swagger_client.models.rime_register_dataset_response import RimeRegisterDatasetResponse
 from rime_sdk.swagger.swagger_client.models.rime_register_external_agent_request import RimeRegisterExternalAgentRequest
+from rime_sdk.swagger.swagger_client.models.rime_register_firewall_agent_request import RimeRegisterFirewallAgentRequest
+from rime_sdk.swagger.swagger_client.models.rime_register_firewall_agent_response import RimeRegisterFirewallAgentResponse
 from rime_sdk.swagger.swagger_client.models.rime_register_internal_agent_response import RimeRegisterInternalAgentResponse
 from rime_sdk.swagger.swagger_client.models.rime_register_model_response import RimeRegisterModelResponse
 from rime_sdk.swagger.swagger_client.models.rime_register_prediction_set_response import RimeRegisterPredictionSetResponse
 from rime_sdk.swagger.swagger_client.models.rime_remove_user_from_workspace_response import RimeRemoveUserFromWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_reset_password_response import RimeResetPasswordResponse
 from rime_sdk.swagger.swagger_client.models.rime_resolve_detection_event_response import RimeResolveDetectionEventResponse
 from rime_sdk.swagger.swagger_client.models.rime_safe_url import RimeSafeURL
```

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/__init__.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/agent_manager_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/agent_manager_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -127,14 +127,113 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def agent_manager_create_firewall_agent(self, body, **kwargs):  # noqa: E501
+        """CreateFirewallAgent  # noqa: E501
+
+        Creates a firewall agent and returns the api key.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.agent_manager_create_firewall_agent(body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param RimeCreateFirewallAgentRequest body: (required)
+        :return: RimeCreateFirewallAgentResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.agent_manager_create_firewall_agent_with_http_info(body, **kwargs)  # noqa: E501
+        else:
+            (data) = self.agent_manager_create_firewall_agent_with_http_info(body, **kwargs)  # noqa: E501
+            return data
+
+    def agent_manager_create_firewall_agent_with_http_info(self, body, **kwargs):  # noqa: E501
+        """CreateFirewallAgent  # noqa: E501
+
+        Creates a firewall agent and returns the api key.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.agent_manager_create_firewall_agent_with_http_info(body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param RimeCreateFirewallAgentRequest body: (required)
+        :return: RimeCreateFirewallAgentResponse
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
+                    " to method agent_manager_create_firewall_agent" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'body' is set
+        if ('body' not in params or
+                params['body'] is None):
+            raise ValueError("Missing the required parameter `body` when calling `agent_manager_create_firewall_agent`")  # noqa: E501
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
+            '/v1-beta/agents/firewall', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RimeCreateFirewallAgentResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def agent_manager_delete_agent(self, agent_id_uuid, **kwargs):  # noqa: E501
         """DeleteAgent  # noqa: E501
 
         Deletes a specified agent. Must be called on an already deactivated agent. An error is returned if the deletion fails or if the agent is not in a deletable state.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.agent_manager_delete_agent(agent_id_uuid, async_req=True)
@@ -541,14 +640,15 @@
         >>> result = thread.get()
 
         :param async_req bool
         :param str page_size: The maximum number of Agent objects to return in a single page.
         :param str page_token: Specifies a page of the list returned by a ListAgents query. The ListAgents query returns a pageToken when there is more than one page of results. Specify either this field or the firstPageQuery field.
         :param list[str] first_page_query_agent_status_types: Specifies a set of agent status types. The query filters for results that match the specified types.   - AGENT_STATUS_PENDING: Resources have been created for the agent but the agent has not started yet.  - AGENT_STATUS_ACTIVE: Agent can run jobs.  - AGENT_STATUS_UNRESPONSIVE: No agent heartbeat for three minutes.  - AGENT_STATUS_DEACTIVATED: Agent can no longer run jobs and can be deleted. (Deprecated after Deactivation and Deletion endpoints are combined)
         :param list[str] first_page_query_agent_ids: Specifies a set of agent IDs. The query filters for results that match the specified IDs.
+        :param str first_page_query_type: Specifies the type of agent (validation or firewall). The query filters for results that match the specified type.   - AGENT_TYPE_VALIDATION: We use the zero value for VALIDATION for backwards compatibility with existing agents. protolint:disable:next ENUM_FIELD_NAMES_ZERO_VALUE_END_WITH
         :return: RimeListAgentsResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.agent_manager_list_agents_with_http_info(**kwargs)  # noqa: E501
@@ -566,20 +666,21 @@
         >>> result = thread.get()
 
         :param async_req bool
         :param str page_size: The maximum number of Agent objects to return in a single page.
         :param str page_token: Specifies a page of the list returned by a ListAgents query. The ListAgents query returns a pageToken when there is more than one page of results. Specify either this field or the firstPageQuery field.
         :param list[str] first_page_query_agent_status_types: Specifies a set of agent status types. The query filters for results that match the specified types.   - AGENT_STATUS_PENDING: Resources have been created for the agent but the agent has not started yet.  - AGENT_STATUS_ACTIVE: Agent can run jobs.  - AGENT_STATUS_UNRESPONSIVE: No agent heartbeat for three minutes.  - AGENT_STATUS_DEACTIVATED: Agent can no longer run jobs and can be deleted. (Deprecated after Deactivation and Deletion endpoints are combined)
         :param list[str] first_page_query_agent_ids: Specifies a set of agent IDs. The query filters for results that match the specified IDs.
+        :param str first_page_query_type: Specifies the type of agent (validation or firewall). The query filters for results that match the specified type.   - AGENT_TYPE_VALIDATION: We use the zero value for VALIDATION for backwards compatibility with existing agents. protolint:disable:next ENUM_FIELD_NAMES_ZERO_VALUE_END_WITH
         :return: RimeListAgentsResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['page_size', 'page_token', 'first_page_query_agent_status_types', 'first_page_query_agent_ids']  # noqa: E501
+        all_params = ['page_size', 'page_token', 'first_page_query_agent_status_types', 'first_page_query_agent_ids', 'first_page_query_type']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -602,14 +703,16 @@
             query_params.append(('pageToken', params['page_token']))  # noqa: E501
         if 'first_page_query_agent_status_types' in params:
             query_params.append(('firstPageQuery.agentStatusTypes', params['first_page_query_agent_status_types']))  # noqa: E501
             collection_formats['firstPageQuery.agentStatusTypes'] = 'multi'  # noqa: E501
         if 'first_page_query_agent_ids' in params:
             query_params.append(('firstPageQuery.agentIds', params['first_page_query_agent_ids']))  # noqa: E501
             collection_formats['firstPageQuery.agentIds'] = 'multi'  # noqa: E501
+        if 'first_page_query_type' in params:
+            query_params.append(('firstPageQuery.type', params['first_page_query_type']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -632,14 +735,114 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def agent_manager_list_firewall_instances(self, **kwargs):  # noqa: E501
+        """ListFirewallInstances  # noqa: E501
+
+        Returns a paginated list of firewall instances.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.agent_manager_list_firewall_instances(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str page_size:
+        :param str page_token: Specifies a page of the list returned by a ListFirewallInstances query. The ListFirewallInstances query returns a pageToken when there is more than one page of results. Specify either this field or the firstPageQuery field.
+        :param list[str] first_page_query_agent_ids: Specifies a set of agent IDs. The query filters for firewall instances that belong to the specified agents.
+        :return: RimeListFirewallInstancesResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.agent_manager_list_firewall_instances_with_http_info(**kwargs)  # noqa: E501
+        else:
+            (data) = self.agent_manager_list_firewall_instances_with_http_info(**kwargs)  # noqa: E501
+            return data
+
+    def agent_manager_list_firewall_instances_with_http_info(self, **kwargs):  # noqa: E501
+        """ListFirewallInstances  # noqa: E501
+
+        Returns a paginated list of firewall instances.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.agent_manager_list_firewall_instances_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str page_size:
+        :param str page_token: Specifies a page of the list returned by a ListFirewallInstances query. The ListFirewallInstances query returns a pageToken when there is more than one page of results. Specify either this field or the firstPageQuery field.
+        :param list[str] first_page_query_agent_ids: Specifies a set of agent IDs. The query filters for firewall instances that belong to the specified agents.
+        :return: RimeListFirewallInstancesResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['page_size', 'page_token', 'first_page_query_agent_ids']  # noqa: E501
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
+                    " to method agent_manager_list_firewall_instances" % key
+                )
+            params[key] = val
+        del params['kwargs']
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'page_size' in params:
+            query_params.append(('pageSize', params['page_size']))  # noqa: E501
+        if 'page_token' in params:
+            query_params.append(('pageToken', params['page_token']))  # noqa: E501
+        if 'first_page_query_agent_ids' in params:
+            query_params.append(('firstPageQuery.agentIds', params['first_page_query_agent_ids']))  # noqa: E501
+            collection_formats['firstPageQuery.agentIds'] = 'multi'  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['X-Firewall-Api-Key', 'X-Firewall-Auth-Token', 'rime-api-key']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/v1/agents/firewall/instances', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RimeListFirewallInstancesResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def agent_manager_register_external_agent(self, body, **kwargs):  # noqa: E501
         """RegisterExternalAgent is used by external agents during startup to upload the signing key to the backend. This call is idempotent; it will be called by the external agent upon every restart. No matter there is a signing key exists in the DB, the key is uploaded and created in the DB.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.agent_manager_register_external_agent(body, async_req=True)
         >>> result = thread.get()
@@ -729,14 +932,111 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def agent_manager_register_firewall_agent(self, body, **kwargs):  # noqa: E501
+        """RegisterFirewallAgent is used by firewall agents during startup to upload the signing key to the CP backend. In addtion, the CP will return a public key that is used to verify user API tokens.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.agent_manager_register_firewall_agent(body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param RimeRegisterFirewallAgentRequest body: (required)
+        :return: RimeRegisterFirewallAgentResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.agent_manager_register_firewall_agent_with_http_info(body, **kwargs)  # noqa: E501
+        else:
+            (data) = self.agent_manager_register_firewall_agent_with_http_info(body, **kwargs)  # noqa: E501
+            return data
+
+    def agent_manager_register_firewall_agent_with_http_info(self, body, **kwargs):  # noqa: E501
+        """RegisterFirewallAgent is used by firewall agents during startup to upload the signing key to the CP backend. In addtion, the CP will return a public key that is used to verify user API tokens.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.agent_manager_register_firewall_agent_with_http_info(body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param RimeRegisterFirewallAgentRequest body: (required)
+        :return: RimeRegisterFirewallAgentResponse
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
+                    " to method agent_manager_register_firewall_agent" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'body' is set
+        if ('body' not in params or
+                params['body'] is None):
+            raise ValueError("Missing the required parameter `body` when calling `agent_manager_register_firewall_agent`")  # noqa: E501
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
+            '/internal/agents/firewall', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RimeRegisterFirewallAgentResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def agent_manager_register_internal_agent(self, **kwargs):  # noqa: E501
         """RegisterInternalAgent is used by internal agents during startup to obtain an ID. This call is idempotent; it will be called by internal agent upon every restart. If no record of an internal agent exists, a new agent is created in the DB.Otherwise, the Agent Management service returns the ID of the existing agent.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.agent_manager_register_internal_agent(async_req=True)
         >>> result = thread.get()
```

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/config_validator_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/config_validator_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/data_collector_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/data_collector_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/detection_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/detection_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/feature_flag_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/feature_flag_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/file_scanning_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/file_scanning_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/file_upload_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/file_upload_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/firewall_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/firewall_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/firewall_instance_manager_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/firewall_instance_manager_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,15 +327,15 @@
         This lists the Firewall Instances on the cluster.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.firewall_instance_manager_list_firewall_instances(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :return: GenerativefirewallListFirewallInstancesResponse
+        :return: ApigenerativefirewallListFirewallInstancesResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.firewall_instance_manager_list_firewall_instances_with_http_info(**kwargs)  # noqa: E501
         else:
@@ -348,15 +348,15 @@
         This lists the Firewall Instances on the cluster.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.firewall_instance_manager_list_firewall_instances_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :return: GenerativefirewallListFirewallInstancesResponse
+        :return: ApigenerativefirewallListFirewallInstancesResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = []  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -396,15 +396,15 @@
             '/v1-beta/firewall-instance', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='GenerativefirewallListFirewallInstancesResponse',  # noqa: E501
+            response_type='ApigenerativefirewallListFirewallInstancesResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/firewall_service_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/firewall_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/generative_model_testing_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/generative_model_testing_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/image_registry_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/image_registry_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/integration_service_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/integration_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/job_reader_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/job_reader_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/model_card_service_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/model_card_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/model_testing_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/model_testing_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/monitor_service_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/monitor_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/notification_setting_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/notification_setting_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/project_service_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/project_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/registry_service_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/registry_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/results_reader_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/results_reader_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/rime_info_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/rime_info_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/schedule_service_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/schedule_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/user_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/validation_service_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/validation_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api/workspace_service_api.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api/workspace_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/api_client.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/configuration.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/__init__.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 """
 
 from __future__ import absolute_import
 
 # import models into model package
 from rime_sdk.swagger.swagger_client.models.agent_id_uuid_upgrade_body import AgentIdUuidUpgradeBody
 from rime_sdk.swagger.swagger_client.models.agent_id_uuid_upgrade_body1 import AgentIdUuidUpgradeBody1
+from rime_sdk.swagger.swagger_client.models.apigenerativefirewall_list_firewall_instances_response import ApigenerativefirewallListFirewallInstancesResponse
 from rime_sdk.swagger.swagger_client.models.apigenerativefirewall_standard_info import ApigenerativefirewallStandardInfo
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_category_test_identifier import ArtifactIdentifierCategoryTestIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_subset_test_metric_identifier import ArtifactIdentifierSubsetTestMetricIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_test_case_metric_identifier import ArtifactIdentifierTestCaseMetricIdentifier
 from rime_sdk.swagger.swagger_client.models.config_generation_category_config_generation_service_response import ConfigGenerationCategoryConfigGenerationServiceResponse
 from rime_sdk.swagger.swagger_client.models.config_generation_profiling_config_generation_service_response import ConfigGenerationProfilingConfigGenerationServiceResponse
 from rime_sdk.swagger.swagger_client.models.config_generation_test_suite_config_generation_service_response import ConfigGenerationTestSuiteConfigGenerationServiceResponse
@@ -89,35 +90,37 @@
 from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_tokenizer import GenerativefirewallFirewallTokenizer
 from rime_sdk.swagger.swagger_client.models.generativefirewall_flagged_substring import GenerativefirewallFlaggedSubstring
 from rime_sdk.swagger.swagger_client.models.generativefirewall_get_firewall_effective_config_response import GenerativefirewallGetFirewallEffectiveConfigResponse
 from rime_sdk.swagger.swagger_client.models.generativefirewall_get_firewall_instance_response import GenerativefirewallGetFirewallInstanceResponse
 from rime_sdk.swagger.swagger_client.models.generativefirewall_individual_rules_config import GenerativefirewallIndividualRulesConfig
 from rime_sdk.swagger.swagger_client.models.generativefirewall_language_detection_details import GenerativefirewallLanguageDetectionDetails
 from rime_sdk.swagger.swagger_client.models.generativefirewall_language_detection_rule_config import GenerativefirewallLanguageDetectionRuleConfig
-from rime_sdk.swagger.swagger_client.models.generativefirewall_list_firewall_instances_response import GenerativefirewallListFirewallInstancesResponse
 from rime_sdk.swagger.swagger_client.models.generativefirewall_off_topic_rule_config import GenerativefirewallOffTopicRuleConfig
 from rime_sdk.swagger.swagger_client.models.generativefirewall_pii_detection_details import GenerativefirewallPiiDetectionDetails
 from rime_sdk.swagger.swagger_client.models.generativefirewall_pii_detection_rule_config import GenerativefirewallPiiDetectionRuleConfig
 from rime_sdk.swagger.swagger_client.models.generativefirewall_pii_entity_type import GenerativefirewallPiiEntityType
 from rime_sdk.swagger.swagger_client.models.generativefirewall_prompt_injection_details import GenerativefirewallPromptInjectionDetails
 from rime_sdk.swagger.swagger_client.models.generativefirewall_prompt_injection_v2_rule_config import GenerativefirewallPromptInjectionV2RuleConfig
+from rime_sdk.swagger.swagger_client.models.generativefirewall_rule_false_positive_rate import GenerativefirewallRuleFalsePositiveRate
 from rime_sdk.swagger.swagger_client.models.generativefirewall_rule_output import GenerativefirewallRuleOutput
 from rime_sdk.swagger.swagger_client.models.generativefirewall_rule_sensitivity import GenerativefirewallRuleSensitivity
 from rime_sdk.swagger.swagger_client.models.generativefirewall_toxicity_detection_details import GenerativefirewallToxicityDetectionDetails
+from rime_sdk.swagger.swagger_client.models.generativefirewall_toxicity_rule_config import GenerativefirewallToxicityRuleConfig
 from rime_sdk.swagger.swagger_client.models.generativefirewall_unknown_external_source_rule_config import GenerativefirewallUnknownExternalSourceRuleConfig
 from rime_sdk.swagger.swagger_client.models.generativefirewall_update_firewall_instance_response import GenerativefirewallUpdateFirewallInstanceResponse
 from rime_sdk.swagger.swagger_client.models.generativefirewall_validate_request import GenerativefirewallValidateRequest
 from rime_sdk.swagger.swagger_client.models.generativefirewall_validate_response import GenerativefirewallValidateResponse
 from rime_sdk.swagger.swagger_client.models.generativetesting_generative_testing_result import GenerativetestingGenerativeTestingResult
 from rime_sdk.swagger.swagger_client.models.generativetesting_generative_testing_result_standard_info import GenerativetestingGenerativeTestingResultStandardInfo
 from rime_sdk.swagger.swagger_client.models.generativetesting_get_generative_model_test_results_request_query import GenerativetestingGetGenerativeModelTestResultsRequestQuery
 from rime_sdk.swagger.swagger_client.models.generativetesting_get_generative_model_test_results_response import GenerativetestingGetGenerativeModelTestResultsResponse
 from rime_sdk.swagger.swagger_client.models.generativetesting_objective_sub_category import GenerativetestingObjectiveSubCategory
 from rime_sdk.swagger.swagger_client.models.generativetesting_start_generative_model_test_request import GenerativetestingStartGenerativeModelTestRequest
 from rime_sdk.swagger.swagger_client.models.generativetesting_start_generative_model_test_response import GenerativetestingStartGenerativeModelTestResponse
+from rime_sdk.swagger.swagger_client.models.generativetesting_threat import GenerativetestingThreat
 from rime_sdk.swagger.swagger_client.models.googlerpc_status import GooglerpcStatus
 from rime_sdk.swagger.swagger_client.models.heartbeat_agent_id_uuid_body import HeartbeatAgentIdUuidBody
 from rime_sdk.swagger.swagger_client.models.image_reference_reference_type import ImageReferenceReferenceType
 from rime_sdk.swagger.swagger_client.models.integration_integration_level import IntegrationIntegrationLevel
 from rime_sdk.swagger.swagger_client.models.integration_integration_schema import IntegrationIntegrationSchema
 from rime_sdk.swagger.swagger_client.models.integration_integration_type import IntegrationIntegrationType
 from rime_sdk.swagger.swagger_client.models.integration_variable_sensitivity import IntegrationVariableSensitivity
@@ -126,14 +129,15 @@
 from rime_sdk.swagger.swagger_client.models.job_data_generative_model_test import JobDataGenerativeModelTest
 from rime_sdk.swagger.swagger_client.models.job_data_scan import JobDataScan
 from rime_sdk.swagger.swagger_client.models.job_data_stress_test import JobDataStressTest
 from rime_sdk.swagger.swagger_client.models.language_detection_details_language_substring import LanguageDetectionDetailsLanguageSubstring
 from rime_sdk.swagger.swagger_client.models.list_agents_request_list_agents_query import ListAgentsRequestListAgentsQuery
 from rime_sdk.swagger.swagger_client.models.list_datasets_request_datasets_query import ListDatasetsRequestDatasetsQuery
 from rime_sdk.swagger.swagger_client.models.list_file_scan_results_request_file_scan_query import ListFileScanResultsRequestFileScanQuery
+from rime_sdk.swagger.swagger_client.models.list_firewall_instances_request_list_firewall_instances_query import ListFirewallInstancesRequestListFirewallInstancesQuery
 from rime_sdk.swagger.swagger_client.models.list_images_request_pip_library_filter import ListImagesRequestPipLibraryFilter
 from rime_sdk.swagger.swagger_client.models.list_metric_identifiers_response_aggregated_metric import ListMetricIdentifiersResponseAggregatedMetric
 from rime_sdk.swagger.swagger_client.models.list_metric_identifiers_response_feature_metric_without_subsets import ListMetricIdentifiersResponseFeatureMetricWithoutSubsets
 from rime_sdk.swagger.swagger_client.models.list_metric_identifiers_response_feature_metrics import ListMetricIdentifiersResponseFeatureMetrics
 from rime_sdk.swagger.swagger_client.models.list_metric_identifiers_response_subset_metric import ListMetricIdentifiersResponseSubsetMetric
 from rime_sdk.swagger.swagger_client.models.list_metric_identifiers_response_subset_metrics import ListMetricIdentifiersResponseSubsetMetrics
 from rime_sdk.swagger.swagger_client.models.list_models_request_model_query import ListModelsRequestModelQuery
@@ -221,14 +225,15 @@
 from rime_sdk.swagger.swagger_client.models.resetpassword_user_id_uuid_body import ResetpasswordUserIdUuidBody
 from rime_sdk.swagger.swagger_client.models.rime_api_token_info import RimeAPITokenInfo
 from rime_sdk.swagger.swagger_client.models.rime_actor_role import RimeActorRole
 from rime_sdk.swagger.swagger_client.models.rime_add_users_to_workspace_response import RimeAddUsersToWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_agent import RimeAgent
 from rime_sdk.swagger.swagger_client.models.rime_agent_desired_state import RimeAgentDesiredState
 from rime_sdk.swagger.swagger_client.models.rime_agent_status import RimeAgentStatus
+from rime_sdk.swagger.swagger_client.models.rime_agent_type import RimeAgentType
 from rime_sdk.swagger.swagger_client.models.rime_attack_objective import RimeAttackObjective
 from rime_sdk.swagger.swagger_client.models.rime_cancel_job_response import RimeCancelJobResponse
 from rime_sdk.swagger.swagger_client.models.rime_category_metric import RimeCategoryMetric
 from rime_sdk.swagger.swagger_client.models.rime_category_test_result import RimeCategoryTestResult
 from rime_sdk.swagger.swagger_client.models.rime_config_type import RimeConfigType
 from rime_sdk.swagger.swagger_client.models.rime_configure_integration_request_integration_variable import RimeConfigureIntegrationRequestIntegrationVariable
 from rime_sdk.swagger.swagger_client.models.rime_configure_integration_response import RimeConfigureIntegrationResponse
@@ -237,14 +242,16 @@
 from rime_sdk.swagger.swagger_client.models.rime_create_api_token_request import RimeCreateAPITokenRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_api_token_response import RimeCreateAPITokenResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_agent_request import RimeCreateAgentRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_agent_response import RimeCreateAgentResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_custom_monitor_response import RimeCreateCustomMonitorResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_customer_managed_key_request import RimeCreateCustomerManagedKeyRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_customer_managed_key_response import RimeCreateCustomerManagedKeyResponse
+from rime_sdk.swagger.swagger_client.models.rime_create_firewall_agent_request import RimeCreateFirewallAgentRequest
+from rime_sdk.swagger.swagger_client.models.rime_create_firewall_agent_response import RimeCreateFirewallAgentResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_firewall_request import RimeCreateFirewallRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_firewall_response import RimeCreateFirewallResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_image_request import RimeCreateImageRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_image_response import RimeCreateImageResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_integration_request import RimeCreateIntegrationRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_integration_response import RimeCreateIntegrationResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_model_card_request import RimeCreateModelCardRequest
@@ -329,14 +336,15 @@
 from rime_sdk.swagger.swagger_client.models.rime_list_agents_response import RimeListAgentsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_current_user_roles_response import RimeListCurrentUserRolesResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_datasets_response import RimeListDatasetsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_detection_events_request_query import RimeListDetectionEventsRequestQuery
 from rime_sdk.swagger.swagger_client.models.rime_list_detection_events_response import RimeListDetectionEventsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_enabled_features_response import RimeListEnabledFeaturesResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_file_scan_results_response import RimeListFileScanResultsResponse
+from rime_sdk.swagger.swagger_client.models.rime_list_firewall_instances_response import RimeListFirewallInstancesResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_images_request import RimeListImagesRequest
 from rime_sdk.swagger.swagger_client.models.rime_list_images_response import RimeListImagesResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_jobs_for_project_request_query import RimeListJobsForProjectRequestQuery
 from rime_sdk.swagger.swagger_client.models.rime_list_jobs_for_project_response import RimeListJobsForProjectResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_metric_identifiers_response import RimeListMetricIdentifiersResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_model_cards_response import RimeListModelCardsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_models_response import RimeListModelsResponse
@@ -363,14 +371,16 @@
 from rime_sdk.swagger.swagger_client.models.rime_order import RimeOrder
 from rime_sdk.swagger.swagger_client.models.rime_parent_role_subject_role_pair import RimeParentRoleSubjectRolePair
 from rime_sdk.swagger.swagger_client.models.rime_ri_email_recipient import RimeRIEmailRecipient
 from rime_sdk.swagger.swagger_client.models.rime_ri_plan import RimeRIPlan
 from rime_sdk.swagger.swagger_client.models.rime_register_data_stream_response import RimeRegisterDataStreamResponse
 from rime_sdk.swagger.swagger_client.models.rime_register_dataset_response import RimeRegisterDatasetResponse
 from rime_sdk.swagger.swagger_client.models.rime_register_external_agent_request import RimeRegisterExternalAgentRequest
+from rime_sdk.swagger.swagger_client.models.rime_register_firewall_agent_request import RimeRegisterFirewallAgentRequest
+from rime_sdk.swagger.swagger_client.models.rime_register_firewall_agent_response import RimeRegisterFirewallAgentResponse
 from rime_sdk.swagger.swagger_client.models.rime_register_internal_agent_response import RimeRegisterInternalAgentResponse
 from rime_sdk.swagger.swagger_client.models.rime_register_model_response import RimeRegisterModelResponse
 from rime_sdk.swagger.swagger_client.models.rime_register_prediction_set_response import RimeRegisterPredictionSetResponse
 from rime_sdk.swagger.swagger_client.models.rime_remove_user_from_workspace_response import RimeRemoveUserFromWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_reset_password_response import RimeResetPasswordResponse
 from rime_sdk.swagger.swagger_client.models.rime_resolve_detection_event_response import RimeResolveDetectionEventResponse
 from rime_sdk.swagger.swagger_client.models.rime_safe_url import RimeSafeURL
```

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body1.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body1.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/apigenerativefirewall_standard_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/apigenerativefirewall_standard_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/config_generation_category_config_generation_service_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/config_generation_category_config_generation_service_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/config_generation_profiling_config_generation_service_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/config_generation_profiling_config_generation_service_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/config_generation_test_suite_config_generation_service_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/config_generation_test_suite_config_generation_service_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/crossplanetask_cross_plane_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/crossplanetask_cross_plane_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/dataset_dataset.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/dataset_dataset.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_detection_event.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/detection_detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_event_detail.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/detection_event_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_event_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/detection_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_resolution.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/detection_resolution.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_file_security_report.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_file_security_report.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_package_url.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_package_url.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata_license.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata_license.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/fileserver_check_object_exists_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/fileserver_check_object_exists_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/fileserver_delete_object_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/fileserver_delete_object_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/fileserver_get_read_object_presigned_link_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/fileserver_get_read_object_presigned_link_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/fileserver_get_upload_object_presigned_link_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/fileserver_get_upload_object_presigned_link_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/fileserver_list_objects_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/fileserver_list_objects_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewall_firewall.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/firewall_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/firewallinstance_firewall_instance_firewall_instance_id_uuid_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/firewallinstance_firewall_instance_firewall_instance_id_uuid_body.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,39 +27,44 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'firewall_instance_id': 'object',
         'config': 'GenerativefirewallFirewallRuleConfig',
         'deployment_status': 'GenerativefirewallFirewallInstanceStatus',
-        'description': 'str'
+        'description': 'str',
+        'agent_id': 'RimeUUID'
     }
 
     attribute_map = {
         'firewall_instance_id': 'firewallInstanceId',
         'config': 'config',
         'deployment_status': 'deploymentStatus',
-        'description': 'description'
+        'description': 'description',
+        'agent_id': 'agentId'
     }
 
-    def __init__(self, firewall_instance_id=None, config=None, deployment_status=None, description=None):  # noqa: E501
+    def __init__(self, firewall_instance_id=None, config=None, deployment_status=None, description=None, agent_id=None):  # noqa: E501
         """FirewallinstanceFirewallInstanceFirewallInstanceIdUuidBody - a model defined in Swagger"""  # noqa: E501
         self._firewall_instance_id = None
         self._config = None
         self._deployment_status = None
         self._description = None
+        self._agent_id = None
         self.discriminator = None
         if firewall_instance_id is not None:
             self.firewall_instance_id = firewall_instance_id
         if config is not None:
             self.config = config
         if deployment_status is not None:
             self.deployment_status = deployment_status
         if description is not None:
             self.description = description
+        if agent_id is not None:
+            self.agent_id = agent_id
 
     @property
     def firewall_instance_id(self):
         """Gets the firewall_instance_id of this FirewallinstanceFirewallInstanceFirewallInstanceIdUuidBody.  # noqa: E501
 
         Unique ID of an object in RIME.  # noqa: E501
 
@@ -141,14 +146,35 @@
 
         :param description: The description of this FirewallinstanceFirewallInstanceFirewallInstanceIdUuidBody.  # noqa: E501
         :type: str
         """
 
         self._description = description
 
+    @property
+    def agent_id(self):
+        """Gets the agent_id of this FirewallinstanceFirewallInstanceFirewallInstanceIdUuidBody.  # noqa: E501
+
+
+        :return: The agent_id of this FirewallinstanceFirewallInstanceFirewallInstanceIdUuidBody.  # noqa: E501
+        :rtype: RimeUUID
+        """
+        return self._agent_id
+
+    @agent_id.setter
+    def agent_id(self, agent_id):
+        """Sets the agent_id of this FirewallinstanceFirewallInstanceFirewallInstanceIdUuidBody.
+
+
+        :param agent_id: The agent_id of this FirewallinstanceFirewallInstanceFirewallInstanceIdUuidBody.  # noqa: E501
+        :type: RimeUUID
+        """
+
+        self._agent_id = agent_id
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/flagged_substring_request_body_component.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/flagged_substring_request_body_component.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generative_testing_result_example.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generative_testing_result_example.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_custom_pii_entity.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_custom_pii_entity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_denial_of_service_rule_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_denial_of_service_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_info.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,39 +27,44 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'firewall_instance_id': 'RimeUUID',
         'config': 'GenerativefirewallFirewallRuleConfig',
         'deployment_status': 'GenerativefirewallFirewallInstanceStatus',
-        'description': 'str'
+        'description': 'str',
+        'agent_id': 'RimeUUID'
     }
 
     attribute_map = {
         'firewall_instance_id': 'firewallInstanceId',
         'config': 'config',
         'deployment_status': 'deploymentStatus',
-        'description': 'description'
+        'description': 'description',
+        'agent_id': 'agentId'
     }
 
-    def __init__(self, firewall_instance_id=None, config=None, deployment_status=None, description=None):  # noqa: E501
+    def __init__(self, firewall_instance_id=None, config=None, deployment_status=None, description=None, agent_id=None):  # noqa: E501
         """GenerativefirewallFirewallInstanceInfo - a model defined in Swagger"""  # noqa: E501
         self._firewall_instance_id = None
         self._config = None
         self._deployment_status = None
         self._description = None
+        self._agent_id = None
         self.discriminator = None
         if firewall_instance_id is not None:
             self.firewall_instance_id = firewall_instance_id
         if config is not None:
             self.config = config
         if deployment_status is not None:
             self.deployment_status = deployment_status
         if description is not None:
             self.description = description
+        if agent_id is not None:
+            self.agent_id = agent_id
 
     @property
     def firewall_instance_id(self):
         """Gets the firewall_instance_id of this GenerativefirewallFirewallInstanceInfo.  # noqa: E501
 
 
         :return: The firewall_instance_id of this GenerativefirewallFirewallInstanceInfo.  # noqa: E501
@@ -139,14 +144,35 @@
 
         :param description: The description of this GenerativefirewallFirewallInstanceInfo.  # noqa: E501
         :type: str
         """
 
         self._description = description
 
+    @property
+    def agent_id(self):
+        """Gets the agent_id of this GenerativefirewallFirewallInstanceInfo.  # noqa: E501
+
+
+        :return: The agent_id of this GenerativefirewallFirewallInstanceInfo.  # noqa: E501
+        :rtype: RimeUUID
+        """
+        return self._agent_id
+
+    @agent_id.setter
+    def agent_id(self, agent_id):
+        """Sets the agent_id of this GenerativefirewallFirewallInstanceInfo.
+
+
+        :param agent_id: The agent_id of this GenerativefirewallFirewallInstanceInfo.  # noqa: E501
+        :type: RimeUUID
+        """
+
+        self._agent_id = agent_id
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_status.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_tokenizer.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_flagged_substring.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_flagged_substring.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_effective_config_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_effective_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_instance_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_instance_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_individual_rules_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_individual_rules_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,38 +31,44 @@
         'off_topic': 'GenerativefirewallOffTopicRuleConfig',
         'pii_detection_input': 'GenerativefirewallPiiDetectionRuleConfig',
         'pii_detection_output': 'GenerativefirewallPiiDetectionRuleConfig',
         'denial_of_service_input': 'GenerativefirewallDenialOfServiceRuleConfig',
         'denial_of_service_output': 'GenerativefirewallDenialOfServiceRuleConfig',
         'unknown_external_source': 'GenerativefirewallUnknownExternalSourceRuleConfig',
         'language_detection': 'GenerativefirewallLanguageDetectionRuleConfig',
-        'prompt_injection_v2': 'GenerativefirewallPromptInjectionV2RuleConfig'
+        'prompt_injection_v2': 'GenerativefirewallPromptInjectionV2RuleConfig',
+        'toxicity_rule_config_input': 'GenerativefirewallToxicityRuleConfig',
+        'toxicity_rule_config_output': 'GenerativefirewallToxicityRuleConfig'
     }
 
     attribute_map = {
         'off_topic': 'offTopic',
         'pii_detection_input': 'piiDetectionInput',
         'pii_detection_output': 'piiDetectionOutput',
         'denial_of_service_input': 'denialOfServiceInput',
         'denial_of_service_output': 'denialOfServiceOutput',
         'unknown_external_source': 'unknownExternalSource',
         'language_detection': 'languageDetection',
-        'prompt_injection_v2': 'promptInjectionV2'
+        'prompt_injection_v2': 'promptInjectionV2',
+        'toxicity_rule_config_input': 'toxicityRuleConfigInput',
+        'toxicity_rule_config_output': 'toxicityRuleConfigOutput'
     }
 
-    def __init__(self, off_topic=None, pii_detection_input=None, pii_detection_output=None, denial_of_service_input=None, denial_of_service_output=None, unknown_external_source=None, language_detection=None, prompt_injection_v2=None):  # noqa: E501
+    def __init__(self, off_topic=None, pii_detection_input=None, pii_detection_output=None, denial_of_service_input=None, denial_of_service_output=None, unknown_external_source=None, language_detection=None, prompt_injection_v2=None, toxicity_rule_config_input=None, toxicity_rule_config_output=None):  # noqa: E501
         """GenerativefirewallIndividualRulesConfig - a model defined in Swagger"""  # noqa: E501
         self._off_topic = None
         self._pii_detection_input = None
         self._pii_detection_output = None
         self._denial_of_service_input = None
         self._denial_of_service_output = None
         self._unknown_external_source = None
         self._language_detection = None
         self._prompt_injection_v2 = None
+        self._toxicity_rule_config_input = None
+        self._toxicity_rule_config_output = None
         self.discriminator = None
         if off_topic is not None:
             self.off_topic = off_topic
         if pii_detection_input is not None:
             self.pii_detection_input = pii_detection_input
         if pii_detection_output is not None:
             self.pii_detection_output = pii_detection_output
@@ -72,14 +78,18 @@
             self.denial_of_service_output = denial_of_service_output
         if unknown_external_source is not None:
             self.unknown_external_source = unknown_external_source
         if language_detection is not None:
             self.language_detection = language_detection
         if prompt_injection_v2 is not None:
             self.prompt_injection_v2 = prompt_injection_v2
+        if toxicity_rule_config_input is not None:
+            self.toxicity_rule_config_input = toxicity_rule_config_input
+        if toxicity_rule_config_output is not None:
+            self.toxicity_rule_config_output = toxicity_rule_config_output
 
     @property
     def off_topic(self):
         """Gets the off_topic of this GenerativefirewallIndividualRulesConfig.  # noqa: E501
 
 
         :return: The off_topic of this GenerativefirewallIndividualRulesConfig.  # noqa: E501
@@ -241,14 +251,56 @@
 
         :param prompt_injection_v2: The prompt_injection_v2 of this GenerativefirewallIndividualRulesConfig.  # noqa: E501
         :type: GenerativefirewallPromptInjectionV2RuleConfig
         """
 
         self._prompt_injection_v2 = prompt_injection_v2
 
+    @property
+    def toxicity_rule_config_input(self):
+        """Gets the toxicity_rule_config_input of this GenerativefirewallIndividualRulesConfig.  # noqa: E501
+
+
+        :return: The toxicity_rule_config_input of this GenerativefirewallIndividualRulesConfig.  # noqa: E501
+        :rtype: GenerativefirewallToxicityRuleConfig
+        """
+        return self._toxicity_rule_config_input
+
+    @toxicity_rule_config_input.setter
+    def toxicity_rule_config_input(self, toxicity_rule_config_input):
+        """Sets the toxicity_rule_config_input of this GenerativefirewallIndividualRulesConfig.
+
+
+        :param toxicity_rule_config_input: The toxicity_rule_config_input of this GenerativefirewallIndividualRulesConfig.  # noqa: E501
+        :type: GenerativefirewallToxicityRuleConfig
+        """
+
+        self._toxicity_rule_config_input = toxicity_rule_config_input
+
+    @property
+    def toxicity_rule_config_output(self):
+        """Gets the toxicity_rule_config_output of this GenerativefirewallIndividualRulesConfig.  # noqa: E501
+
+
+        :return: The toxicity_rule_config_output of this GenerativefirewallIndividualRulesConfig.  # noqa: E501
+        :rtype: GenerativefirewallToxicityRuleConfig
+        """
+        return self._toxicity_rule_config_output
+
+    @toxicity_rule_config_output.setter
+    def toxicity_rule_config_output(self, toxicity_rule_config_output):
+        """Sets the toxicity_rule_config_output of this GenerativefirewallIndividualRulesConfig.
+
+
+        :param toxicity_rule_config_output: The toxicity_rule_config_output of this GenerativefirewallIndividualRulesConfig.  # noqa: E501
+        :type: GenerativefirewallToxicityRuleConfig
+        """
+
+        self._toxicity_rule_config_output = toxicity_rule_config_output
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_details.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_rule_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_list_firewall_instances_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/apigenerativefirewall_list_firewall_instances_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class GenerativefirewallListFirewallInstancesResponse(object):
+class ApigenerativefirewallListFirewallInstancesResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -32,36 +32,36 @@
     }
 
     attribute_map = {
         'firewall_instances': 'firewallInstances'
     }
 
     def __init__(self, firewall_instances=None):  # noqa: E501
-        """GenerativefirewallListFirewallInstancesResponse - a model defined in Swagger"""  # noqa: E501
+        """ApigenerativefirewallListFirewallInstancesResponse - a model defined in Swagger"""  # noqa: E501
         self._firewall_instances = None
         self.discriminator = None
         if firewall_instances is not None:
             self.firewall_instances = firewall_instances
 
     @property
     def firewall_instances(self):
-        """Gets the firewall_instances of this GenerativefirewallListFirewallInstancesResponse.  # noqa: E501
+        """Gets the firewall_instances of this ApigenerativefirewallListFirewallInstancesResponse.  # noqa: E501
 
 
-        :return: The firewall_instances of this GenerativefirewallListFirewallInstancesResponse.  # noqa: E501
+        :return: The firewall_instances of this ApigenerativefirewallListFirewallInstancesResponse.  # noqa: E501
         :rtype: list[GenerativefirewallFirewallInstanceInfo]
         """
         return self._firewall_instances
 
     @firewall_instances.setter
     def firewall_instances(self, firewall_instances):
-        """Sets the firewall_instances of this GenerativefirewallListFirewallInstancesResponse.
+        """Sets the firewall_instances of this ApigenerativefirewallListFirewallInstancesResponse.
 
 
-        :param firewall_instances: The firewall_instances of this GenerativefirewallListFirewallInstancesResponse.  # noqa: E501
+        :param firewall_instances: The firewall_instances of this ApigenerativefirewallListFirewallInstancesResponse.  # noqa: E501
         :type: list[GenerativefirewallFirewallInstanceInfo]
         """
 
         self._firewall_instances = firewall_instances
 
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
-        if issubclass(GenerativefirewallListFirewallInstancesResponse, dict):
+        if issubclass(ApigenerativefirewallListFirewallInstancesResponse, dict):
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
-        if not isinstance(other, GenerativefirewallListFirewallInstancesResponse):
+        if not isinstance(other, ApigenerativefirewallListFirewallInstancesResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_off_topic_rule_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_off_topic_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_details.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_rule_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_entity_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_entity_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_details.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_details.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,51 +24,79 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'objectives': 'list[RimeAttackObjective]'
+        'objectives': 'list[RimeAttackObjective]',
+        'techniques': 'list[str]'
     }
 
     attribute_map = {
-        'objectives': 'objectives'
+        'objectives': 'objectives',
+        'techniques': 'techniques'
     }
 
-    def __init__(self, objectives=None):  # noqa: E501
+    def __init__(self, objectives=None, techniques=None):  # noqa: E501
         """GenerativefirewallPromptInjectionDetails - a model defined in Swagger"""  # noqa: E501
         self._objectives = None
+        self._techniques = None
         self.discriminator = None
         if objectives is not None:
             self.objectives = objectives
+        if techniques is not None:
+            self.techniques = techniques
 
     @property
     def objectives(self):
         """Gets the objectives of this GenerativefirewallPromptInjectionDetails.  # noqa: E501
 
-        Objectives represents the attack objectives found in the text, such as privacy or abuse violations.  # noqa: E501
+        Objectives represent the attack objectives found in the text, such as privacy or abuse violations.  # noqa: E501
 
         :return: The objectives of this GenerativefirewallPromptInjectionDetails.  # noqa: E501
         :rtype: list[RimeAttackObjective]
         """
         return self._objectives
 
     @objectives.setter
     def objectives(self, objectives):
         """Sets the objectives of this GenerativefirewallPromptInjectionDetails.
 
-        Objectives represents the attack objectives found in the text, such as privacy or abuse violations.  # noqa: E501
+        Objectives represent the attack objectives found in the text, such as privacy or abuse violations.  # noqa: E501
 
         :param objectives: The objectives of this GenerativefirewallPromptInjectionDetails.  # noqa: E501
         :type: list[RimeAttackObjective]
         """
 
         self._objectives = objectives
 
+    @property
+    def techniques(self):
+        """Gets the techniques of this GenerativefirewallPromptInjectionDetails.  # noqa: E501
+
+        Attack Techniques represent the technique used in a prompt injection for example: unicode obfuscation, base64 etc. These values may change between versions.  # noqa: E501
+
+        :return: The techniques of this GenerativefirewallPromptInjectionDetails.  # noqa: E501
+        :rtype: list[str]
+        """
+        return self._techniques
+
+    @techniques.setter
+    def techniques(self, techniques):
+        """Sets the techniques of this GenerativefirewallPromptInjectionDetails.
+
+        Attack Techniques represent the technique used in a prompt injection for example: unicode obfuscation, base64 etc. These values may change between versions.  # noqa: E501
+
+        :param techniques: The techniques of this GenerativefirewallPromptInjectionDetails.  # noqa: E501
+        :type: list[str]
+        """
+
+        self._techniques = techniques
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_v2_rule_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,63 +11,61 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class GenerativefirewallPromptInjectionV2RuleConfig(object):
+class RimeStartContinuousTestResponse(object):
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
-        'enabled': 'bool'
+        'job': 'RimeJobMetadata'
     }
 
     attribute_map = {
-        'enabled': 'enabled'
+        'job': 'job'
     }
 
-    def __init__(self, enabled=None):  # noqa: E501
-        """GenerativefirewallPromptInjectionV2RuleConfig - a model defined in Swagger"""  # noqa: E501
-        self._enabled = None
+    def __init__(self, job=None):  # noqa: E501
+        """RimeStartContinuousTestResponse - a model defined in Swagger"""  # noqa: E501
+        self._job = None
         self.discriminator = None
-        if enabled is not None:
-            self.enabled = enabled
+        if job is not None:
+            self.job = job
 
     @property
-    def enabled(self):
-        """Gets the enabled of this GenerativefirewallPromptInjectionV2RuleConfig.  # noqa: E501
+    def job(self):
+        """Gets the job of this RimeStartContinuousTestResponse.  # noqa: E501
 
-        Whether the rule is enabled.  # noqa: E501
 
-        :return: The enabled of this GenerativefirewallPromptInjectionV2RuleConfig.  # noqa: E501
-        :rtype: bool
+        :return: The job of this RimeStartContinuousTestResponse.  # noqa: E501
+        :rtype: RimeJobMetadata
         """
-        return self._enabled
+        return self._job
 
-    @enabled.setter
-    def enabled(self, enabled):
-        """Sets the enabled of this GenerativefirewallPromptInjectionV2RuleConfig.
+    @job.setter
+    def job(self, job):
+        """Sets the job of this RimeStartContinuousTestResponse.
 
-        Whether the rule is enabled.  # noqa: E501
 
-        :param enabled: The enabled of this GenerativefirewallPromptInjectionV2RuleConfig.  # noqa: E501
-        :type: bool
+        :param job: The job of this RimeStartContinuousTestResponse.  # noqa: E501
+        :type: RimeJobMetadata
         """
 
-        self._enabled = enabled
+        self._job = job
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -82,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(GenerativefirewallPromptInjectionV2RuleConfig, dict):
+        if issubclass(RimeStartContinuousTestResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -98,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, GenerativefirewallPromptInjectionV2RuleConfig):
+        if not isinstance(other, RimeStartContinuousTestResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_output.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_output.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_sensitivity.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_detection_details.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_detection_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_unknown_external_source_rule_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_unknown_external_source_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_update_firewall_instance_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_update_firewall_instance_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,44 +34,47 @@
         'attack_objective': 'RimeAttackObjective',
         'objective_sub_category': 'GenerativetestingObjectiveSubCategory',
         'failing_examples': 'list[GenerativeTestingResultExample]',
         'severity': 'RimeSeverity',
         'owasp_standards': 'list[GenerativetestingGenerativeTestingResultStandardInfo]',
         'nist_standards': 'list[GenerativetestingGenerativeTestingResultStandardInfo]',
         'mitre_standards': 'list[GenerativetestingGenerativeTestingResultStandardInfo]',
-        'attacks_attempted': 'str'
+        'attacks_attempted': 'str',
+        'threat': 'GenerativetestingThreat'
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
         'mitre_standards': 'mitreStandards',
-        'attacks_attempted': 'attacksAttempted'
+        'attacks_attempted': 'attacksAttempted',
+        'threat': 'threat'
     }
 
-    def __init__(self, id=None, job_id=None, attack_technique=None, attack_objective=None, objective_sub_category=None, failing_examples=None, severity=None, owasp_standards=None, nist_standards=None, mitre_standards=None, attacks_attempted=None):  # noqa: E501
+    def __init__(self, id=None, job_id=None, attack_technique=None, attack_objective=None, objective_sub_category=None, failing_examples=None, severity=None, owasp_standards=None, nist_standards=None, mitre_standards=None, attacks_attempted=None, threat=None):  # noqa: E501
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
         self._attacks_attempted = None
+        self._threat = None
         self.discriminator = None
         if id is not None:
             self.id = id
         if job_id is not None:
             self.job_id = job_id
         if attack_technique is not None:
             self.attack_technique = attack_technique
@@ -87,14 +90,16 @@
             self.owasp_standards = owasp_standards
         if nist_standards is not None:
             self.nist_standards = nist_standards
         if mitre_standards is not None:
             self.mitre_standards = mitre_standards
         if attacks_attempted is not None:
             self.attacks_attempted = attacks_attempted
+        if threat is not None:
+            self.threat = threat
 
     @property
     def id(self):
         """Gets the id of this GenerativetestingGenerativeTestingResult.  # noqa: E501
 
 
         :return: The id of this GenerativetestingGenerativeTestingResult.  # noqa: E501
@@ -327,14 +332,35 @@
 
         :param attacks_attempted: The attacks_attempted of this GenerativetestingGenerativeTestingResult.  # noqa: E501
         :type: str
         """
 
         self._attacks_attempted = attacks_attempted
 
+    @property
+    def threat(self):
+        """Gets the threat of this GenerativetestingGenerativeTestingResult.  # noqa: E501
+
+
+        :return: The threat of this GenerativetestingGenerativeTestingResult.  # noqa: E501
+        :rtype: GenerativetestingThreat
+        """
+        return self._threat
+
+    @threat.setter
+    def threat(self, threat):
+        """Sets the threat of this GenerativetestingGenerativeTestingResult.
+
+
+        :param threat: The threat of this GenerativetestingGenerativeTestingResult.  # noqa: E501
+        :type: GenerativetestingThreat
+        """
+
+        self._threat = threat
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result_standard_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result_standard_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_request_query.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_objective_sub_category.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativetesting_objective_sub_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,40 +28,45 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'url': 'str',
         'http_headers': 'dict(str, str)',
         'endpoint_payload_template': 'str',
         'response_json_path': 'str',
-        'http_auth_integration_id': 'RimeUUID'
+        'http_auth_integration_id': 'RimeUUID',
+        'name': 'str'
     }
 
     attribute_map = {
         'url': 'url',
         'http_headers': 'httpHeaders',
         'endpoint_payload_template': 'endpointPayloadTemplate',
         'response_json_path': 'responseJsonPath',
-        'http_auth_integration_id': 'httpAuthIntegrationId'
+        'http_auth_integration_id': 'httpAuthIntegrationId',
+        'name': 'name'
     }
 
-    def __init__(self, url=None, http_headers=None, endpoint_payload_template=None, response_json_path=None, http_auth_integration_id=None):  # noqa: E501
+    def __init__(self, url=None, http_headers=None, endpoint_payload_template=None, response_json_path=None, http_auth_integration_id=None, name=None):  # noqa: E501
         """GenerativetestingStartGenerativeModelTestRequest - a model defined in Swagger"""  # noqa: E501
         self._url = None
         self._http_headers = None
         self._endpoint_payload_template = None
         self._response_json_path = None
         self._http_auth_integration_id = None
+        self._name = None
         self.discriminator = None
         self.url = url
         if http_headers is not None:
             self.http_headers = http_headers
         self.endpoint_payload_template = endpoint_payload_template
         self.response_json_path = response_json_path
         if http_auth_integration_id is not None:
             self.http_auth_integration_id = http_auth_integration_id
+        if name is not None:
+            self.name = name
 
     @property
     def url(self):
         """Gets the url of this GenerativetestingStartGenerativeModelTestRequest.  # noqa: E501
 
         Parameters for connecting to the user's generative model.  # noqa: E501
 
@@ -170,14 +175,37 @@
 
         :param http_auth_integration_id: The http_auth_integration_id of this GenerativetestingStartGenerativeModelTestRequest.  # noqa: E501
         :type: RimeUUID
         """
 
         self._http_auth_integration_id = http_auth_integration_id
 
+    @property
+    def name(self):
+        """Gets the name of this GenerativetestingStartGenerativeModelTestRequest.  # noqa: E501
+
+        The name to identify the generative model testing job.  # noqa: E501
+
+        :return: The name of this GenerativetestingStartGenerativeModelTestRequest.  # noqa: E501
+        :rtype: str
+        """
+        return self._name
+
+    @name.setter
+    def name(self, name):
+        """Sets the name of this GenerativetestingStartGenerativeModelTestRequest.
+
+        The name to identify the generative model testing job.  # noqa: E501
+
+        :param name: The name of this GenerativetestingStartGenerativeModelTestRequest.  # noqa: E501
+        :type: str
+        """
+
+        self._name = name
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/googlerpc_status.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_level.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/integration_integration_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/integration_integration_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/job_data_generative_model_test.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/job_data_generative_model_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,31 +25,36 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'workspace_id': 'RimeUUID',
-        'progress': 'RimeGenerativeModelTestProgress'
+        'progress': 'RimeGenerativeModelTestProgress',
+        'name': 'str'
     }
 
     attribute_map = {
         'workspace_id': 'workspaceId',
-        'progress': 'progress'
+        'progress': 'progress',
+        'name': 'name'
     }
 
-    def __init__(self, workspace_id=None, progress=None):  # noqa: E501
+    def __init__(self, workspace_id=None, progress=None, name=None):  # noqa: E501
         """JobDataGenerativeModelTest - a model defined in Swagger"""  # noqa: E501
         self._workspace_id = None
         self._progress = None
+        self._name = None
         self.discriminator = None
         if workspace_id is not None:
             self.workspace_id = workspace_id
         if progress is not None:
             self.progress = progress
+        if name is not None:
+            self.name = name
 
     @property
     def workspace_id(self):
         """Gets the workspace_id of this JobDataGenerativeModelTest.  # noqa: E501
 
 
         :return: The workspace_id of this JobDataGenerativeModelTest.  # noqa: E501
@@ -85,14 +90,35 @@
 
         :param progress: The progress of this JobDataGenerativeModelTest.  # noqa: E501
         :type: RimeGenerativeModelTestProgress
         """
 
         self._progress = progress
 
+    @property
+    def name(self):
+        """Gets the name of this JobDataGenerativeModelTest.  # noqa: E501
+
+
+        :return: The name of this JobDataGenerativeModelTest.  # noqa: E501
+        :rtype: str
+        """
+        return self._name
+
+    @name.setter
+    def name(self, name):
+        """Sets the name of this JobDataGenerativeModelTest.
+
+
+        :param name: The name of this JobDataGenerativeModelTest.  # noqa: E501
+        :type: str
+        """
+
+        self._name = name
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/job_data_scan.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/job_data_scan.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/language_detection_details_language_substring.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/language_detection_details_language_substring.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,31 +25,36 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'agent_status_types': 'list[RimeAgentStatus]',
-        'agent_ids': 'list[str]'
+        'agent_ids': 'list[str]',
+        'type': 'RimeAgentType'
     }
 
     attribute_map = {
         'agent_status_types': 'agentStatusTypes',
-        'agent_ids': 'agentIds'
+        'agent_ids': 'agentIds',
+        'type': 'type'
     }
 
-    def __init__(self, agent_status_types=None, agent_ids=None):  # noqa: E501
+    def __init__(self, agent_status_types=None, agent_ids=None, type=None):  # noqa: E501
         """ListAgentsRequestListAgentsQuery - a model defined in Swagger"""  # noqa: E501
         self._agent_status_types = None
         self._agent_ids = None
+        self._type = None
         self.discriminator = None
         if agent_status_types is not None:
             self.agent_status_types = agent_status_types
         if agent_ids is not None:
             self.agent_ids = agent_ids
+        if type is not None:
+            self.type = type
 
     @property
     def agent_status_types(self):
         """Gets the agent_status_types of this ListAgentsRequestListAgentsQuery.  # noqa: E501
 
         Specifies a set of agent status types. The query filters for results that match the specified types.  # noqa: E501
 
@@ -89,14 +94,35 @@
 
         :param agent_ids: The agent_ids of this ListAgentsRequestListAgentsQuery.  # noqa: E501
         :type: list[str]
         """
 
         self._agent_ids = agent_ids
 
+    @property
+    def type(self):
+        """Gets the type of this ListAgentsRequestListAgentsQuery.  # noqa: E501
+
+
+        :return: The type of this ListAgentsRequestListAgentsQuery.  # noqa: E501
+        :rtype: RimeAgentType
+        """
+        return self._type
+
+    @type.setter
+    def type(self, type):
+        """Sets the type of this ListAgentsRequestListAgentsQuery.
+
+
+        :param type: The type of this ListAgentsRequestListAgentsQuery.  # noqa: E501
+        :type: RimeAgentType
+        """
+
+        self._type = type
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_file_scan_results_request_file_scan_query.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_file_scan_results_request_file_scan_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/model_model.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/model_model.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_monitor.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_threshold.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_threshold.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitor_transform.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitor_transform.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_digest_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/notification_digest_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_notification.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/notification_notification.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_notification_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/notification_notification_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_object_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/notification_object_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/pii_detection_details_flagged_entity.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/pii_detection_details_flagged_entity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_activate_schedule_for_project_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_activate_schedule_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_create_project_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_create_project_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_create_project_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_create_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_deactivate_schedule_for_project_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_deactivate_schedule_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_get_project_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_get_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_owner_details.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_project.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_project.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_project_status.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_project_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_project_with_details.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_project_with_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_schedule_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_schedule_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_update_project_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_update_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/protobuf_any.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_connection_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_connection_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_params.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_data_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_data_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_generative_language_model_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_generative_language_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_metadata.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_open_ai_chat_completion_model_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_open_ai_chat_completion_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_pred_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_pred_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registry_validity_status.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registry_validity_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/repo_metadata_reputation.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/repo_metadata_reputation.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_actor_role.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_actor_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,38 +31,41 @@
         'agent_id': 'RimeUUID',
         'name': 'str',
         'creation_time': 'datetime',
         'status': 'RimeAgentStatus',
         'internal': 'bool',
         'last_heartbeat_time': 'datetime',
         'version': 'str',
-        'desired_state': 'RimeAgentDesiredState'
+        'desired_state': 'RimeAgentDesiredState',
+        'type': 'RimeAgentType'
     }
 
     attribute_map = {
         'agent_id': 'agentId',
         'name': 'name',
         'creation_time': 'creationTime',
         'status': 'status',
         'internal': 'internal',
         'last_heartbeat_time': 'lastHeartbeatTime',
         'version': 'version',
-        'desired_state': 'desiredState'
+        'desired_state': 'desiredState',
+        'type': 'type'
     }
 
-    def __init__(self, agent_id=None, name=None, creation_time=None, status=None, internal=None, last_heartbeat_time=None, version=None, desired_state=None):  # noqa: E501
+    def __init__(self, agent_id=None, name=None, creation_time=None, status=None, internal=None, last_heartbeat_time=None, version=None, desired_state=None, type=None):  # noqa: E501
         """RimeAgent - a model defined in Swagger"""  # noqa: E501
         self._agent_id = None
         self._name = None
         self._creation_time = None
         self._status = None
         self._internal = None
         self._last_heartbeat_time = None
         self._version = None
         self._desired_state = None
+        self._type = None
         self.discriminator = None
         if agent_id is not None:
             self.agent_id = agent_id
         if name is not None:
             self.name = name
         if creation_time is not None:
             self.creation_time = creation_time
@@ -72,14 +75,16 @@
             self.internal = internal
         if last_heartbeat_time is not None:
             self.last_heartbeat_time = last_heartbeat_time
         if version is not None:
             self.version = version
         if desired_state is not None:
             self.desired_state = desired_state
+        if type is not None:
+            self.type = type
 
     @property
     def agent_id(self):
         """Gets the agent_id of this RimeAgent.  # noqa: E501
 
 
         :return: The agent_id of this RimeAgent.  # noqa: E501
@@ -251,14 +256,35 @@
 
         :param desired_state: The desired_state of this RimeAgent.  # noqa: E501
         :type: RimeAgentDesiredState
         """
 
         self._desired_state = desired_state
 
+    @property
+    def type(self):
+        """Gets the type of this RimeAgent.  # noqa: E501
+
+
+        :return: The type of this RimeAgent.  # noqa: E501
+        :rtype: RimeAgentType
+        """
+        return self._type
+
+    @type.setter
+    def type(self, type):
+        """Sets the type of this RimeAgent.
+
+
+        :param type: The type of this RimeAgent.  # noqa: E501
+        :type: RimeAgentType
+        """
+
+        self._type = type
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent_desired_state.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_agent_desired_state.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent_status.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_agent_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_attack_objective.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_attack_objective.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_category_metric.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_category_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_config_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_config_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_schedule_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_schedule_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_schedule_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_schedule_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_schedule_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_schedule_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_detailed_upgrade_status.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_detailed_upgrade_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_failing_row.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_failing_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_feature_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_feature_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_float_list.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_float_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_generative_model_test_progress.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_generative_model_test_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_file_scan_result_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_file_scan_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_schedule_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_schedule_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_time_series_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_time_series_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_upgrade_for_agent_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_upgrade_for_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_image_reference.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_image_reference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_int_list.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_int_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_integration_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_integration_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_data.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_data.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_view.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_view.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_language.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_language.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_license_feature.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_license_feature.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_license_limit.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_license_limit.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_limit_status.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_limit_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_managed_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image_package_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_managed_image_package_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_card.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_task.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_model_task.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_named_double.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_named_double.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_order.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_order.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_safe_url.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_safe_url.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_search_spec.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_search_spec.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_severity.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_str_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,61 +11,61 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeStartContinuousTestResponse(object):
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
-        'job': 'RimeJobMetadata'
+        'values': 'list[str]'
     }
 
     attribute_map = {
-        'job': 'job'
+        'values': 'values'
     }
 
-    def __init__(self, job=None):  # noqa: E501
-        """RimeStartContinuousTestResponse - a model defined in Swagger"""  # noqa: E501
-        self._job = None
+    def __init__(self, values=None):  # noqa: E501
+        """RimeStrList - a model defined in Swagger"""  # noqa: E501
+        self._values = None
         self.discriminator = None
-        if job is not None:
-            self.job = job
+        if values is not None:
+            self.values = values
 
     @property
-    def job(self):
-        """Gets the job of this RimeStartContinuousTestResponse.  # noqa: E501
+    def values(self):
+        """Gets the values of this RimeStrList.  # noqa: E501
 
 
-        :return: The job of this RimeStartContinuousTestResponse.  # noqa: E501
-        :rtype: RimeJobMetadata
+        :return: The values of this RimeStrList.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._job
+        return self._values
 
-    @job.setter
-    def job(self, job):
-        """Sets the job of this RimeStartContinuousTestResponse.
+    @values.setter
+    def values(self, values):
+        """Sets the values of this RimeStrList.
 
 
-        :param job: The job of this RimeStartContinuousTestResponse.  # noqa: E501
-        :type: RimeJobMetadata
+        :param values: The values of this RimeStrList.  # noqa: E501
+        :type: list[str]
         """
 
-        self._job = job
+        self._values = values
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeStartContinuousTestResponse, dict):
+        if issubclass(RimeStrList, dict):
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
-        if not isinstance(other, RimeStartContinuousTestResponse):
+        if not isinstance(other, RimeStrList):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_str_list.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/generativetesting_threat.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,61 +11,50 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeStrList(object):
+class GenerativetestingThreat(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
+
+    """
+    allowed enum values
+    """
+    UNSPECIFIED = "THREAT_UNSPECIFIED"
+    VIOLENCE = "THREAT_VIOLENCE"
+    ILLEGAL_ACTIVITIES = "THREAT_ILLEGAL_ACTIVITIES"
+    DATA_EXTRACTION = "THREAT_DATA_EXTRACTION"
+    SENSITIVE_INFORMATION_DISCLOSURE = "THREAT_SENSITIVE_INFORMATION_DISCLOSURE"
+    HUMAN_EXPLOITATION = "THREAT_HUMAN_EXPLOITATION"
+    PROPAGATING_MISINFORMATION = "THREAT_PROPAGATING_MISINFORMATION"
+    MALICIOUS_CODE_GENERATION = "THREAT_MALICIOUS_CODE_GENERATION"
+    META_PROMPT_EXTRACTION = "THREAT_META_PROMPT_EXTRACTION"
+    SELF_HARM = "THREAT_SELF_HARM"
+    UNETHICAL_ACTIONS = "THREAT_UNETHICAL_ACTIONS"
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
+        """GenerativetestingThreat - a model defined in Swagger"""  # noqa: E501
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
@@ -80,15 +69,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeStrList, dict):
+        if issubclass(GenerativetestingThreat, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +85,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeStrList):
+        if not isinstance(other, GenerativetestingThreat):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_subject_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_subject_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_suggestion.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_suggestion.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_table_column.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_table_column.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_metric.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_time_interval.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_time_interval.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_token_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_token_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_toxicity_threat_category.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_toxicity_threat_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_schedule_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_schedule_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_upgrade_status_for_agent_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_upgrade_status_for_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_upgrade_agent_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_upgrade_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_upgrade_status.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_upgrade_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_role.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_uuid.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_uuid.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_workspace.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/role_users_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/role_users_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/role_workspace_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/role_workspace_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rule_output_rule_evaluation_metadata.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rule_output_rule_evaluation_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/rule_output_rule_evaluation_metadata_model_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/rule_output_rule_evaluation_metadata_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_activate_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_activate_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_deactivate_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_deactivate_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schedule_schedule.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/schedule_schedule.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schedules_schedule_schedule_id_uuid_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/schedules_schedule_schedule_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemafilescanning_package_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/schemafilescanning_package_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemanotification_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/schemanotification_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/schemaregistry_model_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/schemaregistry_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/statedb_job_status.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/statedb_job_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_category_results_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_category_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/user_private_info.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/user_private_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/user_role.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/user_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/user_user_detail.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/user_user_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body1.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body1.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validate_request_input.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/validate_request_input.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validate_request_output.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/validate_request_output.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validate_response_processed_request.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/validate_response_processed_request.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,101 +24,103 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'request_id': 'RimeUUID',
-        'input_truncated': 'str',
+        'request_id': 'str',
+        'user_input_text': 'str',
         'input_token_count': 'int',
-        'contexts_truncated': 'str',
+        'contexts': 'list[str]',
         'contexts_token_count': 'int',
-        'output_truncated': 'str',
+        'output_text': 'str',
         'output_token_count': 'int'
     }
 
     attribute_map = {
         'request_id': 'requestId',
-        'input_truncated': 'inputTruncated',
+        'user_input_text': 'userInputText',
         'input_token_count': 'inputTokenCount',
-        'contexts_truncated': 'contextsTruncated',
+        'contexts': 'contexts',
         'contexts_token_count': 'contextsTokenCount',
-        'output_truncated': 'outputTruncated',
+        'output_text': 'outputText',
         'output_token_count': 'outputTokenCount'
     }
 
-    def __init__(self, request_id=None, input_truncated=None, input_token_count=None, contexts_truncated=None, contexts_token_count=None, output_truncated=None, output_token_count=None):  # noqa: E501
+    def __init__(self, request_id=None, user_input_text=None, input_token_count=None, contexts=None, contexts_token_count=None, output_text=None, output_token_count=None):  # noqa: E501
         """ValidateResponseProcessedRequest - a model defined in Swagger"""  # noqa: E501
         self._request_id = None
-        self._input_truncated = None
+        self._user_input_text = None
         self._input_token_count = None
-        self._contexts_truncated = None
+        self._contexts = None
         self._contexts_token_count = None
-        self._output_truncated = None
+        self._output_text = None
         self._output_token_count = None
         self.discriminator = None
         if request_id is not None:
             self.request_id = request_id
-        if input_truncated is not None:
-            self.input_truncated = input_truncated
+        if user_input_text is not None:
+            self.user_input_text = user_input_text
         if input_token_count is not None:
             self.input_token_count = input_token_count
-        if contexts_truncated is not None:
-            self.contexts_truncated = contexts_truncated
+        if contexts is not None:
+            self.contexts = contexts
         if contexts_token_count is not None:
             self.contexts_token_count = contexts_token_count
-        if output_truncated is not None:
-            self.output_truncated = output_truncated
+        if output_text is not None:
+            self.output_text = output_text
         if output_token_count is not None:
             self.output_token_count = output_token_count
 
     @property
     def request_id(self):
         """Gets the request_id of this ValidateResponseProcessedRequest.  # noqa: E501
 
+        Unique identifier of the request.  # noqa: E501
 
         :return: The request_id of this ValidateResponseProcessedRequest.  # noqa: E501
-        :rtype: RimeUUID
+        :rtype: str
         """
         return self._request_id
 
     @request_id.setter
     def request_id(self, request_id):
         """Sets the request_id of this ValidateResponseProcessedRequest.
 
+        Unique identifier of the request.  # noqa: E501
 
         :param request_id: The request_id of this ValidateResponseProcessedRequest.  # noqa: E501
-        :type: RimeUUID
+        :type: str
         """
 
         self._request_id = request_id
 
     @property
-    def input_truncated(self):
-        """Gets the input_truncated of this ValidateResponseProcessedRequest.  # noqa: E501
+    def user_input_text(self):
+        """Gets the user_input_text of this ValidateResponseProcessedRequest.  # noqa: E501
 
         Information about the `user_input_text`. The raw input is truncated if it exceeds a certain token length so we do not denial of service downstream logging and data systems.  # noqa: E501
 
-        :return: The input_truncated of this ValidateResponseProcessedRequest.  # noqa: E501
+        :return: The user_input_text of this ValidateResponseProcessedRequest.  # noqa: E501
         :rtype: str
         """
-        return self._input_truncated
+        return self._user_input_text
 
-    @input_truncated.setter
-    def input_truncated(self, input_truncated):
-        """Sets the input_truncated of this ValidateResponseProcessedRequest.
+    @user_input_text.setter
+    def user_input_text(self, user_input_text):
+        """Sets the user_input_text of this ValidateResponseProcessedRequest.
 
         Information about the `user_input_text`. The raw input is truncated if it exceeds a certain token length so we do not denial of service downstream logging and data systems.  # noqa: E501
 
-        :param input_truncated: The input_truncated of this ValidateResponseProcessedRequest.  # noqa: E501
+        :param user_input_text: The user_input_text of this ValidateResponseProcessedRequest.  # noqa: E501
         :type: str
         """
 
-        self._input_truncated = input_truncated
+        self._user_input_text = user_input_text
 
     @property
     def input_token_count(self):
         """Gets the input_token_count of this ValidateResponseProcessedRequest.  # noqa: E501
 
 
         :return: The input_token_count of this ValidateResponseProcessedRequest.  # noqa: E501
@@ -134,35 +136,35 @@
         :param input_token_count: The input_token_count of this ValidateResponseProcessedRequest.  # noqa: E501
         :type: int
         """
 
         self._input_token_count = input_token_count
 
     @property
-    def contexts_truncated(self):
-        """Gets the contexts_truncated of this ValidateResponseProcessedRequest.  # noqa: E501
+    def contexts(self):
+        """Gets the contexts of this ValidateResponseProcessedRequest.  # noqa: E501
 
         Information about the `contexts`. The contexts are truncated if it exceeds a certain token length so we do not denial of service downstream logging and data systems.  # noqa: E501
 
-        :return: The contexts_truncated of this ValidateResponseProcessedRequest.  # noqa: E501
-        :rtype: str
+        :return: The contexts of this ValidateResponseProcessedRequest.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._contexts_truncated
+        return self._contexts
 
-    @contexts_truncated.setter
-    def contexts_truncated(self, contexts_truncated):
-        """Sets the contexts_truncated of this ValidateResponseProcessedRequest.
+    @contexts.setter
+    def contexts(self, contexts):
+        """Sets the contexts of this ValidateResponseProcessedRequest.
 
         Information about the `contexts`. The contexts are truncated if it exceeds a certain token length so we do not denial of service downstream logging and data systems.  # noqa: E501
 
-        :param contexts_truncated: The contexts_truncated of this ValidateResponseProcessedRequest.  # noqa: E501
-        :type: str
+        :param contexts: The contexts of this ValidateResponseProcessedRequest.  # noqa: E501
+        :type: list[str]
         """
 
-        self._contexts_truncated = contexts_truncated
+        self._contexts = contexts
 
     @property
     def contexts_token_count(self):
         """Gets the contexts_token_count of this ValidateResponseProcessedRequest.  # noqa: E501
 
 
         :return: The contexts_token_count of this ValidateResponseProcessedRequest.  # noqa: E501
@@ -178,35 +180,35 @@
         :param contexts_token_count: The contexts_token_count of this ValidateResponseProcessedRequest.  # noqa: E501
         :type: int
         """
 
         self._contexts_token_count = contexts_token_count
 
     @property
-    def output_truncated(self):
-        """Gets the output_truncated of this ValidateResponseProcessedRequest.  # noqa: E501
+    def output_text(self):
+        """Gets the output_text of this ValidateResponseProcessedRequest.  # noqa: E501
 
         Information about the `output_text`. The output text is truncated if it exceeds a certain token length so we do not denial of service downstream logging and data systems.  # noqa: E501
 
-        :return: The output_truncated of this ValidateResponseProcessedRequest.  # noqa: E501
+        :return: The output_text of this ValidateResponseProcessedRequest.  # noqa: E501
         :rtype: str
         """
-        return self._output_truncated
+        return self._output_text
 
-    @output_truncated.setter
-    def output_truncated(self, output_truncated):
-        """Sets the output_truncated of this ValidateResponseProcessedRequest.
+    @output_text.setter
+    def output_text(self, output_text):
+        """Sets the output_text of this ValidateResponseProcessedRequest.
 
         Information about the `output_text`. The output text is truncated if it exceeds a certain token length so we do not denial of service downstream logging and data systems.  # noqa: E501
 
-        :param output_truncated: The output_truncated of this ValidateResponseProcessedRequest.  # noqa: E501
+        :param output_text: The output_text of this ValidateResponseProcessedRequest.  # noqa: E501
         :type: str
         """
 
-        self._output_truncated = output_truncated
+        self._output_text = output_text
 
     @property
     def output_token_count(self):
         """Gets the output_token_count of this ValidateResponseProcessedRequest.  # noqa: E501
 
 
         :return: The output_token_count of this ValidateResponseProcessedRequest.  # noqa: E501
```

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validate_response_product_metadata.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/validate_response_product_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/swagger/swagger_client/rest.py` & `rime_sdk-2.8.0rc7/rime_sdk/swagger/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/test_batch.py` & `rime_sdk-2.8.0rc7/rime_sdk/test_batch.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk/test_run.py` & `rime_sdk-2.8.0rc7/rime_sdk/test_run.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc6/rime_sdk.egg-info/PKG-INFO` & `rime_sdk-2.8.0rc7/rime_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime-sdk
-Version: 2.8.0rc6
+Version: 2.8.0rc7
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.8.0rc6/rime_sdk.egg-info/SOURCES.txt` & `rime_sdk-2.8.0rc7/rime_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 rime_sdk/swagger/swagger_client/api/schedule_service_api.py
 rime_sdk/swagger/swagger_client/api/user_api.py
 rime_sdk/swagger/swagger_client/api/validation_service_api.py
 rime_sdk/swagger/swagger_client/api/workspace_service_api.py
 rime_sdk/swagger/swagger_client/models/__init__.py
 rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body.py
 rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body1.py
+rime_sdk/swagger/swagger_client/models/apigenerativefirewall_list_firewall_instances_response.py
 rime_sdk/swagger/swagger_client/models/apigenerativefirewall_standard_info.py
 rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
 rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
 rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
 rime_sdk/swagger/swagger_client/models/config_generation_category_config_generation_service_response.py
 rime_sdk/swagger/swagger_client/models/config_generation_profiling_config_generation_service_response.py
 rime_sdk/swagger/swagger_client/models/config_generation_test_suite_config_generation_service_response.py
@@ -143,35 +144,37 @@
 rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_tokenizer.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_flagged_substring.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_effective_config_response.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_instance_response.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_individual_rules_config.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_details.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_rule_config.py
-rime_sdk/swagger/swagger_client/models/generativefirewall_list_firewall_instances_response.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_off_topic_rule_config.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_details.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_rule_config.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_pii_entity_type.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_details.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_v2_rule_config.py
+rime_sdk/swagger/swagger_client/models/generativefirewall_rule_false_positive_rate.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_rule_output.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_rule_sensitivity.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_detection_details.py
+rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_rule_config.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_unknown_external_source_rule_config.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_update_firewall_instance_response.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_validate_response.py
 rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result.py
 rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result_standard_info.py
 rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_request_query.py
 rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_response.py
 rime_sdk/swagger/swagger_client/models/generativetesting_objective_sub_category.py
 rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_request.py
 rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_response.py
+rime_sdk/swagger/swagger_client/models/generativetesting_threat.py
 rime_sdk/swagger/swagger_client/models/googlerpc_status.py
 rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
 rime_sdk/swagger/swagger_client/models/integration_integration_level.py
 rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
 rime_sdk/swagger/swagger_client/models/integration_integration_type.py
 rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
@@ -180,14 +183,15 @@
 rime_sdk/swagger/swagger_client/models/job_data_generative_model_test.py
 rime_sdk/swagger/swagger_client/models/job_data_scan.py
 rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
 rime_sdk/swagger/swagger_client/models/language_detection_details_language_substring.py
 rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
 rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
 rime_sdk/swagger/swagger_client/models/list_file_scan_results_request_file_scan_query.py
+rime_sdk/swagger/swagger_client/models/list_firewall_instances_request_list_firewall_instances_query.py
 rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
 rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
 rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
 rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
 rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
 rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
 rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
@@ -274,14 +278,15 @@
 rime_sdk/swagger/swagger_client/models/repo_metadata_reputation.py
 rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/rime_actor_role.py
 rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
 rime_sdk/swagger/swagger_client/models/rime_agent.py
 rime_sdk/swagger/swagger_client/models/rime_agent_desired_state.py
 rime_sdk/swagger/swagger_client/models/rime_agent_status.py
+rime_sdk/swagger/swagger_client/models/rime_agent_type.py
 rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
 rime_sdk/swagger/swagger_client/models/rime_attack_objective.py
 rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
 rime_sdk/swagger/swagger_client/models/rime_category_metric.py
 rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
 rime_sdk/swagger/swagger_client/models/rime_config_type.py
 rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
@@ -291,14 +296,16 @@
 rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
 rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
 rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
 rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
 rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
 rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py
 rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py
+rime_sdk/swagger/swagger_client/models/rime_create_firewall_agent_request.py
+rime_sdk/swagger/swagger_client/models/rime_create_firewall_agent_response.py
 rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
 rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
 rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
 rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
 rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
 rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
 rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
@@ -383,14 +390,15 @@
 rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
 rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
+rime_sdk/swagger/swagger_client/models/rime_list_firewall_instances_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
 rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
 rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
@@ -415,14 +423,16 @@
 rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
 rime_sdk/swagger/swagger_client/models/rime_named_double.py
 rime_sdk/swagger/swagger_client/models/rime_order.py
 rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
 rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
 rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
 rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py
+rime_sdk/swagger/swagger_client/models/rime_register_firewall_agent_request.py
+rime_sdk/swagger/swagger_client/models/rime_register_firewall_agent_response.py
 rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
 rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
 rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
 rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
 rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
 rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
 rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
```

### Comparing `rime_sdk-2.8.0rc6/setup.py` & `rime_sdk-2.8.0rc7/setup.py`

 * *Files identical despite different names*

