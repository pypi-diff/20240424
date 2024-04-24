# Comparing `tmp/waylay_sdk_registry_types-2.13.0b20240415.tar.gz` & `tmp/waylay-sdk-registry-types-2.13.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk_registry_types-2.13.0b20240415.tar", last modified: Mon Apr 15 08:45:54 2024, max compression
+gzip compressed data, was "waylay-sdk-registry-types-2.13.0rc0.tar", last modified: Fri Mar 29 13:21:52 2024, max compression
```

## Comparing `waylay_sdk_registry_types-2.13.0b20240415.tar` & `waylay-sdk-registry-types-2.13.0rc0.tar`

### file list

```diff
@@ -1,416 +1,414 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:54.314009 waylay_sdk_registry_types-2.13.0b20240415/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-04-15 08:45:54.314009 waylay_sdk_registry_types-2.13.0b20240415/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:45:54.314009 waylay_sdk_registry_types-2.13.0b20240415/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:54.234010 waylay_sdk_registry_types-2.13.0b20240415/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:54.230010 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:54.230010 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:54.234010 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:54.306009 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/
--rw-r--r--   0 runner    (1001) docker     (127)    32761 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/active_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/active_event_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/active_event_sse_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/alt_embedded_version_i_kfserving_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/alt_embedded_version_i_plug_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/alt_embedded_version_i_webscript_response_with_invoke_link_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/alt_version_hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/any_function_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/any_job_for_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/any_job_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/any_job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/any_job_status_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/archive_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/asset_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/asset_condition_content_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/asset_condition_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/asset_path_params_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/asset_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/asset_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/asset_summary_with_hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/asset_summary_with_hal_link_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/assets_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/async_deploy_query_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/async_query_default_false.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/async_verify_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/batch_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/batch_job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/batch_job_status_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/batch_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/build1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/build_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/build_job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/build_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/build_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/build_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/cleanup_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/compiled_runtime_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/completed_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/completed_event_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/completed_event_sse_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/content_query_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/content_validation_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/create_function_query_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/create_function_query_v2_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/create_kf_serving_async_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/create_plug_async_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/create_webscript_async_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/create_webscripts_copy_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/delayed_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/delayed_event_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/delayed_event_sse_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/deploy1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/deploy_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/deploy_args_deploy_spec_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/deploy_job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/deploy_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/deploy_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/deploy_spec_openfaas_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/deploy_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/deprecate_previous_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/documentation_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/entity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/entity_with_links_i_kfserving_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/entity_with_links_i_plug_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/entity_with_links_i_webscript_response_with_invoke_link_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/error_and_status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/event_ack.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/event_close.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/event_keep_alive.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/event_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/event_type_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/event_with_close_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/example_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/exposed_openfaas_deploy_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/failed_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/failed_event_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/failed_event_sse_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/failure_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/file_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/force_delete_query_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/function_deploy_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/function_deploy_overrides_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/function_job_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/function_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/function_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/function_name_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/function_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/function_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/function_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_content_params_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_invokable_webscript_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_model_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_plug_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_plug_response_v2_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_plug_response_v2_links_draft.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_plug_response_v2_links_published.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_runtime_by_name_and_version_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_runtime_by_name_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_runtime_example_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_runtime_versions_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_webscript_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_webscript_response_v2_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/invokable_webscript_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/invokable_webscript_response_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/invokable_webscript_response_entity_webscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/invoke_hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/invoke_internal_hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_and_function_hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_cause.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_causes.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_payload_active_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_payload_completed_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_payload_delayed_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_payload_failed_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_payload_waiting_children_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_payload_waiting_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_response_active_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_response_completed_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_response_delayed_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_response_failed_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_response_waiting_children_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_response_waiting_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_events_and_function_hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_events_filter_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_events_hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_hal_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_reference_params.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_state_active.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_state_completed.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_state_delayed.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_state_failed.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_state_finished.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_state_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_state_unknown.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_state_waiting.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_state_waiting_children.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_status_and_entity_hal_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_status_hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_status_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_submitted_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_type_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_type_build.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_type_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_type_notify.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_type_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_type_undeploy.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_type_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/jobs_for_model_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/jobs_for_model_response_v2_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/jobs_for_plug_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/jobs_for_plug_response_v2_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/jobs_for_webscript_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/jobs_for_webscript_response_v2_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/jobs_hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/jobs_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/keep_alive_event_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_delete_multiple_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_delete_multiple_with_job_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_delete_query_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_delete_query_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_delete_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_delete_with_job_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_latest_version_query_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_latest_versions_query_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_latest_versions_query_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_models_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_versions_query_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kfserving_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/language_release.py
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/latest_function_versions_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/latest_function_versions_query_show_related.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/latest_functions_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/latest_models_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/latest_plug_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/latest_plug_version_query_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/latest_plug_versions_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/latest_plug_versions_query_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/latest_plugs_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/latest_plugs_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/latest_version_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/latest_webscripts_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_configuration_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_configuration_object_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_configuration_response_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_create_debug_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_debug_plug_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_debug_plug_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_documentation_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_function_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_create_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_meta_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_request_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_request_metadata_documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_request_metadata_documentation_any_of.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_request_metadata_raw_data_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_response_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_script_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_script_meta_raw_data_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_script_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_required_properties_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_required_property_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/media_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/message_and_status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/model1.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/model2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/model_versions_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/name.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/name_and_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/named_kf_serving_versions_query_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/named_parameters_typeof_as_job_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/named_parameters_typeof_as_job_reference_job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/named_parameters_typeof_from_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/named_parameters_typeof_from_legacy_documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/named_parameters_typeof_is_not_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/named_plug_versions_query_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/named_webscript_versions_query_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/notify_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/object.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/openfaas_deploy_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/openfaas_function_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/operation_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/operation_status_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/paging_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/parent_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/patch_interface_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/patch_metadata_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/patch_plug_request_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug1.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug2.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_delete_force_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_listing_and_query_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_listing_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_property_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_property_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_property_format_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_versions_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/post_model_job_async_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/post_model_job_sync_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/post_plug_job_async_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/post_plug_job_sync_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/post_webscript_job_async_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/post_webscript_job_sync_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/provided_dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/publish_function_query.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/queue_events.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/rebuild_computed_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/rebuild_model_async_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/rebuild_model_sync_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/rebuild_plug_async_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/rebuild_plug_sync_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/rebuild_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/rebuild_query_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/rebuild_submitted_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/rebuild_webscript_async_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/rebuild_webscript_sync_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/registry_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/remove_function_query_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/remove_plug_query_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/request_deploy_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/request_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/resource_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/root_page_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_name_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_summary_attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_version_and_path_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_version_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_version_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_version_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_version_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_version_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_version_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_version_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/scale1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/scale_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/scale_job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/scale_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/schema_by_id_params.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/schema_params.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/semantic_version_range.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/show_related_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/status.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/status_any.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/status_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/status_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/status_include.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/stream_closing.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/stream_ready.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/supported_events.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/tag_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/tags_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/timestamp_absolute.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/timestamp_age.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/timestamp_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/undeploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/undeploy1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/undeploy_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/undeploy_job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/undeploy_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/undeploy_submitted_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/undeploy_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/undeployed_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/unhealthy_invokable_webscript_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/update_draft_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/update_metadata_request_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/update_metadata_request_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/update_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/user_plug_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/verify1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/verify_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/verify_job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/verify_model_sync_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/verify_plug_sync_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/verify_query_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/verify_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/verify_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/verify_webscript_sync_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/version_includes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/versions_query_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/versions_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/waiting_children_event_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/waiting_children_event_sse_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/waiting_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/waiting_event_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/waiting_event_sse_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/webscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/webscript1.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/webscript2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/webscript_latest_version_query_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/webscript_latest_versions_query_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/webscript_latest_versions_query_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/webscript_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/webscript_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/webscript_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/webscript_response_with_invoke_link_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/webscript_versions_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/with_asset_hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/with_embedded_alt_versions_i_kfserving_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/with_embedded_alt_versions_i_plug_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/with_embedded_alt_versions_i_webscript_response_with_invoke_link_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/with_entity_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/with_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/with_paging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:54.310009 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/queries/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/queries/about_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/queries/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    43474 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/queries/models_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    45043 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/queries/plugs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/queries/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9424 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/queries/runtimes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/queries/schemas_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    43474 2024-04-15 08:45:50.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/queries/webscripts_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:54.310009 waylay_sdk_registry_types-2.13.0b20240415/src/waylay_sdk_registry_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-04-15 08:45:54.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay_sdk_registry_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24733 2024-04-15 08:45:54.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay_sdk_registry_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:45:54.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay_sdk_registry_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-15 08:45:54.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay_sdk_registry_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 08:45:54.000000 waylay_sdk_registry_types-2.13.0b20240415/src/waylay_sdk_registry_types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.657172 waylay-sdk-registry-types-2.13.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-03-29 13:21:52.653172 waylay-sdk-registry-types-2.13.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 13:21:52.657172 waylay-sdk-registry-types-2.13.0rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.581172 waylay-sdk-registry-types-2.13.0rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.581172 waylay-sdk-registry-types-2.13.0rc0/src/waylay/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.581172 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.581172 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.649172 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    32620 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/active_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/active_event_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/active_event_sse_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/alt_embedded_version_i_kfserving_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/alt_embedded_version_i_plug_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/alt_embedded_version_i_webscript_response_with_invoke_link_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/alt_version_hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/any_function_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/any_job_for_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/any_job_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/any_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/any_job_status_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/archive_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_condition_content_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_condition_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_path_params_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_summary_with_hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_summary_with_hal_link_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/assets_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/async_deploy_query_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/async_query_default_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/async_verify_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/batch_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/batch_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/batch_job_status_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/batch_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/cleanup_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/compiled_runtime_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/completed_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/completed_event_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/completed_event_sse_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/content_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/content_validation_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/create_function_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/create_function_query_v2_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/create_kf_serving_async_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/create_plug_async_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/create_webscript_async_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/create_webscripts_copy_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/delayed_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/delayed_event_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/delayed_event_sse_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_args_deploy_spec_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_spec_openfaas_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deprecate_previous_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/documentation_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/entity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/entity_with_links_i_kfserving_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/entity_with_links_i_plug_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/entity_with_links_i_webscript_response_with_invoke_link_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/error_and_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/event_ack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/event_close.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/event_keep_alive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/event_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/event_type_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/event_with_close_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/example_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/exposed_openfaas_deploy_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/failed_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/failed_event_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/failed_event_sse_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/failure_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/force_delete_query_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_deploy_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_deploy_overrides_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_job_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_name_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_content_params_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_invokable_webscript_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_model_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_plug_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_plug_response_v2_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_plug_response_v2_links_draft.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_plug_response_v2_links_published.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_runtime_by_name_and_version_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_runtime_by_name_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_runtime_example_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_runtime_versions_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_webscript_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_webscript_response_v2_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/invokable_webscript_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/invokable_webscript_response_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/invokable_webscript_response_entity_webscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/invoke_hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/invoke_internal_hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_and_function_hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_cause.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_causes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_payload_active_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_payload_completed_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_payload_delayed_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_payload_failed_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_payload_waiting_children_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_payload_waiting_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_response_active_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_response_completed_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_response_delayed_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_response_failed_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_response_waiting_children_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_response_waiting_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_events_and_function_hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_events_filter_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_events_hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_hal_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_reference_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_completed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_delayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_failed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_finished.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_unknown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_waiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_waiting_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_status_and_entity_hal_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_status_hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_status_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_submitted_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_type_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_type_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_type_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_type_notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_type_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_type_undeploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_type_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_model_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_model_response_v2_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_plug_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_plug_response_v2_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_webscript_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_webscript_response_v2_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/keep_alive_event_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_delete_multiple_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_delete_multiple_with_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_delete_query_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_delete_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_delete_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_delete_with_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_latest_version_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_latest_versions_query_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_latest_versions_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_models_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_versions_query_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kfserving_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/language_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_function_versions_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_function_versions_query_show_related.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_functions_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_models_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_plug_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_plug_version_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_plug_versions_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_plug_versions_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_plugs_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_plugs_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_version_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_webscripts_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_configuration_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_configuration_object_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_configuration_response_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_create_debug_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_debug_plug_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_debug_plug_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_documentation_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_function_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_create_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_meta_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_request_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_request_metadata_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_request_metadata_documentation_any_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_request_metadata_raw_data_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_response_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_script_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_script_meta_raw_data_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_script_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_required_properties_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_required_property_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/media_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/message_and_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/model1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/model2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/model_versions_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/name_and_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_kf_serving_versions_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_parameters_typeof_as_job_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_parameters_typeof_as_job_reference_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_parameters_typeof_from_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_parameters_typeof_from_legacy_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_parameters_typeof_is_not_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_plug_versions_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_webscript_versions_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/notify_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/openfaas_deploy_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/openfaas_function_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/operation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/operation_status_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/paging_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/parent_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/patch_interface_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/patch_metadata_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/patch_plug_request_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_delete_force_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_listing_and_query_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_listing_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_property_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_property_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_property_format_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_versions_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/post_model_job_async_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/post_model_job_sync_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/post_plug_job_async_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/post_plug_job_sync_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/post_webscript_job_async_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/post_webscript_job_sync_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/provided_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/publish_function_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/queue_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_computed_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_model_async_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_model_sync_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_plug_async_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_plug_sync_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_submitted_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_webscript_async_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_webscript_sync_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/registry_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/remove_function_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/remove_plug_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/request_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/resource_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/root_page_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_name_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_summary_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_and_path_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/scale1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/scale_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/scale_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/scale_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/schema_by_id_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/schema_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/semantic_version_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/show_related_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/status_any.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/status_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/status_include.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/stream_closing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/stream_ready.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/supported_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/tag_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/tags_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/timestamp_absolute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/timestamp_age.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/timestamp_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy_submitted_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeployed_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/unhealthy_invokable_webscript_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/update_draft_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/update_metadata_request_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/update_metadata_request_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/update_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/user_plug_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_model_sync_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_plug_sync_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_query_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_webscript_sync_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/version_includes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/versions_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/versions_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/waiting_children_event_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/waiting_children_event_sse_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/waiting_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/waiting_event_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/waiting_event_sse_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_latest_version_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_latest_versions_query_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_latest_versions_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_response_with_invoke_link_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_versions_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/with_asset_hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/with_embedded_alt_versions_i_kfserving_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/with_embedded_alt_versions_i_plug_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/with_embedded_alt_versions_i_webscript_response_with_invoke_link_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/with_entity_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/with_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/with_paging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.653172 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39273 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/models_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40842 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/plugs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9424 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/runtimes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/schemas_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39273 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/webscripts_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.653172 waylay-sdk-registry-types-2.13.0rc0/src/waylay_sdk_registry_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-03-29 13:21:52.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay_sdk_registry_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24621 2024-03-29 13:21:52.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay_sdk_registry_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 13:21:52.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay_sdk_registry_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-29 13:21:52.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay_sdk_registry_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-29 13:21:52.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay_sdk_registry_types.egg-info/top_level.txt
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/LICENSE.txt` & `waylay-sdk-registry-types-2.13.0rc0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/PKG-INFO` & `waylay-sdk-registry-types-2.13.0rc0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-registry-types
-Version: 2.13.0b20240415
+Version: 2.13.0rc0
 Summary: Waylay Function Registry Types 
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,23 +13,22 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-registry-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/registry.html
 Keywords: Waylay Function Registry,Types
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.0
-Requires-Dist: waylay-sdk-registry==2.13.0b20240415
+Requires-Dist: waylay-sdk~=0.0.4rc5
+Requires-Dist: waylay-sdk-registry==2.13.0rc0
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -45,51 +44,56 @@
 Requires-Dist: pyyaml; extra == "dev"
 Requires-Dist: jsf>=0.11.1; extra == "dev"
 
 # Waylay Registry Service
 V2 API to build and deploy Waylay functions (plugs, webscripts, BYOML models).
 
 This Python package is automatically generated based on the 
-Waylay Registry OpenAPI specification (API version: 2.13.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/registry.html).
+Waylay Registry OpenAPI specification (API version: 2.13.0-beta.0)
 
 It is considered an extension of the waylay-sdk-registry package, and it consists of the typed model classes for all path params, query params, body params and responses for each of the api methods in `waylay-sdk-registry`.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-registry is included in:
-- ```pip install waylay-sdk-core[registry]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[registry]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-registry and waylay-sdk-registry-types are included in:
-- ```pip install waylay-sdk-core[registry,registry-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[registry,registry-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-registry-types` is installed
-from waylay.services.registry.models.root_page_response import RootPageResponse
+from ..models.function_type import FunctionType
+from ..models.job_state_result import JobStateResult
+from ..models.job_type_schema import JobTypeSchema
+from ..models.jobs_response import JobsResponse
 try:
-    # Get Service Status
-    # calls `GET /registry/v2/`
-    api_response = await waylay_client.registry.about.get(
+    # List Jobs
+    # calls `GET /registry/v2/jobs/`
+    api_response = await waylay_client.registry.jobs.list(
+        # query parameters:
+        query = {
+        },
     )
-    print("The response of registry.about.get:\n")
+    print("The response of registry.jobs.list:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling registry.about.get: %s\n" % e)
+    print("Exception when calling registry.jobs.list: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/README.md` & `waylay-sdk-registry-types-2.13.0rc0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 # Waylay Registry Service
 V2 API to build and deploy Waylay functions (plugs, webscripts, BYOML models).
 
 This Python package is automatically generated based on the 
-Waylay Registry OpenAPI specification (API version: 2.13.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/registry.html).
+Waylay Registry OpenAPI specification (API version: 2.13.0-beta.0)
 
 It is considered an extension of the waylay-sdk-registry package, and it consists of the typed model classes for all path params, query params, body params and responses for each of the api methods in `waylay-sdk-registry`.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-registry is included in:
-- ```pip install waylay-sdk-core[registry]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[registry]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-registry and waylay-sdk-registry-types are included in:
-- ```pip install waylay-sdk-core[registry,registry-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[registry,registry-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-registry-types` is installed
-from waylay.services.registry.models.root_page_response import RootPageResponse
+from ..models.function_type import FunctionType
+from ..models.job_state_result import JobStateResult
+from ..models.job_type_schema import JobTypeSchema
+from ..models.jobs_response import JobsResponse
 try:
-    # Get Service Status
-    # calls `GET /registry/v2/`
-    api_response = await waylay_client.registry.about.get(
+    # List Jobs
+    # calls `GET /registry/v2/jobs/`
+    api_response = await waylay_client.registry.jobs.list(
+        # query parameters:
+        query = {
+        },
     )
-    print("The response of registry.about.get:\n")
+    print("The response of registry.jobs.list:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling registry.about.get: %s\n" % e)
+    print("Exception when calling registry.jobs.list: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/pyproject.toml` & `waylay-sdk-registry-types-2.13.0rc0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-registry-types"
-version = "2.13.0b20240415"
+version = "2.13.0rc0"
 description = "Waylay Function Registry Types "
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay Function Registry" , "Types"]
 requires-python = ">= 3.9"
 dependencies = [
-    "waylay-sdk-core ~= 0.2.0",
-    "waylay-sdk-registry == 2.13.0b20240415",
+    "waylay-sdk ~= 0.0.4rc5",
+    "waylay-sdk-registry == 2.13.0rc0",
     "pydantic ~= 2.6",
     "typing-extensions ~= 4.10",
     "eval-type-backport ~= 0.1.3; python_version < '3.10'",
 ]
 readme = "README.md"
 license={file = "LICENSE.txt"}
 
 [project.urls]
 Homepage = "https://www.waylay.io/"
-Documentation = "https://docs.waylay.io/#/api/?id=software-development-kits"
+Documentation = "https://docs.waylay.io/#/"
 Repository = "https://github.com/waylayio/waylay-sdk-registry-py.git"
-"Openapi Specification" = "https://docs.waylay.io/openapi/public/redocly/registry.html"
 
 [project.optional-dependencies]
 dev = [
     "mypy",
     "ruff",
     "types-python-jose",
     "types-appdirs",
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/__init__.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # coding: utf-8
 """Waylay Function Registry: REST Models.
 
 This code was generated from the OpenAPI documentation of 'Waylay Function Registry'
 
-version: 2.13.0
+version: 2.13.0-beta.0
 
 V2 API to build and deploy Waylay functions (plugs, webscripts, BYOML models).
 
 Generated by OpenAPI Generator (https://openapi-generator.tech)
 
 Do not edit the class manually.
 """
 
-__version__ = "2.13.0b20240415"
+__version__ = "2.13.0rc0"
 
 # import models into model package
 from .active_event_data import ActiveEventData
 from .active_event_sse import ActiveEventSSE
 from .active_event_sse_event import ActiveEventSSEEvent
 from .alt_embedded_version_i_kfserving_response_v2 import (
     AltEmbeddedVersionIKfservingResponseV2,
@@ -331,15 +331,14 @@
 from .rebuild_query_v2 import RebuildQueryV2
 from .rebuild_submitted_response import RebuildSubmittedResponse
 from .rebuild_webscript_async_response_v2 import RebuildWebscriptAsyncResponseV2
 from .rebuild_webscript_sync_response_v2 import RebuildWebscriptSyncResponseV2
 from .registry_error_response import RegistryErrorResponse
 from .remove_function_query_v2 import RemoveFunctionQueryV2
 from .remove_plug_query_v2 import RemovePlugQueryV2
-from .request_deploy_query import RequestDeployQuery
 from .request_operation import RequestOperation
 from .resource_limits import ResourceLimits
 from .root_page_response import RootPageResponse
 from .runtime_attributes import RuntimeAttributes
 from .runtime_info import RuntimeInfo
 from .runtime_name_query import RuntimeNameQuery
 from .runtime_params import RuntimeParams
@@ -364,15 +363,14 @@
 from .scale_type import ScaleType
 from .schema_by_id_params import SchemaByIdParams
 from .schema_params import SchemaParams
 from .semantic_version_range import SemanticVersionRange
 from .show_related_type import ShowRelatedType
 from .status import Status
 from .status_any import StatusAny
-from .status_exclude import StatusExclude
 from .status_filter import StatusFilter
 from .status_include import StatusInclude
 from .status_response import StatusResponse
 from .stream_closing import StreamClosing
 from .stream_ready import StreamReady
 from .supported_events import SupportedEvents
 from .tag import Tag
@@ -726,15 +724,14 @@
     "RebuildQueryV2",
     "RebuildSubmittedResponse",
     "RebuildWebscriptAsyncResponseV2",
     "RebuildWebscriptSyncResponseV2",
     "RegistryErrorResponse",
     "RemoveFunctionQueryV2",
     "RemovePlugQueryV2",
-    "RequestDeployQuery",
     "RequestOperation",
     "ResourceLimits",
     "RootPageResponse",
     "RuntimeAttributes",
     "RuntimeInfo",
     "RuntimeNameQuery",
     "RuntimeParams",
@@ -759,15 +756,14 @@
     "ScaleType",
     "SchemaByIdParams",
     "SchemaParams",
     "SemanticVersionRange",
     "ShowRelatedType",
     "Status",
     "StatusAny",
-    "StatusExclude",
     "StatusFilter",
     "StatusInclude",
     "StatusResponse",
     "StreamClosing",
     "StreamReady",
     "SupportedEvents",
     "Tag",
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/active_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/active_event_data.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/active_event_sse.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/active_event_sse.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/alt_embedded_version_i_kfserving_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/alt_embedded_version_i_kfserving_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/alt_embedded_version_i_plug_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/alt_embedded_version_i_plug_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/alt_embedded_version_i_webscript_response_with_invoke_link_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/alt_embedded_version_i_webscript_response_with_invoke_link_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/alt_version_hal_link.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/alt_version_hal_link.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/any_function_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/any_function_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/any_job_for_function.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/any_job_for_function.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/any_job_result.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/any_job_result.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/any_job_status.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/any_job_status.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/any_job_status_summary.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/any_job_status_summary.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/archive_format.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/archive_format.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/asset_condition.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_condition.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/asset_condition_content_type.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_condition_content_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/asset_condition_pattern.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_condition_pattern.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/asset_path_params_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_path_params_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/asset_role.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_role.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/asset_summary.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_summary.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/asset_summary_with_hal_link.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_summary_with_hal_link.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/asset_summary_with_hal_link_links.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_summary_with_hal_link_links.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/assets_conditions.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/assets_conditions.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/async_deploy_query_v1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/async_deploy_query_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,29 +18,29 @@
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
 class AsyncDeployQueryV1(WaylayBaseModel):
     """AsyncDeployQueryV1."""
 
+    scale_to_zero: StrictBool | None = Field(
+        default=False,
+        description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. Saves computing resources when the function is not to be used immediately.",
+        alias="scaleToZero",
+    )
     var_async: StrictBool | None = Field(
         default=True,
         description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.",
         alias="async",
     )
     dry_run: StrictBool | None = Field(
         default=None,
         description="If set to <code>true</code>, validates the deployment conditions, but does not change anything.",
         alias="dryRun",
     )
-    scale_to_zero: StrictBool | None = Field(
-        default=False,
-        description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.",
-        alias="scaleToZero",
-    )
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
         extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/async_query_default_false.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/async_query_default_false.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/async_verify_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/async_verify_query.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -18,24 +18,24 @@
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
 class AsyncVerifyQuery(WaylayBaseModel):
     """AsyncVerifyQuery."""
 
-    scale_to_zero: StrictBool | None = Field(
-        default=None,
-        description="Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command.",
-        alias="scaleToZero",
-    )
     var_async: StrictBool | None = Field(
         default=True,
         description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.",
         alias="async",
     )
+    scale_to_zero: StrictBool | None = Field(
+        default=None,
+        description="Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command.",
+        alias="scaleToZero",
+    )
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
         extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/batch.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/batch.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/batch_args.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/batch_args.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/batch_job_status.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/batch_job_status.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/batch_result.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/batch_result.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/build.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/build1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build1.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/build_args.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build_args.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,16 +30,17 @@
     """Input arguments to a job that builds a function.."""
 
     runtime_name: StrictStr = Field(alias="runtimeName")
     runtime_version: Annotated[str, Field(strict=True)] = Field(
         description="A semantic version with _exactly_ a `major`, `minor` and `patch` specifier. No `pre-release` or `build` identifiers are allowed. See https://semver.org",
         alias="runtimeVersion",
     )
-    revision: StrictStr = Field(
-        description="The revision hash of the current (draft) function revision"
+    revision: StrictStr | None = Field(
+        default=None,
+        description="The revision hash of the current (draft) function revision",
     )
     storage_location: StrictStr = Field(
         description="Location of the function assets.", alias="storageLocation"
     )
     image_name: StrictStr = Field(
         description="Provided (or defaulted) image name to publish the function image.",
         alias="imageName",
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/build_job_status.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build_job_status.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/build_result.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build_result.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/build_spec.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build_spec.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/cleanup_result.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/cleanup_result.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/compiled_runtime_version.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/compiled_runtime_version.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/completed_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/completed_event_data.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/completed_event_sse.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/completed_event_sse.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/content_query_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/content_query_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/content_validation_listing.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/content_validation_listing.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/create_function_query_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/create_function_query_v2.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,44 +29,40 @@
 from ..models.deprecate_previous_policy import DeprecatePreviousPolicy
 from ..models.semantic_version_range import SemanticVersionRange
 
 
 class CreateFunctionQueryV2(WaylayBaseModel):
     """CreateFunctionQueryV2."""
 
-    deploy: StrictBool | None = Field(
-        default=True,
-        description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.",
-    )
     author: StrictStr | None = Field(
         default=None,
         description="Optionally changes the author metadata when updating a function.",
     )
     comment: StrictStr | None = Field(
         default=None,
         description="An optional user-specified comment corresponding to the operation.",
     )
-    scale_to_zero: StrictBool | None = Field(
-        default=False,
-        description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.",
-        alias="scaleToZero",
-    )
     deprecate_previous: DeprecatePreviousPolicy | None = Field(
         default=None, alias="deprecatePrevious"
     )
     dry_run: StrictBool | None = Field(
         default=None,
         description="If set to <code>true</code>, validates the deployment conditions, but does not change anything.",
         alias="dryRun",
     )
     var_async: StrictBool | None = Field(
         default=True,
         description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.",
         alias="async",
     )
+    scale_to_zero: StrictBool | None = Field(
+        default=False,
+        description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. Saves computing resources when the function is not to be used immediately.",
+        alias="scaleToZero",
+    )
     version: SemanticVersionRange | None = None
     name: StrictStr | None = Field(
         default=None,
         description="If set, the value will be used as the function name instead of the one specified in the manifest.",
     )
     draft: StrictBool | None = Field(
         default=False,
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/create_function_query_v2_copy.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/create_function_query_v2_copy.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/create_kf_serving_async_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/create_kf_serving_async_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/create_plug_async_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/create_plug_async_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/create_webscript_async_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/create_webscript_async_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/create_webscripts_copy_parameter.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/create_webscripts_copy_parameter.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/delayed_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/delayed_event_data.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/delayed_event_sse.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/delayed_event_sse.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/deploy.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/deploy1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy1.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/deploy_args.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_args.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,38 +20,30 @@
     field_validator,
 )
 from typing_extensions import (
     Annotated,  # >=3.11
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.deploy_args_deploy_spec_overrides import DeployArgsDeploySpecOverrides
 
-
-class DeployArgs(WaylayBaseModel):
-    """Input argument to an (openfaas) deployment job for a function.."""
+class VerifyArgs(WaylayBaseModel):
+    """Input arguments for an (openfaas) deployment verification job.."""
 
     namespace: StrictStr = Field(
         description="The (openfaas) namespace for the target function."
     )
     endpoint: StrictStr = Field(description="The (openfaas) endpoint service name")
-    image_name: StrictStr = Field(
-        description="The image name to use for deploying this function",
-        alias="imageName",
-    )
     runtime_name: StrictStr = Field(alias="runtimeName")
     runtime_version: Annotated[str, Field(strict=True)] = Field(
         description="A semantic version with _exactly_ a `major`, `minor` and `patch` specifier. No `pre-release` or `build` identifiers are allowed. See https://semver.org",
         alias="runtimeVersion",
     )
-    revision: StrictStr = Field(
-        description="The revision hash of the current (draft) function revision"
-    )
-    deploy_spec_overrides: DeployArgsDeploySpecOverrides = Field(
-        alias="deploySpecOverrides"
+    revision: StrictStr | None = Field(
+        default=None,
+        description="The revision hash of the current (draft) function revision",
     )
 
     @field_validator("runtime_version")
     @classmethod
     def runtime_version_validate_regular_expression(cls, value):
         """Validate the regular expression."""
         if not re.match(r"^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$", value):
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/deploy_args_deploy_spec_overrides.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_args_deploy_spec_overrides.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/deploy_job_status.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_job_status.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/deploy_result.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_result.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/deploy_spec.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_spec.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/deploy_spec_openfaas_spec.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_spec_openfaas_spec.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/deprecate_previous_policy.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deprecate_previous_policy.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/documentation.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/documentation.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/documentation_property.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/documentation_property.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/entity_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/entity_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/entity_with_links_i_kfserving_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/entity_with_links_i_kfserving_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/entity_with_links_i_plug_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/entity_with_links_i_plug_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/entity_with_links_i_webscript_response_with_invoke_link_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/entity_with_links_i_webscript_response_with_invoke_link_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/error_and_status_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/error_and_status_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/error_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/error_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/event_sse.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/event_sse.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/event_type_sse.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/event_type_sse.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/event_with_close_sse.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/event_with_close_sse.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/example_reference.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/example_reference.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/exposed_openfaas_deploy_spec.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/exposed_openfaas_deploy_spec.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/failed_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/failed_event_data.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/failed_event_sse.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/failed_event_sse.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/failure_reason.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/failure_reason.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/file_upload.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/file_upload.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/force_delete_query_v1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/force_delete_query_v1.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/function_deploy_overrides.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_deploy_overrides.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/function_deploy_overrides_type.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_deploy_overrides_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/function_job_args.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_job_args.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,16 +29,17 @@
     """Job arguments shared by all function jobs."""
 
     runtime_name: StrictStr = Field(alias="runtimeName")
     runtime_version: Annotated[str, Field(strict=True)] = Field(
         description="A semantic version with _exactly_ a `major`, `minor` and `patch` specifier. No `pre-release` or `build` identifiers are allowed. See https://semver.org",
         alias="runtimeVersion",
     )
-    revision: StrictStr = Field(
-        description="The revision hash of the current (draft) function revision"
+    revision: StrictStr | None = Field(
+        default=None,
+        description="The revision hash of the current (draft) function revision",
     )
 
     @field_validator("runtime_version")
     @classmethod
     def runtime_version_validate_regular_expression(cls, value):
         """Validate the regular expression."""
         if not re.match(r"^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$", value):
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/function_manifest.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_manifest.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/function_meta.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_meta.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/function_name_version.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_name_version.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/function_ref.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_ref.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/function_spec.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_spec.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/function_type.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_content_params_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_content_params_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_invokable_webscript_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_invokable_webscript_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_model_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_model_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_plug_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_plug_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_plug_response_v2_links.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_plug_response_v2_links.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_plug_response_v2_links_draft.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_plug_response_v2_links_draft.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_plug_response_v2_links_published.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_plug_response_v2_links_published.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_runtime_by_name_and_version_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_runtime_by_name_and_version_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_runtime_by_name_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_runtime_by_name_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_runtime_example_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_runtime_example_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_runtime_versions_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_runtime_versions_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_webscript_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_webscript_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/get_webscript_response_v2_links.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_webscript_response_v2_links.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/hal_link.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/hal_link.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/invokable_webscript_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/invokable_webscript_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/invokable_webscript_response_entity.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/invokable_webscript_response_entity.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/invokable_webscript_response_entity_webscript.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/invokable_webscript_response_entity_webscript.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/invoke_hal_link.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/invoke_hal_link.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/invoke_internal_hal_link.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/invoke_internal_hal_link.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_and_function_hal_link.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_and_function_hal_link.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_cause.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_cause.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_causes.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_causes.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_payload_active_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_payload_active_event_data.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_payload_completed_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_payload_completed_event_data.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_payload_delayed_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_payload_delayed_event_data.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_payload_failed_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_payload_failed_event_data.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_payload_waiting_children_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_payload_waiting_children_event_data.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_payload_waiting_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_payload_waiting_event_data.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_response_active_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_response_active_event_data.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_response_completed_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_response_completed_event_data.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_response_delayed_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_response_delayed_event_data.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_response_failed_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_response_failed_event_data.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_response_waiting_children_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_response_waiting_children_event_data.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_response_waiting_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_response_waiting_event_data.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_event_sse.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_sse.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_events_and_function_hal_link.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_events_and_function_hal_link.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_events_filter_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_events_filter_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_events_hal_link.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_events_hal_link.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_hal_links.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_hal_links.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_reference.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_reference.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_reference_params.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_reference_params.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_state.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_state_finished.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_finished.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_state_result.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_result.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_state_waiting.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_waiting.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_state_waiting_children.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_waiting_children.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_status.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_status.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_status_and_entity_hal_links.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_status_and_entity_hal_links.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_status_hal_link.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_status_hal_link.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_submitted_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_submitted_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_type.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_version_level.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,21 +10,18 @@
 """
 
 from __future__ import annotations
 
 from enum import Enum
 
 
-class JobType(str, Enum):
-    """JobType."""
+class LatestVersionLevel(str, Enum):
+    """Level of latest versions that should be included.."""
 
-    BUILD = "build"
-    DEPLOY = "deploy"
-    VERIFY = "verify"
-    UNDEPLOY = "undeploy"
-    BATCH = "batch"
-    SCALE = "scale"
-    CLEANUP = "cleanup"
-    NOTIFY = "notify"
+    MAJOR = "major"
+    MINOR = "minor"
+    PATCH = "patch"
+    TRUE = "true"
+    FALSE = "false"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/job_type_schema.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_type_schema.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/jobs_for_model_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_model_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/jobs_for_model_response_v2_links.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_model_response_v2_links.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/jobs_for_plug_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_plug_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/jobs_for_plug_response_v2_links.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_plug_response_v2_links.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/jobs_for_webscript_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_webscript_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/jobs_for_webscript_response_v2_links.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_webscript_response_v2_links.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/jobs_hal_link.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_hal_link.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/jobs_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/keep_alive_event_sse.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/keep_alive_event_sse.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_delete_multiple_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_delete_multiple_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_delete_multiple_with_job_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_delete_multiple_with_job_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_delete_query_v1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_delete_query_v1.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_delete_query_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_delete_query_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_delete_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_delete_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_delete_with_job_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_delete_with_job_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_latest_version_query_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_latest_version_query_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_latest_versions_query_v1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_latest_versions_query_v1.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_latest_versions_query_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_latest_versions_query_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_manifest.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_manifest.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_models_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_models_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kf_serving_versions_query_v1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_versions_query_v1.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/kfserving_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kfserving_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/language_release.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/language_release.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/latest_function_versions_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_function_versions_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/latest_functions_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_functions_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/latest_models_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_models_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/latest_plug_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_plug_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/latest_plug_version_query_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_plug_version_query_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/latest_plug_versions_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_plug_versions_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/latest_plug_versions_query_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_plug_versions_query_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/latest_plugs_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_plugs_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/latest_plugs_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_plugs_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/latest_version_level.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/waiting_children_event_sse_event.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 """
 
 from __future__ import annotations
 
 from enum import Enum
 
 
-class LatestVersionLevel(str, Enum):
-    """Level of latest versions that should be included.."""
+class WaitingChildrenEventSSEEvent(str, Enum):
+    """The job queue event that trigged this message."""
 
-    MAJOR = "major"
-    MINOR = "minor"
-    PATCH = "patch"
-    TRUE = "true"
-    FALSE = "false"
+    WAITING_MINUS_CHILDREN = "waiting-children"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/latest_webscripts_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_webscripts_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_configuration_object.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_configuration_object.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_configuration_object_format.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_configuration_object_format.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_configuration_response_object.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_configuration_response_object.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_create_debug_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_create_debug_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_debug_plug_manifest.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_debug_plug_manifest.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_debug_plug_request.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_debug_plug_request.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_documentation.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_documentation.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_documentation_request.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_documentation_request.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_function_meta.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_function_meta.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_create_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_create_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_create_request.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_create_request.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_create_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_create_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_meta_request.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_meta_request.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_request.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_request.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_request_metadata.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_request_metadata.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_request_metadata_documentation.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_request_metadata_documentation.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_request_metadata_documentation_any_of.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_request_metadata_documentation_any_of.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_request_metadata_raw_data_inner.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_request_metadata_raw_data_inner.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_response_metadata.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_response_metadata.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_script_meta.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_script_meta.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_script_meta_raw_data_inner.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_script_meta_raw_data_inner.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_plug_script_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_script_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_required_properties_inner.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_required_properties_inner.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/legacy_required_property_object.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_required_property_object.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/media_type.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/media_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/message_and_status_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/message_and_status_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/message_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/message_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/model.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/model.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/model1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/model1.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/model2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/model2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/model_versions_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/model_versions_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/name.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/name.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/name_and_version.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/name_and_version.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/named_kf_serving_versions_query_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_kf_serving_versions_query_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/named_parameters_typeof_as_job_reference.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_parameters_typeof_as_job_reference.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/named_parameters_typeof_as_job_reference_job_status.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_parameters_typeof_as_job_reference_job_status.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/named_parameters_typeof_from_legacy.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_parameters_typeof_from_legacy.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/named_parameters_typeof_from_legacy_documentation.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_parameters_typeof_from_legacy_documentation.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/named_parameters_typeof_is_not_legacy.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_parameters_typeof_is_not_legacy.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/named_plug_versions_query_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_plug_versions_query_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/named_webscript_versions_query_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_webscript_versions_query_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/notify_result.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/notify_result.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/openfaas_deploy_args.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/openfaas_deploy_args.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/openfaas_function_ref.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/openfaas_function_ref.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/operation.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/operation.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/operation_status.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/operation_status.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/operation_status_error.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/operation_status_error.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/paging_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/paging_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/parent_keys.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/parent_keys.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/patch_interface_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/patch_interface_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/patch_metadata_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/patch_metadata_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/patch_plug_request_v1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/patch_plug_request_v1.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug1.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_delete_force_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_delete_force_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_interface.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_interface.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_listing_and_query_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_listing_and_query_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_listing_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_listing_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_manifest.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_manifest.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_meta.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_meta.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_property.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_property.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_property_data_type.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_property_data_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_property_format.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_property_format.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_property_format_type.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_property_format_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/plug_versions_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_versions_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/post_model_job_async_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/post_model_job_async_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/post_model_job_sync_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/post_model_job_sync_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/post_plug_job_async_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/post_plug_job_async_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/post_plug_job_sync_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/post_plug_job_sync_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/post_webscript_job_async_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/post_webscript_job_async_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/post_webscript_job_sync_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/post_webscript_job_sync_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/provided_dependency.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/provided_dependency.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/publish_function_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/publish_function_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/queue_events.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/queue_events.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/rebuild_computed_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_computed_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/rebuild_model_async_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_model_async_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/rebuild_model_sync_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_model_sync_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/rebuild_plug_async_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_plug_async_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/rebuild_plug_sync_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_plug_sync_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/rebuild_policy.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_policy.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/rebuild_query_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_query_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,14 @@
 
 from ..models.rebuild_policy import RebuildPolicy
 
 
 class RebuildQueryV2(WaylayBaseModel):
     """RebuildQueryV2."""
 
-    scale_to_zero: StrictBool | None = Field(
-        default=None,
-        description="Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command.",
-        alias="scaleToZero",
-    )
     comment: StrictStr | None = Field(
         default=None,
         description="An optional user-specified comment corresponding to the operation.",
     )
     dry_run: StrictBool | None = Field(
         default=None,
         description="If set to <code>true</code>, checks whether rebuild jobs are needed, but do not start any jobs.",
@@ -57,14 +52,19 @@
         alias="forceVersion",
     )
     ignore_checks: StrictBool | None = Field(
         default=None,
         description="If set to true, checks that normally prevent a rebuild are overriden. These checks include: * function state in `pending`, `running`, `failed` or `undeployed` * backoff period due to recent failures * usage of deprecated dependencies * running jobs on entity * the `dryRun` option",
         alias="ignoreChecks",
     )
+    scale_to_zero: StrictBool | None = Field(
+        default=None,
+        description="Indicates whether the function needs to be scaled down after successful (re-)deployment. If not set, the function is scaled to zero only if it was not active before this command.",
+        alias="scaleToZero",
+    )
     skip_rebuild: StrictBool | None = Field(
         default=None,
         description="If set, the function will not be rebuild. Always uses the current runtime version when re-deploying/re-verifying the function.",
         alias="skipRebuild",
     )
 
     @field_validator("force_version")
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/rebuild_submitted_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_submitted_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/rebuild_webscript_async_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_webscript_async_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/rebuild_webscript_sync_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_webscript_sync_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/registry_error_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/registry_error_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/remove_function_query_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/remove_function_query_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/remove_plug_query_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/remove_plug_query_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/request_deploy_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_summary_attrs.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,26 +10,30 @@
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
     Field,
-    StrictBool,
+    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
+from ..models.archive_format import ArchiveFormat
+from ..models.function_type import FunctionType
 
-class RequestDeployQuery(WaylayBaseModel):
-    """RequestDeployQuery."""
 
-    deploy: StrictBool | None = Field(
-        default=True,
-        description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.",
-    )
+class RuntimeSummaryAttrs(WaylayBaseModel):
+    """RuntimeSummaryAttrs."""
+
+    name: StrictStr
+    title: StrictStr
+    description: StrictStr | None = None
+    function_type: FunctionType = Field(alias="functionType")
+    archive_format: ArchiveFormat = Field(alias="archiveFormat")
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
         extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/request_operation.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/request_operation.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/resource_limits.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/resource_limits.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/root_page_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/root_page_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_attributes.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_attributes.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_info.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_info.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_name_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_name_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_params.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_params.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_reference.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_reference.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_specification.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_specification.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_summary.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_summary.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_summary_attrs.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/unhealthy_invokable_webscript_error.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,26 +14,27 @@
 from pydantic import (
     ConfigDict,
     Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.archive_format import ArchiveFormat
-from ..models.function_type import FunctionType
+from ..models.invokable_webscript_response_entity import (
+    InvokableWebscriptResponseEntity,
+)
+from ..models.invoke_internal_hal_link import InvokeInternalHALLink
 
 
-class RuntimeSummaryAttrs(WaylayBaseModel):
-    """RuntimeSummaryAttrs."""
+class UnhealthyInvokableWebscriptError(WaylayBaseModel):
+    """Webscript Not Healthy."""
 
-    name: StrictStr
-    title: StrictStr
-    description: StrictStr | None = None
-    function_type: FunctionType = Field(alias="functionType")
-    archive_format: ArchiveFormat = Field(alias="archiveFormat")
+    entity: InvokableWebscriptResponseEntity
+    links: InvokeInternalHALLink = Field(alias="_links")
+    error: StrictStr
+    code: StrictStr
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
         extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_summary_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_summary_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_version_and_path_params.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_and_path_params.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_version_info.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_info.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_version_params.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_params.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_version_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_version_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_version_specification.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_specification.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_version_status.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_status.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/runtime_version_summary.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_summary.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/scale.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/scale.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/scale1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/scale1.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/scale_args.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy_args.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,41 +12,45 @@
 from __future__ import annotations
 
 import re
 
 from pydantic import (
     ConfigDict,
     Field,
-    StrictFloat,
-    StrictInt,
+    StrictBool,
     StrictStr,
     field_validator,
 )
 from typing_extensions import (
     Annotated,  # >=3.11
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-class ScaleArgs(WaylayBaseModel):
-    """Input argument to an (openfaas) scale job for a function.."""
+class UndeployArgs(WaylayBaseModel):
+    """Input argument to an (openfaas) undeployment job for a function.."""
 
     namespace: StrictStr = Field(
         description="The (openfaas) namespace for the target function."
     )
     endpoint: StrictStr = Field(description="The (openfaas) endpoint service name")
     runtime_name: StrictStr = Field(alias="runtimeName")
     runtime_version: Annotated[str, Field(strict=True)] = Field(
         description="A semantic version with _exactly_ a `major`, `minor` and `patch` specifier. No `pre-release` or `build` identifiers are allowed. See https://semver.org",
         alias="runtimeVersion",
     )
-    revision: StrictStr = Field(
-        description="The revision hash of the current (draft) function revision"
+    revision: StrictStr | None = Field(
+        default=None,
+        description="The revision hash of the current (draft) function revision",
     )
-    replicas: StrictFloat | StrictInt = Field(description="Number of target replicas")
+    is_native_plug: StrictBool = Field(
+        description="If true, the function is not expected to be deployed on openfaas.",
+        alias="isNativePlug",
+    )
+    delete_entity: StrictBool = Field(alias="deleteEntity")
 
     @field_validator("runtime_version")
     @classmethod
     def runtime_version_validate_regular_expression(cls, value):
         """Validate the regular expression."""
         if not re.match(r"^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$", value):
             raise ValueError(
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/scale_job_status.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/scale_job_status.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/schema_by_id_params.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/schema_by_id_params.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/schema_params.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/schema_params.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/semantic_version_range.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/semantic_version_range.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/status.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/status.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/status_filter.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/status_filter.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 )
 
 from typing_extensions import (
     Annotated,  # >=3.9
 )
 
 from ..models.status_any import StatusAny
-from ..models.status_exclude import StatusExclude
 from ..models.status_include import StatusInclude
 
 StatusFilter = Union[
-    Annotated[StatusInclude, ""], Annotated[StatusExclude, ""], Annotated[StatusAny, ""]
+    Annotated[StatusInclude, ""],
+    Annotated[
+        str,
+        "Any status value with a `-` postfix appended, excludes that status as a filter.",
+    ],
+    Annotated[StatusAny, ""],
 ]
 """Inclusion or exclusion filter on the `status` property.."""
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/status_include.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/status_include.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/status_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/status_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/stream_closing.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/stream_closing.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/stream_ready.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/stream_ready.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/supported_events.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/supported_events.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/tag.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/tag.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/tag_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/tag_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/timestamp_absolute.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/timestamp_absolute.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/timestamp_age.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/timestamp_age.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/timestamp_spec.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/timestamp_spec.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/undeploy.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/undeploy1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy1.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/undeploy_args.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/scale_args.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,44 +12,42 @@
 from __future__ import annotations
 
 import re
 
 from pydantic import (
     ConfigDict,
     Field,
-    StrictBool,
+    StrictFloat,
+    StrictInt,
     StrictStr,
     field_validator,
 )
 from typing_extensions import (
     Annotated,  # >=3.11
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-class UndeployArgs(WaylayBaseModel):
-    """Input argument to an (openfaas) undeployment job for a function.."""
+class ScaleArgs(WaylayBaseModel):
+    """Input argument to an (openfaas) scale job for a function.."""
 
     namespace: StrictStr = Field(
         description="The (openfaas) namespace for the target function."
     )
     endpoint: StrictStr = Field(description="The (openfaas) endpoint service name")
     runtime_name: StrictStr = Field(alias="runtimeName")
     runtime_version: Annotated[str, Field(strict=True)] = Field(
         description="A semantic version with _exactly_ a `major`, `minor` and `patch` specifier. No `pre-release` or `build` identifiers are allowed. See https://semver.org",
         alias="runtimeVersion",
     )
-    revision: StrictStr = Field(
-        description="The revision hash of the current (draft) function revision"
+    revision: StrictStr | None = Field(
+        default=None,
+        description="The revision hash of the current (draft) function revision",
     )
-    is_native_plug: StrictBool = Field(
-        description="If true, the function is not expected to be deployed on openfaas.",
-        alias="isNativePlug",
-    )
-    delete_entity: StrictBool = Field(alias="deleteEntity")
+    replicas: StrictFloat | StrictInt = Field(description="Number of target replicas")
 
     @field_validator("runtime_version")
     @classmethod
     def runtime_version_validate_regular_expression(cls, value):
         """Validate the regular expression."""
         if not re.match(r"^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$", value):
             raise ValueError(
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/undeploy_job_status.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy_job_status.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/undeploy_result.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy_result.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/undeploy_submitted_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy_submitted_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/undeployed_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeployed_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/unhealthy_invokable_webscript_error.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/with_asset_hal_link.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,31 +10,24 @@
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
     Field,
-    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.invokable_webscript_response_entity import (
-    InvokableWebscriptResponseEntity,
-)
-from ..models.invoke_internal_hal_link import InvokeInternalHALLink
+from ..models.asset_summary_with_hal_link_links import AssetSummaryWithHALLinkLinks
 
 
-class UnhealthyInvokableWebscriptError(WaylayBaseModel):
-    """Webscript Not Healthy."""
+class WithAssetHALLink(WaylayBaseModel):
+    """WithAssetHALLink."""
 
-    entity: InvokableWebscriptResponseEntity
-    links: InvokeInternalHALLink = Field(alias="_links")
-    error: StrictStr
-    code: StrictStr
+    links: AssetSummaryWithHALLinkLinks = Field(alias="_links")
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
         extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/update_draft_query.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/update_draft_query.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,23 +19,14 @@
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
 class UpdateDraftQuery(WaylayBaseModel):
     """UpdateDraftQuery."""
 
-    scale_to_zero: StrictBool | None = Field(
-        default=False,
-        description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.",
-        alias="scaleToZero",
-    )
-    deploy: StrictBool | None = Field(
-        default=True,
-        description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.",
-    )
     chown: StrictBool | None = Field(
         default=False,
         description="If set, ownership of the draft function is transferred to the current user.",
     )
     comment: StrictStr | None = Field(
         default=None,
         description="An optional user-specified comment corresponding to the operation.",
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/update_metadata_request_v1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/update_metadata_request_v1.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/update_metadata_request_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/update_metadata_request_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/update_record.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/update_record.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/user_plug_meta.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/user_plug_meta.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/verify.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/verify1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify1.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/verify_args.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_args.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,29 +20,39 @@
     field_validator,
 )
 from typing_extensions import (
     Annotated,  # >=3.11
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
+from ..models.deploy_args_deploy_spec_overrides import DeployArgsDeploySpecOverrides
 
-class VerifyArgs(WaylayBaseModel):
-    """Input arguments for an (openfaas) deployment verification job.."""
+
+class DeployArgs(WaylayBaseModel):
+    """Input argument to an (openfaas) deployment job for a function.."""
 
     namespace: StrictStr = Field(
         description="The (openfaas) namespace for the target function."
     )
     endpoint: StrictStr = Field(description="The (openfaas) endpoint service name")
+    image_name: StrictStr = Field(
+        description="The image name to use for deploying this function",
+        alias="imageName",
+    )
     runtime_name: StrictStr = Field(alias="runtimeName")
     runtime_version: Annotated[str, Field(strict=True)] = Field(
         description="A semantic version with _exactly_ a `major`, `minor` and `patch` specifier. No `pre-release` or `build` identifiers are allowed. See https://semver.org",
         alias="runtimeVersion",
     )
-    revision: StrictStr = Field(
-        description="The revision hash of the current (draft) function revision"
+    revision: StrictStr | None = Field(
+        default=None,
+        description="The revision hash of the current (draft) function revision",
+    )
+    deploy_spec_overrides: DeployArgsDeploySpecOverrides = Field(
+        alias="deploySpecOverrides"
     )
 
     @field_validator("runtime_version")
     @classmethod
     def runtime_version_validate_regular_expression(cls, value):
         """Validate the regular expression."""
         if not re.match(r"^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$", value):
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/verify_job_status.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_job_status.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/verify_model_sync_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_model_sync_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/verify_plug_sync_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_plug_sync_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/verify_query_v1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_query_v1.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/verify_result.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_result.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/verify_webscript_sync_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_webscript_sync_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/version_includes.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/version_includes.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/versions_query_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/versions_query_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/versions_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/versions_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/waiting_children_event_sse.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/waiting_children_event_sse.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/waiting_children_event_sse_event.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript1.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,17 +7,28 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
-from enum import Enum
-
-
-class WaitingChildrenEventSSEEvent(str, Enum):
-    """The job queue event that trigged this message."""
-
-    WAITING_MINUS_CHILDREN = "waiting-children"
-
-    def __str__(self) -> str:
-        return str(self.value)
+from pydantic import (
+    ConfigDict,
+)
+from waylay.sdk.api._models import BaseModel as WaylayBaseModel
+
+from ..models.hal_link import HALLink
+
+
+class Webscript1(WaylayBaseModel):
+    """Webscript1."""
+
+    event: HALLink | None = None
+    job: HALLink | None = None
+    webscript: HALLink
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
+    )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/waiting_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/waiting_event_data.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/waiting_event_sse.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/waiting_event_sse.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/webscript.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/webscript1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript2.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,18 +15,17 @@
     ConfigDict,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.hal_link import HALLink
 
 
-class Webscript1(WaylayBaseModel):
-    """Webscript1."""
+class Webscript2(WaylayBaseModel):
+    """Webscript2."""
 
-    event: HALLink | None = None
     job: HALLink | None = None
     webscript: HALLink
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/webscript2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/with_limit.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
+    Field,
+    StrictFloat,
+    StrictInt,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.hal_link import HALLink
 
+class WithLimit(WaylayBaseModel):
+    """WithLimit."""
 
-class Webscript2(WaylayBaseModel):
-    """Webscript2."""
-
-    job: HALLink | None = None
-    webscript: HALLink
+    limit: StrictFloat | StrictInt | None = Field(
+        default=None, description="The page size used for this query result."
+    )
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
         extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/webscript_latest_version_query_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_latest_version_query_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/webscript_latest_versions_query_v1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_latest_versions_query_v1.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/webscript_latest_versions_query_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_latest_versions_query_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/webscript_manifest.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_manifest.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/webscript_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/webscript_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/webscript_response_with_invoke_link_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_response_with_invoke_link_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/webscript_versions_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_versions_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/with_asset_hal_link.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/default_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 # coding: utf-8
-"""Waylay Function Registry models.
+"""Waylay Function Registry query parameters.
 
 This code was generated from the OpenAPI documentation of 'Waylay Function Registry'
 
 Generated by OpenAPI Generator (https://openapi-generator.tech)
 
 Do not edit the class manually.
-
 """
 
-from __future__ import annotations
+from __future__ import annotations  # for Python 3.7–3.9
 
 from pydantic import (
     ConfigDict,
-    Field,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.asset_summary_with_hal_link_links import AssetSummaryWithHALLinkLinks
 
+def _get_query_alias_for(field_name: str) -> str:
+    return field_name
 
-class WithAssetHALLink(WaylayBaseModel):
-    """WithAssetHALLink."""
 
-    links: AssetSummaryWithHALLinkLinks = Field(alias="_links")
+class GetQuery(WaylayBaseModel):
+    """Model for `get` query parameters."""
 
     model_config = ConfigDict(
-        populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
-        extra="ignore",
+        extra="allow",
+        alias_generator=_get_query_alias_for,
+        populate_by_name=True,
     )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/with_embedded_alt_versions_i_kfserving_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/with_embedded_alt_versions_i_kfserving_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/with_embedded_alt_versions_i_plug_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/with_embedded_alt_versions_i_plug_response_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/with_embedded_alt_versions_i_webscript_response_with_invoke_link_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/with_embedded_alt_versions_i_webscript_response_with_invoke_link_v2.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/with_entity_attributes.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/with_entity_attributes.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/models/with_paging.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/with_paging.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/queries/about_api.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/schemas_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,30 @@
 
 from pydantic import (
     ConfigDict,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
+def _get_by_role_query_alias_for(field_name: str) -> str:
+    return field_name
+
+
+class GetByRoleQuery(WaylayBaseModel):
+    """Model for `get_by_role` query parameters."""
+
+    model_config = ConfigDict(
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
+        alias_generator=_get_by_role_query_alias_for,
+        populate_by_name=True,
+    )
+
+
 def _get_query_alias_for(field_name: str) -> str:
     return field_name
 
 
 class GetQuery(WaylayBaseModel):
     """Model for `get` query parameters."""
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/queries/jobs_api.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/jobs_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/queries/models_api.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/models_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,28 +30,26 @@
 from ..models.job_type_schema import JobTypeSchema
 from ..models.rebuild_policy import RebuildPolicy
 from ..models.show_related_type import ShowRelatedType
 from ..models.status_filter import StatusFilter
 
 
 def _create_query_alias_for(field_name: str) -> str:
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "author":
         return "author"
     if field_name == "comment":
         return "comment"
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
     if field_name == "deprecate_previous":
         return "deprecatePrevious"
     if field_name == "dry_run":
         return "dryRun"
     if field_name == "var_async":
         return "async"
+    if field_name == "scale_to_zero":
+        return "scaleToZero"
     if field_name == "version":
         return "version"
     if field_name == "name":
         return "name"
     if field_name == "draft":
         return "draft"
     if field_name == "runtime":
@@ -60,38 +58,26 @@
         return "copy"
     return field_name
 
 
 class CreateQuery(WaylayBaseModel):
     """Model for `create` query parameters."""
 
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     author: Annotated[
         StrictStr | None,
         Field(
             description="Optionally changes the author metadata when updating a function."
         ),
     ] = None
     comment: Annotated[
         StrictStr | None,
         Field(
             description="An optional user-specified comment corresponding to the operation."
         ),
     ] = None
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
     deprecate_previous: Annotated[
         DeprecatePreviousPolicy | None,
         Field(
             description="Set the cleanup policy used to automatically deprecate/delete previous versions."
         ),
     ] = None
     dry_run: Annotated[
@@ -102,14 +88,20 @@
     ] = None
     var_async: Annotated[
         StrictBool | None,
         Field(
             description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
+    scale_to_zero: Annotated[
+        StrictBool | None,
+        Field(
+            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. Saves computing resources when the function is not to be used immediately."
+        ),
+    ] = None
     version: Annotated[
         Any | None,
         Field(
             description="If set, the function version will be an increment of the latest existing version that satisfies the `version` range. Note that this increment always takes precedence over an explicit `version` in the function manifest."
         ),
     ] = None
     name: Annotated[
@@ -143,44 +135,28 @@
         extra="allow",
         alias_generator=_create_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _delete_asset_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "chown":
         return "chown"
     if field_name == "comment":
         return "comment"
     if field_name == "author":
         return "author"
     if field_name == "var_async":
         return "async"
     return field_name
 
 
 class DeleteAssetQuery(WaylayBaseModel):
     """Model for `delete_asset` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     chown: Annotated[
         StrictBool | None,
         Field(
             description="If set, ownership of the draft function is transferred to the current user."
         ),
     ] = None
     comment: Annotated[
@@ -755,42 +731,36 @@
         extra="allow",
         alias_generator=_publish_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _rebuild_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
     if field_name == "comment":
         return "comment"
     if field_name == "dry_run":
         return "dryRun"
     if field_name == "var_async":
         return "async"
     if field_name == "upgrade":
         return "upgrade"
     if field_name == "force_version":
         return "forceVersion"
     if field_name == "ignore_checks":
         return "ignoreChecks"
+    if field_name == "scale_to_zero":
+        return "scaleToZero"
     if field_name == "skip_rebuild":
         return "skipRebuild"
     return field_name
 
 
 class RebuildQuery(WaylayBaseModel):
     """Model for `rebuild` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command."
-        ),
-    ] = None
     comment: Annotated[
         StrictStr | None,
         Field(
             description="An optional user-specified comment corresponding to the operation."
         ),
     ] = None
     dry_run: Annotated[
@@ -819,14 +789,20 @@
     ] = None
     ignore_checks: Annotated[
         StrictBool | None,
         Field(
             description="If set to true, checks that normally prevent a rebuild are overriden. These checks include: * function state in `pending`, `running`, `failed` or `undeployed` * backoff period due to recent failures * usage of deprecated dependencies * running jobs on entity * the `dryRun` option"
         ),
     ] = None
+    scale_to_zero: Annotated[
+        StrictBool | None,
+        Field(
+            description="Indicates whether the function needs to be scaled down after successful (re-)deployment. If not set, the function is scaled to zero only if it was not active before this command."
+        ),
+    ] = None
     skip_rebuild: Annotated[
         StrictBool | None,
         Field(
             description="If set, the function will not be rebuild. Always uses the current runtime version when re-deploying/re-verifying the function."
         ),
     ] = None
 
@@ -934,44 +910,28 @@
         extra="allow",
         alias_generator=_remove_versions_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _update_asset_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "chown":
         return "chown"
     if field_name == "comment":
         return "comment"
     if field_name == "author":
         return "author"
     if field_name == "var_async":
         return "async"
     return field_name
 
 
 class UpdateAssetQuery(WaylayBaseModel):
     """Model for `update_asset` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     chown: Annotated[
         StrictBool | None,
         Field(
             description="If set, ownership of the draft function is transferred to the current user."
         ),
     ] = None
     comment: Annotated[
@@ -999,44 +959,28 @@
         extra="allow",
         alias_generator=_update_asset_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _update_assets_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "chown":
         return "chown"
     if field_name == "comment":
         return "comment"
     if field_name == "author":
         return "author"
     if field_name == "var_async":
         return "async"
     return field_name
 
 
 class UpdateAssetsQuery(WaylayBaseModel):
     """Model for `update_assets` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     chown: Annotated[
         StrictBool | None,
         Field(
             description="If set, ownership of the draft function is transferred to the current user."
         ),
     ] = None
     comment: Annotated[
@@ -1064,34 +1008,34 @@
         extra="allow",
         alias_generator=_update_assets_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _verify_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
     if field_name == "var_async":
         return "async"
+    if field_name == "scale_to_zero":
+        return "scaleToZero"
     return field_name
 
 
 class VerifyQuery(WaylayBaseModel):
     """Model for `verify` query parameters."""
 
-    scale_to_zero: Annotated[
+    var_async: Annotated[
         StrictBool | None,
         Field(
-            description="Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command."
+            description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
-    var_async: Annotated[
+    scale_to_zero: Annotated[
         StrictBool | None,
         Field(
-            description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
+            description="Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command."
         ),
     ] = None
 
     model_config = ConfigDict(
         validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/queries/plugs_api.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/plugs_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,28 +31,26 @@
 from ..models.plug_type import PlugType
 from ..models.rebuild_policy import RebuildPolicy
 from ..models.show_related_type import ShowRelatedType
 from ..models.status_filter import StatusFilter
 
 
 def _create_query_alias_for(field_name: str) -> str:
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "author":
         return "author"
     if field_name == "comment":
         return "comment"
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
     if field_name == "deprecate_previous":
         return "deprecatePrevious"
     if field_name == "dry_run":
         return "dryRun"
     if field_name == "var_async":
         return "async"
+    if field_name == "scale_to_zero":
+        return "scaleToZero"
     if field_name == "version":
         return "version"
     if field_name == "name":
         return "name"
     if field_name == "draft":
         return "draft"
     if field_name == "runtime":
@@ -61,38 +59,26 @@
         return "copy"
     return field_name
 
 
 class CreateQuery(WaylayBaseModel):
     """Model for `create` query parameters."""
 
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     author: Annotated[
         StrictStr | None,
         Field(
             description="Optionally changes the author metadata when updating a function."
         ),
     ] = None
     comment: Annotated[
         StrictStr | None,
         Field(
             description="An optional user-specified comment corresponding to the operation."
         ),
     ] = None
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
     deprecate_previous: Annotated[
         DeprecatePreviousPolicy | None,
         Field(
             description="Set the cleanup policy used to automatically deprecate/delete previous versions."
         ),
     ] = None
     dry_run: Annotated[
@@ -103,14 +89,20 @@
     ] = None
     var_async: Annotated[
         StrictBool | None,
         Field(
             description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
+    scale_to_zero: Annotated[
+        StrictBool | None,
+        Field(
+            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. Saves computing resources when the function is not to be used immediately."
+        ),
+    ] = None
     version: Annotated[
         Any | None,
         Field(
             description="If set, the function version will be an increment of the latest existing version that satisfies the `version` range. Note that this increment always takes precedence over an explicit `version` in the function manifest."
         ),
     ] = None
     name: Annotated[
@@ -144,44 +136,28 @@
         extra="allow",
         alias_generator=_create_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _delete_asset_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "chown":
         return "chown"
     if field_name == "comment":
         return "comment"
     if field_name == "author":
         return "author"
     if field_name == "var_async":
         return "async"
     return field_name
 
 
 class DeleteAssetQuery(WaylayBaseModel):
     """Model for `delete_asset` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     chown: Annotated[
         StrictBool | None,
         Field(
             description="If set, ownership of the draft function is transferred to the current user."
         ),
     ] = None
     comment: Annotated[
@@ -807,42 +783,36 @@
         extra="allow",
         alias_generator=_publish_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _rebuild_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
     if field_name == "comment":
         return "comment"
     if field_name == "dry_run":
         return "dryRun"
     if field_name == "var_async":
         return "async"
     if field_name == "upgrade":
         return "upgrade"
     if field_name == "force_version":
         return "forceVersion"
     if field_name == "ignore_checks":
         return "ignoreChecks"
+    if field_name == "scale_to_zero":
+        return "scaleToZero"
     if field_name == "skip_rebuild":
         return "skipRebuild"
     return field_name
 
 
 class RebuildQuery(WaylayBaseModel):
     """Model for `rebuild` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command."
-        ),
-    ] = None
     comment: Annotated[
         StrictStr | None,
         Field(
             description="An optional user-specified comment corresponding to the operation."
         ),
     ] = None
     dry_run: Annotated[
@@ -871,14 +841,20 @@
     ] = None
     ignore_checks: Annotated[
         StrictBool | None,
         Field(
             description="If set to true, checks that normally prevent a rebuild are overriden. These checks include: * function state in `pending`, `running`, `failed` or `undeployed` * backoff period due to recent failures * usage of deprecated dependencies * running jobs on entity * the `dryRun` option"
         ),
     ] = None
+    scale_to_zero: Annotated[
+        StrictBool | None,
+        Field(
+            description="Indicates whether the function needs to be scaled down after successful (re-)deployment. If not set, the function is scaled to zero only if it was not active before this command."
+        ),
+    ] = None
     skip_rebuild: Annotated[
         StrictBool | None,
         Field(
             description="If set, the function will not be rebuild. Always uses the current runtime version when re-deploying/re-verifying the function."
         ),
     ] = None
 
@@ -986,44 +962,28 @@
         extra="allow",
         alias_generator=_remove_versions_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _update_asset_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "chown":
         return "chown"
     if field_name == "comment":
         return "comment"
     if field_name == "author":
         return "author"
     if field_name == "var_async":
         return "async"
     return field_name
 
 
 class UpdateAssetQuery(WaylayBaseModel):
     """Model for `update_asset` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     chown: Annotated[
         StrictBool | None,
         Field(
             description="If set, ownership of the draft function is transferred to the current user."
         ),
     ] = None
     comment: Annotated[
@@ -1051,44 +1011,28 @@
         extra="allow",
         alias_generator=_update_asset_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _update_assets_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "chown":
         return "chown"
     if field_name == "comment":
         return "comment"
     if field_name == "author":
         return "author"
     if field_name == "var_async":
         return "async"
     return field_name
 
 
 class UpdateAssetsQuery(WaylayBaseModel):
     """Model for `update_assets` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     chown: Annotated[
         StrictBool | None,
         Field(
             description="If set, ownership of the draft function is transferred to the current user."
         ),
     ] = None
     comment: Annotated[
@@ -1116,34 +1060,34 @@
         extra="allow",
         alias_generator=_update_assets_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _verify_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
     if field_name == "var_async":
         return "async"
+    if field_name == "scale_to_zero":
+        return "scaleToZero"
     return field_name
 
 
 class VerifyQuery(WaylayBaseModel):
     """Model for `verify` query parameters."""
 
-    scale_to_zero: Annotated[
+    var_async: Annotated[
         StrictBool | None,
         Field(
-            description="Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command."
+            description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
-    var_async: Annotated[
+    scale_to_zero: Annotated[
         StrictBool | None,
         Field(
-            description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
+            description="Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command."
         ),
     ] = None
 
     model_config = ConfigDict(
         validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/queries/runtimes_api.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/runtimes_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay/services/registry/queries/webscripts_api.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/webscripts_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,28 +30,26 @@
 from ..models.job_type_schema import JobTypeSchema
 from ..models.rebuild_policy import RebuildPolicy
 from ..models.show_related_type import ShowRelatedType
 from ..models.status_filter import StatusFilter
 
 
 def _create_query_alias_for(field_name: str) -> str:
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "author":
         return "author"
     if field_name == "comment":
         return "comment"
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
     if field_name == "deprecate_previous":
         return "deprecatePrevious"
     if field_name == "dry_run":
         return "dryRun"
     if field_name == "var_async":
         return "async"
+    if field_name == "scale_to_zero":
+        return "scaleToZero"
     if field_name == "version":
         return "version"
     if field_name == "name":
         return "name"
     if field_name == "draft":
         return "draft"
     if field_name == "runtime":
@@ -60,38 +58,26 @@
         return "copy"
     return field_name
 
 
 class CreateQuery(WaylayBaseModel):
     """Model for `create` query parameters."""
 
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     author: Annotated[
         StrictStr | None,
         Field(
             description="Optionally changes the author metadata when updating a function."
         ),
     ] = None
     comment: Annotated[
         StrictStr | None,
         Field(
             description="An optional user-specified comment corresponding to the operation."
         ),
     ] = None
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
     deprecate_previous: Annotated[
         DeprecatePreviousPolicy | None,
         Field(
             description="Set the cleanup policy used to automatically deprecate/delete previous versions."
         ),
     ] = None
     dry_run: Annotated[
@@ -102,14 +88,20 @@
     ] = None
     var_async: Annotated[
         StrictBool | None,
         Field(
             description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
+    scale_to_zero: Annotated[
+        StrictBool | None,
+        Field(
+            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. Saves computing resources when the function is not to be used immediately."
+        ),
+    ] = None
     version: Annotated[
         Any | None,
         Field(
             description="If set, the function version will be an increment of the latest existing version that satisfies the `version` range. Note that this increment always takes precedence over an explicit `version` in the function manifest."
         ),
     ] = None
     name: Annotated[
@@ -143,44 +135,28 @@
         extra="allow",
         alias_generator=_create_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _delete_asset_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "chown":
         return "chown"
     if field_name == "comment":
         return "comment"
     if field_name == "author":
         return "author"
     if field_name == "var_async":
         return "async"
     return field_name
 
 
 class DeleteAssetQuery(WaylayBaseModel):
     """Model for `delete_asset` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     chown: Annotated[
         StrictBool | None,
         Field(
             description="If set, ownership of the draft function is transferred to the current user."
         ),
     ] = None
     comment: Annotated[
@@ -755,42 +731,36 @@
         extra="allow",
         alias_generator=_publish_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _rebuild_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
     if field_name == "comment":
         return "comment"
     if field_name == "dry_run":
         return "dryRun"
     if field_name == "var_async":
         return "async"
     if field_name == "upgrade":
         return "upgrade"
     if field_name == "force_version":
         return "forceVersion"
     if field_name == "ignore_checks":
         return "ignoreChecks"
+    if field_name == "scale_to_zero":
+        return "scaleToZero"
     if field_name == "skip_rebuild":
         return "skipRebuild"
     return field_name
 
 
 class RebuildQuery(WaylayBaseModel):
     """Model for `rebuild` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command."
-        ),
-    ] = None
     comment: Annotated[
         StrictStr | None,
         Field(
             description="An optional user-specified comment corresponding to the operation."
         ),
     ] = None
     dry_run: Annotated[
@@ -819,14 +789,20 @@
     ] = None
     ignore_checks: Annotated[
         StrictBool | None,
         Field(
             description="If set to true, checks that normally prevent a rebuild are overriden. These checks include: * function state in `pending`, `running`, `failed` or `undeployed` * backoff period due to recent failures * usage of deprecated dependencies * running jobs on entity * the `dryRun` option"
         ),
     ] = None
+    scale_to_zero: Annotated[
+        StrictBool | None,
+        Field(
+            description="Indicates whether the function needs to be scaled down after successful (re-)deployment. If not set, the function is scaled to zero only if it was not active before this command."
+        ),
+    ] = None
     skip_rebuild: Annotated[
         StrictBool | None,
         Field(
             description="If set, the function will not be rebuild. Always uses the current runtime version when re-deploying/re-verifying the function."
         ),
     ] = None
 
@@ -934,44 +910,28 @@
         extra="allow",
         alias_generator=_remove_versions_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _update_asset_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "chown":
         return "chown"
     if field_name == "comment":
         return "comment"
     if field_name == "author":
         return "author"
     if field_name == "var_async":
         return "async"
     return field_name
 
 
 class UpdateAssetQuery(WaylayBaseModel):
     """Model for `update_asset` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     chown: Annotated[
         StrictBool | None,
         Field(
             description="If set, ownership of the draft function is transferred to the current user."
         ),
     ] = None
     comment: Annotated[
@@ -999,44 +959,28 @@
         extra="allow",
         alias_generator=_update_asset_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _update_assets_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "chown":
         return "chown"
     if field_name == "comment":
         return "comment"
     if field_name == "author":
         return "author"
     if field_name == "var_async":
         return "async"
     return field_name
 
 
 class UpdateAssetsQuery(WaylayBaseModel):
     """Model for `update_assets` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     chown: Annotated[
         StrictBool | None,
         Field(
             description="If set, ownership of the draft function is transferred to the current user."
         ),
     ] = None
     comment: Annotated[
@@ -1064,34 +1008,34 @@
         extra="allow",
         alias_generator=_update_assets_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _verify_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
     if field_name == "var_async":
         return "async"
+    if field_name == "scale_to_zero":
+        return "scaleToZero"
     return field_name
 
 
 class VerifyQuery(WaylayBaseModel):
     """Model for `verify` query parameters."""
 
-    scale_to_zero: Annotated[
+    var_async: Annotated[
         StrictBool | None,
         Field(
-            description="Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command."
+            description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
-    var_async: Annotated[
+    scale_to_zero: Annotated[
         StrictBool | None,
         Field(
-            description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
+            description="Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command."
         ),
     ] = None
 
     model_config = ConfigDict(
         validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay_sdk_registry_types.egg-info/PKG-INFO` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay_sdk_registry_types.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-registry-types
-Version: 2.13.0b20240415
+Version: 2.13.0rc0
 Summary: Waylay Function Registry Types 
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,23 +13,22 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-registry-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/registry.html
 Keywords: Waylay Function Registry,Types
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.0
-Requires-Dist: waylay-sdk-registry==2.13.0b20240415
+Requires-Dist: waylay-sdk~=0.0.4rc5
+Requires-Dist: waylay-sdk-registry==2.13.0rc0
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -45,51 +44,56 @@
 Requires-Dist: pyyaml; extra == "dev"
 Requires-Dist: jsf>=0.11.1; extra == "dev"
 
 # Waylay Registry Service
 V2 API to build and deploy Waylay functions (plugs, webscripts, BYOML models).
 
 This Python package is automatically generated based on the 
-Waylay Registry OpenAPI specification (API version: 2.13.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/registry.html).
+Waylay Registry OpenAPI specification (API version: 2.13.0-beta.0)
 
 It is considered an extension of the waylay-sdk-registry package, and it consists of the typed model classes for all path params, query params, body params and responses for each of the api methods in `waylay-sdk-registry`.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-registry is included in:
-- ```pip install waylay-sdk-core[registry]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[registry]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-registry and waylay-sdk-registry-types are included in:
-- ```pip install waylay-sdk-core[registry,registry-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[registry,registry-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-registry-types` is installed
-from waylay.services.registry.models.root_page_response import RootPageResponse
+from ..models.function_type import FunctionType
+from ..models.job_state_result import JobStateResult
+from ..models.job_type_schema import JobTypeSchema
+from ..models.jobs_response import JobsResponse
 try:
-    # Get Service Status
-    # calls `GET /registry/v2/`
-    api_response = await waylay_client.registry.about.get(
+    # List Jobs
+    # calls `GET /registry/v2/jobs/`
+    api_response = await waylay_client.registry.jobs.list(
+        # query parameters:
+        query = {
+        },
     )
-    print("The response of registry.about.get:\n")
+    print("The response of registry.jobs.list:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling registry.about.get: %s\n" % e)
+    print("Exception when calling registry.jobs.list: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240415/src/waylay_sdk_registry_types.egg-info/SOURCES.txt` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay_sdk_registry_types.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,14 @@
 src/waylay/services/registry/models/rebuild_query_v2.py
 src/waylay/services/registry/models/rebuild_submitted_response.py
 src/waylay/services/registry/models/rebuild_webscript_async_response_v2.py
 src/waylay/services/registry/models/rebuild_webscript_sync_response_v2.py
 src/waylay/services/registry/models/registry_error_response.py
 src/waylay/services/registry/models/remove_function_query_v2.py
 src/waylay/services/registry/models/remove_plug_query_v2.py
-src/waylay/services/registry/models/request_deploy_query.py
 src/waylay/services/registry/models/request_operation.py
 src/waylay/services/registry/models/resource_limits.py
 src/waylay/services/registry/models/root_page_response.py
 src/waylay/services/registry/models/runtime_attributes.py
 src/waylay/services/registry/models/runtime_info.py
 src/waylay/services/registry/models/runtime_name_query.py
 src/waylay/services/registry/models/runtime_params.py
@@ -323,15 +322,14 @@
 src/waylay/services/registry/models/scale_type.py
 src/waylay/services/registry/models/schema_by_id_params.py
 src/waylay/services/registry/models/schema_params.py
 src/waylay/services/registry/models/semantic_version_range.py
 src/waylay/services/registry/models/show_related_type.py
 src/waylay/services/registry/models/status.py
 src/waylay/services/registry/models/status_any.py
-src/waylay/services/registry/models/status_exclude.py
 src/waylay/services/registry/models/status_filter.py
 src/waylay/services/registry/models/status_include.py
 src/waylay/services/registry/models/status_response.py
 src/waylay/services/registry/models/stream_closing.py
 src/waylay/services/registry/models/stream_ready.py
 src/waylay/services/registry/models/supported_events.py
 src/waylay/services/registry/models/tag.py
@@ -387,15 +385,15 @@
 src/waylay/services/registry/models/with_embedded_alt_versions_i_kfserving_response_v2.py
 src/waylay/services/registry/models/with_embedded_alt_versions_i_plug_response_v2.py
 src/waylay/services/registry/models/with_embedded_alt_versions_i_webscript_response_with_invoke_link_v2.py
 src/waylay/services/registry/models/with_entity_attributes.py
 src/waylay/services/registry/models/with_limit.py
 src/waylay/services/registry/models/with_paging.py
 src/waylay/services/registry/queries/__init__.py
-src/waylay/services/registry/queries/about_api.py
+src/waylay/services/registry/queries/default_api.py
 src/waylay/services/registry/queries/jobs_api.py
 src/waylay/services/registry/queries/models_api.py
 src/waylay/services/registry/queries/plugs_api.py
 src/waylay/services/registry/queries/py.typed
 src/waylay/services/registry/queries/runtimes_api.py
 src/waylay/services/registry/queries/schemas_api.py
 src/waylay/services/registry/queries/webscripts_api.py
```

