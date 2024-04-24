# Comparing `tmp/types-tensorflow-2.15.0.20240422.tar.gz` & `tmp/types-tensorflow-2.16.0.20240423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-tensorflow-2.15.0.20240422.tar", last modified: Mon Apr 22 02:19:04 2024, max compression
+gzip compressed data, was "types-tensorflow-2.16.0.20240423.tar", last modified: Tue Apr 23 02:20:11 2024, max compression
```

## Comparing `types-tensorflow-2.15.0.20240422.tar` & `types-tensorflow-2.16.0.20240423.tar`

### file list

```diff
@@ -1,204 +1,206 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.828945 types-tensorflow-2.15.0.20240422/
--rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-22 02:19:04.000000 types-tensorflow-2.15.0.20240422/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 02:19:04.000000 types-tensorflow-2.15.0.20240422/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-22 02:19:04.828945 types-tensorflow-2.15.0.20240422/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 02:19:04.828945 types-tensorflow-2.15.0.20240422/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-04-22 02:19:04.000000 types-tensorflow-2.15.0.20240422/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.804945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-22 02:19:04.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)    16608 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/_aliases.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/audio.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/autodiff.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.804945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/autograph/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/autograph/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/autograph/experimental.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/bitwise.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.800945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/compiler/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.804945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/compiler/xla/
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/compiler/xla/autotune_results_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.808945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/compiler/xla/service/
--rw-r--r--   0 runner    (1001) docker     (127)    79109 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/compiler/xla/service/metrics_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    81470 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.808945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/config/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/config/experimental.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.800945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.808945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/example/
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/example/example_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/example/feature_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.812945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/allocation_description_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12387 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/api_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/attr_value_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/cost_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22002 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/dataset_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/dataset_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/device_attributes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/full_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12916 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/function_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/kernel_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/log_memory_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12531 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/node_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15145 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/op_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/optimized_function_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/reader_base_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/resource_handle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/step_stats_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12870 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/summary_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/tensor_description_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/tensor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/variable_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/versions_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.816945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/cluster_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    74211 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/data_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    26003 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/debug_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    28263 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    27444 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/rpc_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    26715 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/saver_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/service_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19383 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/struct_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.816945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tpu/
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    50609 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/util/
--rw-r--r--   0 runner    (1001) docker     (127)    14861 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/util/event_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/util/test_log_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/data/
--rw-r--r--   0 runner    (1001) docker     (127)    11419 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/data/experimental.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/distribute/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/distribute/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/distribute/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/distribute/experimental/coordinator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/dtypes.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/experimental/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/experimental/dtensor.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/feature_column/
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/feature_column/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/initializers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/io/
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/io/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/io/gfile.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/activations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7526 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/callbacks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/constraints.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/initializers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)    12597 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/layers/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/layers/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/layers/experimental/preprocessing.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/layers/preprocessing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/layers/preprocessing/index_lookup.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/losses.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/metrics.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/models.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/optimizers/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/optimizers/schedules.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/regularizers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/linalg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/math.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/nn.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 02:19:04.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.820945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.824945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/distribute/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/distribute/distribute_lib.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.824945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/feature_column/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/feature_column/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8752 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/feature_column/feature_column_v2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.824945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/framework/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/framework/dtypes.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.824945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/keras/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/keras/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.824945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/keras/protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.824945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/trackable/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/trackable/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/trackable/autotrackable.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/trackable/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/trackable/resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/trackable/ressource.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.800945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/training/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.824945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/training/tracking/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/training/tracking/autotrackable.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/random.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/raw_ops.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.824945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/saved_model/
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/saved_model/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/saved_model/experimental.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/sparse.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/strings.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/summary.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.824945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/train/
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/train/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/train/experimental.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.800945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.828945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/autotuning_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/bfc_memory_map_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/coordination_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    25411 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/coordination_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/distributed_runtime_payloads_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19832 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/dnn_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12745 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/rpc_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    24216 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/test_log_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.828945 types-tensorflow-2.15.0.20240422/tensorflow-stubs/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-22 02:18:48.000000 types-tensorflow-2.15.0.20240422/tensorflow-stubs/types/experimental.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:19:04.828945 types-tensorflow-2.15.0.20240422/types_tensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-22 02:19:04.000000 types-tensorflow-2.15.0.20240422/types_tensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-22 02:19:04.000000 types-tensorflow-2.15.0.20240422/types_tensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 02:19:04.000000 types-tensorflow-2.15.0.20240422/types_tensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-22 02:19:04.000000 types-tensorflow-2.15.0.20240422/types_tensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 02:19:04.000000 types-tensorflow-2.15.0.20240422/types_tensorflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.436521 types-tensorflow-2.16.0.20240423/
+-rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-04-23 02:20:10.000000 types-tensorflow-2.16.0.20240423/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 02:20:10.000000 types-tensorflow-2.16.0.20240423/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-23 02:20:11.436521 types-tensorflow-2.16.0.20240423/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 02:20:11.436521 types-tensorflow-2.16.0.20240423/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-04-23 02:20:10.000000 types-tensorflow-2.16.0.20240423/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.416521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-23 02:20:10.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    16662 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/_aliases.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/audio.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/autodiff.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.416521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/autograph/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/autograph/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/autograph/experimental.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/bitwise.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.408521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/compiler/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.416521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/compiler/xla/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.416521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/compiler/xla/service/
+-rw-r--r--   0 runner    (1001) docker     (127)    80163 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/compiler/xla/service/hlo_profile_printer_data_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/compiler/xla/service/metrics_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/compiler/xla/service/test_compilation_environment_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6041 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/compiler/xla/service/xla_compile_result_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    95569 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   126501 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/compiler/xla/xla_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.416521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/config/experimental.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.412521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.416521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/example/example_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/example/feature_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.424521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/allocation_description_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12387 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/api_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/attr_value_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/cost_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/cpp_shape_inference_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    23929 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/dataset_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/dataset_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/device_attributes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/full_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12916 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/function_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/graph_debug_info_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/kernel_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/log_memory_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13024 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/node_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15145 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/op_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/optimized_function_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/reader_base_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/resource_handle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/step_stats_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12870 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/summary_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/tensor_description_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/tensor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/variable_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/versions_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.428521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/cluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    77429 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/data_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    26006 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/debug_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29456 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    27702 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/rpc_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    26715 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/saver_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/service_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20084 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/struct_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.428521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/tpu/
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    51846 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.428521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    14861 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/util/event_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/util/test_log_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.428521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    11419 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/data/experimental.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.428521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/distribute/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/distribute/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/distribute/coordinator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.428521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/distribute/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/distribute/experimental/coordinator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/dtypes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.428521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/experimental/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/experimental/dtensor.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.432521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/feature_column/
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/feature_column/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/initializers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.432521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/io/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/io/gfile.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.432521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/activations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/callbacks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/constraints.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/initializers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.432521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/layers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/losses.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/metrics.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/models.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.432521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/optimizers/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.432521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/optimizers/schedules.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/regularizers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/linalg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/math.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/nn.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 02:20:10.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.432521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.432521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/distribute/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/distribute/distribute_lib.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.432521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/feature_column/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/feature_column/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8752 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/feature_column/feature_column_v2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.432521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/framework/dtypes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.432521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/keras/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.432521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/keras/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.436521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/trackable/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/trackable/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/trackable/autotrackable.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/trackable/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/trackable/resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/trackable/ressource.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.412521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/training/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.436521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/training/tracking/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/training/tracking/autotrackable.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/random.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/raw_ops.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.436521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/saved_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/saved_model/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/saved_model/experimental.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/sparse.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/strings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/summary.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.436521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/train/
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/train/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/train/experimental.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.412521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/tsl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.436521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/tsl/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/tsl/protobuf/bfc_memory_map_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/tsl/protobuf/coordination_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    25411 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/tsl/protobuf/coordination_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/tsl/protobuf/distributed_runtime_payloads_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21347 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/tsl/protobuf/dnn_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12745 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/tsl/protobuf/rpc_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/tsl/protobuf/status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    24216 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/tsl/protobuf/test_log_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.436521 types-tensorflow-2.16.0.20240423/tensorflow-stubs/types/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/types/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-23 02:18:48.000000 types-tensorflow-2.16.0.20240423/tensorflow-stubs/types/experimental.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:20:11.436521 types-tensorflow-2.16.0.20240423/types_tensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-23 02:20:11.000000 types-tensorflow-2.16.0.20240423/types_tensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-04-23 02:20:11.000000 types-tensorflow-2.16.0.20240423/types_tensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 02:20:11.000000 types-tensorflow-2.16.0.20240423/types_tensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-23 02:20:11.000000 types-tensorflow-2.16.0.20240423/types_tensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-23 02:20:11.000000 types-tensorflow-2.16.0.20240423/types_tensorflow.egg-info/top_level.txt
```

### Comparing `types-tensorflow-2.15.0.20240422/CHANGELOG.md` & `types-tensorflow-2.16.0.20240423/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 2.16.0.20240423 (2024-04-23)
+
+Bump tensorflow to 2.16.* (#11696)
+
 ## 2.15.0.20240422 (2024-04-22)
 
 Simplify protoc install in protobuf generation scripts (#11785)
 
 ## 2.15.0.20240417 (2024-04-17)
 
 Remove remaining bare `Incomplete`s (#11768)
```

### Comparing `types-tensorflow-2.15.0.20240422/PKG-INFO` & `types-tensorflow-2.16.0.20240423/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tensorflow
-Version: 2.15.0.20240422
+Version: 2.16.0.20240423
 Summary: Typing stubs for tensorflow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,22 +22,22 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tensorflow`.
 
 This version of `types-tensorflow` aims to provide accurate annotations
-for `tensorflow==2.15.*`.
+for `tensorflow==2.16.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tensorflow. All fixes for
 types and metadata should be contributed there.
 
-Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 25.1 on tensorflow==2.12.1.
+Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 25.1 on tensorflow==2.16.1 .
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1017c525f84b5e78a75ad909c6a4ef2b5c0610e6` and was tested
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
 pytype 2024.4.11.
```

### Comparing `types-tensorflow-2.15.0.20240422/setup.py` & `types-tensorflow-2.16.0.20240423/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,46 +11,46 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tensorflow`.
 
 This version of `types-tensorflow` aims to provide accurate annotations
-for `tensorflow==2.15.*`.
+for `tensorflow==2.16.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tensorflow. All fixes for
 types and metadata should be contributed there.
 
-Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 25.1 on tensorflow==2.12.1.
+Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 25.1 on tensorflow==2.16.1 .
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1017c525f84b5e78a75ad909c6a4ef2b5c0610e6` and was tested
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2.15.0.20240422",
+      version="2.16.0.20240423",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['types-protobuf', 'types-requests', 'numpy>=1.20'],
       packages=['tensorflow-stubs'],
-      package_data={'tensorflow-stubs': ['__init__.pyi', '_aliases.pyi', 'audio.pyi', 'autodiff.pyi', 'autograph/__init__.pyi', 'autograph/experimental.pyi', 'bitwise.pyi', 'compiler/xla/autotune_results_pb2.pyi', 'compiler/xla/service/hlo_pb2.pyi', 'compiler/xla/service/metrics_pb2.pyi', 'compiler/xla/xla_data_pb2.pyi', 'config/__init__.pyi', 'config/experimental.pyi', 'core/example/example_parser_configuration_pb2.pyi', 'core/example/example_pb2.pyi', 'core/example/feature_pb2.pyi', 'core/framework/allocation_description_pb2.pyi', 'core/framework/api_def_pb2.pyi', 'core/framework/attr_value_pb2.pyi', 'core/framework/cost_graph_pb2.pyi', 'core/framework/dataset_metadata_pb2.pyi', 'core/framework/dataset_options_pb2.pyi', 'core/framework/dataset_pb2.pyi', 'core/framework/device_attributes_pb2.pyi', 'core/framework/full_type_pb2.pyi', 'core/framework/function_pb2.pyi', 'core/framework/graph_pb2.pyi', 'core/framework/graph_transfer_info_pb2.pyi', 'core/framework/kernel_def_pb2.pyi', 'core/framework/log_memory_pb2.pyi', 'core/framework/model_pb2.pyi', 'core/framework/node_def_pb2.pyi', 'core/framework/op_def_pb2.pyi', 'core/framework/optimized_function_graph_pb2.pyi', 'core/framework/reader_base_pb2.pyi', 'core/framework/resource_handle_pb2.pyi', 'core/framework/step_stats_pb2.pyi', 'core/framework/summary_pb2.pyi', 'core/framework/tensor_description_pb2.pyi', 'core/framework/tensor_pb2.pyi', 'core/framework/tensor_shape_pb2.pyi', 'core/framework/tensor_slice_pb2.pyi', 'core/framework/types_pb2.pyi', 'core/framework/variable_pb2.pyi', 'core/framework/versions_pb2.pyi', 'core/protobuf/__init__.pyi', 'core/protobuf/bfc_memory_map_pb2.pyi', 'core/protobuf/cluster_pb2.pyi', 'core/protobuf/composite_tensor_variant_pb2.pyi', 'core/protobuf/config_pb2.pyi', 'core/protobuf/control_flow_pb2.pyi', 'core/protobuf/core_platform_payloads_pb2.pyi', 'core/protobuf/data_service_pb2.pyi', 'core/protobuf/debug_event_pb2.pyi', 'core/protobuf/debug_pb2.pyi', 'core/protobuf/device_filters_pb2.pyi', 'core/protobuf/device_properties_pb2.pyi', 'core/protobuf/error_codes_pb2.pyi', 'core/protobuf/fingerprint_pb2.pyi', 'core/protobuf/graph_debug_info_pb2.pyi', 'core/protobuf/meta_graph_pb2.pyi', 'core/protobuf/named_tensor_pb2.pyi', 'core/protobuf/queue_runner_pb2.pyi', 'core/protobuf/remote_tensor_handle_pb2.pyi', 'core/protobuf/rewriter_config_pb2.pyi', 'core/protobuf/rpc_options_pb2.pyi', 'core/protobuf/saved_model_pb2.pyi', 'core/protobuf/saved_object_graph_pb2.pyi', 'core/protobuf/saver_pb2.pyi', 'core/protobuf/service_config_pb2.pyi', 'core/protobuf/snapshot_pb2.pyi', 'core/protobuf/struct_pb2.pyi', 'core/protobuf/tensor_bundle_pb2.pyi', 'core/protobuf/tensorflow_server_pb2.pyi', 'core/protobuf/tpu/compilation_result_pb2.pyi', 'core/protobuf/tpu/dynamic_padding_pb2.pyi', 'core/protobuf/tpu/optimization_parameters_pb2.pyi', 'core/protobuf/tpu/topology_pb2.pyi', 'core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi', 'core/protobuf/trackable_object_graph_pb2.pyi', 'core/protobuf/transport_options_pb2.pyi', 'core/protobuf/verifier_config_pb2.pyi', 'core/util/event_pb2.pyi', 'core/util/memmapped_file_system_pb2.pyi', 'core/util/saved_tensor_slice_pb2.pyi', 'core/util/test_log_pb2.pyi', 'data/__init__.pyi', 'data/experimental.pyi', 'distribute/__init__.pyi', 'distribute/experimental/coordinator.pyi', 'dtypes.pyi', 'experimental/__init__.pyi', 'experimental/dtensor.pyi', 'feature_column/__init__.pyi', 'initializers.pyi', 'io/__init__.pyi', 'io/gfile.pyi', 'keras/__init__.pyi', 'keras/activations.pyi', 'keras/callbacks.pyi', 'keras/constraints.pyi', 'keras/initializers.pyi', 'keras/layers/__init__.pyi', 'keras/layers/experimental/preprocessing.pyi', 'keras/layers/preprocessing/__init__.pyi', 'keras/layers/preprocessing/index_lookup.pyi', 'keras/losses.pyi', 'keras/metrics.pyi', 'keras/models.pyi', 'keras/optimizers/__init__.pyi', 'keras/optimizers/legacy/__init__.pyi', 'keras/optimizers/schedules.pyi', 'keras/regularizers.pyi', 'linalg.pyi', 'math.pyi', 'nn.pyi', 'python/__init__.pyi', 'python/distribute/distribute_lib.pyi', 'python/feature_column/__init__.pyi', 'python/feature_column/feature_column_v2.pyi', 'python/feature_column/sequence_feature_column.pyi', 'python/framework/dtypes.pyi', 'python/keras/__init__.pyi', 'python/keras/protobuf/projector_config_pb2.pyi', 'python/keras/protobuf/saved_metadata_pb2.pyi', 'python/keras/protobuf/versions_pb2.pyi', 'python/trackable/__init__.pyi', 'python/trackable/autotrackable.pyi', 'python/trackable/base.pyi', 'python/trackable/resource.pyi', 'python/trackable/ressource.pyi', 'python/training/tracking/autotrackable.pyi', 'random.pyi', 'raw_ops.pyi', 'saved_model/__init__.pyi', 'saved_model/experimental.pyi', 'sparse.pyi', 'strings.pyi', 'summary.pyi', 'train/__init__.pyi', 'train/experimental.pyi', 'tsl/protobuf/autotuning_pb2.pyi', 'tsl/protobuf/bfc_memory_map_pb2.pyi', 'tsl/protobuf/coordination_config_pb2.pyi', 'tsl/protobuf/coordination_service_pb2.pyi', 'tsl/protobuf/distributed_runtime_payloads_pb2.pyi', 'tsl/protobuf/dnn_pb2.pyi', 'tsl/protobuf/error_codes_pb2.pyi', 'tsl/protobuf/histogram_pb2.pyi', 'tsl/protobuf/rpc_options_pb2.pyi', 'tsl/protobuf/test_log_pb2.pyi', 'types/experimental.pyi', 'METADATA.toml', 'py.typed']},
+      package_data={'tensorflow-stubs': ['__init__.pyi', '_aliases.pyi', 'audio.pyi', 'autodiff.pyi', 'autograph/__init__.pyi', 'autograph/experimental.pyi', 'bitwise.pyi', 'compiler/xla/service/hlo_pb2.pyi', 'compiler/xla/service/hlo_profile_printer_data_pb2.pyi', 'compiler/xla/service/metrics_pb2.pyi', 'compiler/xla/service/test_compilation_environment_pb2.pyi', 'compiler/xla/service/xla_compile_result_pb2.pyi', 'compiler/xla/xla_data_pb2.pyi', 'compiler/xla/xla_pb2.pyi', 'config/__init__.pyi', 'config/experimental.pyi', 'core/example/example_parser_configuration_pb2.pyi', 'core/example/example_pb2.pyi', 'core/example/feature_pb2.pyi', 'core/framework/allocation_description_pb2.pyi', 'core/framework/api_def_pb2.pyi', 'core/framework/attr_value_pb2.pyi', 'core/framework/cost_graph_pb2.pyi', 'core/framework/cpp_shape_inference_pb2.pyi', 'core/framework/dataset_metadata_pb2.pyi', 'core/framework/dataset_options_pb2.pyi', 'core/framework/dataset_pb2.pyi', 'core/framework/device_attributes_pb2.pyi', 'core/framework/full_type_pb2.pyi', 'core/framework/function_pb2.pyi', 'core/framework/graph_debug_info_pb2.pyi', 'core/framework/graph_pb2.pyi', 'core/framework/graph_transfer_info_pb2.pyi', 'core/framework/kernel_def_pb2.pyi', 'core/framework/log_memory_pb2.pyi', 'core/framework/model_pb2.pyi', 'core/framework/node_def_pb2.pyi', 'core/framework/op_def_pb2.pyi', 'core/framework/optimized_function_graph_pb2.pyi', 'core/framework/reader_base_pb2.pyi', 'core/framework/resource_handle_pb2.pyi', 'core/framework/step_stats_pb2.pyi', 'core/framework/summary_pb2.pyi', 'core/framework/tensor_description_pb2.pyi', 'core/framework/tensor_pb2.pyi', 'core/framework/tensor_shape_pb2.pyi', 'core/framework/tensor_slice_pb2.pyi', 'core/framework/types_pb2.pyi', 'core/framework/variable_pb2.pyi', 'core/framework/versions_pb2.pyi', 'core/protobuf/__init__.pyi', 'core/protobuf/bfc_memory_map_pb2.pyi', 'core/protobuf/cluster_pb2.pyi', 'core/protobuf/composite_tensor_variant_pb2.pyi', 'core/protobuf/config_pb2.pyi', 'core/protobuf/control_flow_pb2.pyi', 'core/protobuf/core_platform_payloads_pb2.pyi', 'core/protobuf/data_service_pb2.pyi', 'core/protobuf/debug_event_pb2.pyi', 'core/protobuf/debug_pb2.pyi', 'core/protobuf/device_filters_pb2.pyi', 'core/protobuf/device_properties_pb2.pyi', 'core/protobuf/error_codes_pb2.pyi', 'core/protobuf/fingerprint_pb2.pyi', 'core/protobuf/meta_graph_pb2.pyi', 'core/protobuf/named_tensor_pb2.pyi', 'core/protobuf/queue_runner_pb2.pyi', 'core/protobuf/remote_tensor_handle_pb2.pyi', 'core/protobuf/rewriter_config_pb2.pyi', 'core/protobuf/rpc_options_pb2.pyi', 'core/protobuf/saved_model_pb2.pyi', 'core/protobuf/saved_object_graph_pb2.pyi', 'core/protobuf/saver_pb2.pyi', 'core/protobuf/service_config_pb2.pyi', 'core/protobuf/snapshot_pb2.pyi', 'core/protobuf/status_pb2.pyi', 'core/protobuf/struct_pb2.pyi', 'core/protobuf/tensor_bundle_pb2.pyi', 'core/protobuf/tensorflow_server_pb2.pyi', 'core/protobuf/tpu/compilation_result_pb2.pyi', 'core/protobuf/tpu/dynamic_padding_pb2.pyi', 'core/protobuf/tpu/optimization_parameters_pb2.pyi', 'core/protobuf/tpu/topology_pb2.pyi', 'core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi', 'core/protobuf/trackable_object_graph_pb2.pyi', 'core/protobuf/transport_options_pb2.pyi', 'core/protobuf/verifier_config_pb2.pyi', 'core/util/event_pb2.pyi', 'core/util/memmapped_file_system_pb2.pyi', 'core/util/saved_tensor_slice_pb2.pyi', 'core/util/test_log_pb2.pyi', 'data/__init__.pyi', 'data/experimental.pyi', 'distribute/__init__.pyi', 'distribute/coordinator.pyi', 'distribute/experimental/coordinator.pyi', 'dtypes.pyi', 'experimental/__init__.pyi', 'experimental/dtensor.pyi', 'feature_column/__init__.pyi', 'initializers.pyi', 'io/__init__.pyi', 'io/gfile.pyi', 'keras/__init__.pyi', 'keras/activations.pyi', 'keras/callbacks.pyi', 'keras/constraints.pyi', 'keras/initializers.pyi', 'keras/layers/__init__.pyi', 'keras/losses.pyi', 'keras/metrics.pyi', 'keras/models.pyi', 'keras/optimizers/__init__.pyi', 'keras/optimizers/legacy/__init__.pyi', 'keras/optimizers/schedules.pyi', 'keras/regularizers.pyi', 'linalg.pyi', 'math.pyi', 'nn.pyi', 'python/__init__.pyi', 'python/distribute/distribute_lib.pyi', 'python/feature_column/__init__.pyi', 'python/feature_column/feature_column_v2.pyi', 'python/feature_column/sequence_feature_column.pyi', 'python/framework/dtypes.pyi', 'python/keras/__init__.pyi', 'python/keras/protobuf/projector_config_pb2.pyi', 'python/keras/protobuf/saved_metadata_pb2.pyi', 'python/keras/protobuf/versions_pb2.pyi', 'python/trackable/__init__.pyi', 'python/trackable/autotrackable.pyi', 'python/trackable/base.pyi', 'python/trackable/resource.pyi', 'python/trackable/ressource.pyi', 'python/training/tracking/autotrackable.pyi', 'random.pyi', 'raw_ops.pyi', 'saved_model/__init__.pyi', 'saved_model/experimental.pyi', 'sparse.pyi', 'strings.pyi', 'summary.pyi', 'train/__init__.pyi', 'train/experimental.pyi', 'tsl/protobuf/bfc_memory_map_pb2.pyi', 'tsl/protobuf/coordination_config_pb2.pyi', 'tsl/protobuf/coordination_service_pb2.pyi', 'tsl/protobuf/distributed_runtime_payloads_pb2.pyi', 'tsl/protobuf/dnn_pb2.pyi', 'tsl/protobuf/error_codes_pb2.pyi', 'tsl/protobuf/histogram_pb2.pyi', 'tsl/protobuf/rpc_options_pb2.pyi', 'tsl/protobuf/status_pb2.pyi', 'tsl/protobuf/test_log_pb2.pyi', 'types/__init__.pyi', 'types/experimental.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/__init__.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import abc
 from _typeshed import Incomplete, Unused
 from abc import ABC, ABCMeta, abstractmethod
 from builtins import bool as _bool
 from collections.abc import Callable, Iterable, Iterator, Sequence
 from contextlib import contextmanager
 from enum import Enum
 from types import TracebackType
@@ -13,14 +14,15 @@
     data as data,
     experimental as experimental,
     feature_column as feature_column,
     initializers as initializers,
     io as io,
     keras as keras,
     math as math,
+    types as types,
 )
 from tensorflow._aliases import AnyArray, DTypeLike, ShapeLike, Slice, TensorCompatible
 from tensorflow.autodiff import GradientTape as GradientTape
 from tensorflow.core.protobuf import struct_pb2
 from tensorflow.dtypes import *
 from tensorflow.experimental.dtensor import Layout
 from tensorflow.keras import losses as losses
@@ -253,15 +255,15 @@
     @property
     def graph(self) -> Graph: ...
     @property
     def device(self) -> str: ...
     def __neg__(self) -> IndexedSlices: ...
     def consumers(self) -> list[Operation]: ...
 
-class name_scope:
+class name_scope(metaclass=abc.ABCMeta):
     def __init__(self, name: str) -> None: ...
     def __enter__(self) -> str: ...
     def __exit__(self, typ: type[BaseException] | None, value: BaseException | None, traceback: TracebackType | None) -> None: ...
 
 _P = ParamSpec("_P")
 _R = TypeVar("_R")
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/_aliases.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/_aliases.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/autodiff.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/autodiff.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/autograph/__init__.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/autograph/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/autograph/experimental.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/autograph/experimental.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/bitwise.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/bitwise.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/compiler/xla/autotune_results_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/graph_pb2.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,92 +1,91 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
-Copyright 2022 The TensorFlow Authors. All Rights Reserved.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-==============================================================================
 """
 
 import builtins
 import collections.abc
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import tensorflow.tsl.protobuf.autotuning_pb2
+import tensorflow.core.framework.function_pb2
+import tensorflow.core.framework.graph_debug_info_pb2
+import tensorflow.core.framework.node_def_pb2
+import tensorflow.core.framework.versions_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing.final
-class AutotuneResults(google.protobuf.message.Message):
-    """A collection of algorithms for particular dot/convs.  Usually this is "the
-    best" algorithm for the particular dot/conv, although that's not strictly
-    required.
-
-    Users don't interact with this proto directly.  It's used internally to
-    facilitate ahead-of-time autotuning -- The string used by
-    xla::{Serialize,Load}AutotuneResults is, internally, a serialization of this
-    proto.
-
-    LINT.IfChange
-    """
+class GraphDef(google.protobuf.message.Message):
+    """Represents the graph of operations"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing.final
-    class Entry(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-        DEVICE_FIELD_NUMBER: builtins.int
-        HLO_FIELD_NUMBER: builtins.int
-        RESULT_FIELD_NUMBER: builtins.int
-        device: builtins.str
-        hlo: builtins.str
-        @property
-        def result(self) -> tensorflow.tsl.protobuf.autotuning_pb2.AutotuneResult:
-            """nb: These results are always tied to a particular version of
-            cublas/cudnn, but this is *especially* true for cublasLt results.  For
-            cublasLt gemms, the result is an index into the list of candidate
-            algorithms returned by cublasLt.  Different version of cublasLt ->
-            different list of algos -> different interpretation of results!
-            """
-
-        def __init__(
-            self,
-            *,
-            device: builtins.str | None = ...,
-            hlo: builtins.str | None = ...,
-            result: tensorflow.tsl.protobuf.autotuning_pb2.AutotuneResult | None = ...,
-        ) -> None: ...
-        def HasField(self, field_name: typing.Literal["result", b"result"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing.Literal["device", b"device", "hlo", b"hlo", "result", b"result"]) -> None: ...
-
+    NODE_FIELD_NUMBER: builtins.int
+    VERSIONS_FIELD_NUMBER: builtins.int
     VERSION_FIELD_NUMBER: builtins.int
-    DOTS_FIELD_NUMBER: builtins.int
-    CONVS_FIELD_NUMBER: builtins.int
+    LIBRARY_FIELD_NUMBER: builtins.int
+    DEBUG_INFO_FIELD_NUMBER: builtins.int
     version: builtins.int
+    """Deprecated single version field; use versions above instead.  Since all
+    GraphDef changes before "versions" was introduced were forward
+    compatible, this field is entirely ignored.
+    """
     @property
-    def dots(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___AutotuneResults.Entry]: ...
+    def node(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.core.framework.node_def_pb2.NodeDef]: ...
     @property
-    def convs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___AutotuneResults.Entry]: ...
+    def versions(self) -> tensorflow.core.framework.versions_pb2.VersionDef:
+        """Compatibility versions of the graph.  See core/public/version.h for version
+        history.  The GraphDef version is distinct from the TensorFlow version, and
+        each release of TensorFlow will support a range of GraphDef versions.
+        """
+
+    @property
+    def library(self) -> tensorflow.core.framework.function_pb2.FunctionDefLibrary:
+        """"library" provides user-defined functions.
+
+        Naming:
+          * library.function.name are in a flat namespace.
+            NOTE: We may need to change it to be hierarchical to support
+            different orgs. E.g.,
+            { "/google/nn", { ... }},
+            { "/google/vision", { ... }}
+            { "/org_foo/module_bar", { ... }}
+            map<string, FunctionDefLib> named_lib;
+          * If node[i].op is the name of one function in "library",
+            node[i] is deemed as a function call. Otherwise, node[i].op
+            must be a primitive operation supported by the runtime.
+
+
+        Function call semantics:
+
+          * The callee may start execution as soon as some of its inputs
+            are ready. The caller may want to use Tuple() mechanism to
+            ensure all inputs are ready in the same time.
+
+          * The consumer of return values may start executing as soon as
+            the return values the consumer depends on are ready.  The
+            consumer may want to use Tuple() mechanism to ensure the
+            consumer does not start until all return values of the callee
+            function are ready.
+        """
+
+    @property
+    def debug_info(self) -> tensorflow.core.framework.graph_debug_info_pb2.GraphDebugInfo:
+        """Stack traces for the nodes in this graph."""
+
     def __init__(
         self,
         *,
+        node: collections.abc.Iterable[tensorflow.core.framework.node_def_pb2.NodeDef] | None = ...,
+        versions: tensorflow.core.framework.versions_pb2.VersionDef | None = ...,
         version: builtins.int | None = ...,
-        dots: collections.abc.Iterable[global___AutotuneResults.Entry] | None = ...,
-        convs: collections.abc.Iterable[global___AutotuneResults.Entry] | None = ...,
+        library: tensorflow.core.framework.function_pb2.FunctionDefLibrary | None = ...,
+        debug_info: tensorflow.core.framework.graph_debug_info_pb2.GraphDebugInfo | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing.Literal["convs", b"convs", "dots", b"dots", "version", b"version"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["debug_info", b"debug_info", "library", b"library", "versions", b"versions"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["debug_info", b"debug_info", "library", b"library", "node", b"node", "version", b"version", "versions", b"versions"]) -> None: ...
 
-global___AutotuneResults = AutotuneResults
+global___GraphDef = GraphDef
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 """
 
 import builtins
 import collections.abc
 import sys
 import typing
 
+import google.protobuf.any_pb2
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import tensorflow.compiler.xla.xla_data_pb2
 
 if sys.version_info >= (3, 10):
@@ -214,15 +215,15 @@
 MUST_ALIAS: Kind.ValueType  # 2
 """The buffers must alias at runtime."""
 global___Kind = Kind
 
 @typing.final
 class HloInstructionProto(google.protobuf.message.Message):
     """Serialization of HloInstruction.
-    Next ID: 81
+    Next ID: 87
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing.final
     class SliceDimensions(google.protobuf.message.Message):
         """Describes the [begin, end) index range and stride for slices."""
@@ -306,16 +307,19 @@
     UNIQUE_INDICES_FIELD_NUMBER: builtins.int
     RNG_ALGORITHM_FIELD_NUMBER: builtins.int
     COMPARISON_TYPE_FIELD_NUMBER: builtins.int
     IS_CROSS_PROGRAM_PREFETCH_FIELD_NUMBER: builtins.int
     CROSS_PROGRAM_PREFETCH_INDEX_FIELD_NUMBER: builtins.int
     PADDING_TYPE_FIELD_NUMBER: builtins.int
     CUSTOM_CALL_API_VERSION_FIELD_NUMBER: builtins.int
-    ASYNC_GROUP_ID_FIELD_NUMBER: builtins.int
     ASYNC_EXECUTION_THREAD_FIELD_NUMBER: builtins.int
+    K_FIELD_NUMBER: builtins.int
+    LARGEST_FIELD_NUMBER: builtins.int
+    STATISTICS_VIZ_FIELD_NUMBER: builtins.int
+    DOT_SPARSITY_FIELD_NUMBER: builtins.int
     name: builtins.str
     opcode: builtins.str
     parameter_number: builtins.int
     """Parameter number is only present for kParameter."""
     fusion_kind: builtins.str
     """Fusion state, only present for kFusion."""
     tuple_index: builtins.int
@@ -416,24 +420,23 @@
     """If a convolution is dynamic, a dynamic padding type will be specified."""
     custom_call_api_version: global___CustomCallApiVersion.ValueType
     """The API version used by the custom call function. This field is only
     present for custom-call.
     TODO(b/189822916): Remove this field when all clients are migrated to the
     status-returning API.
     """
-    async_group_id: builtins.int
-    """Represents a unique identifier for an async group which consists of an
-    async start, async done, and zero or more async update operations.
-    Negative async_group_id is equivalent to no async group id.
-    """
     async_execution_thread: builtins.str
     """Represents a unique execution thread name for one or more async groups.
     Each HLO module may contain a main thread and one or more parallel threads.
     Empty async_execution_thread is equivalent to main thread.
     """
+    k: builtins.int
+    """Represents the K value for top-k."""
+    largest: builtins.bool
+    """Represents the largest flag for top-k."""
     @property
     def shape(self) -> tensorflow.compiler.xla.xla_data_pb2.ShapeProto: ...
     @property
     def metadata(self) -> tensorflow.compiler.xla.xla_data_pb2.OpMetadata: ...
     @property
     def literal(self) -> tensorflow.compiler.xla.xla_data_pb2.LiteralProto:
         """Literal, only present for kConstant."""
@@ -532,14 +535,24 @@
         between output and operands for kCustomCall and kFusion.
         """
 
     @property
     def frontend_attributes(self) -> tensorflow.compiler.xla.xla_data_pb2.FrontendAttributes:
         """Frontend attributes to pass to the XLA backend."""
 
+    @property
+    def statistics_viz(self) -> tensorflow.compiler.xla.xla_data_pb2.StatisticsViz:
+        """Represents the information for tracking propagation of values within HLO
+        graph.
+        """
+
+    @property
+    def dot_sparsity(self) -> tensorflow.compiler.xla.xla_data_pb2.SparsityDescriptor:
+        """Sparsity descriptor for dot operation."""
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         opcode: builtins.str | None = ...,
         shape: tensorflow.compiler.xla.xla_data_pb2.ShapeProto | None = ...,
         metadata: tensorflow.compiler.xla.xla_data_pb2.OpMetadata | None = ...,
@@ -601,19 +614,22 @@
         unique_indices: builtins.bool | None = ...,
         rng_algorithm: tensorflow.compiler.xla.xla_data_pb2.RandomAlgorithm.ValueType | None = ...,
         comparison_type: builtins.str | None = ...,
         is_cross_program_prefetch: builtins.bool | None = ...,
         cross_program_prefetch_index: builtins.int | None = ...,
         padding_type: tensorflow.compiler.xla.xla_data_pb2.PaddingType.ValueType | None = ...,
         custom_call_api_version: global___CustomCallApiVersion.ValueType | None = ...,
-        async_group_id: builtins.int | None = ...,
         async_execution_thread: builtins.str | None = ...,
+        k: builtins.int | None = ...,
+        largest: builtins.bool | None = ...,
+        statistics_viz: tensorflow.compiler.xla.xla_data_pb2.StatisticsViz | None = ...,
+        dot_sparsity: tensorflow.compiler.xla.xla_data_pb2.SparsityDescriptor | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing.Literal["cholesky_options", b"cholesky_options", "convolution_dimension_numbers", b"convolution_dimension_numbers", "cross_program_prefetch_index", b"cross_program_prefetch_index", "domain_entry_sharding", b"domain_entry_sharding", "domain_exit_sharding", b"domain_exit_sharding", "dot_dimension_numbers", b"dot_dimension_numbers", "frontend_attributes", b"frontend_attributes", "gather_dimension_numbers", b"gather_dimension_numbers", "literal", b"literal", "metadata", b"metadata", "optional_cross_program_prefetch_index", b"optional_cross_program_prefetch_index", "outfeed_shape", b"outfeed_shape", "padding_config", b"padding_config", "parameter_replication", b"parameter_replication", "precision_config", b"precision_config", "scatter_dimension_numbers", b"scatter_dimension_numbers", "shape", b"shape", "sharding", b"sharding", "triangular_solve_options", b"triangular_solve_options", "window", b"window"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing.Literal["all_reduce_id", b"all_reduce_id", "async_execution_thread", b"async_execution_thread", "async_group_id", b"async_group_id", "backend_config", b"backend_config", "batch_group_count", b"batch_group_count", "called_computation_ids", b"called_computation_ids", "channel_id", b"channel_id", "cholesky_options", b"cholesky_options", "comparison_direction", b"comparison_direction", "comparison_type", b"comparison_type", "constrain_layout", b"constrain_layout", "control_predecessor_ids", b"control_predecessor_ids", "convolution_dimension_numbers", b"convolution_dimension_numbers", "cross_program_prefetch_index", b"cross_program_prefetch_index", "custom_call_api_version", b"custom_call_api_version", "custom_call_has_side_effect", b"custom_call_has_side_effect", "custom_call_schedule", b"custom_call_schedule", "custom_call_target", b"custom_call_target", "delta", b"delta", "dimensions", b"dimensions", "distribution", b"distribution", "domain_entry_sharding", b"domain_entry_sharding", "domain_exit_sharding", b"domain_exit_sharding", "dot_dimension_numbers", b"dot_dimension_numbers", "dynamic_slice_sizes", b"dynamic_slice_sizes", "epsilon", b"epsilon", "exponent_bits", b"exponent_bits", "feature_group_count", b"feature_group_count", "feature_index", b"feature_index", "fft_length", b"fft_length", "fft_type", b"fft_type", "frontend_attributes", b"frontend_attributes", "fusion_kind", b"fusion_kind", "gather_dimension_numbers", b"gather_dimension_numbers", "gather_slice_sizes", b"gather_slice_sizes", "id", b"id", "indices_are_sorted", b"indices_are_sorted", "infeed_config", b"infeed_config", "is_cross_program_prefetch", b"is_cross_program_prefetch", "is_host_transfer", b"is_host_transfer", "is_stable", b"is_stable", "literal", b"literal", "mantissa_bits", b"mantissa_bits", "metadata", b"metadata", "name", b"name", "opcode", b"opcode", "operand_ids", b"operand_ids", "operand_shapes_with_layout", b"operand_shapes_with_layout", "optional_cross_program_prefetch_index", b"optional_cross_program_prefetch_index", "outfeed_config", b"outfeed_config", "outfeed_shape", b"outfeed_shape", "output_operand_aliasing", b"output_operand_aliasing", "padding_config", b"padding_config", "padding_type", b"padding_type", "parameter_number", b"parameter_number", "parameter_replication", b"parameter_replication", "precision_config", b"precision_config", "replica_groups", b"replica_groups", "rng_algorithm", b"rng_algorithm", "scatter_dimension_numbers", b"scatter_dimension_numbers", "shape", b"shape", "sharding", b"sharding", "slice_dimensions", b"slice_dimensions", "source_target_pairs", b"source_target_pairs", "triangular_solve_options", b"triangular_solve_options", "tuple_index", b"tuple_index", "unique_indices", b"unique_indices", "use_global_device_ids", b"use_global_device_ids", "window", b"window"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["cholesky_options", b"cholesky_options", "convolution_dimension_numbers", b"convolution_dimension_numbers", "cross_program_prefetch_index", b"cross_program_prefetch_index", "domain_entry_sharding", b"domain_entry_sharding", "domain_exit_sharding", b"domain_exit_sharding", "dot_dimension_numbers", b"dot_dimension_numbers", "dot_sparsity", b"dot_sparsity", "frontend_attributes", b"frontend_attributes", "gather_dimension_numbers", b"gather_dimension_numbers", "literal", b"literal", "metadata", b"metadata", "optional_cross_program_prefetch_index", b"optional_cross_program_prefetch_index", "outfeed_shape", b"outfeed_shape", "padding_config", b"padding_config", "parameter_replication", b"parameter_replication", "precision_config", b"precision_config", "scatter_dimension_numbers", b"scatter_dimension_numbers", "shape", b"shape", "sharding", b"sharding", "statistics_viz", b"statistics_viz", "triangular_solve_options", b"triangular_solve_options", "window", b"window"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["all_reduce_id", b"all_reduce_id", "async_execution_thread", b"async_execution_thread", "backend_config", b"backend_config", "batch_group_count", b"batch_group_count", "called_computation_ids", b"called_computation_ids", "channel_id", b"channel_id", "cholesky_options", b"cholesky_options", "comparison_direction", b"comparison_direction", "comparison_type", b"comparison_type", "constrain_layout", b"constrain_layout", "control_predecessor_ids", b"control_predecessor_ids", "convolution_dimension_numbers", b"convolution_dimension_numbers", "cross_program_prefetch_index", b"cross_program_prefetch_index", "custom_call_api_version", b"custom_call_api_version", "custom_call_has_side_effect", b"custom_call_has_side_effect", "custom_call_schedule", b"custom_call_schedule", "custom_call_target", b"custom_call_target", "delta", b"delta", "dimensions", b"dimensions", "distribution", b"distribution", "domain_entry_sharding", b"domain_entry_sharding", "domain_exit_sharding", b"domain_exit_sharding", "dot_dimension_numbers", b"dot_dimension_numbers", "dot_sparsity", b"dot_sparsity", "dynamic_slice_sizes", b"dynamic_slice_sizes", "epsilon", b"epsilon", "exponent_bits", b"exponent_bits", "feature_group_count", b"feature_group_count", "feature_index", b"feature_index", "fft_length", b"fft_length", "fft_type", b"fft_type", "frontend_attributes", b"frontend_attributes", "fusion_kind", b"fusion_kind", "gather_dimension_numbers", b"gather_dimension_numbers", "gather_slice_sizes", b"gather_slice_sizes", "id", b"id", "indices_are_sorted", b"indices_are_sorted", "infeed_config", b"infeed_config", "is_cross_program_prefetch", b"is_cross_program_prefetch", "is_host_transfer", b"is_host_transfer", "is_stable", b"is_stable", "k", b"k", "largest", b"largest", "literal", b"literal", "mantissa_bits", b"mantissa_bits", "metadata", b"metadata", "name", b"name", "opcode", b"opcode", "operand_ids", b"operand_ids", "operand_shapes_with_layout", b"operand_shapes_with_layout", "optional_cross_program_prefetch_index", b"optional_cross_program_prefetch_index", "outfeed_config", b"outfeed_config", "outfeed_shape", b"outfeed_shape", "output_operand_aliasing", b"output_operand_aliasing", "padding_config", b"padding_config", "padding_type", b"padding_type", "parameter_number", b"parameter_number", "parameter_replication", b"parameter_replication", "precision_config", b"precision_config", "replica_groups", b"replica_groups", "rng_algorithm", b"rng_algorithm", "scatter_dimension_numbers", b"scatter_dimension_numbers", "shape", b"shape", "sharding", b"sharding", "slice_dimensions", b"slice_dimensions", "source_target_pairs", b"source_target_pairs", "statistics_viz", b"statistics_viz", "triangular_solve_options", b"triangular_solve_options", "tuple_index", b"tuple_index", "unique_indices", b"unique_indices", "use_global_device_ids", b"use_global_device_ids", "window", b"window"]) -> None: ...
     def WhichOneof(self, oneof_group: typing.Literal["optional_cross_program_prefetch_index", b"optional_cross_program_prefetch_index"]) -> typing.Literal["cross_program_prefetch_index"] | None: ...
 
 global___HloInstructionProto = HloInstructionProto
 
 @typing.final
 class HloComputationProto(google.protobuf.message.Message):
     """Serialization of HloComputation."""
@@ -732,15 +748,15 @@
 
         entry = {
          output_shape_index={1},
          parameter_number=0,
          parameter_shape_index={1, 2},
         }
 
-        This entry indicates that the first paremter's {1, 2} element is
+        This entry indicates that the first parameter's {1, 2} element is
         aliased with the {1} element of the root instruction.
         """
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         OUTPUT_SHAPE_INDEX_FIELD_NUMBER: builtins.int
         PARAMETER_NUMBER_FIELD_NUMBER: builtins.int
@@ -777,80 +793,62 @@
         entries: collections.abc.Iterable[global___HloInputOutputAliasProto.AliasEntryProto] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing.Literal["entries", b"entries"]) -> None: ...
 
 global___HloInputOutputAliasProto = HloInputOutputAliasProto
 
 @typing.final
-class DynamicParameterBindingProto(google.protobuf.message.Message):
+class HloBufferDonorProto(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing.final
-    class Binding(google.protobuf.message.Message):
-        """A list of bindings which indicates that the `target_param_dim_num` in
-        the subshape `target_param_index` of parameter `target_param_num`
-        is a dynamic dimension and its real dynamic size is represented
-        by `dynamic_param_index` in parameter `dynamic_param_num`.
-
-        As an example, imagine we have a program:
-
-        ENTRY main {
-          a = f32[] parameter(0)
-          b = f32[10] parameter(1)
-          ROOT root = (f32[], f32[10]) tuple(%a, %b)
+    class BufferDonorEntryProto(google.protobuf.message.Message):
+        """The following proto describes an input (described by parameter number and a
+        ShapeIndex of the parameter) that can donate its butter to any output
+        tensor. It is similar to HloInputOutputAliasProto, but without a paired
+        output. For example:
+
+        entry = {
+         parameter_number=0,
+         parameter_shape_index={1, 2},
         }
 
-        Let's say 'b' (param index 1) is a dynamic shape whose input has
-        an upperbound of 10 and real size is determined at runtime.'a'
-        represents the real size of b's first dimension.
-
-        In this case, the fields are set in the following way:
-        dynamic_param_num = 1
-        dynamic_param_index = {}
-        target_param_num = 0
-        target_param_index = {}
-        target_param_dim_num = 0
+        This entry indicates that the first parameter's {1, 2} element can donate
+        its buffer.
         """
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-        DYNAMIC_PARAM_NUM_FIELD_NUMBER: builtins.int
-        DYNAMIC_PARAM_INDEX_FIELD_NUMBER: builtins.int
-        TARGET_PARAM_NUM_FIELD_NUMBER: builtins.int
-        TARGET_PARAM_INDEX_FIELD_NUMBER: builtins.int
-        TARGET_PARAM_DIM_NUM_FIELD_NUMBER: builtins.int
-        dynamic_param_num: builtins.int
-        target_param_num: builtins.int
-        target_param_dim_num: builtins.int
-        @property
-        def dynamic_param_index(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
+        PARAMETER_NUMBER_FIELD_NUMBER: builtins.int
+        PARAMETER_SHAPE_INDEX_FIELD_NUMBER: builtins.int
+        parameter_number: builtins.int
+        """Number of the parameter in entry computation."""
         @property
-        def target_param_index(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
+        def parameter_shape_index(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
+            """ShapeIndex of the parameter instruction."""
+
         def __init__(
             self,
             *,
-            dynamic_param_num: builtins.int | None = ...,
-            dynamic_param_index: collections.abc.Iterable[builtins.int] | None = ...,
-            target_param_num: builtins.int | None = ...,
-            target_param_index: collections.abc.Iterable[builtins.int] | None = ...,
-            target_param_dim_num: builtins.int | None = ...,
+            parameter_number: builtins.int | None = ...,
+            parameter_shape_index: collections.abc.Iterable[builtins.int] | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing.Literal["dynamic_param_index", b"dynamic_param_index", "dynamic_param_num", b"dynamic_param_num", "target_param_dim_num", b"target_param_dim_num", "target_param_index", b"target_param_index", "target_param_num", b"target_param_num"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["parameter_number", b"parameter_number", "parameter_shape_index", b"parameter_shape_index"]) -> None: ...
 
     ENTRIES_FIELD_NUMBER: builtins.int
     @property
-    def entries(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DynamicParameterBindingProto.Binding]: ...
+    def entries(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___HloBufferDonorProto.BufferDonorEntryProto]: ...
     def __init__(
         self,
         *,
-        entries: collections.abc.Iterable[global___DynamicParameterBindingProto.Binding] | None = ...,
+        entries: collections.abc.Iterable[global___HloBufferDonorProto.BufferDonorEntryProto] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing.Literal["entries", b"entries"]) -> None: ...
 
-global___DynamicParameterBindingProto = DynamicParameterBindingProto
+global___HloBufferDonorProto = HloBufferDonorProto
 
 @typing.final
 class CrossProgramPrefetch(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMETER_FIELD_NUMBER: builtins.int
     INDEX_FIELD_NUMBER: builtins.int
@@ -867,14 +865,109 @@
         offset: builtins.int | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing.Literal["index", b"index", "offset", b"offset", "parameter", b"parameter"]) -> None: ...
 
 global___CrossProgramPrefetch = CrossProgramPrefetch
 
 @typing.final
+class StackFrameIndexProto(google.protobuf.message.Message):
+    """Serialization of stack frames index representations.
+    Stack frames index presented in four flat arrays:
+    1. File names array.
+    2. Function names array.
+    3. File location array.
+    4. Frame array.
+    All reference ids in sub-protos are 1-based positions of the
+    entity in the flat array.
+    Ids are 1-based to keep 0 value as representation of non-set property.
+    """
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    @typing.final
+    class FileLocation(google.protobuf.message.Message):
+        """Serialization of file position."""
+
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        FILE_NAME_ID_FIELD_NUMBER: builtins.int
+        FUNCTION_NAME_ID_FIELD_NUMBER: builtins.int
+        LINE_FIELD_NUMBER: builtins.int
+        COLUMN_FIELD_NUMBER: builtins.int
+        file_name_id: builtins.int
+        """1-based position of file name."""
+        function_name_id: builtins.int
+        """1-based position of function name."""
+        line: builtins.int
+        """Line number."""
+        column: builtins.int
+        """Column number."""
+        def __init__(
+            self,
+            *,
+            file_name_id: builtins.int | None = ...,
+            function_name_id: builtins.int | None = ...,
+            line: builtins.int | None = ...,
+            column: builtins.int | None = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing.Literal["column", b"column", "file_name_id", b"file_name_id", "function_name_id", b"function_name_id", "line", b"line"]) -> None: ...
+
+    @typing.final
+    class StackFrame(google.protobuf.message.Message):
+        """Serialization of frame."""
+
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        FILE_LOCATION_ID_FIELD_NUMBER: builtins.int
+        PARENT_FRAME_ID_FIELD_NUMBER: builtins.int
+        file_location_id: builtins.int
+        """1-based position of file location."""
+        parent_frame_id: builtins.int
+        """1-based position of the parent frame."""
+        def __init__(
+            self,
+            *,
+            file_location_id: builtins.int | None = ...,
+            parent_frame_id: builtins.int | None = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing.Literal["file_location_id", b"file_location_id", "parent_frame_id", b"parent_frame_id"]) -> None: ...
+
+    FILE_NAMES_FIELD_NUMBER: builtins.int
+    FUNCTION_NAMES_FIELD_NUMBER: builtins.int
+    FILE_LOCATIONS_FIELD_NUMBER: builtins.int
+    STACK_FRAMES_FIELD_NUMBER: builtins.int
+    @property
+    def file_names(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+        """Flat index array of file names."""
+
+    @property
+    def function_names(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+        """Flat index array of function names."""
+
+    @property
+    def file_locations(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___StackFrameIndexProto.FileLocation]:
+        """Flat index array of file locations."""
+
+    @property
+    def stack_frames(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___StackFrameIndexProto.StackFrame]:
+        """Flat index array of frames."""
+
+    def __init__(
+        self,
+        *,
+        file_names: collections.abc.Iterable[builtins.str] | None = ...,
+        function_names: collections.abc.Iterable[builtins.str] | None = ...,
+        file_locations: collections.abc.Iterable[global___StackFrameIndexProto.FileLocation] | None = ...,
+        stack_frames: collections.abc.Iterable[global___StackFrameIndexProto.StackFrame] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing.Literal["file_locations", b"file_locations", "file_names", b"file_names", "function_names", b"function_names", "stack_frames", b"stack_frames"]) -> None: ...
+
+global___StackFrameIndexProto = StackFrameIndexProto
+
+@typing.final
 class HloModuleProto(google.protobuf.message.Message):
     """Serialization of HloModule."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _ProfileType:
         ValueType = typing.NewType("ValueType", builtins.int)
@@ -903,48 +996,54 @@
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         PROFILE_TYPE_FIELD_NUMBER: builtins.int
         RELATIVE_SPEEDUP_FIELD_NUMBER: builtins.int
         PROFILE_SOURCE_FIELD_NUMBER: builtins.int
         COMPILATION_EVENT_FIELD_NUMBER: builtins.int
+        FINGERPRINT_FIELD_NUMBER: builtins.int
         profile_type: global___HloModuleProto.ProfileType.ValueType
         """The optimization profiles that this module contains."""
         relative_speedup: builtins.float
         """Speedup of tuned config compared to default config."""
         profile_source: tensorflow.compiler.xla.xla_data_pb2.ProfileSource.ValueType
         """The source of the optimization profile that this module contains."""
         compilation_event: tensorflow.compiler.xla.xla_data_pb2.CompilationEvent.ValueType
         """The compilation event that triggered the use of the profile."""
+        fingerprint: builtins.str
+        """The fingerprint of the unoptimized module this profile was applied to."""
         def __init__(
             self,
             *,
             profile_type: global___HloModuleProto.ProfileType.ValueType | None = ...,
             relative_speedup: builtins.float | None = ...,
             profile_source: tensorflow.compiler.xla.xla_data_pb2.ProfileSource.ValueType | None = ...,
             compilation_event: tensorflow.compiler.xla.xla_data_pb2.CompilationEvent.ValueType | None = ...,
+            fingerprint: builtins.str | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing.Literal["compilation_event", b"compilation_event", "profile_source", b"profile_source", "profile_type", b"profile_type", "relative_speedup", b"relative_speedup"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["compilation_event", b"compilation_event", "fingerprint", b"fingerprint", "profile_source", b"profile_source", "profile_type", b"profile_type", "relative_speedup", b"relative_speedup"]) -> None: ...
 
     NAME_FIELD_NUMBER: builtins.int
     ENTRY_COMPUTATION_NAME_FIELD_NUMBER: builtins.int
     ENTRY_COMPUTATION_ID_FIELD_NUMBER: builtins.int
     COMPUTATIONS_FIELD_NUMBER: builtins.int
     HOST_PROGRAM_SHAPE_FIELD_NUMBER: builtins.int
     ID_FIELD_NUMBER: builtins.int
     SCHEDULE_FIELD_NUMBER: builtins.int
     INPUT_OUTPUT_ALIAS_FIELD_NUMBER: builtins.int
-    DYNAMIC_PARAMETER_BINDING_FIELD_NUMBER: builtins.int
+    BUFFER_DONOR_FIELD_NUMBER: builtins.int
     CROSS_PROGRAM_PREFETCHES_FIELD_NUMBER: builtins.int
     IS_DYNAMIC_FIELD_NUMBER: builtins.int
     SPMD_OUTPUT_SHARDING_FIELD_NUMBER: builtins.int
     SPMD_PARAMETERS_SHARDINGS_FIELD_NUMBER: builtins.int
     USE_AUTO_SPMD_PARTITIONING_FIELD_NUMBER: builtins.int
     PROFILE_INFO_FIELD_NUMBER: builtins.int
     DEVICE_ASSIGNMENT_FIELD_NUMBER: builtins.int
+    STACK_FRAME_INDEX_FIELD_NUMBER: builtins.int
+    FRONTEND_ATTRIBUTES_FIELD_NUMBER: builtins.int
     name: builtins.str
     entry_computation_name: builtins.str
     entry_computation_id: builtins.int
     id: builtins.int
     """The id of this module."""
     is_dynamic: builtins.bool
     """True if the module contains dynamic computation."""
@@ -965,51 +1064,63 @@
         """The schedule for this module."""
 
     @property
     def input_output_alias(self) -> global___HloInputOutputAliasProto:
         """Describes alias information between inputs and outputs."""
 
     @property
-    def dynamic_parameter_binding(self) -> global___DynamicParameterBindingProto: ...
+    def buffer_donor(self) -> global___HloBufferDonorProto:
+        """Describes the information of input buffer donors."""
+
     @property
     def cross_program_prefetches(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___CrossProgramPrefetch]: ...
     @property
     def spmd_output_sharding(self) -> tensorflow.compiler.xla.xla_data_pb2.OpSharding: ...
     @property
     def spmd_parameters_shardings(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.compiler.xla.xla_data_pb2.OpSharding]: ...
     @property
     def profile_info(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___HloModuleProto.ProfileInfo]:
         """Profile information for the HLO module."""
 
     @property
     def device_assignment(self) -> tensorflow.compiler.xla.xla_data_pb2.DeviceAssignmentProto:
         """DeviceAssignment object information."""
 
+    @property
+    def stack_frame_index(self) -> global___StackFrameIndexProto:
+        """Stack frames index."""
+
+    @property
+    def frontend_attributes(self) -> tensorflow.compiler.xla.xla_data_pb2.FrontendAttributes:
+        """Frontend attributes to pass to the XLA backend."""
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         entry_computation_name: builtins.str | None = ...,
         entry_computation_id: builtins.int | None = ...,
         computations: collections.abc.Iterable[global___HloComputationProto] | None = ...,
         host_program_shape: tensorflow.compiler.xla.xla_data_pb2.ProgramShapeProto | None = ...,
         id: builtins.int | None = ...,
         schedule: global___HloScheduleProto | None = ...,
         input_output_alias: global___HloInputOutputAliasProto | None = ...,
-        dynamic_parameter_binding: global___DynamicParameterBindingProto | None = ...,
+        buffer_donor: global___HloBufferDonorProto | None = ...,
         cross_program_prefetches: collections.abc.Iterable[global___CrossProgramPrefetch] | None = ...,
         is_dynamic: builtins.bool | None = ...,
         spmd_output_sharding: tensorflow.compiler.xla.xla_data_pb2.OpSharding | None = ...,
         spmd_parameters_shardings: collections.abc.Iterable[tensorflow.compiler.xla.xla_data_pb2.OpSharding] | None = ...,
         use_auto_spmd_partitioning: builtins.bool | None = ...,
         profile_info: collections.abc.Iterable[global___HloModuleProto.ProfileInfo] | None = ...,
         device_assignment: tensorflow.compiler.xla.xla_data_pb2.DeviceAssignmentProto | None = ...,
+        stack_frame_index: global___StackFrameIndexProto | None = ...,
+        frontend_attributes: tensorflow.compiler.xla.xla_data_pb2.FrontendAttributes | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing.Literal["device_assignment", b"device_assignment", "dynamic_parameter_binding", b"dynamic_parameter_binding", "host_program_shape", b"host_program_shape", "input_output_alias", b"input_output_alias", "schedule", b"schedule", "spmd_output_sharding", b"spmd_output_sharding"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing.Literal["computations", b"computations", "cross_program_prefetches", b"cross_program_prefetches", "device_assignment", b"device_assignment", "dynamic_parameter_binding", b"dynamic_parameter_binding", "entry_computation_id", b"entry_computation_id", "entry_computation_name", b"entry_computation_name", "host_program_shape", b"host_program_shape", "id", b"id", "input_output_alias", b"input_output_alias", "is_dynamic", b"is_dynamic", "name", b"name", "profile_info", b"profile_info", "schedule", b"schedule", "spmd_output_sharding", b"spmd_output_sharding", "spmd_parameters_shardings", b"spmd_parameters_shardings", "use_auto_spmd_partitioning", b"use_auto_spmd_partitioning"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["buffer_donor", b"buffer_donor", "device_assignment", b"device_assignment", "frontend_attributes", b"frontend_attributes", "host_program_shape", b"host_program_shape", "input_output_alias", b"input_output_alias", "schedule", b"schedule", "spmd_output_sharding", b"spmd_output_sharding", "stack_frame_index", b"stack_frame_index"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["buffer_donor", b"buffer_donor", "computations", b"computations", "cross_program_prefetches", b"cross_program_prefetches", "device_assignment", b"device_assignment", "entry_computation_id", b"entry_computation_id", "entry_computation_name", b"entry_computation_name", "frontend_attributes", b"frontend_attributes", "host_program_shape", b"host_program_shape", "id", b"id", "input_output_alias", b"input_output_alias", "is_dynamic", b"is_dynamic", "name", b"name", "profile_info", b"profile_info", "schedule", b"schedule", "spmd_output_sharding", b"spmd_output_sharding", "spmd_parameters_shardings", b"spmd_parameters_shardings", "stack_frame_index", b"stack_frame_index", "use_auto_spmd_partitioning", b"use_auto_spmd_partitioning"]) -> None: ...
 
 global___HloModuleProto = HloModuleProto
 
 @typing.final
 class LogicalBufferProto(google.protobuf.message.Message):
     """Serialization of LogicalBuffer."""
 
@@ -1431,14 +1542,15 @@
     PIPELINE_NAME_FIELD_NUMBER: builtins.int
     DUMP_FILENAMES_FIELD_NUMBER: builtins.int
     MODULE_CHANGED_FIELD_NUMBER: builtins.int
     MODULE_ID_FIELD_NUMBER: builtins.int
     MODULE_GROUP_MODULE_IDS_FIELD_NUMBER: builtins.int
     START_TIMESTAMP_USEC_FIELD_NUMBER: builtins.int
     END_TIMESTAMP_USEC_FIELD_NUMBER: builtins.int
+    CUSTOM_METADATA_FIELD_NUMBER: builtins.int
     pass_id: builtins.int
     """For a given module, pass_id uniquely identifies a run of an HLO pass on
     that module. Note that a pass_id may not always refer to the same pass
     because the order of passes during compilation may change. For finding
     metadata for a particular pass, pass_name and pipeline_name would be more
     reliable, although note that they may not be unique.
     """
@@ -1466,113 +1578,38 @@
 
     @property
     def module_group_module_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """If the module went through this pass as part of a module group, this is
         set as the ids of all the modules in the module group. Empty otherwise.
         """
 
+    @property
+    def custom_metadata(self) -> google.protobuf.any_pb2.Any:
+        """Custom metadata for the pass."""
+
     def __init__(
         self,
         *,
         pass_id: builtins.int | None = ...,
         pass_name: builtins.str | None = ...,
         pipeline_name: builtins.str | None = ...,
         dump_filenames: collections.abc.Iterable[builtins.str] | None = ...,
         module_changed: builtins.bool | None = ...,
         module_id: builtins.int | None = ...,
         module_group_module_ids: collections.abc.Iterable[builtins.int] | None = ...,
         start_timestamp_usec: builtins.int | None = ...,
         end_timestamp_usec: builtins.int | None = ...,
+        custom_metadata: google.protobuf.any_pb2.Any | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing.Literal["dump_filenames", b"dump_filenames", "end_timestamp_usec", b"end_timestamp_usec", "module_changed", b"module_changed", "module_group_module_ids", b"module_group_module_ids", "module_id", b"module_id", "pass_id", b"pass_id", "pass_name", b"pass_name", "pipeline_name", b"pipeline_name", "start_timestamp_usec", b"start_timestamp_usec"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["custom_metadata", b"custom_metadata"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["custom_metadata", b"custom_metadata", "dump_filenames", b"dump_filenames", "end_timestamp_usec", b"end_timestamp_usec", "module_changed", b"module_changed", "module_group_module_ids", b"module_group_module_ids", "module_id", b"module_id", "pass_id", b"pass_id", "pass_name", b"pass_name", "pipeline_name", b"pipeline_name", "start_timestamp_usec", b"start_timestamp_usec"]) -> None: ...
 
 global___HloPassMetadata = HloPassMetadata
 
 @typing.final
-class EntryFunctionAttributes(google.protobuf.message.Message):
-    """Encodes attributes for an entry function."""
-
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    @typing.final
-    class ShapeIndex(google.protobuf.message.Message):
-        """Acts as the underlying container for an xla::ShapeIndex."""
-
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-        INDICES_FIELD_NUMBER: builtins.int
-        @property
-        def indices(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
-        def __init__(
-            self,
-            *,
-            indices: collections.abc.Iterable[builtins.int] | None = ...,
-        ) -> None: ...
-        def ClearField(self, field_name: typing.Literal["indices", b"indices"]) -> None: ...
-
-    @typing.final
-    class BufferParameterAttributes(google.protobuf.message.Message):
-        """Encodes attributes for a single buffer parameter."""
-
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-        LMHLO_PARAMS_FIELD_NUMBER: builtins.int
-        LMHLO_PARAMS_PRESENT_FIELD_NUMBER: builtins.int
-        LMHLO_PARAM_SHAPE_INDEX_FIELD_NUMBER: builtins.int
-        LMHLO_CONSTANT_NAME_FIELD_NUMBER: builtins.int
-        LMHLO_MUST_ALIAS_FIELD_NUMBER: builtins.int
-        LMHLO_OUTPUT_INDEX_FIELD_NUMBER: builtins.int
-        lmhlo_params: builtins.int
-        """Represents an lmhlo.params function argument attribute."""
-        lmhlo_params_present: builtins.bool
-        """TODO(hanbinyoon): Deprecate when optional fields are available in proto3
-        (Protocol Buffers v3.15.0).
-        """
-        lmhlo_constant_name: builtins.str
-        """Represents an lmhlo.constant_name function argument attribute."""
-        lmhlo_must_alias: builtins.bool
-        """Represents an lmhlo.must_alias function argument attribute."""
-        @property
-        def lmhlo_param_shape_index(self) -> global___EntryFunctionAttributes.ShapeIndex:
-            """Represents an lmhlo.param_shape_index function argument attribute."""
-
-        @property
-        def lmhlo_output_index(self) -> global___EntryFunctionAttributes.ShapeIndex:
-            """Represents an lmhlo.params function argument attribute."""
-
-        def __init__(
-            self,
-            *,
-            lmhlo_params: builtins.int | None = ...,
-            lmhlo_params_present: builtins.bool | None = ...,
-            lmhlo_param_shape_index: global___EntryFunctionAttributes.ShapeIndex | None = ...,
-            lmhlo_constant_name: builtins.str | None = ...,
-            lmhlo_must_alias: builtins.bool | None = ...,
-            lmhlo_output_index: global___EntryFunctionAttributes.ShapeIndex | None = ...,
-        ) -> None: ...
-        def HasField(self, field_name: typing.Literal["lmhlo_output_index", b"lmhlo_output_index", "lmhlo_param_shape_index", b"lmhlo_param_shape_index"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing.Literal["lmhlo_constant_name", b"lmhlo_constant_name", "lmhlo_must_alias", b"lmhlo_must_alias", "lmhlo_output_index", b"lmhlo_output_index", "lmhlo_param_shape_index", b"lmhlo_param_shape_index", "lmhlo_params", b"lmhlo_params", "lmhlo_params_present", b"lmhlo_params_present"]) -> None: ...
-
-    BUFFERS_FIELD_NUMBER: builtins.int
-    RESULT_XLA_SHAPE_FIELD_NUMBER: builtins.int
-    result_xla_shape: builtins.str
-    """xla::Shape in string format."""
-    @property
-    def buffers(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___EntryFunctionAttributes.BufferParameterAttributes]: ...
-    def __init__(
-        self,
-        *,
-        buffers: collections.abc.Iterable[global___EntryFunctionAttributes.BufferParameterAttributes] | None = ...,
-        result_xla_shape: builtins.str | None = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing.Literal["buffers", b"buffers", "result_xla_shape", b"result_xla_shape"]) -> None: ...
-
-global___EntryFunctionAttributes = EntryFunctionAttributes
-
-@typing.final
 class XlaRuntimeExecutableProto(google.protobuf.message.Message):
     """Encodes the underlying Xla runtime executable compiled from the XLA module."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HLO_MODULE_PROTO_FIELD_NUMBER: builtins.int
     OBJ_FILE_FIELD_NUMBER: builtins.int
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
-Copyright 2017 The TensorFlow Authors. All Rights Reserved.
+Copyright 2017 The OpenXLA Authors.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
 http://www.apache.org/licenses/LICENSE-2.0
 
@@ -40,21 +40,23 @@
 
 class _PrimitiveTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_PrimitiveType.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     PRIMITIVE_TYPE_INVALID: _PrimitiveType.ValueType  # 0
     """Invalid primitive type to serve as default."""
     PRED: _PrimitiveType.ValueType  # 1
     """Predicates are two-state booleans."""
-    S8: _PrimitiveType.ValueType  # 2
+    S4: _PrimitiveType.ValueType  # 21
     """Signed integral values of fixed width."""
+    S8: _PrimitiveType.ValueType  # 2
     S16: _PrimitiveType.ValueType  # 3
     S32: _PrimitiveType.ValueType  # 4
     S64: _PrimitiveType.ValueType  # 5
-    U8: _PrimitiveType.ValueType  # 6
+    U4: _PrimitiveType.ValueType  # 22
     """Unsigned integral values of fixed width."""
+    U8: _PrimitiveType.ValueType  # 6
     U16: _PrimitiveType.ValueType  # 7
     U32: _PrimitiveType.ValueType  # 8
     U64: _PrimitiveType.ValueType  # 9
     F16: _PrimitiveType.ValueType  # 10
     """Floating-point values of fixed width.
 
     Note: if f16s are not natively supported on the device, they will be
@@ -74,19 +76,43 @@
     existing IEEE types.
 
     F8E4M3FN has 4 exponent bits and 3 mantissa bits. The "FN" means only
     Finite and NaN values are supported. Unlike IEEE types, infinities are not
     supported.  NaN is represented when the exponent and mantissa bits are all
     1s. All other values are finite.
 
+    F8E4M3B11FNUZ has 4 exponent bits and 3 mantissa bits and a bias of 11. The
+    "FNUZ" means only Finite and NaN values are supported; zero is unsigned.
+    Unlike IEEE types, infinities are not supported.  NaN is represented when
+    the exponent and mantissa bits are all 0s with a sign bit of 1. All other
+    values are finite.
+
     Support for these dtypes is under development. They do not yet work
     properly in most cases.
     TODO(b/259609697): Fully support FP8.
     """
     F8E4M3FN: _PrimitiveType.ValueType  # 20
+    F8E4M3B11FNUZ: _PrimitiveType.ValueType  # 23
+    F8E5M2FNUZ: _PrimitiveType.ValueType  # 24
+    """FP8 dtypes, as described in this paper: https://arxiv.org/abs/2206.02915
+
+    F8E5M2FNUZ has 5 exponent bits and 2 mantissa bits.
+    F8E4M3FNUZ has 4 exponent bits and 3 mantissa bits.
+
+    The "FNUZ" means only Finite and NaN values are supported; zero is
+    unsigned. Unlike IEEE types, infinities are not supported.  NaN is
+    represented when the exponent and mantissa bits are all 0s with a sign bit
+    of 1. All other values are finite.
+
+    These differences mean there's an additional exponent value available. To
+    keep the same dynamic range as an IEEE-like FP8 type, the exponent is
+    biased one more than would be expected given the number of exponent bits
+    (8 for Float8E4M3FNUZ and 16 for Float8E5M2FNUZ).
+    """
+    F8E4M3FNUZ: _PrimitiveType.ValueType  # 25
     C64: _PrimitiveType.ValueType  # 15
     """Complex values of fixed width.
     Paired F32 (real, imag), as in std::complex<float>.
     """
     C128: _PrimitiveType.ValueType  # 18
     """Paired F64 (real, imag), as in std::complex<double>."""
     TUPLE: _PrimitiveType.ValueType  # 13
@@ -119,21 +145,23 @@
     LINT.IfChange
     """
 
 PRIMITIVE_TYPE_INVALID: PrimitiveType.ValueType  # 0
 """Invalid primitive type to serve as default."""
 PRED: PrimitiveType.ValueType  # 1
 """Predicates are two-state booleans."""
-S8: PrimitiveType.ValueType  # 2
+S4: PrimitiveType.ValueType  # 21
 """Signed integral values of fixed width."""
+S8: PrimitiveType.ValueType  # 2
 S16: PrimitiveType.ValueType  # 3
 S32: PrimitiveType.ValueType  # 4
 S64: PrimitiveType.ValueType  # 5
-U8: PrimitiveType.ValueType  # 6
+U4: PrimitiveType.ValueType  # 22
 """Unsigned integral values of fixed width."""
+U8: PrimitiveType.ValueType  # 6
 U16: PrimitiveType.ValueType  # 7
 U32: PrimitiveType.ValueType  # 8
 U64: PrimitiveType.ValueType  # 9
 F16: PrimitiveType.ValueType  # 10
 """Floating-point values of fixed width.
 
 Note: if f16s are not natively supported on the device, they will be
@@ -153,19 +181,43 @@
 existing IEEE types.
 
 F8E4M3FN has 4 exponent bits and 3 mantissa bits. The "FN" means only
 Finite and NaN values are supported. Unlike IEEE types, infinities are not
 supported.  NaN is represented when the exponent and mantissa bits are all
 1s. All other values are finite.
 
+F8E4M3B11FNUZ has 4 exponent bits and 3 mantissa bits and a bias of 11. The
+"FNUZ" means only Finite and NaN values are supported; zero is unsigned.
+Unlike IEEE types, infinities are not supported.  NaN is represented when
+the exponent and mantissa bits are all 0s with a sign bit of 1. All other
+values are finite.
+
 Support for these dtypes is under development. They do not yet work
 properly in most cases.
 TODO(b/259609697): Fully support FP8.
 """
 F8E4M3FN: PrimitiveType.ValueType  # 20
+F8E4M3B11FNUZ: PrimitiveType.ValueType  # 23
+F8E5M2FNUZ: PrimitiveType.ValueType  # 24
+"""FP8 dtypes, as described in this paper: https://arxiv.org/abs/2206.02915
+
+F8E5M2FNUZ has 5 exponent bits and 2 mantissa bits.
+F8E4M3FNUZ has 4 exponent bits and 3 mantissa bits.
+
+The "FNUZ" means only Finite and NaN values are supported; zero is
+unsigned. Unlike IEEE types, infinities are not supported.  NaN is
+represented when the exponent and mantissa bits are all 0s with a sign bit
+of 1. All other values are finite.
+
+These differences mean there's an additional exponent value available. To
+keep the same dynamic range as an IEEE-like FP8 type, the exponent is
+biased one more than would be expected given the number of exponent bits
+(8 for Float8E4M3FNUZ and 16 for Float8E5M2FNUZ).
+"""
+F8E4M3FNUZ: PrimitiveType.ValueType  # 25
 C64: PrimitiveType.ValueType  # 15
 """Complex values of fixed width.
 Paired F32 (real, imag), as in std::complex<float>.
 """
 C128: PrimitiveType.ValueType  # 18
 """Paired F64 (real, imag), as in std::complex<double>."""
 TUPLE: PrimitiveType.ValueType  # 13
@@ -201,14 +253,19 @@
     """The corresponding dimension is Dense, every entry is stored."""
     DIM_COMPRESSED: _DimLevelType.ValueType  # 1
     """The corresponding dimension is Compressed, only nonzeros are stored."""
     DIM_SINGLETON: _DimLevelType.ValueType  # 2
     """The corresponding dimension contains a single coordinate, no sibling
     elements for each parent.
     """
+    DIM_LOOSE_COMPRESSED: _DimLevelType.ValueType  # 3
+    """The corresponding dimension is Compressed, but with potential trailing
+    zeros, thus an extra upper bound (high) is used to exclude those zeros.
+    E.g., indices = [1, 2, 0, 0, 3, 4, 0, 0], position = [(0, 2), (4, 6)].
+    """
 
 class DimLevelType(_DimLevelType, metaclass=_DimLevelTypeEnumTypeWrapper):
     """A DimLevelType indicates the encoding method for a dimension in an array.
     The semantics of this field are identical to those of the MLIR SparseTensor
     dialect.
     This should be kept in sync with the SparseTensor DimLevelType enum:
     https://github.com/llvm/llvm-project/blob/5674a3c88088e668b684326c2194a6282e8270ff/mlir/include/mlir/Dialect/SparseTensor/IR/SparseTensorAttrDefs.td#L86
@@ -218,14 +275,19 @@
 """The corresponding dimension is Dense, every entry is stored."""
 DIM_COMPRESSED: DimLevelType.ValueType  # 1
 """The corresponding dimension is Compressed, only nonzeros are stored."""
 DIM_SINGLETON: DimLevelType.ValueType  # 2
 """The corresponding dimension contains a single coordinate, no sibling
 elements for each parent.
 """
+DIM_LOOSE_COMPRESSED: DimLevelType.ValueType  # 3
+"""The corresponding dimension is Compressed, but with potential trailing
+zeros, thus an extra upper bound (high) is used to exclude those zeros.
+E.g., indices = [1, 2, 0, 0, 3, 4, 0, 0], position = [(0, 2), (4, 6)].
+"""
 global___DimLevelType = DimLevelType
 
 class _ProfileType:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
 class _ProfileTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ProfileType.ValueType], builtins.type):
@@ -324,14 +386,31 @@
 """Inverse FFT; complex in, complex out."""
 RFFT: FftType.ValueType  # 2
 """Forward real FFT; real in, fft_length / 2 + 1 complex out"""
 IRFFT: FftType.ValueType  # 3
 """Inverse real FFT; fft_length / 2 + 1 complex in,"""
 global___FftType = FftType
 
+class _SparsityType:
+    ValueType = typing.NewType("ValueType", builtins.int)
+    V: typing_extensions.TypeAlias = ValueType
+
+class _SparsityTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_SparsityType.ValueType], builtins.type):
+    DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+    SPARSITY_INVALID: _SparsityType.ValueType  # 0
+    SPARSITY_STRUCTURED_N_M: _SparsityType.ValueType  # 1
+    """Structured N:M sparsity."""
+
+class SparsityType(_SparsityType, metaclass=_SparsityTypeEnumTypeWrapper): ...
+
+SPARSITY_INVALID: SparsityType.ValueType  # 0
+SPARSITY_STRUCTURED_N_M: SparsityType.ValueType  # 1
+"""Structured N:M sparsity."""
+global___SparsityType = SparsityType
+
 class _RandomDistribution:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
 class _RandomDistributionEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_RandomDistribution.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     RNG_INVALID: _RandomDistribution.ValueType  # 0
@@ -470,19 +549,34 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DIM_LEVEL_TYPES_FIELD_NUMBER: builtins.int
     DIM_UNIQUE_FIELD_NUMBER: builtins.int
     DIM_ORDERED_FIELD_NUMBER: builtins.int
     MINOR_TO_MAJOR_FIELD_NUMBER: builtins.int
     TILES_FIELD_NUMBER: builtins.int
+    TAIL_PADDING_ALIGNMENT_IN_ELEMENTS_FIELD_NUMBER: builtins.int
+    ELEMENT_SIZE_IN_BITS_FIELD_NUMBER: builtins.int
     MEMORY_SPACE_FIELD_NUMBER: builtins.int
     INDEX_PRIMITIVE_TYPE_FIELD_NUMBER: builtins.int
     POINTER_PRIMITIVE_TYPE_FIELD_NUMBER: builtins.int
     PHYSICAL_SHAPE_FIELD_NUMBER: builtins.int
     DYNAMIC_SHAPE_METADATA_PREFIX_BYTES_FIELD_NUMBER: builtins.int
+    tail_padding_alignment_in_elements: builtins.int
+    """The shape is padded at the end to multiple of, in terms of number of
+    elements. This is useful when tiling does not bring the shape to certain
+    desired granules. Tiling effectively pads/reshapes/transposes the shape
+    to another shape. This field pads the total number of elements of that
+    new shape to a multiple of certain number of elements. This is useful such
+    as we want a layout which does not tile the data but still requires it to
+    be padded to certain number of elements.
+    """
+    element_size_in_bits: builtins.int
+    """(Optional) Bit size of each element. When unspecified or being 0, default
+    to ShapeUtil::ByteSizeOfPrimitiveType.
+    """
     memory_space: builtins.int
     """Memory space where this array resides. The integer field is interpreted in
     a backend-specific manner.
     """
     index_primitive_type: global___PrimitiveType.ValueType
     """The integer types to be used for indices and pointers.  These fields must
     not be used unless the layout represents a sparse array.  The PrimitiveType
@@ -542,22 +636,24 @@
         self,
         *,
         dim_level_types: collections.abc.Iterable[global___DimLevelType.ValueType] | None = ...,
         dim_unique: collections.abc.Iterable[builtins.bool] | None = ...,
         dim_ordered: collections.abc.Iterable[builtins.bool] | None = ...,
         minor_to_major: collections.abc.Iterable[builtins.int] | None = ...,
         tiles: collections.abc.Iterable[global___TileProto] | None = ...,
+        tail_padding_alignment_in_elements: builtins.int | None = ...,
+        element_size_in_bits: builtins.int | None = ...,
         memory_space: builtins.int | None = ...,
         index_primitive_type: global___PrimitiveType.ValueType | None = ...,
         pointer_primitive_type: global___PrimitiveType.ValueType | None = ...,
         physical_shape: global___ShapeProto | None = ...,
         dynamic_shape_metadata_prefix_bytes: builtins.int | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing.Literal["physical_shape", b"physical_shape"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing.Literal["dim_level_types", b"dim_level_types", "dim_ordered", b"dim_ordered", "dim_unique", b"dim_unique", "dynamic_shape_metadata_prefix_bytes", b"dynamic_shape_metadata_prefix_bytes", "index_primitive_type", b"index_primitive_type", "memory_space", b"memory_space", "minor_to_major", b"minor_to_major", "physical_shape", b"physical_shape", "pointer_primitive_type", b"pointer_primitive_type", "tiles", b"tiles"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["dim_level_types", b"dim_level_types", "dim_ordered", b"dim_ordered", "dim_unique", b"dim_unique", "dynamic_shape_metadata_prefix_bytes", b"dynamic_shape_metadata_prefix_bytes", "element_size_in_bits", b"element_size_in_bits", "index_primitive_type", b"index_primitive_type", "memory_space", b"memory_space", "minor_to_major", b"minor_to_major", "physical_shape", b"physical_shape", "pointer_primitive_type", b"pointer_primitive_type", "tail_padding_alignment_in_elements", b"tail_padding_alignment_in_elements", "tiles", b"tiles"]) -> None: ...
 
 global___LayoutProto = LayoutProto
 
 @typing.final
 class ShapeProto(google.protobuf.message.Message):
     """A shape describes the number of dimensions in the array, the size of each
     dimension, and the primitive component type.
@@ -720,14 +816,17 @@
     SOURCE_LINE_FIELD_NUMBER: builtins.int
     PROFILE_TYPE_FIELD_NUMBER: builtins.int
     CREATION_PASS_ID_FIELD_NUMBER: builtins.int
     LOGICAL_CREATION_PASS_ID_FIELD_NUMBER: builtins.int
     SIZE_OF_GENERATED_CODE_IN_BYTES_FIELD_NUMBER: builtins.int
     SIZE_OF_MEMORY_WORKING_SET_IN_BYTES_FIELD_NUMBER: builtins.int
     PROFILE_INFO_FIELD_NUMBER: builtins.int
+    DEDUPLICATED_NAME_FIELD_NUMBER: builtins.int
+    PRESERVE_LAYOUT_FIELD_NUMBER: builtins.int
+    STACK_FRAME_ID_FIELD_NUMBER: builtins.int
     op_type: builtins.str
     """The framework op name that generated this XLA op.
 
     Frameworks that build on top of XLA should mirror the names of their ops
     back to users by specifying the op_type. In this way, even if the
     framework's "ops" are implemented as multiple XLA HLO Ops, they can be
     grouped appropriately. (e.g. if a SoftMax layer is emitted into XLA as
@@ -758,14 +857,28 @@
     """
     size_of_generated_code_in_bytes: builtins.int
     """The footprint of the generated code for the instruction."""
     size_of_memory_working_set_in_bytes: builtins.int
     """The size of the working set, i.e., the amount of memory, used by the
     instruction in a compiler-managed fast device memory.
     """
+    deduplicated_name: builtins.str
+    """Deduplicated HLO name for this op. In some cases, we can have multiple
+    instructions (e.g. fusions) that are considered duplicates. We want to
+    group them together under the same name so that we can group them together
+    during analysis (e.g. HLO Op Profile tool in Xprof).
+    E.g. If we have fusion.1, fusion.2, and fusion.3 marked as duplicates,
+    fusion.2 and fusion.3 will have deduplicated_name = fusion.1
+    """
+    preserve_layout: builtins.bool
+    """Whether to preserve the layout of the HLO op."""
+    stack_frame_id: builtins.int
+    """1-based position of the frame in frames flat array.
+    Ids are 1-based to keep 0 value as representation of non-set property.
+    """
     @property
     def profile_type(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[global___ProfileType.ValueType]:
         """Deprecated, use [ProfileInfo][profile_type] instead."""
 
     @property
     def profile_info(self) -> global___OpMetadata.ProfileInfo:
         """Profile information for the Op."""
@@ -779,17 +892,20 @@
         source_line: builtins.int | None = ...,
         profile_type: collections.abc.Iterable[global___ProfileType.ValueType] | None = ...,
         creation_pass_id: builtins.int | None = ...,
         logical_creation_pass_id: builtins.int | None = ...,
         size_of_generated_code_in_bytes: builtins.int | None = ...,
         size_of_memory_working_set_in_bytes: builtins.int | None = ...,
         profile_info: global___OpMetadata.ProfileInfo | None = ...,
+        deduplicated_name: builtins.str | None = ...,
+        preserve_layout: builtins.bool | None = ...,
+        stack_frame_id: builtins.int | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing.Literal["profile_info", b"profile_info"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing.Literal["creation_pass_id", b"creation_pass_id", "logical_creation_pass_id", b"logical_creation_pass_id", "op_name", b"op_name", "op_type", b"op_type", "profile_info", b"profile_info", "profile_type", b"profile_type", "size_of_generated_code_in_bytes", b"size_of_generated_code_in_bytes", "size_of_memory_working_set_in_bytes", b"size_of_memory_working_set_in_bytes", "source_file", b"source_file", "source_line", b"source_line"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["creation_pass_id", b"creation_pass_id", "deduplicated_name", b"deduplicated_name", "logical_creation_pass_id", b"logical_creation_pass_id", "op_name", b"op_name", "op_type", b"op_type", "preserve_layout", b"preserve_layout", "profile_info", b"profile_info", "profile_type", b"profile_type", "size_of_generated_code_in_bytes", b"size_of_generated_code_in_bytes", "size_of_memory_working_set_in_bytes", b"size_of_memory_working_set_in_bytes", "source_file", b"source_file", "source_line", b"source_line", "stack_frame_id", b"stack_frame_id"]) -> None: ...
 
 global___OpMetadata = OpMetadata
 
 @typing.final
 class ExecutionProfile(google.protobuf.message.Message):
     """Profile data from the execution of a computation."""
 
@@ -1019,14 +1135,16 @@
     of the repeated fields is implied by the shape.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SHAPE_FIELD_NUMBER: builtins.int
     PREDS_FIELD_NUMBER: builtins.int
+    S4S_FIELD_NUMBER: builtins.int
+    U4S_FIELD_NUMBER: builtins.int
     S8S_FIELD_NUMBER: builtins.int
     U8S_FIELD_NUMBER: builtins.int
     S32S_FIELD_NUMBER: builtins.int
     S64S_FIELD_NUMBER: builtins.int
     U32S_FIELD_NUMBER: builtins.int
     U64S_FIELD_NUMBER: builtins.int
     F32S_FIELD_NUMBER: builtins.int
@@ -1036,24 +1154,32 @@
     TUPLE_LITERALS_FIELD_NUMBER: builtins.int
     F16S_FIELD_NUMBER: builtins.int
     BF16S_FIELD_NUMBER: builtins.int
     U16S_FIELD_NUMBER: builtins.int
     S16S_FIELD_NUMBER: builtins.int
     F8E5M2S_FIELD_NUMBER: builtins.int
     F8E4M3FNS_FIELD_NUMBER: builtins.int
+    F8E4M3B11FNUZS_FIELD_NUMBER: builtins.int
+    F8E5M2FNUZS_FIELD_NUMBER: builtins.int
+    F8E4M3FNUZS_FIELD_NUMBER: builtins.int
     SPARSE_INDICES_FIELD_NUMBER: builtins.int
+    s4s: builtins.bytes
+    u4s: builtins.bytes
     s8s: builtins.bytes
     u8s: builtins.bytes
     f16s: builtins.bytes
     """The F16s, BF16s, U16s and S16s are encoded in little endian byte order"""
     bf16s: builtins.bytes
     u16s: builtins.bytes
     s16s: builtins.bytes
     f8e5m2s: builtins.bytes
     f8e4m3fns: builtins.bytes
+    f8e4m3b11fnuzs: builtins.bytes
+    f8e5m2fnuzs: builtins.bytes
+    f8e4m3fnuzs: builtins.bytes
     @property
     def shape(self) -> global___ShapeProto: ...
     @property
     def preds(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.bool]: ...
     @property
     def s32s(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     @property
@@ -1074,21 +1200,23 @@
     def c128s(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]:
         """Stored as interleaved real, imag doubles."""
 
     @property
     def tuple_literals(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___LiteralProto]: ...
     @property
     def sparse_indices(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
-        """Next = 21"""
+        """Next = 26"""
 
     def __init__(
         self,
         *,
         shape: global___ShapeProto | None = ...,
         preds: collections.abc.Iterable[builtins.bool] | None = ...,
+        s4s: builtins.bytes | None = ...,
+        u4s: builtins.bytes | None = ...,
         s8s: builtins.bytes | None = ...,
         u8s: builtins.bytes | None = ...,
         s32s: collections.abc.Iterable[builtins.int] | None = ...,
         s64s: collections.abc.Iterable[builtins.int] | None = ...,
         u32s: collections.abc.Iterable[builtins.int] | None = ...,
         u64s: collections.abc.Iterable[builtins.int] | None = ...,
         f32s: collections.abc.Iterable[builtins.float] | None = ...,
@@ -1098,18 +1226,21 @@
         tuple_literals: collections.abc.Iterable[global___LiteralProto] | None = ...,
         f16s: builtins.bytes | None = ...,
         bf16s: builtins.bytes | None = ...,
         u16s: builtins.bytes | None = ...,
         s16s: builtins.bytes | None = ...,
         f8e5m2s: builtins.bytes | None = ...,
         f8e4m3fns: builtins.bytes | None = ...,
+        f8e4m3b11fnuzs: builtins.bytes | None = ...,
+        f8e5m2fnuzs: builtins.bytes | None = ...,
+        f8e4m3fnuzs: builtins.bytes | None = ...,
         sparse_indices: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing.Literal["shape", b"shape"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing.Literal["bf16s", b"bf16s", "c128s", b"c128s", "c64s", b"c64s", "f16s", b"f16s", "f32s", b"f32s", "f64s", b"f64s", "f8e4m3fns", b"f8e4m3fns", "f8e5m2s", b"f8e5m2s", "preds", b"preds", "s16s", b"s16s", "s32s", b"s32s", "s64s", b"s64s", "s8s", b"s8s", "shape", b"shape", "sparse_indices", b"sparse_indices", "tuple_literals", b"tuple_literals", "u16s", b"u16s", "u32s", b"u32s", "u64s", b"u64s", "u8s", b"u8s"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["bf16s", b"bf16s", "c128s", b"c128s", "c64s", b"c64s", "f16s", b"f16s", "f32s", b"f32s", "f64s", b"f64s", "f8e4m3b11fnuzs", b"f8e4m3b11fnuzs", "f8e4m3fns", b"f8e4m3fns", "f8e4m3fnuzs", b"f8e4m3fnuzs", "f8e5m2fnuzs", b"f8e5m2fnuzs", "f8e5m2s", b"f8e5m2s", "preds", b"preds", "s16s", b"s16s", "s32s", b"s32s", "s4s", b"s4s", "s64s", b"s64s", "s8s", b"s8s", "shape", b"shape", "sparse_indices", b"sparse_indices", "tuple_literals", b"tuple_literals", "u16s", b"u16s", "u32s", b"u32s", "u4s", b"u4s", "u64s", b"u64s", "u8s", b"u8s"]) -> None: ...
 
 global___LiteralProto = LiteralProto
 
 @typing.final
 class WindowDimension(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -1389,14 +1520,52 @@
         rhs_batch_dimensions: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing.Literal["lhs_batch_dimensions", b"lhs_batch_dimensions", "lhs_contracting_dimensions", b"lhs_contracting_dimensions", "rhs_batch_dimensions", b"rhs_batch_dimensions", "rhs_contracting_dimensions", b"rhs_contracting_dimensions"]) -> None: ...
 
 global___DotDimensionNumbers = DotDimensionNumbers
 
 @typing.final
+class SparsityDescriptor(google.protobuf.message.Message):
+    """Contains sparsity metadata for a sparse dot operation.
+    The only supported type atm is structured 2:4 sparsity, which is natively
+    supported on NVidia GPUs.
+    Restrictions:
+    - only one operand of the dot operation may be sparse;
+    - only the contracting dimension may be sparse.
+    """
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    TYPE_FIELD_NUMBER: builtins.int
+    INDEX_FIELD_NUMBER: builtins.int
+    DIMENSION_FIELD_NUMBER: builtins.int
+    N_FIELD_NUMBER: builtins.int
+    M_FIELD_NUMBER: builtins.int
+    type: global___SparsityType.ValueType
+    index: builtins.int
+    """Sparse operand index (0 or 1)."""
+    dimension: builtins.int
+    """Sparse dimension number."""
+    n: builtins.int
+    """Structured N:M sparsity (N < M)."""
+    m: builtins.int
+    def __init__(
+        self,
+        *,
+        type: global___SparsityType.ValueType | None = ...,
+        index: builtins.int | None = ...,
+        dimension: builtins.int | None = ...,
+        n: builtins.int | None = ...,
+        m: builtins.int | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing.Literal["dimension", b"dimension", "index", b"index", "m", b"m", "n", b"n", "type", b"type"]) -> None: ...
+
+global___SparsityDescriptor = SparsityDescriptor
+
+@typing.final
 class TriangularSolveOptions(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _Transpose:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
@@ -1459,14 +1628,31 @@
         lower: builtins.bool | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing.Literal["lower", b"lower"]) -> None: ...
 
 global___CholeskyOptions = CholeskyOptions
 
 @typing.final
+class SortOptions(google.protobuf.message.Message):
+    """Attributes of the sort custom call (cub::DeviceRadixSort)."""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    DESCENDING_FIELD_NUMBER: builtins.int
+    descending: builtins.bool
+    def __init__(
+        self,
+        *,
+        descending: builtins.bool | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing.Literal["descending", b"descending"]) -> None: ...
+
+global___SortOptions = SortOptions
+
+@typing.final
 class FrontendAttributes(google.protobuf.message.Message):
     """Generic map of attributes used to pass hints / configuration options from
     the Python frontend to the XLA backend.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -1495,14 +1681,62 @@
         map: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing.Literal["map", b"map"]) -> None: ...
 
 global___FrontendAttributes = FrontendAttributes
 
 @typing.final
+class Statistic(google.protobuf.message.Message):
+    """Represents a single statistic to track."""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    STAT_NAME_FIELD_NUMBER: builtins.int
+    STAT_VAL_FIELD_NUMBER: builtins.int
+    stat_name: builtins.str
+    """Must be a single word consisting of any alphanumeric characters"""
+    stat_val: builtins.float
+    """Must be within a range of [0, 100], in order for the graph dumper to
+    properly render the statistic onto the graph.
+    """
+    def __init__(
+        self,
+        *,
+        stat_name: builtins.str | None = ...,
+        stat_val: builtins.float | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing.Literal["stat_name", b"stat_name", "stat_val", b"stat_val"]) -> None: ...
+
+global___Statistic = Statistic
+
+@typing.final
+class StatisticsViz(google.protobuf.message.Message):
+    """Represents the information needed to visualize propagation statistics when
+    rendering an HLO graph. This includes an array of statistics as well as the
+    index of the statistic to render.
+    """
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    STAT_INDEX_TO_VISUALIZE_FIELD_NUMBER: builtins.int
+    STATISTICS_FIELD_NUMBER: builtins.int
+    stat_index_to_visualize: builtins.int
+    @property
+    def statistics(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Statistic]: ...
+    def __init__(
+        self,
+        *,
+        stat_index_to_visualize: builtins.int | None = ...,
+        statistics: collections.abc.Iterable[global___Statistic] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing.Literal["stat_index_to_visualize", b"stat_index_to_visualize", "statistics", b"statistics"]) -> None: ...
+
+global___StatisticsViz = StatisticsViz
+
+@typing.final
 class OpSharding(google.protobuf.message.Message):
     """LINT.IfChange"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _Type:
         ValueType = typing.NewType("ValueType", builtins.int)
@@ -1520,14 +1754,18 @@
         """This sharding is a tuple - only the tuple_shardings field is valid."""
         OTHER: OpSharding._Type.ValueType  # 3
         """None of the above; tile_shape and tile_assignment are both used."""
         MANUAL: OpSharding._Type.ValueType  # 4
         """This op is manually sharded: the shapes are already partitioned and the
         partitioner should not change this op.
         """
+        UNKNOWN: OpSharding._Type.ValueType  # 5
+        """This sharding is a placeholder sharding with lowest precedence, it can be
+        overwriten by any other shardings.
+        """
 
     class Type(_Type, metaclass=_TypeEnumTypeWrapper): ...
     REPLICATED: OpSharding.Type.ValueType  # 0
     """This sharding is replicated across all devices (implies maximal,
     all other fields are unused).
     """
     MAXIMAL: OpSharding.Type.ValueType  # 1
@@ -1536,29 +1774,76 @@
     """This sharding is a tuple - only the tuple_shardings field is valid."""
     OTHER: OpSharding.Type.ValueType  # 3
     """None of the above; tile_shape and tile_assignment are both used."""
     MANUAL: OpSharding.Type.ValueType  # 4
     """This op is manually sharded: the shapes are already partitioned and the
     partitioner should not change this op.
     """
+    UNKNOWN: OpSharding.Type.ValueType  # 5
+    """This sharding is a placeholder sharding with lowest precedence, it can be
+    overwriten by any other shardings.
+    """
+
+    class _ShardGroupType:
+        ValueType = typing.NewType("ValueType", builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+
+    class _ShardGroupTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[OpSharding._ShardGroupType.ValueType], builtins.type):
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+        AS: OpSharding._ShardGroupType.ValueType  # 0
+        """This op will be sharded exactly the same as the other op. (hard
+        restriction)
+        """
+        LIKE: OpSharding._ShardGroupType.ValueType  # 1
+        """This op will try to allow sharding propagation within the same group even
+        there is no data dependencies among them, but there is no guarantee that
+        the final shardings within the same group will be exactly the same. (soft
+        restriction)
+        """
+
+    class ShardGroupType(_ShardGroupType, metaclass=_ShardGroupTypeEnumTypeWrapper):
+        """Used to decide whether this op is to be sharded like some other ops, or to
+        which other ops will be sharded like.
+        """
+
+    AS: OpSharding.ShardGroupType.ValueType  # 0
+    """This op will be sharded exactly the same as the other op. (hard
+    restriction)
+    """
+    LIKE: OpSharding.ShardGroupType.ValueType  # 1
+    """This op will try to allow sharding propagation within the same group even
+    there is no data dependencies among them, but there is no guarantee that
+    the final shardings within the same group will be exactly the same. (soft
+    restriction)
+    """
 
     TYPE_FIELD_NUMBER: builtins.int
     TILE_SHAPE_FIELD_NUMBER: builtins.int
     TILE_ASSIGNMENT_DIMENSIONS_FIELD_NUMBER: builtins.int
     TILE_ASSIGNMENT_DEVICES_FIELD_NUMBER: builtins.int
     TUPLE_SHARDINGS_FIELD_NUMBER: builtins.int
     REPLICATE_ON_LAST_TILE_DIM_FIELD_NUMBER: builtins.int
     METADATA_FIELD_NUMBER: builtins.int
     LAST_TILE_DIMS_FIELD_NUMBER: builtins.int
+    IOTA_RESHAPE_DIMS_FIELD_NUMBER: builtins.int
+    IOTA_TRANSPOSE_PERM_FIELD_NUMBER: builtins.int
+    IS_SHARD_GROUP_FIELD_NUMBER: builtins.int
+    SHARD_GROUP_ID_FIELD_NUMBER: builtins.int
+    SHARD_GROUP_TYPE_FIELD_NUMBER: builtins.int
     type: global___OpSharding.Type.ValueType
     replicate_on_last_tile_dim: builtins.bool
     """Only used for OTHER type. If true, data is sharded according to other
     dimensions of tile_assignment(), but replicated across devices along the
     last dimension. (Experimental)
     """
+    is_shard_group: builtins.bool
+    """This field decides whether this op is in a shard group."""
+    shard_group_id: builtins.int
+    """This field is used to store the unique id of the shard group."""
+    shard_group_type: global___OpSharding.ShardGroupType.ValueType
     @property
     def tile_shape(self) -> global___ShapeProto:
         """The shape of the sharded tile."""
 
     @property
     def tile_assignment_dimensions(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """The shape of the tile assignment tensor - this must be the same rank as
@@ -1566,14 +1851,15 @@
         tile_assignment_devices.size().
         """
 
     @property
     def tile_assignment_devices(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """Flattened list of device IDs. The order of flattening is the same as used
         by IndexUtil::MultiToLinearIndex(tile_assignment_shape).
+        Only one of tile_assignment_devices and iota_dimensions shall be non-empty.
         """
 
     @property
     def tuple_shardings(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___OpSharding]:
         """If type == TUPLE, the sub-shardings, one per leaf node in the tuple shape,
         in pre-order. The tuple shape could be nested; here we store just a
         flattened list of all leaves in the tuple shape. Note that the tuple shape
@@ -1596,28 +1882,46 @@
         """This field is used to represented the sharding type of each subgroup.
         For example, sharding={devices=[2,2,2,2]0,1,2,...,15 last_tile_dims={
         replicate, manual, unreduced}} means that each of the last 3 dimensions
         in [2,2,2,2] represents a subgrouping in replicate, manual,
         unreduced sharding type respectively.
         """
 
+    @property
+    def iota_reshape_dims(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
+        """Dimensions used to reshape the 1D iota array of device IDs.
+        Only one of tile_assignment_devices and iota_reshape_dims shall be
+        non-empty.
+        """
+
+    @property
+    def iota_transpose_perm(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
+        """Dimension permutations to transposed the iota array reshaped to
+        iota_reshape_dims. This must have the same size as iota_reshape_dims.
+        """
+
     def __init__(
         self,
         *,
         type: global___OpSharding.Type.ValueType | None = ...,
         tile_shape: global___ShapeProto | None = ...,
         tile_assignment_dimensions: collections.abc.Iterable[builtins.int] | None = ...,
         tile_assignment_devices: collections.abc.Iterable[builtins.int] | None = ...,
         tuple_shardings: collections.abc.Iterable[global___OpSharding] | None = ...,
         replicate_on_last_tile_dim: builtins.bool | None = ...,
         metadata: collections.abc.Iterable[global___OpMetadata] | None = ...,
         last_tile_dims: collections.abc.Iterable[global___OpSharding.Type.ValueType] | None = ...,
+        iota_reshape_dims: collections.abc.Iterable[builtins.int] | None = ...,
+        iota_transpose_perm: collections.abc.Iterable[builtins.int] | None = ...,
+        is_shard_group: builtins.bool | None = ...,
+        shard_group_id: builtins.int | None = ...,
+        shard_group_type: global___OpSharding.ShardGroupType.ValueType | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing.Literal["tile_shape", b"tile_shape"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing.Literal["last_tile_dims", b"last_tile_dims", "metadata", b"metadata", "replicate_on_last_tile_dim", b"replicate_on_last_tile_dim", "tile_assignment_devices", b"tile_assignment_devices", "tile_assignment_dimensions", b"tile_assignment_dimensions", "tile_shape", b"tile_shape", "tuple_shardings", b"tuple_shardings", "type", b"type"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["iota_reshape_dims", b"iota_reshape_dims", "iota_transpose_perm", b"iota_transpose_perm", "is_shard_group", b"is_shard_group", "last_tile_dims", b"last_tile_dims", "metadata", b"metadata", "replicate_on_last_tile_dim", b"replicate_on_last_tile_dim", "shard_group_id", b"shard_group_id", "shard_group_type", b"shard_group_type", "tile_assignment_devices", b"tile_assignment_devices", "tile_assignment_dimensions", b"tile_assignment_dimensions", "tile_shape", b"tile_shape", "tuple_shardings", b"tuple_shardings", "type", b"type"]) -> None: ...
 
 global___OpSharding = OpSharding
 
 @typing.final
 class ReplicaGroup(google.protobuf.message.Message):
     """Describes the replica groups in a cross replica op (e.g., all-reduce and
     all-to-all).
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/config/__init__.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/config/experimental.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/config/experimental.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/example/example_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/example/example_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/example/feature_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/example/feature_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/allocation_description_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/allocation_description_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/api_def_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/api_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/attr_value_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/attr_value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/cost_graph_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/cost_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/dataset_options_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/dataset_options_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 
 import builtins
+import collections.abc
 import sys
 import typing
 
 import google.protobuf.descriptor
+import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import tensorflow.core.framework.model_pb2
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
@@ -194,57 +196,60 @@
     def ClearField(self, field_name: typing.Literal["auto_shard_policy", b"auto_shard_policy", "num_devices", b"num_devices", "optional_num_devices", b"optional_num_devices"]) -> None: ...
     def WhichOneof(self, oneof_group: typing.Literal["optional_num_devices", b"optional_num_devices"]) -> typing.Literal["num_devices"] | None: ...
 
 global___DistributeOptions = DistributeOptions
 
 @typing.final
 class OptimizationOptions(google.protobuf.message.Message):
-    """next: 20"""
+    """next: 22"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     APPLY_DEFAULT_OPTIMIZATIONS_FIELD_NUMBER: builtins.int
     FILTER_FUSION_FIELD_NUMBER: builtins.int
     MAP_AND_BATCH_FUSION_FIELD_NUMBER: builtins.int
     MAP_AND_FILTER_FUSION_FIELD_NUMBER: builtins.int
     MAP_FUSION_FIELD_NUMBER: builtins.int
     MAP_PARALLELIZATION_FIELD_NUMBER: builtins.int
     NOOP_ELIMINATION_FIELD_NUMBER: builtins.int
     PARALLEL_BATCH_FIELD_NUMBER: builtins.int
     SHUFFLE_AND_REPEAT_FUSION_FIELD_NUMBER: builtins.int
     FILTER_PARALLELIZATION_FIELD_NUMBER: builtins.int
     INJECT_PREFETCH_FIELD_NUMBER: builtins.int
+    SEQ_INTERLEAVE_PREFETCH_FIELD_NUMBER: builtins.int
     apply_default_optimizations: builtins.bool
     filter_fusion: builtins.bool
     map_and_batch_fusion: builtins.bool
     map_and_filter_fusion: builtins.bool
     map_fusion: builtins.bool
     map_parallelization: builtins.bool
     noop_elimination: builtins.bool
     parallel_batch: builtins.bool
     shuffle_and_repeat_fusion: builtins.bool
     filter_parallelization: builtins.bool
     inject_prefetch: builtins.bool
+    seq_interleave_prefetch: builtins.bool
     def __init__(
         self,
         *,
         apply_default_optimizations: builtins.bool | None = ...,
         filter_fusion: builtins.bool | None = ...,
         map_and_batch_fusion: builtins.bool | None = ...,
         map_and_filter_fusion: builtins.bool | None = ...,
         map_fusion: builtins.bool | None = ...,
         map_parallelization: builtins.bool | None = ...,
         noop_elimination: builtins.bool | None = ...,
         parallel_batch: builtins.bool | None = ...,
         shuffle_and_repeat_fusion: builtins.bool | None = ...,
         filter_parallelization: builtins.bool | None = ...,
         inject_prefetch: builtins.bool | None = ...,
+        seq_interleave_prefetch: builtins.bool | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing.Literal["apply_default_optimizations", b"apply_default_optimizations", "filter_fusion", b"filter_fusion", "filter_parallelization", b"filter_parallelization", "inject_prefetch", b"inject_prefetch", "map_and_batch_fusion", b"map_and_batch_fusion", "map_and_filter_fusion", b"map_and_filter_fusion", "map_fusion", b"map_fusion", "map_parallelization", b"map_parallelization", "noop_elimination", b"noop_elimination", "optional_apply_default_optimizations", b"optional_apply_default_optimizations", "optional_filter_fusion", b"optional_filter_fusion", "optional_filter_parallelization", b"optional_filter_parallelization", "optional_inject_prefetch", b"optional_inject_prefetch", "optional_map_and_batch_fusion", b"optional_map_and_batch_fusion", "optional_map_and_filter_fusion", b"optional_map_and_filter_fusion", "optional_map_fusion", b"optional_map_fusion", "optional_map_parallelization", b"optional_map_parallelization", "optional_noop_elimination", b"optional_noop_elimination", "optional_parallel_batch", b"optional_parallel_batch", "optional_shuffle_and_repeat_fusion", b"optional_shuffle_and_repeat_fusion", "parallel_batch", b"parallel_batch", "shuffle_and_repeat_fusion", b"shuffle_and_repeat_fusion"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing.Literal["apply_default_optimizations", b"apply_default_optimizations", "filter_fusion", b"filter_fusion", "filter_parallelization", b"filter_parallelization", "inject_prefetch", b"inject_prefetch", "map_and_batch_fusion", b"map_and_batch_fusion", "map_and_filter_fusion", b"map_and_filter_fusion", "map_fusion", b"map_fusion", "map_parallelization", b"map_parallelization", "noop_elimination", b"noop_elimination", "optional_apply_default_optimizations", b"optional_apply_default_optimizations", "optional_filter_fusion", b"optional_filter_fusion", "optional_filter_parallelization", b"optional_filter_parallelization", "optional_inject_prefetch", b"optional_inject_prefetch", "optional_map_and_batch_fusion", b"optional_map_and_batch_fusion", "optional_map_and_filter_fusion", b"optional_map_and_filter_fusion", "optional_map_fusion", b"optional_map_fusion", "optional_map_parallelization", b"optional_map_parallelization", "optional_noop_elimination", b"optional_noop_elimination", "optional_parallel_batch", b"optional_parallel_batch", "optional_shuffle_and_repeat_fusion", b"optional_shuffle_and_repeat_fusion", "parallel_batch", b"parallel_batch", "shuffle_and_repeat_fusion", b"shuffle_and_repeat_fusion"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["apply_default_optimizations", b"apply_default_optimizations", "filter_fusion", b"filter_fusion", "filter_parallelization", b"filter_parallelization", "inject_prefetch", b"inject_prefetch", "map_and_batch_fusion", b"map_and_batch_fusion", "map_and_filter_fusion", b"map_and_filter_fusion", "map_fusion", b"map_fusion", "map_parallelization", b"map_parallelization", "noop_elimination", b"noop_elimination", "optional_apply_default_optimizations", b"optional_apply_default_optimizations", "optional_filter_fusion", b"optional_filter_fusion", "optional_filter_parallelization", b"optional_filter_parallelization", "optional_inject_prefetch", b"optional_inject_prefetch", "optional_map_and_batch_fusion", b"optional_map_and_batch_fusion", "optional_map_and_filter_fusion", b"optional_map_and_filter_fusion", "optional_map_fusion", b"optional_map_fusion", "optional_map_parallelization", b"optional_map_parallelization", "optional_noop_elimination", b"optional_noop_elimination", "optional_parallel_batch", b"optional_parallel_batch", "optional_seq_interleave_prefetch", b"optional_seq_interleave_prefetch", "optional_shuffle_and_repeat_fusion", b"optional_shuffle_and_repeat_fusion", "parallel_batch", b"parallel_batch", "seq_interleave_prefetch", b"seq_interleave_prefetch", "shuffle_and_repeat_fusion", b"shuffle_and_repeat_fusion"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["apply_default_optimizations", b"apply_default_optimizations", "filter_fusion", b"filter_fusion", "filter_parallelization", b"filter_parallelization", "inject_prefetch", b"inject_prefetch", "map_and_batch_fusion", b"map_and_batch_fusion", "map_and_filter_fusion", b"map_and_filter_fusion", "map_fusion", b"map_fusion", "map_parallelization", b"map_parallelization", "noop_elimination", b"noop_elimination", "optional_apply_default_optimizations", b"optional_apply_default_optimizations", "optional_filter_fusion", b"optional_filter_fusion", "optional_filter_parallelization", b"optional_filter_parallelization", "optional_inject_prefetch", b"optional_inject_prefetch", "optional_map_and_batch_fusion", b"optional_map_and_batch_fusion", "optional_map_and_filter_fusion", b"optional_map_and_filter_fusion", "optional_map_fusion", b"optional_map_fusion", "optional_map_parallelization", b"optional_map_parallelization", "optional_noop_elimination", b"optional_noop_elimination", "optional_parallel_batch", b"optional_parallel_batch", "optional_seq_interleave_prefetch", b"optional_seq_interleave_prefetch", "optional_shuffle_and_repeat_fusion", b"optional_shuffle_and_repeat_fusion", "parallel_batch", b"parallel_batch", "seq_interleave_prefetch", b"seq_interleave_prefetch", "shuffle_and_repeat_fusion", b"shuffle_and_repeat_fusion"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing.Literal["optional_apply_default_optimizations", b"optional_apply_default_optimizations"]) -> typing.Literal["apply_default_optimizations"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing.Literal["optional_filter_fusion", b"optional_filter_fusion"]) -> typing.Literal["filter_fusion"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing.Literal["optional_filter_parallelization", b"optional_filter_parallelization"]) -> typing.Literal["filter_parallelization"] | None: ...
     @typing.overload
@@ -258,14 +263,16 @@
     @typing.overload
     def WhichOneof(self, oneof_group: typing.Literal["optional_map_parallelization", b"optional_map_parallelization"]) -> typing.Literal["map_parallelization"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing.Literal["optional_noop_elimination", b"optional_noop_elimination"]) -> typing.Literal["noop_elimination"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing.Literal["optional_parallel_batch", b"optional_parallel_batch"]) -> typing.Literal["parallel_batch"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing.Literal["optional_seq_interleave_prefetch", b"optional_seq_interleave_prefetch"]) -> typing.Literal["seq_interleave_prefetch"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing.Literal["optional_shuffle_and_repeat_fusion", b"optional_shuffle_and_repeat_fusion"]) -> typing.Literal["shuffle_and_repeat_fusion"] | None: ...
 
 global___OptimizationOptions = OptimizationOptions
 
 @typing.final
 class ThreadingOptions(google.protobuf.message.Message):
     """next: 3"""
@@ -292,34 +299,43 @@
 global___ThreadingOptions = ThreadingOptions
 
 @typing.final
 class Options(google.protobuf.message.Message):
     """Message stored with Dataset objects to control how datasets are processed and
     optimized.
 
-    next: 9
+    next: 12
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    DATASET_NAME_FIELD_NUMBER: builtins.int
+    FRAMEWORK_TYPE_FIELD_NUMBER: builtins.int
     DETERMINISTIC_FIELD_NUMBER: builtins.int
     AUTOTUNE_OPTIONS_FIELD_NUMBER: builtins.int
     DISTRIBUTE_OPTIONS_FIELD_NUMBER: builtins.int
     OPTIMIZATION_OPTIONS_FIELD_NUMBER: builtins.int
     SLACK_FIELD_NUMBER: builtins.int
     THREADING_OPTIONS_FIELD_NUMBER: builtins.int
     EXTERNAL_STATE_POLICY_FIELD_NUMBER: builtins.int
     SYMBOLIC_CHECKPOINT_FIELD_NUMBER: builtins.int
+    WARM_START_FIELD_NUMBER: builtins.int
+    dataset_name: builtins.str
     deterministic: builtins.bool
     slack: builtins.bool
     external_state_policy: global___ExternalStatePolicy.ValueType
     symbolic_checkpoint: builtins.bool
+    warm_start: builtins.bool
+    @property
+    def framework_type(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+        """List of frameworks used to generate this dataset."""
+
     @property
     def autotune_options(self) -> global___AutotuneOptions:
-        """The distribution strategy options associated with the dataset."""
+        """The autotune options associated with the dataset."""
 
     @property
     def distribute_options(self) -> global___DistributeOptions:
         """The distribution strategy options associated with the dataset."""
 
     @property
     def optimization_options(self) -> global___OptimizationOptions:
@@ -328,28 +344,35 @@
     @property
     def threading_options(self) -> global___ThreadingOptions:
         """The threading options associated with the dataset."""
 
     def __init__(
         self,
         *,
+        dataset_name: builtins.str | None = ...,
+        framework_type: collections.abc.Iterable[builtins.str] | None = ...,
         deterministic: builtins.bool | None = ...,
         autotune_options: global___AutotuneOptions | None = ...,
         distribute_options: global___DistributeOptions | None = ...,
         optimization_options: global___OptimizationOptions | None = ...,
         slack: builtins.bool | None = ...,
         threading_options: global___ThreadingOptions | None = ...,
         external_state_policy: global___ExternalStatePolicy.ValueType | None = ...,
         symbolic_checkpoint: builtins.bool | None = ...,
+        warm_start: builtins.bool | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing.Literal["autotune_options", b"autotune_options", "deterministic", b"deterministic", "distribute_options", b"distribute_options", "external_state_policy", b"external_state_policy", "optimization_options", b"optimization_options", "optional_deterministic", b"optional_deterministic", "optional_external_state_policy", b"optional_external_state_policy", "optional_slack", b"optional_slack", "optional_symbolic_checkpoint", b"optional_symbolic_checkpoint", "slack", b"slack", "symbolic_checkpoint", b"symbolic_checkpoint", "threading_options", b"threading_options"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing.Literal["autotune_options", b"autotune_options", "deterministic", b"deterministic", "distribute_options", b"distribute_options", "external_state_policy", b"external_state_policy", "optimization_options", b"optimization_options", "optional_deterministic", b"optional_deterministic", "optional_external_state_policy", b"optional_external_state_policy", "optional_slack", b"optional_slack", "optional_symbolic_checkpoint", b"optional_symbolic_checkpoint", "slack", b"slack", "symbolic_checkpoint", b"symbolic_checkpoint", "threading_options", b"threading_options"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["autotune_options", b"autotune_options", "dataset_name", b"dataset_name", "deterministic", b"deterministic", "distribute_options", b"distribute_options", "external_state_policy", b"external_state_policy", "optimization_options", b"optimization_options", "optional_dataset_name", b"optional_dataset_name", "optional_deterministic", b"optional_deterministic", "optional_external_state_policy", b"optional_external_state_policy", "optional_slack", b"optional_slack", "optional_symbolic_checkpoint", b"optional_symbolic_checkpoint", "optional_warm_start", b"optional_warm_start", "slack", b"slack", "symbolic_checkpoint", b"symbolic_checkpoint", "threading_options", b"threading_options", "warm_start", b"warm_start"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["autotune_options", b"autotune_options", "dataset_name", b"dataset_name", "deterministic", b"deterministic", "distribute_options", b"distribute_options", "external_state_policy", b"external_state_policy", "framework_type", b"framework_type", "optimization_options", b"optimization_options", "optional_dataset_name", b"optional_dataset_name", "optional_deterministic", b"optional_deterministic", "optional_external_state_policy", b"optional_external_state_policy", "optional_slack", b"optional_slack", "optional_symbolic_checkpoint", b"optional_symbolic_checkpoint", "optional_warm_start", b"optional_warm_start", "slack", b"slack", "symbolic_checkpoint", b"symbolic_checkpoint", "threading_options", b"threading_options", "warm_start", b"warm_start"]) -> None: ...
+    @typing.overload
+    def WhichOneof(self, oneof_group: typing.Literal["optional_dataset_name", b"optional_dataset_name"]) -> typing.Literal["dataset_name"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing.Literal["optional_deterministic", b"optional_deterministic"]) -> typing.Literal["deterministic"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing.Literal["optional_external_state_policy", b"optional_external_state_policy"]) -> typing.Literal["external_state_policy"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing.Literal["optional_slack", b"optional_slack"]) -> typing.Literal["slack"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing.Literal["optional_symbolic_checkpoint", b"optional_symbolic_checkpoint"]) -> typing.Literal["symbolic_checkpoint"] | None: ...
+    @typing.overload
+    def WhichOneof(self, oneof_group: typing.Literal["optional_warm_start", b"optional_warm_start"]) -> typing.Literal["warm_start"] | None: ...
 
 global___Options = Options
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/dataset_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/device_attributes_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/device_attributes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/full_type_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/full_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/function_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/graph_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,84 +1,79 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
-"""
+Protocol buffer representing the shape of tensors."""
 
 import builtins
 import collections.abc
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import tensorflow.core.framework.function_pb2
-import tensorflow.core.framework.node_def_pb2
-import tensorflow.core.framework.versions_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing.final
-class GraphDef(google.protobuf.message.Message):
-    """Represents the graph of operations"""
+class TensorShapeProto(google.protobuf.message.Message):
+    """Dimensions of a tensor."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    NODE_FIELD_NUMBER: builtins.int
-    VERSIONS_FIELD_NUMBER: builtins.int
-    VERSION_FIELD_NUMBER: builtins.int
-    LIBRARY_FIELD_NUMBER: builtins.int
-    version: builtins.int
-    """Deprecated single version field; use versions above instead.  Since all
-    GraphDef changes before "versions" was introduced were forward
-    compatible, this field is entirely ignored.
-    """
-    @property
-    def node(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.core.framework.node_def_pb2.NodeDef]: ...
-    @property
-    def versions(self) -> tensorflow.core.framework.versions_pb2.VersionDef:
-        """Compatibility versions of the graph.  See core/public/version.h for version
-        history.  The GraphDef version is distinct from the TensorFlow version, and
-        each release of TensorFlow will support a range of GraphDef versions.
+    @typing.final
+    class Dim(google.protobuf.message.Message):
+        """One dimension of the tensor."""
+
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        SIZE_FIELD_NUMBER: builtins.int
+        NAME_FIELD_NUMBER: builtins.int
+        size: builtins.int
+        """Size of the tensor in that dimension.
+        This value must be >= -1, but values of -1 are reserved for "unknown"
+        shapes (values of -1 mean "unknown" dimension).  Certain wrappers
+        that work with TensorShapeProto may fail at runtime when deserializing
+        a TensorShapeProto containing a dim value of -1.
         """
+        name: builtins.str
+        """Optional name of the tensor dimension."""
+        def __init__(
+            self,
+            *,
+            size: builtins.int | None = ...,
+            name: builtins.str | None = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing.Literal["name", b"name", "size", b"size"]) -> None: ...
+
+    DIM_FIELD_NUMBER: builtins.int
+    UNKNOWN_RANK_FIELD_NUMBER: builtins.int
+    unknown_rank: builtins.bool
+    """If true, the number of dimensions in the shape is unknown.
 
+    If true, "dim.size()" must be 0.
+    """
     @property
-    def library(self) -> tensorflow.core.framework.function_pb2.FunctionDefLibrary:
-        """"library" provides user-defined functions.
+    def dim(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TensorShapeProto.Dim]:
+        """Dimensions of the tensor, such as {"input", 30}, {"output", 40}
+        for a 30 x 40 2D tensor.  If an entry has size -1, this
+        corresponds to a dimension of unknown size. The names are
+        optional.
+
+        The order of entries in "dim" matters: It indicates the layout of the
+        values in the tensor in-memory representation.
+
+        The first entry in "dim" is the outermost dimension used to layout the
+        values, the last entry is the innermost dimension.  This matches the
+        in-memory layout of RowMajor Eigen tensors.
 
-        Naming:
-          * library.function.name are in a flat namespace.
-            NOTE: We may need to change it to be hierarchical to support
-            different orgs. E.g.,
-            { "/google/nn", { ... }},
-            { "/google/vision", { ... }}
-            { "/org_foo/module_bar", { ... }}
-            map<string, FunctionDefLib> named_lib;
-          * If node[i].op is the name of one function in "library",
-            node[i] is deemed as a function call. Otherwise, node[i].op
-            must be a primitive operation supported by the runtime.
-
-
-        Function call semantics:
-
-          * The callee may start execution as soon as some of its inputs
-            are ready. The caller may want to use Tuple() mechanism to
-            ensure all inputs are ready in the same time.
-
-          * The consumer of return values may start executing as soon as
-            the return values the consumer depends on are ready.  The
-            consumer may want to use Tuple() mechanism to ensure the
-            consumer does not start until all return values of the callee
-            function are ready.
+        If "dim.size()" > 0, "unknown_rank" must be false.
         """
 
     def __init__(
         self,
         *,
-        node: collections.abc.Iterable[tensorflow.core.framework.node_def_pb2.NodeDef] | None = ...,
-        versions: tensorflow.core.framework.versions_pb2.VersionDef | None = ...,
-        version: builtins.int | None = ...,
-        library: tensorflow.core.framework.function_pb2.FunctionDefLibrary | None = ...,
+        dim: collections.abc.Iterable[global___TensorShapeProto.Dim] | None = ...,
+        unknown_rank: builtins.bool | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing.Literal["library", b"library", "versions", b"versions"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing.Literal["library", b"library", "node", b"node", "version", b"version", "versions", b"versions"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["dim", b"dim", "unknown_rank", b"unknown_rank"]) -> None: ...
 
-global___GraphDef = GraphDef
+global___TensorShapeProto = TensorShapeProto
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/kernel_def_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/kernel_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/log_memory_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/log_memory_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/model_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/model_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -247,33 +247,41 @@
             algorithm: global___AutotuneAlgorithm.ValueType | None = ...,
             cpu_budget: builtins.int | None = ...,
             ram_budget: builtins.int | None = ...,
             model_input_time: builtins.float | None = ...,
         ) -> None: ...
         def ClearField(self, field_name: typing.Literal["algorithm", b"algorithm", "cpu_budget", b"cpu_budget", "model_input_time", b"model_input_time", "ram_budget", b"ram_budget"]) -> None: ...
 
+    DATASET_NAME_FIELD_NUMBER: builtins.int
     NODES_FIELD_NUMBER: builtins.int
     OUTPUT_FIELD_NUMBER: builtins.int
     ID_COUNTER_FIELD_NUMBER: builtins.int
     OPTIMIZATION_PARAMS_FIELD_NUMBER: builtins.int
+    GAP_TIMES_FIELD_NUMBER: builtins.int
+    dataset_name: builtins.str
+    """User-defined name for the dataset. Empty if no name was set."""
     output: builtins.int
     """ID of the output node of this model."""
     id_counter: builtins.int
     """Counter for node IDs of this model."""
     @property
     def nodes(self) -> google.protobuf.internal.containers.MessageMap[builtins.int, global___ModelProto.Node]:
         """Map of node IDs to nodes of this model."""
 
     @property
     def optimization_params(self) -> global___ModelProto.OptimizationParams: ...
+    @property
+    def gap_times(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     def __init__(
         self,
         *,
+        dataset_name: builtins.str | None = ...,
         nodes: collections.abc.Mapping[builtins.int, global___ModelProto.Node] | None = ...,
         output: builtins.int | None = ...,
         id_counter: builtins.int | None = ...,
         optimization_params: global___ModelProto.OptimizationParams | None = ...,
+        gap_times: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing.Literal["optimization_params", b"optimization_params"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing.Literal["id_counter", b"id_counter", "nodes", b"nodes", "optimization_params", b"optimization_params", "output", b"output"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["dataset_name", b"dataset_name", "gap_times", b"gap_times", "id_counter", b"id_counter", "nodes", b"nodes", "optimization_params", b"optimization_params", "output", b"output"]) -> None: ...
 
 global___ModelProto = ModelProto
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/node_def_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/node_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/op_def_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/op_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/reader_base_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/reader_base_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/resource_handle_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/resource_handle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/step_stats_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/step_stats_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/summary_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/summary_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/tensor_description_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/tensor_description_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/tensor_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/tensor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,78 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
-Protocol buffer representing the shape of tensors."""
+"""
 
 import builtins
 import collections.abc
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
+import tensorflow.core.framework.tensor_shape_pb2
+import tensorflow.core.framework.types_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing.final
-class TensorShapeProto(google.protobuf.message.Message):
-    """Dimensions of a tensor."""
-
+class ResourceDtypeAndShape(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing.final
-    class Dim(google.protobuf.message.Message):
-        """One dimension of the tensor."""
-
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-        SIZE_FIELD_NUMBER: builtins.int
-        NAME_FIELD_NUMBER: builtins.int
-        size: builtins.int
-        """Size of the tensor in that dimension.
-        This value must be >= -1, but values of -1 are reserved for "unknown"
-        shapes (values of -1 mean "unknown" dimension).  Certain wrappers
-        that work with TensorShapeProto may fail at runtime when deserializing
-        a TensorShapeProto containing a dim value of -1.
-        """
-        name: builtins.str
-        """Optional name of the tensor dimension."""
-        def __init__(
-            self,
-            *,
-            size: builtins.int | None = ...,
-            name: builtins.str | None = ...,
-        ) -> None: ...
-        def ClearField(self, field_name: typing.Literal["name", b"name", "size", b"size"]) -> None: ...
-
-    DIM_FIELD_NUMBER: builtins.int
-    UNKNOWN_RANK_FIELD_NUMBER: builtins.int
-    unknown_rank: builtins.bool
-    """If true, the number of dimensions in the shape is unknown.
+    DTYPE_FIELD_NUMBER: builtins.int
+    SHAPE_FIELD_NUMBER: builtins.int
+    dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
+    @property
+    def shape(self) -> tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto: ...
+    def __init__(
+        self,
+        *,
+        dtype: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
+        shape: tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing.Literal["shape", b"shape"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["dtype", b"dtype", "shape", b"shape"]) -> None: ...
 
-    If true, "dim.size()" must be 0.
+global___ResourceDtypeAndShape = ResourceDtypeAndShape
+
+@typing.final
+class RemoteTensorHandle(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    OP_ID_FIELD_NUMBER: builtins.int
+    OUTPUT_NUM_FIELD_NUMBER: builtins.int
+    DEVICE_FIELD_NUMBER: builtins.int
+    OP_DEVICE_FIELD_NUMBER: builtins.int
+    DTYPE_FIELD_NUMBER: builtins.int
+    RESOURCE_DTYPES_AND_SHAPES_FIELD_NUMBER: builtins.int
+    op_id: builtins.int
+    """The ID of the operation that produced this tensor."""
+    output_num: builtins.int
+    """The index into the outputs of the operation that produced this tensor."""
+    device: builtins.str
+    """Device where the tensor is located. Cannot be empty.
+    For multi-device functions, it's the default device passed to placer.
+    """
+    op_device: builtins.str
+    """Device of the operation producing this tensor. Can be empty if the
+    operation producing this tensor is a multi-device function.
     """
+    dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
+    """Tensor type."""
     @property
-    def dim(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TensorShapeProto.Dim]:
-        """Dimensions of the tensor, such as {"input", 30}, {"output", 40}
-        for a 30 x 40 2D tensor.  If an entry has size -1, this
-        corresponds to a dimension of unknown size. The names are
-        optional.
-
-        The order of entries in "dim" matters: It indicates the layout of the
-        values in the tensor in-memory representation.
-
-        The first entry in "dim" is the outermost dimension used to layout the
-        values, the last entry is the innermost dimension.  This matches the
-        in-memory layout of RowMajor Eigen tensors.
-
-        If "dim.size()" > 0, "unknown_rank" must be false.
-        """
+    def resource_dtypes_and_shapes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ResourceDtypeAndShape]:
+        """Optional data types and shapes of a remote resource variable."""
 
     def __init__(
         self,
         *,
-        dim: collections.abc.Iterable[global___TensorShapeProto.Dim] | None = ...,
-        unknown_rank: builtins.bool | None = ...,
+        op_id: builtins.int | None = ...,
+        output_num: builtins.int | None = ...,
+        device: builtins.str | None = ...,
+        op_device: builtins.str | None = ...,
+        dtype: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
+        resource_dtypes_and_shapes: collections.abc.Iterable[global___ResourceDtypeAndShape] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing.Literal["dim", b"dim", "unknown_rank", b"unknown_rank"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["device", b"device", "dtype", b"dtype", "op_device", b"op_device", "op_id", b"op_id", "output_num", b"output_num", "resource_dtypes_and_shapes", b"resource_dtypes_and_shapes"]) -> None: ...
 
-global___TensorShapeProto = TensorShapeProto
+global___RemoteTensorHandle = RemoteTensorHandle
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/types_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/types_pb2.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -63,19 +63,26 @@
     """Arbitrary C++ data types"""
     DT_UINT32: _DataType.ValueType  # 22
     DT_UINT64: _DataType.ValueType  # 23
     DT_FLOAT8_E5M2: _DataType.ValueType  # 24
     """5 exponent bits, 2 mantissa bits."""
     DT_FLOAT8_E4M3FN: _DataType.ValueType  # 25
     """4 exponent bits, 3 mantissa bits, finite-only, with"""
-    DT_FLOAT_REF: _DataType.ValueType  # 101
+    DT_INT4: _DataType.ValueType  # 29
     """2 NaNs (0bS1111111).
-
-    Do not use!  These are only for parameters.  Every enum above
-    should have a corresponding value below (verified by types_test).
+    TODO - b/299182407: Leaving room for remaining float8 types.
+    DT_FLOAT8_E4M3FNUZ = 26;
+    DT_FLOAT8_E4M3B11FNUZ = 27;
+    DT_FLOAT8_E5M2FNUZ = 28;
+    """
+    DT_UINT4: _DataType.ValueType  # 30
+    DT_FLOAT_REF: _DataType.ValueType  # 101
+    """Do not use!  These are only for TF1's obsolete reference Variables.
+    Every enum above should have a corresponding value below (verified by
+    types_test).
     """
     DT_DOUBLE_REF: _DataType.ValueType  # 102
     DT_INT32_REF: _DataType.ValueType  # 103
     DT_UINT8_REF: _DataType.ValueType  # 104
     DT_INT16_REF: _DataType.ValueType  # 105
     DT_INT8_REF: _DataType.ValueType  # 106
     DT_STRING_REF: _DataType.ValueType  # 107
@@ -93,14 +100,21 @@
     DT_HALF_REF: _DataType.ValueType  # 119
     DT_RESOURCE_REF: _DataType.ValueType  # 120
     DT_VARIANT_REF: _DataType.ValueType  # 121
     DT_UINT32_REF: _DataType.ValueType  # 122
     DT_UINT64_REF: _DataType.ValueType  # 123
     DT_FLOAT8_E5M2_REF: _DataType.ValueType  # 124
     DT_FLOAT8_E4M3FN_REF: _DataType.ValueType  # 125
+    DT_INT4_REF: _DataType.ValueType  # 129
+    """TODO - b/299182407: Leaving room for remaining float8 types.
+    DT_FLOAT8_E4M3FNUZ_REF = 126;
+    DT_FLOAT8_E4M3B11FNUZ_REF = 127;
+    DT_FLOAT8_E5M2FNUZ_REF = 128;
+    """
+    DT_UINT4_REF: _DataType.ValueType  # 130
 
 class DataType(_DataType, metaclass=_DataTypeEnumTypeWrapper):
     """(== suppress_warning documentation-presence ==)
     LINT.IfChange
     """
 
 DT_INVALID: DataType.ValueType  # 0
@@ -142,19 +156,26 @@
 """Arbitrary C++ data types"""
 DT_UINT32: DataType.ValueType  # 22
 DT_UINT64: DataType.ValueType  # 23
 DT_FLOAT8_E5M2: DataType.ValueType  # 24
 """5 exponent bits, 2 mantissa bits."""
 DT_FLOAT8_E4M3FN: DataType.ValueType  # 25
 """4 exponent bits, 3 mantissa bits, finite-only, with"""
-DT_FLOAT_REF: DataType.ValueType  # 101
+DT_INT4: DataType.ValueType  # 29
 """2 NaNs (0bS1111111).
-
-Do not use!  These are only for parameters.  Every enum above
-should have a corresponding value below (verified by types_test).
+TODO - b/299182407: Leaving room for remaining float8 types.
+DT_FLOAT8_E4M3FNUZ = 26;
+DT_FLOAT8_E4M3B11FNUZ = 27;
+DT_FLOAT8_E5M2FNUZ = 28;
+"""
+DT_UINT4: DataType.ValueType  # 30
+DT_FLOAT_REF: DataType.ValueType  # 101
+"""Do not use!  These are only for TF1's obsolete reference Variables.
+Every enum above should have a corresponding value below (verified by
+types_test).
 """
 DT_DOUBLE_REF: DataType.ValueType  # 102
 DT_INT32_REF: DataType.ValueType  # 103
 DT_UINT8_REF: DataType.ValueType  # 104
 DT_INT16_REF: DataType.ValueType  # 105
 DT_INT8_REF: DataType.ValueType  # 106
 DT_STRING_REF: DataType.ValueType  # 107
@@ -172,14 +193,21 @@
 DT_HALF_REF: DataType.ValueType  # 119
 DT_RESOURCE_REF: DataType.ValueType  # 120
 DT_VARIANT_REF: DataType.ValueType  # 121
 DT_UINT32_REF: DataType.ValueType  # 122
 DT_UINT64_REF: DataType.ValueType  # 123
 DT_FLOAT8_E5M2_REF: DataType.ValueType  # 124
 DT_FLOAT8_E4M3FN_REF: DataType.ValueType  # 125
+DT_INT4_REF: DataType.ValueType  # 129
+"""TODO - b/299182407: Leaving room for remaining float8 types.
+DT_FLOAT8_E4M3FNUZ_REF = 126;
+DT_FLOAT8_E4M3B11FNUZ_REF = 127;
+DT_FLOAT8_E5M2FNUZ_REF = 128;
+"""
+DT_UINT4_REF: DataType.ValueType  # 130
 global___DataType = DataType
 
 @typing.final
 class SerializedDType(google.protobuf.message.Message):
     """Represents a serialized tf.dtypes.Dtype"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/variable_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/variable_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/framework/versions_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/versions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/cluster_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/cluster_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,17 @@
     @property
     def tasks(self) -> google.protobuf.internal.containers.ScalarMap[builtins.int, builtins.str]:
         """Mapping from task ID to "hostname:port" string.
 
         If the `name` field contains "worker", and the `tasks` map contains a
         mapping from 7 to "example.org:2222", then the device prefix
         "/job:worker/task:7" will be assigned to "example.org:2222".
+
+        If a job has multiple replicas, host-ports will be comma-delimited, with
+        one entry for each replica.
         """
 
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         tasks: collections.abc.Mapping[builtins.int, builtins.str] | None = ...,
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/config_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/config_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,16 @@
             PRIORITY_FIELD_NUMBER: builtins.int
             DEVICE_ORDINAL_FIELD_NUMBER: builtins.int
             @property
             def memory_limit_mb(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]:
                 """Per "virtual" device memory limit, in MB. The number of elements in
                 the list is the number of virtual devices to create on the
                 corresponding visible GPU (see "virtual_devices" below).
-                If empty, it will create single virtual device taking all available
-                memory from the device.
+                If empty and `num_virtual_devices_per_gpu` is not set, it will create
+                single virtual device taking all available memory from the device.
 
                 For the concept of "visible" and "virtual" GPU, see the comments for
                 "visible_device_list" above for more information.
                 """
 
             @property
             def priority(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
@@ -87,26 +87,34 @@
                 memory_limit_mb: collections.abc.Iterable[builtins.float] | None = ...,
                 priority: collections.abc.Iterable[builtins.int] | None = ...,
                 device_ordinal: collections.abc.Iterable[builtins.int] | None = ...,
             ) -> None: ...
             def ClearField(self, field_name: typing.Literal["device_ordinal", b"device_ordinal", "memory_limit_mb", b"memory_limit_mb", "priority", b"priority"]) -> None: ...
 
         VIRTUAL_DEVICES_FIELD_NUMBER: builtins.int
+        NUM_VIRTUAL_DEVICES_PER_GPU_FIELD_NUMBER: builtins.int
         USE_UNIFIED_MEMORY_FIELD_NUMBER: builtins.int
         NUM_DEV_TO_DEV_COPY_STREAMS_FIELD_NUMBER: builtins.int
         COLLECTIVE_RING_ORDER_FIELD_NUMBER: builtins.int
         TIMESTAMPED_ALLOCATOR_FIELD_NUMBER: builtins.int
         KERNEL_TRACKER_MAX_INTERVAL_FIELD_NUMBER: builtins.int
         KERNEL_TRACKER_MAX_BYTES_FIELD_NUMBER: builtins.int
         KERNEL_TRACKER_MAX_PENDING_FIELD_NUMBER: builtins.int
         INTERNAL_FRAGMENTATION_FRACTION_FIELD_NUMBER: builtins.int
         USE_CUDA_MALLOC_ASYNC_FIELD_NUMBER: builtins.int
         DISALLOW_RETRY_ON_ALLOCATION_FAILURE_FIELD_NUMBER: builtins.int
         GPU_HOST_MEM_LIMIT_IN_MB_FIELD_NUMBER: builtins.int
         GPU_HOST_MEM_DISALLOW_GROWTH_FIELD_NUMBER: builtins.int
+        GPU_SYSTEM_MEMORY_SIZE_IN_MB_FIELD_NUMBER: builtins.int
+        num_virtual_devices_per_gpu: builtins.int
+        """The number of virtual devices to create on each visible GPU. The
+        available memory will be split equally among all virtual devices. If the
+        field `memory_limit_mb` in `VirtualDevices` is not empty, this field will
+        be ignored.
+        """
         use_unified_memory: builtins.bool
         """If true, uses CUDA unified memory for memory allocations. If
         per_process_gpu_memory_fraction option is greater than 1.0, then unified
         memory is used regardless of the value for this field. See comments for
         per_process_gpu_memory_fraction field for more details and requirements
         of the unified memory. This option is useful to oversubscribe memory if
         multiple processes are sharing a single GPU while individually using less
@@ -181,14 +189,21 @@
         never grows.  This can be useful for latency-sensitive systems, because
         growing the GPU host memory pool can be expensive.
 
         You probably only want to use this in combination with
         gpu_host_mem_limit_in_mb, because the default GPU host memory limit is
         quite high.
         """
+        gpu_system_memory_size_in_mb: builtins.int
+        """Memory limit for gpu system. This can also be set by
+        TF_DEVICE_MIN_SYS_MEMORY_IN_MB, which takes precedence over
+        gpu_system_memory_size_in_mb. With this, user can configure the gpu
+        system memory size for better resource estimation of multi-tenancy(one
+        gpu with multiple model) use case.
+        """
         @property
         def virtual_devices(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___GPUOptions.Experimental.VirtualDevices]:
             """The multi virtual device settings. If empty (not set), it will create
             single virtual device on each visible GPU, according to the settings
             in "visible_device_list" above. Otherwise, the number of elements in the
             list must be the same as the number of visible GPUs (after
             "visible_device_list" filtering if it is set), and the string represented
@@ -227,28 +242,30 @@
                result in undefined behavior.
             """
 
         def __init__(
             self,
             *,
             virtual_devices: collections.abc.Iterable[global___GPUOptions.Experimental.VirtualDevices] | None = ...,
+            num_virtual_devices_per_gpu: builtins.int | None = ...,
             use_unified_memory: builtins.bool | None = ...,
             num_dev_to_dev_copy_streams: builtins.int | None = ...,
             collective_ring_order: builtins.str | None = ...,
             timestamped_allocator: builtins.bool | None = ...,
             kernel_tracker_max_interval: builtins.int | None = ...,
             kernel_tracker_max_bytes: builtins.int | None = ...,
             kernel_tracker_max_pending: builtins.int | None = ...,
             internal_fragmentation_fraction: builtins.float | None = ...,
             use_cuda_malloc_async: builtins.bool | None = ...,
             disallow_retry_on_allocation_failure: builtins.bool | None = ...,
             gpu_host_mem_limit_in_mb: builtins.float | None = ...,
             gpu_host_mem_disallow_growth: builtins.bool | None = ...,
+            gpu_system_memory_size_in_mb: builtins.int | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing.Literal["collective_ring_order", b"collective_ring_order", "disallow_retry_on_allocation_failure", b"disallow_retry_on_allocation_failure", "gpu_host_mem_disallow_growth", b"gpu_host_mem_disallow_growth", "gpu_host_mem_limit_in_mb", b"gpu_host_mem_limit_in_mb", "internal_fragmentation_fraction", b"internal_fragmentation_fraction", "kernel_tracker_max_bytes", b"kernel_tracker_max_bytes", "kernel_tracker_max_interval", b"kernel_tracker_max_interval", "kernel_tracker_max_pending", b"kernel_tracker_max_pending", "num_dev_to_dev_copy_streams", b"num_dev_to_dev_copy_streams", "timestamped_allocator", b"timestamped_allocator", "use_cuda_malloc_async", b"use_cuda_malloc_async", "use_unified_memory", b"use_unified_memory", "virtual_devices", b"virtual_devices"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["collective_ring_order", b"collective_ring_order", "disallow_retry_on_allocation_failure", b"disallow_retry_on_allocation_failure", "gpu_host_mem_disallow_growth", b"gpu_host_mem_disallow_growth", "gpu_host_mem_limit_in_mb", b"gpu_host_mem_limit_in_mb", "gpu_system_memory_size_in_mb", b"gpu_system_memory_size_in_mb", "internal_fragmentation_fraction", b"internal_fragmentation_fraction", "kernel_tracker_max_bytes", b"kernel_tracker_max_bytes", "kernel_tracker_max_interval", b"kernel_tracker_max_interval", "kernel_tracker_max_pending", b"kernel_tracker_max_pending", "num_dev_to_dev_copy_streams", b"num_dev_to_dev_copy_streams", "num_virtual_devices_per_gpu", b"num_virtual_devices_per_gpu", "timestamped_allocator", b"timestamped_allocator", "use_cuda_malloc_async", b"use_cuda_malloc_async", "use_unified_memory", b"use_unified_memory", "virtual_devices", b"virtual_devices"]) -> None: ...
 
     PER_PROCESS_GPU_MEMORY_FRACTION_FIELD_NUMBER: builtins.int
     ALLOW_GROWTH_FIELD_NUMBER: builtins.int
     ALLOCATOR_TYPE_FIELD_NUMBER: builtins.int
     DEFERRED_DELETION_BYTES_FIELD_NUMBER: builtins.int
     VISIBLE_DEVICE_LIST_FIELD_NUMBER: builtins.int
     POLLING_ACTIVE_DELAY_USECS_FIELD_NUMBER: builtins.int
@@ -691,18 +708,24 @@
         OPTIMIZE_FOR_STATIC_GRAPH_FIELD_NUMBER: builtins.int
         ENABLE_MLIR_BRIDGE_FIELD_NUMBER: builtins.int
         MLIR_BRIDGE_ROLLOUT_FIELD_NUMBER: builtins.int
         ENABLE_MLIR_GRAPH_OPTIMIZATION_FIELD_NUMBER: builtins.int
         DISABLE_OUTPUT_PARTITION_GRAPHS_FIELD_NUMBER: builtins.int
         XLA_FUSION_AUTOTUNER_THRESH_FIELD_NUMBER: builtins.int
         USE_TFRT_FIELD_NUMBER: builtins.int
+        ENABLE_MULTI_HOST_FIELD_NUMBER: builtins.int
+        BACKEND_SERVER_PORT_FIELD_NUMBER: builtins.int
+        TARGET_TPU_FIELD_NUMBER: builtins.int
+        TARGET_GPU_FIELD_NUMBER: builtins.int
+        STREAM_MERGE_THRESHOLD_FIELD_NUMBER: builtins.int
         DISABLE_FUNCTIONAL_OPS_LOWERING_FIELD_NUMBER: builtins.int
         XLA_PREFER_SINGLE_GRAPH_CLUSTER_FIELD_NUMBER: builtins.int
         COORDINATION_CONFIG_FIELD_NUMBER: builtins.int
         DISABLE_OPTIMIZE_FOR_STATIC_GRAPH_FIELD_NUMBER: builtins.int
+        DISABLE_EAGER_EXECUTOR_STREAMING_ENQUEUE_FIELD_NUMBER: builtins.int
         collective_group_leader: builtins.str
         """Task name for group resolution."""
         executor_type: builtins.str
         """Which executor to use, the default executor will be used
         if it is an empty string or "DEFAULT"
         """
         recv_buf_max_chunk: builtins.int
@@ -797,14 +820,31 @@
         autotuner is enabled. Default value of zero disables the autotuner.
 
         The XLA fusion autotuner can improve performance by executing a heuristic
         search on the compiler parameters.
         """
         use_tfrt: builtins.bool
         """Whether runtime execution uses TFRT."""
+        enable_multi_host: builtins.bool
+        """If true, use Pathways with TFRT API for multi host support."""
+        backend_server_port: builtins.int
+        """Port for the Pathways server. Ignored if enable_multi_host=false."""
+        target_tpu: builtins.bool
+        """If true, TFRT will use TPU specific compiler passes and perform TPU
+        specific initialization.
+        """
+        target_gpu: builtins.bool
+        """If true, TFRT will use GPU specific compiler passes and perform GPU
+        specific initialization.
+        """
+        stream_merge_threshold: builtins.int
+        """The threshold to merge small streams in TFRT. The stream with cost
+        smaller than the threshold will be merged. Setting it to value 1
+        disables all merges.
+        """
         disable_functional_ops_lowering: builtins.bool
         """Whether functional control flow op lowering should be disabled. This is
         useful when executing within a portable runtime where control flow op
         kernels may not be loaded due to selective registration.
         """
         xla_prefer_single_graph_cluster: builtins.bool
         """Provides a hint to XLA auto clustering to prefer forming a single large
@@ -817,14 +857,19 @@
         If this option is set to true when a session is created, the full
         GraphDef will be retained to enable calls to Session::Extend().
         Calling Extend() without setting this flag will result in errors.
 
         This option is meant to replace `optimize_for_static_graph` and it
         aims to negate its value.
         """
+        disable_eager_executor_streaming_enqueue: builtins.bool
+        """Whether eager remote execution will stream all the function calls or
+        allow them to happen in parallel. When true, streaming execution is
+        disabled, and parallel execution is allowed.
+        """
         @property
         def session_metadata(self) -> global___SessionMetadata:
             """Metadata about the session.
 
             If set, this can be used by the runtime and the Ops for debugging,
             monitoring, etc.
 
@@ -852,21 +897,27 @@
             optimize_for_static_graph: builtins.bool | None = ...,
             enable_mlir_bridge: builtins.bool | None = ...,
             mlir_bridge_rollout: global___ConfigProto.Experimental.MlirBridgeRollout.ValueType | None = ...,
             enable_mlir_graph_optimization: builtins.bool | None = ...,
             disable_output_partition_graphs: builtins.bool | None = ...,
             xla_fusion_autotuner_thresh: builtins.int | None = ...,
             use_tfrt: builtins.bool | None = ...,
+            enable_multi_host: builtins.bool | None = ...,
+            backend_server_port: builtins.int | None = ...,
+            target_tpu: builtins.bool | None = ...,
+            target_gpu: builtins.bool | None = ...,
+            stream_merge_threshold: builtins.int | None = ...,
             disable_functional_ops_lowering: builtins.bool | None = ...,
             xla_prefer_single_graph_cluster: builtins.bool | None = ...,
             coordination_config: tensorflow.tsl.protobuf.coordination_config_pb2.CoordinationServiceConfig | None = ...,
             disable_optimize_for_static_graph: builtins.bool | None = ...,
+            disable_eager_executor_streaming_enqueue: builtins.bool | None = ...,
         ) -> None: ...
         def HasField(self, field_name: typing.Literal["coordination_config", b"coordination_config", "session_metadata", b"session_metadata"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing.Literal["collective_deterministic_sequential_execution", b"collective_deterministic_sequential_execution", "collective_group_leader", b"collective_group_leader", "collective_nccl", b"collective_nccl", "coordination_config", b"coordination_config", "disable_functional_ops_lowering", b"disable_functional_ops_lowering", "disable_optimize_for_static_graph", b"disable_optimize_for_static_graph", "disable_output_partition_graphs", b"disable_output_partition_graphs", "disable_thread_spinning", b"disable_thread_spinning", "enable_mlir_bridge", b"enable_mlir_bridge", "enable_mlir_graph_optimization", b"enable_mlir_graph_optimization", "executor_type", b"executor_type", "mlir_bridge_rollout", b"mlir_bridge_rollout", "optimize_for_static_graph", b"optimize_for_static_graph", "recv_buf_max_chunk", b"recv_buf_max_chunk", "session_metadata", b"session_metadata", "share_cluster_devices_in_session", b"share_cluster_devices_in_session", "share_session_state_in_clusterspec_propagation", b"share_session_state_in_clusterspec_propagation", "use_numa_affinity", b"use_numa_affinity", "use_tfrt", b"use_tfrt", "xla_fusion_autotuner_thresh", b"xla_fusion_autotuner_thresh", "xla_prefer_single_graph_cluster", b"xla_prefer_single_graph_cluster"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["backend_server_port", b"backend_server_port", "collective_deterministic_sequential_execution", b"collective_deterministic_sequential_execution", "collective_group_leader", b"collective_group_leader", "collective_nccl", b"collective_nccl", "coordination_config", b"coordination_config", "disable_eager_executor_streaming_enqueue", b"disable_eager_executor_streaming_enqueue", "disable_functional_ops_lowering", b"disable_functional_ops_lowering", "disable_optimize_for_static_graph", b"disable_optimize_for_static_graph", "disable_output_partition_graphs", b"disable_output_partition_graphs", "disable_thread_spinning", b"disable_thread_spinning", "enable_mlir_bridge", b"enable_mlir_bridge", "enable_mlir_graph_optimization", b"enable_mlir_graph_optimization", "enable_multi_host", b"enable_multi_host", "executor_type", b"executor_type", "mlir_bridge_rollout", b"mlir_bridge_rollout", "optimize_for_static_graph", b"optimize_for_static_graph", "recv_buf_max_chunk", b"recv_buf_max_chunk", "session_metadata", b"session_metadata", "share_cluster_devices_in_session", b"share_cluster_devices_in_session", "share_session_state_in_clusterspec_propagation", b"share_session_state_in_clusterspec_propagation", "stream_merge_threshold", b"stream_merge_threshold", "target_gpu", b"target_gpu", "target_tpu", b"target_tpu", "use_numa_affinity", b"use_numa_affinity", "use_tfrt", b"use_tfrt", "xla_fusion_autotuner_thresh", b"xla_fusion_autotuner_thresh", "xla_prefer_single_graph_cluster", b"xla_prefer_single_graph_cluster"]) -> None: ...
 
     DEVICE_COUNT_FIELD_NUMBER: builtins.int
     INTRA_OP_PARALLELISM_THREADS_FIELD_NUMBER: builtins.int
     INTER_OP_PARALLELISM_THREADS_FIELD_NUMBER: builtins.int
     USE_PER_SESSION_THREADS_FIELD_NUMBER: builtins.int
     SESSION_INTER_OP_THREAD_POOL_FIELD_NUMBER: builtins.int
     PLACEMENT_PERIOD_FIELD_NUMBER: builtins.int
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/data_service_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/data_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
+import tensorflow.core.framework.graph_debug_info_pb2
 import tensorflow.core.framework.tensor_pb2
-import tensorflow.core.protobuf.graph_debug_info_pb2
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
@@ -284,25 +284,25 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ID_FIELD_NUMBER: builtins.int
     FILE_LINE_COL_FIELD_NUMBER: builtins.int
     id: builtins.str
     """A unique ID for the stack frame: A UUID-like string."""
     @property
-    def file_line_col(self) -> tensorflow.core.protobuf.graph_debug_info_pb2.GraphDebugInfo.FileLineCol:
+    def file_line_col(self) -> tensorflow.core.framework.graph_debug_info_pb2.GraphDebugInfo.FileLineCol:
         """Stack frame, i.e., a frame of a stack trace, containing information
         regarding the file name, line number, function name, code content
         of the line, and column number (if available).
         """
 
     def __init__(
         self,
         *,
         id: builtins.str | None = ...,
-        file_line_col: tensorflow.core.protobuf.graph_debug_info_pb2.GraphDebugInfo.FileLineCol | None = ...,
+        file_line_col: tensorflow.core.framework.graph_debug_info_pb2.GraphDebugInfo.FileLineCol | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing.Literal["file_line_col", b"file_line_col"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing.Literal["file_line_col", b"file_line_col", "id", b"id"]) -> None: ...
 
 global___StackFrameWithId = StackFrameWithId
 
 @typing.final
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/debug_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/debug_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,17 @@
     """Hash of the regularized (sorted) SignatureDefs."""
     saved_object_graph_hash: builtins.int
     """Hash of the regularized SavedObjectGraph."""
     checkpoint_hash: builtins.int
     """Hash of the checkpoint."""
     @property
     def version(self) -> tensorflow.core.framework.versions_pb2.VersionDef:
-        """Version specification of the fingerprint."""
+        """Version specification of the fingerprint.
+        TODO(b/290068219): add USM version when GA
+        """
 
     def __init__(
         self,
         *,
         saved_model_checksum: builtins.int | None = ...,
         graph_def_program_hash: builtins.int | None = ...,
         signature_def_hash: builtins.int | None = ...,
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/compiler/xla/service/hlo_profile_printer_data_pb2.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,120 +1,149 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
+Copyright 2018 The OpenXLA Authors.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+==============================================================================
 """
 
 import builtins
 import collections.abc
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing.final
-class GraphDebugInfo(google.protobuf.message.Message):
+class HloProfilePrinterData(google.protobuf.message.Message):
+    """Describes how to pretty-print a profile counter array gathered for a specific
+    HloModule.
+    """
+
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing.final
-    class FileLineCol(google.protobuf.message.Message):
-        """This represents a file/line location in the source code."""
+    class HloInstructionInfo(google.protobuf.message.Message):
+        """Pretty-printer information about an HloInstruction."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-        FILE_INDEX_FIELD_NUMBER: builtins.int
-        LINE_FIELD_NUMBER: builtins.int
-        COL_FIELD_NUMBER: builtins.int
-        FUNC_FIELD_NUMBER: builtins.int
-        CODE_FIELD_NUMBER: builtins.int
-        file_index: builtins.int
-        """File name index, which can be used to retrieve the file name string from
-        `files`. The value should be between 0 and (len(files)-1)
+        LONG_NAME_FIELD_NUMBER: builtins.int
+        SHORT_NAME_FIELD_NUMBER: builtins.int
+        CATEGORY_FIELD_NUMBER: builtins.int
+        FLOP_COUNT_FIELD_NUMBER: builtins.int
+        TRANSCENDENTAL_COUNT_FIELD_NUMBER: builtins.int
+        BYTES_ACCESSED_FIELD_NUMBER: builtins.int
+        OPTIMAL_SECONDS_FIELD_NUMBER: builtins.int
+        PROFILE_INDEX_FIELD_NUMBER: builtins.int
+        long_name: builtins.str
+        short_name: builtins.str
+        category: builtins.str
+        flop_count: builtins.float
+        """Metrics computed by HloCostAnalysis."""
+        transcendental_count: builtins.float
+        bytes_accessed: builtins.int
+        optimal_seconds: builtins.float
+        profile_index: builtins.int
+        """The index into the profile counters array for the HloInstruction
+        corresponding to this HloInstructionInfo.
         """
-        line: builtins.int
-        """Line number in the file."""
-        col: builtins.int
-        """Col number in the file line."""
-        func: builtins.str
-        """Name of function contains the file line."""
-        code: builtins.str
-        """Source code contained in this file line."""
         def __init__(
             self,
             *,
-            file_index: builtins.int | None = ...,
-            line: builtins.int | None = ...,
-            col: builtins.int | None = ...,
-            func: builtins.str | None = ...,
-            code: builtins.str | None = ...,
+            long_name: builtins.str | None = ...,
+            short_name: builtins.str | None = ...,
+            category: builtins.str | None = ...,
+            flop_count: builtins.float | None = ...,
+            transcendental_count: builtins.float | None = ...,
+            bytes_accessed: builtins.int | None = ...,
+            optimal_seconds: builtins.float | None = ...,
+            profile_index: builtins.int | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing.Literal["code", b"code", "col", b"col", "file_index", b"file_index", "func", b"func", "line", b"line"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["bytes_accessed", b"bytes_accessed", "category", b"category", "flop_count", b"flop_count", "long_name", b"long_name", "optimal_seconds", b"optimal_seconds", "profile_index", b"profile_index", "short_name", b"short_name", "transcendental_count", b"transcendental_count"]) -> None: ...
 
     @typing.final
-    class StackTrace(google.protobuf.message.Message):
-        """This represents a stack trace which is a ordered list of `FileLineCol`."""
+    class HloComputationInfo(google.protobuf.message.Message):
+        """Pretty-printer information about an HloComputation."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-        FILE_LINE_COLS_FIELD_NUMBER: builtins.int
+        NAME_FIELD_NUMBER: builtins.int
+        PROFILE_INDEX_FIELD_NUMBER: builtins.int
+        INSTRUCTION_INFOS_FIELD_NUMBER: builtins.int
+        name: builtins.str
+        profile_index: builtins.int
+        """The index into the profile counters array for the HloComputation
+        corresponding to this HloComputationInfo.
+        """
         @property
-        def file_line_cols(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___GraphDebugInfo.FileLineCol]:
-            """Each line in the stack trace."""
+        def instruction_infos(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___HloProfilePrinterData.HloInstructionInfo]:
+            """HloInstructionInfos for every HloInstruction in the HloComputation for
+            corresponding to this HloComputattionInfo.
+            """
 
         def __init__(
             self,
             *,
-            file_line_cols: collections.abc.Iterable[global___GraphDebugInfo.FileLineCol] | None = ...,
+            name: builtins.str | None = ...,
+            profile_index: builtins.int | None = ...,
+            instruction_infos: collections.abc.Iterable[global___HloProfilePrinterData.HloInstructionInfo] | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing.Literal["file_line_cols", b"file_line_cols"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["instruction_infos", b"instruction_infos", "name", b"name", "profile_index", b"profile_index"]) -> None: ...
 
     @typing.final
-    class TracesEntry(google.protobuf.message.Message):
+    class ExtraMetricsEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
-        @property
-        def value(self) -> global___GraphDebugInfo.StackTrace: ...
+        value: builtins.int
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
-            value: global___GraphDebugInfo.StackTrace | None = ...,
+            value: builtins.int | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-    FILES_FIELD_NUMBER: builtins.int
-    TRACES_FIELD_NUMBER: builtins.int
+    COMPUTATION_INFOS_FIELD_NUMBER: builtins.int
+    PROFILE_COUNTERS_SIZE_FIELD_NUMBER: builtins.int
+    EXTRA_METRICS_FIELD_NUMBER: builtins.int
+    ENTRY_COMPUTATION_FIELD_NUMBER: builtins.int
+    profile_counters_size: builtins.int
+    """The size of the profile counters array we will pretty-print."""
+    entry_computation: builtins.str
+    """Name of the entry computation."""
     @property
-    def files(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
-        """This stores all the source code file names and can be indexed by the
-        `file_index`.
-        """
+    def computation_infos(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___HloProfilePrinterData.HloComputationInfo]:
+        """HloComputationInfos for every HloComputation in the HloModule."""
 
     @property
-    def traces(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___GraphDebugInfo.StackTrace]:
-        """This maps a node name to a stack trace in the source code.
-        The map key is a mangling of the containing function and op name with
-        syntax:
-          op.name '@' func_name
-        For ops in the top-level graph, the func_name is the empty string.
-        Note that op names are restricted to a small number of characters which
-        exclude '@', making it impossible to collide keys of this form. Function
-        names accept a much wider set of characters.
-        It would be preferable to avoid mangling and use a tuple key of (op.name,
-        func_name), but this is not supported with protocol buffers.
-        """
+    def extra_metrics(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.int]:
+        """Maps extra metric name to the index into the profile counters array."""
 
     def __init__(
         self,
         *,
-        files: collections.abc.Iterable[builtins.str] | None = ...,
-        traces: collections.abc.Mapping[builtins.str, global___GraphDebugInfo.StackTrace] | None = ...,
+        computation_infos: collections.abc.Iterable[global___HloProfilePrinterData.HloComputationInfo] | None = ...,
+        profile_counters_size: builtins.int | None = ...,
+        extra_metrics: collections.abc.Mapping[builtins.str, builtins.int] | None = ...,
+        entry_computation: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing.Literal["files", b"files", "traces", b"traces"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["computation_infos", b"computation_infos", "entry_computation", b"entry_computation", "extra_metrics", b"extra_metrics", "profile_counters_size", b"profile_counters_size"]) -> None: ...
 
-global___GraphDebugInfo = GraphDebugInfo
+global___HloProfilePrinterData = HloProfilePrinterData
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import google.protobuf.any_pb2
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import tensorflow.core.framework.graph_pb2
 import tensorflow.core.framework.op_def_pb2
+import tensorflow.core.framework.tensor_pb2
 import tensorflow.core.framework.tensor_shape_pb2
 import tensorflow.core.framework.types_pb2
 import tensorflow.core.protobuf.saved_object_graph_pb2
 import tensorflow.core.protobuf.saver_pb2
 import tensorflow.core.protobuf.struct_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
@@ -617,17 +618,36 @@
             *,
             key: builtins.str | None = ...,
             value: global___TensorInfo | None = ...,
         ) -> None: ...
         def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
+    @typing.final
+    class DefaultsEntry(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        @property
+        def value(self) -> tensorflow.core.framework.tensor_pb2.TensorProto: ...
+        def __init__(
+            self,
+            *,
+            key: builtins.str | None = ...,
+            value: tensorflow.core.framework.tensor_pb2.TensorProto | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
+
     INPUTS_FIELD_NUMBER: builtins.int
     OUTPUTS_FIELD_NUMBER: builtins.int
     METHOD_NAME_FIELD_NUMBER: builtins.int
+    DEFAULTS_FIELD_NUMBER: builtins.int
     method_name: builtins.str
     """Extensible method_name information enabling third-party users to mark a
     SignatureDef as supporting a particular method. This enables producers and
     consumers of SignatureDefs, e.g. a model definition library and a serving
     library to have a clear hand-off regarding the semantics of a computation.
 
     Note that multiple SignatureDefs in a single MetaGraphDef may have the same
@@ -638,22 +658,27 @@
     def inputs(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___TensorInfo]:
         """Named input parameters."""
 
     @property
     def outputs(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___TensorInfo]:
         """Named output parameters."""
 
+    @property
+    def defaults(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, tensorflow.core.framework.tensor_pb2.TensorProto]:
+        """Named input to corresponding default values if any."""
+
     def __init__(
         self,
         *,
         inputs: collections.abc.Mapping[builtins.str, global___TensorInfo] | None = ...,
         outputs: collections.abc.Mapping[builtins.str, global___TensorInfo] | None = ...,
         method_name: builtins.str | None = ...,
+        defaults: collections.abc.Mapping[builtins.str, tensorflow.core.framework.tensor_pb2.TensorProto] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing.Literal["inputs", b"inputs", "method_name", b"method_name", "outputs", b"outputs"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["defaults", b"defaults", "inputs", b"inputs", "method_name", b"method_name", "outputs", b"outputs"]) -> None: ...
 
 global___SignatureDef = SignatureDef
 
 @typing.final
 class AssetFileDef(google.protobuf.message.Message):
     """An asset file def for a single file or a set of sharded files with the same
     name.
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,78 +1,69 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
+Copyright 2016 The TensorFlow Authors. All Rights Reserved.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+==============================================================================
 """
 
 import builtins
 import collections.abc
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import tensorflow.core.framework.tensor_shape_pb2
-import tensorflow.core.framework.types_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing.final
-class ResourceDtypeAndShape(google.protobuf.message.Message):
+class MemmappedFileSystemDirectoryElement(google.protobuf.message.Message):
+    """A message that describes one region of memmapped file."""
+
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DTYPE_FIELD_NUMBER: builtins.int
-    SHAPE_FIELD_NUMBER: builtins.int
-    dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
-    @property
-    def shape(self) -> tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto: ...
+    OFFSET_FIELD_NUMBER: builtins.int
+    NAME_FIELD_NUMBER: builtins.int
+    LENGTH_FIELD_NUMBER: builtins.int
+    offset: builtins.int
+    name: builtins.str
+    length: builtins.int
     def __init__(
         self,
         *,
-        dtype: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
-        shape: tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto | None = ...,
+        offset: builtins.int | None = ...,
+        name: builtins.str | None = ...,
+        length: builtins.int | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing.Literal["shape", b"shape"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing.Literal["dtype", b"dtype", "shape", b"shape"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["length", b"length", "name", b"name", "offset", b"offset"]) -> None: ...
 
-global___ResourceDtypeAndShape = ResourceDtypeAndShape
+global___MemmappedFileSystemDirectoryElement = MemmappedFileSystemDirectoryElement
 
 @typing.final
-class RemoteTensorHandle(google.protobuf.message.Message):
+class MemmappedFileSystemDirectory(google.protobuf.message.Message):
+    """A directory of regions in a memmapped file."""
+
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    OP_ID_FIELD_NUMBER: builtins.int
-    OUTPUT_NUM_FIELD_NUMBER: builtins.int
-    DEVICE_FIELD_NUMBER: builtins.int
-    OP_DEVICE_FIELD_NUMBER: builtins.int
-    DTYPE_FIELD_NUMBER: builtins.int
-    RESOURCE_DTYPES_AND_SHAPES_FIELD_NUMBER: builtins.int
-    op_id: builtins.int
-    """The ID of the operation that produced this tensor."""
-    output_num: builtins.int
-    """The index into the outputs of the operation that produced this tensor."""
-    device: builtins.str
-    """Device where the tensor is located. Cannot be empty.
-    For multi-device functions, it's the default device passed to placer.
-    """
-    op_device: builtins.str
-    """Device of the operation producing this tensor. Can be empty if the
-    operation producing this tensor is a multi-device function.
-    """
-    dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
-    """Tensor type."""
+    ELEMENT_FIELD_NUMBER: builtins.int
     @property
-    def resource_dtypes_and_shapes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ResourceDtypeAndShape]:
-        """Optional data types and shapes of a remote resource variable."""
-
+    def element(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___MemmappedFileSystemDirectoryElement]: ...
     def __init__(
         self,
         *,
-        op_id: builtins.int | None = ...,
-        output_num: builtins.int | None = ...,
-        device: builtins.str | None = ...,
-        op_device: builtins.str | None = ...,
-        dtype: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
-        resource_dtypes_and_shapes: collections.abc.Iterable[global___ResourceDtypeAndShape] | None = ...,
+        element: collections.abc.Iterable[global___MemmappedFileSystemDirectoryElement] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing.Literal["device", b"device", "dtype", b"dtype", "op_device", b"op_device", "op_id", b"op_id", "output_num", b"output_num", "resource_dtypes_and_shapes", b"resource_dtypes_and_shapes"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["element", b"element"]) -> None: ...
 
-global___RemoteTensorHandle = RemoteTensorHandle
+global___MemmappedFileSystemDirectory = MemmappedFileSystemDirectory
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -262,14 +262,15 @@
     PIN_TO_HOST_OPTIMIZATION_FIELD_NUMBER: builtins.int
     IMPLEMENTATION_SELECTOR_FIELD_NUMBER: builtins.int
     AUTO_MIXED_PRECISION_FIELD_NUMBER: builtins.int
     AUTO_MIXED_PRECISION_MKL_FIELD_NUMBER: builtins.int
     AUTO_MIXED_PRECISION_ONEDNN_BFLOAT16_FIELD_NUMBER: builtins.int
     AUTO_MIXED_PRECISION_CPU_FIELD_NUMBER: builtins.int
     DISABLE_META_OPTIMIZER_FIELD_NUMBER: builtins.int
+    DISABLE_TFG_OPTIMIZER_FIELD_NUMBER: builtins.int
     USE_PLUGIN_OPTIMIZERS_FIELD_NUMBER: builtins.int
     EXPERIMENTAL_CONDITIONAL_CODE_MOTION_FIELD_NUMBER: builtins.int
     META_OPTIMIZER_ITERATIONS_FIELD_NUMBER: builtins.int
     MIN_GRAPH_NODES_FIELD_NUMBER: builtins.int
     EXPERIMENTAL_DISABLE_COMPRESSED_TENSOR_OPTIMIZATION_FIELD_NUMBER: builtins.int
     EXPERIMENTAL_DISABLE_FOLDING_QUANTIZATION_EMULATION_FIELD_NUMBER: builtins.int
     MEMORY_OPTIMIZATION_FIELD_NUMBER: builtins.int
@@ -355,14 +356,16 @@
     This will try to emulate the float16 inputs and outputs of an operator
     on CPU to have better correlation with float16 on GPU; however the
     computation in the operator is based on float32.
     Note that this can change the numerical stability of the graph.
     """
     disable_meta_optimizer: builtins.bool
     """Disable the entire meta optimizer (off by default)."""
+    disable_tfg_optimizer: builtins.bool
+    """Disable the TFG optimizer (off by default)."""
     use_plugin_optimizers: global___RewriterConfig.Toggle.ValueType
     """Optimizers registered by plugin (default is ON)"""
     experimental_conditional_code_motion: global___RewriterConfig.Toggle.ValueType
     """Conditional code motion (default is ON)."""
     meta_optimizer_iterations: global___RewriterConfig.NumIterationsType.ValueType
     """Controls how many times we run the optimizers in meta optimizer (default
     is once).
@@ -467,14 +470,15 @@
         pin_to_host_optimization: global___RewriterConfig.Toggle.ValueType | None = ...,
         implementation_selector: global___RewriterConfig.Toggle.ValueType | None = ...,
         auto_mixed_precision: global___RewriterConfig.Toggle.ValueType | None = ...,
         auto_mixed_precision_mkl: global___RewriterConfig.Toggle.ValueType | None = ...,
         auto_mixed_precision_onednn_bfloat16: global___RewriterConfig.Toggle.ValueType | None = ...,
         auto_mixed_precision_cpu: global___RewriterConfig.Toggle.ValueType | None = ...,
         disable_meta_optimizer: builtins.bool | None = ...,
+        disable_tfg_optimizer: builtins.bool | None = ...,
         use_plugin_optimizers: global___RewriterConfig.Toggle.ValueType | None = ...,
         experimental_conditional_code_motion: global___RewriterConfig.Toggle.ValueType | None = ...,
         meta_optimizer_iterations: global___RewriterConfig.NumIterationsType.ValueType | None = ...,
         min_graph_nodes: builtins.int | None = ...,
         experimental_disable_compressed_tensor_optimization: builtins.bool | None = ...,
         experimental_disable_folding_quantization_emulation: builtins.bool | None = ...,
         memory_optimization: global___RewriterConfig.MemOptType.ValueType | None = ...,
@@ -485,10 +489,10 @@
         scoped_allocator_opts: global___ScopedAllocatorOptions | None = ...,
         optimizers: collections.abc.Iterable[builtins.str] | None = ...,
         custom_optimizers: collections.abc.Iterable[global___RewriterConfig.CustomGraphOptimizer] | None = ...,
         inter_optimizer_verifier_config: tensorflow.core.protobuf.verifier_config_pb2.VerifierConfig | None = ...,
         post_optimization_verifier_config: tensorflow.core.protobuf.verifier_config_pb2.VerifierConfig | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing.Literal["auto_parallel", b"auto_parallel", "inter_optimizer_verifier_config", b"inter_optimizer_verifier_config", "post_optimization_verifier_config", b"post_optimization_verifier_config", "scoped_allocator_opts", b"scoped_allocator_opts"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing.Literal["arithmetic_optimization", b"arithmetic_optimization", "auto_mixed_precision", b"auto_mixed_precision", "auto_mixed_precision_cpu", b"auto_mixed_precision_cpu", "auto_mixed_precision_mkl", b"auto_mixed_precision_mkl", "auto_mixed_precision_onednn_bfloat16", b"auto_mixed_precision_onednn_bfloat16", "auto_parallel", b"auto_parallel", "common_subgraph_elimination", b"common_subgraph_elimination", "constant_folding", b"constant_folding", "cpu_layout_conversion", b"cpu_layout_conversion", "custom_optimizers", b"custom_optimizers", "debug_stripper", b"debug_stripper", "dependency_optimization", b"dependency_optimization", "disable_meta_optimizer", b"disable_meta_optimizer", "disable_model_pruning", b"disable_model_pruning", "experimental_conditional_code_motion", b"experimental_conditional_code_motion", "experimental_disable_compressed_tensor_optimization", b"experimental_disable_compressed_tensor_optimization", "experimental_disable_folding_quantization_emulation", b"experimental_disable_folding_quantization_emulation", "fail_on_optimizer_errors", b"fail_on_optimizer_errors", "function_optimization", b"function_optimization", "implementation_selector", b"implementation_selector", "inter_optimizer_verifier_config", b"inter_optimizer_verifier_config", "layout_optimizer", b"layout_optimizer", "loop_optimization", b"loop_optimization", "memory_optimization", b"memory_optimization", "memory_optimizer_target_node_name_scope", b"memory_optimizer_target_node_name_scope", "meta_optimizer_iterations", b"meta_optimizer_iterations", "meta_optimizer_timeout_ms", b"meta_optimizer_timeout_ms", "min_graph_nodes", b"min_graph_nodes", "optimizers", b"optimizers", "pin_to_host_optimization", b"pin_to_host_optimization", "post_optimization_verifier_config", b"post_optimization_verifier_config", "remapping", b"remapping", "scoped_allocator_optimization", b"scoped_allocator_optimization", "scoped_allocator_opts", b"scoped_allocator_opts", "shape_optimization", b"shape_optimization", "use_plugin_optimizers", b"use_plugin_optimizers"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["arithmetic_optimization", b"arithmetic_optimization", "auto_mixed_precision", b"auto_mixed_precision", "auto_mixed_precision_cpu", b"auto_mixed_precision_cpu", "auto_mixed_precision_mkl", b"auto_mixed_precision_mkl", "auto_mixed_precision_onednn_bfloat16", b"auto_mixed_precision_onednn_bfloat16", "auto_parallel", b"auto_parallel", "common_subgraph_elimination", b"common_subgraph_elimination", "constant_folding", b"constant_folding", "cpu_layout_conversion", b"cpu_layout_conversion", "custom_optimizers", b"custom_optimizers", "debug_stripper", b"debug_stripper", "dependency_optimization", b"dependency_optimization", "disable_meta_optimizer", b"disable_meta_optimizer", "disable_model_pruning", b"disable_model_pruning", "disable_tfg_optimizer", b"disable_tfg_optimizer", "experimental_conditional_code_motion", b"experimental_conditional_code_motion", "experimental_disable_compressed_tensor_optimization", b"experimental_disable_compressed_tensor_optimization", "experimental_disable_folding_quantization_emulation", b"experimental_disable_folding_quantization_emulation", "fail_on_optimizer_errors", b"fail_on_optimizer_errors", "function_optimization", b"function_optimization", "implementation_selector", b"implementation_selector", "inter_optimizer_verifier_config", b"inter_optimizer_verifier_config", "layout_optimizer", b"layout_optimizer", "loop_optimization", b"loop_optimization", "memory_optimization", b"memory_optimization", "memory_optimizer_target_node_name_scope", b"memory_optimizer_target_node_name_scope", "meta_optimizer_iterations", b"meta_optimizer_iterations", "meta_optimizer_timeout_ms", b"meta_optimizer_timeout_ms", "min_graph_nodes", b"min_graph_nodes", "optimizers", b"optimizers", "pin_to_host_optimization", b"pin_to_host_optimization", "post_optimization_verifier_config", b"post_optimization_verifier_config", "remapping", b"remapping", "scoped_allocator_optimization", b"scoped_allocator_optimization", "scoped_allocator_opts", b"scoped_allocator_opts", "shape_optimization", b"shape_optimization", "use_plugin_optimizers", b"use_plugin_optimizers"]) -> None: ...
 
 global___RewriterConfig = RewriterConfig
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/saver_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/saver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/service_config_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/service_config_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -13,29 +13,31 @@
 import tensorflow.core.protobuf.data_service_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing.final
 class DispatcherConfig(google.protobuf.message.Message):
     """Configuration for a tf.data service DispatchServer.
-    Next id: 11
+    Next id: 13
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PORT_FIELD_NUMBER: builtins.int
     PROTOCOL_FIELD_NUMBER: builtins.int
     WORK_DIR_FIELD_NUMBER: builtins.int
     FAULT_TOLERANT_MODE_FIELD_NUMBER: builtins.int
     WORKER_ADDRESSES_FIELD_NUMBER: builtins.int
     DEPLOYMENT_MODE_FIELD_NUMBER: builtins.int
     JOB_GC_CHECK_INTERVAL_MS_FIELD_NUMBER: builtins.int
     JOB_GC_TIMEOUT_MS_FIELD_NUMBER: builtins.int
+    GC_DYNAMIC_SHARDING_JOBS_FIELD_NUMBER: builtins.int
     CLIENT_TIMEOUT_MS_FIELD_NUMBER: builtins.int
     WORKER_TIMEOUT_MS_FIELD_NUMBER: builtins.int
+    WORKER_MAX_CONCURRENT_SNAPSHOTS_FIELD_NUMBER: builtins.int
     port: builtins.int
     """The port for the dispatcher to bind to. A value of 0 indicates that the
     dispatcher may bind to any available port.
     """
     protocol: builtins.str
     """The protocol for the dispatcher to use when connecting to workers."""
     work_dir: builtins.str
@@ -55,25 +57,39 @@
     jobs. A value of 0 indicates that the decision should be left up to the
     runtime.
     """
     job_gc_timeout_ms: builtins.int
     """How long a job needs to be unused before it becomes a candidate for garbage
     collection. A value of -1 indicates that jobs should never be garbage
     collected. A value of 0 indicates that the decision should be left up to
-    the runtime.
+    the runtime. Note: This does not apply to dynamic sharding unless users
+    explicitly opt-in by enabling `gc_dynamic_sharding_jobs` below.
+    """
+    gc_dynamic_sharding_jobs: builtins.bool
+    """Whether dynamically sharded jobs should be eligible for garbage collection.
+    These jobs are not garbage collected by default, since if a job is garbage
+    collected and then re-created, it will revisit all data from the start. If
+    revisiting data is acceptible and you want automatic reclamation of
+    iterator memory, set `gc_dynamic_sharding_jobs` to `true`.
     """
     client_timeout_ms: builtins.int
     """How long to wait before garbage-collecting a client that hasn't
     heartbeated to the dispatcher. A value of 0 indicates that the timeout
     should be left to the runtime.
     """
     worker_timeout_ms: builtins.int
     """How long to wait for a worker to heartbeat before considering it missing.
     A value of 0 indicates that the timeout should be left to the runtime.
     """
+    worker_max_concurrent_snapshots: builtins.int
+    """The maximum number of snapshots that a worker can concurrently process at a
+    given point in time. This is a tradeoff between worker resource usage and
+    snapshot wall time. A value of 0 indicates that the decision should be left
+    up to the runtime.
+    """
     @property
     def worker_addresses(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """(Optional.) If the job uses auto-sharding, it needs to specify a fixed list
         of worker addresses that will register with the dispatcher. The worker
         addresses should be in the format "host" or "host:port", where "port" is an
         integer, named port, or %port% to match any port.
         """
@@ -85,39 +101,42 @@
         protocol: builtins.str | None = ...,
         work_dir: builtins.str | None = ...,
         fault_tolerant_mode: builtins.bool | None = ...,
         worker_addresses: collections.abc.Iterable[builtins.str] | None = ...,
         deployment_mode: tensorflow.core.protobuf.data_service_pb2.DeploymentMode.ValueType | None = ...,
         job_gc_check_interval_ms: builtins.int | None = ...,
         job_gc_timeout_ms: builtins.int | None = ...,
+        gc_dynamic_sharding_jobs: builtins.bool | None = ...,
         client_timeout_ms: builtins.int | None = ...,
         worker_timeout_ms: builtins.int | None = ...,
+        worker_max_concurrent_snapshots: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing.Literal["client_timeout_ms", b"client_timeout_ms", "deployment_mode", b"deployment_mode", "fault_tolerant_mode", b"fault_tolerant_mode", "job_gc_check_interval_ms", b"job_gc_check_interval_ms", "job_gc_timeout_ms", b"job_gc_timeout_ms", "port", b"port", "protocol", b"protocol", "work_dir", b"work_dir", "worker_addresses", b"worker_addresses", "worker_timeout_ms", b"worker_timeout_ms"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["client_timeout_ms", b"client_timeout_ms", "deployment_mode", b"deployment_mode", "fault_tolerant_mode", b"fault_tolerant_mode", "gc_dynamic_sharding_jobs", b"gc_dynamic_sharding_jobs", "job_gc_check_interval_ms", b"job_gc_check_interval_ms", "job_gc_timeout_ms", b"job_gc_timeout_ms", "port", b"port", "protocol", b"protocol", "work_dir", b"work_dir", "worker_addresses", b"worker_addresses", "worker_max_concurrent_snapshots", b"worker_max_concurrent_snapshots", "worker_timeout_ms", b"worker_timeout_ms"]) -> None: ...
 
 global___DispatcherConfig = DispatcherConfig
 
 @typing.final
 class WorkerConfig(google.protobuf.message.Message):
     """Configuration for a tf.data service WorkerServer.
-    Next id: 12
+    Next id: 13
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PORT_FIELD_NUMBER: builtins.int
     PROTOCOL_FIELD_NUMBER: builtins.int
     DISPATCHER_ADDRESS_FIELD_NUMBER: builtins.int
     WORKER_ADDRESS_FIELD_NUMBER: builtins.int
     WORKER_TAGS_FIELD_NUMBER: builtins.int
     HEARTBEAT_INTERVAL_MS_FIELD_NUMBER: builtins.int
     DISPATCHER_TIMEOUT_MS_FIELD_NUMBER: builtins.int
     DATA_TRANSFER_PROTOCOL_FIELD_NUMBER: builtins.int
     DATA_TRANSFER_ADDRESS_FIELD_NUMBER: builtins.int
     CROSS_TRAINER_CACHE_SIZE_BYTES_FIELD_NUMBER: builtins.int
+    SNAPSHOT_MAX_CHUNK_SIZE_BYTES_FIELD_NUMBER: builtins.int
     SHUTDOWN_QUIET_PERIOD_MS_FIELD_NUMBER: builtins.int
     port: builtins.int
     """The port for the worker to bind to. A value of 0 indicates that the
     worker may bind to any available port.
     """
     protocol: builtins.str
     """The protocol for the worker to use when connecting to the dispatcher."""
@@ -144,14 +163,18 @@
     specified, will be replaced with the worker's bound port. This is useful
     when the port is set to `0`.
     """
     cross_trainer_cache_size_bytes: builtins.int
     """Maximum size of the cross-trainer cache in bytes. If enabled, make sure
     your training job provides sufficient memory resources.
     """
+    snapshot_max_chunk_size_bytes: builtins.int
+    """The maximum size of a distributed snapshot chunk file. A value of 0
+    indicates that the decision should be left up to the runtime.
+    """
     shutdown_quiet_period_ms: builtins.int
     """When shutting down a worker, how long to wait for the gRPC server to
     process the final requests. This is used to achieve clean shutdown in unit
     tests.
     """
     @property
     def worker_tags(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
@@ -170,12 +193,13 @@
         worker_address: builtins.str | None = ...,
         worker_tags: collections.abc.Iterable[builtins.str] | None = ...,
         heartbeat_interval_ms: builtins.int | None = ...,
         dispatcher_timeout_ms: builtins.int | None = ...,
         data_transfer_protocol: builtins.str | None = ...,
         data_transfer_address: builtins.str | None = ...,
         cross_trainer_cache_size_bytes: builtins.int | None = ...,
+        snapshot_max_chunk_size_bytes: builtins.int | None = ...,
         shutdown_quiet_period_ms: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing.Literal["cross_trainer_cache_size_bytes", b"cross_trainer_cache_size_bytes", "data_transfer_address", b"data_transfer_address", "data_transfer_protocol", b"data_transfer_protocol", "dispatcher_address", b"dispatcher_address", "dispatcher_timeout_ms", b"dispatcher_timeout_ms", "heartbeat_interval_ms", b"heartbeat_interval_ms", "port", b"port", "protocol", b"protocol", "shutdown_quiet_period_ms", b"shutdown_quiet_period_ms", "worker_address", b"worker_address", "worker_tags", b"worker_tags"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["cross_trainer_cache_size_bytes", b"cross_trainer_cache_size_bytes", "data_transfer_address", b"data_transfer_address", "data_transfer_protocol", b"data_transfer_protocol", "dispatcher_address", b"dispatcher_address", "dispatcher_timeout_ms", b"dispatcher_timeout_ms", "heartbeat_interval_ms", b"heartbeat_interval_ms", "port", b"port", "protocol", b"protocol", "shutdown_quiet_period_ms", b"shutdown_quiet_period_ms", "snapshot_max_chunk_size_bytes", b"snapshot_max_chunk_size_bytes", "worker_address", b"worker_address", "worker_tags", b"worker_tags"]) -> None: ...
 
 global___WorkerConfig = WorkerConfig
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/struct_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/struct_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,16 @@
     TENSOR_SPEC_VALUE_FIELD_NUMBER: builtins.int
     TYPE_SPEC_VALUE_FIELD_NUMBER: builtins.int
     BOUNDED_TENSOR_SPEC_VALUE_FIELD_NUMBER: builtins.int
     LIST_VALUE_FIELD_NUMBER: builtins.int
     TUPLE_VALUE_FIELD_NUMBER: builtins.int
     DICT_VALUE_FIELD_NUMBER: builtins.int
     NAMED_TUPLE_VALUE_FIELD_NUMBER: builtins.int
+    TENSOR_VALUE_FIELD_NUMBER: builtins.int
+    NUMPY_VALUE_FIELD_NUMBER: builtins.int
     float64_value: builtins.float
     """Represents a double-precision floating-point value (a Python `float`)."""
     int64_value: builtins.int
     """Represents a signed integer value, limited to 64 bits.
     Larger values from Python's arbitrary-precision integers are unsupported.
     """
     string_value: builtins.str
@@ -117,14 +119,22 @@
     def dict_value(self) -> global___DictValue:
         """Represents a dict `Value`."""
 
     @property
     def named_tuple_value(self) -> global___NamedTupleValue:
         """Represents Python's namedtuple."""
 
+    @property
+    def tensor_value(self) -> tensorflow.core.framework.tensor_pb2.TensorProto:
+        """Represents a value for tf.Tensor."""
+
+    @property
+    def numpy_value(self) -> tensorflow.core.framework.tensor_pb2.TensorProto:
+        """Represents a value for np.ndarray."""
+
     def __init__(
         self,
         *,
         none_value: global___NoneValue | None = ...,
         float64_value: builtins.float | None = ...,
         int64_value: builtins.int | None = ...,
         string_value: builtins.str | None = ...,
@@ -134,18 +144,20 @@
         tensor_spec_value: global___TensorSpecProto | None = ...,
         type_spec_value: global___TypeSpecProto | None = ...,
         bounded_tensor_spec_value: global___BoundedTensorSpecProto | None = ...,
         list_value: global___ListValue | None = ...,
         tuple_value: global___TupleValue | None = ...,
         dict_value: global___DictValue | None = ...,
         named_tuple_value: global___NamedTupleValue | None = ...,
+        tensor_value: tensorflow.core.framework.tensor_pb2.TensorProto | None = ...,
+        numpy_value: tensorflow.core.framework.tensor_pb2.TensorProto | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing.Literal["bool_value", b"bool_value", "bounded_tensor_spec_value", b"bounded_tensor_spec_value", "dict_value", b"dict_value", "float64_value", b"float64_value", "int64_value", b"int64_value", "kind", b"kind", "list_value", b"list_value", "named_tuple_value", b"named_tuple_value", "none_value", b"none_value", "string_value", b"string_value", "tensor_dtype_value", b"tensor_dtype_value", "tensor_shape_value", b"tensor_shape_value", "tensor_spec_value", b"tensor_spec_value", "tuple_value", b"tuple_value", "type_spec_value", b"type_spec_value"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing.Literal["bool_value", b"bool_value", "bounded_tensor_spec_value", b"bounded_tensor_spec_value", "dict_value", b"dict_value", "float64_value", b"float64_value", "int64_value", b"int64_value", "kind", b"kind", "list_value", b"list_value", "named_tuple_value", b"named_tuple_value", "none_value", b"none_value", "string_value", b"string_value", "tensor_dtype_value", b"tensor_dtype_value", "tensor_shape_value", b"tensor_shape_value", "tensor_spec_value", b"tensor_spec_value", "tuple_value", b"tuple_value", "type_spec_value", b"type_spec_value"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing.Literal["kind", b"kind"]) -> typing.Literal["none_value", "float64_value", "int64_value", "string_value", "bool_value", "tensor_shape_value", "tensor_dtype_value", "tensor_spec_value", "type_spec_value", "bounded_tensor_spec_value", "list_value", "tuple_value", "dict_value", "named_tuple_value"] | None: ...
+    def HasField(self, field_name: typing.Literal["bool_value", b"bool_value", "bounded_tensor_spec_value", b"bounded_tensor_spec_value", "dict_value", b"dict_value", "float64_value", b"float64_value", "int64_value", b"int64_value", "kind", b"kind", "list_value", b"list_value", "named_tuple_value", b"named_tuple_value", "none_value", b"none_value", "numpy_value", b"numpy_value", "string_value", b"string_value", "tensor_dtype_value", b"tensor_dtype_value", "tensor_shape_value", b"tensor_shape_value", "tensor_spec_value", b"tensor_spec_value", "tensor_value", b"tensor_value", "tuple_value", b"tuple_value", "type_spec_value", b"type_spec_value"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["bool_value", b"bool_value", "bounded_tensor_spec_value", b"bounded_tensor_spec_value", "dict_value", b"dict_value", "float64_value", b"float64_value", "int64_value", b"int64_value", "kind", b"kind", "list_value", b"list_value", "named_tuple_value", b"named_tuple_value", "none_value", b"none_value", "numpy_value", b"numpy_value", "string_value", b"string_value", "tensor_dtype_value", b"tensor_dtype_value", "tensor_shape_value", b"tensor_shape_value", "tensor_spec_value", b"tensor_spec_value", "tensor_value", b"tensor_value", "tuple_value", b"tuple_value", "type_spec_value", b"type_spec_value"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["kind", b"kind"]) -> typing.Literal["none_value", "float64_value", "int64_value", "string_value", "bool_value", "tensor_shape_value", "tensor_dtype_value", "tensor_spec_value", "type_spec_value", "bounded_tensor_spec_value", "list_value", "tuple_value", "dict_value", "named_tuple_value", "tensor_value", "numpy_value"] | None: ...
 
 global___StructuredValue = StructuredValue
 
 @typing.final
 class NoneValue(google.protobuf.message.Message):
     """Represents None."""
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -32,25 +32,28 @@
 class ServerDef(google.protobuf.message.Message):
     """Defines the configuration of a single TensorFlow server."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CLUSTER_FIELD_NUMBER: builtins.int
     JOB_NAME_FIELD_NUMBER: builtins.int
+    REPLICA_FIELD_NUMBER: builtins.int
     TASK_INDEX_FIELD_NUMBER: builtins.int
     DEFAULT_SESSION_CONFIG_FIELD_NUMBER: builtins.int
     PROTOCOL_FIELD_NUMBER: builtins.int
     PORT_FIELD_NUMBER: builtins.int
     CLUSTER_DEVICE_FILTERS_FIELD_NUMBER: builtins.int
     job_name: builtins.str
     """The name of the job of which this server is a member.
 
     NOTE(mrry): The `cluster` field must contain a `JobDef` with a `name` field
     that matches this name.
     """
+    replica: builtins.int
+    """Replica this server manages."""
     task_index: builtins.int
     """The task index of this server in its job.
 
     NOTE: The `cluster` field must contain a `JobDef` with a matching `name`
     and a mapping in its `tasks` field for this index.
     """
     protocol: builtins.str
@@ -75,17 +78,18 @@
         """
 
     def __init__(
         self,
         *,
         cluster: tensorflow.core.protobuf.cluster_pb2.ClusterDef | None = ...,
         job_name: builtins.str | None = ...,
+        replica: builtins.int | None = ...,
         task_index: builtins.int | None = ...,
         default_session_config: tensorflow.core.protobuf.config_pb2.ConfigProto | None = ...,
         protocol: builtins.str | None = ...,
         port: builtins.int | None = ...,
         cluster_device_filters: tensorflow.core.protobuf.device_filters_pb2.ClusterDeviceFilters | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing.Literal["cluster", b"cluster", "cluster_device_filters", b"cluster_device_filters", "default_session_config", b"default_session_config"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing.Literal["cluster", b"cluster", "cluster_device_filters", b"cluster_device_filters", "default_session_config", b"default_session_config", "job_name", b"job_name", "port", b"port", "protocol", b"protocol", "task_index", b"task_index"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["cluster", b"cluster", "cluster_device_filters", b"cluster_device_filters", "default_session_config", b"default_session_config", "job_name", b"job_name", "port", b"port", "protocol", b"protocol", "replica", b"replica", "task_index", b"task_index"]) -> None: ...
 
 global___ServerDef = ServerDef
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -389,14 +389,42 @@
         use_nesterov: builtins.bool | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing.Literal["momentum", b"momentum", "use_nesterov", b"use_nesterov"]) -> None: ...
 
 global___MomentumParameters = MomentumParameters
 
 @typing.final
+class LionParameters(google.protobuf.message.Message):
+    """https://www.tensorflow.org/api_docs/python/tf/keras/optimizers/Lion
+    momenta(new) = beta2 * momenta(old) + (1 - beta2) * grad
+    momenta_t = beta1 * momenta(old) + (1 - beta1) * grad
+    var(new) = var(old) - lr * sign(momenta_t)
+    Algorithm described in https://arxiv.org/abs/2302.06675.
+    """
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    BETA1_FIELD_NUMBER: builtins.int
+    BETA2_FIELD_NUMBER: builtins.int
+    USE_NON_LAZY_LION_FIELD_NUMBER: builtins.int
+    beta1: builtins.float
+    beta2: builtins.float
+    use_non_lazy_lion: builtins.bool
+    def __init__(
+        self,
+        *,
+        beta1: builtins.float | None = ...,
+        beta2: builtins.float | None = ...,
+        use_non_lazy_lion: builtins.bool | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing.Literal["beta1", b"beta1", "beta2", b"beta2", "use_non_lazy_lion", b"use_non_lazy_lion"]) -> None: ...
+
+global___LionParameters = LionParameters
+
+@typing.final
 class RmsPropParameters(google.protobuf.message.Message):
     """https://www.tensorflow.org/api_docs/python/tf/keras/optimizers/RMSprop
     https://github.com/tensorflow/tensorflow/blob/6b6471f3ffb7f1fefe42d814aa5fb9ab7a535b58/tensorflow/core/kernels/training_ops.cc#L4229
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -894,14 +922,15 @@
     ADAGRAD_FIELD_NUMBER: builtins.int
     ADAGRAD_MOMENTUM_FIELD_NUMBER: builtins.int
     BOUNDED_ADAGRAD_FIELD_NUMBER: builtins.int
     STOCHASTIC_GRADIENT_DESCENT_FIELD_NUMBER: builtins.int
     FTRL_FIELD_NUMBER: builtins.int
     ADAM_FIELD_NUMBER: builtins.int
     MOMENTUM_FIELD_NUMBER: builtins.int
+    LION_FIELD_NUMBER: builtins.int
     RMS_PROP_FIELD_NUMBER: builtins.int
     CENTERED_RMS_PROP_FIELD_NUMBER: builtins.int
     MDL_ADAGRAD_LIGHT_FIELD_NUMBER: builtins.int
     ADADELTA_FIELD_NUMBER: builtins.int
     PROXIMAL_ADAGRAD_FIELD_NUMBER: builtins.int
     ONLINE_YOGI_FIELD_NUMBER: builtins.int
     PROXIMAL_YOGI_FIELD_NUMBER: builtins.int
@@ -971,14 +1000,16 @@
     @property
     def ftrl(self) -> global___FtrlParameters: ...
     @property
     def adam(self) -> global___AdamParameters: ...
     @property
     def momentum(self) -> global___MomentumParameters: ...
     @property
+    def lion(self) -> global___LionParameters: ...
+    @property
     def rms_prop(self) -> global___RmsPropParameters: ...
     @property
     def centered_rms_prop(self) -> global___CenteredRmsPropParameters: ...
     @property
     def mdl_adagrad_light(self) -> global___MdlAdagradLightParameters: ...
     @property
     def adadelta(self) -> global___AdadeltaParameters: ...
@@ -1009,28 +1040,29 @@
         adagrad: global___AdagradParameters | None = ...,
         adagrad_momentum: global___AdagradMomentumParameters | None = ...,
         bounded_adagrad: global___BoundedAdagradParameters | None = ...,
         stochastic_gradient_descent: global___StochasticGradientDescentParameters | None = ...,
         ftrl: global___FtrlParameters | None = ...,
         adam: global___AdamParameters | None = ...,
         momentum: global___MomentumParameters | None = ...,
+        lion: global___LionParameters | None = ...,
         rms_prop: global___RmsPropParameters | None = ...,
         centered_rms_prop: global___CenteredRmsPropParameters | None = ...,
         mdl_adagrad_light: global___MdlAdagradLightParameters | None = ...,
         adadelta: global___AdadeltaParameters | None = ...,
         proximal_adagrad: global___ProximalAdagradParameters | None = ...,
         online_yogi: global___OnlineYogiParameters | None = ...,
         proximal_yogi: global___ProximalYogiParameters | None = ...,
         frequency_estimator: global___FrequencyEstimatorParameters | None = ...,
         user_defined_program: global___UserDefinedProgramParameters | None = ...,
         assign: global___AssignParameters | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing.Literal["adadelta", b"adadelta", "adagrad", b"adagrad", "adagrad_momentum", b"adagrad_momentum", "adam", b"adam", "assign", b"assign", "bounded_adagrad", b"bounded_adagrad", "centered_rms_prop", b"centered_rms_prop", "clipping_limits", b"clipping_limits", "frequency_estimator", b"frequency_estimator", "ftrl", b"ftrl", "gradient_clipping_limits", b"gradient_clipping_limits", "hot_id_replication_configuration", b"hot_id_replication_configuration", "learning_rate", b"learning_rate", "mdl_adagrad_light", b"mdl_adagrad_light", "momentum", b"momentum", "online_yogi", b"online_yogi", "parameters", b"parameters", "proximal_adagrad", b"proximal_adagrad", "proximal_yogi", b"proximal_yogi", "rms_prop", b"rms_prop", "simulated_quantization", b"simulated_quantization", "stochastic_gradient_descent", b"stochastic_gradient_descent", "user_defined_program", b"user_defined_program"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing.Literal["adadelta", b"adadelta", "adagrad", b"adagrad", "adagrad_momentum", b"adagrad_momentum", "adam", b"adam", "assign", b"assign", "bounded_adagrad", b"bounded_adagrad", "centered_rms_prop", b"centered_rms_prop", "clipping_limits", b"clipping_limits", "frequency_estimator", b"frequency_estimator", "ftrl", b"ftrl", "gradient_accumulation_status", b"gradient_accumulation_status", "gradient_clipping_limits", b"gradient_clipping_limits", "hot_id_replication_configuration", b"hot_id_replication_configuration", "learning_rate", b"learning_rate", "low_dimensional_packing_status", b"low_dimensional_packing_status", "mdl_adagrad_light", b"mdl_adagrad_light", "momentum", b"momentum", "multiply_weight_decay_factor_by_learning_rate", b"multiply_weight_decay_factor_by_learning_rate", "online_yogi", b"online_yogi", "parameters", b"parameters", "proximal_adagrad", b"proximal_adagrad", "proximal_yogi", b"proximal_yogi", "rms_prop", b"rms_prop", "simulated_quantization", b"simulated_quantization", "stochastic_gradient_descent", b"stochastic_gradient_descent", "user_defined_program", b"user_defined_program", "weight_decay_factor", b"weight_decay_factor"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing.Literal["parameters", b"parameters"]) -> typing.Literal["adagrad", "adagrad_momentum", "bounded_adagrad", "stochastic_gradient_descent", "ftrl", "adam", "momentum", "rms_prop", "centered_rms_prop", "mdl_adagrad_light", "adadelta", "proximal_adagrad", "online_yogi", "proximal_yogi", "frequency_estimator", "user_defined_program", "assign"] | None: ...
+    def HasField(self, field_name: typing.Literal["adadelta", b"adadelta", "adagrad", b"adagrad", "adagrad_momentum", b"adagrad_momentum", "adam", b"adam", "assign", b"assign", "bounded_adagrad", b"bounded_adagrad", "centered_rms_prop", b"centered_rms_prop", "clipping_limits", b"clipping_limits", "frequency_estimator", b"frequency_estimator", "ftrl", b"ftrl", "gradient_clipping_limits", b"gradient_clipping_limits", "hot_id_replication_configuration", b"hot_id_replication_configuration", "learning_rate", b"learning_rate", "lion", b"lion", "mdl_adagrad_light", b"mdl_adagrad_light", "momentum", b"momentum", "online_yogi", b"online_yogi", "parameters", b"parameters", "proximal_adagrad", b"proximal_adagrad", "proximal_yogi", b"proximal_yogi", "rms_prop", b"rms_prop", "simulated_quantization", b"simulated_quantization", "stochastic_gradient_descent", b"stochastic_gradient_descent", "user_defined_program", b"user_defined_program"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["adadelta", b"adadelta", "adagrad", b"adagrad", "adagrad_momentum", b"adagrad_momentum", "adam", b"adam", "assign", b"assign", "bounded_adagrad", b"bounded_adagrad", "centered_rms_prop", b"centered_rms_prop", "clipping_limits", b"clipping_limits", "frequency_estimator", b"frequency_estimator", "ftrl", b"ftrl", "gradient_accumulation_status", b"gradient_accumulation_status", "gradient_clipping_limits", b"gradient_clipping_limits", "hot_id_replication_configuration", b"hot_id_replication_configuration", "learning_rate", b"learning_rate", "lion", b"lion", "low_dimensional_packing_status", b"low_dimensional_packing_status", "mdl_adagrad_light", b"mdl_adagrad_light", "momentum", b"momentum", "multiply_weight_decay_factor_by_learning_rate", b"multiply_weight_decay_factor_by_learning_rate", "online_yogi", b"online_yogi", "parameters", b"parameters", "proximal_adagrad", b"proximal_adagrad", "proximal_yogi", b"proximal_yogi", "rms_prop", b"rms_prop", "simulated_quantization", b"simulated_quantization", "stochastic_gradient_descent", b"stochastic_gradient_descent", "user_defined_program", b"user_defined_program", "weight_decay_factor", b"weight_decay_factor"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["parameters", b"parameters"]) -> typing.Literal["adagrad", "adagrad_momentum", "bounded_adagrad", "stochastic_gradient_descent", "ftrl", "adam", "momentum", "lion", "rms_prop", "centered_rms_prop", "mdl_adagrad_light", "adadelta", "proximal_adagrad", "online_yogi", "proximal_yogi", "frequency_estimator", "user_defined_program", "assign"] | None: ...
 
 global___OptimizationParameters = OptimizationParameters
 
 @typing.final
 class StateVariableSpecification(google.protobuf.message.Message):
     """Specification of an optimization algorithm's state variables (both the main
     value vector and any extra accumulators, etc.). This proto is only used
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -58,21 +58,25 @@
     V2: TPUHardwareFeature.EmbeddingFeature.ValueType  # 2
     """Embedding lookup accelerator V2. The embedding lookup operation can be
     placed anywhere of the computation. Multiple instances of embedding
     lookup layer is allowed.
     """
 
     EMBEDDING_FEATURE_FIELD_NUMBER: builtins.int
+    NUM_EMBEDDING_DEVICES_PER_CHIP_FIELD_NUMBER: builtins.int
     embedding_feature: global___TPUHardwareFeature.EmbeddingFeature.ValueType
+    num_embedding_devices_per_chip: builtins.int
+    """Number of embedding accelerator devices per chip."""
     def __init__(
         self,
         *,
         embedding_feature: global___TPUHardwareFeature.EmbeddingFeature.ValueType | None = ...,
+        num_embedding_devices_per_chip: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing.Literal["embedding_feature", b"embedding_feature"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["embedding_feature", b"embedding_feature", "num_embedding_devices_per_chip", b"num_embedding_devices_per_chip"]) -> None: ...
 
 global___TPUHardwareFeature = TPUHardwareFeature
 
 @typing.final
 class TopologyProto(google.protobuf.message.Message):
     """Describes the geometry of a TPU mesh."""
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/util/event_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/util/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/compiler/xla/service/test_compilation_environment_pb2.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
-Copyright 2016 The TensorFlow Authors. All Rights Reserved.
+Copyright 2022 The OpenXLA Authors.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
 http://www.apache.org/licenses/LICENSE-2.0
 
@@ -14,56 +14,58 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ==============================================================================
 """
 
 import builtins
-import collections.abc
 import typing
 
 import google.protobuf.descriptor
-import google.protobuf.internal.containers
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing.final
-class MemmappedFileSystemDirectoryElement(google.protobuf.message.Message):
-    """A message that describes one region of memmapped file."""
-
+class TestCompilationEnvironment1(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    OFFSET_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
-    LENGTH_FIELD_NUMBER: builtins.int
-    offset: builtins.int
-    name: builtins.str
-    length: builtins.int
+    SOME_FLAG_FIELD_NUMBER: builtins.int
+    some_flag: builtins.int
     def __init__(
         self,
         *,
-        offset: builtins.int | None = ...,
-        name: builtins.str | None = ...,
-        length: builtins.int | None = ...,
+        some_flag: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing.Literal["length", b"length", "name", b"name", "offset", b"offset"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["some_flag", b"some_flag"]) -> None: ...
 
-global___MemmappedFileSystemDirectoryElement = MemmappedFileSystemDirectoryElement
+global___TestCompilationEnvironment1 = TestCompilationEnvironment1
 
 @typing.final
-class MemmappedFileSystemDirectory(google.protobuf.message.Message):
-    """A directory of regions in a memmapped file."""
+class TestCompilationEnvironment2(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    SOME_OTHER_FLAG_FIELD_NUMBER: builtins.int
+    some_other_flag: builtins.int
+    def __init__(
+        self,
+        *,
+        some_other_flag: builtins.int | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing.Literal["some_other_flag", b"some_other_flag"]) -> None: ...
+
+global___TestCompilationEnvironment2 = TestCompilationEnvironment2
+
+@typing.final
+class TestCompilationEnvironment3(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ELEMENT_FIELD_NUMBER: builtins.int
-    @property
-    def element(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___MemmappedFileSystemDirectoryElement]: ...
+    A_THIRD_FLAG_FIELD_NUMBER: builtins.int
+    a_third_flag: builtins.int
     def __init__(
         self,
         *,
-        element: collections.abc.Iterable[global___MemmappedFileSystemDirectoryElement] | None = ...,
+        a_third_flag: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing.Literal["element", b"element"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["a_third_flag", b"a_third_flag"]) -> None: ...
 
-global___MemmappedFileSystemDirectory = MemmappedFileSystemDirectory
+global___TestCompilationEnvironment3 = TestCompilationEnvironment3
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/core/util/test_log_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/util/test_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/data/__init__.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/data/experimental.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/data/experimental.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/dtypes.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/dtypes.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/experimental/dtensor.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/experimental/dtensor.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/feature_column/__init__.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/feature_column/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/io/__init__.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/io/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,17 @@
         key: str
 
     class UniformRowLength(NamedTuple):  # type: ignore[misc]
         length: int
 
     dtype: DTypeLike
     value_key: str | None = ...
-    partitions: tuple[RowSplits | RowLengths | RowStarts | RowLimits | ValueRowIds | UniformRowLength, ...] = ...  # type: ignore[name-defined]
+    partitions: tuple[  # type: ignore[name-defined]
+        RowSplits | RowLengths | RowStarts | RowLimits | ValueRowIds | UniformRowLength, ...
+    ] = ...
     row_splits_dtype: DTypeLike = ...
     validate: bool = ...
 
 def parse_example(
     serialized: TensorCompatible, features: _FeatureSpecs, example_names: Iterable[str] | None = None, name: str | None = None
 ) -> dict[str, TensorLike]: ...
 def __getattr__(name: str) -> Incomplete: ...
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/io/gfile.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/io/gfile.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/activations.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/activations.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -7,31 +7,29 @@
 from tensorflow._aliases import FloatArray, FloatDataSequence, FloatTensorCompatible, Integer
 
 # The implementation uses isinstance so it must be dict and not any Mapping.
 _Activation: TypeAlias = str | None | Callable[[Tensor], Tensor] | dict[str, Any]
 # Ints are not allowed.
 _ActivationInput: TypeAlias = Tensor | FloatDataSequence | FloatArray | np.number[Any] | float
 
-def deserialize(
-    name: str, custom_objects: dict[str, Callable[..., Any]] | None = None, use_legacy_format: bool = False
-) -> Callable[..., Any]: ...
+def deserialize(config: dict[str, Any], custom_objects: dict[str, Callable[..., Any]] | None = None) -> Callable[..., Any]: ...
 def elu(x: _ActivationInput, alpha: FloatTensorCompatible | FloatDataSequence = 1.0) -> Tensor: ...
 def exponential(x: _ActivationInput) -> Tensor: ...
 def gelu(x: _ActivationInput, approximate: bool = False) -> Tensor: ...
 def get(identifier: _Activation) -> Callable[[Tensor], Tensor]: ...
 def hard_sigmoid(x: _ActivationInput) -> Tensor: ...
 def linear(x: _ActivationInput) -> Tensor: ...
 def mish(x: _ActivationInput) -> Tensor: ...
 def relu(
     x: _ActivationInput,
-    alpha: FloatTensorCompatible = 0.0,
+    negative_slope: FloatTensorCompatible = 0.0,
     max_value: FloatTensorCompatible | FloatDataSequence | None = None,
     threshold: FloatTensorCompatible | FloatDataSequence = 0.0,
 ) -> Tensor: ...
 def selu(x: _ActivationInput) -> Tensor: ...
-def serialize(activation: Callable[..., Any], use_legacy_format: bool = False) -> str | dict[str, Any]: ...
+def serialize(activation: Callable[..., Any]) -> str | dict[str, Any]: ...
 def sigmoid(x: _ActivationInput) -> Tensor: ...
 def softmax(x: Tensor, axis: Integer = -1) -> Tensor: ...
 def softplus(x: _ActivationInput) -> Tensor: ...
 def softsign(x: _ActivationInput) -> Tensor: ...
 def swish(x: _ActivationInput) -> Tensor: ...
 def tanh(x: _ActivationInput) -> Tensor: ...
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/callbacks.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/callbacks.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,81 +1,73 @@
-from collections.abc import Callable, Iterable, Mapping, Sequence
+from collections.abc import Callable, Mapping, Sequence
 from typing import Any, Literal
 from typing_extensions import TypeAlias
 
 import tensorflow as tf
 from requests.api import _HeadersMapping
 from tensorflow.keras import Model
 from tensorflow.keras.optimizers.schedules import LearningRateSchedule
-from tensorflow.saved_model import SaveOptions
-from tensorflow.train import CheckpointOptions
 
 _Logs: TypeAlias = Mapping[str, Any] | None | Any
 
 class Callback:
-    model: Model[Any, Any]
     params: dict[str, Any]
-    def set_model(self, model: Model[Any, Any]) -> None: ...
     def set_params(self, params: dict[str, Any]) -> None: ...
+    def set_model(self, model: Model[Any, Any]) -> None: ...
+    @property
+    def model(self) -> Model[Any, Any]: ...
     def on_batch_begin(self, batch: int, logs: _Logs = None) -> None: ...
     def on_batch_end(self, batch: int, logs: _Logs = None) -> None: ...
     def on_epoch_begin(self, epoch: int, logs: _Logs = None) -> None: ...
     def on_epoch_end(self, epoch: int, logs: _Logs = None) -> None: ...
-    def on_predict_batch_begin(self, batch: int, logs: _Logs = None) -> None: ...
-    def on_predict_batch_end(self, batch: int, logs: _Logs = None) -> None: ...
-    def on_predict_begin(self, logs: _Logs = None) -> None: ...
-    def on_predict_end(self, logs: _Logs = None) -> None: ...
-    def on_test_batch_begin(self, batch: int, logs: _Logs = None) -> None: ...
-    def on_test_batch_end(self, batch: int, logs: _Logs = None) -> None: ...
-    def on_test_begin(self, logs: _Logs = None) -> None: ...
-    def on_test_end(self, logs: _Logs = None) -> None: ...
     def on_train_batch_begin(self, batch: int, logs: _Logs = None) -> None: ...
     def on_train_batch_end(self, batch: int, logs: _Logs = None) -> None: ...
+    def on_test_batch_begin(self, batch: int, logs: _Logs = None) -> None: ...
+    def on_test_batch_end(self, batch: int, logs: _Logs = None) -> None: ...
+    def on_predict_batch_begin(self, batch: int, logs: _Logs = None) -> None: ...
+    def on_predict_batch_end(self, batch: int, logs: _Logs = None) -> None: ...
     def on_train_begin(self, logs: _Logs = None) -> None: ...
     def on_train_end(self, logs: _Logs = None) -> None: ...
+    def on_test_begin(self, logs: _Logs = None) -> None: ...
+    def on_test_end(self, logs: _Logs = None) -> None: ...
+    def on_predict_begin(self, logs: _Logs = None) -> None: ...
+    def on_predict_end(self, logs: _Logs = None) -> None: ...
 
-# A CallbackList has exact same api as a callback, but does not actually subclass it.
-class CallbackList:
-    model: Model[Any, Any]
-    params: dict[str, Any]
+class CallbackList(Callback):
     def __init__(
         self,
         callbacks: Sequence[Callback] | None = None,
         add_history: bool = False,
         add_progbar: bool = False,
         # model: Model[Any, object] | None = None,
         model: Model[Any, Any] | None = None,
         **params: Any,
     ) -> None: ...
-    def set_model(self, model: Model[Any, Any]) -> None: ...
+    def append(self, callback: Callback) -> None: ...
     def set_params(self, params: dict[str, Any]) -> None: ...
-    def on_batch_begin(self, batch: int, logs: _Logs | None = None) -> None: ...
-    def on_batch_end(self, batch: int, logs: _Logs | None = None) -> None: ...
-    def on_epoch_begin(self, epoch: int, logs: _Logs | None = None) -> None: ...
-    def on_epoch_end(self, epoch: int, logs: _Logs | None = None) -> None: ...
-    def on_predict_batch_begin(self, batch: int, logs: _Logs | None = None) -> None: ...
-    def on_predict_batch_end(self, batch: int, logs: _Logs | None = None) -> None: ...
-    def on_predict_begin(self, logs: _Logs | None = None) -> None: ...
-    def on_predict_end(self, logs: _Logs | None = None) -> None: ...
-    def on_test_batch_begin(self, batch: int, logs: _Logs | None = None) -> None: ...
-    def on_test_batch_end(self, batch: int, logs: _Logs | None = None) -> None: ...
-    def on_test_begin(self, logs: _Logs | None = None) -> None: ...
-    def on_test_end(self, logs: _Logs | None = None) -> None: ...
-    def on_train_batch_begin(self, batch: int, logs: _Logs | None = None) -> None: ...
-    def on_train_batch_end(self, batch: int, logs: _Logs | None = None) -> None: ...
-    def on_train_begin(self, logs: _Logs | None = None) -> None: ...
-    def on_train_end(self, logs: _Logs | None = None) -> None: ...
+    def set_model(self, model: Model[Any, Any]) -> None: ...
+    def on_batch_begin(self, batch: int, logs: _Logs = None) -> None: ...
+    def on_batch_end(self, batch: int, logs: _Logs = None) -> None: ...
+    def on_epoch_begin(self, epoch: int, logs: _Logs = None) -> None: ...
+    def on_epoch_end(self, epoch: int, logs: _Logs = None) -> None: ...
+    def on_train_batch_begin(self, batch: int, logs: _Logs = None) -> None: ...
+    def on_train_batch_end(self, batch: int, logs: _Logs = None) -> None: ...
+    def on_test_batch_begin(self, batch: int, logs: _Logs = None) -> None: ...
+    def on_test_batch_end(self, batch: int, logs: _Logs = None) -> None: ...
+    def on_predict_batch_begin(self, batch: int, logs: _Logs = None) -> None: ...
+    def on_predict_batch_end(self, batch: int, logs: _Logs = None) -> None: ...
+    def on_train_begin(self, logs: _Logs = None) -> None: ...
+    def on_train_end(self, logs: _Logs = None) -> None: ...
+    def on_test_begin(self, logs: _Logs = None) -> None: ...
+    def on_test_end(self, logs: _Logs = None) -> None: ...
+    def on_predict_begin(self, logs: _Logs = None) -> None: ...
+    def on_predict_end(self, logs: _Logs = None) -> None: ...
 
 class BackupAndRestore(Callback):
-    def __init__(
-        self, backup_dir: str, save_freq: str = "epoch", delete_checkpoint: bool = True, save_before_preemption: bool = False
-    ) -> None: ...
-
-class BaseLogger(Callback):
-    def __init__(self, stateful_metrics: Iterable[str] | None = None) -> None: ...
+    def __init__(self, backup_dir: str, save_freq: str = "epoch", delete_checkpoint: bool = True) -> None: ...
 
 class CSVLogger(Callback):
     def __init__(self, filename: str, separator: str = ",", append: bool = False) -> None: ...
 
 class EarlyStopping(Callback):
     monitor_op: Any
     def __init__(
@@ -94,63 +86,59 @@
     history: dict[str, list[Any]]
 
 class LambdaCallback(Callback):
     def __init__(
         self,
         on_epoch_begin: Callable[[int, _Logs], object] | None = None,
         on_epoch_end: Callable[[int, _Logs], object] | None = None,
-        on_batch_begin: Callable[[int, _Logs], object] | None = None,
-        on_batch_end: Callable[[int, _Logs], object] | None = None,
         on_train_begin: Callable[[_Logs], object] | None = None,
         on_train_end: Callable[[_Logs], object] | None = None,
+        on_train_batch_begin: Callable[[int, _Logs], object] | None = None,
+        on_train_batch_end: Callable[[int, _Logs], object] | None = None,
         **kwargs: Any,
     ) -> None: ...
 
 class LearningRateScheduler(Callback):
     def __init__(
         self,
         schedule: LearningRateSchedule | Callable[[int], float | tf.Tensor] | Callable[[int, float], float | tf.Tensor],
         verbose: Literal[0, 1] = 0,
     ) -> None: ...
 
 class ModelCheckpoint(Callback):
     monitor_op: Any
     filepath: str
-    _options: CheckpointOptions | SaveOptions | None
     def __init__(
         self,
         filepath: str,
         monitor: str = "val_loss",
         verbose: Literal[0, 1] = 0,
         save_best_only: bool = False,
         save_weights_only: bool = False,
         mode: Literal["auto", "min", "max"] = "auto",
         save_freq: str | int = "epoch",
-        options: CheckpointOptions | SaveOptions | None = None,
         initial_value_threshold: float | None = None,
     ) -> None: ...
     def _save_model(self, epoch: int, batch: int | None, logs: _Logs) -> None: ...
 
 class ProgbarLogger(Callback):
     use_steps: bool
-    def __init__(
-        self, count_mode: Literal["steps", "samples"] = "samples", stateful_metrics: Iterable[str] | None = None
-    ) -> None: ...
+    def __init__(self) -> None: ...
 
 class ReduceLROnPlateau(Callback):
     def __init__(
         self,
         monitor: str = "val_loss",
         factor: float = 0.1,
         patience: int = 10,
         verbose: Literal[0, 1] = 0,
         mode: Literal["auto", "min", "max"] = "auto",
         min_delta: float = 1e-4,
         cooldown: int = 0,
-        min_lr: float = 0,
+        min_lr: float = 0.0,
         **kwargs,
     ) -> None: ...
     def in_cooldown(self) -> bool: ...
 
 class RemoteMonitor(Callback):
     def __init__(
         self,
@@ -172,13 +160,12 @@
         write_graph: bool = True,
         write_images: bool = False,
         write_steps_per_second: bool = False,
         update_freq: int | Literal["epoch"] = "epoch",
         profile_batch: int | tuple[int, int] = 0,
         embeddings_freq: int = 0,
         embeddings_metadata: dict[str, None] | None = None,
-        **kwargs: Any,
     ) -> None: ...
     def _write_keras_model_train_graph(self) -> None: ...
     def _stop_trace(self, batch: int | None = None) -> None: ...
 
 class TerminateOnNaN(Callback): ...
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/constraints.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/constraints.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/initializers.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/initializers.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class Initializer:
     def __call__(self, shape: ShapeLike, dtype: DTypeLike | None = None) -> Tensor: ...
     def get_config(self) -> dict[str, Any]: ...
     @classmethod
     def from_config(cls, config: dict[str, Any]) -> Self: ...
 
 class Constant(Initializer):
-    def __init__(self, value: TensorCompatible = 0) -> None: ...
+    def __init__(self, value: TensorCompatible = 0.0) -> None: ...
 
 class GlorotNormal(Initializer):
     def __init__(self, seed: int | None = None) -> None: ...
 
 class GlorotUniform(Initializer):
     def __init__(self, seed: int | None = None) -> None: ...
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/layers/__init__.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/layers/__init__.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from _typeshed import Incomplete
-from collections.abc import Callable, Iterable, Mapping, Sequence
-from typing import Any, Generic, Literal, TypeVar, overload
+from collections.abc import Callable, Iterable, Sequence
+from typing import Any, Generic, Literal, TypeVar, overload, type_check_only
 from typing_extensions import Self, TypeAlias
 
 import tensorflow as tf
-from tensorflow import Tensor, Variable, VariableAggregation, VariableSynchronization
-from tensorflow._aliases import AnyArray, DTypeLike, TensorCompatible, TensorLike
+from tensorflow import Tensor, Variable
+from tensorflow._aliases import AnyArray, DataSequence, DTypeLike, Float, TensorCompatible, TensorLike
 from tensorflow.keras.activations import _Activation
 from tensorflow.keras.constraints import Constraint
 from tensorflow.keras.initializers import _Initializer
-from tensorflow.keras.layers.preprocessing import IntegerLookup as IntegerLookup, StringLookup as StringLookup
 from tensorflow.keras.regularizers import Regularizer, _Regularizer
-from tensorflow.python.feature_column.feature_column_v2 import DenseColumn, SequenceDenseColumn
 
 _InputT = TypeVar("_InputT", contravariant=True)
 _OutputT = TypeVar("_OutputT", covariant=True)
 
 class InputSpec:
     dtype: str | None
     shape: tuple[int | None, ...]
@@ -47,15 +45,24 @@
     input_spec: InputSpec | Any
 
     @property
     def trainable(self) -> bool: ...
     @trainable.setter
     def trainable(self, value: bool) -> None: ...
     def __init__(
-        self, trainable: bool = True, name: str | None = None, dtype: DTypeLike | None = None, dynamic: bool = False
+        self,
+        *,
+        activity_regularizer: _Regularizer = None,
+        trainable: bool = True,
+        dtype: DTypeLike | None = None,
+        autocast: bool = True,
+        name: str | None = None,
+        # **kwargs
+        input_dim: int | None = None,
+        input_shape: Any = None,
     ) -> None: ...
 
     # *args/**kwargs are allowed, but have obscure footguns and tensorflow documentation discourages their usage.
     # First argument will automatically be cast to layer's compute dtype, but any other tensor arguments will not be.
     # Also various tensorflow tools/apis can misbehave if they encounter a layer with *args/**kwargs.
     def __call__(self, inputs: _InputT, *, training: bool = False, mask: TensorCompatible | None = None) -> _OutputT: ...
     def call(self, inputs: _InputT, /) -> _OutputT: ...
@@ -65,26 +72,25 @@
     def build(self, input_shape: Any, /) -> None: ...
     @overload
     def compute_output_shape(self: Layer[tf.Tensor, tf.Tensor], input_shape: tf.TensorShape, /) -> tf.TensorShape: ...
     @overload
     def compute_output_shape(self, input_shape: Any, /) -> Any: ...
     def add_weight(
         self,
-        name: str | None = None,
         shape: Iterable[int | None] | None = None,
-        dtype: DTypeLike | None = None,
         initializer: _Initializer | None = None,
+        dtype: DTypeLike | None = None,
+        trainable: bool = True,
+        autocast: bool = True,
         regularizer: _Regularizer = None,
-        trainable: bool | None = None,
         constraint: _Constraint = None,
-        use_resource: bool | None = None,
-        synchronization: VariableSynchronization = ...,
-        aggregation: VariableAggregation = ...,
+        aggregation: Literal["mean", "sum", "only_first_replica"] = "mean",
+        name: str | None = None,
     ) -> tf.Variable: ...
-    def add_loss(self, losses: tf.Tensor | Sequence[tf.Tensor] | Callable[[], tf.Tensor]) -> None: ...
+    def add_loss(self, loss: tf.Tensor | Sequence[tf.Tensor] | Callable[[], tf.Tensor]) -> None: ...
     def count_params(self) -> int: ...
     @property
     def trainable_variables(self) -> list[Variable]: ...
     @property
     def non_trainable_variables(self) -> list[Variable]: ...
     @property
     def trainable_weights(self) -> list[Variable]: ...
@@ -108,14 +114,97 @@
 # all layer constructors.
 
 # TODO: Replace last Any after adding tf.keras.mixed_precision.Policy.
 _LayerDtype: TypeAlias = DTypeLike | dict[str, Any] | Any
 
 _Constraint: TypeAlias = str | dict[str, Any] | Constraint | None
 
+# IndexLookup is not exported by Keras
+@type_check_only
+class _IndexLookup(Layer[tf.Tensor, tf.Tensor]):
+    def __init__(
+        self,
+        max_tokens: int | None,
+        num_oov_indices: int,
+        mask_token: str | None,
+        oov_token: str,
+        vocabulary_dtype: Literal["int64", "string"],
+        vocabulary: str | None | TensorCompatible = None,
+        idf_weights: TensorCompatible | None = None,
+        invert: bool = False,
+        output_mode: Literal["int", "count", "multi_hot", "one_hot", "tf_idf"] = "int",
+        sparse: bool = False,
+        pad_to_max_tokens: bool = False,
+        name: str | None = None,
+        *,
+        # **kwargs
+        vocabulary_size: int | None = None,
+        has_input_vocabulary: bool = ...,
+        trainable: bool | None = None,
+        dtype: _LayerDtype | None = None,
+        # **kwargs passed to Layer
+        activity_regularizer: _Regularizer = None,
+        autocast: bool = True,
+    ) -> None: ...
+    def compute_output_signature(self, input_spec) -> tf.TensorSpec: ...
+    def get_vocabulary(self, include_special_tokens: bool = True) -> list[Incomplete]: ...
+    def vocabulary_size(self) -> int: ...
+
+class StringLookup(_IndexLookup):
+    def __init__(
+        self,
+        max_tokens: int | None = None,
+        num_oov_indices: int = 1,
+        mask_token: str | None = None,
+        oov_token: str = "[UNK]",
+        vocabulary: str | None | TensorCompatible = None,
+        idf_weights: TensorCompatible | None = None,
+        invert: bool = False,
+        output_mode: Literal["int", "count", "multi_hot", "one_hot", "tf_idf"] = "int",
+        pad_to_max_tokens: bool = False,
+        sparse: bool = False,
+        encoding: str = "utf-8",
+        name: str | None = None,
+        *,
+        # **kwargs passed to IndexLookup
+        vocabulary_size: int | None = None,
+        has_input_vocabulary: bool = ...,
+        trainable: bool | None = None,
+        dtype: _LayerDtype | None = None,
+        activity_regularizer: _Regularizer = None,
+        autocast: bool = True,
+    ) -> None: ...
+    def adapt(self, data: tf.data.Dataset[TensorLike] | AnyArray | DataSequence, steps: Float | None = None) -> None: ...
+
+class IntegerLookup(_IndexLookup):
+    def __init__(
+        self,
+        max_tokens: int | None = None,
+        num_oov_indices: int = 1,
+        mask_token: int | None = None,
+        oov_token: int = -1,
+        vocabulary: str | None | TensorCompatible = None,
+        vocabulary_dtype: Literal["int64"] = "int64",
+        idf_weights: TensorCompatible | None = None,
+        invert: bool = False,
+        output_mode: Literal["int", "count", "multi_hot", "one_hot", "tf_idf"] = "int",
+        sparse: bool = False,
+        pad_to_max_tokens: bool = False,
+        name: str | None = None,
+        *,
+        # **kwargs passed to IndexLookup
+        vocabulary_size: int | None = None,
+        has_input_vocabulary: bool = ...,
+        trainable: bool | None = None,
+        dtype: _LayerDtype | None = None,
+        activity_regularizer: _Regularizer = None,
+        autocast: bool = True,
+    ) -> None: ...
+    def adapt(self, data: tf.data.Dataset[TensorLike] | AnyArray | DataSequence, steps: Float | None = None) -> None: ...
+
 # Layer's compute_output_shape commonly have instance as first argument name instead of self.
 # This is an artifact of actual implementation commonly uses a decorator to define it.
 # Layer.build has same weirdness sometimes. For both marked as positional only.
 class Dense(Layer[tf.Tensor, tf.Tensor]):
     def __init__(
         self,
         units: int,
@@ -124,17 +213,20 @@
         kernel_initializer: _Initializer = "glorot_uniform",
         bias_initializer: _Initializer = "zeros",
         kernel_regularizer: _Regularizer = None,
         bias_regularizer: _Regularizer = None,
         activity_regularizer: _Regularizer = None,
         kernel_constraint: _Constraint = None,
         bias_constraint: _Constraint = None,
+        lora_rank: int | None = None,
+        *,
+        # **kwargs passed to Layer
         trainable: bool = True,
         dtype: _LayerDtype | None = None,
-        dynamic: bool = False,
+        autocast: bool = True,
         name: str | None = None,
     ) -> None: ...
 
 class BatchNormalization(Layer[tf.Tensor, tf.Tensor]):
     def __init__(
         self,
         axis: int = -1,
@@ -146,57 +238,71 @@
         gamma_initializer: _Initializer = "ones",
         moving_mean_initializer: _Initializer = "zeros",
         moving_variance_initializer: _Initializer = "ones",
         beta_regularizer: _Regularizer = None,
         gamma_regularizer: _Regularizer = None,
         beta_constraint: _Constraint = None,
         gamma_constraint: _Constraint = None,
+        synchronized: bool = False,
+        *,
+        # **kwargs passed to Layer
+        activity_regularizer: _Regularizer = None,
         trainable: bool = True,
         dtype: _LayerDtype | None = None,
-        dynamic: bool = False,
+        autocast: bool = True,
         name: str | None = None,
     ) -> None: ...
 
 class ReLU(Layer[tf.Tensor, tf.Tensor]):
     def __init__(
         self,
         max_value: float | None = None,
         negative_slope: float | None = 0.0,
         threshold: float | None = 0.0,
+        *,
+        # **kwargs passed to Layer
+        activity_regularizer: _Regularizer = None,
         trainable: bool = True,
         dtype: _LayerDtype | None = None,
-        dynamic: bool = False,
+        autocast: bool = True,
         name: str | None = None,
     ) -> None: ...
 
 class Dropout(Layer[tf.Tensor, tf.Tensor]):
     def __init__(
         self,
         rate: float,
         noise_shape: TensorCompatible | Sequence[int | None] | None = None,
         seed: int | None = None,
+        *,
+        # **kwargs passed to Layer
+        activity_regularizer: _Regularizer = None,
         trainable: bool = True,
         dtype: _LayerDtype | None = None,
-        dynamic: bool = False,
+        autocast: bool = True,
         name: str | None = None,
     ) -> None: ...
 
 class Embedding(Layer[tf.Tensor, tf.Tensor]):
     def __init__(
         self,
         input_dim: int,
         output_dim: int,
         embeddings_initializer: _Initializer = "uniform",
         embeddings_regularizer: _Regularizer = None,
         embeddings_constraint: _Constraint = None,
         mask_zero: bool = False,
+        lora_rank: int | None = None,
+        *,
         input_length: int | None = None,
+        # **kwargs passed to Layer
+        activity_regularizer: _Regularizer = None,
         trainable: bool = True,
         dtype: _LayerDtype | None = None,
-        dynamic: bool = False,
+        autocast: bool = True,
         name: str | None = None,
     ) -> None: ...
 
 class Conv2D(Layer[tf.Tensor, tf.Tensor]):
     def __init__(
         self,
         filters: int,
@@ -211,74 +317,81 @@
         kernel_initializer: _Initializer = "glorot_uniform",
         bias_initializer: _Initializer = "zeros",
         kernel_regularizer: _Regularizer = None,
         bias_regularizer: _Regularizer = None,
         activity_regularizer: _Regularizer = None,
         kernel_constraint: _Constraint = None,
         bias_constraint: _Constraint = None,
+        *,
+        # **kwargs passed to Layer
         trainable: bool = True,
         dtype: _LayerDtype | None = None,
-        dynamic: bool = False,
+        autocast: bool = True,
         name: str | None = None,
     ) -> None: ...
 
+Convolution2D = Conv2D
+
 class Identity(Layer[tf.Tensor, tf.Tensor]):
     def __init__(
-        self, trainable: bool = True, dtype: _LayerDtype = None, dynamic: bool = False, name: str | None = None
+        self,
+        *,
+        # **kwargs passed to Layer
+        activity_regularizer: _Regularizer = None,
+        trainable: bool = True,
+        dtype: _LayerDtype | None = None,
+        autocast: bool = True,
+        name: str | None = None,
     ) -> None: ...
 
 class LayerNormalization(Layer[tf.Tensor, tf.Tensor]):
     def __init__(
         self,
         axis: int = -1,
         epsilon: float = 0.001,
         center: bool = True,
         scale: bool = True,
+        rms_scaling: bool = False,
         beta_initializer: _Initializer = "zeros",
         gamma_initializer: _Initializer = "ones",
         beta_regularizer: _Regularizer = None,
         gamma_regularizer: _Regularizer = None,
         beta_constraint: _Constraint = None,
         gamma_constraint: _Constraint = None,
+        *,
+        # **kwargs passed to Layer
+        activity_regularizer: _Regularizer = None,
         trainable: bool = True,
         dtype: _LayerDtype | None = None,
-        dynamic: bool = False,
-        name: str | None = None,
-    ) -> None: ...
-
-class DenseFeatures(Layer[Mapping[str, TensorLike], tf.Tensor]):
-    def __init__(
-        self,
-        feature_columns: Sequence[DenseColumn | SequenceDenseColumn],
-        trainable: bool = True,
-        dtype: _LayerDtype = None,
-        dynamic: bool = False,
+        autocast: bool = True,
         name: str | None = None,
     ) -> None: ...
 
 class MultiHeadAttention(Layer[Any, tf.Tensor]):
     def __init__(
         self,
         num_heads: int,
         key_dim: int | None,
         value_dim: int | None = None,
         dropout: float = 0.0,
         use_bias: bool = True,
         output_shape: tuple[int, ...] | None = None,
         attention_axes: tuple[int, ...] | None = None,
-        kernel_initialize: _Initializer = "glorot_uniform",
+        kernel_initializer: _Initializer = "glorot_uniform",
         bias_initializer: _Initializer = "zeros",
         kernel_regularizer: Regularizer | None = None,
         bias_regularizer: _Regularizer | None = None,
         activity_regularizer: _Regularizer | None = None,
         kernel_constraint: _Constraint | None = None,
         bias_constraint: _Constraint | None = None,
+        *,
+        # **kwargs passed to Layer
         trainable: bool = True,
         dtype: _LayerDtype | None = None,
-        dynamic: bool = False,
+        autocast: bool = True,
         name: str | None = None,
     ) -> None: ...
     # @override
     @overload  # type: ignore
     def __call__(
         self,
         query: tf.Tensor,
@@ -313,14 +426,17 @@
     ) -> tuple[tf.Tensor, tf.Tensor] | tf.Tensor: ...
 
 class GaussianDropout(Layer[tf.Tensor, tf.Tensor]):
     def __init__(
         self,
         rate: float,
         seed: int | None = None,
+        *,
+        # **kwargs passed to Layer
+        activity_regularizer: _Regularizer = None,
         trainable: bool = True,
-        dtype: _LayerDtype = None,
-        dynamic: bool = False,
+        dtype: _LayerDtype | None = None,
+        autocast: bool = True,
         name: str | None = None,
     ) -> None: ...
 
 def __getattr__(name: str) -> Incomplete: ...
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/layers/experimental/preprocessing.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/saved_model/experimental.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,39 @@
-import abc
-from typing import overload
+from enum import Enum
+from typing_extensions import Self
 
 import tensorflow as tf
-from tensorflow._aliases import AnyArray, DataSequence, Float, Integer, TensorCompatible, TensorLike
-from tensorflow.keras.layers import Layer
+from tensorflow._aliases import Integer, TensorValue
+from tensorflow.python.trackable.resource import CapturableResource
 
-class PreprocessingLayer(Layer[TensorLike, TensorLike], metaclass=abc.ABCMeta):
-    @property
-    def is_adapted(self) -> bool: ...
-    @overload  # type: ignore
-    def __call__(self, inputs: tf.Tensor, *, training: bool = False, mask: TensorCompatible | None = None) -> tf.Tensor: ...
-    @overload
-    def __call__(
-        self, inputs: tf.SparseTensor, *, training: bool = False, mask: TensorCompatible | None = None
-    ) -> tf.SparseTensor: ...
-    @overload
-    def __call__(
-        self, inputs: tf.RaggedTensor, *, training: bool = False, mask: TensorCompatible | None = None
-    ) -> tf.RaggedTensor: ...
-    def adapt(
+class Fingerprint:
+    saved_model_checksum: TensorValue | None
+    graph_def_program_hash: TensorValue | None = None
+    signature_def_hash: TensorValue | None = None
+    saved_object_graph_hash: TensorValue | None = None
+    checkpoint_hash: TensorValue | None = None
+    version: TensorValue | None = None
+    # In practice it seems like any type is accepted, but that might cause issues later on.
+    def __init__(
         self,
-        data: tf.data.Dataset[TensorLike] | AnyArray | DataSequence,
-        batch_size: Integer | None = None,
-        steps: Float | None = None,
+        saved_model_checksum: Integer | None = None,
+        graph_def_program_hash: Integer | None = None,
+        signature_def_hash: Integer | None = None,
+        saved_object_graph_hash: Integer | None = None,
+        checkpoint_hash: Integer | None = None,
+        version: Integer | None = None,
     ) -> None: ...
-    def compile(self, run_eagerly: bool | None = None, steps_per_execution: Integer | None = None) -> None: ...
+    @classmethod
+    def from_proto(cls, proto) -> Self: ...
+    def singleprint(self) -> str: ...
+
+class TrackableResource(CapturableResource):
+    @property
+    def resource_handle(self) -> tf.Tensor: ...
+    def __init__(self, device: str = "") -> None: ...
+
+class VariablePolicy(Enum):
+    EXPAND_DISTRIBUTED_VARIABLES = "expand_distributed_variables"
+    NONE = None
+    SAVE_VARIABLE_DEVICES = "save_variable_devices"
+
+def read_fingerprint(export_dir: str) -> Fingerprint: ...
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/layers/preprocessing/__init__.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/linalg.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,56 @@
-from typing import Literal
+from _typeshed import Incomplete
+from builtins import bool as _bool
+from collections.abc import Iterable
+from typing import Literal, overload
 
-from tensorflow._aliases import TensorCompatible
-from tensorflow.keras.layers.preprocessing.index_lookup import _IndexLookup
+import tensorflow as tf
+from tensorflow import RaggedTensor, Tensor, norm as norm
+from tensorflow._aliases import DTypeLike, IntArray, Integer, ScalarTensorCompatible, TensorCompatible
+from tensorflow.math import l2_normalize as l2_normalize
 
-class StringLookup(_IndexLookup):
-    def __init__(
-        self,
-        max_tokens: int | None = None,
-        num_oov_indices: int = 1,
-        mask_token: str | None = None,
-        oov_token: str = "[UNK]",
-        vocabulary: str | None | TensorCompatible = None,
-        idf_weights: TensorCompatible | None = None,
-        encoding: str = "utf-8",
-        invert: bool = False,
-        output_mode: Literal["int", "count", "multi_hot", "one_hot", "tf_idf"] = "int",
-        sparse: bool = False,
-        pad_to_max_tokens: bool = False,
-    ) -> None: ...
-
-class IntegerLookup(_IndexLookup):
-    def __init__(
-        self,
-        max_tokens: int | None = None,
-        num_oov_indices: int = 1,
-        mask_token: int | None = None,
-        oov_token: int = -1,
-        vocabulary: str | None | TensorCompatible = None,
-        vocabulary_dtype: Literal["int64", "int32"] = "int64",
-        idf_weights: TensorCompatible | None = None,
-        invert: bool = False,
-        output_mode: Literal["int", "count", "multi_hot", "one_hot", "tf_idf"] = "int",
-        sparse: bool = False,
-        pad_to_max_tokens: bool = False,
-    ) -> None: ...
+@overload
+def matmul(
+    a: TensorCompatible,
+    b: TensorCompatible,
+    transpose_a: _bool = False,
+    transpose_b: _bool = False,
+    adjoint_a: _bool = False,
+    adjoint_b: _bool = False,
+    a_is_sparse: _bool = False,
+    b_is_sparse: _bool = False,
+    output_type: DTypeLike | None = None,
+    grad_a: _bool = False,
+    grad_b: _bool = False,
+    name: str | None = None,
+) -> Tensor: ...
+@overload
+def matmul(
+    a: RaggedTensor,
+    b: RaggedTensor,
+    transpose_a: _bool = False,
+    transpose_b: _bool = False,
+    adjoint_a: _bool = False,
+    adjoint_b: _bool = False,
+    a_is_sparse: _bool = False,
+    b_is_sparse: _bool = False,
+    output_type: DTypeLike | None = None,
+    grad_a: _bool = False,
+    grad_b: _bool = False,
+    name: str | None = None,
+) -> RaggedTensor: ...
+def set_diag(
+    input: TensorCompatible,
+    diagonal: TensorCompatible,
+    name: str | None = "set_diag",
+    k: int = 0,
+    align: Literal["RIGHT_LEFT", "RIGHT_RIGHT", "LEFT_LEFT", "LEFT_RIGHT"] = "RIGHT_LEFT",
+) -> Tensor: ...
+def eye(
+    num_rows: ScalarTensorCompatible,
+    num_columns: ScalarTensorCompatible | None = None,
+    batch_shape: Iterable[int] | IntArray | tf.Tensor | None = None,
+    dtype: DTypeLike = ...,
+    name: str | None = None,
+) -> Tensor: ...
+def band_part(input: TensorCompatible, num_lower: Integer, num_upper: Integer, name: str | None = None) -> Tensor: ...
+def __getattr__(name: str) -> Incomplete: ...
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/losses.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/losses.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -10,15 +10,17 @@
     binary_crossentropy as binary_crossentropy,
     categorical_crossentropy as categorical_crossentropy,
 )
 
 class Loss(ABC):
     reduction: _ReductionValues
     name: str | None
-    def __init__(self, reduction: _ReductionValues = "auto", name: str | None = None) -> None: ...
+    def __init__(
+        self, name: str | None = None, reduction: _ReductionValues = "sum_over_batch_size", dtype: Incomplete | None = None
+    ) -> None: ...
     @abstractmethod
     def call(self, y_true: Tensor, y_pred: Tensor) -> Tensor: ...
     @classmethod
     def from_config(cls, config: dict[str, Any]) -> Self: ...
     def get_config(self) -> dict[str, Any]: ...
     def __call__(
         self, y_true: TensorCompatible, y_pred: TensorCompatible, sample_weight: TensorCompatible | None = None
@@ -26,100 +28,108 @@
 
 class BinaryCrossentropy(Loss):
     def __init__(
         self,
         from_logits: bool = False,
         label_smoothing: float = 0.0,
         axis: int = -1,
-        reduction: _ReductionValues = ...,
+        reduction: _ReductionValues = "sum_over_batch_size",
         name: str | None = "binary_crossentropy",
     ) -> None: ...
     def call(self, y_true: Tensor, y_pred: Tensor) -> Tensor: ...
 
 class BinaryFocalCrossentropy(Loss):
     def __init__(
         self,
         apply_class_balancing: bool = False,
         alpha: float = 0.25,
         gamma: float = 2.0,
         from_logits: bool = False,
         label_smoothing: float = 0.0,
         axis: int = -1,
-        reduction: _ReductionValues = ...,
+        reduction: _ReductionValues = "sum_over_batch_size",
         name: str | None = "binary_focal_crossentropy",
     ) -> None: ...
     def call(self, y_true: Tensor, y_pred: Tensor) -> Tensor: ...
 
 class CategoricalCrossentropy(Loss):
     def __init__(
         self,
         from_logits: bool = False,
         label_smoothing: float = 0.0,
         axis: int = -1,
-        reduction: _ReductionValues = ...,
+        reduction: _ReductionValues = "sum_over_batch_size",
         name: str | None = "categorical_crossentropy",
     ) -> None: ...
     def call(self, y_true: Tensor, y_pred: Tensor) -> Tensor: ...
 
 class CategoricalHinge(Loss):
-    def __init__(self, reduction: _ReductionValues = ..., name: str | None = "categorical_hinge") -> None: ...
+    def __init__(self, reduction: _ReductionValues = "sum_over_batch_size", name: str | None = "categorical_hinge") -> None: ...
     def call(self, y_true: Tensor, y_pred: Tensor) -> Tensor: ...
 
 class CosineSimilarity(Loss):
-    def __init__(self, axis: int = -1, reduction: _ReductionValues = ..., name: str | None = "cosine_similarity") -> None: ...
+    def __init__(
+        self, axis: int = -1, reduction: _ReductionValues = "sum_over_batch_size", name: str | None = "cosine_similarity"
+    ) -> None: ...
     def call(self, y_true: Tensor, y_pred: Tensor) -> Tensor: ...
 
 class Hinge(Loss):
-    def __init__(self, reduction: _ReductionValues = ..., name: str | None = "hinge") -> None: ...
+    def __init__(self, reduction: _ReductionValues = "sum_over_batch_size", name: str | None = "hinge") -> None: ...
     def call(self, y_true: Tensor, y_pred: Tensor) -> Tensor: ...
 
 class Huber(Loss):
-    def __init__(self, delta: float = 1.0, reduction: _ReductionValues = ..., name: str | None = "huber_loss") -> None: ...
+    def __init__(
+        self, delta: float = 1.0, reduction: _ReductionValues = "sum_over_batch_size", name: str | None = "huber_loss"
+    ) -> None: ...
     def call(self, y_true: Tensor, y_pred: Tensor) -> Tensor: ...
 
 class KLDivergence(Loss):
-    def __init__(self, reduction: _ReductionValues = ..., name: str | None = "kl_divergence") -> None: ...
+    def __init__(self, reduction: _ReductionValues = "sum_over_batch_size", name: str | None = "kl_divergence") -> None: ...
     def call(self, y_true: Tensor, y_pred: Tensor) -> Tensor: ...
 
 class LogCosh(Loss):
-    def __init__(self, reduction: _ReductionValues = ..., name: str | None = "log_cosh") -> None: ...
+    def __init__(self, reduction: _ReductionValues = "sum_over_batch_size", name: str | None = "log_cosh") -> None: ...
     def call(self, y_true: Tensor, y_pred: Tensor) -> Tensor: ...
 
 class MeanAbsoluteError(Loss):
-    def __init__(self, reduction: _ReductionValues = ..., name: str | None = "mean_absolute_error") -> None: ...
+    def __init__(self, reduction: _ReductionValues = "sum_over_batch_size", name: str | None = "mean_absolute_error") -> None: ...
     def call(self, y_true: Tensor, y_pred: Tensor) -> Tensor: ...
 
 class MeanAbsolutePercentageError(Loss):
-    def __init__(self, reduction: _ReductionValues = ..., name: str | None = "mean_absolute_percentage_error") -> None: ...
+    def __init__(
+        self, reduction: _ReductionValues = "sum_over_batch_size", name: str | None = "mean_absolute_percentage_error"
+    ) -> None: ...
     def call(self, y_true: Tensor, y_pred: Tensor) -> Tensor: ...
 
 class MeanSquaredError(Loss):
-    def __init__(self, reduction: _ReductionValues = ..., name: str | None = "mean_squared_error") -> None: ...
+    def __init__(self, reduction: _ReductionValues = "sum_over_batch_size", name: str | None = "mean_squared_error") -> None: ...
     def call(self, y_true: Tensor, y_pred: Tensor) -> Tensor: ...
 
 class MeanSquaredLogarithmicError(Loss):
-    def __init__(self, reduction: _ReductionValues = ..., name: str | None = "mean_squared_logarithmic_error") -> None: ...
+    def __init__(
+        self, reduction: _ReductionValues = "sum_over_batch_size", name: str | None = "mean_squared_logarithmic_error"
+    ) -> None: ...
     def call(self, y_true: Tensor, y_pred: Tensor) -> Tensor: ...
 
 class Poisson(Loss):
-    def __init__(self, reduction: _ReductionValues = ..., name: str | None = "poisson") -> None: ...
+    def __init__(self, reduction: _ReductionValues = "sum_over_batch_size", name: str | None = "poisson") -> None: ...
     def call(self, y_true: Tensor, y_pred: Tensor) -> Tensor: ...
 
 class SparseCategoricalCrossentropy(Loss):
     def __init__(
         self,
         from_logits: bool = False,
         ignore_class: int | None = None,
-        reduction: _ReductionValues = ...,
+        reduction: _ReductionValues = "sum_over_batch_size",
         name: str = "sparse_categorical_crossentropy",
     ) -> None: ...
     def call(self, y_true: Tensor, y_pred: Tensor) -> Tensor: ...
 
 class SquaredHinge(Loss):
-    def __init__(self, reduction: _ReductionValues = ..., name: str | None = "squared_hinge") -> None: ...
+    def __init__(self, reduction: _ReductionValues = "sum_over_batch_size", name: str | None = "squared_hinge") -> None: ...
     def call(self, y_true: Tensor, y_pred: Tensor) -> Tensor: ...
 
 class Reduction:
     AUTO: Final = "auto"
     NONE: Final = "none"
     SUM: Final = "sum"
     SUM_OVER_BATCH_SIZE: Final = "sum_over_batch_size"
@@ -129,18 +139,16 @@
     def validate(cls, key: object) -> TypeGuard[_ReductionValues]: ...
 
 _ReductionValues: TypeAlias = Literal["auto", "none", "sum", "sum_over_batch_size"]
 
 def categorical_hinge(y_true: TensorCompatible, y_pred: TensorCompatible) -> Tensor: ...
 def huber(y_true: TensorCompatible, y_pred: TensorCompatible, delta: float = 1.0) -> Tensor: ...
 def log_cosh(y_true: TensorCompatible, y_pred: TensorCompatible) -> Tensor: ...
-def deserialize(
-    name: str | dict[str, Any], custom_objects: dict[str, Any] | None = None, use_legacy_format: bool = False
-) -> Loss: ...
-def serialize(loss: KerasSerializable, use_legacy_format: bool = False) -> dict[str, Any]: ...
+def deserialize(name: str | dict[str, Any], custom_objects: dict[str, Any] | None = None) -> Loss: ...
+def serialize(loss: KerasSerializable) -> dict[str, Any]: ...
 
 _FuncT = TypeVar("_FuncT", bound=Callable[..., Any])
 
 @overload
 def get(identifier: None) -> None: ...
 @overload
 def get(identifier: str | dict[str, Any]) -> Loss: ...
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/metrics.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/metrics.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 from tensorflow import Operation, Tensor
 from tensorflow._aliases import DTypeLike, KerasSerializable, TensorCompatible
 from tensorflow.keras.initializers import _Initializer
 
 _Output: TypeAlias = Tensor | dict[str, Tensor]
 
 class Metric(tf.keras.layers.Layer[tf.Tensor, tf.Tensor], metaclass=ABCMeta):
-    def __init__(self, name: str | None = None, dtype: DTypeLike | None = None) -> None: ...
+    def __init__(self, dtype: DTypeLike | None = None, name: str | None = None) -> None: ...
     def __new__(cls, *args: Any, **kwargs: Any) -> Self: ...
-    def merge_state(self, metrics: Iterable[Self]) -> list[Operation]: ...
     def reset_state(self) -> None: ...
     @abstractmethod
     def update_state(
         self, y_true: TensorCompatible, y_pred: TensorCompatible, sample_weight: TensorCompatible | None = None
     ) -> Operation | None: ...
     @abstractmethod
     def result(self) -> _Output: ...
@@ -106,15 +105,15 @@
     def __init__(self, k: int = 5, name: str | None = "top_k_categorical_accuracy", dtype: DTypeLike | None = None) -> None: ...
 
 class SparseTopKCategoricalAccuracy(MeanMetricWrapper):
     def __init__(
         self, k: int = 5, name: str | None = "sparse_top_k_categorical_accuracy", dtype: DTypeLike | None = None
     ) -> None: ...
 
-def serialize(metric: KerasSerializable, use_legacy_format: bool = False) -> dict[str, Any]: ...
+def serialize(metric: KerasSerializable) -> dict[str, Any]: ...
 def binary_crossentropy(
     y_true: TensorCompatible, y_pred: TensorCompatible, from_logits: bool = False, label_smoothing: float = 0.0, axis: int = -1
 ) -> Tensor: ...
 def categorical_crossentropy(
     y_true: TensorCompatible, y_pred: TensorCompatible, from_logits: bool = False, label_smoothing: float = 0.0, axis: int = -1
 ) -> Tensor: ...
 def __getattr__(name: str) -> Incomplete: ...
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/models.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/models.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,78 @@
 from _typeshed import Incomplete
 from collections.abc import Callable, Container, Iterator
 from pathlib import Path
 from typing import Any, Literal
-from typing_extensions import Self, TypeAlias
+from typing_extensions import Self, TypeAlias, deprecated
 
 import numpy as np
 import numpy.typing as npt
-import tensorflow
 import tensorflow as tf
 from tensorflow import Variable
 from tensorflow._aliases import ContainerGeneric, ShapeLike, TensorCompatible
 from tensorflow.keras.layers import Layer, _InputT, _OutputT
 from tensorflow.keras.optimizers import Optimizer
 
 _Loss: TypeAlias = str | tf.keras.losses.Loss | Callable[[TensorCompatible, TensorCompatible], tf.Tensor]
 _Metric: TypeAlias = str | tf.keras.metrics.Metric | Callable[[TensorCompatible, TensorCompatible], tf.Tensor] | None
 
-class Model(Layer[_InputT, _OutputT], tf.Module):
+# Missing keras.src.backend.tensorflow.trainer.TensorFlowTrainer as a base class, which is not exposed by tensorflow
+class Model(Layer[_InputT, _OutputT]):
     _train_counter: tf.Variable
     _test_counter: tf.Variable
     optimizer: Optimizer | None
-    loss: tf.keras.losses.Loss | dict[str, tf.keras.losses.Loss]
+    # This is actually TensorFlowTrainer.loss
+    @deprecated("Instead, use `model.compute_loss(x, y, y_pred, sample_weight)`.")
+    def loss(
+        self, y: TensorCompatible | None, y_pred: TensorCompatible | None, sample_weight: Incomplete | None = None
+    ) -> tf.Tensor | None: ...
     stop_training: bool
 
     def __new__(cls, *args: Any, **kwargs: Any) -> Model[_InputT, _OutputT]: ...
     def __init__(self, *args: Any, **kwargs: Any) -> None: ...
     def __setattr__(self, name: str, value: Any) -> None: ...
     def __reduce__(self): ...
-    def __deepcopy__(self, memo): ...
     def build(self, input_shape: ShapeLike) -> None: ...
     def __call__(self, inputs: _InputT, *, training: bool = False, mask: TensorCompatible | None = None) -> _OutputT: ...
     def call(self, inputs: _InputT, training: bool | None = None, mask: TensorCompatible | None = None) -> _OutputT: ...
     # Ideally loss/metrics/output would share the same structure but higher kinded types are not supported.
     def compile(
         self,
         optimizer: Optimizer | str = "rmsprop",
         loss: ContainerGeneric[_Loss] | None = None,
-        metrics: ContainerGeneric[_Metric] | None = None,
         loss_weights: ContainerGeneric[float] | None = None,
+        metrics: ContainerGeneric[_Metric] | None = None,
         weighted_metrics: ContainerGeneric[_Metric] | None = None,
-        run_eagerly: bool | None = None,
-        steps_per_execution: int | Literal["auto"] | None = None,
-        jit_compile: bool | None = None,
-        pss_evaluation_shards: int | Literal["auto"] = 0,
-        **kwargs: Any,
+        run_eagerly: bool = False,
+        steps_per_execution: int | Literal["auto"] = 1,
+        jit_compile: bool | Literal["auto"] = "auto",
+        auto_scale_loss: bool | None = True,
     ) -> None: ...
     @property
     def metrics(self) -> list[Incomplete]: ...
     @property
     def metrics_names(self) -> list[str]: ...
     @property
     def distribute_strategy(self) -> tf.distribute.Strategy: ...
     @property
     def run_eagerly(self) -> bool: ...
     @property
-    def autotune_steps_per_execution(self) -> bool: ...
-    @property
-    def steps_per_execution(self) -> int | None: ...  # Returns None for a non-compiled model.
-    @property
     def jit_compile(self) -> bool: ...
     @property
     def distribute_reduction_method(self) -> Incomplete | Literal["auto"]: ...
     def train_step(self, data: TensorCompatible): ...
     def compute_loss(
         self,
         x: TensorCompatible | None = None,
         y: TensorCompatible | None = None,
         y_pred: TensorCompatible | None = None,
         sample_weight: Incomplete | None = None,
     ) -> tf.Tensor | None: ...
     def compute_metrics(
-        self, x: TensorCompatible, y: TensorCompatible, y_pred: TensorCompatible, sample_weight
+        self, x: TensorCompatible, y: TensorCompatible, y_pred: TensorCompatible, sample_weight: Incomplete | None = None
     ) -> dict[str, float]: ...
     def get_metrics_result(self) -> dict[str, float]: ...
     def make_train_function(self, force: bool = False) -> Callable[[tf.data.Iterator[Incomplete]], dict[str, float]]: ...
     def fit(
         self,
         x: TensorCompatible | dict[str, TensorCompatible] | tf.data.Dataset[Incomplete] | None = None,
         y: TensorCompatible | dict[str, TensorCompatible] | tf.data.Dataset[Incomplete] | None = None,
@@ -88,148 +86,81 @@
         class_weight: dict[int, float] | None = None,
         sample_weight: npt.NDArray[np.float_] | None = None,
         initial_epoch: int = 0,
         steps_per_epoch: int | None = None,
         validation_steps: int | None = None,
         validation_batch_size: int | None = None,
         validation_freq: int | Container[int] = 1,
-        max_queue_size: int = 10,
-        workers: int = 1,
-        use_multiprocessing: bool = False,
     ) -> tf.keras.callbacks.History: ...
     def test_step(self, data: TensorCompatible) -> dict[str, float]: ...
     def make_test_function(self, force: bool = False) -> Callable[[tf.data.Iterator[Incomplete]], dict[str, float]]: ...
     def evaluate(
         self,
         x: TensorCompatible | dict[str, TensorCompatible] | tf.data.Dataset[Incomplete] | None = None,
         y: TensorCompatible | dict[str, TensorCompatible] | tf.data.Dataset[Incomplete] | None = None,
         batch_size: int | None = None,
         verbose: Literal["auto", 0, 1, 2] = "auto",
         sample_weight: npt.NDArray[np.float_] | None = None,
         steps: int | None = None,
         callbacks: list[tf.keras.callbacks.Callback] | None = None,
-        max_queue_size: int = 10,
-        workers: int = 1,
-        use_multiprocessing: bool = False,
         return_dict: bool = False,
         **kwargs: Any,
     ) -> float | list[float]: ...
     def predict_step(self, data: _InputT) -> _OutputT: ...
     def make_predict_function(self, force: bool = False) -> Callable[[tf.data.Iterator[Incomplete]], _OutputT]: ...
     def predict(
         self,
         x: TensorCompatible | tf.data.Dataset[Incomplete],
         batch_size: int | None = None,
         verbose: Literal["auto", 0, 1, 2] = "auto",
         steps: int | None = None,
         callbacks: list[tf.keras.callbacks.Callback] | None = None,
-        max_queue_size: int = 10,
-        workers: int = 1,
-        use_multiprocessing: bool = False,
     ) -> _OutputT: ...
     def reset_metrics(self) -> None: ...
     def train_on_batch(
         self,
         x: TensorCompatible | dict[str, TensorCompatible] | tf.data.Dataset[Incomplete],
         y: TensorCompatible | dict[str, TensorCompatible] | tf.data.Dataset[Incomplete] | None = None,
         sample_weight: npt.NDArray[np.float_] | None = None,
         class_weight: dict[int, float] | None = None,
-        reset_metrics: bool = True,
         return_dict: bool = False,
     ) -> float | list[float]: ...
     def test_on_batch(
         self,
         x: TensorCompatible | dict[str, TensorCompatible] | tf.data.Dataset[Incomplete],
         y: TensorCompatible | dict[str, TensorCompatible] | tf.data.Dataset[Incomplete] | None = None,
         sample_weight: npt.NDArray[np.float_] | None = None,
-        reset_metrics: bool = True,
         return_dict: bool = False,
     ) -> float | list[float]: ...
     def predict_on_batch(self, x: Iterator[_InputT]) -> npt.NDArray[Incomplete]: ...
-    def fit_generator(
-        self,
-        generator: Iterator[Incomplete],
-        steps_per_epoch: int | None = None,
-        epochs: int = 1,
-        verbose: Literal["auto", 0, 1, 2] = 1,
-        callbacks: list[tf.keras.callbacks.Callback] | None = None,
-        validation_data: TensorCompatible | tf.data.Dataset[Any] | None = None,
-        validation_steps: int | None = None,
-        validation_freq: int | Container[int] = 1,
-        class_weight: dict[int, float] | None = None,
-        max_queue_size: int = 10,
-        workers: int = 1,
-        use_multiprocessing: bool = False,
-        shuffle: bool = True,
-        initial_epoch: int = 0,
-    ) -> tf.keras.callbacks.History: ...
-    def evaluate_generator(
-        self,
-        generator: Iterator[Incomplete],
-        steps: int | None = None,
-        callbacks: list[tf.keras.callbacks.Callback] | None = None,
-        max_queue_size: int = 10,
-        workers: int = 1,
-        use_multiprocessing: bool = False,
-        verbose: Literal["auto", 0, 1, 2] = 0,
-    ) -> float | list[float]: ...
-    def predict_generator(
-        self,
-        generator: Iterator[Incomplete],
-        steps: int | None = None,
-        callbacks: list[tf.keras.callbacks.Callback] | None = None,
-        max_queue_size: int = 10,
-        workers: int = 1,
-        use_multiprocessing: bool = False,
-        verbose: Literal["auto", 0, 1, 2] = 0,
-    ) -> _OutputT: ...
     @property
     def trainable_weights(self) -> list[Variable]: ...
     @property
     def non_trainable_weights(self) -> list[Variable]: ...
     def get_weights(self): ...
-    def save(
-        self, filepath: str | Path, overwrite: bool = True, save_format: Literal["keras", "tf", "h5"] | None = None, **kwargs: Any
-    ) -> None: ...
-    def save_weights(
-        self,
-        filepath: str | Path,
-        overwrite: bool = True,
-        save_format: Literal["tf", "h5"] | None = None,
-        options: tf.train.CheckpointOptions | None = None,
-    ) -> None: ...
-    def load_weights(
-        self,
-        filepath: str | Path,
-        skip_mismatch: bool = False,
-        by_name: bool = False,
-        options: None | tensorflow.train.CheckpointOptions = None,
-    ) -> None: ...
+    def save(self, filepath: str | Path, overwrite: bool = True) -> None: ...
+    def save_weights(self, filepath: str | Path, overwrite: bool = True) -> None: ...
+    # kwargs are from keras.saving.saving_api.load_weights
+    def load_weights(self, filepath: str | Path, skip_mismatch: bool = False, *, by_name: bool = False) -> None: ...
     def get_config(self) -> dict[str, Any]: ...
     @classmethod
     def from_config(cls, config: dict[str, Any], custom_objects: Incomplete | None = None) -> Self: ...
     def to_json(self, **kwargs: Any) -> str: ...
-    def to_yaml(self, **kwargs: Any) -> str: ...
-    def reset_states(self) -> None: ...
-    @property
-    def state_updates(self) -> list[Incomplete]: ...
     @property
     def weights(self) -> list[Variable]: ...
     def summary(
         self,
         line_length: None | int = None,
         positions: None | list[float] = None,
         print_fn: None | Callable[[str], None] = None,
         expand_nested: bool = False,
         show_trainable: bool = False,
         layer_range: None | list[str] | tuple[str, str] = None,
     ) -> None: ...
     @property
     def layers(self) -> list[Layer[Incomplete, Incomplete]]: ...
     def get_layer(self, name: str | None = None, index: int | None = None) -> Layer[Incomplete, Incomplete]: ...
-    def get_weight_paths(self) -> dict[str, tf.Variable]: ...
     def get_compile_config(self) -> dict[str, Any]: ...
     def compile_from_config(self, config: dict[str, Any]) -> Self: ...
-    def export(self, filepath: str | Path) -> None: ...
-    def save_spec(self, dynamic_batch: bool = True) -> tuple[tuple[tf.TensorSpec, ...], dict[str, tf.TensorSpec]] | None: ...
+    def export(self, filepath: str | Path, format: str = "tf_saved_model") -> None: ...
 
 def __getattr__(name: str) -> Incomplete: ...
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/optimizers/schedules.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/optimizers/schedules.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -15,57 +15,57 @@
     def from_config(cls, config: dict[str, Any]) -> Self: ...
 
 class PiecewiseConstantDecay(LearningRateSchedule):
     def __init__(
         self,
         boundaries: Sequence[tf.Tensor] | Sequence[float],
         values: Sequence[float] | Sequence[tf.Tensor],
-        name: str | None = None,
+        name: str = "PiecewiseConstant",
     ) -> None: ...
     def __call__(self, step: int | tf.Tensor) -> float | tf.Tensor: ...
     def get_config(self) -> dict[str, Any]: ...
     @classmethod
     def from_config(cls, config: dict[str, Any]) -> Self: ...
 
 class InverseTimeDecay(LearningRateSchedule):
     def __init__(
         self,
         initial_learning_rate: float | tf.Tensor,
         decay_steps: int,
         decay_rate: float,
         staircase: bool = False,
-        name: str | None = None,
+        name: str = "InverseTimeDecay",
     ) -> None: ...
     def __call__(self, step: int | tf.Tensor) -> float | tf.Tensor: ...
     def get_config(self) -> dict[str, Any]: ...
     @classmethod
     def from_config(cls, config: dict[str, Any]) -> Self: ...
 
 class PolynomialDecay(LearningRateSchedule):
     def __init__(
         self,
         initial_learning_rate: float | tf.Tensor,
         decay_steps: int,
         end_learning_rate: float | tf.Tensor = 0.0001,
         power: float = 1.0,
         cycle: bool = False,
-        name: str | None = None,
+        name: str = "PolynomialDecay",
     ) -> None: ...
     def __call__(self, step: int | tf.Tensor) -> float | tf.Tensor: ...
     def get_config(self) -> dict[str, Any]: ...
     @classmethod
     def from_config(cls, config: dict[str, Any]) -> Self: ...
 
 class CosineDecay(LearningRateSchedule):
     def __init__(
         self,
         initial_learning_rate: float | tf.Tensor,
         decay_steps: int,
         alpha: float | tf.Tensor = 0.0,
-        name: str | None = None,
+        name: str = "CosineDecay",
         warmup_target: int | tf.Tensor | None = None,  # float32 or float64 Tensor
         warmup_steps: int | tf.Tensor = 0,  # int32 or int64 Tensor
     ) -> None: ...
     def __call__(self, step: int | tf.Tensor) -> float | tf.Tensor: ...
     def get_config(self) -> dict[str, Any]: ...
     @classmethod
     def from_config(cls, config: dict[str, Any]) -> Self: ...
@@ -74,32 +74,30 @@
     def __init__(
         self,
         initial_learning_rate: float | tf.Tensor,
         first_decay_steps: int | tf.Tensor,
         t_mul: float | tf.Tensor = 2.0,
         m_mul: float | tf.Tensor = 1.0,
         alpha: float | tf.Tensor = 0.0,
-        name: str | None = None,
+        name: str = "SGDRDecay",
     ) -> None: ...
     def __call__(self, step: int | tf.Tensor) -> float | tf.Tensor: ...
     def get_config(self) -> dict[str, Any]: ...
     @classmethod
     def from_config(cls, config: dict[str, Any]) -> Self: ...
 
 class ExponentialDecay(LearningRateSchedule):
     def __init__(
         self,
         initial_learning_rate: float | tf.Tensor,
         decay_steps: int | tf.Tensor,
         decay_rate: float | tf.Tensor,
         staircase: bool = False,
-        name: str | None = None,
+        name: str = "ExponentialDecay",
     ) -> None: ...
     def __call__(self, step: int | tf.Tensor) -> float | tf.Tensor: ...
     def get_config(self) -> dict[str, Any]: ...
     @classmethod
     def from_config(cls, config: dict[str, Any]) -> Self: ...
 
-def deserialize(
-    config: dict[str, Any], custom_objects: dict[str, type] | None = None, use_legacy_format: bool = False
-) -> LearningRateSchedule: ...
-def serialize(learning_rate_schedule: LearningRateSchedule, use_legacy_format: bool = False) -> dict[str, Any]: ...
+def deserialize(config: dict[str, Any], custom_objects: dict[str, type] | None = None) -> LearningRateSchedule: ...
+def serialize(learning_rate_schedule: LearningRateSchedule) -> dict[str, Any]: ...
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/keras/regularizers.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/keras/regularizers.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from _typeshed import Incomplete
 from collections.abc import Callable
 from typing import Any, overload
 from typing_extensions import Self, TypeAlias
 
 from tensorflow import Tensor
 
 class Regularizer:
@@ -14,8 +15,8 @@
 
 @overload
 def get(identifier: None) -> None: ...
 @overload
 def get(identifier: str | dict[str, Any] | Regularizer) -> Regularizer: ...
 @overload
 def get(identifier: Callable[[Tensor], Tensor]) -> Callable[[Tensor], Tensor]: ...
-def __getattr__(name: str) -> Any: ...
+def __getattr__(name: str) -> Incomplete: ...
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/math.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/math.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/nn.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/nn.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/feature_column/feature_column_v2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/feature_column/feature_column_v2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/random.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/random.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/raw_ops.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/raw_ops.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/saved_model/__init__.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/saved_model/__init__.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from _typeshed import Incomplete
 from collections.abc import Mapping, Sequence
 from pathlib import Path
 from typing import Any, Generic, Literal, TypeVar
 from typing_extensions import ParamSpec, TypeAlias
 
 import tensorflow as tf
 from tensorflow.python.training.tracking.autotrackable import AutoTrackable
 from tensorflow.saved_model.experimental import VariablePolicy
-from tensorflow.types.experimental import ConcreteFunction, GenericFunction
+from tensorflow.types.experimental import ConcreteFunction, PolymorphicFunction
 
 _P = ParamSpec("_P")
 _R = TypeVar("_R", covariant=True)
 
 class Asset:
     @property
     def asset_path(self) -> tf.Tensor: ...
@@ -35,38 +36,42 @@
     ) -> None: ...
 
 class SaveOptions:
     __slots__ = (
         "namespace_whitelist",
         "save_debug_info",
         "function_aliases",
+        "experimental_debug_stripper",
         "experimental_io_device",
         "experimental_variable_policy",
         "experimental_custom_gradients",
         "experimental_image_format",
         "experimental_skip_saver",
+        "experimental_sharding_callback",
     )
     namespace_whitelist: list[str]
     save_debug_info: bool
-    function_aliases: dict[str, tf.types.experimental.GenericFunction[..., object]]
+    function_aliases: dict[str, PolymorphicFunction[..., object]]
     experimental_io_device: str
     experimental_variable_policy: VariablePolicy
     experimental_custom_gradients: bool
     experimental_image_format: bool
     experimental_skip_saver: bool
     def __init__(
         self,
         namespace_whitelist: list[str] | None = None,
         save_debug_info: bool = False,
-        function_aliases: Mapping[str, tf.types.experimental.GenericFunction[..., object]] | None = None,
+        function_aliases: Mapping[str, PolymorphicFunction[..., object]] | None = None,
+        experimental_debug_stripper: bool = False,
         experimental_io_device: str | None = None,
         experimental_variable_policy: str | VariablePolicy | None = None,
         experimental_custom_gradients: bool = True,
         experimental_image_format: bool = False,
         experimental_skip_saver: bool = False,
+        experimental_sharding_callback: Incomplete | None = None,
     ) -> None: ...
 
 def contains_saved_model(export_dir: str | Path) -> bool: ...
 
 class _LoadedAttributes(Generic[_P, _R]):
     signatures: Mapping[str, ConcreteFunction[_P, _R]]
 
@@ -76,15 +81,15 @@
     # TF1 model artifact specific
     graph: tf.Graph
 
 def load(
     export_dir: str, tags: str | Sequence[str] | None = None, options: LoadOptions | None = None
 ) -> _LoadedModel[..., Any]: ...
 
-_TF_Function: TypeAlias = ConcreteFunction[..., object] | GenericFunction[..., object]
+_TF_Function: TypeAlias = ConcreteFunction[..., object] | PolymorphicFunction[..., object]
 
 def save(
     obj: tf.Module,
     export_dir: str,
     signatures: _TF_Function | Mapping[str, _TF_Function] | None = None,
     options: SaveOptions | None = None,
 ) -> None: ...
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/sparse.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/sparse.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/strings.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/strings.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/summary.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/summary.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from collections.abc import Callable, Iterator
 from contextlib import AbstractContextManager, contextmanager
 from typing import Literal
 from typing_extensions import Self
 
 import tensorflow as tf
 from tensorflow._aliases import FloatArray, IntArray
+from tensorflow.core.framework.graph_pb2 import GraphDef
 from tensorflow.experimental.dtensor import Mesh
 
 class SummaryWriter(metaclass=abc.ABCMeta):
     def as_default(self, step: int | None = None) -> AbstractContextManager[Self]: ...
     def close(self) -> None: ...
     def flush(self) -> None: ...
     def init(self) -> None: ...
@@ -32,15 +33,15 @@
     filename_suffix: str | None = None,
     name: str | None = None,
     experimental_trackable: bool = False,
     experimental_mesh: Mesh | None = None,
 ) -> SummaryWriter: ...
 def create_noop_writer() -> SummaryWriter: ...
 def flush(writer: SummaryWriter | None = None, name: str | None = None) -> tf.Operation: ...
-def graph(graph_data: tf.Graph | tf.compat.v1.GraphDef) -> bool: ...
+def graph(graph_data: tf.Graph | GraphDef) -> bool: ...
 def histogram(
     name: str, data: tf.Tensor, step: int | None = None, buckets: int | None = None, description: str | None = None
 ) -> bool: ...
 def image(
     name: str,
     data: tf.Tensor | FloatArray | IntArray,
     step: int | tf.Tensor | None = None,
@@ -50,11 +51,11 @@
 @contextmanager
 def record_if(condition: bool | tf.Tensor | Callable[[], bool]) -> Iterator[None]: ...
 def scalar(name: str, data: float | tf.Tensor, step: int | tf.Tensor | None = None, description: str | None = None) -> bool: ...
 def should_record_summaries() -> bool: ...
 def text(name: str, data: str | tf.Tensor, step: int | tf.Tensor | None = None, description: str | None = None) -> bool: ...
 def trace_export(name: str, step: int | tf.Tensor | None = None, profiler_outdir: str | None = None) -> None: ...
 def trace_off() -> None: ...
-def trace_on(graph: bool = True, profiler: bool = False) -> None: ...
+def trace_on(graph: bool = True, profiler: bool = False, profiler_outdir: str | None = None) -> None: ...
 def write(
     tag: str, tensor: tf.Tensor, step: int | tf.Tensor | None = None, metadata: Incomplete | None = None, name: str | None = None
 ) -> bool: ...
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/train/__init__.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/train/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 
     def __init__(
         self,
         experimental_io_device: None | str = None,
         experimental_enable_async_checkpoint: bool = False,
         experimental_write_callbacks: None | list[Callable[[str], object] | Callable[[], object]] = None,
         enable_async: bool = False,
+        experimental_skip_slot_variables: bool = False,
+        experimental_sharding_callback: Incomplete | None = None,
     ) -> None: ...
 
 _T = TypeVar("_T", bound=list[str] | tuple[str] | dict[int, str])
 
 class ClusterSpec:
     def __init__(self, cluster: dict[str, _T] | ClusterDef | ClusterSpec) -> None: ...
     def as_dict(self) -> dict[str, list[str] | tuple[str] | dict[int, str]]: ...
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/autotuning_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/core/framework/graph_debug_info_pb2.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,253 +1,198 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
-This file defines protos that store the results of autotuning various
-operations.
-
-They are in proto format because we want to log them structured. They offer
-tremendous statistical, testing, and debugging value.
 """
 
 import builtins
 import collections.abc
-import sys
 import typing
 
-import google.protobuf.any_pb2
 import google.protobuf.descriptor
-import google.protobuf.duration_pb2
 import google.protobuf.internal.containers
-import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
-import tensorflow.tsl.protobuf.dnn_pb2
-
-if sys.version_info >= (3, 10):
-    import typing as typing_extensions
-else:
-    import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing.final
-class CudnnVersion(google.protobuf.message.Message):
+class GraphDebugInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    MAJOR_FIELD_NUMBER: builtins.int
-    MINOR_FIELD_NUMBER: builtins.int
-    PATCH_FIELD_NUMBER: builtins.int
-    major: builtins.int
-    minor: builtins.int
-    patch: builtins.int
-    def __init__(
-        self,
-        *,
-        major: builtins.int | None = ...,
-        minor: builtins.int | None = ...,
-        patch: builtins.int | None = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing.Literal["major", b"major", "minor", b"minor", "patch", b"patch"]) -> None: ...
-
-global___CudnnVersion = CudnnVersion
+    @typing.final
+    class FileLineCol(google.protobuf.message.Message):
+        """This represents a file/line location in the source code."""
 
-@typing.final
-class ComputeCapability(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    MAJOR_FIELD_NUMBER: builtins.int
-    MINOR_FIELD_NUMBER: builtins.int
-    major: builtins.int
-    minor: builtins.int
-    def __init__(
-        self,
-        *,
-        major: builtins.int | None = ...,
-        minor: builtins.int | None = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing.Literal["major", b"major", "minor", b"minor"]) -> None: ...
+        FILE_INDEX_FIELD_NUMBER: builtins.int
+        LINE_FIELD_NUMBER: builtins.int
+        COL_FIELD_NUMBER: builtins.int
+        FUNC_FIELD_NUMBER: builtins.int
+        CODE_FIELD_NUMBER: builtins.int
+        file_index: builtins.int
+        """File name index, which can be used to retrieve the file name string from
+        `files`. The value should be between 0 and (len(files)-1)
+        """
+        line: builtins.int
+        """Line number in the file."""
+        col: builtins.int
+        """Col number in the file line."""
+        func: builtins.str
+        """Name of function contains the file line."""
+        code: builtins.str
+        """Source code contained in this file line."""
+        def __init__(
+            self,
+            *,
+            file_index: builtins.int | None = ...,
+            line: builtins.int | None = ...,
+            col: builtins.int | None = ...,
+            func: builtins.str | None = ...,
+            code: builtins.str | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing.Literal["code", b"code", "col", b"col", "file_index", b"file_index", "func", b"func", "line", b"line"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["code", b"code", "col", b"col", "file_index", b"file_index", "func", b"func", "line", b"line"]) -> None: ...
 
-global___ComputeCapability = ComputeCapability
+    @typing.final
+    class StackTrace(google.protobuf.message.Message):
+        """This represents a stack trace which is a ordered list of `FileLineCol`."""
 
-@typing.final
-class AutotuneResult(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    class _FailureKind:
-        ValueType = typing.NewType("ValueType", builtins.int)
-        V: typing_extensions.TypeAlias = ValueType
-
-    class _FailureKindEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[AutotuneResult._FailureKind.ValueType], builtins.type):
-        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
-        UNKNOWN: AutotuneResult._FailureKind.ValueType  # 0
-        REDZONE_MODIFIED: AutotuneResult._FailureKind.ValueType  # 1
-        """Algorithm wrote memory outside its output buffers."""
-        WRONG_RESULT: AutotuneResult._FailureKind.ValueType  # 2
-        """Algorithm gave a different result from a reference algorithm."""
-        DISQUALIFIED: AutotuneResult._FailureKind.ValueType  # 3
-        """Algorithm was rejected for failing to run or for known bugs."""
-
-    class FailureKind(_FailureKind, metaclass=_FailureKindEnumTypeWrapper): ...
-    UNKNOWN: AutotuneResult.FailureKind.ValueType  # 0
-    REDZONE_MODIFIED: AutotuneResult.FailureKind.ValueType  # 1
-    """Algorithm wrote memory outside its output buffers."""
-    WRONG_RESULT: AutotuneResult.FailureKind.ValueType  # 2
-    """Algorithm gave a different result from a reference algorithm."""
-    DISQUALIFIED: AutotuneResult.FailureKind.ValueType  # 3
-    """Algorithm was rejected for failing to run or for known bugs."""
-
-    @typing.final
-    class FailureResult(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-        KIND_FIELD_NUMBER: builtins.int
-        MSG_FIELD_NUMBER: builtins.int
-        REFERENCE_CONV_FIELD_NUMBER: builtins.int
-        REFERENCE_GEMM_FIELD_NUMBER: builtins.int
-        REFERENCE_CUDA_CONV_PLAN_FIELD_NUMBER: builtins.int
-        REFERENCE_ALGORITHM_FIELD_NUMBER: builtins.int
-        BUFFER_ADDRESS_FIELD_NUMBER: builtins.int
-        kind: global___AutotuneResult.FailureKind.ValueType
-        msg: builtins.str
-        buffer_address: builtins.int
-        @property
-        def reference_conv(self) -> global___AutotuneResult.ConvKey: ...
+        FILE_LINE_COLS_FIELD_NUMBER: builtins.int
+        FRAME_ID_FIELD_NUMBER: builtins.int
         @property
-        def reference_gemm(self) -> global___AutotuneResult.GemmKey: ...
-        @property
-        def reference_cuda_conv_plan(self) -> global___AutotuneResult.CudaConvPlanKey: ...
+        def file_line_cols(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___GraphDebugInfo.FileLineCol]:
+            """Deprecated."""
+
         @property
-        def reference_algorithm(self) -> tensorflow.tsl.protobuf.dnn_pb2.AlgorithmProto: ...
+        def frame_id(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
         def __init__(
             self,
             *,
-            kind: global___AutotuneResult.FailureKind.ValueType | None = ...,
-            msg: builtins.str | None = ...,
-            reference_conv: global___AutotuneResult.ConvKey | None = ...,
-            reference_gemm: global___AutotuneResult.GemmKey | None = ...,
-            reference_cuda_conv_plan: global___AutotuneResult.CudaConvPlanKey | None = ...,
-            reference_algorithm: tensorflow.tsl.protobuf.dnn_pb2.AlgorithmProto | None = ...,
-            buffer_address: builtins.int | None = ...,
+            file_line_cols: collections.abc.Iterable[global___GraphDebugInfo.FileLineCol] | None = ...,
+            frame_id: collections.abc.Iterable[builtins.int] | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing.Literal["key", b"key", "reference_algorithm", b"reference_algorithm", "reference_conv", b"reference_conv", "reference_cuda_conv_plan", b"reference_cuda_conv_plan", "reference_gemm", b"reference_gemm"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing.Literal["buffer_address", b"buffer_address", "key", b"key", "kind", b"kind", "msg", b"msg", "reference_algorithm", b"reference_algorithm", "reference_conv", b"reference_conv", "reference_cuda_conv_plan", b"reference_cuda_conv_plan", "reference_gemm", b"reference_gemm"]) -> None: ...
-        def WhichOneof(self, oneof_group: typing.Literal["key", b"key"]) -> typing.Literal["reference_conv", "reference_gemm", "reference_cuda_conv_plan", "reference_algorithm"] | None: ...
+        def ClearField(self, field_name: typing.Literal["file_line_cols", b"file_line_cols", "frame_id", b"frame_id"]) -> None: ...
 
     @typing.final
-    class ConvKey(google.protobuf.message.Message):
-        """Legacy and unused in new data; superseded by AlgorithmProto."""
-
+    class FramesByIdEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-        ALGORITHM_FIELD_NUMBER: builtins.int
-        TENSOR_OPS_ENABLED_FIELD_NUMBER: builtins.int
-        algorithm: builtins.int
-        tensor_ops_enabled: builtins.bool
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.int
+        @property
+        def value(self) -> global___GraphDebugInfo.FileLineCol: ...
         def __init__(
             self,
             *,
-            algorithm: builtins.int | None = ...,
-            tensor_ops_enabled: builtins.bool | None = ...,
+            key: builtins.int | None = ...,
+            value: global___GraphDebugInfo.FileLineCol | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing.Literal["algorithm", b"algorithm", "tensor_ops_enabled", b"tensor_ops_enabled"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     @typing.final
-    class GemmKey(google.protobuf.message.Message):
+    class TracesByIdEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-        ALGORITHM_FIELD_NUMBER: builtins.int
-        algorithm: builtins.int
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.int
+        @property
+        def value(self) -> global___GraphDebugInfo.StackTrace: ...
         def __init__(
             self,
             *,
-            algorithm: builtins.int | None = ...,
+            key: builtins.int | None = ...,
+            value: global___GraphDebugInfo.StackTrace | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing.Literal["algorithm", b"algorithm"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     @typing.final
-    class CudaConvPlanKey(google.protobuf.message.Message):
-        """Legacy and unused in new data; superseded by AlgorithmProto."""
-
+    class TracesEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-        EXEC_PLAN_ID_FIELD_NUMBER: builtins.int
-        exec_plan_id: builtins.str
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        @property
+        def value(self) -> global___GraphDebugInfo.StackTrace: ...
         def __init__(
             self,
             *,
-            exec_plan_id: builtins.str | None = ...,
+            key: builtins.str | None = ...,
+            value: global___GraphDebugInfo.StackTrace | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing.Literal["exec_plan_id", b"exec_plan_id"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-    SCRATCH_BYTES_FIELD_NUMBER: builtins.int
-    RUN_TIME_FIELD_NUMBER: builtins.int
-    FAILURE_FIELD_NUMBER: builtins.int
-    CONV_FIELD_NUMBER: builtins.int
-    GEMM_FIELD_NUMBER: builtins.int
-    CUDA_CONV_PLAN_FIELD_NUMBER: builtins.int
-    ALGORITHM_FIELD_NUMBER: builtins.int
-    scratch_bytes: builtins.int
-    @property
-    def run_time(self) -> google.protobuf.duration_pb2.Duration: ...
-    @property
-    def failure(self) -> global___AutotuneResult.FailureResult: ...
-    @property
-    def conv(self) -> global___AutotuneResult.ConvKey: ...
-    @property
-    def gemm(self) -> global___AutotuneResult.GemmKey: ...
-    @property
-    def cuda_conv_plan(self) -> global___AutotuneResult.CudaConvPlanKey: ...
-    @property
-    def algorithm(self) -> tensorflow.tsl.protobuf.dnn_pb2.AlgorithmProto: ...
-    def __init__(
-        self,
-        *,
-        scratch_bytes: builtins.int | None = ...,
-        run_time: google.protobuf.duration_pb2.Duration | None = ...,
-        failure: global___AutotuneResult.FailureResult | None = ...,
-        conv: global___AutotuneResult.ConvKey | None = ...,
-        gemm: global___AutotuneResult.GemmKey | None = ...,
-        cuda_conv_plan: global___AutotuneResult.CudaConvPlanKey | None = ...,
-        algorithm: tensorflow.tsl.protobuf.dnn_pb2.AlgorithmProto | None = ...,
-    ) -> None: ...
-    def HasField(self, field_name: typing.Literal["algorithm", b"algorithm", "conv", b"conv", "cuda_conv_plan", b"cuda_conv_plan", "failure", b"failure", "gemm", b"gemm", "key", b"key", "run_time", b"run_time"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing.Literal["algorithm", b"algorithm", "conv", b"conv", "cuda_conv_plan", b"cuda_conv_plan", "failure", b"failure", "gemm", b"gemm", "key", b"key", "run_time", b"run_time", "scratch_bytes", b"scratch_bytes"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing.Literal["key", b"key"]) -> typing.Literal["conv", "gemm", "cuda_conv_plan", "algorithm"] | None: ...
-
-global___AutotuneResult = AutotuneResult
+    @typing.final
+    class NameToTraceIdEntry(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-@typing.final
-class AutotuningLog(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        value: builtins.int
+        def __init__(
+            self,
+            *,
+            key: builtins.str | None = ...,
+            value: builtins.int | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-    INSTR_FIELD_NUMBER: builtins.int
-    RESULTS_FIELD_NUMBER: builtins.int
-    CUDNN_VERSION_FIELD_NUMBER: builtins.int
-    COMPUTE_CAPABILITY_FIELD_NUMBER: builtins.int
-    DEVICE_PCI_BUS_ID_FIELD_NUMBER: builtins.int
-    BLAS_VERSION_FIELD_NUMBER: builtins.int
-    device_pci_bus_id: builtins.str
-    """stream_executor::DeviceDescription::pci_bus_id."""
-    blas_version: builtins.str
-    @property
-    def instr(self) -> google.protobuf.any_pb2.Any: ...
-    @property
-    def results(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___AutotuneResult]:
-        """Records all auto-tuning results per algorithm."""
+    FILES_FIELD_NUMBER: builtins.int
+    FRAMES_BY_ID_FIELD_NUMBER: builtins.int
+    TRACES_BY_ID_FIELD_NUMBER: builtins.int
+    TRACES_FIELD_NUMBER: builtins.int
+    NAME_TO_TRACE_ID_FIELD_NUMBER: builtins.int
+    @property
+    def files(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+        """This stores all the source code file names and can be indexed by the
+        `file_index`.
+        """
+
+    @property
+    def frames_by_id(self) -> google.protobuf.internal.containers.MessageMap[builtins.int, global___GraphDebugInfo.FileLineCol]:
+        """Stack traces and frames are uniqueified during construction. These maps
+        index from the unique id for a frame/trace to the value.
+        """
+
+    @property
+    def traces_by_id(self) -> google.protobuf.internal.containers.MessageMap[builtins.int, global___GraphDebugInfo.StackTrace]: ...
+    @property
+    def traces(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___GraphDebugInfo.StackTrace]:
+        """Deprecated."""
+
+    @property
+    def name_to_trace_id(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.int]:
+        """This maps a node name to a trace id contained in `traces_by_id`.
+
+        The map key is a mangling of the containing function and op name with
+        syntax:
+          op.name '@' func_name
+        For ops in the top-level graph, the func_name is the empty string and hence
+        the `@` may be ommitted.
+        Note that op names are restricted to a small number of characters which
+        exclude '@', making it impossible to collide keys of this form. Function
+        names accept a much wider set of characters.
+        It would be preferable to avoid mangling and use a tuple key of (op.name,
+        func_name), but this is not supported with protocol buffers.
+        """
 
-    @property
-    def cudnn_version(self) -> global___CudnnVersion: ...
-    @property
-    def compute_capability(self) -> global___ComputeCapability: ...
     def __init__(
         self,
         *,
-        instr: google.protobuf.any_pb2.Any | None = ...,
-        results: collections.abc.Iterable[global___AutotuneResult] | None = ...,
-        cudnn_version: global___CudnnVersion | None = ...,
-        compute_capability: global___ComputeCapability | None = ...,
-        device_pci_bus_id: builtins.str | None = ...,
-        blas_version: builtins.str | None = ...,
+        files: collections.abc.Iterable[builtins.str] | None = ...,
+        frames_by_id: collections.abc.Mapping[builtins.int, global___GraphDebugInfo.FileLineCol] | None = ...,
+        traces_by_id: collections.abc.Mapping[builtins.int, global___GraphDebugInfo.StackTrace] | None = ...,
+        traces: collections.abc.Mapping[builtins.str, global___GraphDebugInfo.StackTrace] | None = ...,
+        name_to_trace_id: collections.abc.Mapping[builtins.str, builtins.int] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing.Literal["compute_capability", b"compute_capability", "cudnn_version", b"cudnn_version", "instr", b"instr"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing.Literal["blas_version", b"blas_version", "compute_capability", b"compute_capability", "cudnn_version", b"cudnn_version", "device_pci_bus_id", b"device_pci_bus_id", "instr", b"instr", "results", b"results"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["files", b"files", "frames_by_id", b"frames_by_id", "name_to_trace_id", b"name_to_trace_id", "traces", b"traces", "traces_by_id", b"traces_by_id"]) -> None: ...
 
-global___AutotuningLog = AutotuningLog
+global___GraphDebugInfo = GraphDebugInfo
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/bfc_memory_map_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/tsl/protobuf/bfc_memory_map_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/coordination_config_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/tsl/protobuf/coordination_config_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -48,14 +48,16 @@
     ENABLE_HEALTH_CHECK_FIELD_NUMBER: builtins.int
     CLUSTER_REGISTER_TIMEOUT_IN_MS_FIELD_NUMBER: builtins.int
     HEARTBEAT_TIMEOUT_IN_MS_FIELD_NUMBER: builtins.int
     COORDINATED_JOB_LIST_FIELD_NUMBER: builtins.int
     SHUTDOWN_BARRIER_TIMEOUT_IN_MS_FIELD_NUMBER: builtins.int
     AGENT_DESTRUCTION_WITHOUT_SHUTDOWN_FIELD_NUMBER: builtins.int
     RECOVERABLE_JOBS_FIELD_NUMBER: builtins.int
+    ALLOW_NEW_INCARNATION_TO_RECONNECT_FIELD_NUMBER: builtins.int
+    FORCE_DISABLE_FIELD_NUMBER: builtins.int
     service_type: builtins.str
     """Type of coordination service implementation to enable.
     For example, setting the service type as "standalone" starts a service
     instance on the leader task to provide the coordination services such as
     heartbeats and consistent key-value store.
     """
     service_leader: builtins.str
@@ -78,14 +80,25 @@
     disconnect individually.
     """
     agent_destruction_without_shutdown: builtins.bool
     """If set, agents do not make an explicit Shutdown() call. Service will only
     find out about the disconnecte agent via stale heartbeats. Used for
     testing.
     """
+    allow_new_incarnation_to_reconnect: builtins.bool
+    """If a task restarts with a new incarnation, we may allow it to reconnect
+    silently. This is useful when we know that a task can immediately resume
+    work upon re-connecting to the service.
+    """
+    force_disable: builtins.bool
+    """Disables coordination service.
+    Some libraries enable coordination service by default even if the user did
+    not specify any config. This field allows users to explicitly disable
+    coordination service under all situations.
+    """
     @property
     def coordinated_job_list(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___CoordinatedJob]: ...
     @property
     def recoverable_jobs(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """The list of jobs which are recoverable. If a task in this list fails,
         it will not propagate error to other tasks.
         If empty, no jobs will be recoverable and every task failure will cause
@@ -100,11 +113,13 @@
         enable_health_check: builtins.bool | None = ...,
         cluster_register_timeout_in_ms: builtins.int | None = ...,
         heartbeat_timeout_in_ms: builtins.int | None = ...,
         coordinated_job_list: collections.abc.Iterable[global___CoordinatedJob] | None = ...,
         shutdown_barrier_timeout_in_ms: builtins.int | None = ...,
         agent_destruction_without_shutdown: builtins.bool | None = ...,
         recoverable_jobs: collections.abc.Iterable[builtins.str] | None = ...,
+        allow_new_incarnation_to_reconnect: builtins.bool | None = ...,
+        force_disable: builtins.bool | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing.Literal["agent_destruction_without_shutdown", b"agent_destruction_without_shutdown", "cluster_register_timeout_in_ms", b"cluster_register_timeout_in_ms", "coordinated_job_list", b"coordinated_job_list", "enable_health_check", b"enable_health_check", "heartbeat_timeout_in_ms", b"heartbeat_timeout_in_ms", "recoverable_jobs", b"recoverable_jobs", "service_leader", b"service_leader", "service_type", b"service_type", "shutdown_barrier_timeout_in_ms", b"shutdown_barrier_timeout_in_ms"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["agent_destruction_without_shutdown", b"agent_destruction_without_shutdown", "allow_new_incarnation_to_reconnect", b"allow_new_incarnation_to_reconnect", "cluster_register_timeout_in_ms", b"cluster_register_timeout_in_ms", "coordinated_job_list", b"coordinated_job_list", "enable_health_check", b"enable_health_check", "force_disable", b"force_disable", "heartbeat_timeout_in_ms", b"heartbeat_timeout_in_ms", "recoverable_jobs", b"recoverable_jobs", "service_leader", b"service_leader", "service_type", b"service_type", "shutdown_barrier_timeout_in_ms", b"shutdown_barrier_timeout_in_ms"]) -> None: ...
 
 global___CoordinationServiceConfig = CoordinationServiceConfig
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/coordination_service_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/tsl/protobuf/coordination_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/distributed_runtime_payloads_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/tsl/protobuf/distributed_runtime_payloads_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/dnn_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/tsl/protobuf/dnn_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -33,28 +33,34 @@
     kInt8: _DataType.ValueType  # 3
     kInt32: _DataType.ValueType  # 4
     kComplexFloat: _DataType.ValueType  # 5
     kComplexDouble: _DataType.ValueType  # 6
     kBF16: _DataType.ValueType  # 7
     kF8E5M2: _DataType.ValueType  # 8
     kF8E4M3FN: _DataType.ValueType  # 9
+    kF8E5M2FNUZ: _DataType.ValueType  # 10
+    kF8E4M3FNUZ: _DataType.ValueType  # 11
+    kInt64: _DataType.ValueType  # 12
 
 class DataType(_DataType, metaclass=_DataTypeEnumTypeWrapper):
     """Specifies the data type used by an operation."""
 
 kFloat: DataType.ValueType  # 0
 kDouble: DataType.ValueType  # 1
 kHalf: DataType.ValueType  # 2
 kInt8: DataType.ValueType  # 3
 kInt32: DataType.ValueType  # 4
 kComplexFloat: DataType.ValueType  # 5
 kComplexDouble: DataType.ValueType  # 6
 kBF16: DataType.ValueType  # 7
 kF8E5M2: DataType.ValueType  # 8
 kF8E4M3FN: DataType.ValueType  # 9
+kF8E5M2FNUZ: DataType.ValueType  # 10
+kF8E4M3FNUZ: DataType.ValueType  # 11
+kInt64: DataType.ValueType  # 12
 global___DataType = DataType
 
 class _DataLayout:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
 class _DataLayoutEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_DataLayout.ValueType], builtins.type):
@@ -128,14 +134,18 @@
     """
     kOutputYXInput: _FilterLayout.ValueType  # 1
     """cuDNN's NHWC layout"""
     kOutputInputYX4: _FilterLayout.ValueType  # 2
     """cuDNN's NCHW_VECT_C layout with 4-elem vectors"""
     kOutputInputYX32: _FilterLayout.ValueType  # 5
     """cuDNN's NCHW_VECT_C layout with 32-elem vectors"""
+    kOutputInputYX32_CudnnReordered: _FilterLayout.ValueType  # 6
+    """cuDNN-specific filter reordering (using `cudnnReorderFilterAndBias`)
+    When the filter is reordered, so is the bias (if present).
+    """
     kInputYXOutput: _FilterLayout.ValueType  # 3
     kYXInputOutput: _FilterLayout.ValueType  # 4
 
 class FilterLayout(_FilterLayout, metaclass=_FilterLayoutEnumTypeWrapper):
     """Describes how a convolution filter is laid out in the memory."""
 
 kOutputInputYX: FilterLayout.ValueType  # 0
@@ -149,14 +159,18 @@
 """
 kOutputYXInput: FilterLayout.ValueType  # 1
 """cuDNN's NHWC layout"""
 kOutputInputYX4: FilterLayout.ValueType  # 2
 """cuDNN's NCHW_VECT_C layout with 4-elem vectors"""
 kOutputInputYX32: FilterLayout.ValueType  # 5
 """cuDNN's NCHW_VECT_C layout with 32-elem vectors"""
+kOutputInputYX32_CudnnReordered: FilterLayout.ValueType  # 6
+"""cuDNN-specific filter reordering (using `cudnnReorderFilterAndBias`)
+When the filter is reordered, so is the bias (if present).
+"""
 kInputYXOutput: FilterLayout.ValueType  # 3
 kYXInputOutput: FilterLayout.ValueType  # 4
 global___FilterLayout = FilterLayout
 
 class _ActivationMode:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
@@ -237,24 +251,44 @@
 class _ConvolutionKindEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ConvolutionKind.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     INVALID: _ConvolutionKind.ValueType  # 0
     FORWARD: _ConvolutionKind.ValueType  # 1
     BACKWARD_FILTER: _ConvolutionKind.ValueType  # 2
     BACKWARD_DATA: _ConvolutionKind.ValueType  # 3
     FORWARD_BIAS_ACTIVATION: _ConvolutionKind.ValueType  # 4
+    FORWARD_GRAPH: _ConvolutionKind.ValueType  # 5
 
 class ConvolutionKind(_ConvolutionKind, metaclass=_ConvolutionKindEnumTypeWrapper): ...
 
 INVALID: ConvolutionKind.ValueType  # 0
 FORWARD: ConvolutionKind.ValueType  # 1
 BACKWARD_FILTER: ConvolutionKind.ValueType  # 2
 BACKWARD_DATA: ConvolutionKind.ValueType  # 3
 FORWARD_BIAS_ACTIVATION: ConvolutionKind.ValueType  # 4
+FORWARD_GRAPH: ConvolutionKind.ValueType  # 5
 global___ConvolutionKind = ConvolutionKind
 
+class _FusedMHAKind:
+    ValueType = typing.NewType("ValueType", builtins.int)
+    V: typing_extensions.TypeAlias = ValueType
+
+class _FusedMHAKindEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_FusedMHAKind.ValueType], builtins.type):
+    DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+    BMM1_OUTPUT_UNKNOWN: _FusedMHAKind.ValueType  # 0
+    BMM1_OUTPUT_INPUT_TYPE: _FusedMHAKind.ValueType  # 1
+    BMM1_OUTPUT_FLOAT: _FusedMHAKind.ValueType  # 2
+
+class FusedMHAKind(_FusedMHAKind, metaclass=_FusedMHAKindEnumTypeWrapper):
+    """FusedMHAKind kind"""
+
+BMM1_OUTPUT_UNKNOWN: FusedMHAKind.ValueType  # 0
+BMM1_OUTPUT_INPUT_TYPE: FusedMHAKind.ValueType  # 1
+BMM1_OUTPUT_FLOAT: FusedMHAKind.ValueType  # 2
+global___FusedMHAKind = FusedMHAKind
+
 @typing.final
 class TensorDescriptorProto(google.protobuf.message.Message):
     """Generic tensor representation."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DIMENSIONS_FIELD_NUMBER: builtins.int
```

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/rpc_options_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/tsl/protobuf/rpc_options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/tsl/protobuf/test_log_pb2.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/tsl/protobuf/test_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240422/tensorflow-stubs/types/experimental.pyi` & `types-tensorflow-2.16.0.20240423/tensorflow-stubs/types/experimental.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 
 class Callable(Generic[_P, _R], metaclass=abc.ABCMeta):
     def __call__(self, *args: _P.args, **kwargs: _P.kwargs) -> _R: ...
 
 class ConcreteFunction(Callable[_P, _R], metaclass=abc.ABCMeta):
     def __call__(self, *args: _P.args, **kwargs: _P.kwargs) -> _R: ...
 
-class GenericFunction(Callable[_P, _R], metaclass=abc.ABCMeta):
+class PolymorphicFunction(Callable[_P, _R], metaclass=abc.ABCMeta):
     @overload
     @abc.abstractmethod
     def get_concrete_function(self, *args: _P.args, **kwargs: _P.kwargs) -> ConcreteFunction[_P, _R]: ...
     @overload
     @abc.abstractmethod
     def get_concrete_function(
         self, *args: ContainerGeneric[tf.TypeSpec[Any]], **kwargs: ContainerGeneric[tf.TypeSpec[Any]]
     ) -> ConcreteFunction[_P, _R]: ...
     def experimental_get_compiler_ir(self, *args, **kwargs): ...
 
+GenericFunction = PolymorphicFunction
+
 def __getattr__(name: str) -> Incomplete: ...
```

### Comparing `types-tensorflow-2.15.0.20240422/types_tensorflow.egg-info/PKG-INFO` & `types-tensorflow-2.16.0.20240423/types_tensorflow.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tensorflow
-Version: 2.15.0.20240422
+Version: 2.16.0.20240423
 Summary: Typing stubs for tensorflow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,22 +22,22 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tensorflow`.
 
 This version of `types-tensorflow` aims to provide accurate annotations
-for `tensorflow==2.15.*`.
+for `tensorflow==2.16.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tensorflow. All fixes for
 types and metadata should be contributed there.
 
-Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 25.1 on tensorflow==2.12.1.
+Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 25.1 on tensorflow==2.16.1 .
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1017c525f84b5e78a75ad909c6a4ef2b5c0610e6` and was tested
+This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
 pytype 2024.4.11.
```

### Comparing `types-tensorflow-2.15.0.20240422/types_tensorflow.egg-info/SOURCES.txt` & `types-tensorflow-2.16.0.20240423/types_tensorflow.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,33 +16,38 @@
 tensorflow-stubs/random.pyi
 tensorflow-stubs/raw_ops.pyi
 tensorflow-stubs/sparse.pyi
 tensorflow-stubs/strings.pyi
 tensorflow-stubs/summary.pyi
 tensorflow-stubs/autograph/__init__.pyi
 tensorflow-stubs/autograph/experimental.pyi
-tensorflow-stubs/compiler/xla/autotune_results_pb2.pyi
 tensorflow-stubs/compiler/xla/xla_data_pb2.pyi
+tensorflow-stubs/compiler/xla/xla_pb2.pyi
 tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi
+tensorflow-stubs/compiler/xla/service/hlo_profile_printer_data_pb2.pyi
 tensorflow-stubs/compiler/xla/service/metrics_pb2.pyi
+tensorflow-stubs/compiler/xla/service/test_compilation_environment_pb2.pyi
+tensorflow-stubs/compiler/xla/service/xla_compile_result_pb2.pyi
 tensorflow-stubs/config/__init__.pyi
 tensorflow-stubs/config/experimental.pyi
 tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi
 tensorflow-stubs/core/example/example_pb2.pyi
 tensorflow-stubs/core/example/feature_pb2.pyi
 tensorflow-stubs/core/framework/allocation_description_pb2.pyi
 tensorflow-stubs/core/framework/api_def_pb2.pyi
 tensorflow-stubs/core/framework/attr_value_pb2.pyi
 tensorflow-stubs/core/framework/cost_graph_pb2.pyi
+tensorflow-stubs/core/framework/cpp_shape_inference_pb2.pyi
 tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi
 tensorflow-stubs/core/framework/dataset_options_pb2.pyi
 tensorflow-stubs/core/framework/dataset_pb2.pyi
 tensorflow-stubs/core/framework/device_attributes_pb2.pyi
 tensorflow-stubs/core/framework/full_type_pb2.pyi
 tensorflow-stubs/core/framework/function_pb2.pyi
+tensorflow-stubs/core/framework/graph_debug_info_pb2.pyi
 tensorflow-stubs/core/framework/graph_pb2.pyi
 tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi
 tensorflow-stubs/core/framework/kernel_def_pb2.pyi
 tensorflow-stubs/core/framework/log_memory_pb2.pyi
 tensorflow-stubs/core/framework/model_pb2.pyi
 tensorflow-stubs/core/framework/node_def_pb2.pyi
 tensorflow-stubs/core/framework/op_def_pb2.pyi
@@ -68,26 +73,26 @@
 tensorflow-stubs/core/protobuf/data_service_pb2.pyi
 tensorflow-stubs/core/protobuf/debug_event_pb2.pyi
 tensorflow-stubs/core/protobuf/debug_pb2.pyi
 tensorflow-stubs/core/protobuf/device_filters_pb2.pyi
 tensorflow-stubs/core/protobuf/device_properties_pb2.pyi
 tensorflow-stubs/core/protobuf/error_codes_pb2.pyi
 tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi
-tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi
 tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi
 tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi
 tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi
 tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi
 tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi
 tensorflow-stubs/core/protobuf/rpc_options_pb2.pyi
 tensorflow-stubs/core/protobuf/saved_model_pb2.pyi
 tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi
 tensorflow-stubs/core/protobuf/saver_pb2.pyi
 tensorflow-stubs/core/protobuf/service_config_pb2.pyi
 tensorflow-stubs/core/protobuf/snapshot_pb2.pyi
+tensorflow-stubs/core/protobuf/status_pb2.pyi
 tensorflow-stubs/core/protobuf/struct_pb2.pyi
 tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi
 tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi
 tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi
 tensorflow-stubs/core/protobuf/transport_options_pb2.pyi
 tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi
 tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi
@@ -98,14 +103,15 @@
 tensorflow-stubs/core/util/event_pb2.pyi
 tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi
 tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi
 tensorflow-stubs/core/util/test_log_pb2.pyi
 tensorflow-stubs/data/__init__.pyi
 tensorflow-stubs/data/experimental.pyi
 tensorflow-stubs/distribute/__init__.pyi
+tensorflow-stubs/distribute/coordinator.pyi
 tensorflow-stubs/distribute/experimental/coordinator.pyi
 tensorflow-stubs/experimental/__init__.pyi
 tensorflow-stubs/experimental/dtensor.pyi
 tensorflow-stubs/feature_column/__init__.pyi
 tensorflow-stubs/io/__init__.pyi
 tensorflow-stubs/io/gfile.pyi
 tensorflow-stubs/keras/__init__.pyi
@@ -114,17 +120,14 @@
 tensorflow-stubs/keras/constraints.pyi
 tensorflow-stubs/keras/initializers.pyi
 tensorflow-stubs/keras/losses.pyi
 tensorflow-stubs/keras/metrics.pyi
 tensorflow-stubs/keras/models.pyi
 tensorflow-stubs/keras/regularizers.pyi
 tensorflow-stubs/keras/layers/__init__.pyi
-tensorflow-stubs/keras/layers/experimental/preprocessing.pyi
-tensorflow-stubs/keras/layers/preprocessing/__init__.pyi
-tensorflow-stubs/keras/layers/preprocessing/index_lookup.pyi
 tensorflow-stubs/keras/optimizers/__init__.pyi
 tensorflow-stubs/keras/optimizers/schedules.pyi
 tensorflow-stubs/keras/optimizers/legacy/__init__.pyi
 tensorflow-stubs/python/__init__.pyi
 tensorflow-stubs/python/distribute/distribute_lib.pyi
 tensorflow-stubs/python/feature_column/__init__.pyi
 tensorflow-stubs/python/feature_column/feature_column_v2.pyi
@@ -140,23 +143,24 @@
 tensorflow-stubs/python/trackable/resource.pyi
 tensorflow-stubs/python/trackable/ressource.pyi
 tensorflow-stubs/python/training/tracking/autotrackable.pyi
 tensorflow-stubs/saved_model/__init__.pyi
 tensorflow-stubs/saved_model/experimental.pyi
 tensorflow-stubs/train/__init__.pyi
 tensorflow-stubs/train/experimental.pyi
-tensorflow-stubs/tsl/protobuf/autotuning_pb2.pyi
 tensorflow-stubs/tsl/protobuf/bfc_memory_map_pb2.pyi
 tensorflow-stubs/tsl/protobuf/coordination_config_pb2.pyi
 tensorflow-stubs/tsl/protobuf/coordination_service_pb2.pyi
 tensorflow-stubs/tsl/protobuf/distributed_runtime_payloads_pb2.pyi
 tensorflow-stubs/tsl/protobuf/dnn_pb2.pyi
 tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi
 tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi
 tensorflow-stubs/tsl/protobuf/rpc_options_pb2.pyi
+tensorflow-stubs/tsl/protobuf/status_pb2.pyi
 tensorflow-stubs/tsl/protobuf/test_log_pb2.pyi
+tensorflow-stubs/types/__init__.pyi
 tensorflow-stubs/types/experimental.pyi
 types_tensorflow.egg-info/PKG-INFO
 types_tensorflow.egg-info/SOURCES.txt
 types_tensorflow.egg-info/dependency_links.txt
 types_tensorflow.egg-info/requires.txt
 types_tensorflow.egg-info/top_level.txt
```

