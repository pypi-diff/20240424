# Comparing `tmp/waylay_sdk_rules_types-6.5.0.20240423.tar.gz` & `tmp/waylay-sdk-rules-types-6.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk_rules_types-6.5.0.20240423.tar", last modified: Wed Apr 24 06:58:33 2024, max compression
+gzip compressed data, was "waylay-sdk-rules-types-6.5.0rc1.tar", last modified: Wed Mar 27 15:35:58 2024, max compression
```

## Comparing `waylay_sdk_rules_types-6.5.0.20240423.tar` & `waylay-sdk-rules-types-6.5.0rc1.tar`

### file list

```diff
@@ -1,138 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:58:33.338338 waylay_sdk_rules_types-6.5.0.20240423/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-24 06:58:33.338338 waylay_sdk_rules_types-6.5.0.20240423/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 06:58:33.338338 waylay_sdk_rules_types-6.5.0.20240423/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:58:33.310338 waylay_sdk_rules_types-6.5.0.20240423/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:58:33.310338 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:58:33.310338 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:58:33.310338 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:58:33.330338 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/
--rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/a_tasks_batch_operation_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/actuator_execution_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/actuator_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_id_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_operation_enqueued.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_operation_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_operation_operation_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_operation_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_task_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_task_command_all_of_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_task_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_task_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_update_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_update_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_update_properties_all_of_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/bayesian_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/create_task201_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/create_template201_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/error_with_details_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/execute_plugs_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/execution_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/failure_operation_result_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/gate_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/generic_task_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/generic_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/get_batch_operation200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/get_discovery_template200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/get_template200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/graph_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/list_tasks200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/list_tasks_format_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/list_tasks_tags_key_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/log_level.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/logs_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/logs_inner_level.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/node_state_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/note_element.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/object.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/one_time_task_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/one_time_task_setting_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/operation_result_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/operation_result_object_results.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/paging_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/patch_task_node_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/periodic_task_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/periodic_task_setting_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/plugin_update_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/plugin_update_spec_from_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/plugin_update_spec_from_version_one_of.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/possible_values_enum_declaration_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/property_updates_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/reactive_task_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/reactive_task_setting_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/relation_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/replace_template200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/resource_data_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/retry_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/run_template_log_level_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/scheduled_task_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/scheduled_task_setting_all_of_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/sensor_execution_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/sensor_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/set_discovery_template200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/simplified_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/simplified_graph_triggers_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/state_change_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/states_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/stream_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/stream_data_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/success_operation_result_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/task_defaults_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/task_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/task_entity_paging_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/task_from_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/task_scenario_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/task_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/task_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/task_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/task_type_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/task_with_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/task_with_rule_all_of_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/template_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/template_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/template_entity_common_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/template_entity_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/template_modification.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/template_modification_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/template_run_actuator_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/template_run_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/template_run_invocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/template_run_sensor_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/template_run_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/template_run_with_graph_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/transformer_execution_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/trigger_state_change.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/upgrade_plugins_templates200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/validation_issue.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/validation_issue_severity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/variable_declaration.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/variable_declaration_default_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/variable_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/variable_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/version_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/version_response_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:58:33.334338 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/queries/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/queries/about_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/queries/plugs_execution_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/queries/push_data_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/queries/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/queries/task_nodes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/queries/tasks_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/queries/tasks_batch_operations_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/queries/template_runs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-24 06:58:27.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/queries/templates_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:58:33.334338 waylay_sdk_rules_types-6.5.0.20240423/src/waylay_sdk_rules_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-24 06:58:33.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay_sdk_rules_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-04-24 06:58:33.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay_sdk_rules_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 06:58:33.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay_sdk_rules_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-24 06:58:33.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay_sdk_rules_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 06:58:33.000000 waylay_sdk_rules_types-6.5.0.20240423/src/waylay_sdk_rules_types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:58.376612 waylay-sdk-rules-types-6.5.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-03-27 15:35:58.376612 waylay-sdk-rules-types-6.5.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 15:35:58.376612 waylay-sdk-rules-types-6.5.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:58.352612 waylay-sdk-rules-types-6.5.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:58.352612 waylay-sdk-rules-types-6.5.0rc1/src/waylay/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:58.352612 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:58.352612 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:58.372612 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/a_tasks_batch_operation_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/actuator_execution_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/actuator_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_id_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_operation_enqueued.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_operation_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_operation_operation_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_operation_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_task_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_task_command_all_of_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_task_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_task_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_update_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_update_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_update_properties_all_of_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/bayesian_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/create_task201_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/create_template201_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/error_with_details_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/execute_plugs_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/execution_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/failure_operation_result_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/gate_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/generic_task_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/generic_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/get_batch_operation200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/get_discovery_template200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/get_template200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/graph_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/list_tasks200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/list_tasks_format_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/list_tasks_tags_key_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/log_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/logs_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/logs_inner_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/node_state_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/note_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/one_time_task_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/one_time_task_setting_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/operation_result_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/operation_result_object_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/paging_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/patch_task_node_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/periodic_task_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/periodic_task_setting_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/plugin_update_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/plugin_update_spec_from_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/plugin_update_spec_from_version_one_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/possible_values_enum_declaration_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/property_updates_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/reactive_task_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/reactive_task_setting_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/relation_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/replace_template200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/resource_data_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/run_template_log_level_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/scheduled_task_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/scheduled_task_setting_all_of_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/sensor_execution_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/sensor_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/set_discovery_template200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/simplified_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/simplified_graph_triggers_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/state_change_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/states_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/stream_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/stream_data_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/success_operation_result_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/task_defaults_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/task_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/task_entity_paging_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/task_from_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/task_scenario_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/task_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/task_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/task_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/task_type_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/task_with_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/task_with_rule_all_of_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/template_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/template_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/template_entity_common_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/template_entity_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/template_modification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/template_modification_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/template_run_actuator_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/template_run_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/template_run_invocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/template_run_sensor_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/template_run_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/template_run_with_graph_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/transformer_execution_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/trigger_state_change.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/upgrade_plugins_templates200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/validation_issue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/validation_issue_severity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/variable_declaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/variable_declaration_default_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/variable_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/variable_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/version_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/version_response_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:58.372612 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/queries/plugs_execution_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/queries/push_data_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/queries/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/queries/task_nodes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/queries/tasks_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/queries/tasks_batch_operations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/queries/template_runs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/queries/templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-27 15:35:47.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/queries/version_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:58.372612 waylay-sdk-rules-types-6.5.0rc1/src/waylay_sdk_rules_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-03-27 15:35:58.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay_sdk_rules_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-03-27 15:35:58.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay_sdk_rules_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 15:35:58.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay_sdk_rules_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-27 15:35:58.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay_sdk_rules_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-27 15:35:58.000000 waylay-sdk-rules-types-6.5.0rc1/src/waylay_sdk_rules_types.egg-info/top_level.txt
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/LICENSE.txt` & `waylay-sdk-rules-types-6.5.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/PKG-INFO` & `waylay-sdk-rules-types-6.5.0rc1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-rules-types
-Version: 6.5.0.20240423
+Version: 6.5.0rc1
 Summary: Waylay rules engine Types 
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,23 +13,21 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-rules-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/rules.html
 Keywords: Waylay rules engine,Types
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.1
-Requires-Dist: waylay-sdk-rules==6.5.0.20240423
+Requires-Dist: waylay-sdk~=0.0.4rc5
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -46,50 +44,52 @@
 Requires-Dist: jsf>=0.11.1; extra == "dev"
 
 # Waylay Rules Service
 The REST api to manage rule tasks and rule templates in the Waylay platform.
 
 This Python package is automatically generated based on the 
 Waylay Rules OpenAPI specification (API version: 6.5.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/rules.html).
 
 It is considered an extension of the waylay-sdk-rules package, and it consists of the typed model classes for all path params, query params, body params and responses for each of the api methods in `waylay-sdk-rules`.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-rules is included in:
-- ```pip install waylay-sdk-core[rules]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[rules]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-rules and waylay-sdk-rules-types are included in:
-- ```pip install waylay-sdk-core[rules,rules-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[rules,rules-types]``` to install `waylay-sdk` along with only this service including the typed models, or
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
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-rules-types` is installed
-from waylay.services.rules.models.version_response import VersionResponse
+from ..models.execute_plugs_specification import ExecutePlugsSpecification
+from ..models.transformer_execution_result import TransformerExecutionResult
 try:
-    # Get Service Information
-    # calls `GET /rules/v1`
-    api_response = await waylay_client.rules.about.get(
+    # Execute Specified Transformer Version
+    # calls `POST /rules/v1/transformers/{name}/versions/{version}`
+    api_response = await waylay_client.rules.plugs_execution.execute_transformer_version(
+        'name_example', # name | path param "name"
+        'version_example', # version | path param "version"
     )
-    print("The response of rules.about.get:\n")
+    print("The response of rules.plugs_execution.execute_transformer_version:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling rules.about.get: %s\n" % e)
+    print("Exception when calling rules.plugs_execution.execute_transformer_version: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/README.md` & `waylay-sdk-rules-types-6.5.0rc1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 # Waylay Rules Service
 The REST api to manage rule tasks and rule templates in the Waylay platform.
 
 This Python package is automatically generated based on the 
 Waylay Rules OpenAPI specification (API version: 6.5.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/rules.html).
 
 It is considered an extension of the waylay-sdk-rules package, and it consists of the typed model classes for all path params, query params, body params and responses for each of the api methods in `waylay-sdk-rules`.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-rules is included in:
-- ```pip install waylay-sdk-core[rules]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[rules]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-rules and waylay-sdk-rules-types are included in:
-- ```pip install waylay-sdk-core[rules,rules-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[rules,rules-types]``` to install `waylay-sdk` along with only this service including the typed models, or
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
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-rules-types` is installed
-from waylay.services.rules.models.version_response import VersionResponse
+from ..models.execute_plugs_specification import ExecutePlugsSpecification
+from ..models.transformer_execution_result import TransformerExecutionResult
 try:
-    # Get Service Information
-    # calls `GET /rules/v1`
-    api_response = await waylay_client.rules.about.get(
+    # Execute Specified Transformer Version
+    # calls `POST /rules/v1/transformers/{name}/versions/{version}`
+    api_response = await waylay_client.rules.plugs_execution.execute_transformer_version(
+        'name_example', # name | path param "name"
+        'version_example', # version | path param "version"
     )
-    print("The response of rules.about.get:\n")
+    print("The response of rules.plugs_execution.execute_transformer_version:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling rules.about.get: %s\n" % e)
+    print("Exception when calling rules.plugs_execution.execute_transformer_version: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/pyproject.toml` & `waylay-sdk-rules-types-6.5.0rc1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-rules-types"
-version = "6.5.0.20240423"
+version = "6.5.0rc1"
 description = "Waylay rules engine Types "
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay rules engine" , "Types"]
 requires-python = ">= 3.9"
 dependencies = [
-    "waylay-sdk-core ~= 0.2.1",
-    "waylay-sdk-rules == 6.5.0.20240423",
+    "waylay-sdk ~= 0.0.4rc5",
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
 Repository = "https://github.com/waylayio/waylay-sdk-rules-py.git"
-"Openapi Specification" = "https://docs.waylay.io/openapi/public/redocly/rules.html"
 
 [project.optional-dependencies]
 dev = [
     "mypy",
     "ruff",
     "types-python-jose",
     "types-appdirs",
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/__init__.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 The REST api to manage rule tasks and rule templates in the Waylay platform.
 
 Generated by OpenAPI Generator (https://openapi-generator.tech)
 
 Do not edit the class manually.
 """
 
-__version__ = "6.5.0.20240423"
+__version__ = "6.5.0rc1"
 
 # import models into model package
 from .a_tasks_batch_operation_specification import ATasksBatchOperationSpecification
 from .actuator_execution_result import ActuatorExecutionResult
 from .actuator_node import ActuatorNode
 from .batch_id_query import BatchIdQuery
 from .batch_operation import BatchOperation
@@ -66,15 +66,14 @@
 from .possible_values_enum_declaration_inner import PossibleValuesEnumDeclarationInner
 from .property_updates_spec import PropertyUpdatesSpec
 from .reactive_task_setting import ReactiveTaskSetting
 from .reactive_task_setting_type import ReactiveTaskSettingType
 from .relation_node import RelationNode
 from .replace_template200_response import ReplaceTemplate200Response
 from .resource_data_injection import ResourceDataInjection
-from .retry_config import RetryConfig
 from .run_template_log_level_parameter import RunTemplateLogLevelParameter
 from .scheduled_task_setting import ScheduledTaskSetting
 from .scheduled_task_setting_all_of_type import ScheduledTaskSettingAllOfType
 from .sensor_execution_result import SensorExecutionResult
 from .sensor_node import SensorNode
 from .simplified_graph import SimplifiedGraph
 from .simplified_graph_triggers_inner import SimplifiedGraphTriggersInner
@@ -171,15 +170,14 @@
     "PossibleValuesEnumDeclarationInner",
     "PropertyUpdatesSpec",
     "ReactiveTaskSetting",
     "ReactiveTaskSettingType",
     "RelationNode",
     "ReplaceTemplate200Response",
     "ResourceDataInjection",
-    "RetryConfig",
     "RunTemplateLogLevelParameter",
     "ScheduledTaskSetting",
     "ScheduledTaskSettingAllOfType",
     "SensorExecutionResult",
     "SensorNode",
     "SimplifiedGraph",
     "SimplifiedGraphTriggersInner",
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/a_tasks_batch_operation_specification.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/a_tasks_batch_operation_specification.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/actuator_execution_result.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/relation_node.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,34 +7,40 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
-from typing import Any, Dict, List
+from typing import List
 
 from pydantic import (
     ConfigDict,
     Field,
-    StrictBool,
+    StrictInt,
     StrictStr,
 )
+from typing_extensions import (
+    Annotated,  # >=3.11
+)
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
+from ..models.gate_type import GateType
 
-class ActuatorExecutionResult(WaylayBaseModel):
-    """ActuatorExecutionResult."""
 
-    result: StrictBool | None = Field(
-        default=None,
-        description="flag indicating if the actuator was successfully executed",
-    )
-    error: StrictStr | None = Field(
-        default=None, description="error message in case of failure"
+class RelationNode(WaylayBaseModel):
+    """Representation of a gate in a Rule Template.."""
+
+    label: StrictStr = Field(description="Unique node label")
+    type: GateType
+    parent_labels: List[StrictStr] = Field(alias="parentLabels")
+    combinations: List[List[StrictStr]]
+    position: Annotated[List[StrictInt], Field(min_length=2, max_length=2)] | None = (
+        None
     )
-    raw_data: Dict[str, Any] | None = Field(default=None, alias="rawData")
-    log: List[Dict[str, Any]] | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/actuator_node.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/actuator_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,9 +45,12 @@
     def version_validate_regular_expression(cls, value):
         """Validate the regular expression."""
         if not re.match(r"\d+\.\d+\.\d+", value):
             raise ValueError(r"must validate the regular expression /\d+\.\d+\.\d+/")
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_id_query.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_id_query.py`

 * *Files 25% similar despite different names*

```diff
@@ -22,9 +22,12 @@
 
 class BatchIdQuery(WaylayBaseModel):
     """BatchIdQuery."""
 
     ids: List[StrictStr]
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_operation.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_operation.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,9 +30,12 @@
     operation: BatchOperationOperation
     queue_time: StrictInt = Field(
         description="Timestamp expressed as milliseconds since 00:00:00 UTC on 1 January 1970, not counting leap seconds.",
         alias="queueTime",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_operation_enqueued.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_operation_enqueued.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,9 +28,12 @@
     status_code: StrictInt = Field(alias="statusCode")
     uri: StrictStr = Field(
         description="URI where the batch operation status can be followed"
     )
     entity: BatchOperation
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_operation_operation.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_operation_operation.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,9 +26,12 @@
     """Summary of the batch operation."""
 
     entity: BatchTaskEntity
     action: BatchOperationOperationAction
     description: StrictStr = Field(description="description of the operations")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_operation_operation_action.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_operation_operation_action.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_operation_result.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_operation_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,9 +36,12 @@
     finished_time: StrictInt = Field(
         description="Timestamp expressed as milliseconds since 00:00:00 UTC on 1 January 1970, not counting leap seconds.",
         alias="finishedTime",
     )
     results: OperationResultObjectResults
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_query.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,9 +62,12 @@
     )
     tags: Dict[str, Any] | None = Field(
         default=None,
         description="Key-value pairs on which you can set at task creation and later filter tasks",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_task.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_task.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,9 +25,12 @@
     """BatchTask."""
 
     entity: BatchTaskEntity | None = None
     action: StrictStr | None = None
     query: BatchTaskQuery | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_task_command.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_task_command.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,9 +25,12 @@
     """Execute command on multiple task."""
 
     entity: BatchTaskEntity
     action: BatchTaskCommandAllOfAction
     query: BatchTaskQuery
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_task_command_all_of_action.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_task_command_all_of_action.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_task_query.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_task_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_update_plugin.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_update_plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,9 +28,12 @@
 
     entity: BatchTaskEntity
     action: TemplateModificationOperation
     query: BatchTaskQuery
     action_parameters: PluginUpdateSpec = Field(alias="actionParameters")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/batch_update_properties.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/batch_update_properties.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,9 +30,12 @@
 
     entity: BatchTaskEntity
     action: BatchUpdatePropertiesAllOfAction
     query: BatchTaskQuery
     action_parameters: PropertyUpdatesSpec | None = Field(alias="actionParameters")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/bayesian_graph.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/bayesian_graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,9 +22,12 @@
 class BayesianGraph(WaylayBaseModel):
     """Graph in BN format."""
 
     nodes: List[Dict[str, Any]] | None = None
     posterior: List[Dict[str, Any]] | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/create_task201_response.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/success_operation_result_value.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,31 +7,28 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
-from typing import List
-
 from pydantic import (
     ConfigDict,
     Field,
-    StrictStr,
+    StrictInt,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.validation_issue import ValidationIssue
-
 
-class CreateTask201Response(WaylayBaseModel):
-    """CreateTask201Response."""
+class SuccessOperationResultValue(WaylayBaseModel):
+    """The keys will be task ids.."""
 
-    id: StrictStr = Field(description="Unique task identifier", alias="ID")
-    warnings: List[ValidationIssue] | None = Field(
-        default=None,
-        description="List of task warning issues. Will only be there if query parameter `returnWarnings` was set to `true`",
+    status_code: StrictInt = Field(
+        description="The statusCode of the operation", alias="statusCode"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/create_template201_response.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/create_template201_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,9 +26,12 @@
     """CreateTemplate201Response."""
 
     status_code: StrictInt = Field(alias="statusCode")
     uri: StrictStr
     entity: TemplateEntity
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/error_response.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/error_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,9 +24,12 @@
     """ErrorResponse."""
 
     status_code: StrictInt = Field(alias="statusCode")
     error: StrictStr
     code: StrictStr | None = Field(default=None, description="Optional error code")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/error_with_details_response.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/error_with_details_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,9 +29,12 @@
 
     status_code: StrictInt = Field(alias="statusCode")
     error: StrictStr
     code: StrictStr | None = Field(default=None, description="Optional error code")
     details: List[ValidationIssue] | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/execute_plugs_specification.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/execute_plugs_specification.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,9 +27,12 @@
     properties: Dict[str, Any] | None = None
     resource: StrictStr | None = Field(
         default=None, description="Unique resource identifier"
     )
     stream_data: Dict[str, Any] | None = Field(default=None, alias="streamData")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/execution_trigger.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/execution_trigger.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,9 +32,12 @@
         description="Unique node label", alias="destinationLabel"
     )
     invocation_policy: Annotated[int, Field(strict=True, ge=1)] | None = Field(
         default=None, alias="invocationPolicy"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/failure_operation_result_value.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/failure_operation_result_value.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,9 +25,12 @@
 
     status_code: StrictInt = Field(
         description="The statusCode of the operation", alias="statusCode"
     )
     error: StrictStr = Field(description="Error description of what went wrong.")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/generic_task_settings.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/generic_task_settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,9 +42,12 @@
     )
     variables: Dict[str, Any] | None = Field(
         default=None,
         description="set of variables which will be used when starting a task and will automatically be injected in the template before starting a task.",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/generic_trigger.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/generic_trigger.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,9 +32,12 @@
         default=None, description="Unique node label", alias="destinationLabel"
     )
     invocation_policy: Annotated[int, Field(strict=True, ge=1)] | None = Field(
         default=None, alias="invocationPolicy"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/get_batch_operation200_response.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/get_batch_operation200_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/get_discovery_template200_response.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/get_discovery_template200_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/get_template200_response.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/get_template200_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/graph_definition.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/graph_definition.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/list_tasks200_response.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/list_tasks200_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/logs_inner.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/stream_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
-from datetime import datetime
-
 from pydantic import (
     ConfigDict,
+    Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.logs_inner_level import LogsInnerLevel
+from ..models.stream_data_data import StreamDataData
 
 
-class LogsInner(WaylayBaseModel):
-    """LogsInner."""
+class StreamData(WaylayBaseModel):
+    """StreamData."""
 
-    time: datetime
-    level: LogsInnerLevel
-    message: StrictStr
+    resource: StrictStr = Field(description="Unique resource identifier")
+    data: StreamDataData
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/node_state_specification.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/actuator_execution_result.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,31 +7,37 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
-from typing import Any, Dict
+from typing import Any, Dict, List
 
 from pydantic import (
     ConfigDict,
     Field,
+    StrictBool,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-class NodeStateSpecification(WaylayBaseModel):
-    """NodeStateSpecification."""
+class ActuatorExecutionResult(WaylayBaseModel):
+    """ActuatorExecutionResult."""
 
-    state: StrictStr | None = Field(
+    result: StrictBool | None = Field(
         default=None,
-        description="State to set. Should be one of the supported states of the sensor",
+        description="flag indicating if the actuator was successfully executed",
     )
-    raw_data: Dict[str, Any] | None = Field(
-        default=None, description="rawData to set", alias="rawData"
+    error: StrictStr | None = Field(
+        default=None, description="error message in case of failure"
     )
+    raw_data: Dict[str, Any] | None = Field(default=None, alias="rawData")
+    log: List[Dict[str, Any]] | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/note_element.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/note_element.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,9 +28,12 @@
 class NoteElement(WaylayBaseModel):
     """Representation of a note in a Rule Template.."""
 
     position: Annotated[List[StrictInt], Field(min_length=2, max_length=2)]
     text: StrictStr
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/one_time_task_setting.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/one_time_task_setting.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,9 +21,12 @@
 
 class OneTimeTaskSetting(WaylayBaseModel):
     """OneTimeTaskSetting."""
 
     type: OneTimeTaskSettingType
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/operation_result_object.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/paging_result.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,22 +14,25 @@
 from pydantic import (
     ConfigDict,
     Field,
     StrictInt,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.operation_result_object_results import OperationResultObjectResults
 
+class PagingResult(WaylayBaseModel):
+    """PagingResult."""
 
-class OperationResultObject(WaylayBaseModel):
-    """Finished Batch Operation results."""
-
-    finished_time: StrictInt = Field(
-        description="Timestamp expressed as milliseconds since 00:00:00 UTC on 1 January 1970, not counting leap seconds.",
-        alias="finishedTime",
+    skip: StrictInt = Field(
+        description="Number of items skipped before this page of results."
+    )
+    limit: StrictInt = Field(description="Size of one page of results.")
+    total: StrictInt = Field(
+        description="Total number of items matching the query of which this is one page of results."
     )
-    results: OperationResultObjectResults
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/operation_result_object_results.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/operation_result_object_results.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,9 +30,12 @@
         description="Object containing the successful operation results. The keys will be task ids."
     )
     failure: Dict[str, FailureOperationResultValue] = Field(
         description="Object containing the unsuccessful operation results. The keys will be tasks ids."
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/paging_result.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/reactive_task_setting.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,27 +9,24 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
-    Field,
-    StrictInt,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
+from ..models.reactive_task_setting_type import ReactiveTaskSettingType
 
-class PagingResult(WaylayBaseModel):
-    """PagingResult."""
 
-    skip: StrictInt = Field(
-        description="Number of items skipped before this page of results."
-    )
-    limit: StrictInt = Field(description="Size of one page of results.")
-    total: StrictInt = Field(
-        description="Total number of items matching the query of which this is one page of results."
-    )
+class ReactiveTaskSetting(WaylayBaseModel):
+    """ReactiveTaskSetting."""
+
+    type: ReactiveTaskSettingType
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/patch_task_node_request.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/patch_task_node_request.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/periodic_task_setting.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/queries/push_data_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # coding: utf-8
-"""Waylay rules engine models.
+"""Waylay rules engine query parameters.
 
 This code was generated from the OpenAPI documentation of 'Waylay rules engine'
 
 Generated by OpenAPI Generator (https://openapi-generator.tech)
 
 Do not edit the class manually.
-
 """
 
-from __future__ import annotations
+from __future__ import annotations  # for Python 3.7–3.9
 
 from pydantic import (
     ConfigDict,
-    Field,
-    StrictInt,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.periodic_task_setting_type import PeriodicTaskSettingType
 
+def _push_query_alias_for(field_name: str) -> str:
+    return field_name
 
-class PeriodicTaskSetting(WaylayBaseModel):
-    """PeriodicTaskSetting."""
 
-    type: PeriodicTaskSettingType
-    frequency: StrictInt = Field(description="polling frequency in milliseconds")
+class PushQuery(WaylayBaseModel):
+    """Model for `push` query parameters."""
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
+        alias_generator=_push_query_alias_for,
+        populate_by_name=True,
     )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/plugin_update_spec.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/plugin_update_spec.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,9 +39,12 @@
     def to_version_validate_regular_expression(cls, value):
         """Validate the regular expression."""
         if not re.match(r"\d+\.\d+\.\d+", value):
             raise ValueError(r"must validate the regular expression /\d+\.\d+\.\d+/")
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/plugin_update_spec_from_version.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/plugin_update_spec_from_version.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/possible_values_enum_declaration_inner.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/possible_values_enum_declaration_inner.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/property_updates_spec.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/property_updates_spec.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,9 +29,12 @@
     )
     tags: Dict[str, Any] | None = Field(
         default=None,
         description="Key-value pairs. Will be merged with the current tags. To delete any of the current tags set the value to `null`",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/relation_node.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/state_change_trigger.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,37 +7,40 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
-from typing import List
-
 from pydantic import (
     ConfigDict,
     Field,
-    StrictInt,
     StrictStr,
 )
 from typing_extensions import (
     Annotated,  # >=3.11
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.gate_type import GateType
+from ..models.trigger_state_change import TriggerStateChange
 
 
-class RelationNode(WaylayBaseModel):
-    """Representation of a gate in a Rule Template.."""
+class StateChangeTrigger(WaylayBaseModel):
+    """A trigger that executes on state change.."""
 
-    label: StrictStr = Field(description="Unique node label")
-    type: GateType
-    parent_labels: List[StrictStr] = Field(alias="parentLabels")
-    combinations: List[List[StrictStr]]
-    position: Annotated[List[StrictInt], Field(min_length=2, max_length=2)] | None = (
-        None
+    source_label: StrictStr = Field(
+        description="Unique node label", alias="sourceLabel"
+    )
+    destination_label: StrictStr = Field(
+        description="Unique node label", alias="destinationLabel"
+    )
+    invocation_policy: Annotated[int, Field(strict=True, ge=1)] | None = Field(
+        default=None, alias="invocationPolicy"
     )
+    state_change_trigger: TriggerStateChange = Field(alias="stateChangeTrigger")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/replace_template200_response.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/replace_template200_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,9 +72,12 @@
     )
     triggers: List[SimplifiedGraphTriggersInner] | None = Field(
         default=None,
         description="List of conditions under which actuators/sensors get executed.",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/resource_data_injection.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/resource_data_injection.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,9 +26,12 @@
     resource: StrictStr = Field(description="Unique resource identifier")
     timestamp: StrictInt | None = Field(
         default=None,
         description="Timestamp expressed as milliseconds since 00:00:00 UTC on 1 January 1970, not counting leap seconds.",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/retry_config.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/sensor_execution_result.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,33 +7,44 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
+from typing import Any, Dict, List
+
 from pydantic import (
     ConfigDict,
     Field,
+    StrictBool,
     StrictStr,
 )
-from typing_extensions import (
-    Annotated,  # >=3.11
-)
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-class RetryConfig(WaylayBaseModel):
-    """Configuration for retrying a template node. The node execution will be retried `maxRetries` times. The delay between retries will be exponentially increased starting from `minBackoff` to `maxBackoff`. If the node execution fails after `maxRetries` retries, the node state will be set to `errorState` if it that property is provided. Otherwise node execution will fail. Error state should be one of the possible states defined by the sensor node.."""
+class SensorExecutionResult(WaylayBaseModel):
+    """SensorExecutionResult."""
 
-    max_retries: Annotated[int, Field(strict=True, ge=0)] = Field(alias="maxRetries")
-    min_backoff: StrictStr = Field(alias="minBackoff")
-    max_backoff: StrictStr = Field(alias="maxBackoff")
-    error_state: StrictStr | None = Field(
+    result: StrictBool | None = Field(
+        default=None,
+        description="flag indicating if the sensor was successfully executed",
+    )
+    state: StrictStr | None = Field(
+        default=None, description="observedState field returned by the sensor execution"
+    )
+    error: StrictStr | None = Field(
+        default=None, description="error message in case of failure"
+    )
+    raw_data: Dict[str, Any] | None = Field(
         default=None,
-        description="Optional sensor state which will be used to set the state of the node when the maxRetries is reached.",
-        alias="errorState",
+        description="the rawData returned by the sensor execution",
+        alias="rawData",
     )
+    log: List[Dict[str, Any]] | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/run_template_log_level_parameter.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/run_template_log_level_parameter.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/scheduled_task_setting.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/scheduled_task_setting.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,9 +28,12 @@
     time_zone: StrictStr | None = Field(
         default=None,
         description="Optional identifier of the time zone in which the schedule expression is to be interpreted",
         alias="timeZone",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/sensor_execution_result.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/template_run_sensor_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     Field,
     StrictBool,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-class SensorExecutionResult(WaylayBaseModel):
-    """SensorExecutionResult."""
+class TemplateRunSensorResult(WaylayBaseModel):
+    """TemplateRunSensorResult."""
 
     result: StrictBool | None = Field(
         default=None,
         description="flag indicating if the sensor was successfully executed",
     )
     state: StrictStr | None = Field(
         default=None, description="observedState field returned by the sensor execution"
@@ -37,11 +37,17 @@
     )
     raw_data: Dict[str, Any] | None = Field(
         default=None,
         description="the rawData returned by the sensor execution",
         alias="rawData",
     )
     log: List[Dict[str, Any]] | None = None
+    executed: StrictBool = Field(
+        description="flag indicating if the sensor was executed"
+    )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/sensor_node.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/sensor_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,16 +23,14 @@
     field_validator,
 )
 from typing_extensions import (
     Annotated,  # >=3.11
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.retry_config import RetryConfig
-
 
 class SensorNode(WaylayBaseModel):
     """Representation of a sensor in a Rule Template.."""
 
     label: StrictStr = Field(description="Unique node label")
     name: StrictStr
     version: Annotated[str, Field(strict=True)]
@@ -59,20 +57,22 @@
     timeout: StrictStr | None = "PT50S"
     timeout_state: StrictStr | None = Field(default=None, alias="timeoutState")
     loop_def: Annotated[str, Field(strict=True)] | None = Field(
         default=None,
         description="A loop definition is a string that defines items over which node will be iterated multiple times. The string is an JSON array of JSON objects.During template execution the sensor node with such a defined loop definition will be invoked for every JSON Object in the JSON array. Parameter is optional. Node will be executed only once if loop definition is not defined.",
         alias="loopDef",
     )
-    retry_config: RetryConfig | None = Field(default=None, alias="retryConfig")
 
     @field_validator("version")
     @classmethod
     def version_validate_regular_expression(cls, value):
         """Validate the regular expression."""
         if not re.match(r"\d+\.\d+\.\d+", value):
             raise ValueError(r"must validate the regular expression /\d+\.\d+\.\d+/")
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/set_discovery_template200_response.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/set_discovery_template200_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/simplified_graph.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/simplified_graph.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,9 +39,12 @@
     )
     triggers: List[SimplifiedGraphTriggersInner] | None = Field(
         default=None,
         description="List of conditions under which actuators/sensors get executed.",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/simplified_graph_triggers_inner.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/simplified_graph_triggers_inner.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/state_change_trigger.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/states_trigger.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,37 +7,43 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
+from typing import List
+
 from pydantic import (
     ConfigDict,
     Field,
     StrictStr,
 )
 from typing_extensions import (
     Annotated,  # >=3.11
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.trigger_state_change import TriggerStateChange
-
 
-class StateChangeTrigger(WaylayBaseModel):
-    """A trigger that executes on state change.."""
+class StatesTrigger(WaylayBaseModel):
+    """A trigger that is conditional on the states of the source.."""
 
     source_label: StrictStr = Field(
         description="Unique node label", alias="sourceLabel"
     )
     destination_label: StrictStr = Field(
         description="Unique node label", alias="destinationLabel"
     )
     invocation_policy: Annotated[int, Field(strict=True, ge=1)] | None = Field(
         default=None, alias="invocationPolicy"
     )
-    state_change_trigger: TriggerStateChange = Field(alias="stateChangeTrigger")
+    states_trigger: List[StrictStr] = Field(
+        description="array of states of source node under which to fire",
+        alias="statesTrigger",
+    )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/states_trigger.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/node_state_specification.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,40 +7,34 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
-from typing import List
+from typing import Any, Dict
 
 from pydantic import (
     ConfigDict,
     Field,
     StrictStr,
 )
-from typing_extensions import (
-    Annotated,  # >=3.11
-)
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-class StatesTrigger(WaylayBaseModel):
-    """A trigger that is conditional on the states of the source.."""
+class NodeStateSpecification(WaylayBaseModel):
+    """NodeStateSpecification."""
 
-    source_label: StrictStr = Field(
-        description="Unique node label", alias="sourceLabel"
-    )
-    destination_label: StrictStr = Field(
-        description="Unique node label", alias="destinationLabel"
-    )
-    invocation_policy: Annotated[int, Field(strict=True, ge=1)] | None = Field(
-        default=None, alias="invocationPolicy"
+    state: StrictStr | None = Field(
+        default=None,
+        description="State to set. Should be one of the supported states of the sensor",
     )
-    states_trigger: List[StrictStr] = Field(
-        description="array of states of source node under which to fire",
-        alias="statesTrigger",
+    raw_data: Dict[str, Any] | None = Field(
+        default=None, description="rawData to set", alias="rawData"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/stream_data.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/trigger_state_change.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 from pydantic import (
     ConfigDict,
     Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.stream_data_data import StreamDataData
 
+class TriggerStateChange(WaylayBaseModel):
+    """State change specification under which to trigger the next node.."""
 
-class StreamData(WaylayBaseModel):
-    """StreamData."""
-
-    resource: StrictStr = Field(description="Unique resource identifier")
-    data: StreamDataData
+    state_from: StrictStr = Field(alias="stateFrom")
+    state_to: StrictStr = Field(alias="stateTo")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/task_defaults_element.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/task_defaults_element.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,9 +54,12 @@
         alias="timeZone",
     )
     frequency: StrictInt | None = Field(
         default=None, description="polling frequency in milliseconds"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/task_entity.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/task_entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,9 +46,12 @@
     resource_ids: List[StrictStr] | None = Field(
         default=None,
         description="List of resources that are used in the task",
         alias="resourceIds",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/task_entity_paging_result.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/task_entity_paging_result.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,9 +32,12 @@
     limit: StrictInt = Field(description="Size of one page of results.")
     total: StrictInt = Field(
         description="Total number of items matching the query of which this is one page of results."
     )
     values: List[TaskEntity] | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/task_from_template.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/task_from_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,19 @@
     )
     type: ReactiveTaskSettingType
     time_zone: StrictStr | None = Field(
         default=None,
         description="Optional identifier of the time zone in which the schedule expression is to be interpreted",
         alias="timeZone",
     )
-    frequency: StrictInt = Field(description="polling frequency in milliseconds")
+    frequency: StrictInt | None = Field(
+        default=None, description="polling frequency in milliseconds"
+    )
     start: StrictBool | None = True
     template: StrictStr = Field(description="Unique template identifier")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/task_scenario_type.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/task_scenario_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/task_settings.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/task_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,12 +49,17 @@
     )
     type: ReactiveTaskSettingType
     time_zone: StrictStr | None = Field(
         default=None,
         description="Optional identifier of the time zone in which the schedule expression is to be interpreted",
         alias="timeZone",
     )
-    frequency: StrictInt = Field(description="polling frequency in milliseconds")
+    frequency: StrictInt | None = Field(
+        default=None, description="polling frequency in milliseconds"
+    )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/task_specification.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/task_specification.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/task_type_settings.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/task_type_settings.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/task_with_rule.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/task_with_rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,9 +43,12 @@
         default=None,
         description="List of conditions under which actuators/sensors get executed.",
     )
     notes: List[NoteElement] | None = None
     task: TaskWithRuleAllOfTask
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/task_with_rule_all_of_task.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/task_with_rule_all_of_task.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,13 +49,18 @@
     )
     type: ReactiveTaskSettingType
     time_zone: StrictStr | None = Field(
         default=None,
         description="Optional identifier of the time zone in which the schedule expression is to be interpreted",
         alias="timeZone",
     )
-    frequency: StrictInt = Field(description="polling frequency in milliseconds")
+    frequency: StrictInt | None = Field(
+        default=None, description="polling frequency in milliseconds"
+    )
     start: StrictBool | None = True
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/template_details.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/template_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,9 +74,12 @@
         default=None,
         description="List of conditions under which actuators/sensors get executed.",
     )
     nodes: List[Dict[str, Any]] | None = None
     posterior: List[Dict[str, Any]] | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/template_entity.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/template_entity.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,9 +63,12 @@
     )
     triggers: List[SimplifiedGraphTriggersInner] | None = Field(
         default=None,
         description="List of conditions under which actuators/sensors get executed.",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="allow"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/template_entity_common_attributes.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/template_entity_common_attributes.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,9 +46,12 @@
         default=None, alias="taskDefaults"
     )
     notes: List[NoteElement] | None = Field(
         default=None, description="List of notes as explanation for users"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/template_entity_metadata.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/template_entity_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,9 +55,12 @@
     )
     last_update_time: StrictInt = Field(
         description="Timestamp expressed as milliseconds since 00:00:00 UTC on 1 January 1970, not counting leap seconds.",
         alias="lastUpdateTime",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/template_modification.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/template_modification.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,9 +32,12 @@
     reload_tasks: StrictBool | None = Field(
         default=False,
         description="Should all tasks created from the template be reloaded",
         alias="reloadTasks",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/template_run_actuator_result.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/template_run_actuator_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,9 +35,12 @@
     raw_data: Dict[str, Any] | None = Field(default=None, alias="rawData")
     log: List[Dict[str, Any]] | None = None
     executed: StrictBool = Field(
         description="flag indicating if the actuator was executed"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/template_run_configuration.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/template_run_configuration.py`

 * *Files 22% similar despite different names*

```diff
@@ -39,9 +39,12 @@
     gates_need_full_observation: StrictBool | None = Field(
         default=False,
         description="Only evaluate gates when all inputs are observed",
         alias="gatesNeedFullObservation",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/template_run_invocation.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/template_run_invocation.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,9 +37,12 @@
     )
     actuators: Dict[str, TemplateRunActuatorResult] = Field(
         description="The execution result for each of the actuators of the template"
     )
     log: List[LogsInner]
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/template_run_specification.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/template_run_specification.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,9 +38,12 @@
     resource_meta_data: Dict[str, Dict[str, Any]] | None = Field(
         default=None,
         description="Metadata for any of the resources used in the template.  The current metadata for all resources used in the template is fetched at the start of the template run. This provided metadata is used to overwrite this current metadata",
         alias="resourceMetaData",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/template_run_with_graph_specification.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/template_run_with_graph_specification.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,9 +40,12 @@
         default=None,
         description="Metadata for any of the resources used in the template.  The current metadata for all resources used in the template is fetched at the start of the template run. This provided metadata is used to overwrite this current metadata",
         alias="resourceMetaData",
     )
     graph: GraphDefinition
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/transformer_execution_result.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/transformer_execution_result.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,9 +32,12 @@
     error: StrictStr | None = Field(
         default=None, description="error message in case of failure"
     )
     data: Dict[str, Any] | None = None
     log: List[Dict[str, Any]] | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/trigger_state_change.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/logs_inner.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,24 +7,31 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
+from datetime import datetime
+
 from pydantic import (
     ConfigDict,
-    Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
+from ..models.logs_inner_level import LogsInnerLevel
+
 
-class TriggerStateChange(WaylayBaseModel):
-    """State change specification under which to trigger the next node.."""
+class LogsInner(WaylayBaseModel):
+    """LogsInner."""
 
-    state_from: StrictStr = Field(alias="stateFrom")
-    state_to: StrictStr = Field(alias="stateTo")
+    time: datetime
+    level: LogsInnerLevel
+    message: StrictStr
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/upgrade_plugins_templates200_response.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/variable_format.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,16 +15,24 @@
 
 from pydantic import (
     ConfigDict,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
+from ..models.possible_values_enum_declaration_inner import (
+    PossibleValuesEnumDeclarationInner,
+)
+
 
-class UpgradePluginsTemplates200Response(WaylayBaseModel):
-    """UpgradePluginsTemplates200Response."""
+class VariableFormat(WaylayBaseModel):
+    """Format for a variable definition.."""
 
-    successful: List[StrictStr] | None = None
+    type: StrictStr
+    values: List[PossibleValuesEnumDeclarationInner] | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/validation_issue.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/validation_issue.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,9 +37,12 @@
     )
     suggestion: StrictStr | None = Field(
         default=None,
         description="Suggestion on how to change the object to get the issue fixed",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/validation_issue_severity.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/validation_issue_severity.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/variable_declaration.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/variable_declaration.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,9 +40,12 @@
         description="flag to indicate if value for variable is mandatory or not",
     )
     default_value: VariableDeclarationDefaultValue | None = Field(
         default=None, alias="defaultValue"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/variable_declaration_default_value.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/variable_declaration_default_value.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/variable_format.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/queries/version_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 # coding: utf-8
-"""Waylay rules engine models.
+"""Waylay rules engine query parameters.
 
 This code was generated from the OpenAPI documentation of 'Waylay rules engine'
 
 Generated by OpenAPI Generator (https://openapi-generator.tech)
 
 Do not edit the class manually.
-
 """
 
-from __future__ import annotations
-
-from typing import List
+from __future__ import annotations  # for Python 3.7–3.9
 
 from pydantic import (
     ConfigDict,
-    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.possible_values_enum_declaration_inner import (
-    PossibleValuesEnumDeclarationInner,
-)
 
+def _get_query_alias_for(field_name: str) -> str:
+    return field_name
 
-class VariableFormat(WaylayBaseModel):
-    """Format for a variable definition.."""
 
-    type: StrictStr
-    values: List[PossibleValuesEnumDeclarationInner] | None = None
+class GetQuery(WaylayBaseModel):
+    """Model for `get` query parameters."""
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        validate_assignment=True,
+        protected_namespaces=(),
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

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/variable_type.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/variable_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/models/version_response.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/models/version_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,9 +30,12 @@
     version: StrictStr
     name: StrictStr
     start_time: datetime | None = Field(default=None, alias="startTime")
     uptime: StrictInt | None = None
     status: VersionResponseStatus
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/queries/about_api.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/queries/tasks_batch_operations_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -20,12 +20,29 @@
     return field_name
 
 
 class GetQuery(WaylayBaseModel):
     """Model for `get` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_query_alias_for,
         populate_by_name=True,
     )
+
+
+def _start_query_alias_for(field_name: str) -> str:
+    return field_name
+
+
+class StartQuery(WaylayBaseModel):
+    """Model for `start` query parameters."""
+
+    model_config = ConfigDict(
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
+        alias_generator=_start_query_alias_for,
+        populate_by_name=True,
+    )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/queries/plugs_execution_api.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/queries/plugs_execution_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     return field_name
 
 
 class ExecuteActuatorQuery(WaylayBaseModel):
     """Model for `execute_actuator` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_execute_actuator_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -35,14 +36,15 @@
     return field_name
 
 
 class ExecuteActuatorVersionQuery(WaylayBaseModel):
     """Model for `execute_actuator_version` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_execute_actuator_version_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -50,14 +52,15 @@
     return field_name
 
 
 class ExecuteSensorQuery(WaylayBaseModel):
     """Model for `execute_sensor` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_execute_sensor_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -65,14 +68,15 @@
     return field_name
 
 
 class ExecuteSensorVersionQuery(WaylayBaseModel):
     """Model for `execute_sensor_version` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_execute_sensor_version_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -80,14 +84,15 @@
     return field_name
 
 
 class ExecuteTransformerQuery(WaylayBaseModel):
     """Model for `execute_transformer` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_execute_transformer_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -95,12 +100,13 @@
     return field_name
 
 
 class ExecuteTransformerVersionQuery(WaylayBaseModel):
     """Model for `execute_transformer_version` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_execute_transformer_version_query_alias_for,
         populate_by_name=True,
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/queries/task_nodes_api.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/queries/task_nodes_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     return field_name
 
 
 class GetStatesQuery(WaylayBaseModel):
     """Model for `get_states` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_states_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -35,14 +36,15 @@
     return field_name
 
 
 class GetQuery(WaylayBaseModel):
     """Model for `get` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -50,14 +52,15 @@
     return field_name
 
 
 class PatchQuery(WaylayBaseModel):
     """Model for `patch` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_patch_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -65,12 +68,13 @@
     return field_name
 
 
 class UpdateQuery(WaylayBaseModel):
     """Model for `update` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_update_query_alias_for,
         populate_by_name=True,
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/queries/tasks_api.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/queries/tasks_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         StrictBool | None,
         Field(
             description="If `true`, result body will contain a list of task warnings that where detected"
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_create_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -65,14 +66,15 @@
     return field_name
 
 
 class DeleteQuery(WaylayBaseModel):
     """Model for `delete` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_delete_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -87,14 +89,15 @@
 
     format: Annotated[
         ListTasksFormatParameter | None,
         Field(description="Format of the graph definition"),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_configuration_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -109,14 +112,15 @@
 
     format: Annotated[
         ListTasksFormatParameter | None,
         Field(description="Format of the graph definition"),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -199,14 +203,15 @@
     ] = None
     created_before: Annotated[
         StrictInt | None,
         Field(description="Tasks created before provided time will be returned"),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_list_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -214,14 +219,15 @@
     return field_name
 
 
 class ReplaceQuery(WaylayBaseModel):
     """Model for `replace` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_replace_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -229,14 +235,15 @@
     return field_name
 
 
 class StartQuery(WaylayBaseModel):
     """Model for `start` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_start_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -244,12 +251,13 @@
     return field_name
 
 
 class StopQuery(WaylayBaseModel):
     """Model for `stop` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_stop_query_alias_for,
         populate_by_name=True,
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/queries/template_runs_api.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/queries/template_runs_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         List[StrictStr] | None,
         Field(
             description="The sensors and actuators part of response will contain only elements related to the asked node of the graph. The returned logs also will be filtered and contain only logs related to the asked node(s)."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_run_graph_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -78,12 +79,13 @@
         List[StrictStr] | None,
         Field(
             description="The sensors and actuators part of response will contain only elements related to the asked node of the graph. The returned logs also will be filtered and contain only logs related to the asked node(s)."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_run_query_alias_for,
         populate_by_name=True,
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay/services/rules/queries/templates_api.py` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay/services/rules/queries/templates_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     return field_name
 
 
 class CreateQuery(WaylayBaseModel):
     """Model for `create` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_create_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -45,14 +46,15 @@
     return field_name
 
 
 class DeleteQuery(WaylayBaseModel):
     """Model for `delete` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_delete_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -60,14 +62,15 @@
     return field_name
 
 
 class GetDiscoveryQuery(WaylayBaseModel):
     """Model for `get_discovery` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_discovery_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -82,14 +85,15 @@
 
     format: Annotated[
         ListTasksFormatParameter | None,
         Field(description="Format of the graph definition"),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -133,14 +137,15 @@
         Field(
             description="either name of a plugin (e.g. `mySensor`), or full version specification of the plug (e.g `mySensor:1.0.3`)"
         ),
     ] = None
     tags_x: StrictStr | None = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_list_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -148,14 +153,15 @@
     return field_name
 
 
 class ReplaceQuery(WaylayBaseModel):
     """Model for `replace` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_replace_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -172,14 +178,15 @@
         StrictStr | None,
         Field(
             description="The template to set as discovery template. If you do not specify this parameter, the current discovery template will be cleared."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_set_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -208,12 +215,13 @@
         Field(
             description="either name of a plugin (e.g. `mySensor`), or full version specification of the plug (e.g `mySensor:1.0.3`)"
         ),
     ] = None
     tags_x: StrictStr | None = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_upgrade_plugins_query_alias_for,
         populate_by_name=True,
     )
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay_sdk_rules_types.egg-info/PKG-INFO` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay_sdk_rules_types.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-rules-types
-Version: 6.5.0.20240423
+Version: 6.5.0rc1
 Summary: Waylay rules engine Types 
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,23 +13,21 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-rules-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/rules.html
 Keywords: Waylay rules engine,Types
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.1
-Requires-Dist: waylay-sdk-rules==6.5.0.20240423
+Requires-Dist: waylay-sdk~=0.0.4rc5
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -46,50 +44,52 @@
 Requires-Dist: jsf>=0.11.1; extra == "dev"
 
 # Waylay Rules Service
 The REST api to manage rule tasks and rule templates in the Waylay platform.
 
 This Python package is automatically generated based on the 
 Waylay Rules OpenAPI specification (API version: 6.5.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/rules.html).
 
 It is considered an extension of the waylay-sdk-rules package, and it consists of the typed model classes for all path params, query params, body params and responses for each of the api methods in `waylay-sdk-rules`.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-rules is included in:
-- ```pip install waylay-sdk-core[rules]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[rules]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-rules and waylay-sdk-rules-types are included in:
-- ```pip install waylay-sdk-core[rules,rules-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[rules,rules-types]``` to install `waylay-sdk` along with only this service including the typed models, or
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
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-rules-types` is installed
-from waylay.services.rules.models.version_response import VersionResponse
+from ..models.execute_plugs_specification import ExecutePlugsSpecification
+from ..models.transformer_execution_result import TransformerExecutionResult
 try:
-    # Get Service Information
-    # calls `GET /rules/v1`
-    api_response = await waylay_client.rules.about.get(
+    # Execute Specified Transformer Version
+    # calls `POST /rules/v1/transformers/{name}/versions/{version}`
+    api_response = await waylay_client.rules.plugs_execution.execute_transformer_version(
+        'name_example', # name | path param "name"
+        'version_example', # version | path param "version"
     )
-    print("The response of rules.about.get:\n")
+    print("The response of rules.plugs_execution.execute_transformer_version:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling rules.about.get: %s\n" % e)
+    print("Exception when calling rules.plugs_execution.execute_transformer_version: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_rules_types-6.5.0.20240423/src/waylay_sdk_rules_types.egg-info/SOURCES.txt` & `waylay-sdk-rules-types-6.5.0rc1/src/waylay_sdk_rules_types.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 src/waylay/services/rules/models/property_updates_spec.py
 src/waylay/services/rules/models/py.typed
 src/waylay/services/rules/models/reactive_task_setting.py
 src/waylay/services/rules/models/reactive_task_setting_type.py
 src/waylay/services/rules/models/relation_node.py
 src/waylay/services/rules/models/replace_template200_response.py
 src/waylay/services/rules/models/resource_data_injection.py
-src/waylay/services/rules/models/retry_config.py
 src/waylay/services/rules/models/run_template_log_level_parameter.py
 src/waylay/services/rules/models/scheduled_task_setting.py
 src/waylay/services/rules/models/scheduled_task_setting_all_of_type.py
 src/waylay/services/rules/models/sensor_execution_result.py
 src/waylay/services/rules/models/sensor_node.py
 src/waylay/services/rules/models/set_discovery_template200_response.py
 src/waylay/services/rules/models/simplified_graph.py
@@ -108,21 +107,21 @@
 src/waylay/services/rules/models/variable_declaration.py
 src/waylay/services/rules/models/variable_declaration_default_value.py
 src/waylay/services/rules/models/variable_format.py
 src/waylay/services/rules/models/variable_type.py
 src/waylay/services/rules/models/version_response.py
 src/waylay/services/rules/models/version_response_status.py
 src/waylay/services/rules/queries/__init__.py
-src/waylay/services/rules/queries/about_api.py
 src/waylay/services/rules/queries/plugs_execution_api.py
 src/waylay/services/rules/queries/push_data_api.py
 src/waylay/services/rules/queries/py.typed
 src/waylay/services/rules/queries/task_nodes_api.py
 src/waylay/services/rules/queries/tasks_api.py
 src/waylay/services/rules/queries/tasks_batch_operations_api.py
 src/waylay/services/rules/queries/template_runs_api.py
 src/waylay/services/rules/queries/templates_api.py
+src/waylay/services/rules/queries/version_api.py
 src/waylay_sdk_rules_types.egg-info/PKG-INFO
 src/waylay_sdk_rules_types.egg-info/SOURCES.txt
 src/waylay_sdk_rules_types.egg-info/dependency_links.txt
 src/waylay_sdk_rules_types.egg-info/requires.txt
 src/waylay_sdk_rules_types.egg-info/top_level.txt
```

