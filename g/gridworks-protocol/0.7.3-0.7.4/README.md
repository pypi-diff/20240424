# Comparing `tmp/gridworks_protocol-0.7.3.tar.gz` & `tmp/gridworks_protocol-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_protocol-0.7.3.tar", max compression
+gzip compressed data, was "gridworks_protocol-0.7.4.tar", max compression
```

## Comparing `gridworks_protocol-0.7.3.tar` & `gridworks_protocol-0.7.4.tar`

### file list

```diff
@@ -1,115 +1,115 @@
--rw-r--r--   0        0        0     1070 2024-04-22 22:52:43.432922 gridworks_protocol-0.7.3/LICENSE
--rw-r--r--   0        0        0     3087 2024-04-22 22:52:43.432922 gridworks_protocol-0.7.3/README.md
--rw-r--r--   0        0        0     2291 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     2030 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/__init__.py
--rw-r--r--   0        0        0     1340 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/electric_meter_cac.py
--rw-r--r--   0        0        0      143 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/fibaro_smart_implant_cac.py
--rw-r--r--   0        0        0      132 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/hubitat_cac.py
--rw-r--r--   0        0        0      138 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/hubitat_poller_cac.py
--rw-r--r--   0        0        0      142 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/hubitat_tank_module_cac.py
--rw-r--r--   0        0        0     1489 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py
--rw-r--r--   0        0        0      996 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py
--rw-r--r--   0        0        0     1113 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/relay_cac.py
--rw-r--r--   0        0        0     1119 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/resistive_heater_cac.py
--rw-r--r--   0        0        0      135 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/rest_poller_cac.py
--rw-r--r--   0        0        0     1581 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py
--rw-r--r--   0        0        0      134 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/web_server_cac.py
--rw-r--r--   0        0        0     1388 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/component.py
--rw-r--r--   0        0        0     1095 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/component_attribute_class.py
--rw-r--r--   0        0        0     1660 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/electric_meter_component.py
--rw-r--r--   0        0        0      533 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/fibaro_smart_implant_component.py
--rw-r--r--   0        0        0      962 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/hubitat_component.py
--rw-r--r--   0        0        0     3575 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/hubitat_poller_component.py
--rw-r--r--   0        0        0     4189 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/hubitat_tank_component.py
--rw-r--r--   0        0        0     1480 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/multipurpose_sensor_component.py
--rw-r--r--   0        0        0     1482 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/pipe_flow_sensor_component.py
--rw-r--r--   0        0        0     1268 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/relay_component.py
--rw-r--r--   0        0        0     1466 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/resistive_heater_component.py
--rw-r--r--   0        0        0      674 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/rest_poller_component.py
--rw-r--r--   0        0        0     1309 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/simple_temp_sensor_component.py
--rw-r--r--   0        0        0      687 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/data_classes/components/web_server_component.py
--rw-r--r--   0        0        0      165 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/errors.py
--rw-r--r--   0        0        0    21391 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/data_classes/hardware_layout.py
--rw-r--r--   0        0        0      273 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/mixin.py
--rw-r--r--   0        0        0      377 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/resolver.py
--rw-r--r--   0        0        0     2401 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/sh_node.py
--rw-r--r--   0        0        0      362 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/data_classes/telemetry_tuple.py
--rw-r--r--   0        0        0    14860 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/decoders.py
--rw-r--r--   0        0        0     3690 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/default_decoders.py
--rw-r--r--   0        0        0     3167 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/enums/__init__.py
--rw-r--r--   0        0        0     8935 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/enums/actor_class.py
--rw-r--r--   0        0        0     4686 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/enums/local_comm_interface.py
--rw-r--r--   0        0        0    10910 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/enums/make_model.py
--rw-r--r--   0        0        0     8099 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/enums/role.py
--rw-r--r--   0        0        0     7274 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/enums/telemetry_name.py
--rw-r--r--   0        0        0     4910 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/enums/unit.py
--rw-r--r--   0        0        0      336 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/errors.py
--rw-r--r--   0        0        0      249 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/gs/__init__.py
--rw-r--r--   0        0        0      460 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/gs/gs_dispatch.py
--rw-r--r--   0        0        0      800 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/gs/gs_dispatch_base.py
--rw-r--r--   0        0        0      678 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/gs/gs_dispatch_maker.py
--rw-r--r--   0        0        0      442 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/gs/gs_pwr.py
--rw-r--r--   0        0        0      851 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/gs/gs_pwr_base.py
--rw-r--r--   0        0        0      609 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/gs/gs_pwr_maker.py
--rw-r--r--   0        0        0     3237 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/message.py
--rw-r--r--   0        0        0     1474 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/messages/__init__.py
--rw-r--r--   0        0        0     3068 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/messages/event.py
--rw-r--r--   0        0        0      669 2024-04-22 22:52:43.440922 gridworks_protocol-0.7.3/src/gwproto/messages/misc.py
--rw-r--r--   0        0        0    11428 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/property_format.py
--rw-r--r--   0        0        0        0 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/py.typed
--rw-r--r--   0        0        0     2892 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/topic.py
--rw-r--r--   0        0        0     1051 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/type_helpers/__init__.py
--rw-r--r--   0        0        0     8974 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/types/__init__.py
--rw-r--r--   0        0        0     9990 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/component_attribute_class_gt.py
--rw-r--r--   0        0        0    10683 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/component_gt.py
--rw-r--r--   0        0        0     9168 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/data_channel.py
--rw-r--r--   0        0        0     7734 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/egauge_io.py
--rw-r--r--   0        0        0     8183 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/egauge_register_config.py
--rw-r--r--   0        0        0    13383 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/electric_meter_cac_gt.py
--rw-r--r--   0        0        0    18082 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/electric_meter_component_gt.py
--rw-r--r--   0        0        0     2670 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/fibaro_smart_implant_cac_gt.py
--rw-r--r--   0        0        0     2959 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/fibaro_smart_implant_component_gt.py
--rw-r--r--   0        0        0    12880 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/gt_dispatch_boolean.py
--rw-r--r--   0        0        0    10676 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/gt_dispatch_boolean_local.py
--rw-r--r--   0        0        0     9579 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/gt_driver_booleanactuator_cmd.py
--rw-r--r--   0        0        0     9646 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py
--rw-r--r--   0        0        0     9258 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_cli_atn_cmd.py
--rw-r--r--   0        0        0    11997 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py
--rw-r--r--   0        0        0    11090 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_simple_telemetry_status.py
--rw-r--r--   0        0        0    15695 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_status.py
--rw-r--r--   0        0        0    11589 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py
--rw-r--r--   0        0        0     8430 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/gt_telemetry.py
--rw-r--r--   0        0        0    12904 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/heartbeat_b.py
--rw-r--r--   0        0        0     2281 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/hubitat_cac_gt.py
--rw-r--r--   0        0        0     4772 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/types/hubitat_component_gt.py
--rw-r--r--   0        0        0     2555 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/types/hubitat_gt.py
--rw-r--r--   0        0        0     1328 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/hubitat_poller_cac_gt.py
--rw-r--r--   0        0        0     1573 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/hubitat_poller_component_gt.py
--rw-r--r--   0        0        0     1697 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/types/hubitat_poller_gt.py
--rw-r--r--   0        0        0     2469 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/hubitat_tank_cac_gt.py
--rw-r--r--   0        0        0     3017 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/hubitat_tank_component_gt.py
--rw-r--r--   0        0        0     8831 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/types/hubitat_tank_gt.py
--rw-r--r--   0        0        0    13945 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/multipurpose_sensor_cac_gt.py
--rw-r--r--   0        0        0    13879 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/multipurpose_sensor_component_gt.py
--rw-r--r--   0        0        0    10163 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/pipe_flow_sensor_cac_gt.py
--rw-r--r--   0        0        0    12226 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/pipe_flow_sensor_component_gt.py
--rw-r--r--   0        0        0     5915 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/power_watts.py
--rw-r--r--   0        0        0     9932 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/relay_cac_gt.py
--rw-r--r--   0        0        0    11585 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/relay_component_gt.py
--rw-r--r--   0        0        0    11465 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/resistive_heater_cac_gt.py
--rw-r--r--   0        0        0    11819 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/resistive_heater_component_gt.py
--rw-r--r--   0        0        0     2364 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/rest_poller_cac_gt.py
--rw-r--r--   0        0        0     3033 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/rest_poller_component_gt.py
--rw-r--r--   0        0        0     8900 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/rest_poller_gt.py
--rw-r--r--   0        0        0    12488 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/simple_temp_sensor_cac_gt.py
--rw-r--r--   0        0        0    11394 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/simple_temp_sensor_component_gt.py
--rw-r--r--   0        0        0     9456 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/snapshot_spaceheat.py
--rw-r--r--   0        0        0    14590 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/spaceheat_node_gt.py
--rw-r--r--   0        0        0    12356 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/ta_data_channels.py
--rw-r--r--   0        0        0    11281 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/telemetry_reporting_config.py
--rw-r--r--   0        0        0    11369 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/types/telemetry_snapshot_spaceheat.py
--rw-r--r--   0        0        0     1140 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/types/web_server_cac_gt.py
--rw-r--r--   0        0        0     1463 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/types/web_server_component_gt.py
--rw-r--r--   0        0        0      440 2024-04-22 22:52:54.180996 gridworks_protocol-0.7.3/src/gwproto/types/web_server_gt.py
--rw-r--r--   0        0        0     2890 2024-04-22 22:52:43.444922 gridworks_protocol-0.7.3/src/gwproto/utils.py
--rw-r--r--   0        0        0     4129 1970-01-01 00:00:00.000000 gridworks_protocol-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-23 18:06:37.303031 gridworks_protocol-0.7.4/LICENSE
+-rw-r--r--   0        0        0     3087 2024-04-23 18:06:37.303031 gridworks_protocol-0.7.4/README.md
+-rw-r--r--   0        0        0     2295 2024-04-23 18:06:55.791201 gridworks_protocol-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     2030 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/__init__.py
+-rw-r--r--   0        0        0     1340 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/cacs/electric_meter_cac.py
+-rw-r--r--   0        0        0      143 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/cacs/fibaro_smart_implant_cac.py
+-rw-r--r--   0        0        0      132 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/cacs/hubitat_cac.py
+-rw-r--r--   0        0        0      138 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/cacs/hubitat_poller_cac.py
+-rw-r--r--   0        0        0      142 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/cacs/hubitat_tank_module_cac.py
+-rw-r--r--   0        0        0     1489 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py
+-rw-r--r--   0        0        0      996 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py
+-rw-r--r--   0        0        0     1113 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/cacs/relay_cac.py
+-rw-r--r--   0        0        0     1119 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/cacs/resistive_heater_cac.py
+-rw-r--r--   0        0        0      135 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/cacs/rest_poller_cac.py
+-rw-r--r--   0        0        0     1581 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py
+-rw-r--r--   0        0        0      134 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/cacs/web_server_cac.py
+-rw-r--r--   0        0        0     1388 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/component.py
+-rw-r--r--   0        0        0     1095 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/component_attribute_class.py
+-rw-r--r--   0        0        0     1660 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/components/electric_meter_component.py
+-rw-r--r--   0        0        0      533 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/components/fibaro_smart_implant_component.py
+-rw-r--r--   0        0        0      962 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/components/hubitat_component.py
+-rw-r--r--   0        0        0     3575 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/components/hubitat_poller_component.py
+-rw-r--r--   0        0        0     4189 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/components/hubitat_tank_component.py
+-rw-r--r--   0        0        0     1480 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/components/multipurpose_sensor_component.py
+-rw-r--r--   0        0        0     1482 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/components/pipe_flow_sensor_component.py
+-rw-r--r--   0        0        0     1268 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/components/relay_component.py
+-rw-r--r--   0        0        0     1466 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/components/resistive_heater_component.py
+-rw-r--r--   0        0        0      674 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/components/rest_poller_component.py
+-rw-r--r--   0        0        0     1309 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/components/simple_temp_sensor_component.py
+-rw-r--r--   0        0        0      687 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/components/web_server_component.py
+-rw-r--r--   0        0        0      165 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/errors.py
+-rw-r--r--   0        0        0    21391 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/hardware_layout.py
+-rw-r--r--   0        0        0      273 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/mixin.py
+-rw-r--r--   0        0        0      377 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/resolver.py
+-rw-r--r--   0        0        0     2401 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/sh_node.py
+-rw-r--r--   0        0        0      362 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/data_classes/telemetry_tuple.py
+-rw-r--r--   0        0        0    14860 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/decoders.py
+-rw-r--r--   0        0        0     3690 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/default_decoders.py
+-rw-r--r--   0        0        0     3167 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/enums/__init__.py
+-rw-r--r--   0        0        0     8935 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/enums/actor_class.py
+-rw-r--r--   0        0        0     4686 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/enums/local_comm_interface.py
+-rw-r--r--   0        0        0    10910 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/enums/make_model.py
+-rw-r--r--   0        0        0     8099 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/enums/role.py
+-rw-r--r--   0        0        0     7274 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/enums/telemetry_name.py
+-rw-r--r--   0        0        0     4910 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/enums/unit.py
+-rw-r--r--   0        0        0      336 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/errors.py
+-rw-r--r--   0        0        0      249 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/gs/__init__.py
+-rw-r--r--   0        0        0      460 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/gs/gs_dispatch.py
+-rw-r--r--   0        0        0      800 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/gs/gs_dispatch_base.py
+-rw-r--r--   0        0        0      678 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/gs/gs_dispatch_maker.py
+-rw-r--r--   0        0        0      442 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/gs/gs_pwr.py
+-rw-r--r--   0        0        0      851 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/gs/gs_pwr_base.py
+-rw-r--r--   0        0        0      609 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/gs/gs_pwr_maker.py
+-rw-r--r--   0        0        0     3237 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/message.py
+-rw-r--r--   0        0        0     1474 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/messages/__init__.py
+-rw-r--r--   0        0        0     3068 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/messages/event.py
+-rw-r--r--   0        0        0      669 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/messages/misc.py
+-rw-r--r--   0        0        0    11428 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/property_format.py
+-rw-r--r--   0        0        0        0 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/py.typed
+-rw-r--r--   0        0        0     2892 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/topic.py
+-rw-r--r--   0        0        0     1051 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/type_helpers/__init__.py
+-rw-r--r--   0        0        0     8974 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/types/__init__.py
+-rw-r--r--   0        0        0     9990 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/types/component_attribute_class_gt.py
+-rw-r--r--   0        0        0    10683 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/types/component_gt.py
+-rw-r--r--   0        0        0     9168 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/types/data_channel.py
+-rw-r--r--   0        0        0     7734 2024-04-23 18:06:37.311031 gridworks_protocol-0.7.4/src/gwproto/types/egauge_io.py
+-rw-r--r--   0        0        0     8183 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/egauge_register_config.py
+-rw-r--r--   0        0        0    13383 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/electric_meter_cac_gt.py
+-rw-r--r--   0        0        0    18082 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/electric_meter_component_gt.py
+-rw-r--r--   0        0        0     2670 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/fibaro_smart_implant_cac_gt.py
+-rw-r--r--   0        0        0     2959 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/fibaro_smart_implant_component_gt.py
+-rw-r--r--   0        0        0    12880 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/gt_dispatch_boolean.py
+-rw-r--r--   0        0        0    10676 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/gt_dispatch_boolean_local.py
+-rw-r--r--   0        0        0     9579 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/gt_driver_booleanactuator_cmd.py
+-rw-r--r--   0        0        0     9646 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py
+-rw-r--r--   0        0        0     9258 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/gt_sh_cli_atn_cmd.py
+-rw-r--r--   0        0        0    11997 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py
+-rw-r--r--   0        0        0    11090 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/gt_sh_simple_telemetry_status.py
+-rw-r--r--   0        0        0    15695 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/gt_sh_status.py
+-rw-r--r--   0        0        0    11589 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py
+-rw-r--r--   0        0        0     8430 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/gt_telemetry.py
+-rw-r--r--   0        0        0    12904 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/heartbeat_b.py
+-rw-r--r--   0        0        0     2281 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/hubitat_cac_gt.py
+-rw-r--r--   0        0        0     4772 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/hubitat_component_gt.py
+-rw-r--r--   0        0        0     2555 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/hubitat_gt.py
+-rw-r--r--   0        0        0     1328 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/hubitat_poller_cac_gt.py
+-rw-r--r--   0        0        0     1573 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/hubitat_poller_component_gt.py
+-rw-r--r--   0        0        0     1697 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/hubitat_poller_gt.py
+-rw-r--r--   0        0        0     2469 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/hubitat_tank_cac_gt.py
+-rw-r--r--   0        0        0     3017 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/hubitat_tank_component_gt.py
+-rw-r--r--   0        0        0     8831 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/hubitat_tank_gt.py
+-rw-r--r--   0        0        0    13945 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/multipurpose_sensor_cac_gt.py
+-rw-r--r--   0        0        0    13879 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/multipurpose_sensor_component_gt.py
+-rw-r--r--   0        0        0    10163 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/pipe_flow_sensor_cac_gt.py
+-rw-r--r--   0        0        0    12226 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/pipe_flow_sensor_component_gt.py
+-rw-r--r--   0        0        0     5915 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/power_watts.py
+-rw-r--r--   0        0        0     9932 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/relay_cac_gt.py
+-rw-r--r--   0        0        0    11585 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/relay_component_gt.py
+-rw-r--r--   0        0        0    11465 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/resistive_heater_cac_gt.py
+-rw-r--r--   0        0        0    11819 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/resistive_heater_component_gt.py
+-rw-r--r--   0        0        0     2364 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/rest_poller_cac_gt.py
+-rw-r--r--   0        0        0     3033 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/rest_poller_component_gt.py
+-rw-r--r--   0        0        0     8900 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/rest_poller_gt.py
+-rw-r--r--   0        0        0    12488 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/simple_temp_sensor_cac_gt.py
+-rw-r--r--   0        0        0    11394 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/simple_temp_sensor_component_gt.py
+-rw-r--r--   0        0        0     9456 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/snapshot_spaceheat.py
+-rw-r--r--   0        0        0    14590 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/spaceheat_node_gt.py
+-rw-r--r--   0        0        0    12356 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/ta_data_channels.py
+-rw-r--r--   0        0        0    11281 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/telemetry_reporting_config.py
+-rw-r--r--   0        0        0    11369 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/telemetry_snapshot_spaceheat.py
+-rw-r--r--   0        0        0     1140 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/web_server_cac_gt.py
+-rw-r--r--   0        0        0     1463 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/web_server_component_gt.py
+-rw-r--r--   0        0        0      440 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/types/web_server_gt.py
+-rw-r--r--   0        0        0     2890 2024-04-23 18:06:37.315031 gridworks_protocol-0.7.4/src/gwproto/utils.py
+-rw-r--r--   0        0        0     4131 1970-01-01 00:00:00.000000 gridworks_protocol-0.7.4/PKG-INFO
```

### Comparing `gridworks_protocol-0.7.3/LICENSE` & `gridworks_protocol-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/README.md` & `gridworks_protocol-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/pyproject.toml` & `gridworks_protocol-0.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-protocol"
-version = "0.7.3"
+version = "0.7.4"
 description = "Gridworks Protocol"
 authors = ["Jessica Millar <jmillar@gridworks-consulting.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-protocol"
 repository = "https://github.com/thegridelectric/gridworks-protocol"
 documentation = "https://gridworks-protocol.readthedocs.io"
@@ -16,19 +16,19 @@
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/thegridelectric/gridworks-protocol/releases"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-pydantic = "^1.10.2"
-pendulum = "^3"
+pydantic = "^1.10.11"
 yarl = "^1.9.2"
 pytz = "^2024.1"
 fastapi-utils = "^0.2.1"
+pendulum = "2.1.2"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
```

### Comparing `gridworks_protocol-0.7.3/src/gwproto/__init__.py` & `gridworks_protocol-0.7.4/src/gwproto/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/electric_meter_cac.py` & `gridworks_protocol-0.7.4/src/gwproto/data_classes/cacs/electric_meter_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py` & `gridworks_protocol-0.7.4/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py` & `gridworks_protocol-0.7.4/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/relay_cac.py` & `gridworks_protocol-0.7.4/src/gwproto/data_classes/cacs/relay_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/resistive_heater_cac.py` & `gridworks_protocol-0.7.4/src/gwproto/data_classes/cacs/resistive_heater_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py` & `gridworks_protocol-0.7.4/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/data_classes/component.py` & `gridworks_protocol-0.7.4/src/gwproto/data_classes/component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/data_classes/component_attribute_class.py` & `gridworks_protocol-0.7.4/src/gwproto/data_classes/component_attribute_class.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/data_classes/components/electric_meter_component.py` & `gridworks_protocol-0.7.4/src/gwproto/data_classes/components/electric_meter_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/data_classes/components/fibaro_smart_implant_component.py` & `gridworks_protocol-0.7.4/src/gwproto/data_classes/components/fibaro_smart_implant_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/data_classes/components/hubitat_component.py` & `gridworks_protocol-0.7.4/src/gwproto/data_classes/components/hubitat_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/data_classes/components/hubitat_poller_component.py` & `gridworks_protocol-0.7.4/src/gwproto/data_classes/components/hubitat_poller_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/data_classes/components/hubitat_tank_component.py` & `gridworks_protocol-0.7.4/src/gwproto/data_classes/components/hubitat_tank_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/data_classes/components/multipurpose_sensor_component.py` & `gridworks_protocol-0.7.4/src/gwproto/data_classes/components/multipurpose_sensor_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/data_classes/components/pipe_flow_sensor_component.py` & `gridworks_protocol-0.7.4/src/gwproto/data_classes/components/pipe_flow_sensor_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/data_classes/components/relay_component.py` & `gridworks_protocol-0.7.4/src/gwproto/data_classes/components/relay_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/data_classes/components/resistive_heater_component.py` & `gridworks_protocol-0.7.4/src/gwproto/data_classes/components/resistive_heater_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/data_classes/components/rest_poller_component.py` & `gridworks_protocol-0.7.4/src/gwproto/data_classes/components/rest_poller_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/data_classes/components/simple_temp_sensor_component.py` & `gridworks_protocol-0.7.4/src/gwproto/data_classes/components/simple_temp_sensor_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/data_classes/components/web_server_component.py` & `gridworks_protocol-0.7.4/src/gwproto/data_classes/components/web_server_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/data_classes/hardware_layout.py` & `gridworks_protocol-0.7.4/src/gwproto/data_classes/hardware_layout.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/data_classes/sh_node.py` & `gridworks_protocol-0.7.4/src/gwproto/data_classes/sh_node.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/decoders.py` & `gridworks_protocol-0.7.4/src/gwproto/decoders.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/default_decoders.py` & `gridworks_protocol-0.7.4/src/gwproto/default_decoders.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/enums/__init__.py` & `gridworks_protocol-0.7.4/src/gwproto/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/enums/actor_class.py` & `gridworks_protocol-0.7.4/src/gwproto/enums/actor_class.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/enums/local_comm_interface.py` & `gridworks_protocol-0.7.4/src/gwproto/enums/local_comm_interface.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/enums/make_model.py` & `gridworks_protocol-0.7.4/src/gwproto/enums/make_model.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/enums/role.py` & `gridworks_protocol-0.7.4/src/gwproto/enums/role.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/enums/telemetry_name.py` & `gridworks_protocol-0.7.4/src/gwproto/enums/telemetry_name.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/enums/unit.py` & `gridworks_protocol-0.7.4/src/gwproto/enums/unit.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/gs/gs_dispatch_base.py` & `gridworks_protocol-0.7.4/src/gwproto/gs/gs_dispatch_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/gs/gs_dispatch_maker.py` & `gridworks_protocol-0.7.4/src/gwproto/gs/gs_dispatch_maker.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/gs/gs_pwr_base.py` & `gridworks_protocol-0.7.4/src/gwproto/gs/gs_pwr_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/gs/gs_pwr_maker.py` & `gridworks_protocol-0.7.4/src/gwproto/gs/gs_pwr_maker.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/message.py` & `gridworks_protocol-0.7.4/src/gwproto/message.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/messages/__init__.py` & `gridworks_protocol-0.7.4/src/gwproto/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/messages/event.py` & `gridworks_protocol-0.7.4/src/gwproto/messages/event.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/messages/misc.py` & `gridworks_protocol-0.7.4/src/gwproto/messages/misc.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/property_format.py` & `gridworks_protocol-0.7.4/src/gwproto/property_format.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/topic.py` & `gridworks_protocol-0.7.4/src/gwproto/topic.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/type_helpers/__init__.py` & `gridworks_protocol-0.7.4/src/gwproto/type_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/__init__.py` & `gridworks_protocol-0.7.4/src/gwproto/types/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/component_attribute_class_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/component_attribute_class_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/component_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/data_channel.py` & `gridworks_protocol-0.7.4/src/gwproto/types/data_channel.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/egauge_io.py` & `gridworks_protocol-0.7.4/src/gwproto/types/egauge_io.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/egauge_register_config.py` & `gridworks_protocol-0.7.4/src/gwproto/types/egauge_register_config.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/electric_meter_cac_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/electric_meter_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/electric_meter_component_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/electric_meter_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/fibaro_smart_implant_cac_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/fibaro_smart_implant_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/fibaro_smart_implant_component_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/fibaro_smart_implant_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/gt_dispatch_boolean.py` & `gridworks_protocol-0.7.4/src/gwproto/types/gt_dispatch_boolean.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/gt_dispatch_boolean_local.py` & `gridworks_protocol-0.7.4/src/gwproto/types/gt_dispatch_boolean_local.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/gt_driver_booleanactuator_cmd.py` & `gridworks_protocol-0.7.4/src/gwproto/types/gt_driver_booleanactuator_cmd.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py` & `gridworks_protocol-0.7.4/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_cli_atn_cmd.py` & `gridworks_protocol-0.7.4/src/gwproto/types/gt_sh_cli_atn_cmd.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py` & `gridworks_protocol-0.7.4/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_simple_telemetry_status.py` & `gridworks_protocol-0.7.4/src/gwproto/types/gt_sh_simple_telemetry_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_status.py` & `gridworks_protocol-0.7.4/src/gwproto/types/gt_sh_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py` & `gridworks_protocol-0.7.4/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/gt_telemetry.py` & `gridworks_protocol-0.7.4/src/gwproto/types/gt_telemetry.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/heartbeat_b.py` & `gridworks_protocol-0.7.4/src/gwproto/types/heartbeat_b.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/hubitat_cac_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/hubitat_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/hubitat_component_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/hubitat_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/hubitat_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/hubitat_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/hubitat_poller_cac_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/hubitat_poller_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/hubitat_poller_component_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/hubitat_poller_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/hubitat_poller_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/hubitat_poller_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/hubitat_tank_cac_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/hubitat_tank_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/hubitat_tank_component_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/hubitat_tank_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/hubitat_tank_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/hubitat_tank_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/multipurpose_sensor_cac_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/multipurpose_sensor_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/multipurpose_sensor_component_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/multipurpose_sensor_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/pipe_flow_sensor_cac_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/pipe_flow_sensor_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/pipe_flow_sensor_component_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/pipe_flow_sensor_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/power_watts.py` & `gridworks_protocol-0.7.4/src/gwproto/types/power_watts.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/relay_cac_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/relay_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/relay_component_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/relay_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/resistive_heater_cac_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/resistive_heater_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/resistive_heater_component_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/resistive_heater_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/rest_poller_cac_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/rest_poller_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/rest_poller_component_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/rest_poller_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/rest_poller_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/rest_poller_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/simple_temp_sensor_cac_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/simple_temp_sensor_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/simple_temp_sensor_component_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/simple_temp_sensor_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/snapshot_spaceheat.py` & `gridworks_protocol-0.7.4/src/gwproto/types/snapshot_spaceheat.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/spaceheat_node_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/spaceheat_node_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/ta_data_channels.py` & `gridworks_protocol-0.7.4/src/gwproto/types/ta_data_channels.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/telemetry_reporting_config.py` & `gridworks_protocol-0.7.4/src/gwproto/types/telemetry_reporting_config.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/telemetry_snapshot_spaceheat.py` & `gridworks_protocol-0.7.4/src/gwproto/types/telemetry_snapshot_spaceheat.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/web_server_cac_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/web_server_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/types/web_server_component_gt.py` & `gridworks_protocol-0.7.4/src/gwproto/types/web_server_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/src/gwproto/utils.py` & `gridworks_protocol-0.7.4/src/gwproto/utils.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.3/PKG-INFO` & `gridworks_protocol-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: gridworks-protocol
-Version: 0.7.3
+Version: 0.7.4
 Summary: Gridworks Protocol
 Home-page: https://github.com/thegridelectric/gridworks-protocol
 License: MIT
 Author: Jessica Millar
 Author-email: jmillar@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: fastapi-utils (>=0.2.1,<0.3.0)
-Requires-Dist: pendulum (>=3,<4)
-Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Requires-Dist: pendulum (==2.1.2)
+Requires-Dist: pydantic (>=1.10.11,<2.0.0)
 Requires-Dist: pytz (>=2024.1,<2025.0)
 Requires-Dist: yarl (>=1.9.2,<2.0.0)
 Project-URL: Changelog, https://github.com/thegridelectric/gridworks-protocol/releases
 Project-URL: Documentation, https://gridworks-protocol.readthedocs.io
 Project-URL: Repository, https://github.com/thegridelectric/gridworks-protocol
 Description-Content-Type: text/markdown
```

