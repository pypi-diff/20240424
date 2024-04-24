# Comparing `tmp/zigpy-0.63.5.tar.gz` & `tmp/zigpy-0.64.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zigpy-0.63.5.tar", last modified: Fri Mar  8 18:47:10 2024, max compression
+gzip compressed data, was "zigpy-0.64.0.tar", last modified: Wed Apr 24 14:26:12 2024, max compression
```

## Comparing `zigpy-0.63.5.tar` & `zigpy-0.64.0.tar`

### file list

```diff
@@ -1,121 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 18:47:10.104296 zigpy-0.63.5/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-08 18:47:05.000000 zigpy-0.63.5/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-03-08 18:47:05.000000 zigpy-0.63.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9010 2024-03-08 18:47:10.104296 zigpy-0.63.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-03-08 18:47:05.000000 zigpy-0.63.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-03-08 18:47:05.000000 zigpy-0.63.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 18:47:10.104296 zigpy-0.63.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-08 18:47:05.000000 zigpy-0.63.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 18:47:10.088296 zigpy-0.63.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_app_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    38300 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_appdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    15944 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_appdb_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_appdb_pysqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    46325 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_backups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_datastructures.py
--rw-r--r--   0 runner    (1001) docker     (127)    36540 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    11217 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_listeners.py
--rw-r--r--   0 runner    (1001) docker     (127)    35685 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_quirks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_quirks_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    29238 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_quirks_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_serial.py
--rw-r--r--   0 runner    (1001) docker     (127)    25225 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_struct.py
--rw-r--r--   0 runner    (1001) docker     (127)    12928 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_topology.py
--rw-r--r--   0 runner    (1001) docker     (127)    22446 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    38578 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_zcl.py
--rw-r--r--   0 runner    (1001) docker     (127)    16771 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_zcl_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)    25351 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_zcl_foundation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_zdo.py
--rw-r--r--   0 runner    (1001) docker     (127)    14523 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_zdo_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    17037 2024-03-08 18:47:05.000000 zigpy-0.63.5/tests/test_zigbee_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 18:47:10.092296 zigpy-0.63.5/zigpy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46523 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/appdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 18:47:10.096296 zigpy-0.63.5/zigpy/appdb_schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/appdb_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/appdb_schemas/schema_v0.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/appdb_schemas/schema_v1.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/appdb_schemas/schema_v10.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/appdb_schemas/schema_v11.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/appdb_schemas/schema_v12.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/appdb_schemas/schema_v2.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/appdb_schemas/schema_v3.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/appdb_schemas/schema_v4.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/appdb_schemas/schema_v5.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/appdb_schemas/schema_v6.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/appdb_schemas/schema_v7.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/appdb_schemas/schema_v8.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/appdb_schemas/schema_v9.sql
--rw-r--r--   0 runner    (1001) docker     (127)    48480 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/application.py
--rw-r--r--   0 runner    (1001) docker     (127)    16586 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/backups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 18:47:10.096296 zigpy-0.63.5/zigpy/config/
--rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/config/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (127)    22692 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    11748 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/listeners.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 18:47:10.096296 zigpy-0.63.5/zigpy/ota/
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/ota/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9289 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/ota/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/ota/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    30110 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/ota/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/ota/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 18:47:10.096296 zigpy-0.63.5/zigpy/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/profiles/zgp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/profiles/zha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/profiles/zll.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 18:47:10.096296 zigpy-0.63.5/zigpy/quirks/
--rw-r--r--   0 runner    (1001) docker     (127)    15803 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/quirks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/quirks/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 18:47:10.096296 zigpy-0.63.5/zigpy/quirks/v2/
--rw-r--r--   0 runner    (1001) docker     (127)    28208 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/quirks/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 18:47:10.100296 zigpy-0.63.5/zigpy/quirks/v2/homeassistant/
--rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/quirks/v2/homeassistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/quirks/v2/homeassistant/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/quirks/v2/homeassistant/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/quirks/v2/homeassistant/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/serial.py
--rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8525 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 18:47:10.100296 zigpy-0.63.5/zigpy/types/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26662 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/types/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    19561 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/types/named.py
--rw-r--r--   0 runner    (1001) docker     (127)    13601 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/types/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)    15502 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 18:47:10.100296 zigpy-0.63.5/zigpy/zcl/
--rw-r--r--   0 runner    (1001) docker     (127)    36170 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/zcl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 18:47:10.104296 zigpy-0.63.5/zigpy/zcl/clusters/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/zcl/clusters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28452 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/zcl/clusters/closures.py
--rw-r--r--   0 runner    (1001) docker     (127)    87388 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/zcl/clusters/general.py
--rw-r--r--   0 runner    (1001) docker     (127)    26113 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/zcl/clusters/homeautomation.py
--rw-r--r--   0 runner    (1001) docker     (127)    21147 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/zcl/clusters/hvac.py
--rw-r--r--   0 runner    (1001) docker     (127)    17332 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/zcl/clusters/lighting.py
--rw-r--r--   0 runner    (1001) docker     (127)     9421 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/zcl/clusters/lightlink.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/zcl/clusters/manufacturer_specific.py
--rw-r--r--   0 runner    (1001) docker     (127)    20097 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/zcl/clusters/measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)    16606 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/zcl/clusters/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    15046 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/zcl/clusters/security.py
--rw-r--r--   0 runner    (1001) docker     (127)    18998 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/zcl/clusters/smartenergy.py
--rw-r--r--   0 runner    (1001) docker     (127)    33004 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/zcl/foundation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 18:47:10.104296 zigpy-0.63.5/zigpy/zdo/
--rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/zdo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24087 2024-03-08 18:47:05.000000 zigpy-0.63.5/zigpy/zdo/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 18:47:10.104296 zigpy-0.63.5/zigpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9010 2024-03-08 18:47:10.000000 zigpy-0.63.5/zigpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-03-08 18:47:10.000000 zigpy-0.63.5/zigpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 18:47:10.000000 zigpy-0.63.5/zigpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-08 18:47:10.000000 zigpy-0.63.5/zigpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-08 18:47:10.000000 zigpy-0.63.5/zigpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:26:12.008177 zigpy-0.64.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-24 14:26:06.000000 zigpy-0.64.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-24 14:26:06.000000 zigpy-0.64.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-04-24 14:26:12.008177 zigpy-0.64.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-04-24 14:26:06.000000 zigpy-0.64.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-24 14:26:06.000000 zigpy-0.64.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:26:12.008177 zigpy-0.64.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 14:26:06.000000 zigpy-0.64.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:26:11.992177 zigpy-0.64.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_app_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38747 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_appdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15944 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_appdb_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_appdb_pysqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46325 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_backups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36540 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11217 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_listeners.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35685 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_quirks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_quirks_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29469 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_quirks_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25225 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12928 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22446 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38578 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_zcl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16771 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_zcl_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25351 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_zcl_foundation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_zdo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14523 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_zdo_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17037 2024-04-24 14:26:06.000000 zigpy-0.64.0/tests/test_zigbee_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:26:11.996177 zigpy-0.64.0/zigpy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50233 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/appdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:26:12.000177 zigpy-0.64.0/zigpy/appdb_schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/appdb_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/appdb_schemas/schema_v0.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/appdb_schemas/schema_v1.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/appdb_schemas/schema_v10.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/appdb_schemas/schema_v11.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/appdb_schemas/schema_v12.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/appdb_schemas/schema_v13.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/appdb_schemas/schema_v2.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/appdb_schemas/schema_v3.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/appdb_schemas/schema_v4.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/appdb_schemas/schema_v5.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/appdb_schemas/schema_v6.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/appdb_schemas/schema_v7.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/appdb_schemas/schema_v8.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/appdb_schemas/schema_v9.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    48480 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16586 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/backups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:26:12.000177 zigpy-0.64.0/zigpy/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/config/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8890 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22692 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12181 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/listeners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:26:12.000177 zigpy-0.64.0/zigpy/ota/
+-rw-r--r--   0 runner    (1001) docker     (127)    16419 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/ota/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9271 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/ota/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/ota/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30462 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/ota/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/ota/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:26:12.000177 zigpy-0.64.0/zigpy/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/profiles/zgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/profiles/zha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/profiles/zll.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:26:12.000177 zigpy-0.64.0/zigpy/quirks/
+-rw-r--r--   0 runner    (1001) docker     (127)    15803 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/quirks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/quirks/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:26:12.000177 zigpy-0.64.0/zigpy/quirks/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)    28514 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/quirks/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:26:12.004177 zigpy-0.64.0/zigpy/quirks/v2/homeassistant/
+-rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/quirks/v2/homeassistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/quirks/v2/homeassistant/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/quirks/v2/homeassistant/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/quirks/v2/homeassistant/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8525 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:26:12.004177 zigpy-0.64.0/zigpy/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26694 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/types/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19577 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/types/named.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13601 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/types/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15502 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:26:12.004177 zigpy-0.64.0/zigpy/zcl/
+-rw-r--r--   0 runner    (1001) docker     (127)    36301 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/zcl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:26:12.008177 zigpy-0.64.0/zigpy/zcl/clusters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/zcl/clusters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28488 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/zcl/clusters/closures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87736 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/zcl/clusters/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26185 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/zcl/clusters/homeautomation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21207 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/zcl/clusters/hvac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17356 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/zcl/clusters/lighting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/zcl/clusters/lightlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/zcl/clusters/manufacturer_specific.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20641 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/zcl/clusters/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16846 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/zcl/clusters/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15082 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/zcl/clusters/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19142 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/zcl/clusters/smartenergy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33004 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/zcl/foundation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:26:12.008177 zigpy-0.64.0/zigpy/zdo/
+-rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/zdo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24087 2024-04-24 14:26:06.000000 zigpy-0.64.0/zigpy/zdo/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:26:12.008177 zigpy-0.64.0/zigpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-04-24 14:26:11.000000 zigpy-0.64.0/zigpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-24 14:26:11.000000 zigpy-0.64.0/zigpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:26:11.000000 zigpy-0.64.0/zigpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-24 14:26:11.000000 zigpy-0.64.0/zigpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 14:26:11.000000 zigpy-0.64.0/zigpy.egg-info/top_level.txt
```

### Comparing `zigpy-0.63.5/COPYING` & `zigpy-0.64.0/COPYING`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/LICENSE` & `zigpy-0.64.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/PKG-INFO` & `zigpy-0.64.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy
-Version: 0.63.5
+Version: 0.64.0
 Summary: Library implementing a Zigbee stack
 Author-email: Russell Cloran <rcloran@gmail.com>
 License: GPL-3.0
 Project-URL: repository, https://github.com/zigpy/zigpy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -28,15 +28,14 @@
 Requires-Dist: coveralls; extra == "testing"
 Requires-Dist: coverage[toml]; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-asyncio; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-timeout; extra == "testing"
 Requires-Dist: freezegun; extra == "testing"
-Requires-Dist: ruff==0.0.261; extra == "testing"
 Requires-Dist: pysqlite3-binary; (platform_system == "Linux" and python_version < "3.12") and extra == "testing"
 
 # zigpy
 
 [![Build](https://github.com/zigpy/zigpy/workflows/CI/badge.svg?branch=dev)](https://github.com/zigpy/zigpy/workflows/CI/badge.svg?branch=dev)
 [![Coverage Status](https://codecov.io/gh/zigpy/zigpy/branch/dev/graph/badge.svg)](https://codecov.io/gh/zigpy/zigpy)
```

### Comparing `zigpy-0.63.5/README.md` & `zigpy-0.64.0/README.md`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/pyproject.toml` & `zigpy-0.64.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     "coveralls",
     "coverage[toml]",
     "pytest",
     "pytest-asyncio",
     "pytest-cov",
     "pytest-timeout",
     "freezegun",
-    "ruff==0.0.261",
     'pysqlite3-binary; platform_system=="Linux" and python_version<"3.12"',
 ]
 
 [tool.setuptools-git-versioning]
 enabled = true
 
 [tool.pytest.ini_options]
@@ -108,15 +107,15 @@
 line-length = 88
 
 [tool.ruff.per-file-ignores]
 "tests/*.py" = ["F811"]
 "zigpy/ota/provider.py" = ["SIM117"]
 
 [tool.pyupgrade]
-py37plus = true
+py38plus = true
 
 [tool.autoflake8]
 in-place = true
 recursive = false
 expand-star-imports = false
 exclude = [".venv", ".git", ".tox", "docs", "venv", "bin", "lib", "deps", "build"]
 
@@ -145,15 +144,14 @@
 
 [tool.codespell]
 ignore-words-list = "ser,nd,hass"
 skip = "./.*,tests/*,pyproject.toml"
 quiet-level = 2
 
 [tool.mypy]
-plugins = ["pydantic.mypy"]
 ignore_missing_imports = true
 install_types = true
 non_interactive = true
 show_error_codes = true
 show_error_context = true
 error_summary = true
 disable_error_code = [
```

### Comparing `zigpy-0.63.5/tests/test_app_state.py` & `zigpy-0.64.0/tests/test_app_state.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/tests/test_appdb.py` & `zigpy-0.64.0/tests/test_appdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,26 +133,30 @@
     ep.status = zigpy.endpoint.Status.ZDO_INIT
     ep.profile_id = 260
     ep.device_type = profiles.zha.DeviceType.PUMP
     ep = dev.add_endpoint(2)
     ep.status = zigpy.endpoint.Status.ZDO_INIT
     ep.profile_id = 260
     ep.device_type = 0xFFFD  # Invalid
-    clus = ep.add_input_cluster(0)
-    ep.add_output_cluster(1)
+    in_clus = ep.add_input_cluster(0)
+    out_clus = ep.add_output_cluster(0)
     ep = dev.add_endpoint(3)
     ep.status = zigpy.endpoint.Status.ZDO_INIT
     ep.profile_id = 49246
     ep.device_type = profiles.zll.DeviceType.COLOR_LIGHT
     app.device_initialized(dev)
-    clus.update_attribute(0, 99)
-    clus.update_attribute(4, bytes("Custom", "ascii"))
-    clus.update_attribute(5, bytes("Model", "ascii"))
-    clus.listener_event("cluster_command", 0)
-    clus.listener_event("general_command")
+
+    in_clus.update_attribute(0, 99)
+    in_clus.update_attribute(4, bytes("Custom", "ascii"))
+    in_clus.update_attribute(5, bytes("Model", "ascii"))
+    in_clus.listener_event("cluster_command", 0)
+    in_clus.listener_event("general_command")
+
+    out_clus.update_attribute(0, 99)
+
     dev.relays = relays_1
     signature = dev.get_signature()
     assert ep.endpoint_id in signature[SIG_ENDPOINTS]
     assert SIG_MANUFACTURER not in signature
     assert SIG_MODEL not in signature
     dev.manufacturer = "Custom"
     dev.model = "Model"
@@ -195,17 +199,18 @@
         app2 = await make_app_with_db(db)
     dev = app2.get_device(ieee)
     assert dev.endpoints[1].device_type == profiles.zha.DeviceType.PUMP
     assert dev.endpoints[2].device_type == 0xFFFD
     assert dev.endpoints[2].in_clusters[0]._attr_cache[0] == 99
     assert dev.endpoints[2].in_clusters[0]._attr_cache[4] == bytes("Custom", "ascii")
     assert dev.endpoints[2].in_clusters[0]._attr_cache[5] == bytes("Model", "ascii")
+    assert dev.endpoints[2].out_clusters[0].cluster_id == 0x0000
+    assert dev.endpoints[2].out_clusters[0]._attr_cache[0] == 99
     assert dev.endpoints[2].manufacturer == "Custom"
     assert dev.endpoints[2].model == "Model"
-    assert dev.endpoints[2].out_clusters[1].cluster_id == 1
     assert dev.endpoints[3].device_type == profiles.zll.DeviceType.COLOR_LIGHT
     assert dev.relays == relays_1
     # The timestamp won't be restored exactly but it is more than close enough
     assert abs(dev.last_seen - dev_last_seen) < 0.01
 
     dev = app2.get_device(custom_ieee)
     # This virtual attribute is added by the quirk, there is no corresponding cluster
@@ -782,30 +787,35 @@
         app.handle_join(99, ieee, 0)
 
     dev = app.get_device(ieee)
     ep = dev.add_endpoint(3)
     ep.status = zigpy.endpoint.Status.ZDO_INIT
     ep.profile_id = 260
     ep.device_type = profiles.zha.DeviceType.PUMP
-    clus = ep.add_input_cluster(0)
-    ep.add_output_cluster(1)
-    clus.update_attribute(4, "Custom")
-    clus.update_attribute(5, "Model")
+    in_clus = ep.add_input_cluster(0)
+    in_clus.update_attribute(4, "Custom")
+    in_clus.update_attribute(5, "Model")
     app.device_initialized(dev)
-    clus.add_unsupported_attribute(0x0010)
-    clus.add_unsupported_attribute("physical_env")
+
+    in_clus.add_unsupported_attribute(0x0010)
+    in_clus.add_unsupported_attribute("physical_env")
+
+    out_clus = ep.add_output_cluster(0)
+    out_clus.add_unsupported_attribute(0x0010)
     await app.shutdown()
 
     # Everything should've been saved - check that it re-loads
     app2 = await make_app_with_db(db)
     dev = app2.get_device(ieee)
     assert dev.is_initialized == dev_init
     assert dev.endpoints[3].device_type == profiles.zha.DeviceType.PUMP
     assert 0x0010 in dev.endpoints[3].in_clusters[0].unsupported_attributes
+    assert 0x0010 in dev.endpoints[3].out_clusters[0].unsupported_attributes
     assert "location_desc" in dev.endpoints[3].in_clusters[0].unsupported_attributes
+    assert "location_desc" in dev.endpoints[3].out_clusters[0].unsupported_attributes
     assert 0x0011 in dev.endpoints[3].in_clusters[0].unsupported_attributes
     assert "physical_env" in dev.endpoints[3].in_clusters[0].unsupported_attributes
     await app2.shutdown()
 
     async def mockrequest(
         is_general_req, command, schema, args, manufacturer=None, **kwargs
     ):
@@ -815,31 +825,36 @@
         return [[rar0010]]
 
     # Now lets remove an unsupported attribute and make sure it is removed
     app3 = await make_app_with_db(db)
     dev = app3.get_device(ieee)
     assert dev.is_initialized == dev_init
     assert dev.endpoints[3].device_type == profiles.zha.DeviceType.PUMP
-    cluster = dev.endpoints[3].in_clusters[0]
-    assert 0x0010 in dev.endpoints[3].in_clusters[0].unsupported_attributes
-    cluster.request = mockrequest
-    await cluster.read_attributes([0x0010], allow_cache=False)
-    assert 0x0010 not in dev.endpoints[3].in_clusters[0].unsupported_attributes
-    assert "location_desc" not in dev.endpoints[3].in_clusters[0].unsupported_attributes
-    assert dev.endpoints[3].in_clusters[0].get(0x0010) == "Not Removed"
-    assert 0x0011 in dev.endpoints[3].in_clusters[0].unsupported_attributes
-    assert "physical_env" in dev.endpoints[3].in_clusters[0].unsupported_attributes
+
+    in_cluster = dev.endpoints[3].in_clusters[0]
+    assert 0x0010 in in_cluster.unsupported_attributes
+    in_cluster.request = mockrequest
+    await in_cluster.read_attributes([0x0010], allow_cache=False)
+    assert 0x0010 not in in_cluster.unsupported_attributes
+    assert "location_desc" not in in_cluster.unsupported_attributes
+    assert in_cluster.get(0x0010) == "Not Removed"
+    assert 0x0011 in in_cluster.unsupported_attributes
+    assert "physical_env" in in_cluster.unsupported_attributes
+
+    out_cluster = dev.endpoints[3].out_clusters[0]
+    out_cluster.remove_unsupported_attribute(0x0010)
     await app3.shutdown()
 
     # Everything should've been saved - check that it re-loads
     app4 = await make_app_with_db(db)
     dev = app4.get_device(ieee)
     assert dev.is_initialized == dev_init
     assert dev.endpoints[3].device_type == profiles.zha.DeviceType.PUMP
     assert 0x0010 not in dev.endpoints[3].in_clusters[0].unsupported_attributes
+    assert 0x0010 not in dev.endpoints[3].out_clusters[0].unsupported_attributes
     assert dev.endpoints[3].in_clusters[0].get(0x0010) == "Not Removed"
     assert "location_desc" not in dev.endpoints[3].in_clusters[0].unsupported_attributes
     assert 0x0011 in dev.endpoints[3].in_clusters[0].unsupported_attributes
     assert "physical_env" in dev.endpoints[3].in_clusters[0].unsupported_attributes
     await app4.shutdown()
```

### Comparing `zigpy-0.63.5/tests/test_appdb_migration.py` & `zigpy-0.64.0/tests/test_appdb_migration.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/tests/test_appdb_pysqlite.py` & `zigpy-0.64.0/tests/test_appdb_pysqlite.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/tests/test_application.py` & `zigpy-0.64.0/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/tests/test_backups.py` & `zigpy-0.64.0/tests/test_backups.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/tests/test_config.py` & `zigpy-0.64.0/tests/test_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test configuration."""
+
 import pathlib
 import warnings
 
 import pytest
 import voluptuous as vol
 
 import zigpy.config
@@ -202,7 +203,27 @@
         zigpy.config.validators.cv_json_file(str(path))
 
     path.rmdir()
 
     # File exists
     path.write_text("{}")
     assert zigpy.config.validators.cv_json_file(str(path)) == path
+
+
+def test_cv_folder(tmp_path: pathlib.Path) -> None:
+    """ "Test `cv_folder` validator."""
+
+    folder_path = tmp_path / "folder"
+    file_path = tmp_path / "not_folder"
+
+    # Does not exist
+    with pytest.raises(vol.Invalid):
+        zigpy.config.validators.cv_folder(str(folder_path))
+
+    # Not a folder
+    file_path.write_text("")
+    with pytest.raises(vol.Invalid):
+        zigpy.config.validators.cv_folder(str(file_path))
+
+    # Folder exists
+    folder_path.mkdir()
+    assert zigpy.config.validators.cv_folder(str(folder_path)) == folder_path
```

### Comparing `zigpy-0.63.5/tests/test_datastructures.py` & `zigpy-0.64.0/tests/test_datastructures.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import asyncio
-from unittest.mock import Mock
+from unittest.mock import Mock, patch
 
 import pytest
 
 from zigpy import datastructures
 
 
 async def test_dynamic_bounded_semaphore_simple_locking():
@@ -283,15 +283,15 @@
     await asyncio.sleep(0.09)
     timeout.cancel()
     await asyncio.sleep(0.02)
     assert len(callback.mock_calls) == 0
 
 
 async def test_debouncer():
-    """ "Test debouncer."""
+    """Test debouncer."""
 
     debouncer = datastructures.Debouncer()
     debouncer.clean()
     assert repr(debouncer) == "<Debouncer [tracked:0]>"
 
     obj1 = object()
     assert not debouncer.is_filtered(obj1)
@@ -321,7 +321,30 @@
     assert debouncer.is_filtered(obj2)
     assert repr(debouncer) == "<Debouncer [tracked:1]>"
 
     await asyncio.sleep(0.1)
     assert not debouncer.is_filtered(obj1)
     assert not debouncer.is_filtered(obj2)
     assert repr(debouncer) == "<Debouncer [tracked:0]>"
+
+
+async def test_debouncer_low_resolution_clock():
+    """Test debouncer with a low resolution clock."""
+
+    loop = asyncio.get_running_loop()
+    now = loop.time()
+
+    # Make sure we can debounce on a low resolution clock
+    with patch.object(loop, "time", return_value=now):
+        debouncer = datastructures.Debouncer()
+
+        obj1 = object()
+        debouncer.filter(obj1, expire_in=0.1)
+        assert debouncer.is_filtered(obj1)
+
+        obj2 = object()
+        debouncer.filter(obj2, expire_in=0.1)
+        assert debouncer.is_filtered(obj2)
+
+        # The two objects cannot be compared
+        with pytest.raises(TypeError):
+            obj1 < obj2
```

### Comparing `zigpy-0.63.5/tests/test_device.py` & `zigpy-0.64.0/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/tests/test_endpoint.py` & `zigpy-0.64.0/tests/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/tests/test_group.py` & `zigpy-0.64.0/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/tests/test_listeners.py` & `zigpy-0.64.0/tests/test_listeners.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/tests/test_quirks.py` & `zigpy-0.64.0/tests/test_quirks.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/tests/test_quirks_registry.py` & `zigpy-0.64.0/tests/test_quirks_registry.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/tests/test_quirks_v2.py` & `zigpy-0.64.0/tests/test_quirks_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,17 @@
             OnOff.cluster_id,
         )
     )
 
     quirked = registry.get_device(device_mock)
     assert isinstance(quirked, CustomDeviceV2)
     assert quirked in registry
+    # this would need to be updated if the line number of the call to add_to_registry_v2
+    # changes in this test in the future
+    assert quirked.quirk_metadata.quirk_location.endswith("zigpy/tests/test_quirks_v2.py]-line:104")
 
     ep = quirked.endpoints[1]
 
     assert ep.basic is not None
     assert isinstance(ep.basic, Basic)
     assert isinstance(ep.basic, TestCustomCluster)
     # pylint: disable=protected-access
```

### Comparing `zigpy-0.63.5/tests/test_serial.py` & `zigpy-0.64.0/tests/test_serial.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/tests/test_struct.py` & `zigpy-0.64.0/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/tests/test_topology.py` & `zigpy-0.64.0/tests/test_topology.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/tests/test_types.py` & `zigpy-0.64.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/tests/test_zcl.py` & `zigpy-0.64.0/tests/test_zcl.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/tests/test_zcl_clusters.py` & `zigpy-0.64.0/tests/test_zcl_clusters.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/tests/test_zcl_foundation.py` & `zigpy-0.64.0/tests/test_zcl_foundation.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/tests/test_zdo.py` & `zigpy-0.64.0/tests/test_zdo.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/tests/test_zdo_types.py` & `zigpy-0.64.0/tests/test_zdo_types.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/tests/test_zigbee_util.py` & `zigpy-0.64.0/tests/test_zigbee_util.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/appdb.py` & `zigpy-0.64.0/zigpy/appdb.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,19 +20,20 @@
 import zigpy.profiles
 import zigpy.quirks
 import zigpy.state
 import zigpy.types as t
 import zigpy.typing
 import zigpy.util
 from zigpy.zcl.clusters.general import Basic
+from zigpy.zcl import ClusterType
 from zigpy.zdo import types as zdo_t
 
 LOGGER = logging.getLogger(__name__)
 
-DB_VERSION = 12
+DB_VERSION = 13
 DB_V = f"_v{DB_VERSION}"
 MIN_SQLITE_VERSION = (3, 24, 0)
 
 UNIX_EPOCH = datetime.fromtimestamp(0, tz=timezone.utc)
 DB_V_REGEX = re.compile(r"(?:_v\d+)?$")
 
 MIN_UPDATE_DELTA = timedelta(seconds=30).total_seconds()
@@ -274,68 +275,83 @@
         value: Any,
         timestamp: datetime,
     ) -> None:
         self.enqueue(
             "_save_attribute",
             cluster.endpoint.device.ieee,
             cluster.endpoint.endpoint_id,
+            cluster.cluster_type,
             cluster.cluster_id,
             attrid,
             value,
             timestamp,
         )
 
     def attribute_cleared(self, cluster: zigpy.typing.ClusterType, attrid: int) -> None:
         self.enqueue(
             "_clear_attribute",
             cluster.endpoint.device.ieee,
             cluster.endpoint.endpoint_id,
+            cluster.cluster_type,
             cluster.cluster_id,
             attrid,
         )
 
     def unsupported_attribute_added(
         self, cluster: zigpy.typing.ClusterType, attrid: int
     ) -> None:
         self.enqueue(
             "_unsupported_attribute_added",
             cluster.endpoint.device.ieee,
             cluster.endpoint.endpoint_id,
+            cluster.cluster_type,
             cluster.cluster_id,
             attrid,
         )
 
     async def _unsupported_attribute_added(
-        self, ieee: t.EUI64, endpoint_id: int, cluster_id: int, attrid: int
+        self,
+        ieee: t.EUI64,
+        endpoint_id: int,
+        cluster_type: ClusterType,
+        cluster_id: int,
+        attrid: int,
     ) -> None:
-        q = f"""INSERT INTO unsupported_attributes{DB_V} VALUES (?, ?, ?, ?)
-                   ON CONFLICT (ieee, endpoint_id, cluster, attrid)
+        q = f"""INSERT INTO unsupported_attributes{DB_V} VALUES (?, ?, ?, ?, ?)
+                   ON CONFLICT (ieee, endpoint_id, cluster_type, cluster_id, attr_id)
                    DO NOTHING"""
-        await self.execute(q, (ieee, endpoint_id, cluster_id, attrid))
+        await self.execute(q, (ieee, endpoint_id, cluster_type, cluster_id, attrid))
         await self._db.commit()
 
     def unsupported_attribute_removed(
         self, cluster: zigpy.typing.ClusterType, attrid: int
     ) -> None:
         self.enqueue(
             "_unsupported_attribute_removed",
             cluster.endpoint.device.ieee,
             cluster.endpoint.endpoint_id,
+            cluster.cluster_type,
             cluster.cluster_id,
             attrid,
         )
 
     async def _unsupported_attribute_removed(
-        self, ieee: t.EUI64, endpoint_id: int, cluster_id: int, attrid: int
+        self,
+        ieee: t.EUI64,
+        endpoint_id: int,
+        cluster_type: ClusterType,
+        cluster_id: int,
+        attrid: int,
     ) -> None:
         q = f"""DELETE FROM unsupported_attributes{DB_V} WHERE ieee = ?
                                                          AND endpoint_id = ?
-                                                         AND cluster = ?
-                                                         AND attrid = ?"""
-        await self.execute(q, (ieee, endpoint_id, cluster_id, attrid))
+                                                         AND cluster_type = ?
+                                                         AND cluster_id = ?
+                                                         AND attr_id = ?"""
+        await self.execute(q, (ieee, endpoint_id, cluster_type, cluster_id, attrid))
         await self._db.commit()
 
     def neighbors_updated(self, ieee: t.EUI64, neighbors: list[zdo_t.Neighbor]) -> None:
         """Neighbor update from Mgmt_Lqi_req."""
         self.enqueue("_neighbors_updated", ieee, neighbors)
 
     async def _neighbors_updated(
@@ -447,18 +463,17 @@
 
         if isinstance(device, zigpy.quirks.CustomDevice):
             await self._db.commit()
             return
 
         await self._save_endpoints(device)
         for ep in device.non_zdo_endpoints:
-            await self._save_input_clusters(ep)
+            await self._save_clusters(ep)
             await self._save_attribute_cache(ep)
             await self._save_unsupported_attributes(ep)
-            await self._save_output_clusters(ep)
         await self._db.commit()
 
     async def _save_endpoints(self, device: zigpy.typing.DeviceType) -> None:
         rows = [
             (
                 device.ieee,
                 ep.endpoint_id,
@@ -495,119 +510,126 @@
                 maximum_incoming_transfer_size=excluded.maximum_incoming_transfer_size,
                 server_mask=excluded.server_mask,
                 maximum_outgoing_transfer_size=excluded.maximum_outgoing_transfer_size,
                 descriptor_capability_field=excluded.descriptor_capability_field"""
 
         await self.execute(q, (device.ieee,) + device.node_desc.as_tuple())
 
-    async def _save_input_clusters(self, endpoint: zigpy.typing.EndpointType) -> None:
+    async def _save_clusters(self, endpoint: zigpy.typing.EndpointType) -> None:
         clusters = [
-            (endpoint.device.ieee, endpoint.endpoint_id, cluster.cluster_id)
-            for cluster in endpoint.in_clusters.values()
+            (
+                endpoint.device.ieee,
+                endpoint.endpoint_id,
+                cluster.cluster_type,
+                cluster.cluster_id,
+            )
+            for cluster in endpoint.clusters
         ]
-        q = f"""INSERT INTO in_clusters{DB_V} VALUES (?, ?, ?)
-                    ON CONFLICT (ieee, endpoint_id, cluster)
+        q = f"""INSERT INTO clusters{DB_V} VALUES (?, ?, ?, ?)
+                    ON CONFLICT (ieee, endpoint_id, cluster_type, cluster_id)
                     DO NOTHING"""
         await self._db.executemany(q, clusters)
 
     async def _save_attribute_cache(self, ep: zigpy.typing.EndpointType) -> None:
         clusters = [
             (
                 ep.device.ieee,
                 ep.endpoint_id,
+                cluster.cluster_type,
                 cluster.cluster_id,
                 attrid,
                 value,
                 cluster._attr_last_updated.get(attrid, UNIX_EPOCH).timestamp(),
             )
-            for cluster in ep.in_clusters.values()
+            for cluster in ep.clusters
             for attrid, value in cluster._attr_cache.items()
         ]
-        q = f"""INSERT INTO attributes_cache{DB_V} VALUES (?, ?, ?, ?, ?, ?)
-                    ON CONFLICT (ieee, endpoint_id, cluster, attrid)
+        q = f"""INSERT INTO attributes_cache{DB_V} VALUES (?, ?, ?, ?, ?, ?, ?)
+                    ON CONFLICT (ieee, endpoint_id, cluster_type, cluster_id, attr_id)
                     DO UPDATE SET value=excluded.value, last_updated=excluded.last_updated"""
         await self._db.executemany(q, clusters)
 
     async def _save_unsupported_attributes(self, ep: zigpy.typing.EndpointType) -> None:
         clusters = [
-            (ep.device.ieee, ep.endpoint_id, cluster.cluster_id, attr)
-            for cluster in ep.in_clusters.values()
+            (
+                ep.device.ieee,
+                ep.endpoint_id,
+                cluster.cluster_type,
+                cluster.cluster_id,
+                attr,
+            )
+            for cluster in ep.clusters
             for attr in cluster.unsupported_attributes
             if isinstance(attr, int)
         ]
-        q = f"""INSERT INTO unsupported_attributes{DB_V} VALUES (?, ?, ?, ?)
-                    ON CONFLICT (ieee, endpoint_id, cluster, attrid)
-                    DO NOTHING"""
-        await self._db.executemany(q, clusters)
-
-    async def _save_output_clusters(self, endpoint: zigpy.typing.EndpointType) -> None:
-        clusters = [
-            (endpoint.device.ieee, endpoint.endpoint_id, cluster.cluster_id)
-            for cluster in endpoint.out_clusters.values()
-        ]
-        q = f"""INSERT INTO out_clusters{DB_V} VALUES (?, ?, ?)
-                    ON CONFLICT (ieee, endpoint_id, cluster)
+        q = f"""INSERT INTO unsupported_attributes{DB_V} VALUES (?, ?, ?, ?, ?)
+                    ON CONFLICT (ieee, endpoint_id, cluster_type, cluster_id, attr_id)
                     DO NOTHING"""
         await self._db.executemany(q, clusters)
 
     async def _save_attribute(
         self,
         ieee: t.EUI64,
         endpoint_id: int,
+        cluster_type: ClusterType,
         cluster_id: int,
         attrid: int,
         value: Any,
         timestamp: datetime,
     ) -> None:
         q = f"""
             INSERT INTO attributes_cache{DB_V}
-            VALUES (:ieee, :endpoint_id, :cluster_id, :attrid, :value, :timestamp)
-                ON CONFLICT (ieee, endpoint_id, cluster, attrid) DO UPDATE
+            VALUES (:ieee, :endpoint_id, :cluster_type, :cluster_id, :attr_id, :value, :timestamp)
+                ON CONFLICT (ieee, endpoint_id, cluster_type, cluster_id, attr_id) DO UPDATE
                 SET value=excluded.value, last_updated=excluded.last_updated
                 WHERE
                     value != excluded.value
                     OR :timestamp - last_updated > :min_update_delta
             """
         await self.execute(
             q,
             {
                 "ieee": ieee,
                 "endpoint_id": endpoint_id,
+                "cluster_type": cluster_type,
                 "cluster_id": cluster_id,
-                "attrid": attrid,
+                "attr_id": attrid,
                 "value": value,
                 "timestamp": timestamp.timestamp(),
                 "min_update_delta": MIN_UPDATE_DELTA,
             },
         )
         await self._db.commit()
 
     async def _clear_attribute(
         self,
         ieee: t.EUI64,
         endpoint_id: int,
+        cluster_type: ClusterType,
         cluster_id: int,
         attrid: int,
     ) -> None:
         q = f"""
             DELETE FROM attributes_cache{DB_V}
             WHERE
                 ieee = :ieee
                 AND endpoint_id = :endpoint_id
-                AND cluster = :cluster_id
-                AND attrid = :attrid
+                AND cluster_type = :cluster_type
+                AND cluster_id = :cluster_id
+                AND attr_id = :attr_id
             """
 
         await self.execute(
             q,
             {
                 "ieee": ieee,
                 "endpoint_id": endpoint_id,
+                "cluster_type": cluster_type,
                 "cluster_id": cluster_id,
-                "attrid": attrid,
+                "attr_id": attrid,
             },
         )
         await self._db.commit()
 
     def network_backup_created(self, backup: zigpy.backups.NetworkBackup) -> None:
         self.enqueue("_network_backup_created", json.dumps(backup.as_dict()))
 
@@ -634,15 +656,24 @@
         LOGGER.debug("Loading application state")
         await self._load_devices()
         await self._load_node_descriptors()
         await self._load_endpoints()
         await self._load_clusters()
 
         # Quirks require the manufacturer and model name to be populated
-        await self._load_attributes("attrid=4 OR attrid=5")
+        await self._load_attributes(
+            f"""
+                cluster_type={ClusterType.Server}
+            AND cluster_id={Basic.cluster_id}
+            AND (
+                   attr_id={Basic.AttributeDefs.manufacturer.id}
+                OR attr_id={Basic.AttributeDefs.model.id}
+            )
+            """
+        )
 
         for device in self._application.devices.values():
             device = zigpy.quirks.get_device(device)
             self._application.devices[device.ieee] = device
 
         await self._load_attributes()
         await self._load_unsupported_attributes()
@@ -660,70 +691,82 @@
         else:
             query = f"SELECT * FROM attributes_cache{DB_V}"
 
         async with self.execute(query) as cursor:
             async for (
                 ieee,
                 endpoint_id,
-                cluster,
-                attrid,
+                cluster_type,
+                cluster_id,
+                attr_id,
                 value,
                 last_updated,
             ) in cursor:
                 dev = self._application.get_device(ieee)
 
                 # Some quirks create endpoints and clusters that do not exist
                 if endpoint_id not in dev.endpoints:
                     continue
 
                 ep = dev.endpoints[endpoint_id]
+                clusters = (
+                    ep.in_clusters
+                    if cluster_type == ClusterType.Server
+                    else ep.out_clusters
+                )
 
-                if cluster not in ep.in_clusters:
+                if cluster_id not in clusters:
                     continue
 
-                ep.in_clusters[cluster]._attr_cache[attrid] = value
-                ep.in_clusters[cluster]._attr_last_updated[
-                    attrid
+                clusters[cluster_id]._attr_cache[attr_id] = value
+                clusters[cluster_id]._attr_last_updated[
+                    attr_id
                 ] = datetime.fromtimestamp(last_updated, timezone.utc)
 
                 LOGGER.debug(
                     "[0x%04x:%s:0x%04x] Attribute id: %s value: %s",
                     dev.nwk,
                     endpoint_id,
-                    cluster,
-                    attrid,
+                    cluster_id,
+                    attr_id,
                     value,
                 )
 
                 # Populate the device's manufacturer and model attributes
-                if cluster == Basic.cluster_id and attrid == 0x0004:
+                if cluster_id == Basic.cluster_id and attr_id == Basic.AttributeDefs.manufacturer.id:
                     dev.manufacturer = decode_str_attribute(value)
-                elif cluster == Basic.cluster_id and attrid == 0x0005:
+                elif cluster_id == Basic.cluster_id and attr_id == Basic.AttributeDefs.model.id:
                     dev.model = decode_str_attribute(value)
 
     async def _load_unsupported_attributes(self) -> None:
         """Load unsuppoted attributes."""
 
         async with self.execute(
             f"SELECT * FROM unsupported_attributes{DB_V}"
         ) as cursor:
-            async for (ieee, endpoint_id, cluster_id, attrid) in cursor:
+            async for (ieee, endpoint_id, cluster_type, cluster_id, attr_id) in cursor:
                 dev = self._application.get_device(ieee)
 
                 try:
                     ep = dev.endpoints[endpoint_id]
                 except KeyError:
                     continue
 
+                clusters = (
+                    ep.in_clusters
+                    if cluster_type == ClusterType.Server
+                    else ep.out_clusters
+                )
+
                 try:
-                    cluster = ep.in_clusters[cluster_id]
+                    cluster = clusters[cluster_id]
                 except KeyError:
                     continue
 
-                cluster.add_unsupported_attribute(attrid, inhibit_events=True)
+                cluster.add_unsupported_attribute(attr_id, inhibit_events=True)
 
     async def _load_devices(self) -> None:
         async with self.execute(f"SELECT * FROM devices{DB_V}") as cursor:
             async for (ieee, nwk, status, last_seen) in cursor:
                 dev = self._application.add_device(ieee, nwk)
                 dev.status = zigpy.device.Status(status)
 
@@ -749,25 +792,23 @@
                     ep.device_type = zigpy.profiles.zha.DeviceType(device_type)
                 elif profile_id == zigpy.profiles.zll.PROFILE_ID:
                     ep.device_type = zigpy.profiles.zll.DeviceType(device_type)
                 else:
                     ep.device_type = device_type
 
     async def _load_clusters(self) -> None:
-        async with self.execute(f"SELECT * FROM in_clusters{DB_V}") as cursor:
-            async for (ieee, endpoint_id, cluster) in cursor:
+        async with self.execute(f"SELECT * FROM clusters{DB_V}") as cursor:
+            async for (ieee, endpoint_id, cluster_type, cluster_id) in cursor:
                 dev = self._application.get_device(ieee)
                 ep = dev.endpoints[endpoint_id]
-                ep.add_input_cluster(cluster)
 
-        async with self.execute(f"SELECT * FROM out_clusters{DB_V}") as cursor:
-            async for (ieee, endpoint_id, cluster) in cursor:
-                dev = self._application.get_device(ieee)
-                ep = dev.endpoints[endpoint_id]
-                ep.add_output_cluster(cluster)
+                if ClusterType(cluster_type) == ClusterType.Server:
+                    ep.add_input_cluster(cluster_id)
+                else:
+                    ep.add_output_cluster(cluster_id)
 
     async def _load_groups(self) -> None:
         async with self.execute(f"SELECT * FROM groups{DB_V}") as cursor:
             async for (group_id, name) in cursor:
                 self._application.groups.add_group(group_id, name, suppress_event=True)
 
     async def _load_group_members(self) -> None:
@@ -898,14 +939,15 @@
                 (self._migrate_to_v6, 6),
                 (self._migrate_to_v7, 7),
                 (self._migrate_to_v8, 8),
                 (self._migrate_to_v9, 9),
                 (self._migrate_to_v10, 10),
                 (self._migrate_to_v11, 11),
                 (self._migrate_to_v12, 12),
+                (self._migrate_to_v13, 13),
             ]:
                 if db_version >= min(to_db_version, DB_VERSION):
                     continue
 
                 LOGGER.info(
                     "Migrating database from v%d to v%d", db_version, to_db_version
                 )
@@ -1202,7 +1244,71 @@
         async with self.execute("SELECT * FROM attributes_cache_v11") as cursor:
             async for (ieee, endpoint_id, cluster_id, attrid, value) in cursor:
                 # Set the default `last_updated` to the unix epoch
                 await self.execute(
                     "INSERT INTO attributes_cache_v12 VALUES (?, ?, ?, ?, ?, ?)",
                     (ieee, endpoint_id, cluster_id, attrid, value, 0),
                 )
+
+    async def _migrate_to_v13(self):
+        """Schema v13 combines both cluster types and caching for all attributes."""
+
+        await self._migrate_tables(
+            {
+                "devices_v12": "devices_v13",
+                "endpoints_v12": "endpoints_v13",
+                "neighbors_v12": "neighbors_v13",
+                "routes_v12": "routes_v13",
+                "node_descriptors_v12": "node_descriptors_v13",
+                "groups_v12": "groups_v13",
+                "group_members_v12": "group_members_v13",
+                "relays_v12": "relays_v13",
+                "network_backups_v12": "network_backups_v13",
+                "in_clusters_v12": None,
+                "out_clusters_v12": None,
+                "unsupported_attributes_v12": None,
+                "attributes_cache_v12": None,
+            }
+        )
+
+        async with self.execute("SELECT * FROM in_clusters_v12") as cursor:
+            async for (ieee, endpoint_id, cluster_id) in cursor:
+                await self.execute(
+                    "INSERT INTO clusters_v13 VALUES (?, ?, ?, ?)",
+                    (ieee, endpoint_id, ClusterType.Server, cluster_id),
+                )
+
+        async with self.execute("SELECT * FROM out_clusters_v12") as cursor:
+            async for (ieee, endpoint_id, cluster_id) in cursor:
+                await self.execute(
+                    "INSERT INTO clusters_v13 VALUES (?, ?, ?, ?)",
+                    (ieee, endpoint_id, ClusterType.Client, cluster_id),
+                )
+
+        async with self.execute("SELECT * FROM unsupported_attributes_v12") as cursor:
+            async for (ieee, endpoint_id, cluster_id, attrid) in cursor:
+                await self.execute(
+                    "INSERT INTO unsupported_attributes_v13 VALUES (?, ?, ?, ?, ?)",
+                    (ieee, endpoint_id, ClusterType.Server, cluster_id, attrid),
+                )
+
+        async with self.execute("SELECT * FROM attributes_cache_v12") as cursor:
+            async for (
+                ieee,
+                endpoint_id,
+                cluster_id,
+                attrid,
+                value,
+                last_updated,
+            ) in cursor:
+                await self.execute(
+                    "INSERT INTO attributes_cache_v13 VALUES (?, ?, ?, ?, ?, ?, ?)",
+                    (
+                        ieee,
+                        endpoint_id,
+                        ClusterType.Server,
+                        cluster_id,
+                        attrid,
+                        value,
+                        last_updated,
+                    ),
+                )
```

### Comparing `zigpy-0.63.5/zigpy/appdb_schemas/schema_v0.sql` & `zigpy-0.64.0/zigpy/appdb_schemas/schema_v0.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/appdb_schemas/schema_v1.sql` & `zigpy-0.64.0/zigpy/appdb_schemas/schema_v1.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/appdb_schemas/schema_v10.sql` & `zigpy-0.64.0/zigpy/appdb_schemas/schema_v10.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/appdb_schemas/schema_v11.sql` & `zigpy-0.64.0/zigpy/appdb_schemas/schema_v11.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/appdb_schemas/schema_v12.sql` & `zigpy-0.64.0/zigpy/appdb_schemas/schema_v12.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/appdb_schemas/schema_v2.sql` & `zigpy-0.64.0/zigpy/appdb_schemas/schema_v2.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/appdb_schemas/schema_v3.sql` & `zigpy-0.64.0/zigpy/appdb_schemas/schema_v3.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/appdb_schemas/schema_v4.sql` & `zigpy-0.64.0/zigpy/appdb_schemas/schema_v4.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/appdb_schemas/schema_v5.sql` & `zigpy-0.64.0/zigpy/appdb_schemas/schema_v5.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/appdb_schemas/schema_v6.sql` & `zigpy-0.64.0/zigpy/appdb_schemas/schema_v6.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/appdb_schemas/schema_v7.sql` & `zigpy-0.64.0/zigpy/appdb_schemas/schema_v7.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/appdb_schemas/schema_v8.sql` & `zigpy-0.64.0/zigpy/appdb_schemas/schema_v8.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/appdb_schemas/schema_v9.sql` & `zigpy-0.64.0/zigpy/appdb_schemas/schema_v9.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/application.py` & `zigpy-0.64.0/zigpy/application.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/backups.py` & `zigpy-0.64.0/zigpy/backups.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/config/__init__.py` & `zigpy-0.64.0/zigpy/config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     CONF_TOPO_SKIP_COORDINATOR_DEFAULT,
     CONF_WATCHDOG_ENABLED_DEFAULT,
 )
 from zigpy.config.validators import (
     cv_boolean,
     cv_deprecated,
     cv_exact_object,
+    cv_folder,
     cv_hex,
     cv_json_file,
     cv_key,
     cv_simple_descriptor,
 )
 import zigpy.types as t
 
@@ -181,15 +182,15 @@
     ): vol.Any(None, cv_json_file),
     vol.Optional(
         CONF_OTA_Z2M_REMOTE_INDEX, default=CONF_OTA_Z2M_REMOTE_INDEX_DEFAULT
     ): vol.Any(None, vol.Url()),
     # Advanced OTA config. You *do not* need to use this unless you're testing a new
     # OTA firmware that has no known metadata.
     vol.Optional(CONF_OTA_ADVANCED_DIR, default=CONF_OTA_ADVANCED_DIR_DEFAULT): vol.Any(
-        None, str
+        None, cv_folder
     ),
     vol.Optional(
         CONF_OTA_ALLOW_ADVANCED_DIR, default=CONF_OTA_ALLOW_ADVANCED_DIR_DEFAULT
     ): vol.All(cv_exact_object(CONF_OTA_ALLOW_ADVANCED_DIR_STRING)),
     # Deprecated keys
     vol.Optional(CONF_OTA_SONOFF_URL): vol.Any(
         cv_deprecated("The `sonoff_update_url` key has been removed")
```

### Comparing `zigpy-0.63.5/zigpy/config/defaults.py` & `zigpy-0.64.0/zigpy/config/defaults.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/config/validators.py` & `zigpy-0.64.0/zigpy/config/validators.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,7 +103,17 @@
     """Validate a JSON file."""
     path = pathlib.Path(value)
 
     if not path.is_file():
         raise vol.Invalid(f"{value} is not a JSON file")
 
     return path
+
+
+def cv_folder(value: str) -> pathlib.Path:
+    """Validate a folder path."""
+    path = pathlib.Path(value)
+
+    if not path.is_dir():
+        raise vol.Invalid(f"{value} is not a directory")
+
+    return path
```

### Comparing `zigpy-0.63.5/zigpy/const.py` & `zigpy-0.64.0/zigpy/const.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/datastructures.py` & `zigpy-0.64.0/zigpy/datastructures.py`

 * *Files 5% similar despite different names*

```diff
@@ -220,28 +220,31 @@
 
 
 class Debouncer:
     """Generic debouncer supporting per-invocation expiration."""
 
     def __init__(self):
         self._times: dict[typing.Any, float] = {}
-        self._queue: list[tuple[float, typing.Any]] = []
+        self._queue: list[tuple[float, int, typing.Any]] = []
+
+        self._last_time: int = 0
+        self._dedup_counter: int = 0
 
     @functools.cached_property
     def _loop(self) -> asyncio.BaseEventLoop:
         return asyncio.get_running_loop()
 
     def clean(self, now: float | None = None) -> None:
         """Clean up stale timers."""
         if now is None:
             now = self._loop.time()
 
         # We store the negative expiration time to ensure we can pop expiring objects
         while self._queue and -self._queue[-1][0] < now:
-            _, obj = self._queue.pop()
+            _, _, obj = self._queue.pop()
             self._times.pop(obj)
 
     def is_filtered(self, obj: typing.Any, now: float | None = None) -> bool:
         """Check if an object will be filtered."""
         if now is None:
             now = self._loop.time()
 
@@ -251,20 +254,28 @@
         # If an object still exists after cleaning, it won't be expired
         return obj in self._times
 
     def filter(self, obj: typing.Any, expire_in: float) -> bool:
         """Check if an object should be filtered. If not, store it."""
         now = self._loop.time()
 
+        # For platforms with low-resolution clocks, we need to make sure that `obj` will
+        # never be compared by `heapq`!
+        if now > self._last_time:
+            self._last_time = now
+            self._dedup_counter = 0
+
+        self._dedup_counter += 1
+
         # If the object is filtered, do nothing
         if self.is_filtered(obj, now=now):
             return True
 
         # Otherwise, queue it
         self._times[obj] = now + expire_in
-        heapq.heappush(self._queue, (-(now + expire_in), obj))
+        heapq.heappush(self._queue, (-(now + expire_in), self._dedup_counter, obj))
 
         return False
 
     def __repr__(self) -> str:
         """String representation of the debouncer."""
         return f"<{self.__class__.__name__} [tracked:{len(self._queue)}]>"
```

### Comparing `zigpy-0.63.5/zigpy/device.py` & `zigpy-0.64.0/zigpy/device.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/endpoint.py` & `zigpy-0.64.0/zigpy/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,19 @@
                 self.add_input_cluster(cluster)
 
             for cluster in sd.output_clusters:
                 self.add_output_cluster(cluster)
 
         self.status = Status.ZDO_INIT
 
+    @property
+    def clusters(self) -> list[zigpy.zcl.Cluster]:
+        """Return all clusters on this endpoint."""
+        return [*self.in_clusters.values(), *self.out_clusters.values()]
+
     def add_input_cluster(
         self, cluster_id: int, cluster: zigpy.zcl.Cluster | None = None
     ) -> zigpy.zcl.Cluster:
         """Adds an endpoint's input cluster
 
         (a server cluster supported by the device)
         """
@@ -126,14 +131,21 @@
         if cluster is None:
             if cluster_id in self.out_clusters:
                 return self.out_clusters[cluster_id]
 
             cluster = zigpy.zcl.Cluster.from_id(self, cluster_id, is_server=False)
 
         self.out_clusters[cluster_id] = cluster
+
+        if self._device.application._dblistener is not None:
+            listener = zigpy.zcl.ClusterPersistingListener(
+                self._device.application._dblistener, cluster
+            )
+            cluster.add_listener(listener)
+
         return cluster
 
     async def add_to_group(self, grp_id: int, name: str | None = None) -> ZCLStatus:
         try:
             res = await self.groups.add(grp_id, name)
         except AttributeError:
             self.debug("Cannot add 0x%04x group, no groups cluster", grp_id)
```

### Comparing `zigpy-0.63.5/zigpy/exceptions.py` & `zigpy-0.64.0/zigpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/group.py` & `zigpy-0.64.0/zigpy/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,17 +81,15 @@
             foundation.GeneralCommand.Default_Response
         ].schema(
             status=foundation.Status.SUCCESS,
             command_id=data[2],
         )
 
     def __repr__(self) -> str:
-        return "<{} group_id={} name='{}' members={}>".format(
-            self.__class__.__name__, self.group_id, self.name, super().__repr__()
-        )
+        return f"<{self.__class__.__name__} group_id={self.group_id} name='{self.name}' members={super().__repr__()}>"
 
     @property
     def application(self) -> ControllerApplication:
         """Expose application to FakeEndpoint/GroupCluster."""
         return self.groups.application
 
     @property
```

### Comparing `zigpy-0.63.5/zigpy/listeners.py` & `zigpy-0.64.0/zigpy/listeners.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/ota/__init__.py` & `zigpy-0.64.0/zigpy/ota/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """OTA support for Zigbee devices."""
+
 from __future__ import annotations
 
 import asyncio
 import dataclasses
 import logging
 import sys
 import typing
```

### Comparing `zigpy-0.63.5/zigpy/ota/image.py` & `zigpy-0.64.0/zigpy/ota/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,15 @@
         return self >> 8
 
     @property
     def revision(self):
         return self & 0x00FF
 
     def __repr__(self):
-        return "<{} version={} revision={}>".format(
-            self.__class__.__name__, self.version, self.revision
-        )
+        return f"<{self.__class__.__name__} version={self.version} revision={self.revision}>"
 
 
 class HeaderString(bytes):
     _size = 32
 
     def __new__(cls, value: str | bytes):
         if isinstance(value, str):
@@ -210,15 +208,15 @@
 
 @attr.s
 class HueSBLOTAImage(BaseOTAImage):
     """Unique OTA image format for certain Hue devices. Starts with a valid header but does
     not contain any valid subelements beyond that point.
     """
 
-    SUBELEMENTS_MAGIC = b"\x2A\x00\x01"
+    SUBELEMENTS_MAGIC = b"\x2a\x00\x01"
 
     header = attr.ib(default=None)
     data = attr.ib(default=None)
 
     def serialize(self) -> bytes:
         return self.header.serialize() + self.data
 
@@ -238,15 +236,15 @@
             )
 
         if header.manufacturer_id != 4107:
             raise ValueError(
                 f"Only Hue images are expected. Got: {header.manufacturer_id}"
             )
 
-        return cls(header=header, data=firmware), data[header.image_size :]
+        return cls(header=header, data=firmware), data[header.image_size :]  # type: ignore
 
 
 def parse_ota_image(data: bytes) -> tuple[BaseOTAImage, bytes]:
     """Attempts to extract any known OTA image type from data. Does not validate firmware."""
 
     if len(data) > 4 and int.from_bytes(data[0:4], "little") + 21 == len(data):
         # Legrand OTA images are prefixed with their unwrapped size and include a 1 + 16
```

### Comparing `zigpy-0.63.5/zigpy/ota/manager.py` & `zigpy-0.64.0/zigpy/ota/manager.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/ota/providers.py` & `zigpy-0.64.0/zigpy/ota/providers.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,21 +34,24 @@
     checksum: str | None = None
     file_size: int | None = None
 
     manufacturer_names: tuple[str] = ()
     model_names: tuple[str] = ()
 
     changelog: str | None = None
+    release_notes: str | None = None
 
     min_hardware_version: int | None = None
     max_hardware_version: int | None = None
     min_current_file_version: int | None = None
     max_current_file_version: int | None = None
     specificity: int | None = None
 
+    source: str = "Unknown"
+
     async def _fetch(self) -> bytes:
         raise NotImplementedError()
 
     async def fetch(self) -> BaseOTAImage:
         data = await self._fetch()
 
         if self.file_size is not None and len(data) != self.file_size:
@@ -270,14 +273,15 @@
 
             yield IkeaRemoteOtaImageMetadata(  # type: ignore[call-arg]
                 file_version=int(file_version_match.group("v"), 10),
                 manufacturer_id=self.MANUFACTURER_IDS[0],
                 image_type=fw["fw_image_type"],
                 checksum="sha3-256:" + fw["fw_sha3_256"],
                 url=fw["fw_binary_url"],
+                source="IKEA",
             )
 
 
 class Ledvance(BaseOtaProvider):
     # This isn't static but no more than these two have ever existed
     MANUFACTURER_IDS = [4489, 4364]
 
@@ -367,15 +371,16 @@
                             "Version": (
                                 f"{version['major']}.{version['minor']}"
                                 f".{version['build']}.{version['revision']}"
                             ),
                         }
                     )
                 ),
-                changelog=fw["releaseNotes"],
+                release_notes=fw["releaseNotes"],
+                source="Ledvance",
             )
 
 
 class Salus(BaseOtaProvider):
     MANUFACTURER_IDS = [4216, 43981]
 
     JSON_SCHEMA = {
@@ -416,20 +421,17 @@
                 continue
 
             # Not every firmware is actually Zigbee but since they filter by model name
             # there is little chance an invalid one will ever be matched
             yield SalusRemoteOtaImageMetadata(  # type: ignore[call-arg]
                 file_version=int(fw["version"], 16),
                 model_names=(fw["model"],),
-                manufacturer_id=None,
-                image_type=None,
-                checksum=None,
-                file_size=None,
                 # Upgrade HTTP to HTTPS, the server supports it
                 url=fw["url"].replace("http://", "https://", 1),
+                source="SALUS",
             )
 
 
 class Sonoff(BaseOtaProvider):
     MANUFACTURER_IDS = [4742]
 
     JSON_SCHEMA = {
@@ -469,14 +471,15 @@
             yield RemoteOtaImageMetadata(  # type: ignore[call-arg]
                 file_version=fw["fw_file_version"],
                 manufacturer_id=fw["fw_manufacturer_id"],
                 image_type=fw["fw_image_type"],
                 file_size=fw["fw_filesize"],
                 url=fw["fw_binary_url"],
                 model_names=(fw["model_id"],),
+                source="Sonoff",
             )
 
 
 class Inovelli(BaseOtaProvider):
     MANUFACTURER_IDS = [4655]
 
     JSON_SCHEMA = {
@@ -508,15 +511,15 @@
         },
     }
 
     async def _load_index(
         self, session: aiohttp.ClientSession
     ) -> typing.AsyncIterator[BaseOtaImageMetadata]:
         async with session.get(
-            "https://files.inovelli.com/firmware/firmware-zha.json"
+            "https://files.inovelli.com/firmware/firmware-zha-v2.json"
         ) as rsp:
             fw_lst = await rsp.json()
 
         jsonschema.validate(fw_lst, self.JSON_SCHEMA)
 
         for model, firmwares in fw_lst.items():
             for fw in firmwares:
@@ -527,17 +530,16 @@
                     version = int(fw["version"])
 
                 yield RemoteOtaImageMetadata(  # type: ignore[call-arg]
                     file_version=version,
                     manufacturer_id=fw["manufacturer_id"],
                     image_type=fw["image_type"],
                     model_names=(model,),
-                    checksum=None,
-                    file_size=None,
                     url=fw["firmware"],
+                    source="Inovelli",
                 )
 
 
 class ThirdReality(BaseOtaProvider):
     MANUFACTURER_IDS = [4659, 4877]
 
     JSON_SCHEMA = {
@@ -582,17 +584,16 @@
 
         for fw in fw_lst["versions"]:
             yield RemoteOtaImageMetadata(  # type: ignore[call-arg]
                 file_version=fw["fileVersion"],
                 manufacturer_id=fw["manufacturerId"],
                 model_names=(fw["modelId"],),
                 image_type=fw["imageType"],
-                checksum=None,
-                file_size=None,
                 url=fw["url"],
+                source="ThirdReality",
             )
 
 
 class RemoteProvider(BaseOtaProvider):
     JSON_SCHEMA = {
         "$schema": "http://json-schema.org/draft-07/schema#",
         "type": "object",
@@ -609,14 +610,15 @@
                         "manufacturer_names": {
                             "type": "array",
                             "items": {"type": "string"},
                         },
                         "model_names": {"type": "array", "items": {"type": "string"}},
                         "manufacturer_id": {"type": "integer"},
                         "changelog": {"type": "string"},
+                        "release_notes": {"type": "string"},
                         "checksum": {
                             "type": "string",
                             "pattern": "^sha3-256:[a-f0-9]{64}$",
                         },
                         "min_hardware_version": {"type": "integer"},
                         "max_hardware_version": {"type": "integer"},
                         "min_current_file_version": {"type": "integer"},
@@ -633,14 +635,15 @@
                         "manufacturer_id",
                         # "changelog",
                         "checksum",
                         # "min_hardware_version",
                         # "max_hardware_version",
                         # "min_current_file_version",
                         # "max_current_file_version",
+                        # "release_notes",
                         # "specificity",
                     ],
                 },
             }
         },
         "required": ["firmwares"],
     }
@@ -675,15 +678,17 @@
                 file_size=fw["file_size"],
                 url=fw["binary_url"],
                 min_hardware_version=fw.get("min_hardware_version"),
                 max_hardware_version=fw.get("max_hardware_version"),
                 min_current_file_version=fw.get("min_current_file_version"),
                 max_current_file_version=fw.get("max_current_file_version"),
                 changelog=fw.get("changelog"),
+                release_notes=fw.get("release_notes"),
                 specificity=fw.get("specificity"),
+                source=f"Remote provider ({self.url})",
             )
 
             # To ensure all remote images can be used, extend the list of known
             # manufacturer IDs at runtime if we encounter a new one
             if (
                 self.manufacturer_ids is not None
                 and meta.manufacturer_id not in self.manufacturer_ids
@@ -728,19 +733,17 @@
             yield LocalOtaImageMetadata(  # type: ignore[call-arg]
                 path=path,
                 file_version=image.header.file_version,
                 manufacturer_id=image.header.manufacturer_id,
                 image_type=image.header.image_type,
                 checksum="sha1:" + hasher.hexdigest(),
                 file_size=len(data),
-                manufacturer_names=(),
-                model_names=(),
-                changelog=None,
                 min_hardware_version=image.header.minimum_hardware_version,
                 max_hardware_version=image.header.maximum_hardware_version,
+                source=f"Advanced file provider ({self.image_dir})",
             )
 
 
 def _load_z2m_index(index: dict, *, index_root: pathlib.Path | None = None):
     for obj in index:
         shared_kwargs = {
             "file_version": obj["fileVersion"],
@@ -748,14 +751,15 @@
             "image_type": obj["imageType"],
             "checksum": "sha512:" + obj["sha512"],
             "file_size": obj["fileSize"],
             "manufacturer_names": tuple(obj.get("manufacturerName", [])),
             "model_names": tuple([obj["modelId"]] if "modelId" in obj else []),
             "min_current_file_version": obj.get("minFileVersion"),
             "max_current_file_version": obj.get("maxFileVersion"),
+            "source": "",  # Set in a subclass
         }
 
         if "path" in obj and index_root is not None:
             yield LocalOtaImageMetadata(**shared_kwargs, path=index_root / obj["path"])  # type: ignore[call-arg]
         else:
             yield RemoteOtaImageMetadata(**shared_kwargs, url=obj["url"])  # type: ignore[call-arg]
 
@@ -805,15 +809,15 @@
             None, self.index_file.read_text
         )
         index = json.loads(index_text)
 
         jsonschema.validate(index, self.JSON_SCHEMA)
 
         for img in _load_z2m_index(index, index_root=self.index_file.parent):
-            yield img
+            yield img.replace(source=f"Local Z2M provider ({self.index_file})")
 
 
 class RemoteZ2MProvider(BaseZ2MProvider):
     def __init__(self, url: str):
         super().__init__()
         self.url = url
 
@@ -822,8 +826,8 @@
     ) -> typing.AsyncIterator[BaseOtaImageMetadata]:
         async with session.get(self.url) as rsp:
             fw_lst = await rsp.json(content_type=None)
 
         jsonschema.validate(fw_lst, self.JSON_SCHEMA)
 
         for img in _load_z2m_index(fw_lst):
-            yield img
+            yield img.replace(source=f"Remote Z2M provider ({self.url})")
```

### Comparing `zigpy-0.63.5/zigpy/ota/validators.py` & `zigpy-0.64.0/zigpy/ota/validators.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/profiles/zgp.py` & `zigpy-0.64.0/zigpy/profiles/zgp.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/profiles/zha.py` & `zigpy-0.64.0/zigpy/profiles/zha.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/profiles/zll.py` & `zigpy-0.64.0/zigpy/profiles/zll.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/quirks/__init__.py` & `zigpy-0.64.0/zigpy/quirks/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/quirks/registry.py` & `zigpy-0.64.0/zigpy/quirks/registry.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/quirks/v2/__init__.py` & `zigpy-0.64.0/zigpy/quirks/v2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Quirks v2 module."""
 
 from __future__ import annotations
 
 import collections
 from enum import Enum
+import inspect
 import logging
 import typing
 from typing import TYPE_CHECKING, Any
 
 import attrs
 
 from zigpy.const import (
@@ -101,24 +102,27 @@
                         cluster.cluster_id for cluster in endpoint.out_clusters.values()
                     ],
                 }
                 for key, endpoint in replaces.endpoints.items()
                 if not isinstance(endpoint, ZDO)
             }
         }
-        self.replacement[
-            SIG_SKIP_CONFIG
-        ] = self.quirk_metadata.skip_device_configuration
+        self.replacement[SIG_SKIP_CONFIG] = (
+            self.quirk_metadata.skip_device_configuration
+        )
         if self.quirk_metadata.device_node_descriptor:
             self.replacement[SIG_NODE_DESC] = self.quirk_metadata.device_node_descriptor
 
     @property
     def exposes_metadata(
         self,
-    ) -> dict[tuple[int, int, ClusterType], list[EntityMetadata],]:
+    ) -> dict[
+        tuple[int, int, ClusterType],
+        list[EntityMetadata],
+    ]:
         """Return EntityMetadata for exposed entities.
 
         The key is a tuple of (endpoint_id, cluster_id, cluster_type).
         The value is a list of EntityMetadata instances.
         """
         return self._exposes_metadata
 
@@ -316,14 +320,15 @@
 
 
 @attrs.define
 class QuirksV2RegistryEntry:
     """Quirks V2 registry entry."""
 
     registry: DeviceRegistry = None
+    quirk_location: str = None
     filters: list[FilterType] = attrs.field(factory=list)
     custom_device_class: type[CustomDeviceV2] | None = attrs.field(default=None)
     device_node_descriptor: NodeDescriptor | None = attrs.field(default=None)
     skip_device_configuration: bool = attrs.field(default=False)
     adds_metadata: list[AddsMetadata] = attrs.field(factory=list)
     removes_metadata: list[RemovesMetadata] = attrs.field(factory=list)
     replaces_metadata: list[ReplacesMetadata] = attrs.field(factory=list)
@@ -331,17 +336,17 @@
         ZCLEnumMetadata
         | SwitchMetadata
         | NumberMetadata
         | BinarySensorMetadata
         | WriteAttributeButtonMetadata
         | ZCLCommandButtonMetadata
     ] = attrs.field(factory=list)
-    device_automation_triggers_metadata: dict[
-        tuple[str, str], dict[str, str]
-    ] = attrs.field(factory=dict)
+    device_automation_triggers_metadata: dict[tuple[str, str], dict[str, str]] = (
+        attrs.field(factory=dict)
+    )
 
     def also_applies_to(self, manufacturer: str, model: str) -> QuirksV2RegistryEntry:
         """Register this quirks v2 entry for an additional manufacturer and model."""
         self.registry.add_to_registry_v2(manufacturer, model, self)
         return self
 
     def filter(self, filter_function: FilterType) -> QuirksV2RegistryEntry:
@@ -740,8 +745,13 @@
         return CustomDeviceV2(device.application, device.ieee, device.nwk, device, self)
 
 
 def add_to_registry_v2(
     manufacturer: str, model: str, registry: DeviceRegistry = _DEVICE_REGISTRY
 ) -> QuirksV2RegistryEntry:
     """Add an entry to the registry."""
-    return registry.add_to_registry_v2(manufacturer, model, QuirksV2RegistryEntry())
+    stack: list[inspect.FrameInfo] = inspect.stack()
+    caller: inspect.FrameInfo = stack[1]
+    location: str = f"file[{caller.filename}]-line:{caller.lineno}"
+    quirk_entry = QuirksV2RegistryEntry()
+    quirk_entry.quirk_location = location
+    return registry.add_to_registry_v2(manufacturer, model, quirk_entry)
```

### Comparing `zigpy-0.63.5/zigpy/quirks/v2/homeassistant/__init__.py` & `zigpy-0.64.0/zigpy/quirks/v2/homeassistant/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/quirks/v2/homeassistant/binary_sensor.py` & `zigpy-0.64.0/zigpy/quirks/v2/homeassistant/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/quirks/v2/homeassistant/number.py` & `zigpy-0.64.0/zigpy/quirks/v2/homeassistant/number.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/quirks/v2/homeassistant/sensor.py` & `zigpy-0.64.0/zigpy/quirks/v2/homeassistant/sensor.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/serial.py` & `zigpy-0.64.0/zigpy/serial.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/state.py` & `zigpy-0.64.0/zigpy/state.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/topology.py` & `zigpy-0.64.0/zigpy/topology.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/types/basic.py` & `zigpy-0.64.0/zigpy/types/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 class SerializableBytes:
     """A container object for raw bytes that enforces `serialize()` will be called."""
 
     def __init__(self, value: bytes = b"") -> None:
         if isinstance(value, type(self)):
-            value = value.value
+            value = value.value  # type: ignore
         elif not isinstance(value, (bytes, bytearray)):
             raise ValueError(f"Object is not bytes: {value!r}")  # noqa: TRY004
 
         self.value = value
 
     def __eq__(self, other: typing.Any) -> bool:
         if not isinstance(other, type(self)):
@@ -456,15 +456,15 @@
             pass
 
     else:
 
         class _NewEnum(int_type, enum.Flag):
             # Rebind classmethods to our own class
             _missing_ = classmethod(enum.IntFlag._missing_.__func__)
-            _create_pseudo_member_ = classmethod(
+            _create_pseudo_member_ = classmethod(  # type: ignore
                 enum.IntFlag._create_pseudo_member_.__func__
             )
 
             __or__ = enum.IntFlag.__or__
             __and__ = enum.IntFlag.__and__
             __xor__ = enum.IntFlag.__xor__
             __ror__ = enum.IntFlag.__ror__
```

### Comparing `zigpy-0.63.5/zigpy/types/named.py` & `zigpy-0.64.0/zigpy/types/named.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 if typing.TYPE_CHECKING:
     from typing_extensions import Self
 
 
 class BaseDataclassMixin:
     def replace(self, **kwargs) -> Self:
         if dataclasses.is_dataclass(self):
-            return dataclasses.replace(self, **kwargs)
+            return dataclasses.replace(self, **kwargs)  # type: ignore
         else:
             return attrs.evolve(self, **kwargs)
 
 
 def _hex_string_to_bytes(hex_string: str) -> bytes:
     """Parses a hex string with optional colon delimiters and whitespace into bytes."""
```

### Comparing `zigpy-0.63.5/zigpy/types/struct.py` & `zigpy-0.64.0/zigpy/types/struct.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/typing.py` & `zigpy-0.64.0/zigpy/typing.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/util.py` & `zigpy-0.64.0/zigpy/util.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/zcl/__init__.py` & `zigpy-0.64.0/zigpy/zcl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -787,14 +787,19 @@
             *args,
             manufacturer=manufacturer,
             tsn=tsn,
             **kwargs,
         )
 
     @property
+    def cluster_type(self) -> ClusterType:
+        """Return the type of this cluster."""
+        return self._type
+
+    @property
     def is_client(self) -> bool:
         """Return True if this is a client cluster."""
         return self._type == ClusterType.Client
 
     @property
     def is_server(self) -> bool:
         """Return True if this is a server cluster."""
```

### Comparing `zigpy-0.63.5/zigpy/zcl/clusters/__init__.py` & `zigpy-0.64.0/zigpy/zcl/clusters/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/zcl/clusters/closures.py` & `zigpy-0.64.0/zigpy/zcl/clusters/closures.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 class Shade(Cluster):
     """Attributes and commands for configuring a shade"""
 
     ShadeStatus: Final = ShadeStatus
     ShadeMode: Final = ShadeMode
 
-    cluster_id: Final = 0x0100
+    cluster_id: Final[t.uint16_t] = 0x0100
     name: Final = "Shade Configuration"
     ep_attribute: Final = "shade"
 
     class AttributeDefs(BaseAttributeDefs):
         # Shade Information
         physical_closed_limit: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint16_t, access="r"
@@ -284,15 +284,15 @@
     OperationEvent: Final = OperationEvent
     ProgrammingEvent: Final = ProgrammingEvent
     UserStatus: Final = UserStatus
     UserType: Final = UserType
     DayMask: Final = DayMask
     EventType: Final = EventType
 
-    cluster_id: Final = 0x0101
+    cluster_id: Final[t.uint16_t] = 0x0101
     name: Final = "Door Lock"
     ep_attribute: Final = "door_lock"
 
     class AttributeDefs(BaseAttributeDefs):
         lock_state: Final = ZCLAttributeDef(
             id=0x0000, type=LockState, access="rp", mandatory=True
         )
@@ -726,15 +726,15 @@
 
 
 class WindowCovering(Cluster):
     WindowCoveringType: Final = WindowCoveringType
     ConfigStatus: Final = ConfigStatus
     WindowCoveringMode: Final = WindowCoveringMode
 
-    cluster_id: Final = 0x0102
+    cluster_id: Final[t.uint16_t] = 0x0102
     name: Final = "Window Covering"
     ep_attribute: Final = "window_covering"
 
     class AttributeDefs(BaseAttributeDefs):
         # Window Covering Information
         window_covering_type: Final = ZCLAttributeDef(
             id=0x0000, type=WindowCoveringType, access="r", mandatory=True
```

### Comparing `zigpy-0.63.5/zigpy/zcl/clusters/general.py` & `zigpy-0.64.0/zigpy/zcl/clusters/general.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,15 +210,15 @@
     PowerSource: Final = PowerSource
     PhysicalEnvironment: Final = PhysicalEnvironment
     AlarmMask: Final = AlarmMask
     DisableLocalConfig: Final = DisableLocalConfig
     GenericDeviceClass: Final = GenericDeviceClass
     GenericLightingDeviceType: Final = GenericLightingDeviceType
 
-    cluster_id: Final = 0x0000
+    cluster_id: Final[t.uint16_t] = 0x0000
     ep_attribute: Final = "basic"
 
     class AttributeDefs(BaseAttributeDefs):
         # Basic Device Information
         zcl_version: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint8_t, access="r", mandatory=True
         )
@@ -303,15 +303,15 @@
     about a device’s power source(s), and for configuring
     under/over voltage alarms.
     """
 
     MainsAlarmMask: Final = MainsAlarmMask
     BatterySize: Final = BatterySize
 
-    cluster_id: Final = 0x0001
+    cluster_id: Final[t.uint16_t] = 0x0001
     name: Final = "Power Configuration"
     ep_attribute: Final = "power"
 
     class AttributeDefs(BaseAttributeDefs):
         # Mains Information
         mains_voltage: Final = ZCLAttributeDef(id=0x0000, type=t.uint16_t, access="r")
         mains_frequency: Final = ZCLAttributeDef(id=0x0001, type=t.uint8_t, access="r")
@@ -498,15 +498,15 @@
     """Attributes for determining information about a device’s
     internal temperature, and for configuring under/over
     temperature alarms.
     """
 
     DeviceTempAlarmMask: Final = DeviceTempAlarmMask
 
-    cluster_id: Final = 0x0002
+    cluster_id: Final[t.uint16_t] = 0x0002
     name: Final = "Device Temperature"
     ep_attribute: Final = "device_temperature"
 
     class AttributeDefs(BaseAttributeDefs):
         # Device Temperature Information
         current_temperature: Final = ZCLAttributeDef(
             id=0x0000, type=t.int16s, access="r", mandatory=True
@@ -553,15 +553,15 @@
     """Attributes and commands for putting a device into
     Identification mode (e.g. flashing a light)
     """
 
     EffectIdentifier: Final = EffectIdentifier
     EffectVariant: Final = EffectVariant
 
-    cluster_id: Final = 0x0003
+    cluster_id: Final[t.uint16_t] = 0x0003
     ep_attribute: Final = "identify"
 
     class AttributeDefs(BaseAttributeDefs):
         identify_time: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint16_t, access="rw", mandatory=True
         )
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
@@ -593,15 +593,15 @@
 class Groups(Cluster):
     """Attributes and commands for group configuration and
     manipulation.
     """
 
     NameSupport: Final = NameSupport
 
-    cluster_id: Final = 0x0004
+    cluster_id: Final[t.uint16_t] = 0x0004
     ep_attribute: Final = "groups"
 
     class AttributeDefs(BaseAttributeDefs):
         name_support: Final = ZCLAttributeDef(
             id=0x0000, type=NameSupport, access="r", mandatory=True
         )
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
@@ -659,15 +659,15 @@
 class Scenes(Cluster):
     """Attributes and commands for scene configuration and
     manipulation.
     """
 
     NameSupport: Final = NameSupport
 
-    cluster_id: Final = 0x0005
+    cluster_id: Final[t.uint16_t] = 0x0005
     ep_attribute: Final = "scenes"
 
     class AttributeDefs(BaseAttributeDefs):
         # Scene Management Information
         count: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint8_t, access="r", mandatory=True
         )
@@ -870,15 +870,15 @@
 
     DELAYED_ALL_OFF_FADE_TO_OFF = 0x00
     DELAYED_ALL_OFF_NO_FADE = 0x01
     DELAYED_ALL_OFF_DIM_THEN_FADE_TO_OFF = 0x02
 
     DYING_LIGHT_DIM_UP_THEN_FADE_TO_OFF = 0x00
 
-    cluster_id: Final = 0x0006
+    cluster_id: Final[t.uint16_t] = 0x0006
     name: Final = "On/Off"
     ep_attribute: Final = "on_off"
 
     class AttributeDefs(BaseAttributeDefs):
         on_off: Final = ZCLAttributeDef(
             id=0x0000, type=t.Bool, access="rps", mandatory=True
         )
@@ -930,15 +930,15 @@
 
 class OnOffConfiguration(Cluster):
     """Attributes and commands for configuring On/Off switching devices"""
 
     SwitchType: Final = SwitchType
     SwitchActions: Final = SwitchActions
 
-    cluster_id: Final = 0x0007
+    cluster_id: Final[t.uint16_t] = 0x0007
     name: Final = "On/Off Switch Configuration"
     ep_attribute: Final = "on_off_config"
 
     class AttributeDefs(BaseAttributeDefs):
         switch_type: Final = ZCLAttributeDef(
             id=0x0000, type=SwitchType, access="r", mandatory=True
         )
@@ -969,15 +969,15 @@
     can be set to a level between fully ‘On’ and fully ‘Off’.
     """
 
     MoveMode: Final = MoveMode
     StepMode: Final = StepMode
     Options: Final = Options
 
-    cluster_id: Final = 0x0008
+    cluster_id: Final[t.uint16_t] = 0x0008
     name: Final = "Level control"
     ep_attribute: Final = "level"
 
     class AttributeDefs(BaseAttributeDefs):
         current_level: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint8_t, access="rps", mandatory=True
         )
@@ -1075,15 +1075,15 @@
 
 
 class Alarms(Cluster):
     """Attributes and commands for sending notifications and
     configuring alarm functionality.
     """
 
-    cluster_id: Final = 0x0009
+    cluster_id: Final[t.uint16_t] = 0x0009
     ep_attribute: Final = "alarms"
 
     class AttributeDefs(BaseAttributeDefs):
         alarm_count: Final = ZCLAttributeDef(id=0x0000, type=t.uint16_t, access="r")
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
@@ -1127,15 +1127,15 @@
 class Time(Cluster):
     """Attributes and commands that provide a basic interface
     to a real-time clock.
     """
 
     TimeStatus: Final = TimeStatus
 
-    cluster_id: Final = 0x000A
+    cluster_id: Final[t.uint16_t] = 0x000A
     ep_attribute: Final = "time"
 
     class AttributeDefs(BaseAttributeDefs):
         time: Final = ZCLAttributeDef(
             id=0x0000, type=t.UTCTime, access="r*w", mandatory=True
         )
         time_status: Final = ZCLAttributeDef(
@@ -1207,15 +1207,15 @@
     exchanging location information and channel parameters
     among devices.
     """
 
     LocationMethod: Final = LocationMethod
     NeighborInfo: Final = NeighborInfo
 
-    cluster_id: Final = 0x000B
+    cluster_id: Final[t.uint16_t] = 0x000B
     ep_attribute: Final = "rssi_location"
 
     class AttributeDefs(BaseAttributeDefs):
         # Location Information
         type: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint8_t, access="rw", mandatory=True
         )
@@ -1383,15 +1383,15 @@
     Multi_state_fault = 9
     Configuration_error = 10
 
 
 class AnalogInput(Cluster):
     Reliability: Final = Reliability
 
-    cluster_id: Final = 0x000C
+    cluster_id: Final[t.uint16_t] = 0x000C
     ep_attribute: Final = "analog_input"
 
     class AttributeDefs(BaseAttributeDefs):
         description: Final = ZCLAttributeDef(
             id=0x001C, type=t.CharacterString, access="r*w"
         )
         max_present_value: Final = ZCLAttributeDef(
@@ -1418,15 +1418,15 @@
             id=0x0100, type=t.uint32_t, access="r"
         )
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class AnalogOutput(Cluster):
-    cluster_id: Final = 0x000D
+    cluster_id: Final[t.uint16_t] = 0x000D
     ep_attribute: Final = "analog_output"
 
     class AttributeDefs(BaseAttributeDefs):
         description: Final = ZCLAttributeDef(
             id=0x001C, type=t.CharacterString, access="r*w"
         )
         max_present_value: Final = ZCLAttributeDef(
@@ -1458,15 +1458,15 @@
             id=0x0100, type=t.uint32_t, access="r"
         )
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class AnalogValue(Cluster):
-    cluster_id: Final = 0x000E
+    cluster_id: Final[t.uint16_t] = 0x000E
     ep_attribute: Final = "analog_value"
 
     class AttributeDefs(BaseAttributeDefs):
         description: Final = ZCLAttributeDef(
             id=0x001C, type=t.CharacterString, access="r*w"
         )
         out_of_service: Final = ZCLAttributeDef(
@@ -1491,15 +1491,15 @@
             id=0x0100, type=t.uint32_t, access="r"
         )
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class BinaryInput(Cluster):
-    cluster_id: Final = 0x000F
+    cluster_id: Final[t.uint16_t] = 0x000F
     name: Final = "Binary Input (Basic)"
     ep_attribute: Final = "binary_input"
 
     class AttributeDefs(BaseAttributeDefs):
         active_text: Final = ZCLAttributeDef(
             id=0x0004, type=t.CharacterString, access="r*w"
         )
@@ -1524,15 +1524,15 @@
             id=0x0100, type=t.uint32_t, access="r"
         )
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class BinaryOutput(Cluster):
-    cluster_id: Final = 0x0010
+    cluster_id: Final[t.uint16_t] = 0x0010
     ep_attribute: Final = "binary_output"
 
     class AttributeDefs(BaseAttributeDefs):
         active_text: Final = ZCLAttributeDef(
             id=0x0004, type=t.CharacterString, access="r*w"
         )
         description: Final = ZCLAttributeDef(
@@ -1573,15 +1573,15 @@
             id=0x0100, type=t.uint32_t, access="r"
         )
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class BinaryValue(Cluster):
-    cluster_id: Final = 0x0011
+    cluster_id: Final[t.uint16_t] = 0x0011
     ep_attribute: Final = "binary_value"
 
     class AttributeDefs(BaseAttributeDefs):
         active_text: Final = ZCLAttributeDef(
             id=0x0004, type=t.CharacterString, access="r*w"
         )
         description: Final = ZCLAttributeDef(
@@ -1615,15 +1615,15 @@
             id=0x0100, type=t.uint32_t, access="r"
         )
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class MultistateInput(Cluster):
-    cluster_id: Final = 0x0012
+    cluster_id: Final[t.uint16_t] = 0x0012
     ep_attribute: Final = "multistate_input"
 
     class AttributeDefs(BaseAttributeDefs):
         state_text: Final = ZCLAttributeDef(
             id=0x000E, type=t.List[t.CharacterString], access="r*w"
         )
         description: Final = ZCLAttributeDef(
@@ -1648,15 +1648,15 @@
             id=0x0100, type=t.uint32_t, access="r"
         )
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class MultistateOutput(Cluster):
-    cluster_id: Final = 0x0013
+    cluster_id: Final[t.uint16_t] = 0x0013
     ep_attribute: Final = "multistate_output"
 
     class AttributeDefs(BaseAttributeDefs):
         state_text: Final = ZCLAttributeDef(
             id=0x000E, type=t.List[t.CharacterString], access="r*w"
         )
         description: Final = ZCLAttributeDef(
@@ -1684,15 +1684,15 @@
             id=0x0100, type=t.uint32_t, access="r"
         )
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class MultistateValue(Cluster):
-    cluster_id: Final = 0x0014
+    cluster_id: Final[t.uint16_t] = 0x0014
     ep_attribute: Final = "multistate_value"
 
     class AttributeDefs(BaseAttributeDefs):
         state_text: Final = ZCLAttributeDef(
             id=0x000E, type=t.List[t.CharacterString], access="r*w"
         )
         description: Final = ZCLAttributeDef(
@@ -1738,15 +1738,15 @@
     """Attributes and commands for commissioning and
     managing a ZigBee device.
     """
 
     StartupControl: Final = StartupControl
     NetworkKeyType: Final = NetworkKeyType
 
-    cluster_id: Final = 0x0015
+    cluster_id: Final[t.uint16_t] = 0x0015
     ep_attribute: Final = "commissioning"
 
     class AttributeDefs(BaseAttributeDefs):
         # Startup Parameters
         short_address: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint16_t, access="rw", mandatory=True
         )
@@ -1855,15 +1855,15 @@
         )
         reset_startup_params_response: Final = ZCLCommandDef(
             id=0x03, schema={"status": foundation.Status}, direction=True
         )
 
 
 class Partition(Cluster):
-    cluster_id: Final = 0x0016
+    cluster_id: Final[t.uint16_t] = 0x0016
     ep_attribute: Final = "partition"
 
     class AttributeDefs(BaseAttributeDefs):
         maximum_incoming_transfer_size: Final = ZCLAttributeDef(
             id=0x0000,
             type=t.uint16_t,
             access="r",
@@ -2039,15 +2039,15 @@
     UpgradeTimeoutPolicy: Final = UpgradeTimeoutPolicy
     ImageNotifyCommand: Final = ImageNotifyCommand
     QueryNextImageCommand: Final = QueryNextImageCommand
     ImageBlockCommand: Final = ImageBlockCommand
     ImagePageCommand: Final = ImagePageCommand
     ImageBlockResponseCommand: Final = ImageBlockResponseCommand
 
-    cluster_id: Final = 0x0019
+    cluster_id: Final[t.uint16_t] = 0x0019
     ep_attribute: Final = "ota"
 
     class AttributeDefs(BaseAttributeDefs):
         upgrade_server_id: Final = ZCLAttributeDef(
             id=0x0000, type=t.EUI64, access="r", mandatory=True
         )
         file_offset: Final = ZCLAttributeDef(id=0x0001, type=t.uint32_t, access="r")
@@ -2230,15 +2230,15 @@
 
 
 class PowerProfile(Cluster):
     ScheduleRecord: Final = ScheduleRecord
     PowerProfilePhase: Final = PowerProfilePhase
     PowerProfile: Final = PowerProfileType
 
-    cluster_id: Final = 0x001A
+    cluster_id: Final[t.uint16_t] = 0x001A
     ep_attribute: Final = "power_profile"
 
     class AttributeDefs(BaseAttributeDefs):
         total_profile_num: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint8_t, access="r", mandatory=True
         )
         multiple_scheduling: Final = ZCLAttributeDef(
@@ -2401,15 +2401,15 @@
                 "power_profile_start_time?": t.uint16_t,
             },
             direction=False,
         )
 
 
 class ApplianceControl(Cluster):
-    cluster_id: Final = 0x001B
+    cluster_id: Final[t.uint16_t] = 0x001B
     ep_attribute: Final = "appliance_control"
 
     class AttributeDefs(BaseAttributeDefs):
         start_time: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint16_t, access="rp", mandatory=True
         )
         finish_time: Final = ZCLAttributeDef(
@@ -2417,15 +2417,15 @@
         )
         remaining_time: Final = ZCLAttributeDef(id=0x0002, type=t.uint16_t, access="rp")
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class PollControl(Cluster):
-    cluster_id: Final = 0x0020
+    cluster_id: Final[t.uint16_t] = 0x0020
     name: Final = "Poll Control"
     ep_attribute: Final = "poll_control"
 
     class AttributeDefs(BaseAttributeDefs):
         checkin_interval: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint32_t, access="rw", mandatory=True
         )
@@ -2467,22 +2467,22 @@
         )
 
     class ClientCommandDefs(BaseCommandDefs):
         checkin: Final = ZCLCommandDef(id=0x0000, schema={}, direction=False)
 
 
 class GreenPowerProxy(Cluster):
-    cluster_id: Final = 0x0021
+    cluster_id: Final[t.uint16_t] = 0x0021
     ep_attribute: Final = "green_power"
 
 
 class KeepAlive(Cluster):
     """Keep Alive cluster definition."""
 
-    cluster_id: Final = 0x0025
+    cluster_id: Final[t.uint16_t] = 0x0025
     ep_attribute: Final = "keep_alive"
 
     class AttributeDefs(BaseAttributeDefs):
         """Keep Alive cluster attributes."""
 
         tc_keep_alive_base: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint8_t, access="r", mandatory=True
```

### Comparing `zigpy-0.63.5/zigpy/zcl/clusters/homeautomation.py` & `zigpy-0.64.0/zigpy/zcl/clusters/homeautomation.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     BaseCommandDefs,
     ZCLAttributeDef,
     ZCLCommandDef,
 )
 
 
 class ApplianceIdentification(Cluster):
-    cluster_id: Final = 0x0B00
+    cluster_id: Final[t.uint16_t] = 0x0B00
     name: Final = "Appliance Identification"
     ep_attribute: Final = "appliance_id"
 
     class AttributeDefs(BaseAttributeDefs):
         basic_identification: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint56_t, access="r", mandatory=True
         )
@@ -47,15 +47,15 @@
             id=0x001A, type=t.uint8_t, access="r"
         )
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class MeterIdentification(Cluster):
-    cluster_id: Final = 0x0B01
+    cluster_id: Final[t.uint16_t] = 0x0B01
     name: Final = "Meter Identification"
     ep_attribute: Final = "meter_id"
 
     class AttributeDefs(BaseAttributeDefs):
         company_name: Final = ZCLAttributeDef(
             id=0x0000, type=t.LimitedCharString(16), access="r", mandatory=True
         )
@@ -91,15 +91,15 @@
             id=0x000E, type=t.int24s, access="r", mandatory=True
         )
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class ApplianceEventAlerts(Cluster):
-    cluster_id: Final = 0x0B02
+    cluster_id: Final[t.uint16_t] = 0x0B02
     name: Final = "Appliance Event Alerts"
     ep_attribute: Final = "appliance_event"
 
     class AttributeDefs(BaseAttributeDefs):
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
@@ -109,15 +109,15 @@
     class ClientCommandDefs(BaseCommandDefs):
         get_alerts_response: Final = ZCLCommandDef(id=0x00, schema={}, direction=True)
         alerts_notification: Final = ZCLCommandDef(id=0x01, schema={}, direction=False)
         event_notification: Final = ZCLCommandDef(id=0x02, schema={}, direction=False)
 
 
 class ApplianceStatistics(Cluster):
-    cluster_id: Final = 0x0B03
+    cluster_id: Final[t.uint16_t] = 0x0B03
     name: Final = "Appliance Statistics"
     ep_attribute: Final = "appliance_stats"
 
     class AttributeDefs(BaseAttributeDefs):
         log_max_size: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint32_t, access="r", mandatory=True
         )
@@ -165,15 +165,15 @@
     RMS_Extreme_Over_Voltage = 2 << 6
     RMS_Extreme_Under_Voltage = 2 << 7
     RMS_Voltage_Sag = 2 << 8
     RMS_Voltage_Swell = 2 << 9
 
 
 class ElectricalMeasurement(Cluster):
-    cluster_id: Final = 0x0B04
+    cluster_id: Final[t.uint16_t] = 0x0B04
     name: Final = "Electrical Measurement"
     ep_attribute: Final = "electrical_measurement"
 
     MeasurementType: Final = MeasurementType
     DCOverloadAlarmMark: Final = DCOverloadAlarmMark
     ACAlarmsMask: Final = ACAlarmsMask
 
@@ -539,15 +539,15 @@
         )
         get_measurement_profile_response: Final = ZCLCommandDef(
             id=0x01, schema={}, direction=True
         )
 
 
 class Diagnostic(Cluster):
-    cluster_id: Final = 0x0B05
+    cluster_id: Final[t.uint16_t] = 0x0B05
     ep_attribute: Final = "diagnostic"
 
     class AttributeDefs(BaseAttributeDefs):
         # Hardware Information
         number_of_resets: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint16_t, access="r"
         )
```

### Comparing `zigpy-0.63.5/zigpy/zcl/clusters/hvac.py` & `zigpy-0.64.0/zigpy/zcl/clusters/hvac.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     """An interface for configuring and controlling pumps."""
 
     AlarmMask: Final = PumpAlarmMask
     ControlMode: Final = ControlMode
     OperationMode: Final = OperationMode
     PumpStatus: Final = PumpStatus
 
-    cluster_id: Final = 0x0200
+    cluster_id: Final[t.uint16_t] = 0x0200
     name: Final = "Pump Configuration and Control"
     ep_attribute: Final = "pump"
 
     class AttributeDefs(BaseAttributeDefs):
         # Pump Information
         max_pressure: Final = ZCLAttributeDef(
             id=0x0000, type=t.int16s, access="r", mandatory=True
@@ -343,15 +343,15 @@
     StartOfWeek: Final = StartOfWeek
     SystemMode: Final = SystemMode
     SystemType: Final = SystemType
     TemperatureSetpointHold: Final = TemperatureSetpointHold
     RunningMode: Final = RunningMode
     RunningState: Final = RunningState
 
-    cluster_id: Final = 0x0201
+    cluster_id: Final[t.uint16_t] = 0x0201
     ep_attribute: Final = "thermostat"
 
     class AttributeDefs(BaseAttributeDefs):
         # Thermostat Information
         local_temperature: Final = ZCLAttributeDef(
             id=0x0000, type=t.int16s, access="rp", mandatory=True
         )
@@ -567,15 +567,15 @@
     """An interface for controlling a fan in a heating /
     cooling system.
     """
 
     FanMode: Final = FanMode
     FanModeSequence: Final = FanModeSequence
 
-    cluster_id: Final = 0x0202
+    cluster_id: Final[t.uint16_t] = 0x0202
     name: Final = "Fan Control"
     ep_attribute: Final = "fan"
 
     class AttributeDefs(BaseAttributeDefs):
         fan_mode: Final = ZCLAttributeDef(id=0x0000, type=FanMode, access="")
         fan_mode_sequence: Final = ZCLAttributeDef(
             id=0x0001, type=FanModeSequence, access=""
@@ -600,15 +600,15 @@
 class Dehumidification(Cluster):
     """An interface for controlling dehumidification."""
 
     RelativeHumidityMode: Final = RelativeHumidityMode
     DehumidificationLockout: Final = DehumidificationLockout
     RelativeHumidityDisplay: Final = RelativeHumidityDisplay
 
-    cluster_id: Final = 0x0203
+    cluster_id: Final[t.uint16_t] = 0x0203
     ep_attribute: Final = "dehumidification"
 
     class AttributeDefs(BaseAttributeDefs):
         # Dehumidification Information
         relative_humidity: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint8_t, access="r"
         )
@@ -661,15 +661,15 @@
     thermostat).
     """
 
     TemperatureDisplayMode: Final = TemperatureDisplayMode
     KeypadLockout: Final = KeypadLockout
     ScheduleProgrammingVisibility: Final = ScheduleProgrammingVisibility
 
-    cluster_id: Final = 0x0204
+    cluster_id: Final[t.uint16_t] = 0x0204
     name: Final = "Thermostat User Interface Configuration"
     ep_attribute: Final = "thermostat_ui"
 
     class AttributeDefs(BaseAttributeDefs):
         temperature_display_mode: Final = ZCLAttributeDef(
             id=0x0000,
             type=TemperatureDisplayMode,
```

### Comparing `zigpy-0.63.5/zigpy/zcl/clusters/lighting.py` & `zigpy-0.64.0/zigpy/zcl/clusters/lighting.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     StepMode: Final = StepMode
     ColorLoopUpdateFlags: Final = ColorLoopUpdateFlags
     ColorLoopAction: Final = ColorLoopAction
     ColorLoopDirection: Final = ColorLoopDirection
     DriftCompensation: Final = DriftCompensation
     Options: Final = Options
 
-    cluster_id: Final = 0x0300
+    cluster_id: Final[t.uint16_t] = 0x0300
     name: Final = "Color Control"
     ep_attribute: Final = "light_color"
 
     class AttributeDefs(BaseAttributeDefs):
         current_hue: Final = ZCLAttributeDef(id=0x0000, type=t.uint8_t, access="rp")
         current_saturation: Final = ZCLAttributeDef(
             id=0x0001, type=t.uint8_t, access="rps"
@@ -439,15 +439,15 @@
     """Attributes and commands for configuring a lighting
     ballast
     """
 
     BallastStatus: Final = BallastStatus
     LampAlarmMode: Final = LampAlarmMode
 
-    cluster_id: Final = 0x0301
+    cluster_id: Final[t.uint16_t] = 0x0301
     ep_attribute: Final = "light_ballast"
 
     class AttributeDefs(BaseAttributeDefs):
         physical_min_level: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint8_t, access="r", mandatory=True
         )
         physical_max_level: Final = ZCLAttributeDef(
```

### Comparing `zigpy-0.63.5/zigpy/zcl/clusters/lightlink.py` & `zigpy-0.64.0/zigpy/zcl/clusters/lightlink.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     endpoint_id: t.uint8_t
     profile_id: t.uint16_t
     device_id: t.uint16_t
     version: t.uint8_t
 
 
 class LightLink(Cluster):
-    cluster_id: Final = 0x1000
+    cluster_id: Final[t.uint16_t] = 0x1000
     ep_attribute: Final = "lightlink"
 
     class ServerCommandDefs(BaseCommandDefs):
         scan: Final = ZCLCommandDef(
             id=0x00,
             schema={
                 "inter_pan_transaction_id": t.uint32_t,
```

### Comparing `zigpy-0.63.5/zigpy/zcl/clusters/measurement.py` & `zigpy-0.64.0/zigpy/zcl/clusters/measurement.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     CMOS = 0x01
     Unknown = 0xFF
 
 
 class IlluminanceMeasurement(Cluster):
     LightSensorType: Final = LightSensorType
 
-    cluster_id: Final = 0x0400
+    cluster_id: Final[t.uint16_t] = 0x0400
     name: Final = "Illuminance Measurement"
     ep_attribute: Final = "illuminance"
 
     class AttributeDefs(BaseAttributeDefs):
         measured_value: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint16_t, access="rp", mandatory=True
         )
@@ -46,15 +46,15 @@
     Illuminance_Above_Target = 0x02
 
 
 class IlluminanceLevelSensing(Cluster):
     LevelStatus: Final = LevelStatus
     LightSensorType: Final = LightSensorType
 
-    cluster_id: Final = 0x0401
+    cluster_id: Final[t.uint16_t] = 0x0401
     name: Final = "Illuminance Level Sensing"
     ep_attribute: Final = "illuminance_level"
 
     class AttributeDefs(BaseAttributeDefs):
         level_status: Final = ZCLAttributeDef(
             id=0x0000, type=LevelStatus, access="r", mandatory=True
         )
@@ -66,15 +66,15 @@
             id=0x0010, type=t.uint16_t, access="rw", mandatory=True
         )
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class TemperatureMeasurement(Cluster):
-    cluster_id: Final = 0x0402
+    cluster_id: Final[t.uint16_t] = 0x0402
     name: Final = "Temperature Measurement"
     ep_attribute: Final = "temperature"
 
     class AttributeDefs(BaseAttributeDefs):
         # Temperature Measurement Information
         measured_value: Final = ZCLAttributeDef(
             id=0x0000, type=t.int16s, access="rp", mandatory=True
@@ -89,15 +89,15 @@
         # 0x0010: ('min_percent_change', UNKNOWN),
         # 0x0011: ('min_absolute_change', UNKNOWN),
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class PressureMeasurement(Cluster):
-    cluster_id: Final = 0x0403
+    cluster_id: Final[t.uint16_t] = 0x0403
     name: Final = "Pressure Measurement"
     ep_attribute: Final = "pressure"
 
     class AttributeDefs(BaseAttributeDefs):
         # Pressure Measurement Information
         measured_value: Final = ZCLAttributeDef(
             id=0x0000, type=t.int16s, access="rp", mandatory=True
@@ -118,15 +118,15 @@
         )
         scale: Final = ZCLAttributeDef(id=0x0014, type=t.int8s, access="r")
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class FlowMeasurement(Cluster):
-    cluster_id: Final = 0x0404
+    cluster_id: Final[t.uint16_t] = 0x0404
     name: Final = "Flow Measurement"
     ep_attribute: Final = "flow"
 
     class AttributeDefs(BaseAttributeDefs):
         measured_value: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint16_t, access="rp", mandatory=True
         )
@@ -138,15 +138,15 @@
         )
         tolerance: Final = ZCLAttributeDef(id=0x0003, type=t.uint16_t, access="r")
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class RelativeHumidity(Cluster):
-    cluster_id: Final = 0x0405
+    cluster_id: Final[t.uint16_t] = 0x0405
     name: Final = "Relative Humidity Measurement"
     ep_attribute: Final = "humidity"
 
     class AttributeDefs(BaseAttributeDefs):
         measured_value: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint16_t, access="rp", mandatory=True
         )
@@ -180,15 +180,15 @@
 
 
 class OccupancySensing(Cluster):
     Occupancy: Final = Occupancy
     OccupancySensorType: Final = OccupancySensorType
     OccupancySensorTypeBitmap: Final = OccupancySensorTypeBitmap
 
-    cluster_id: Final = 0x0406
+    cluster_id: Final[t.uint16_t] = 0x0406
     name: Final = "Occupancy Sensing"
     ep_attribute: Final = "occupancy"
 
     class AttributeDefs(BaseAttributeDefs):
         # Occupancy Sensor Information
         occupancy: Final = ZCLAttributeDef(
             id=0x0000, type=Occupancy, access="rp", mandatory=True
@@ -227,15 +227,15 @@
             id=0x0032, type=t.uint8_t, access="rw"
         )
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class LeafWetness(Cluster):
-    cluster_id: Final = 0x0407
+    cluster_id: Final[t.uint16_t] = 0x0407
     name: Final = "Leaf Wetness Measurement"
     ep_attribute: Final = "leaf_wetness"
 
     class AttributeDefs(BaseAttributeDefs):
         # Leaf Wetness Measurement Information
         measured_value: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint16_t, access="rp", mandatory=True
@@ -248,15 +248,15 @@
         )
         tolerance: Final = ZCLAttributeDef(id=0x0003, type=t.uint16_t, access="r")
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class SoilMoisture(Cluster):
-    cluster_id: Final = 0x0408
+    cluster_id: Final[t.uint16_t] = 0x0408
     name: Final = "Soil Moisture Measurement"
     ep_attribute: Final = "soil_moisture"
 
     class AttributeDefs(BaseAttributeDefs):
         # Soil Moisture Measurement Information
         measured_value: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint16_t, access="rp", mandatory=True
@@ -269,15 +269,15 @@
         )
         tolerance: Final = ZCLAttributeDef(id=0x0003, type=t.uint16_t, access="r")
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class PH(Cluster):
-    cluster_id: Final = 0x0409
+    cluster_id: Final[t.uint16_t] = 0x0409
     name: Final = "pH Measurement"
     ep_attribute: Final = "ph"
 
     class AttributeDefs(BaseAttributeDefs):
         # pH Measurement Information
         measured_value: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint16_t, access="rp", mandatory=True
@@ -290,15 +290,15 @@
         )
         tolerance: Final = ZCLAttributeDef(id=0x0003, type=t.uint16_t, access="r")
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class ElectricalConductivity(Cluster):
-    cluster_id: Final = 0x040A
+    cluster_id: Final[t.uint16_t] = 0x040A
     name: Final = "Electrical Conductivity"
     ep_attribute: Final = "electrical_conductivity"
 
     class AttributeDefs(BaseAttributeDefs):
         measured_value: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint16_t, access="rp", mandatory=True
         )
@@ -310,15 +310,15 @@
         )
         tolerance: Final = ZCLAttributeDef(id=0x0003, type=t.uint16_t, access="r")
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class WindSpeed(Cluster):
-    cluster_id: Final = 0x040B
+    cluster_id: Final[t.uint16_t] = 0x040B
     name: Final = "Wind Speed Measurement"
     ep_attribute: Final = "wind_speed"
 
     class AttributeDefs(BaseAttributeDefs):
         # Wind Speed Measurement Information
         measured_value: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint16_t, access="rp", mandatory=True
@@ -349,204 +349,206 @@
         )
         tolerance: Final = ZCLAttributeDef(id=0x0003, type=t.Single, access="r")
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
 
 class CarbonMonoxideConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x040C
+    cluster_id: Final[t.uint16_t] = 0x040C
     name: Final = "Carbon Monoxide (CO) Concentration"
     ep_attribute: Final = "carbon_monoxide_concentration"
 
 
 class CarbonDioxideConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x040D
+    cluster_id: Final[t.uint16_t] = 0x040D
     name: Final = "Carbon Dioxide (CO₂) Concentration"
     ep_attribute: Final = "carbon_dioxide_concentration"
 
 
 class EthyleneConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x040E
+    cluster_id: Final[t.uint16_t] = 0x040E
     name: Final = "Ethylene (CH₂) Concentration"
     ep_attribute: Final = "ethylene_concentration"
 
 
 class EthyleneOxideConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x040F
+    cluster_id: Final[t.uint16_t] = 0x040F
     name: Final = "Ethylene Oxide (C₂H₄O) Concentration"
     ep_attribute: Final = "ethylene_oxide_concentration"
 
 
 class HydrogenConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x0410
+    cluster_id: Final[t.uint16_t] = 0x0410
     name: Final = "Hydrogen (H) Concentration"
     ep_attribute: Final = "hydrogen_concentration"
 
 
 class HydrogenSulfideConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x0411
+    cluster_id: Final[t.uint16_t] = 0x0411
     name: Final = "Hydrogen Sulfide (H₂S) Concentration"
     ep_attribute: Final = "hydrogen_sulfide_concentration"
 
 
 class NitricOxideConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x0412
+    cluster_id: Final[t.uint16_t] = 0x0412
     name: Final = "Nitric Oxide (NO) Concentration"
     ep_attribute: Final = "nitric_oxide_concentration"
 
 
 class NitrogenDioxideConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x0413
+    cluster_id: Final[t.uint16_t] = 0x0413
     name: Final = "Nitrogen Dioxide (NO₂) Concentration"
     ep_attribute: Final = "nitrogen_dioxide_concentration"
 
 
 class OxygenConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x0414
+    cluster_id: Final[t.uint16_t] = 0x0414
     name: Final = "Oxygen (O₂) Concentration"
     ep_attribute: Final = "oxygen_concentration"
 
 
 class OzoneConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x0415
+    cluster_id: Final[t.uint16_t] = 0x0415
     name: Final = "Ozone (O₃) Concentration"
     ep_attribute: Final = "ozone_concentration"
 
 
 class SulfurDioxideConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x0416
+    cluster_id: Final[t.uint16_t] = 0x0416
     name: Final = "Sulfur Dioxide (SO₂) Concentration"
     ep_attribute: Final = "sulfur_dioxide_concentration"
 
 
 class DissolvedOxygenConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x0417
+    cluster_id: Final[t.uint16_t] = 0x0417
     name: Final = "Dissolved Oxygen (DO) Concentration"
     ep_attribute: Final = "dissolved_oxygen_concentration"
 
 
 class BromateConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x0418
+    cluster_id: Final[t.uint16_t] = 0x0418
     name: Final = "Bromate Concentration"
     ep_attribute: Final = "bromate_concentration"
 
 
 class ChloraminesConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x0419
+    cluster_id: Final[t.uint16_t] = 0x0419
     name: Final = "Chloramines Concentration"
     ep_attribute: Final = "chloramines_concentration"
 
 
 class ChlorineConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x041A
+    cluster_id: Final[t.uint16_t] = 0x041A
     name: Final = "Chlorine Concentration"
     ep_attribute: Final = "chlorine_concentration"
 
 
 class FecalColiformAndEColiFraction(_ConcentrationMixin, Cluster):
     """Percent of positive samples"""
 
-    cluster_id: Final = 0x041B
+    cluster_id: Final[t.uint16_t] = 0x041B
     name: Final = "Fecal coliform & E. Coli Fraction"
     ep_attribute: Final = "fecal_coliform_and_e_coli_fraction"
 
 
 class FluorideConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x041C  # XXX: spec repeats 0x041B but this seems like a mistake
+    cluster_id: Final[t.uint16_t] = (
+        0x041C  # XXX: spec repeats 0x041B but this seems like a mistake
+    )
     name: Final = "Fluoride Concentration"
     ep_attribute: Final = "fluoride_concentration"
 
 
 class HaloaceticAcidsConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x041D
+    cluster_id: Final[t.uint16_t] = 0x041D
     name: Final = "Haloacetic Acids Concentration"
     ep_attribute: Final = "haloacetic_acids_concentration"
 
 
 class TotalTrihalomethanesConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x041E
+    cluster_id: Final[t.uint16_t] = 0x041E
     name: Final = "Total Trihalomethanes Concentration"
     ep_attribute: Final = "total_trihalomethanes_concentration"
 
 
 class TotalColiformBacteriaFraction(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x041F
+    cluster_id: Final[t.uint16_t] = 0x041F
     name: Final = "Total Coliform Bacteria Fraction"
     ep_attribute: Final = "total_coliform_bacteria_fraction"
 
 
 # XXX: is this a concentration? What are the units?
 class Turbidity(_ConcentrationMixin, Cluster):
     """Cloudiness of particles in water where an average person would notice a 5 or higher"""
 
-    cluster_id: Final = 0x0420
+    cluster_id: Final[t.uint16_t] = 0x0420
     name: Final = "Turbidity"
     ep_attribute: Final = "turbidity"
 
 
 class CopperConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x0421
+    cluster_id: Final[t.uint16_t] = 0x0421
     name: Final = "Copper Concentration"
     ep_attribute: Final = "copper_concentration"
 
 
 class LeadConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x0422
+    cluster_id: Final[t.uint16_t] = 0x0422
     name: Final = "Lead Concentration"
     ep_attribute: Final = "lead_concentration"
 
 
 class ManganeseConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x0423
+    cluster_id: Final[t.uint16_t] = 0x0423
     name: Final = "Manganese Concentration"
     ep_attribute: Final = "manganese_concentration"
 
 
 class SulfateConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x0424
+    cluster_id: Final[t.uint16_t] = 0x0424
     name: Final = "Sulfate Concentration"
     ep_attribute: Final = "sulfate_concentration"
 
 
 class BromodichloromethaneConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x0425
+    cluster_id: Final[t.uint16_t] = 0x0425
     name: Final = "Bromodichloromethane Concentration"
     ep_attribute: Final = "bromodichloromethane_concentration"
 
 
 class BromoformConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x0426
+    cluster_id: Final[t.uint16_t] = 0x0426
     name: Final = "Bromoform Concentration"
     ep_attribute: Final = "bromoform_concentration"
 
 
 class ChlorodibromomethaneConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x0427
+    cluster_id: Final[t.uint16_t] = 0x0427
     name: Final = "Chlorodibromomethane Concentration"
     ep_attribute: Final = "chlorodibromomethane_concentration"
 
 
 class ChloroformConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x0428
+    cluster_id: Final[t.uint16_t] = 0x0428
     name: Final = "Chloroform Concentration"
     ep_attribute: Final = "chloroform_concentration"
 
 
 class SodiumConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x0429
+    cluster_id: Final[t.uint16_t] = 0x0429
     name: Final = "Sodium Concentration"
     ep_attribute: Final = "sodium_concentration"
 
 
 # XXX: is this a concentration? What are the units?
 class PM25(_ConcentrationMixin, Cluster):
     """Particulate Matter 2.5 microns or less"""
 
-    cluster_id: Final = 0x042A
+    cluster_id: Final[t.uint16_t] = 0x042A
     name: Final = "PM2.5"
     ep_attribute: Final = "pm25"
 
 
 class FormaldehydeConcentration(_ConcentrationMixin, Cluster):
-    cluster_id: Final = 0x042B
+    cluster_id: Final[t.uint16_t] = 0x042B
     name: Final = "Formaldehyde Concentration"
     ep_attribute: Final = "formaldehyde_concentration"
```

### Comparing `zigpy-0.63.5/zigpy/zcl/clusters/protocol.py` & `zigpy-0.64.0/zigpy/zcl/clusters/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 class DateTime(t.Struct):
     date: t.uint32_t
     time: t.uint32_t
 
 
 class GenericTunnel(Cluster):
-    cluster_id: Final = 0x0600
+    cluster_id: Final[t.uint16_t] = 0x0600
     ep_attribute: Final = "generic_tunnel"
 
     class AttributeDefs(BaseAttributeDefs):
         max_income_trans_size: Final = ZCLAttributeDef(id=0x0001, type=t.uint16_t)
         max_outgo_trans_size: Final = ZCLAttributeDef(id=0x0002, type=t.uint16_t)
         protocol_addr: Final = ZCLAttributeDef(id=0x0003, type=t.LVBytes)
 
@@ -37,39 +37,39 @@
         )
         advertise_protocol_address: Final = ZCLCommandDef(
             id=0x01, schema={}, direction=False
         )
 
 
 class BacnetProtocolTunnel(Cluster):
-    cluster_id: Final = 0x0601
+    cluster_id: Final[t.uint16_t] = 0x0601
     ep_attribute: Final = "bacnet_tunnel"
 
     class ServerCommandDefs(BaseCommandDefs):
         transfer_npdu: Final = ZCLCommandDef(
             id=0x00, schema={"npdu": t.LVBytes}, direction=False
         )
 
 
 class AnalogInputRegular(Cluster):
-    cluster_id: Final = 0x0602
+    cluster_id: Final[t.uint16_t] = 0x0602
     ep_attribute: Final = "bacnet_regular_analog_input"
 
     class AttributeDefs(BaseAttributeDefs):
         cov_increment: Final = ZCLAttributeDef(id=0x0016, type=t.Single)
         device_type: Final = ZCLAttributeDef(id=0x001F, type=t.CharacterString)
         object_id: Final = ZCLAttributeDef(id=0x004B, type=t.FixedList[4, t.uint8_t])
         object_name: Final = ZCLAttributeDef(id=0x004D, type=t.CharacterString)
         object_type: Final = ZCLAttributeDef(id=0x004F, type=t.enum16)
         update_interval: Final = ZCLAttributeDef(id=0x0076, type=t.uint8_t)
         profile_name: Final = ZCLAttributeDef(id=0x00A8, type=t.CharacterString)
 
 
 class AnalogInputExtended(Cluster):
-    cluster_id: Final = 0x0603
+    cluster_id: Final[t.uint16_t] = 0x0603
     ep_attribute: Final = "bacnet_extended_analog_input"
 
     class AttributeDefs(BaseAttributeDefs):
         acked_transitions: Final = ZCLAttributeDef(id=0x0000, type=t.bitmap8)
         notification_class: Final = ZCLAttributeDef(id=0x0011, type=t.uint16_t)
         deadband: Final = ZCLAttributeDef(id=0x0019, type=t.Single)
         event_enable: Final = ZCLAttributeDef(id=0x0023, type=t.bitmap8)
@@ -86,29 +86,29 @@
         transfer_apdu: Final = ZCLCommandDef(id=0x00, schema={}, direction=False)
         connect_req: Final = ZCLCommandDef(id=0x01, schema={}, direction=False)
         disconnect_req: Final = ZCLCommandDef(id=0x02, schema={}, direction=False)
         connect_status_noti: Final = ZCLCommandDef(id=0x03, schema={}, direction=False)
 
 
 class AnalogOutputRegular(Cluster):
-    cluster_id: Final = 0x0604
+    cluster_id: Final[t.uint16_t] = 0x0604
     ep_attribute: Final = "bacnet_regular_analog_output"
 
     class AttributeDefs(BaseAttributeDefs):
         cov_increment: Final = ZCLAttributeDef(id=0x0016, type=t.Single)
         device_type: Final = ZCLAttributeDef(id=0x001F, type=t.CharacterString)
         object_id: Final = ZCLAttributeDef(id=0x004B, type=t.FixedList[4, t.uint8_t])
         object_name: Final = ZCLAttributeDef(id=0x004D, type=t.CharacterString)
         object_type: Final = ZCLAttributeDef(id=0x004F, type=t.enum16)
         update_interval: Final = ZCLAttributeDef(id=0x0076, type=t.uint8_t)
         profile_name: Final = ZCLAttributeDef(id=0x00A8, type=t.CharacterString)
 
 
 class AnalogOutputExtended(Cluster):
-    cluster_id: Final = 0x0605
+    cluster_id: Final[t.uint16_t] = 0x0605
     ep_attribute: Final = "bacnet_extended_analog_output"
 
     class AttributeDefs(BaseAttributeDefs):
         acked_transitions: Final = ZCLAttributeDef(id=0x0000, type=t.bitmap8)
         notification_class: Final = ZCLAttributeDef(id=0x0011, type=t.uint16_t)
         deadband: Final = ZCLAttributeDef(id=0x0019, type=t.Single)
         event_enable: Final = ZCLAttributeDef(id=0x0023, type=t.bitmap8)
@@ -119,27 +119,27 @@
         notify_type: Final = ZCLAttributeDef(id=0x0048, type=t.enum8)
         time_delay: Final = ZCLAttributeDef(id=0x0071, type=t.uint8_t)
         # event_time_stamps: Final = ZCLAttributeDef(id=0x0082, type=t.Array[3, t.uint32_t])
         # integer, time of day, or structure of (date, time of day))
 
 
 class AnalogValueRegular(Cluster):
-    cluster_id: Final = 0x0606
+    cluster_id: Final[t.uint16_t] = 0x0606
     ep_attribute: Final = "bacnet_regular_analog_value"
 
     class AttributeDefs(BaseAttributeDefs):
         cov_increment: Final = ZCLAttributeDef(id=0x0016, type=t.Single)
         object_id: Final = ZCLAttributeDef(id=0x004B, type=t.FixedList[4, t.uint8_t])
         object_name: Final = ZCLAttributeDef(id=0x004D, type=t.CharacterString)
         object_type: Final = ZCLAttributeDef(id=0x004F, type=t.enum16)
         profile_name: Final = ZCLAttributeDef(id=0x00A8, type=t.CharacterString)
 
 
 class AnalogValueExtended(Cluster):
-    cluster_id: Final = 0x0607
+    cluster_id: Final[t.uint16_t] = 0x0607
     ep_attribute: Final = "bacnet_extended_analog_value"
 
     class AttributeDefs(BaseAttributeDefs):
         acked_transitions: Final = ZCLAttributeDef(id=0x0000, type=t.bitmap8)
         notification_class: Final = ZCLAttributeDef(id=0x0011, type=t.uint16_t)
         deadband: Final = ZCLAttributeDef(id=0x0019, type=t.Single)
         event_enable: Final = ZCLAttributeDef(id=0x0023, type=t.bitmap8)
@@ -148,15 +148,15 @@
         limit_enable: Final = ZCLAttributeDef(id=0x0034, type=t.bitmap8)
         low_limit: Final = ZCLAttributeDef(id=0x003B, type=t.Single)
         notify_type: Final = ZCLAttributeDef(id=0x0048, type=t.enum8)
         time_delay: Final = ZCLAttributeDef(id=0x0071, type=t.uint8_t)
 
 
 class BinaryInputRegular(Cluster):
-    cluster_id: Final = 0x0608
+    cluster_id: Final[t.uint16_t] = 0x0608
     ep_attribute: Final = "bacnet_regular_binary_input"
 
     class AttributeDefs(BaseAttributeDefs):
         change_of_state_count: Final = ZCLAttributeDef(id=0x000F, type=t.uint32_t)
         change_of_state_time: Final = ZCLAttributeDef(id=0x0010, type=DateTime)
         device_type: Final = ZCLAttributeDef(id=0x001F, type=t.CharacterString)
         elapsed_active_time: Final = ZCLAttributeDef(id=0x0021, type=t.uint32_t)
@@ -165,15 +165,15 @@
         object_type: Final = ZCLAttributeDef(id=0x004F, type=t.enum16)
         time_of_at_reset: Final = ZCLAttributeDef(id=0x0072, type=DateTime)
         time_of_sc_reset: Final = ZCLAttributeDef(id=0x0073, type=DateTime)
         profile_name: Final = ZCLAttributeDef(id=0x00A8, type=t.CharacterString)
 
 
 class BinaryInputExtended(Cluster):
-    cluster_id: Final = 0x0609
+    cluster_id: Final[t.uint16_t] = 0x0609
     ep_attribute: Final = "bacnet_extended_binary_input"
 
     class AttributeDefs(BaseAttributeDefs):
         acked_transitions: Final = ZCLAttributeDef(id=0x0000, type=t.bitmap8)
         alarm_value: Final = ZCLAttributeDef(id=0x0006, type=t.Bool)
         notification_class: Final = ZCLAttributeDef(id=0x0011, type=t.uint16_t)
         event_enable: Final = ZCLAttributeDef(id=0x0023, type=t.bitmap8)
@@ -181,15 +181,15 @@
         notify_type: Final = ZCLAttributeDef(id=0x0048, type=t.enum8)
         time_delay: Final = ZCLAttributeDef(id=0x0071, type=t.uint8_t)
         # 0x0082: ZCLAttributeDef('event_time_stamps', type=TODO.array),  # Array[3] of (16-bit unsigned
         # integer, time of day, or structure of (date, time of day))
 
 
 class BinaryOutputRegular(Cluster):
-    cluster_id: Final = 0x060A
+    cluster_id: Final[t.uint16_t] = 0x060A
     ep_attribute: Final = "bacnet_regular_binary_output"
 
     class AttributeDefs(BaseAttributeDefs):
         change_of_state_count: Final = ZCLAttributeDef(id=0x000F, type=t.uint32_t)
         change_of_state_time: Final = ZCLAttributeDef(id=0x0010, type=DateTime)
         device_type: Final = ZCLAttributeDef(id=0x001F, type=t.CharacterString)
         elapsed_active_time: Final = ZCLAttributeDef(id=0x0021, type=t.uint32_t)
@@ -199,30 +199,30 @@
         object_type: Final = ZCLAttributeDef(id=0x004F, type=t.enum16)
         time_of_at_reset: Final = ZCLAttributeDef(id=0x0072, type=DateTime)
         time_of_sc_reset: Final = ZCLAttributeDef(id=0x0073, type=DateTime)
         profile_name: Final = ZCLAttributeDef(id=0x00A8, type=t.CharacterString)
 
 
 class BinaryOutputExtended(Cluster):
-    cluster_id: Final = 0x060B
+    cluster_id: Final[t.uint16_t] = 0x060B
     ep_attribute: Final = "bacnet_extended_binary_output"
 
     class AttributeDefs(BaseAttributeDefs):
         acked_transitions: Final = ZCLAttributeDef(id=0x0000, type=t.bitmap8)
         notification_class: Final = ZCLAttributeDef(id=0x0011, type=t.uint16_t)
         event_enable: Final = ZCLAttributeDef(id=0x0023, type=t.bitmap8)
         event_state: Final = ZCLAttributeDef(id=0x0024, type=t.enum8)
         notify_type: Final = ZCLAttributeDef(id=0x0048, type=t.enum8)
         time_delay: Final = ZCLAttributeDef(id=0x0071, type=t.uint8_t)
         # 0x0082: ZCLAttributeDef('event_time_stamps', type=TODO.array),  # Array[3] of (16-bit unsigned
         # integer, time of day, or structure of (date, time of day))
 
 
 class BinaryValueRegular(Cluster):
-    cluster_id: Final = 0x060C
+    cluster_id: Final[t.uint16_t] = 0x060C
     ep_attribute: Final = "bacnet_regular_binary_value"
 
     class AttributeDefs(BaseAttributeDefs):
         change_of_state_count: Final = ZCLAttributeDef(id=0x000F, type=t.uint32_t)
         change_of_state_time: Final = ZCLAttributeDef(id=0x0010, type=DateTime)
         elapsed_active_time: Final = ZCLAttributeDef(id=0x0021, type=t.uint32_t)
         object_id: Final = ZCLAttributeDef(id=0x004B, type=t.FixedList[4, t.uint8_t])
@@ -230,15 +230,15 @@
         object_type: Final = ZCLAttributeDef(id=0x004F, type=t.enum16)
         time_of_at_reset: Final = ZCLAttributeDef(id=0x0072, type=DateTime)
         time_of_sc_reset: Final = ZCLAttributeDef(id=0x0073, type=DateTime)
         profile_name: Final = ZCLAttributeDef(id=0x00A8, type=t.CharacterString)
 
 
 class BinaryValueExtended(Cluster):
-    cluster_id: Final = 0x060D
+    cluster_id: Final[t.uint16_t] = 0x060D
     ep_attribute: Final = "bacnet_extended_binary_value"
 
     class AttributeDefs(BaseAttributeDefs):
         acked_transitions: Final = ZCLAttributeDef(id=0x0000, type=t.bitmap8)
         alarm_value: Final = ZCLAttributeDef(id=0x0006, type=t.Bool)
         notification_class: Final = ZCLAttributeDef(id=0x0011, type=t.uint16_t)
         event_enable: Final = ZCLAttributeDef(id=0x0023, type=t.bitmap8)
@@ -246,27 +246,27 @@
         notify_type: Final = ZCLAttributeDef(id=0x0048, type=t.enum8)
         time_delay: Final = ZCLAttributeDef(id=0x0071, type=t.uint8_t)
         # 0x0082: ZCLAttributeDef('event_time_stamps', type=TODO.array),  # Array[3] of (16-bit unsigned
         # integer, time of day, or structure of (date, time of day))
 
 
 class MultistateInputRegular(Cluster):
-    cluster_id: Final = 0x060E
+    cluster_id: Final[t.uint16_t] = 0x060E
     ep_attribute: Final = "bacnet_regular_multistate_input"
 
     class AttributeDefs(BaseAttributeDefs):
         device_type: Final = ZCLAttributeDef(id=0x001F, type=t.CharacterString)
         object_id: Final = ZCLAttributeDef(id=0x004B, type=t.FixedList[4, t.uint8_t])
         object_name: Final = ZCLAttributeDef(id=0x004D, type=t.CharacterString)
         object_type: Final = ZCLAttributeDef(id=0x004F, type=t.enum16)
         profile_name: Final = ZCLAttributeDef(id=0x00A8, type=t.CharacterString)
 
 
 class MultistateInputExtended(Cluster):
-    cluster_id: Final = 0x060F
+    cluster_id: Final[t.uint16_t] = 0x060F
     ep_attribute: Final = "bacnet_extended_multistate_input"
 
     class AttributeDefs(BaseAttributeDefs):
         acked_transitions: Final = ZCLAttributeDef(id=0x0000, type=t.bitmap8)
         alarm_value: Final = ZCLAttributeDef(id=0x0006, type=t.uint16_t)
         notification_class: Final = ZCLAttributeDef(id=0x0011, type=t.uint16_t)
         event_enable: Final = ZCLAttributeDef(id=0x0023, type=t.bitmap8)
@@ -275,54 +275,54 @@
         notify_type: Final = ZCLAttributeDef(id=0x0048, type=t.enum8)
         time_delay: Final = ZCLAttributeDef(id=0x0071, type=t.uint8_t)
         # 0x0082: ZCLAttributeDef('event_time_stamps', type=TODO.array),  # Array[3] of (16-bit unsigned
         # integer, time of day, or structure of (date, time of day))
 
 
 class MultistateOutputRegular(Cluster):
-    cluster_id: Final = 0x0610
+    cluster_id: Final[t.uint16_t] = 0x0610
     ep_attribute: Final = "bacnet_regular_multistate_output"
 
     class AttributeDefs(BaseAttributeDefs):
         device_type: Final = ZCLAttributeDef(id=0x001F, type=t.CharacterString)
         feed_back_value: Final = ZCLAttributeDef(id=0x0028, type=t.enum8)
         object_id: Final = ZCLAttributeDef(id=0x004B, type=t.FixedList[4, t.uint8_t])
         object_name: Final = ZCLAttributeDef(id=0x004D, type=t.CharacterString)
         object_type: Final = ZCLAttributeDef(id=0x004F, type=t.enum16)
         profile_name: Final = ZCLAttributeDef(id=0x00A8, type=t.CharacterString)
 
 
 class MultistateOutputExtended(Cluster):
-    cluster_id: Final = 0x0611
+    cluster_id: Final[t.uint16_t] = 0x0611
     ep_attribute: Final = "bacnet_extended_multistate_output"
 
     class AttributeDefs(BaseAttributeDefs):
         acked_transitions: Final = ZCLAttributeDef(id=0x0000, type=t.bitmap8)
         notification_class: Final = ZCLAttributeDef(id=0x0011, type=t.uint16_t)
         event_enable: Final = ZCLAttributeDef(id=0x0023, type=t.bitmap8)
         event_state: Final = ZCLAttributeDef(id=0x0024, type=t.enum8)
         notify_type: Final = ZCLAttributeDef(id=0x0048, type=t.enum8)
         time_delay: Final = ZCLAttributeDef(id=0x0071, type=t.uint8_t)
         # 0x0082: ZCLAttributeDef('event_time_stamps', type=TODO.array),  # Array[3] of (16-bit unsigned
         # integer, time of day, or structure of (date, time of day))
 
 
 class MultistateValueRegular(Cluster):
-    cluster_id: Final = 0x0612
+    cluster_id: Final[t.uint16_t] = 0x0612
     ep_attribute: Final = "bacnet_regular_multistate_value"
 
     class AttributeDefs(BaseAttributeDefs):
         object_id: Final = ZCLAttributeDef(id=0x004B, type=t.FixedList[4, t.uint8_t])
         object_name: Final = ZCLAttributeDef(id=0x004D, type=t.CharacterString)
         object_type: Final = ZCLAttributeDef(id=0x004F, type=t.enum16)
         profile_name: Final = ZCLAttributeDef(id=0x00A8, type=t.CharacterString)
 
 
 class MultistateValueExtended(Cluster):
-    cluster_id: Final = 0x0613
+    cluster_id: Final[t.uint16_t] = 0x0613
     ep_attribute: Final = "bacnet_extended_multistate_value"
 
     class AttributeDefs(BaseAttributeDefs):
         acked_transitions: Final = ZCLAttributeDef(id=0x0000, type=t.bitmap8)
         alarm_value: Final = ZCLAttributeDef(id=0x0006, type=t.uint16_t)
         notification_class: Final = ZCLAttributeDef(id=0x0011, type=t.uint16_t)
         event_enable: Final = ZCLAttributeDef(id=0x0023, type=t.bitmap8)
```

### Comparing `zigpy-0.63.5/zigpy/zcl/clusters/security.py` & `zigpy-0.64.0/zigpy/zcl/clusters/security.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     """
 
     ZoneState: Final = ZoneState
     ZoneType: Final = ZoneType
     ZoneStatus: Final = ZoneStatus
     EnrollResponse: Final = EnrollResponse
 
-    cluster_id: Final = 0x0500
+    cluster_id: Final[t.uint16_t] = 0x0500
     name: Final = "IAS Zone"
     ep_attribute: Final = "ias_zone"
 
     class AttributeDefs(BaseAttributeDefs):
         # Zone Information
         zone_state: Final = ZCLAttributeDef(
             id=0x0000, type=ZoneState, access="r", mandatory=True
@@ -237,15 +237,15 @@
     AudibleNotification: Final = AudibleNotification
     BypassResponse: Final = BypassResponse
     PanelStatus: Final = PanelStatus
     ZoneType: Final = IasZone.ZoneType
     ZoneStatus: Final = IasZone.ZoneStatus
     ZoneStatusRsp: Final = ZoneStatusRsp
 
-    cluster_id: Final = 0x0501
+    cluster_id: Final[t.uint16_t] = 0x0501
     name: Final = "IAS Ancillary Control Equipment"
     ep_attribute: Final = "ias_ace"
 
     class AttributeDefs(BaseAttributeDefs):
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
@@ -480,15 +480,15 @@
     (siren, strobe lighting, etc.) when a system alarm condition is detected
     """
 
     StrobeLevel: Final = StrobeLevel
     Warning: Final = WarningType
     Squawk: Final = Squawk
 
-    cluster_id: Final = 0x0502
+    cluster_id: Final[t.uint16_t] = 0x0502
     name: Final = "IAS Warning Device"
     ep_attribute: Final = "ias_wd"
 
     class AttributeDefs(BaseAttributeDefs):
         max_duration: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint16_t, access="rw", mandatory=True
         )
```

### Comparing `zigpy-0.63.5/zigpy/zcl/clusters/smartenergy.py` & `zigpy-0.64.0/zigpy/zcl/clusters/smartenergy.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,20 @@
     BaseCommandDefs,
     ZCLAttributeDef,
     ZCLCommandDef,
 )
 
 
 class Price(Cluster):
-    cluster_id: Final = 0x0700
+    cluster_id: Final[t.uint16_t] = 0x0700
     ep_attribute: Final = "smartenergy_price"
 
 
 class Drlc(Cluster):
-    cluster_id: Final = 0x0701
+    cluster_id: Final[t.uint16_t] = 0x0701
     ep_attribute: Final = "smartenergy_drlc"
 
 
 class RegisteredTier(t.enum8):
     No_Tier = 0x00
     Tier_1 = 0x01
     Tier_2 = 0x02
@@ -40,15 +40,15 @@
     Tier_14 = 0x0E
     Extended_Tier = 0x0F
 
 
 class Metering(Cluster):
     RegisteredTier: Final = RegisteredTier
 
-    cluster_id: Final = 0x0702
+    cluster_id: Final[t.uint16_t] = 0x0702
     ep_attribute: Final = "smartenergy_metering"
 
     class AttributeDefs(BaseAttributeDefs):
         current_summ_delivered: Final = ZCLAttributeDef(
             id=0x0000, type=t.uint48_t, access="r"
         )
         current_summ_received: Final = ZCLAttributeDef(
@@ -436,49 +436,49 @@
         req_fast_poll_mode_response: Final = ZCLCommandDef(
             id=0x03, schema={}, direction=True
         )
         get_snapshot_response: Final = ZCLCommandDef(id=0x04, schema={}, direction=True)
 
 
 class Messaging(Cluster):
-    cluster_id: Final = 0x0703
+    cluster_id: Final[t.uint16_t] = 0x0703
     ep_attribute: Final = "smartenergy_messaging"
 
 
 class Tunneling(Cluster):
-    cluster_id: Final = 0x0704
+    cluster_id: Final[t.uint16_t] = 0x0704
     ep_attribute: Final = "smartenergy_tunneling"
 
 
 class Prepayment(Cluster):
-    cluster_id: Final = 0x0705
+    cluster_id: Final[t.uint16_t] = 0x0705
     ep_attribute: Final = "smartenergy_prepayment"
 
 
 class EnergyManagement(Cluster):
-    cluster_id: Final = 0x0706
+    cluster_id: Final[t.uint16_t] = 0x0706
     ep_attribute: Final = "smartenergy_energy_management"
 
 
 class Calendar(Cluster):
-    cluster_id: Final = 0x0707
+    cluster_id: Final[t.uint16_t] = 0x0707
     ep_attribute: Final = "smartenergy_calendar"
 
 
 class DeviceManagement(Cluster):
-    cluster_id: Final = 0x0708
+    cluster_id: Final[t.uint16_t] = 0x0708
     ep_attribute: Final = "smartenergy_device_management"
 
 
 class Events(Cluster):
-    cluster_id: Final = 0x0709
+    cluster_id: Final[t.uint16_t] = 0x0709
     ep_attribute: Final = "smartenergy_events"
 
 
 class MduPairing(Cluster):
-    cluster_id: Final = 0x070A
+    cluster_id: Final[t.uint16_t] = 0x070A
     ep_attribute: Final = "smartenergy_mdu_pairing"
 
 
 class KeyEstablishment(Cluster):
-    cluster_id: Final = 0x0800
+    cluster_id: Final[t.uint16_t] = 0x0800
     ep_attribute: Final = "smartenergy_key_establishment"
```

### Comparing `zigpy-0.63.5/zigpy/zcl/foundation.py` & `zigpy-0.64.0/zigpy/zcl/foundation.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/zdo/__init__.py` & `zigpy-0.64.0/zigpy/zdo/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy/zdo/types.py` & `zigpy-0.64.0/zigpy/zdo/types.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.63.5/zigpy.egg-info/PKG-INFO` & `zigpy-0.64.0/zigpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy
-Version: 0.63.5
+Version: 0.64.0
 Summary: Library implementing a Zigbee stack
 Author-email: Russell Cloran <rcloran@gmail.com>
 License: GPL-3.0
 Project-URL: repository, https://github.com/zigpy/zigpy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -28,15 +28,14 @@
 Requires-Dist: coveralls; extra == "testing"
 Requires-Dist: coverage[toml]; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-asyncio; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-timeout; extra == "testing"
 Requires-Dist: freezegun; extra == "testing"
-Requires-Dist: ruff==0.0.261; extra == "testing"
 Requires-Dist: pysqlite3-binary; (platform_system == "Linux" and python_version < "3.12") and extra == "testing"
 
 # zigpy
 
 [![Build](https://github.com/zigpy/zigpy/workflows/CI/badge.svg?branch=dev)](https://github.com/zigpy/zigpy/workflows/CI/badge.svg?branch=dev)
 [![Coverage Status](https://codecov.io/gh/zigpy/zigpy/branch/dev/graph/badge.svg)](https://codecov.io/gh/zigpy/zigpy)
```

### Comparing `zigpy-0.63.5/zigpy.egg-info/SOURCES.txt` & `zigpy-0.64.0/zigpy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 zigpy.egg-info/top_level.txt
 zigpy/appdb_schemas/__init__.py
 zigpy/appdb_schemas/schema_v0.sql
 zigpy/appdb_schemas/schema_v1.sql
 zigpy/appdb_schemas/schema_v10.sql
 zigpy/appdb_schemas/schema_v11.sql
 zigpy/appdb_schemas/schema_v12.sql
+zigpy/appdb_schemas/schema_v13.sql
 zigpy/appdb_schemas/schema_v2.sql
 zigpy/appdb_schemas/schema_v3.sql
 zigpy/appdb_schemas/schema_v4.sql
 zigpy/appdb_schemas/schema_v5.sql
 zigpy/appdb_schemas/schema_v6.sql
 zigpy/appdb_schemas/schema_v7.sql
 zigpy/appdb_schemas/schema_v8.sql
```

