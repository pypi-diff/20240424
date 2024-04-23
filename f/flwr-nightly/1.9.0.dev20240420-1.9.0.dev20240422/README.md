# Comparing `tmp/flwr_nightly-1.9.0.dev20240420.tar.gz` & `tmp/flwr_nightly-1.9.0.dev20240422.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.9.0.dev20240420.tar", max compression
+gzip compressed data, was "flwr_nightly-1.9.0.dev20240422.tar", max compression
```

## Comparing `flwr_nightly-1.9.0.dev20240420.tar` & `flwr_nightly-1.9.0.dev20240422.tar`

### file list

```diff
@@ -1,211 +1,211 @@
--rw-r--r--   0        0        0    11358 2024-04-20 23:05:17.316061 flwr_nightly-1.9.0.dev20240420/LICENSE
--rw-r--r--   0        0        0    12916 2024-04-20 23:05:17.316061 flwr_nightly-1.9.0.dev20240420/README.md
--rw-r--r--   0        0        0     5883 2024-04-20 23:05:29.468123 flwr_nightly-1.9.0.dev20240420/pyproject.toml
--rw-r--r--   0        0        0      937 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/__init__.py
--rw-r--r--   0        0        0      720 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/__init__.py
--rw-r--r--   0        0        0     1095 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/app.py
--rw-r--r--   0        0        0     5597 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/config_utils.py
--rw-r--r--   0        0        0     2215 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/example.py
--rw-r--r--   0        0        0      789 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/__init__.py
--rw-r--r--   0        0        0     5380 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/new.py
--rw-r--r--   0        0        0      725 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/__init__.py
--rw-r--r--   0        0        0     3078 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/.gitignore.tpl
--rw-r--r--   0        0        0      668 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/README.md.tpl
--rw-r--r--   0        0        0      729 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/__init__.py
--rw-r--r--   0        0        0      736 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/code/__init__.py
--rw-r--r--   0        0        0       21 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
--rw-r--r--   0        0        0      521 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
--rw-r--r--   0        0        0     1173 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
--rw-r--r--   0        0        0     1911 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
--rw-r--r--   0        0        0      248 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
--rw-r--r--   0        0        0      594 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
--rw-r--r--   0        0        0      371 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
--rw-r--r--   0        0        0     3684 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
--rw-r--r--   0        0        0      489 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
--rw-r--r--   0        0        0      558 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
--rw-r--r--   0        0        0      537 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
--rw-r--r--   0        0        0      789 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/run/__init__.py
--rw-r--r--   0        0        0     2331 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/run/run.py
--rw-r--r--   0        0        0     4153 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/utils.py
--rw-r--r--   0        0        0     1262 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    24670 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     8183 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     8636 2024-04-20 23:05:17.732063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/client_app.py
--rw-r--r--   0        0        0     7435 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      735 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     8775 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      752 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     9052 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0     2404 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/heartbeat.py
--rw-r--r--   0        0        0      719 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     6553 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1824 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     1143 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/mod/__init__.py
--rw-r--r--   0        0        0     5397 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/mod/centraldp_mods.py
--rw-r--r--   0        0        0     2623 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/mod/comms_mods.py
--rw-r--r--   0        0        0     4918 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/mod/localdp_mod.py
--rw-r--r--   0        0        0      849 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/mod/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     1095 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
--rw-r--r--   0        0        0    19699 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
--rw-r--r--   0        0        0     1226 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/mod/utils.py
--rw-r--r--   0        0        0     1778 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/node_state.py
--rw-r--r--   0        0        0     2195 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/node_state_tests.py
--rw-r--r--   0        0        0    10283 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      735 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0    11302 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0      793 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/supernode/__init__.py
--rw-r--r--   0        0        0     3436 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/supernode/app.py
--rw-r--r--   0        0        0     1006 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/typing.py
--rw-r--r--   0        0        0     3721 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1882 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     2424 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0     1313 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/context.py
--rw-r--r--   0        0        0      891 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     6113 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/differential_privacy.py
--rw-r--r--   0        0        0     1074 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/differential_privacy_constants.py
--rw-r--r--   0        0        0     2004 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     2812 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/exit_handlers.py
--rw-r--r--   0        0        0     2273 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     6096 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0    12385 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/message.py
--rw-r--r--   0        0        0     4961 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/object_ref.py
--rw-r--r--   0        0        0     2095 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0     1385 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/pyproject.py
--rw-r--r--   0        0        0     1054 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/record/__init__.py
--rw-r--r--   0        0        0     4652 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/record/configsrecord.py
--rw-r--r--   0        0        0     1393 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/record/conversion_utils.py
--rw-r--r--   0        0        0     3923 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/record/metricsrecord.py
--rw-r--r--   0        0        0     4849 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/record/parametersrecord.py
--rw-r--r--   0        0        0     4553 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/record/recordset.py
--rw-r--r--   0        0        0     3879 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/record/typeddict.py
--rw-r--r--   0        0        0    13798 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/recordset_compat.py
--rw-r--r--   0        0        0    11707 2024-04-20 23:05:17.736063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/retry_invoker.py
--rw-r--r--   0        0        0      731 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/secure_aggregation/__init__.py
--rw-r--r--   0        0        0      738 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/secure_aggregation/crypto/__init__.py
--rw-r--r--   0        0        0     2792 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/secure_aggregation/crypto/shamir.py
--rw-r--r--   0        0        0     3546 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
--rw-r--r--   0        0        0     3026 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
--rw-r--r--   0        0        0     2310 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/secure_aggregation/quantization.py
--rw-r--r--   0        0        0     2183 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
--rw-r--r--   0        0        0     3221 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
--rw-r--r--   0        0        0    22250 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7865 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     4382 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      666 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      683 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     3207 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     5016 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     7304 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     2022 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     1084 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/error_pb2.py
--rw-r--r--   0        0        0      734 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/error_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/error_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/error_pb2_grpc.pyi
--rw-r--r--   0        0        0     5018 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     9161 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0    10605 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     2811 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1081 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     6009 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/recordset_pb2.py
--rw-r--r--   0        0        0    14161 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/recordset_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/recordset_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/recordset_pb2_grpc.pyi
--rw-r--r--   0        0        0     2472 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0     4320 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0     9781 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1785 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    24199 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     6127 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2399 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0      892 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/compat/__init__.py
--rw-r--r--   0        0        0     5271 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/compat/app.py
--rw-r--r--   0        0        0     3503 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/compat/app_utils.py
--rw-r--r--   0        0        0     7365 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/compat/driver_client_proxy.py
--rw-r--r--   0        0        0     1766 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/compat/legacy_context.py
--rw-r--r--   0        0        0     1061 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      766 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     5090 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/driver/abc_driver.py
--rw-r--r--   0        0        0    13928 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/driver/driver.py
--rw-r--r--   0        0        0     5121 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/history.py
--rw-r--r--   0        0        0     5592 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/run_serverapp.py
--rw-r--r--   0        0        0    17664 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/server.py
--rw-r--r--   0        0        0     4402 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/server_app.py
--rw-r--r--   0        0        0     1349 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/server_config.py
--rw-r--r--   0        0        0     2836 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0    13468 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     6532 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/bulyan.py
--rw-r--r--   0        0        0    17458 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/dp_adaptive_clipping.py
--rw-r--r--   0        0        0    12904 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/dp_fixed_clipping.py
--rw-r--r--   0        0        0     4877 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     7219 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5900 2024-04-20 23:05:17.740063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6505 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     6763 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11799 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9784 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8132 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2704 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5242 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     6862 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     5890 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     6080 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedxgb_bagging.py
--rw-r--r--   0        0        0     5607 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedxgb_cyclic.py
--rw-r--r--   0        0        0     4047 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     6801 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6285 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10150 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7543 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      707 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/__init__.py
--rw-r--r--   0        0        0      712 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/driver/__init__.py
--rw-r--r--   0        0        0     1932 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/driver/driver_grpc.py
--rw-r--r--   0        0        0     4780 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/driver/driver_servicer.py
--rw-r--r--   0        0        0      711 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/__init__.py
--rw-r--r--   0        0        0      735 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     5993 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6458 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4887 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11818 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0      758 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     3387 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0      731 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     3622 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      735 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     7621 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0      783 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/vce/__init__.py
--rw-r--r--   0        0        0     1466 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
--rw-r--r--   0        0        0     2260 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
--rw-r--r--   0        0        0     6375 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
--rw-r--r--   0        0        0    12454 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/vce/vce_api.py
--rw-r--r--   0        0        0     1003 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/state/__init__.py
--rw-r--r--   0        0        0    10083 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/state/in_memory_state.py
--rw-r--r--   0        0        0    24580 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/state/sqlite_state.py
--rw-r--r--   0        0        0     6762 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/state/state.py
--rw-r--r--   0        0        0     1654 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/state/state_factory.py
--rw-r--r--   0        0        0     2207 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/state/utils.py
--rw-r--r--   0        0        0      913 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/typing.py
--rw-r--r--   0        0        0      908 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5485 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     5301 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0      902 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/workflow/__init__.py
--rw-r--r--   0        0        0     1082 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/workflow/constant.py
--rw-r--r--   0        0        0    12547 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/workflow/default_workflows.py
--rw-r--r--   0        0        0      880 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/workflow/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     5838 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
--rw-r--r--   0        0        0    29038 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
--rw-r--r--   0        0        0     1400 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0    13904 2024-04-20 23:05:17.744063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      734 2024-04-20 23:05:17.748063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0    19367 2024-04-20 23:05:17.748063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/simulation/ray_transport/ray_actor.py
--rw-r--r--   0        0        0     6738 2024-04-20 23:05:17.748063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0     2392 2024-04-20 23:05:17.748063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/simulation/ray_transport/utils.py
--rw-r--r--   0        0        0    15685 2024-04-20 23:05:17.748063 flwr_nightly-1.9.0.dev20240420/src/py/flwr/simulation/run_simulation.py
--rw-r--r--   0        0        0    15260 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240420/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-22 23:05:12.519093 flwr_nightly-1.9.0.dev20240422/LICENSE
+-rw-r--r--   0        0        0    12916 2024-04-22 23:05:12.519093 flwr_nightly-1.9.0.dev20240422/README.md
+-rw-r--r--   0        0        0     5776 2024-04-22 23:05:30.159178 flwr_nightly-1.9.0.dev20240422/pyproject.toml
+-rw-r--r--   0        0        0      937 2024-04-22 23:05:12.939095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0      720 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/__init__.py
+-rw-r--r--   0        0        0     1095 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/app.py
+-rw-r--r--   0        0        0     5597 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/config_utils.py
+-rw-r--r--   0        0        0     2215 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/example.py
+-rw-r--r--   0        0        0      789 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/__init__.py
+-rw-r--r--   0        0        0     5380 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/new.py
+-rw-r--r--   0        0        0      725 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/__init__.py
+-rw-r--r--   0        0        0     3078 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/.gitignore.tpl
+-rw-r--r--   0        0        0      668 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/README.md.tpl
+-rw-r--r--   0        0        0      729 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/__init__.py
+-rw-r--r--   0        0        0      736 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/code/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
+-rw-r--r--   0        0        0      521 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
+-rw-r--r--   0        0        0     1173 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
+-rw-r--r--   0        0        0     1911 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
+-rw-r--r--   0        0        0      248 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
+-rw-r--r--   0        0        0      594 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
+-rw-r--r--   0        0        0      371 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
+-rw-r--r--   0        0        0     3684 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
+-rw-r--r--   0        0        0      489 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
+-rw-r--r--   0        0        0      558 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
+-rw-r--r--   0        0        0      537 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
+-rw-r--r--   0        0        0      789 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/run/__init__.py
+-rw-r--r--   0        0        0     2331 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/run/run.py
+-rw-r--r--   0        0        0     4153 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/utils.py
+-rw-r--r--   0        0        0     1262 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    24670 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     8183 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     8636 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/client_app.py
+-rw-r--r--   0        0        0     7435 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      735 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     8775 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      752 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     9052 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0     2404 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/heartbeat.py
+-rw-r--r--   0        0        0      719 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     6553 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1824 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     1143 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/mod/__init__.py
+-rw-r--r--   0        0        0     5397 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/mod/centraldp_mods.py
+-rw-r--r--   0        0        0     2623 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/mod/comms_mods.py
+-rw-r--r--   0        0        0     4918 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/mod/localdp_mod.py
+-rw-r--r--   0        0        0      849 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/mod/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     1095 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
+-rw-r--r--   0        0        0    19699 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
+-rw-r--r--   0        0        0     1226 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/mod/utils.py
+-rw-r--r--   0        0        0     1778 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/node_state.py
+-rw-r--r--   0        0        0     2195 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/node_state_tests.py
+-rw-r--r--   0        0        0    10283 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      735 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0    11302 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0      793 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/supernode/__init__.py
+-rw-r--r--   0        0        0     3861 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/supernode/app.py
+-rw-r--r--   0        0        0     1006 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/typing.py
+-rw-r--r--   0        0        0     3721 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1882 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     2424 2024-04-22 23:05:12.943095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0     1313 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/context.py
+-rw-r--r--   0        0        0      891 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     6113 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/differential_privacy.py
+-rw-r--r--   0        0        0     1074 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/differential_privacy_constants.py
+-rw-r--r--   0        0        0     2004 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     2812 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/exit_handlers.py
+-rw-r--r--   0        0        0     2273 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     6096 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0    12385 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/message.py
+-rw-r--r--   0        0        0     4961 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/object_ref.py
+-rw-r--r--   0        0        0     2095 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0     1385 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/pyproject.py
+-rw-r--r--   0        0        0     1054 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/record/__init__.py
+-rw-r--r--   0        0        0     4652 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/record/configsrecord.py
+-rw-r--r--   0        0        0     1393 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/record/conversion_utils.py
+-rw-r--r--   0        0        0     3923 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/record/metricsrecord.py
+-rw-r--r--   0        0        0     4849 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/record/parametersrecord.py
+-rw-r--r--   0        0        0     4553 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/record/recordset.py
+-rw-r--r--   0        0        0     3879 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/record/typeddict.py
+-rw-r--r--   0        0        0    13798 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/recordset_compat.py
+-rw-r--r--   0        0        0    11707 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/retry_invoker.py
+-rw-r--r--   0        0        0      731 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0      738 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/secure_aggregation/crypto/__init__.py
+-rw-r--r--   0        0        0     2792 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/secure_aggregation/crypto/shamir.py
+-rw-r--r--   0        0        0     3546 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
+-rw-r--r--   0        0        0     3026 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
+-rw-r--r--   0        0        0     2310 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/secure_aggregation/quantization.py
+-rw-r--r--   0        0        0     2183 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
+-rw-r--r--   0        0        0     3221 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
+-rw-r--r--   0        0        0    22250 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7865 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     4382 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      666 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      683 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     3207 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     5016 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     7304 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     2022 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1084 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/error_pb2.py
+-rw-r--r--   0        0        0      734 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/error_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/error_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/error_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5018 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     9161 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0    10605 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     2811 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1081 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6009 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/recordset_pb2.py
+-rw-r--r--   0        0        0    14161 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/recordset_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/recordset_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/recordset_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2472 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0     4320 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9781 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1785 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    24199 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     6127 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2399 2024-04-22 23:05:12.947095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0      892 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/compat/__init__.py
+-rw-r--r--   0        0        0     5287 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/compat/app.py
+-rw-r--r--   0        0        0     3503 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/compat/app_utils.py
+-rw-r--r--   0        0        0     7370 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/compat/driver_client_proxy.py
+-rw-r--r--   0        0        0     1766 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/compat/legacy_context.py
+-rw-r--r--   0        0        0     1061 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      862 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     5090 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/driver/driver.py
+-rw-r--r--   0        0        0    11418 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/driver/grpc_driver.py
+-rw-r--r--   0        0        0     5121 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0     5604 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/run_serverapp.py
+-rw-r--r--   0        0        0    17664 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0     4402 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/server_app.py
+-rw-r--r--   0        0        0     1349 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/server_config.py
+-rw-r--r--   0        0        0     2836 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0    13468 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     6532 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/bulyan.py
+-rw-r--r--   0        0        0    17458 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/dp_adaptive_clipping.py
+-rw-r--r--   0        0        0    12904 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/dp_fixed_clipping.py
+-rw-r--r--   0        0        0     4877 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     7219 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5900 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6505 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     6763 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11799 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9784 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8132 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2704 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5242 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     6862 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     5890 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     6080 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedxgb_bagging.py
+-rw-r--r--   0        0        0     5607 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedxgb_cyclic.py
+-rw-r--r--   0        0        0     4047 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     6801 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6285 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10150 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7543 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      707 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/driver/__init__.py
+-rw-r--r--   0        0        0     1932 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/driver/driver_grpc.py
+-rw-r--r--   0        0        0     4780 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/driver/driver_servicer.py
+-rw-r--r--   0        0        0      711 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/__init__.py
+-rw-r--r--   0        0        0      735 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     5993 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6458 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4887 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11818 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0      758 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     3387 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0      731 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     3622 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      735 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     7621 2024-04-22 23:05:12.951095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0      783 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/vce/__init__.py
+-rw-r--r--   0        0        0     1466 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
+-rw-r--r--   0        0        0     2260 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
+-rw-r--r--   0        0        0     6375 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
+-rw-r--r--   0        0        0    12454 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/vce/vce_api.py
+-rw-r--r--   0        0        0     1003 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/state/__init__.py
+-rw-r--r--   0        0        0    10083 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/state/in_memory_state.py
+-rw-r--r--   0        0        0    24580 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/state/sqlite_state.py
+-rw-r--r--   0        0        0     6762 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/state/state.py
+-rw-r--r--   0        0        0     1654 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/state/state_factory.py
+-rw-r--r--   0        0        0     2207 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/state/utils.py
+-rw-r--r--   0        0        0      913 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/typing.py
+-rw-r--r--   0        0        0      908 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5485 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     5301 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0      902 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/workflow/__init__.py
+-rw-r--r--   0        0        0     1082 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/workflow/constant.py
+-rw-r--r--   0        0        0    12547 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/workflow/default_workflows.py
+-rw-r--r--   0        0        0      880 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/workflow/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     5838 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
+-rw-r--r--   0        0        0    29038 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
+-rw-r--r--   0        0        0     1400 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0    13904 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      734 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0    19367 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/simulation/ray_transport/ray_actor.py
+-rw-r--r--   0        0        0     6738 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0     2392 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/simulation/ray_transport/utils.py
+-rw-r--r--   0        0        0    15694 2024-04-22 23:05:12.955095 flwr_nightly-1.9.0.dev20240422/src/py/flwr/simulation/run_simulation.py
+-rw-r--r--   0        0        0    15260 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240422/PKG-INFO
```

### Comparing `flwr_nightly-1.9.0.dev20240420/LICENSE` & `flwr_nightly-1.9.0.dev20240422/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/README.md` & `flwr_nightly-1.9.0.dev20240422/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/pyproject.toml` & `flwr_nightly-1.9.0.dev20240422/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.9.0.dev20240420"
+version = "1.9.0.dev20240422"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.ai>"]
 readme = "README.md"
 homepage = "https://flower.ai"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.ai"
@@ -132,15 +132,15 @@
 [tool.isort]
 line_length = 88
 indent = "    "
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
-known_first_party = ["flwr", "flwr_experimental", "flwr_tool"]
+known_first_party = ["flwr", "flwr_tool"]
 
 [tool.black]
 line-length = 88
 target-version = ["py38", "py39", "py310", "py311"]
 
 [tool.pylint."MESSAGES CONTROL"]
 disable = "duplicate-code,too-few-public-methods,useless-import-alias"
@@ -168,20 +168,14 @@
     "numpy.typing.mypy_plugin",
 ]
 ignore_missing_imports = true
 strict = true
 
 [[tool.mypy.overrides]]
 module = [
-    "flwr_experimental.*",
-]
-ignore_errors = true
-
-[[tool.mypy.overrides]]
-module = [
     "importlib.metadata.*",
     "importlib_metadata.*",
 ]
 follow_imports = "skip"
 follow_imports_for_stubs = true
 disallow_untyped_calls = false
```

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/app.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/config_utils.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/config_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/example.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/example.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/new.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/new.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/.gitignore.tpl` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/.gitignore.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/README.md.tpl` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/README.md.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/code/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/code/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/run/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/run/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/run/run.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/run/run.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/cli/utils.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/cli/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/app.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/client.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/client_app.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/client_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/grpc_rere_client/connection.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/grpc_rere_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/heartbeat.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/heartbeat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/mod/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/mod/centraldp_mods.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/mod/centraldp_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/mod/comms_mods.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/mod/comms_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/mod/localdp_mod.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/mod/localdp_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/mod/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/mod/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/mod/utils.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/mod/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/node_state.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/node_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/node_state_tests.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/node_state_tests.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/rest_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/supernode/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/supernode/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/supernode/app.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/supernode/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,45 +24,57 @@
 
 def run_supernode() -> None:
     """Run Flower SuperNode."""
     log(INFO, "Starting Flower SuperNode")
 
     event(EventType.RUN_SUPERNODE_ENTER)
 
-    args = _parse_args_run_supernode().parse_args()
+    _ = _parse_args_run_supernode().parse_args()
 
     log(
         DEBUG,
-        "Flower will load ClientApp `%s`",
-        getattr(args, "client-app"),
+        "Flower SuperNode starting...",
     )
 
     # Graceful shutdown
     register_exit_handlers(
         event_type=EventType.RUN_SUPERNODE_LEAVE,
     )
 
 
 def _parse_args_run_supernode() -> argparse.ArgumentParser:
     """Parse flower-supernode command line arguments."""
     parser = argparse.ArgumentParser(
         description="Start a Flower SuperNode",
     )
 
-    parse_args_run_client_app(parser=parser)
+    parser.add_argument(
+        "client-app",
+        nargs="?",
+        default="",
+        help="For example: `client:app` or `project.package.module:wrapper.app`. "
+        "This is optional and serves as the default ClientApp to be loaded when "
+        "the ServerApp does not specify `fab_id` and `fab_version`. "
+        "If not provided, defaults to an empty string.",
+    )
+    _parse_args_common(parser)
 
     return parser
 
 
 def parse_args_run_client_app(parser: argparse.ArgumentParser) -> None:
     """Parse command line arguments."""
     parser.add_argument(
         "client-app",
         help="For example: `client:app` or `project.package.module:wrapper.app`",
     )
+    _parse_args_common(parser)
+
+
+def _parse_args_common(parser: argparse.ArgumentParser) -> None:
     parser.add_argument(
         "--insecure",
         action="store_true",
         help="Run the client without HTTPS. By default, the client runs with "
         "HTTPS enabled. Use this flag only if you understand the risks.",
     )
     parser.add_argument(
```

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/client/typing.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/client/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/address.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/constant.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/context.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/date.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/differential_privacy.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/differential_privacy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/differential_privacy_constants.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/differential_privacy_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/dp.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/exit_handlers.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/exit_handlers.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/grpc.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/logger.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/message.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/message.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/object_ref.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/object_ref.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/parameter.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/pyproject.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/pyproject.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/record/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/record/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/record/configsrecord.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/record/configsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/record/conversion_utils.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/record/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/record/metricsrecord.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/record/metricsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/record/parametersrecord.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/record/parametersrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/record/recordset.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/record/recordset.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/record/typeddict.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/record/typeddict.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/recordset_compat.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/recordset_compat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/retry_invoker.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/retry_invoker.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/secure_aggregation/crypto/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/secure_aggregation/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/secure_aggregation/crypto/shamir.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/secure_aggregation/crypto/shamir.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/secure_aggregation/quantization.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/secure_aggregation/quantization.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/secure_aggregation/secaggplus_constants.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/secure_aggregation/secaggplus_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/secure_aggregation/secaggplus_utils.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/secure_aggregation/secaggplus_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/serde.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/typing.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/common/version.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/error_pb2.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/error_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/error_pb2.pyi` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/error_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/recordset_pb2.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/recordset_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/recordset_pb2.pyi` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/recordset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/app.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/compat/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/compat/app.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/compat/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from flwr.common.logger import log, warn_deprecated_feature
 from flwr.server.client_manager import ClientManager
 from flwr.server.history import History
 from flwr.server.server import Server, init_defaults, run_fl
 from flwr.server.server_config import ServerConfig
 from flwr.server.strategy import Strategy
 
-from ..driver import Driver
+from ..driver import Driver, GrpcDriver
 from .app_utils import start_update_client_manager_thread
 
 DEFAULT_SERVER_ADDRESS_DRIVER = "[::]:9091"
 
 ERROR_MESSAGE_DRIVER_NOT_CONNECTED = """
 [Driver] Error: Not connected.
 
@@ -110,15 +110,15 @@
             sys.exit(f"Server IP address ({server_address}) cannot be parsed.")
         host, port, is_v6 = parsed_address
         address = f"[{host}]:{port}" if is_v6 else f"{host}:{port}"
 
         # Create the Driver
         if isinstance(root_certificates, str):
             root_certificates = Path(root_certificates).read_bytes()
-        driver = Driver(
+        driver = GrpcDriver(
             driver_service_address=address, root_certificates=root_certificates
         )
 
     # Initialize the Driver API server and config
     initialized_server, initialized_config = init_defaults(
         server=server,
         config=config,
```

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/compat/app_utils.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/compat/app_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/compat/driver_client_proxy.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/compat/driver_client_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from flwr import common
 from flwr.common import DEFAULT_TTL, MessageType, MessageTypeLegacy, RecordSet
 from flwr.common import recordset_compat as compat
 from flwr.common import serde
 from flwr.proto import driver_pb2, node_pb2, task_pb2  # pylint: disable=E0611
 from flwr.server.client_proxy import ClientProxy
 
-from ..driver.driver import GrpcDriverHelper
+from ..driver.grpc_driver import GrpcDriverHelper
 
 SLEEP_TIME = 1
 
 
 class DriverClientProxy(ClientProxy):
     """Flower client proxy which delegates work using the Driver API."""
```

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/compat/legacy_context.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/compat/legacy_context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/criterion.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,15 @@
-# Copyright 2022 Flower Labs GmbH. All Rights Reserved.
+# Copyright 2020 Flower Labs GmbH. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Flower driver SDK."""
-
-
-from .driver import Driver
-
-__all__ = [
-    "Driver",
-]
+"""Server-side part of the gRPC transport layer using Request-Response."""
```

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/driver/abc_driver.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/driver/driver.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/driver/grpc_driver.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Flower driver service client."""
+"""Flower gRPC Driver."""
 
 import time
 import warnings
 from logging import DEBUG, ERROR, WARNING
 from typing import Iterable, List, Optional, Tuple
 
 import grpc
@@ -35,14 +35,16 @@
     PushTaskInsRequest,
     PushTaskInsResponse,
 )
 from flwr.proto.driver_pb2_grpc import DriverStub  # pylint: disable=E0611
 from flwr.proto.node_pb2 import Node  # pylint: disable=E0611
 from flwr.proto.task_pb2 import TaskIns  # pylint: disable=E0611
 
+from .driver import Driver
+
 DEFAULT_SERVER_ADDRESS_DRIVER = "[::]:9091"
 
 ERROR_MESSAGE_DRIVER_NOT_CONNECTED = """
 [Driver] Error: Not connected.
 
 Call `connect()` on the `GrpcDriverHelper` instance before calling any of the other
 `GrpcDriverHelper` methods.
@@ -129,15 +131,15 @@
             raise ConnectionError("`GrpcDriverHelper` instance not connected")
 
         # Call Driver API
         res: PullTaskResResponse = self.stub.PullTaskRes(request=req)
         return res
 
 
-class Driver:
+class GrpcDriver(Driver):
     """`Driver` class provides an interface to the Driver API.
 
     Parameters
     ----------
     driver_service_address : Optional[str]
         The IPv4 or IPv6 address of the Driver API server.
         Defaults to `"[::]:9091"`.
@@ -194,38 +196,14 @@
         group_id: str,
         ttl: Optional[float] = None,
     ) -> Message:
         """Create a new message with specified parameters.
 
         This method constructs a new `Message` with given content and metadata.
         The `run_id` and `src_node_id` will be set automatically.
-
-        Parameters
-        ----------
-        content : RecordSet
-            The content for the new message. This holds records that are to be sent
-            to the destination node.
-        message_type : str
-            The type of the message, defining the action to be executed on
-            the receiving end.
-        dst_node_id : int
-            The ID of the destination node to which the message is being sent.
-        group_id : str
-            The ID of the group to which this message is associated. In some settings,
-            this is used as the FL round.
-        ttl : Optional[float] (default: None)
-            Time-to-live for the round trip of this message, i.e., the time from sending
-            this message to receiving a reply. It specifies in seconds the duration for
-            which the message and its potential reply are considered valid. If unset,
-            the default TTL (i.e., `common.DEFAULT_TTL`) will be used.
-
-        Returns
-        -------
-        message : Message
-            A new `Message` instance with the specified content and metadata.
         """
         _, run_id = self._get_grpc_driver_helper_and_run_id()
         if ttl:
             warnings.warn(
                 "A custom TTL was set, but note that the SuperLink does not enforce "
                 "the TTL yet. The SuperLink will start enforcing the TTL in a future "
                 "version of Flower.",
@@ -253,25 +231,14 @@
         return [node.node_id for node in res.nodes]
 
     def push_messages(self, messages: Iterable[Message]) -> Iterable[str]:
         """Push messages to specified node IDs.
 
         This method takes an iterable of messages and sends each message
         to the node specified in `dst_node_id`.
-
-        Parameters
-        ----------
-        messages : Iterable[Message]
-            An iterable of messages to be sent.
-
-        Returns
-        -------
-        message_ids : Iterable[str]
-            An iterable of IDs for the messages that were sent, which can be used
-            to pull replies.
         """
         grpc_driver_helper, _ = self._get_grpc_driver_helper_and_run_id()
         # Construct TaskIns
         task_ins_list: List[TaskIns] = []
         for msg in messages:
             # Check message
             self._check_message(msg)
@@ -284,26 +251,16 @@
             PushTaskInsRequest(task_ins_list=task_ins_list)
         )
         return list(res.task_ids)
 
     def pull_messages(self, message_ids: Iterable[str]) -> Iterable[Message]:
         """Pull messages based on message IDs.
 
-        This method is used to collect messages from the SuperLink
-        that correspond to a set of given message IDs.
-
-        Parameters
-        ----------
-        message_ids : Iterable[str]
-            An iterable of message IDs for which reply messages are to be retrieved.
-
-        Returns
-        -------
-        messages : Iterable[Message]
-            An iterable of messages received.
+        This method is used to collect messages from the SuperLink that correspond to a
+        set of given message IDs.
         """
         grpc_driver, _ = self._get_grpc_driver_helper_and_run_id()
         # Pull TaskRes
         res = grpc_driver.pull_task_res(
             PullTaskResRequest(node=self.node, task_ids=message_ids)
         )
         # Convert TaskRes to Message
@@ -315,37 +272,16 @@
         messages: Iterable[Message],
         *,
         timeout: Optional[float] = None,
     ) -> Iterable[Message]:
         """Push messages to specified node IDs and pull the reply messages.
 
         This method sends a list of messages to their destination node IDs and then
-        waits for the replies. It continues to pull replies until either all
-        replies are received or the specified timeout duration is exceeded.
-
-        Parameters
-        ----------
-        messages : Iterable[Message]
-            An iterable of messages to be sent.
-        timeout : Optional[float] (default: None)
-            The timeout duration in seconds. If specified, the method will wait for
-            replies for this duration. If `None`, there is no time limit and the method
-            will wait until replies for all messages are received.
-
-        Returns
-        -------
-        replies : Iterable[Message]
-            An iterable of reply messages received from the SuperLink.
-
-        Notes
-        -----
-        This method uses `push_messages` to send the messages and `pull_messages`
-        to collect the replies. If `timeout` is set, the method may not return
-        replies for all sent messages. A message remains valid until its TTL,
-        which is not affected by `timeout`.
+        waits for the replies. It continues to pull replies until either all replies are
+        received or the specified timeout duration is exceeded.
         """
         # Push messages
         msg_ids = set(self.push_messages(messages))
 
         # Pull messages
         end_time = time.time() + (timeout if timeout is not None else 0.0)
         ret: List[Message] = []
```

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/history.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/run_serverapp.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/run_serverapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from pathlib import Path
 from typing import Optional
 
 from flwr.common import Context, EventType, RecordSet, event
 from flwr.common.logger import log, update_console_handler
 from flwr.common.object_ref import load_app
 
-from .driver.driver import Driver
+from .driver import Driver, GrpcDriver
 from .server_app import LoadServerAppError, ServerApp
 
 
 def run(
     driver: Driver,
     server_app_dir: str,
     server_app_attr: Optional[str] = None,
@@ -124,21 +124,21 @@
         "root_certificates: `%s`",
         root_certificates,
     )
 
     server_app_dir = args.dir
     server_app_attr = getattr(args, "server-app")
 
-    # Initialize Driver
-    driver = Driver(
+    # Initialize GrpcDriver
+    driver = GrpcDriver(
         driver_service_address=args.server,
         root_certificates=root_certificates,
     )
 
-    # Run the Server App with the Driver
+    # Run the ServerApp with the Driver
     run(driver=driver, server_app_dir=server_app_dir, server_app_attr=server_app_attr)
 
     # Clean up
     driver.close()
 
     event(EventType.RUN_SERVER_APP_LEAVE)
```

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/server.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/server_app.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/server_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/server_config.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/server_config.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/bulyan.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/bulyan.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/dp_adaptive_clipping.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/dp_adaptive_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/dp_fixed_clipping.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/dp_fixed_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedxgb_bagging.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedxgb_bagging.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedxgb_cyclic.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedxgb_cyclic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/driver/driver_grpc.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/driver/driver_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/driver/driver_servicer.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/message_handler/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Server-side part of the gRPC transport layer using Request-Response."""
+"""Shared request-response message handlers."""
```

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Shared request-response message handlers."""
+"""Server-side part of the REST transport layer."""
```

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Server-side part of the REST transport layer."""
+"""Ray-based Flower ClientProxy implementation."""
```

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/vce/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/vce/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/vce/backend/backend.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/vce/backend/backend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/fleet/vce/vce_api.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/fleet/vce/vce_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/state/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/state/in_memory_state.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/state/sqlite_state.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/state/sqlite_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/state/state.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/state/state_factory.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/superlink/state/utils.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/superlink/state/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/typing.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/workflow/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/workflow/constant.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/workflow/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/workflow/default_workflows.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/workflow/default_workflows.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/workflow/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/workflow/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/simulation/app.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/server/driver/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,25 @@
-# Copyright 2020 Flower Labs GmbH. All Rights Reserved.
+# Copyright 2022 Flower Labs GmbH. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Ray-based Flower ClientProxy implementation."""
+"""Flower driver SDK."""
+
+
+from .driver import Driver
+from .grpc_driver import GrpcDriver, GrpcDriverHelper
+
+__all__ = [
+    "Driver",
+    "GrpcDriver",
+    "GrpcDriverHelper",
+]
```

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/simulation/ray_transport/ray_actor.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/simulation/ray_transport/ray_actor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/simulation/ray_transport/utils.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/simulation/ray_transport/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240420/src/py/flwr/simulation/run_simulation.py` & `flwr_nightly-1.9.0.dev20240422/src/py/flwr/simulation/run_simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from typing import Dict, Optional
 
 import grpc
 
 from flwr.client import ClientApp
 from flwr.common import EventType, event, log
 from flwr.common.typing import ConfigsRecordValues
-from flwr.server.driver.driver import Driver
+from flwr.server.driver import Driver, GrpcDriver
 from flwr.server.run_serverapp import run
 from flwr.server.server_app import ServerApp
 from flwr.server.superlink.driver.driver_grpc import run_driver_api_grpc
 from flwr.server.superlink.fleet import vce
 from flwr.server.superlink.state import StateFactory
 from flwr.simulation.ray_transport.utils import (
     enable_tf_gpu_growth as enable_gpu_growth,
@@ -200,15 +200,15 @@
         certificates=None,
     )
 
     f_stop = asyncio.Event()
     serverapp_th = None
     try:
         # Initialize Driver
-        driver = Driver(
+        driver = GrpcDriver(
             driver_service_address=driver_api_address,
             root_certificates=None,
         )
 
         # Get and run ServerApp thread
         serverapp_th = run_serverapp_th(
             server_app_attr=server_app_attr,
```

### Comparing `flwr_nightly-1.9.0.dev20240420/PKG-INFO` & `flwr_nightly-1.9.0.dev20240422/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.9.0.dev20240420
+Version: 1.9.0.dev20240422
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.ai
 License: Apache-2.0
 Keywords: flower,fl,federated learning,federated analytics,federated evaluation,machine learning
 Author: The Flower Authors
 Author-email: hello@flower.ai
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240420 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240422 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.ai
 License: Apache-2.0 Keywords: flower,fl,federated learning,federated
 analytics,federated evaluation,machine learning Author: The Flower Authors
 Author-email: hello@flower.ai Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
```

