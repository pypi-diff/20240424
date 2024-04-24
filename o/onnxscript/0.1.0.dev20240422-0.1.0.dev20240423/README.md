# Comparing `tmp/onnxscript-0.1.0.dev20240422.tar.gz` & `tmp/onnxscript-0.1.0.dev20240423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-0.1.0.dev20240422.tar", last modified: Mon Apr 22 00:01:15 2024, max compression
+gzip compressed data, was "onnxscript-0.1.0.dev20240423.tar", last modified: Tue Apr 23 00:01:14 2024, max compression
```

## Comparing `onnxscript-0.1.0.dev20240422.tar` & `onnxscript-0.1.0.dev20240423.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.384276 onnxscript-0.1.0.dev20240422/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    10897 2024-04-22 00:01:15.380277 onnxscript-0.1.0.dev20240422/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/VERSION
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.352276 onnxscript-0.1.0.dev20240422/onnxscript/
--rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.352276 onnxscript-0.1.0.dev20240422/onnxscript/_internal/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/_internal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/_internal/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/_internal/autocast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/_internal/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/_internal/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/_internal/version_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.352276 onnxscript-0.1.0.dev20240422/onnxscript/_legacy_ir/
--rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/_legacy_ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/_legacy_ir/visitor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.352276 onnxscript-0.1.0.dev20240422/onnxscript/_thirdparty/
--rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/_thirdparty/asciichartpy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.352276 onnxscript-0.1.0.dev20240422/onnxscript/backend/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/backend/onnx_export.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/converter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.344276 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.356276 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.364276 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/evaluator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.348276 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.348276 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/tools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.364276 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.364276 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/_flags.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.364276 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/graph_building/
--rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/graph_building/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27757 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.368276 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/ops/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/ops/vision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/tensor_typing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.372276 onnxscript-0.1.0.dev20240422/onnxscript/ir/
--rw-r--r--   0 vsts      (1001) docker     (127)     2394 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    73221 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/ir/_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/ir/_display.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3908 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/ir/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/ir/_graph_comparison.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/ir/_invariants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10417 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/ir/_linked_list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/ir/_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/ir/_name_authority.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19580 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/ir/_protocols.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1489 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/ir/convenience.py
--rw-r--r--   0 vsts      (1001) docker     (127)    46998 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/ir/serde.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.372276 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/
--rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.376276 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset20.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/onnx_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.376276 onnxscript-0.1.0.dev20240422/onnxscript/optimizer/
--rw-r--r--   0 vsts      (1001) docker     (127)     4316 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/optimizer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/optimizer/constant_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/optimizer/copy_propagation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/optimizer/evaluator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/optimizer/fold_constants_v0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/optimizer/remove_unused.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/optimizer/remove_unused_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/optimizer/simple_function_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.380277 onnxscript-0.1.0.dev20240422/onnxscript/rewriter/
--rw-r--r--   0 vsts      (1001) docker     (127)     1375 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/rewriter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/rewriter/_ir_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2831 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/rewriter/_tape.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6926 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/rewriter/broadcast_to_matmul.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2170 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/rewriter/cast_constant_of_shape.py
--rw-r--r--   0 vsts      (1001) docker     (127)      686 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/rewriter/erfgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8918 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/rewriter/function_rule.py
--rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/rewriter/gemm_to_matmul_add.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36273 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/rewriter/generic_pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/rewriter/no_op.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.380277 onnxscript-0.1.0.dev20240422/onnxscript/rewriter/onnxruntime/
--rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/rewriter/onnxruntime/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1222 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5746 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1922 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/rewriter/onnxruntime/softmax.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.380277 onnxscript-0.1.0.dev20240422/onnxscript/rewriter/onnxruntime/transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)      543 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/rewriter/onnxruntime/transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1097 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1628 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24688 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)    42362 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/rewriter/pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/sourceinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/tensor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.380277 onnxscript-0.1.0.dev20240422/onnxscript/testing/
--rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/type_annotation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.380277 onnxscript-0.1.0.dev20240422/onnxscript/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/utils/evaluation_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/utils/timing_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/utils/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/onnxscript/values.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 00:01:15.380277 onnxscript-0.1.0.dev20240422/onnxscript.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    10897 2024-04-22 00:01:15.000000 onnxscript-0.1.0.dev20240422/onnxscript.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8202 2024-04-22 00:01:15.000000 onnxscript-0.1.0.dev20240422/onnxscript.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-22 00:01:15.000000 onnxscript-0.1.0.dev20240422/onnxscript.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-22 00:01:15.000000 onnxscript-0.1.0.dev20240422/onnxscript.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-22 00:01:15.000000 onnxscript-0.1.0.dev20240422/onnxscript.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-22 00:01:15.384276 onnxscript-0.1.0.dev20240422/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1292 2024-04-22 00:00:49.000000 onnxscript-0.1.0.dev20240422/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.036362 onnxscript-0.1.0.dev20240423/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    10897 2024-04-23 00:01:14.036362 onnxscript-0.1.0.dev20240423/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/VERSION
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:13.988362 onnxscript-0.1.0.dev20240423/onnxscript/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:13.992362 onnxscript-0.1.0.dev20240423/onnxscript/_internal/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_internal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_internal/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_internal/autocast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_internal/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_internal/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_internal/version_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:13.992362 onnxscript-0.1.0.dev20240423/onnxscript/_legacy_ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_legacy_ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_legacy_ir/visitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:13.992362 onnxscript-0.1.0.dev20240423/onnxscript/_thirdparty/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/_thirdparty/asciichartpy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:13.996362 onnxscript-0.1.0.dev20240423/onnxscript/backend/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/converter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:13.980362 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:13.996362 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.008362 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/evaluator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:13.980362 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:13.980362 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/tools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.012362 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.012362 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/_flags.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.012362 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/graph_building/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/graph_building/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27757 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.016362 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/vision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/tensor_typing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.020362 onnxscript-0.1.0.dev20240423/onnxscript/ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2394 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8489 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/_convenience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    77495 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/_display.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3908 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/_graph_comparison.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/_invariants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10417 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/_linked_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/_name_authority.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19580 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/_protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    47188 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/ir/serde.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.020362 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.028362 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset20.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/onnx_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.028362 onnxscript-0.1.0.dev20240423/onnxscript/optimizer/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4316 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/optimizer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/optimizer/constant_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/optimizer/copy_propagation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/optimizer/evaluator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/optimizer/fold_constants_v0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/optimizer/remove_unused.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/optimizer/remove_unused_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/optimizer/simple_function_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.032362 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1375 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/_ir_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/_tape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6926 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/broadcast_to_matmul.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2170 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/cast_constant_of_shape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      686 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/erfgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8918 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/function_rule.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/gemm_to_matmul_add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36273 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/generic_pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/no_op.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.032362 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1222 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5746 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1922 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/softmax.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.036362 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      543 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1097 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1628 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24688 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41992 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/rewriter/pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/sourceinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/tensor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.036362 onnxscript-0.1.0.dev20240423/onnxscript/testing/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/type_annotation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.036362 onnxscript-0.1.0.dev20240423/onnxscript/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/utils/evaluation_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/utils/timing_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/utils/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/onnxscript/values.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-23 00:01:14.036362 onnxscript-0.1.0.dev20240423/onnxscript.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10897 2024-04-23 00:01:13.000000 onnxscript-0.1.0.dev20240423/onnxscript.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8203 2024-04-23 00:01:13.000000 onnxscript-0.1.0.dev20240423/onnxscript.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-23 00:01:13.000000 onnxscript-0.1.0.dev20240423/onnxscript.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-23 00:01:13.000000 onnxscript-0.1.0.dev20240423/onnxscript.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-23 00:01:13.000000 onnxscript-0.1.0.dev20240423/onnxscript.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-23 00:01:14.036362 onnxscript-0.1.0.dev20240423/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1292 2024-04-23 00:00:58.000000 onnxscript-0.1.0.dev20240423/setup.py
```

### Comparing `onnxscript-0.1.0.dev20240422/LICENSE` & `onnxscript-0.1.0.dev20240423/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/PKG-INFO` & `onnxscript-0.1.0.dev20240423/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240422
+Version: 0.1.0.dev20240423
 Summary: Naturally author ONNX functions and models using a subset of Python
 Home-page: https://onnxscript.ai/
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
```

### Comparing `onnxscript-0.1.0.dev20240422/README.md` & `onnxscript-0.1.0.dev20240423/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/__init__.py` & `onnxscript-0.1.0.dev20240423/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/_internal/analysis.py` & `onnxscript-0.1.0.dev20240423/onnxscript/_internal/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/_internal/ast_utils.py` & `onnxscript-0.1.0.dev20240423/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/_internal/autocast.py` & `onnxscript-0.1.0.dev20240423/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/_internal/deprecation.py` & `onnxscript-0.1.0.dev20240423/onnxscript/_internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/_internal/param_manipulation.py` & `onnxscript-0.1.0.dev20240423/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/_internal/runtime_typing.py` & `onnxscript-0.1.0.dev20240423/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/_internal/utils.py` & `onnxscript-0.1.0.dev20240423/onnxscript/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/_internal/version_utils.py` & `onnxscript-0.1.0.dev20240423/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/_legacy_ir/__init__.py` & `onnxscript-0.1.0.dev20240423/onnxscript/_legacy_ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/_legacy_ir/visitor.py` & `onnxscript-0.1.0.dev20240423/onnxscript/_legacy_ir/visitor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/_thirdparty/asciichartpy.py` & `onnxscript-0.1.0.dev20240423/onnxscript/_thirdparty/asciichartpy.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/backend/onnx_backend.py` & `onnxscript-0.1.0.dev20240423/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/backend/onnx_export.py` & `onnxscript-0.1.0.dev20240423/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/converter.py` & `onnxscript-0.1.0.dev20240423/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/context.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/diagnostics/infra/utils.py` & `onnxscript-0.1.0.dev20240423/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/evaluator.py` & `onnxscript-0.1.0.dev20240423/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py` & `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/_flags.py` & `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/_flags.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/graph_building/__init__.py` & `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/graph_building/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py` & `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py` & `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/ops/common.py` & `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/ops/vision.py` & `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/ops/vision.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-0.1.0.dev20240423/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/ir/__init__.py` & `onnxscript-0.1.0.dev20240423/onnxscript/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/ir/_core.py` & `onnxscript-0.1.0.dev20240423/onnxscript/ir/_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import math
 import mmap
 import os
 import sys
 import textwrap
 import typing
 from typing import (
+    AbstractSet,
     Any,
     Collection,
     Generic,
     Iterable,
     Iterator,
     OrderedDict,
     Sequence,
@@ -80,15 +81,15 @@
     def _printable_type_shape(self) -> str:
         """Return a string representation of the shape and data type."""
         return f"{self.dtype},{self.shape}"
 
     def _repr_base(self) -> str:
         """Base string for the repr method.
 
-        Example: Tensor<FLOAT:=1,5x42>
+        Example: Tensor<FLOAT,[5,42]>
         """
         return f"{self.__class__.__name__}<{self._printable_type_shape()}>"
 
     @property
     def size(self) -> int:
         """The number of elements in the tensor."""
         return np.prod(self.shape.numpy())  # type: ignore[return-value,attr-defined]
@@ -235,15 +236,15 @@
 
     def __dlpack_device__(self) -> tuple[int, int]:
         if _compatible_with_dlpack(self._raw):
             return self._raw.__dlpack_device__()
         return self.__array__().__dlpack_device__()
 
     def __repr__(self) -> str:
-        return f"{self._repr_base()}({self._raw!r})"
+        return f"{self._repr_base()}({self._raw!r}, name={self.name!r})"
 
     @property
     def dtype(self) -> _enums.DataType:
         """The data type of the tensor. Immutable."""
         return self._dtype
 
     @property
@@ -1232,14 +1233,50 @@
     ) -> None:
         super().__init__(None, index=None)
         self._name = name
         self._shape = shape
         self._type = type
 
 
+def _check_node_safe_to_remove(
+    node: Node, to_remove: AbstractSet[Node], graph_outputs: AbstractSet[Value]
+) -> None:
+    """Check if a node is safe to remove.
+
+    1. It checks to make sure there are no users of the node that are not
+        to be removed before removing it.
+    2. It checks the node does not contribute to any graph outputs.
+
+    This check is typically O(1) assuming the number of consumers of the node is small
+
+    Args:
+        node: The node to check.
+        to_remove: A set of nodes that are to be removed.
+            This set is used to check if the node is still being used by other
+            nodes that are not to be removed.
+        graph_outputs: A set of values that are outputs of the graph.
+
+    Raises:
+        ValueError: If the node does not belong to this graph or if there are users of the node.
+        ValueError: If the node is still being used by other nodes not to be removed.
+    """
+    for output in node.outputs:
+        if output in graph_outputs:
+            raise ValueError(
+                f"Node '{node!r}' is still an output of the graph and cannot be removed when safe=True."
+            )
+        for consumer, _ in output.consumers():
+            if consumer in to_remove:
+                continue
+            raise ValueError(
+                f"Node '{consumer!r}' is still being used by other nodes that are not to be "
+                f"removed. All of its uses: {list(output.consumers())!r}"
+            )
+
+
 class Graph(_protocols.GraphProtocol, Sequence[Node], _display.PrettyPrintable):
     """IR Graph.
 
     Graph represents a computation graph. In addition to the ONNX specification
     specified fields, it also contains a mapping of :attr:`opset_imports`. This
     allows different subgraphs to import different opsets. It is the responsibility
     of the deserializer to reconcile the different opsets.
@@ -1350,15 +1387,15 @@
     def __reversed__(self) -> Iterator[Node]:
         return reversed(self._nodes)
 
     def _set_node_graph_to_self_and_assign_names(self, node: Node) -> Node:
         """Set the graph reference for the node and assign names to it and its outputs if they don't have one."""
         if node.graph is not None and node.graph is not self:
             raise ValueError(
-                f"The node {node} belongs to another graph. Please remove it first with Graph.remove()."
+                f"The node '{node!r}' belongs to another graph. Please remove it first with Graph.remove()."
             )
         # Give the node and its output values names if they don't not have one
         if node.name is None:
             self._name_authority.name_node(node)
         for value in node._outputs:  # pylint: disable=protected-access
             if value.name is None:
                 self._name_authority.name_value(value)
@@ -1386,27 +1423,52 @@
 
         Raises:
             ValueError: If any node belongs to another graph.
         """
         nodes = [self._set_node_graph_to_self_and_assign_names(node) for node in nodes]
         self._nodes.extend(nodes)
 
-    def remove(self, node: Node, /) -> None:
-        """Remove a node from the graph in O(1) time.
+    def remove(self, nodes: Node | Iterable[Node], /, safe: bool = False) -> None:
+        """Remove nodes from the graph in O(#num of nodes) time.
+
+        If any errors are raise, to ensure the graph is not left in an inconsistent state,
+        the graph is not modified.
 
         Args:
-            node: The node to remove.
+            nodes: The node to remove.
+            safe: If True, performs the following actions before removal:
+                1. It checks to make sure there are no users of the node that are not
+                    to be removed before removing it.
+                2. It checks the node does not contribute to any graph outputs.
+                3. It removes references to all inputs so it is no longer a user of other nodes.
 
         Raises:
-            ValueError: If the node does not belong to this graph.
+            ValueError: If any node to remove does not belong to this graph.
+            ValueError: (When ``safe=True``) If the node does not belong to this graph or if there are users of the node.
+            ValueError: (When ``safe=True``) If the node is still being used by other nodes not to be removed.
         """
-        if node.graph is not self:
-            raise ValueError(f"The node {node} does not belong to this graph.")
-        node.graph = None
-        self._nodes.remove(node)
+        if not isinstance(nodes, Iterable):
+            nodes_set: AbstractSet[Node] = {nodes}
+        else:
+            nodes_set = frozenset(nodes)
+        graph_outputs = frozenset(self.outputs)
+        for node in nodes_set:
+            if node.graph is not self:
+                raise ValueError(f"The node '{node!r}' does not belong to this graph.")
+            if safe:
+                # Check 1, 2
+                _check_node_safe_to_remove(node, nodes_set, graph_outputs)
+        for node in nodes_set:
+            if safe:
+                # 3. Detach from all inputs so that it is no longer a user of other nodes
+                for i in range(len(node.inputs)):
+                    node.replace_input_with(i, None)
+            # Set attributes to remove the node from this graph
+            node.graph = None
+            self._nodes.remove(node)
 
     def insert_after(self, node: Node, new_nodes: Iterable[Node] | Node, /) -> None:
         """Insert new nodes after the given node in O(#new_nodes) time.
 
         Args:
             node: The node to insert after.
             new_nodes: The new nodes to insert.
@@ -1874,17 +1936,34 @@
         """Append a node to the function in O(1) time."""
         self._graph.append(node)
 
     def extend(self, nodes: Iterable[Node], /) -> None:
         """Extend the function with the given nodes in O(#new_nodes) time."""
         self._graph.extend(nodes)
 
-    def remove(self, node: Node, /) -> None:
-        """Remove a node from the function in O(1) time."""
-        self._graph.remove(node)
+    def remove(self, nodes: Node | Iterable[Node], /, safe: bool = False) -> None:
+        """Remove nodes from the graph in O(#num of nodes) time.
+
+        If any errors are raise, to ensure the graph is not left in an inconsistent state,
+        the graph is not modified.
+
+        Args:
+            nodes: The node to remove.
+            safe: If True, performs the following actions before removal:
+                1. It checks to make sure there are no users of the node that are not
+                    to be removed before removing it.
+                2. It checks the node does not contribute to any graph outputs.
+                3. It removes references to all inputs so it is no longer a user of other nodes.
+
+        Raises:
+            ValueError: If any node to remove does not belong to this graph.
+            ValueError: (When ``safe=True``) If the node does not belong to this graph or if there are users of the node.
+            ValueError: (When ``safe=True``) If the node is still being used by other nodes not to be removed.
+        """
+        self._graph.remove(nodes, safe=safe)
 
     def insert_after(self, node: Node, new_nodes: Iterable[Node], /) -> None:
         """Insert new nodes after the given node in O(#new_nodes) time."""
         self._graph.insert_after(node, new_nodes)
 
     def insert_before(self, node: Node, new_nodes: Iterable[Node], /) -> None:
         """Insert new nodes before the given node in O(#new_nodes) time."""
@@ -2025,63 +2104,68 @@
     def __str__(self) -> str:
         return str(self.value)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.name!r}, {self.type!r}, {self.value!r})"
 
 
+class _SpecializedAttr(Attr):
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}({self.name!r}, {self.value!r})"
+
+
 # NOTE: The following classes are just supporting classes (partially applied) for convenience
 # But I think they would be useful to have in the IR by having the type info
 # explicitly in the class type.
-class AttrFloat32(Attr):
+class AttrFloat32(_SpecializedAttr):
     def __init__(self, name: str, value: float, doc_string: str | None = None):
         super().__init__(
             name,
             _enums.AttributeType.FLOAT,
             value,
             doc_string=doc_string,
         )
 
 
-class AttrInt64(Attr):
+class AttrInt64(_SpecializedAttr):
     def __init__(self, name: str, value: int, doc_string: str | None = None):
         super().__init__(
             name,
             _enums.AttributeType.INT,
             value,
             doc_string=doc_string,
         )
 
 
-class AttrString(Attr):
+class AttrString(_SpecializedAttr):
     def __init__(self, name: str, value: str, doc_string: str | None = None):
         super().__init__(
             name,
             _enums.AttributeType.STRING,
             value,
             doc_string=doc_string,
         )
 
 
-class AttrTensor(Attr):
+class AttrTensor(_SpecializedAttr):
     def __init__(
         self,
         name: str,
         value: _protocols.TensorProtocol,
         doc_string: str | None = None,
     ):
         super().__init__(
             name,
             _enums.AttributeType.TENSOR,
             value,
             doc_string=doc_string,
         )
 
 
-class AttrGraph(Attr):
+class AttrGraph(_SpecializedAttr):
     def __init__(
         self,
         name: str,
         value: Graph,
         doc_string: str | None = None,
     ):
         super().__init__(
@@ -2091,75 +2175,75 @@
             doc_string=doc_string,
         )
 
     def __str__(self) -> str:
         return textwrap.indent("\n" + super().__str__(), " " * 4)
 
 
-class AttrFloat32s(Attr):
+class AttrFloat32s(_SpecializedAttr):
     def __init__(
         self,
         name: str,
         value: Sequence[float],
         doc_string: str | None = None,
     ):
         super().__init__(
             name,
             _enums.AttributeType.FLOATS,
             value,
             doc_string=doc_string,
         )
 
 
-class AttrInt64s(Attr):
+class AttrInt64s(_SpecializedAttr):
     def __init__(
         self,
         name: str,
         value: Sequence[int],
         doc_string: str | None = None,
     ):
         super().__init__(
             name,
             _enums.AttributeType.INTS,
             value,
             doc_string=doc_string,
         )
 
 
-class AttrStrings(Attr):
+class AttrStrings(_SpecializedAttr):
     def __init__(
         self,
         name: str,
         value: Sequence[str],
         doc_string: str | None = None,
     ):
         super().__init__(
             name,
             _enums.AttributeType.STRINGS,
             value,
             doc_string=doc_string,
         )
 
 
-class AttrTensors(Attr):
+class AttrTensors(_SpecializedAttr):
     def __init__(
         self,
         name: str,
         value: Sequence[_protocols.TensorProtocol],
         doc_string: str | None = None,
     ):
         super().__init__(
             name,
             _enums.AttributeType.TENSORS,
             value,
             doc_string=doc_string,
         )
 
 
-class AttrGraphs(Attr):
+class AttrGraphs(_SpecializedAttr):
     def __init__(
         self,
         name: str,
         value: Sequence[Graph],
         doc_string: str | None = None,
     ):
         super().__init__(
@@ -2167,45 +2251,45 @@
             _enums.AttributeType.GRAPHS,
             value,
             doc_string=doc_string,
         )
 
 
 # NOTE: SparseTensor should be a sparse tensor proto
-class AttrSparseTensor(Attr):
+class AttrSparseTensor(_SpecializedAttr):
     def __init__(
         self,
         name: str,
         value: Sequence[_protocols.SparseTensorProtocol],
         doc_string: str | None = None,
     ):
         super().__init__(
             name,
             _enums.AttributeType.SPARSE_TENSOR,
             value,
             doc_string=doc_string,
         )
 
 
-class AttrSparseTensors(Attr):
+class AttrSparseTensors(_SpecializedAttr):
     def __init__(
         self,
         name: str,
         value: Sequence[_protocols.SparseTensorProtocol],
         doc_string: str | None = None,
     ):
         super().__init__(
             name,
             _enums.AttributeType.SPARSE_TENSORS,
             value,
             doc_string=doc_string,
         )
 
 
-class AttrTypeProto(Attr):
+class AttrTypeProto(_SpecializedAttr):
     def __init__(
         self,
         name: str,
         value: _protocols.TypeProtocol,
         doc_string: str | None = None,
     ):
         # TODO(justinchuby): Include shape as well
```

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/ir/_display.py` & `onnxscript-0.1.0.dev20240423/onnxscript/ir/_display.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/ir/_enums.py` & `onnxscript-0.1.0.dev20240423/onnxscript/ir/_enums.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/ir/_graph_comparison.py` & `onnxscript-0.1.0.dev20240423/onnxscript/ir/_graph_comparison.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/ir/_invariants.py` & `onnxscript-0.1.0.dev20240423/onnxscript/ir/_invariants.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/ir/_linked_list.py` & `onnxscript-0.1.0.dev20240423/onnxscript/ir/_linked_list.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/ir/_metadata.py` & `onnxscript-0.1.0.dev20240423/onnxscript/ir/_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/ir/_name_authority.py` & `onnxscript-0.1.0.dev20240423/onnxscript/ir/_name_authority.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/ir/_protocols.py` & `onnxscript-0.1.0.dev20240423/onnxscript/ir/_protocols.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/ir/serde.py` & `onnxscript-0.1.0.dev20240423/onnxscript/ir/serde.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,18 @@
         return self._proto.doc_string
 
     @property
     def raw(self) -> onnx.TensorProto:
         return self._proto
 
     def __repr__(self) -> str:
-        return f"{self._repr_base()}({self.name!r})"
+        # It is a little hard to display the content when there can be types
+        # unsupported by numpy
+        # Preferably we should display some content when the tensor is small
+        return f"{self._repr_base()}(name={self.name!r})"
 
     def __array__(self, dtype: Any = None) -> np.ndarray:
         """Return the tensor as a numpy array, compatible with np.array."""
         return self.numpy().__array__(dtype)
 
     def numpy(self) -> np.ndarray:
         """Return the tensor as a numpy array."""
```

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/irbuilder.py` & `onnxscript-0.1.0.dev20240423/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/main.py` & `onnxscript-0.1.0.dev20240423/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/__init__.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset20.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset20.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/onnx_types.py` & `onnxscript-0.1.0.dev20240423/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/optimizer/__init__.py` & `onnxscript-0.1.0.dev20240423/onnxscript/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/optimizer/constant_folding.py` & `onnxscript-0.1.0.dev20240423/onnxscript/optimizer/constant_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/optimizer/copy_propagation.py` & `onnxscript-0.1.0.dev20240423/onnxscript/optimizer/copy_propagation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/optimizer/evaluator.py` & `onnxscript-0.1.0.dev20240423/onnxscript/optimizer/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/optimizer/fold_constants_v0.py` & `onnxscript-0.1.0.dev20240423/onnxscript/optimizer/fold_constants_v0.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/optimizer/remove_unused.py` & `onnxscript-0.1.0.dev20240423/onnxscript/optimizer/remove_unused.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/optimizer/remove_unused_function.py` & `onnxscript-0.1.0.dev20240423/onnxscript/optimizer/remove_unused_function.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/optimizer/simple_function_folding.py` & `onnxscript-0.1.0.dev20240423/onnxscript/optimizer/simple_function_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/rewriter/__init__.py` & `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/rewriter/_ir_utils.py` & `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/_ir_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/rewriter/_tape.py` & `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/_tape.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,18 @@
 """Convenience methods for constructing the IR."""
 
 # NOTE: This is a temporary solution for constructing the IR. It should be replaced
 # with a more permanent solution in the future.
 
 from __future__ import annotations
 
-from typing import Any, Iterable, Mapping, Sequence
-
-import onnx
+from typing import Iterable, Mapping, Sequence
 
 from onnxscript import ir
-
-
-def _convert_attributes(attrs: Mapping[str, Any]) -> list[ir.Attr]:
-    attributes: list[ir.Attr] = []
-    for name, attr in attrs.items():
-        if isinstance(attr, int):
-            attributes.append(ir.AttrInt64(name, attr))
-        elif isinstance(attr, float):
-            attributes.append(ir.AttrFloat32(name, attr))
-        elif isinstance(attr, str):
-            attributes.append(ir.AttrString(name, attr))
-        elif isinstance(attr, Sequence) and all(isinstance(x, int) for x in attr):
-            attributes.append(ir.AttrInt64s(name, attr))
-        elif isinstance(attr, Sequence) and all(isinstance(x, float) for x in attr):
-            attributes.append(ir.AttrFloat32s(name, attr))
-        elif isinstance(attr, Sequence) and all(isinstance(x, str) for x in attr):
-            attributes.append(ir.AttrStrings(name, attr))
-        elif isinstance(attr, ir.Attr):
-            attributes.append(attr)
-        elif isinstance(attr, onnx.TensorProto):
-            attributes.append(ir.AttrTensor(name, ir.serde.TensorProtoTensor(attr)))
-        else:
-            raise TypeError(f"Unsupported attribute type: '{type(attr)}'")
-    return attributes
+from onnxscript.ir import _convenience
 
 
 class Tape(Iterable[ir.Node]):
     """A tape for recording nodes that are created."""
 
     def __init__(self) -> None:
         self._nodes: list[ir.Node] = []
@@ -49,36 +24,36 @@
     def nodes(self) -> Sequence[ir.Node]:
         return tuple(self._nodes)
 
     def op(
         self,
         op_type: str,
         inputs: Sequence[ir.Value | None],
-        attributes: Mapping[str, Any] | None = None,
+        attributes: Mapping[str, _convenience.SupportedAttrTypes] | None = None,
         domain: str = "",
     ) -> ir.Value:
         if attributes is None:
-            attrs: Sequence[ir.Attr] = ()
+            attrs: Sequence[ir.Attr | ir.RefAttr] = ()
         else:
-            attrs = _convert_attributes(attributes)
+            attrs = _convenience.convert_attributes(attributes)
         node = ir.Node(domain, op_type, inputs, attributes=attrs, num_outputs=1)
         self._nodes.append(node)
 
         return node.outputs[0]
 
     def op_multi_output(
         self,
         op_type: str,
         inputs: Sequence[ir.Value | None],
-        attributes: Mapping[str, Any] | None = None,
+        attributes: Mapping[str, _convenience.SupportedAttrTypes] | None = None,
         *,
         num_outputs: int,
         domain: str = "",
     ) -> Sequence[ir.Value]:
         if attributes is None:
-            attrs = ()
+            attrs: Sequence[ir.Attr | ir.RefAttr] = ()
         else:
-            attrs = _convert_attributes(attributes)  # type: ignore[assignment]
+            attrs = _convenience.convert_attributes(attributes)
         node = ir.Node(domain, op_type, inputs, attributes=attrs, num_outputs=num_outputs)
         self._nodes.append(node)
 
         return node.outputs
```

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/rewriter/broadcast_to_matmul.py` & `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/broadcast_to_matmul.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/rewriter/cast_constant_of_shape.py` & `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/cast_constant_of_shape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/rewriter/erfgelu.py` & `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/erfgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/rewriter/function_rule.py` & `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/function_rule.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/rewriter/gemm_to_matmul_add.py` & `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/gemm_to_matmul_add.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/rewriter/generic_pattern.py` & `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/generic_pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/rewriter/no_op.py` & `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/no_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/rewriter/onnxruntime/__init__.py` & `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py` & `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py` & `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/rewriter/onnxruntime/softmax.py` & `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/softmax.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/rewriter/onnxruntime/transformers/__init__.py` & `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py` & `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py` & `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/rewriter/onnxruntime/transformers/layernorm.py` & `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/transformers/layernorm.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py` & `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/rewriter/pattern.py` & `onnxscript-0.1.0.dev20240423/onnxscript/rewriter/pattern.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import numpy as np
 import onnx
 import onnx.numpy_helper
 import onnx.printer
 
 from onnxscript import ir
+from onnxscript.ir import _convenience
 from onnxscript.rewriter import _ir_utils
 
 # Overview of the pattern module: The classes below are used to define both
 # patterns (that we search for) and replacements for rewrite rules.
 # The matches() method of a pattern is used to check if an IR component
 # matches the pattern.
 # The to_ir() method of a pattern is used to create a new IR component
@@ -1019,47 +1020,38 @@
             # However, we merge the last deleted node and last inserted node
             # to avoid replacing the values produced by the last deleted node
             # in all places where they are used. So, we reuse the output
             # values from the last deleted node and replace the node itself
             # TODO: simplify this
             last_deleted = deleted_nodes[-1]
             last_inserted = inserted_nodes[-1]
-            assert len(last_deleted.outputs) == len(last_inserted.outputs)
             # Reconnect the users of the deleted node to use the new outputs
-            for last_deleted_output, last_inserted_output in zip(
-                last_deleted.outputs, last_inserted.outputs
-            ):
-                for node, index in tuple(last_deleted_output.consumers()):
-                    # Fix consumers because we are mutating consumers in the loop
-                    node.replace_input_with(index, last_inserted_output)
-
-                # Update graph/function outputs if the node generates output
-                for old_output, new_output in zip(last_deleted.outputs, last_inserted.outputs):
-                    for idx, graph_or_function_output in enumerate(graph_or_function.outputs):
-                        if graph_or_function_output is old_output:
-                            graph_or_function.outputs[idx] = new_output
+            _convenience.replace_all_uses_with(last_deleted.outputs, last_inserted.outputs)
+            # Update graph/function outputs if the node generates output
+            replacement_mapping = dict(zip(last_deleted.outputs, last_inserted.outputs))
+            for idx, graph_or_function_output in enumerate(graph_or_function.outputs):
+                if graph_or_function_output in replacement_mapping:
+                    graph_or_function.outputs[idx] = replacement_mapping[
+                        graph_or_function_output
+                    ]
 
             # insert new nodes after the index node
-            # TODO(justinchuby): Do not access by index [i]
-            graph_or_function.insert_after(graph_or_function[i], inserted_nodes)
-
-            for old_node in deleted_nodes:
-                graph_or_function.remove(old_node)
+            graph_or_function.insert_after(last_deleted, inserted_nodes)
+            graph_or_function.remove(deleted_nodes, safe=True)
 
     for replaced_node, inserted_nodes in to_insert:
         graph_or_function.insert_after(replaced_node, inserted_nodes)
         # TODO: improve this
         # This is updating the graph/function outputs to use the new outputs
         for inserted_node in inserted_nodes:
             for new_output in inserted_node.outputs:
                 if (index := new_output.meta.get(_ir_utils.GRAPH_OUTPUT_META_KEY)) is not None:  # type: ignore[assignment]
                     graph_or_function.outputs[index] = new_output
 
-    for n in to_delete:
-        graph_or_function.remove(n)
+    graph_or_function.remove(to_delete, safe=True)
 
 
 class RewriteRuleSet:
     def __init__(self, rules: Sequence[RewriteRule], *, commute: bool = False) -> None:
         if commute:
             rules = list(itertools.chain.from_iterable([rule.commute() for rule in rules]))
         self.rules = rules
```

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/sourceinfo.py` & `onnxscript-0.1.0.dev20240423/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/tensor.py` & `onnxscript-0.1.0.dev20240423/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/testing/__init__.py` & `onnxscript-0.1.0.dev20240423/onnxscript/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/type_annotation.py` & `onnxscript-0.1.0.dev20240423/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/utils/evaluation_utils.py` & `onnxscript-0.1.0.dev20240423/onnxscript/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/utils/timing_utils.py` & `onnxscript-0.1.0.dev20240423/onnxscript/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/utils/utils.py` & `onnxscript-0.1.0.dev20240423/onnxscript/utils/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript/values.py` & `onnxscript-0.1.0.dev20240423/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript.egg-info/PKG-INFO` & `onnxscript-0.1.0.dev20240423/onnxscript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240422
+Version: 0.1.0.dev20240423
 Summary: Naturally author ONNX functions and models using a subset of Python
 Home-page: https://onnxscript.ai/
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
```

### Comparing `onnxscript-0.1.0.dev20240422/onnxscript.egg-info/SOURCES.txt` & `onnxscript-0.1.0.dev20240423/onnxscript.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -115,24 +115,24 @@
 onnxscript/function_libs/torch_lib/ops/nested.py
 onnxscript/function_libs/torch_lib/ops/nn.py
 onnxscript/function_libs/torch_lib/ops/prims.py
 onnxscript/function_libs/torch_lib/ops/sparse.py
 onnxscript/function_libs/torch_lib/ops/special.py
 onnxscript/function_libs/torch_lib/ops/vision.py
 onnxscript/ir/__init__.py
+onnxscript/ir/_convenience.py
 onnxscript/ir/_core.py
 onnxscript/ir/_display.py
 onnxscript/ir/_enums.py
 onnxscript/ir/_graph_comparison.py
 onnxscript/ir/_invariants.py
 onnxscript/ir/_linked_list.py
 onnxscript/ir/_metadata.py
 onnxscript/ir/_name_authority.py
 onnxscript/ir/_protocols.py
-onnxscript/ir/convenience.py
 onnxscript/ir/serde.py
 onnxscript/onnx_opset/__init__.py
 onnxscript/onnx_opset/_impl/opset1.py
 onnxscript/onnx_opset/_impl/opset10.py
 onnxscript/onnx_opset/_impl/opset11.py
 onnxscript/onnx_opset/_impl/opset12.py
 onnxscript/onnx_opset/_impl/opset13.py
```

### Comparing `onnxscript-0.1.0.dev20240422/pyproject.toml` & `onnxscript-0.1.0.dev20240423/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240422/setup.py` & `onnxscript-0.1.0.dev20240423/setup.py`

 * *Files identical despite different names*

