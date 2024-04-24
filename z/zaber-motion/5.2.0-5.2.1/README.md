# Comparing `tmp/zaber_motion-5.2.0.tar.gz` & `tmp/zaber_motion-5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zaber_motion-5.2.0.tar", last modified: Thu Apr 11 23:21:27 2024, max compression
+gzip compressed data, was "zaber_motion-5.2.1.tar", last modified: Tue Apr 23 23:21:49 2024, max compression
```

## Comparing `zaber_motion-5.2.0.tar` & `zaber_motion-5.2.1.tar`

### file list

```diff
@@ -1,221 +1,221 @@
-drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-04-11 23:21:27.572068 zaber_motion-5.2.0/
--rw-rw-rw-   0 ubuntu    (1001) root         (0)   109244 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/LICENSE.txt
--rw-rw-rw-   0 ubuntu    (1001) root         (0)       66 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/MANIFEST.in
--rw-r--r--   0 ubuntu    (1001) root         (0)   128259 2024-04-11 23:21:27.572068 zaber_motion-5.2.0/PKG-INFO
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      470 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/README.md
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1474 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/pyproject.toml
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      105 2024-04-11 23:21:27.573068 zaber_motion-5.2.0/setup.cfg
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1359 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/setup.py
-drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-04-11 23:21:27.563068 zaber_motion-5.2.0/zaber_motion/
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     6891 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/__init__.py
-drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-04-11 23:21:27.566068 zaber_motion-5.2.0/zaber_motion/ascii/
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     3721 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/__init__.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2185 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/alert_event.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     8708 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/all_axes.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    52240 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/axis.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    13661 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/axis_group.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2681 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/axis_identity.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    16542 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/axis_settings.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      301 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/axis_type.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1265 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/can_set_state_axis_response.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1530 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/can_set_state_device_response.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    35017 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/connection.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1959 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/conversion_factor.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    25265 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/device.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2801 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/device_identity.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    38262 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/device_io.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2077 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/device_io_info.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    15418 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/device_settings.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      274 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/digital_output_action.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1629 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/get_axis_setting.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1435 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/get_axis_setting_result.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2013 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/get_setting.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1501 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/get_setting_result.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1439 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/io_port_label.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      307 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/io_port_type.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    37243 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/lockstep.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1671 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/lockstep_axes.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      386 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/message_type.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    20711 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/oscilloscope.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2423 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/oscilloscope_capture_properties.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     7109 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/oscilloscope_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      268 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/oscilloscope_data_source.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1601 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/paramset_info.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2078 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/pid_tuning.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2848 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/pvt.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2071 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/pvt_axis_definition.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      256 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/pvt_axis_type.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     3190 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/pvt_buffer.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      247 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/pvt_mode.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    33848 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/pvt_sequence.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2896 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/response.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    20870 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/servo_tuner.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1782 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/servo_tuning_param.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      384 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/servo_tuning_paramset.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    26300 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/setting_constants.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2166 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/simple_tuning.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2340 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/simple_tuning_param_definition.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    26082 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/storage.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    83863 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/stream.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2110 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/stream_axis_definition.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      253 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/stream_axis_type.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     3084 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/stream_buffer.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      273 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/stream_mode.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2836 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/streams.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     5345 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/transport.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    26432 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/trigger.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      244 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/trigger_action.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      297 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/trigger_condition.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1429 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/trigger_enabled_state.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      275 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/trigger_operation.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2231 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/trigger_state.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     6058 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/triggers.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2966 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/unknown_response_event.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2855 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/warning_flags.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     5066 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/ascii/warnings.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1505 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/async_utils.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1664 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/axis_address.py
-drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-04-11 23:21:27.567068 zaber_motion-5.2.0/zaber_motion/binary/
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      653 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/binary/__init__.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1941 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/binary/binary_settings.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     3133 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/binary/command_code.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    19670 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/binary/connection.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    29083 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/binary/device.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     3361 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/binary/device_identity.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     3513 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/binary/device_settings.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      276 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/binary/device_type.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     3116 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/binary/error_code.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1498 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/binary/message.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      415 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/binary/reply_code.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1552 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/binary/reply_only_event.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1588 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/binary/unknown_response_event.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1442 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/bindings.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     4187 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/call.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     7475 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/convert_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      257 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/device_db_source_type.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2190 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/events.py
-drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-04-11 23:21:27.570068 zaber_motion-5.2.0/zaber_motion/exceptions/
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     7583 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/__init__.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1121 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/binary_command_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      991 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/binary_command_failed_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1045 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/command_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     3097 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/command_failed_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      308 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/command_preempted_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1129 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/command_too_long_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1971 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/command_too_long_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      304 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/connection_closed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      292 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/connection_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      308 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/conversion_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1158 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/device_address_conflict_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1126 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/device_address_conflict_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      314 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/device_busy_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1092 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/device_db_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      911 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/device_db_failed_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      283 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/device_detection_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      335 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/device_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      317 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/device_not_identified_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1065 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/g_code_execution_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1321 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/g_code_execution_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1036 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/g_code_syntax_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1300 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/g_code_syntax_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      309 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/internal_error_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      295 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/invalid_argument_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      300 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/invalid_data_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      310 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/invalid_operation_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1058 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/invalid_packet_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1198 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/invalid_packet_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      282 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/invalid_park_state_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1140 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/invalid_pvt_point.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1091 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/invalid_response_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      928 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/invalid_response_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      342 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/io_channel_out_of_range_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      297 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/io_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      322 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/lockstep_enabled_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      329 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/lockstep_not_enabled_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      386 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/motion_lib_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1070 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/movement_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1852 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/movement_failed_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1137 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/movement_interrupted_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1875 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/movement_interrupted_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      292 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/no_device_found_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      297 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/no_value_for_key_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      308 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/not_supported_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1095 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/operation_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1861 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/operation_failed_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      307 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/os_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      317 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/out_of_request_ids_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      323 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/pvt_discontinuity_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1037 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/pvt_execution_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1749 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/pvt_execution_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      326 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/pvt_mode_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1102 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/pvt_movement_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1292 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/pvt_movement_failed_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1169 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/pvt_movement_interrupted_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1327 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      285 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/pvt_setup_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      300 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/request_timeout_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      349 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/serial_port_busy_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     3563 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/set_device_state_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1085 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/set_device_state_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2372 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/set_peripheral_state_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1120 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/set_peripheral_state_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      307 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/setting_not_found_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      320 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/stream_discontinuity_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1060 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/stream_execution_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1232 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/stream_execution_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      323 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/stream_mode_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1134 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/stream_movement_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1313 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/stream_movement_failed_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1199 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/stream_movement_interrupted_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1348 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      282 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/stream_setup_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      341 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/timeout_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      320 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/transport_already_used_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      335 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/exceptions/unknown_request_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2088 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/firmware_version.py
-drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-04-11 23:21:27.571068 zaber_motion-5.2.0/zaber_motion/gcode/
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      578 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/gcode/__init__.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2340 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/gcode/axis_definition.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1547 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/gcode/axis_mapping.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2250 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/gcode/axis_transformation.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2360 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/gcode/device_definition.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    12481 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/gcode/offline_translator.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1555 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/gcode/translate_message.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1401 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/gcode/translate_result.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    13105 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/gcode/translator.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2206 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/gcode/translator_config.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     3346 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/library.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      279 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/log_output_mode.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1937 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/measurement.py
-drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-04-11 23:21:27.571068 zaber_motion-5.2.0/zaber_motion/microscopy/
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      370 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/microscopy/__init__.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     4647 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/microscopy/filter_changer.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     4175 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/microscopy/illuminator.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    19521 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/microscopy/illuminator_channel.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     7395 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/microscopy/microscope.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     4844 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/microscopy/microscope_config.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    13576 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/microscopy/objective_changer.py
-drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-04-11 23:21:27.571068 zaber_motion-5.2.0/zaber_motion/product/
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      394 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/product/__init__.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    26843 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/product/process.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     4171 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/product/process_controller.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      292 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/product/process_controller_mode.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2074 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/product/process_controller_source.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      281 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/product/process_controller_source_sensor.py
-drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-04-11 23:21:27.571068 zaber_motion-5.2.0/zaber_motion/protobufs/
--rw-rw-rw-   0 ubuntu    (1001) root         (0)        0 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/protobufs/__init__.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    83532 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/protobufs/main_pb2.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)   257403 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/protobufs/main_pb2.pyi
--rw-rw-rw-   0 ubuntu    (1001) root         (0)        0 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/py.typed
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      278 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/rotation_direction.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      987 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/serialization.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2108 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/tools.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1553 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/unit_table.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    10446 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/units.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)       22 2024-04-11 23:19:42.000000 zaber_motion-5.2.0/zaber_motion/version.py
-drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-04-11 23:21:27.571068 zaber_motion-5.2.0/zaber_motion.egg-info/
--rw-r--r--   0 ubuntu    (1001) root         (0)   128259 2024-04-11 23:21:27.000000 zaber_motion-5.2.0/zaber_motion.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1001) root         (0)     8939 2024-04-11 23:21:27.000000 zaber_motion-5.2.0/zaber_motion.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1001) root         (0)        1 2024-04-11 23:21:27.000000 zaber_motion-5.2.0/zaber_motion.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1001) root         (0)      212 2024-04-11 23:21:27.000000 zaber_motion-5.2.0/zaber_motion.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1001) root         (0)       27 2024-04-11 23:21:27.000000 zaber_motion-5.2.0/zaber_motion.egg-info/top_level.txt
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-04-23 23:21:49.155132 zaber_motion-5.2.1/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)   109244 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/LICENSE.txt
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)       66 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/MANIFEST.in
+-rw-r--r--   0 ubuntu    (1001) root         (0)   128259 2024-04-23 23:21:49.155132 zaber_motion-5.2.1/PKG-INFO
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      470 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/README.md
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1474 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/pyproject.toml
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      105 2024-04-23 23:21:49.155132 zaber_motion-5.2.1/setup.cfg
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1359 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/setup.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-04-23 23:21:49.146132 zaber_motion-5.2.1/zaber_motion/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     6891 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/__init__.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-04-23 23:21:49.149132 zaber_motion-5.2.1/zaber_motion/ascii/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     3721 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/__init__.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2185 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/alert_event.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     8708 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/all_axes.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    52240 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/axis.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    13661 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/axis_group.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2681 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/axis_identity.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    16542 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/axis_settings.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      301 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/axis_type.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1265 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/can_set_state_axis_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1530 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/can_set_state_device_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    35017 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/connection.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1959 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/conversion_factor.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    25265 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/device.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2801 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/device_identity.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    38262 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/device_io.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2077 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/device_io_info.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    15418 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/device_settings.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      274 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/digital_output_action.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1629 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/get_axis_setting.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1435 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/get_axis_setting_result.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2013 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/get_setting.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1501 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/get_setting_result.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1439 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/io_port_label.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      307 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/io_port_type.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    37243 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/lockstep.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1671 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/lockstep_axes.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      386 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/message_type.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    20711 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/oscilloscope.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2423 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/oscilloscope_capture_properties.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     7109 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/oscilloscope_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      268 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/oscilloscope_data_source.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1601 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/paramset_info.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2078 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/pid_tuning.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2848 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/pvt.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2071 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/pvt_axis_definition.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      256 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/pvt_axis_type.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     3190 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/pvt_buffer.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      247 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/pvt_mode.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    33848 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/pvt_sequence.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2896 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    20870 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/servo_tuner.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1782 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/servo_tuning_param.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      384 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/servo_tuning_paramset.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    26300 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/setting_constants.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2166 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/simple_tuning.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2340 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/simple_tuning_param_definition.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    26082 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/storage.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    83863 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/stream.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2110 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/stream_axis_definition.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      253 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/stream_axis_type.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     3084 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/stream_buffer.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      273 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/stream_mode.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2836 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/streams.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     5345 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/transport.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    26432 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/trigger.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      244 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/trigger_action.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      297 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/trigger_condition.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1429 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/trigger_enabled_state.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      275 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/trigger_operation.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2231 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/trigger_state.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     6058 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/triggers.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2966 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/unknown_response_event.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2855 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/warning_flags.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     5066 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/ascii/warnings.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1505 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/async_utils.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1664 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/axis_address.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-04-23 23:21:49.150132 zaber_motion-5.2.1/zaber_motion/binary/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      653 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/binary/__init__.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1941 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/binary/binary_settings.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     3133 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/binary/command_code.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    19670 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/binary/connection.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    29083 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/binary/device.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     3361 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/binary/device_identity.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     3513 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/binary/device_settings.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      276 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/binary/device_type.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     3116 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/binary/error_code.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1498 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/binary/message.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      415 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/binary/reply_code.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1552 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/binary/reply_only_event.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1588 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/binary/unknown_response_event.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1442 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/bindings.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     4187 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/call.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     7475 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/convert_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      257 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/device_db_source_type.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2190 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/events.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-04-23 23:21:49.153132 zaber_motion-5.2.1/zaber_motion/exceptions/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     7583 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/__init__.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1121 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/binary_command_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      991 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/binary_command_failed_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1045 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/command_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     3097 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/command_failed_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      308 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/command_preempted_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1129 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/command_too_long_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1971 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/command_too_long_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      304 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/connection_closed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      292 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/connection_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      308 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/conversion_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1158 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/device_address_conflict_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1126 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/device_address_conflict_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      314 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/device_busy_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1092 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/device_db_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      911 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/device_db_failed_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      283 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/device_detection_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      335 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/device_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      317 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/device_not_identified_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1065 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/g_code_execution_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1321 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/g_code_execution_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1036 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/g_code_syntax_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1300 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/g_code_syntax_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      309 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/internal_error_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      295 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/invalid_argument_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      300 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/invalid_data_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      310 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/invalid_operation_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1058 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/invalid_packet_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1198 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/invalid_packet_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      282 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/invalid_park_state_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1140 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/invalid_pvt_point.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1091 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/invalid_response_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      928 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/invalid_response_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      342 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/io_channel_out_of_range_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      297 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/io_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      322 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/lockstep_enabled_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      329 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/lockstep_not_enabled_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      386 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/motion_lib_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1070 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/movement_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1852 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/movement_failed_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1137 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/movement_interrupted_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1875 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/movement_interrupted_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      292 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/no_device_found_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      297 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/no_value_for_key_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      308 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/not_supported_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1095 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/operation_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1861 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/operation_failed_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      307 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/os_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      317 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/out_of_request_ids_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      323 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/pvt_discontinuity_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1037 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/pvt_execution_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1749 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/pvt_execution_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      326 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/pvt_mode_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1102 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/pvt_movement_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1292 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/pvt_movement_failed_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1169 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/pvt_movement_interrupted_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1327 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      285 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/pvt_setup_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      300 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/request_timeout_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      349 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/serial_port_busy_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     3563 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/set_device_state_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1085 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/set_device_state_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2372 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/set_peripheral_state_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1120 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/set_peripheral_state_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      307 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/setting_not_found_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      320 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/stream_discontinuity_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1060 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/stream_execution_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1232 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/stream_execution_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      323 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/stream_mode_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1134 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/stream_movement_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1313 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/stream_movement_failed_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1199 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/stream_movement_interrupted_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1348 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      282 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/stream_setup_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      341 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/timeout_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      320 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/transport_already_used_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      335 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/exceptions/unknown_request_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2088 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/firmware_version.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-04-23 23:21:49.153132 zaber_motion-5.2.1/zaber_motion/gcode/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      578 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/gcode/__init__.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2340 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/gcode/axis_definition.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1547 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/gcode/axis_mapping.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2250 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/gcode/axis_transformation.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2360 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/gcode/device_definition.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    12481 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/gcode/offline_translator.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1555 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/gcode/translate_message.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1401 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/gcode/translate_result.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    13105 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/gcode/translator.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2206 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/gcode/translator_config.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     3346 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/library.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      279 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/log_output_mode.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1937 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/measurement.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-04-23 23:21:49.154132 zaber_motion-5.2.1/zaber_motion/microscopy/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      370 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/microscopy/__init__.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     4647 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/microscopy/filter_changer.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     4175 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/microscopy/illuminator.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    19521 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/microscopy/illuminator_channel.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     7395 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/microscopy/microscope.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     4844 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/microscopy/microscope_config.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    13576 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/microscopy/objective_changer.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-04-23 23:21:49.154132 zaber_motion-5.2.1/zaber_motion/product/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      394 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/product/__init__.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    26843 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/product/process.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     4171 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/product/process_controller.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      292 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/product/process_controller_mode.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2074 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/product/process_controller_source.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      281 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/product/process_controller_source_sensor.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-04-23 23:21:49.154132 zaber_motion-5.2.1/zaber_motion/protobufs/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)        0 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/protobufs/__init__.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    83532 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/protobufs/main_pb2.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)   257403 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/protobufs/main_pb2.pyi
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)        0 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/py.typed
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      278 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/rotation_direction.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      987 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/serialization.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2108 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/tools.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1553 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/unit_table.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    10446 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/units.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)       22 2024-04-23 23:20:03.000000 zaber_motion-5.2.1/zaber_motion/version.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-04-23 23:21:49.154132 zaber_motion-5.2.1/zaber_motion.egg-info/
+-rw-r--r--   0 ubuntu    (1001) root         (0)   128259 2024-04-23 23:21:49.000000 zaber_motion-5.2.1/zaber_motion.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1001) root         (0)     8939 2024-04-23 23:21:49.000000 zaber_motion-5.2.1/zaber_motion.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1001) root         (0)        1 2024-04-23 23:21:49.000000 zaber_motion-5.2.1/zaber_motion.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1001) root         (0)      212 2024-04-23 23:21:49.000000 zaber_motion-5.2.1/zaber_motion.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1001) root         (0)       27 2024-04-23 23:21:49.000000 zaber_motion-5.2.1/zaber_motion.egg-info/top_level.txt
```

### Comparing `zaber_motion-5.2.0/LICENSE.txt` & `zaber_motion-5.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/PKG-INFO` & `zaber_motion-5.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zaber_motion
-Version: 5.2.0
+Version: 5.2.1
 Summary: An official library for communicating with Zaber devices.
 Author-email: "Zaber Technologies Inc." <contact@zaber.com>
 License: The MIT License (MIT)
         
         Copyright 2018-2022 Zaber Technologies Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `zaber_motion-5.2.0/pyproject.toml` & `zaber_motion-5.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zaber_motion"
-version = "5.2.0"
+version = "5.2.1"
 description = "An official library for communicating with Zaber devices."
 authors = [{ name = "Zaber Technologies Inc.", email = "contact@zaber.com" }]
 license = { file = "LICENSE.txt" }
 readme = { file = "README.md", content-type = "text/markdown" }
 dependencies = [
   "protobuf>=3.20.0,<4.22.0",
   "rx>=3.0.0",
```

### Comparing `zaber_motion-5.2.0/setup.py` & `zaber_motion-5.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/__init__.py` & `zaber_motion-5.2.1/zaber_motion/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/__init__.py` & `zaber_motion-5.2.1/zaber_motion/ascii/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/alert_event.py` & `zaber_motion-5.2.1/zaber_motion/ascii/alert_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/all_axes.py` & `zaber_motion-5.2.1/zaber_motion/ascii/all_axes.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/axis.py` & `zaber_motion-5.2.1/zaber_motion/ascii/axis.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/axis_group.py` & `zaber_motion-5.2.1/zaber_motion/ascii/axis_group.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/axis_identity.py` & `zaber_motion-5.2.1/zaber_motion/ascii/axis_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/axis_settings.py` & `zaber_motion-5.2.1/zaber_motion/ascii/axis_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/can_set_state_axis_response.py` & `zaber_motion-5.2.1/zaber_motion/ascii/can_set_state_axis_response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/can_set_state_device_response.py` & `zaber_motion-5.2.1/zaber_motion/ascii/can_set_state_device_response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/connection.py` & `zaber_motion-5.2.1/zaber_motion/ascii/connection.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/conversion_factor.py` & `zaber_motion-5.2.1/zaber_motion/ascii/conversion_factor.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/device.py` & `zaber_motion-5.2.1/zaber_motion/ascii/device.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/device_identity.py` & `zaber_motion-5.2.1/zaber_motion/ascii/device_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/device_io.py` & `zaber_motion-5.2.1/zaber_motion/ascii/device_io.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/device_io_info.py` & `zaber_motion-5.2.1/zaber_motion/ascii/device_io_info.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/device_settings.py` & `zaber_motion-5.2.1/zaber_motion/ascii/device_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/get_axis_setting.py` & `zaber_motion-5.2.1/zaber_motion/ascii/get_axis_setting.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/get_axis_setting_result.py` & `zaber_motion-5.2.1/zaber_motion/ascii/get_axis_setting_result.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/get_setting.py` & `zaber_motion-5.2.1/zaber_motion/ascii/get_setting.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/get_setting_result.py` & `zaber_motion-5.2.1/zaber_motion/ascii/get_setting_result.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/io_port_label.py` & `zaber_motion-5.2.1/zaber_motion/ascii/io_port_label.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/lockstep.py` & `zaber_motion-5.2.1/zaber_motion/ascii/lockstep.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/lockstep_axes.py` & `zaber_motion-5.2.1/zaber_motion/ascii/lockstep_axes.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/oscilloscope.py` & `zaber_motion-5.2.1/zaber_motion/ascii/oscilloscope.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/oscilloscope_capture_properties.py` & `zaber_motion-5.2.1/zaber_motion/ascii/oscilloscope_capture_properties.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/oscilloscope_data.py` & `zaber_motion-5.2.1/zaber_motion/ascii/oscilloscope_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/paramset_info.py` & `zaber_motion-5.2.1/zaber_motion/ascii/paramset_info.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/pid_tuning.py` & `zaber_motion-5.2.1/zaber_motion/ascii/pid_tuning.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/pvt.py` & `zaber_motion-5.2.1/zaber_motion/ascii/pvt.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/pvt_axis_definition.py` & `zaber_motion-5.2.1/zaber_motion/ascii/pvt_axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/pvt_buffer.py` & `zaber_motion-5.2.1/zaber_motion/ascii/pvt_buffer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/pvt_sequence.py` & `zaber_motion-5.2.1/zaber_motion/ascii/pvt_sequence.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/response.py` & `zaber_motion-5.2.1/zaber_motion/ascii/response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/servo_tuner.py` & `zaber_motion-5.2.1/zaber_motion/ascii/servo_tuner.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/servo_tuning_param.py` & `zaber_motion-5.2.1/zaber_motion/ascii/servo_tuning_param.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/setting_constants.py` & `zaber_motion-5.2.1/zaber_motion/ascii/setting_constants.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/simple_tuning.py` & `zaber_motion-5.2.1/zaber_motion/ascii/simple_tuning.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/simple_tuning_param_definition.py` & `zaber_motion-5.2.1/zaber_motion/ascii/simple_tuning_param_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/storage.py` & `zaber_motion-5.2.1/zaber_motion/ascii/storage.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/stream.py` & `zaber_motion-5.2.1/zaber_motion/ascii/stream.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/stream_axis_definition.py` & `zaber_motion-5.2.1/zaber_motion/ascii/stream_axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/stream_buffer.py` & `zaber_motion-5.2.1/zaber_motion/ascii/stream_buffer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/streams.py` & `zaber_motion-5.2.1/zaber_motion/ascii/streams.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/transport.py` & `zaber_motion-5.2.1/zaber_motion/ascii/transport.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/trigger.py` & `zaber_motion-5.2.1/zaber_motion/ascii/trigger.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/trigger_enabled_state.py` & `zaber_motion-5.2.1/zaber_motion/ascii/trigger_enabled_state.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/trigger_state.py` & `zaber_motion-5.2.1/zaber_motion/ascii/trigger_state.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/triggers.py` & `zaber_motion-5.2.1/zaber_motion/ascii/triggers.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/unknown_response_event.py` & `zaber_motion-5.2.1/zaber_motion/ascii/unknown_response_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/warning_flags.py` & `zaber_motion-5.2.1/zaber_motion/ascii/warning_flags.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/ascii/warnings.py` & `zaber_motion-5.2.1/zaber_motion/ascii/warnings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/async_utils.py` & `zaber_motion-5.2.1/zaber_motion/async_utils.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/axis_address.py` & `zaber_motion-5.2.1/zaber_motion/axis_address.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/binary/__init__.py` & `zaber_motion-5.2.1/zaber_motion/binary/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/binary/binary_settings.py` & `zaber_motion-5.2.1/zaber_motion/binary/binary_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/binary/command_code.py` & `zaber_motion-5.2.1/zaber_motion/binary/command_code.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/binary/connection.py` & `zaber_motion-5.2.1/zaber_motion/binary/connection.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/binary/device.py` & `zaber_motion-5.2.1/zaber_motion/binary/device.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/binary/device_identity.py` & `zaber_motion-5.2.1/zaber_motion/binary/device_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/binary/device_settings.py` & `zaber_motion-5.2.1/zaber_motion/binary/device_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/binary/error_code.py` & `zaber_motion-5.2.1/zaber_motion/binary/error_code.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/binary/message.py` & `zaber_motion-5.2.1/zaber_motion/binary/message.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/binary/reply_only_event.py` & `zaber_motion-5.2.1/zaber_motion/binary/reply_only_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/binary/unknown_response_event.py` & `zaber_motion-5.2.1/zaber_motion/binary/unknown_response_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/bindings.py` & `zaber_motion-5.2.1/zaber_motion/bindings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/call.py` & `zaber_motion-5.2.1/zaber_motion/call.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/convert_exception.py` & `zaber_motion-5.2.1/zaber_motion/convert_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/events.py` & `zaber_motion-5.2.1/zaber_motion/events.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/__init__.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/binary_command_failed_exception.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/binary_command_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/binary_command_failed_exception_data.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/binary_command_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/command_failed_exception.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/command_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/command_failed_exception_data.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/command_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/command_too_long_exception.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/command_too_long_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/command_too_long_exception_data.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/command_too_long_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/device_address_conflict_exception.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/device_address_conflict_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/device_address_conflict_exception_data.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/device_address_conflict_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/device_db_failed_exception.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/device_db_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/device_db_failed_exception_data.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/device_db_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/g_code_execution_exception.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/g_code_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/g_code_execution_exception_data.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/g_code_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/g_code_syntax_exception.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/g_code_syntax_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/g_code_syntax_exception_data.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/g_code_syntax_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/invalid_packet_exception.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/invalid_packet_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/invalid_packet_exception_data.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/invalid_packet_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/invalid_pvt_point.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/invalid_pvt_point.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/invalid_response_exception.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/invalid_response_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/invalid_response_exception_data.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/invalid_response_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/movement_failed_exception.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/movement_failed_exception_data.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/movement_interrupted_exception.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/movement_interrupted_exception_data.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/operation_failed_exception.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/operation_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/operation_failed_exception_data.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/operation_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/pvt_execution_exception.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/pvt_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/pvt_execution_exception_data.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/pvt_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/pvt_movement_failed_exception.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/pvt_movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/pvt_movement_failed_exception_data.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/pvt_movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/pvt_movement_interrupted_exception.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/pvt_movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/set_device_state_exception_data.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/set_device_state_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/set_device_state_failed_exception.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/set_device_state_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/set_peripheral_state_exception_data.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/set_peripheral_state_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/set_peripheral_state_failed_exception.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/set_peripheral_state_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/stream_execution_exception.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/stream_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/stream_execution_exception_data.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/stream_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/stream_movement_failed_exception.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/stream_movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/stream_movement_failed_exception_data.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/stream_movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/stream_movement_interrupted_exception.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/stream_movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py` & `zaber_motion-5.2.1/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/firmware_version.py` & `zaber_motion-5.2.1/zaber_motion/firmware_version.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/gcode/__init__.py` & `zaber_motion-5.2.1/zaber_motion/gcode/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/gcode/axis_definition.py` & `zaber_motion-5.2.1/zaber_motion/gcode/axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/gcode/axis_mapping.py` & `zaber_motion-5.2.1/zaber_motion/gcode/axis_mapping.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/gcode/axis_transformation.py` & `zaber_motion-5.2.1/zaber_motion/gcode/axis_transformation.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/gcode/device_definition.py` & `zaber_motion-5.2.1/zaber_motion/gcode/device_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/gcode/offline_translator.py` & `zaber_motion-5.2.1/zaber_motion/gcode/offline_translator.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/gcode/translate_message.py` & `zaber_motion-5.2.1/zaber_motion/gcode/translate_message.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/gcode/translate_result.py` & `zaber_motion-5.2.1/zaber_motion/gcode/translate_result.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/gcode/translator.py` & `zaber_motion-5.2.1/zaber_motion/gcode/translator.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/gcode/translator_config.py` & `zaber_motion-5.2.1/zaber_motion/gcode/translator_config.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/library.py` & `zaber_motion-5.2.1/zaber_motion/library.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/measurement.py` & `zaber_motion-5.2.1/zaber_motion/measurement.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/microscopy/filter_changer.py` & `zaber_motion-5.2.1/zaber_motion/microscopy/filter_changer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/microscopy/illuminator.py` & `zaber_motion-5.2.1/zaber_motion/microscopy/illuminator.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/microscopy/illuminator_channel.py` & `zaber_motion-5.2.1/zaber_motion/microscopy/illuminator_channel.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/microscopy/microscope.py` & `zaber_motion-5.2.1/zaber_motion/microscopy/microscope.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/microscopy/microscope_config.py` & `zaber_motion-5.2.1/zaber_motion/microscopy/microscope_config.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/microscopy/objective_changer.py` & `zaber_motion-5.2.1/zaber_motion/microscopy/objective_changer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/product/process.py` & `zaber_motion-5.2.1/zaber_motion/product/process.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/product/process_controller.py` & `zaber_motion-5.2.1/zaber_motion/product/process_controller.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/product/process_controller_source.py` & `zaber_motion-5.2.1/zaber_motion/product/process_controller_source.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/protobufs/main_pb2.py` & `zaber_motion-5.2.1/zaber_motion/protobufs/main_pb2.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/protobufs/main_pb2.pyi` & `zaber_motion-5.2.1/zaber_motion/protobufs/main_pb2.pyi`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/serialization.py` & `zaber_motion-5.2.1/zaber_motion/serialization.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/tools.py` & `zaber_motion-5.2.1/zaber_motion/tools.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/unit_table.py` & `zaber_motion-5.2.1/zaber_motion/unit_table.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion/units.py` & `zaber_motion-5.2.1/zaber_motion/units.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.0/zaber_motion.egg-info/PKG-INFO` & `zaber_motion-5.2.1/zaber_motion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zaber_motion
-Version: 5.2.0
+Version: 5.2.1
 Summary: An official library for communicating with Zaber devices.
 Author-email: "Zaber Technologies Inc." <contact@zaber.com>
 License: The MIT License (MIT)
         
         Copyright 2018-2022 Zaber Technologies Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `zaber_motion-5.2.0/zaber_motion.egg-info/SOURCES.txt` & `zaber_motion-5.2.1/zaber_motion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

