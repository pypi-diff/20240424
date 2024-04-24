# Comparing `tmp/hahomematic-2024.4.9b1.tar.gz` & `tmp/hahomematic-2024.4.9b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2024.4.9b1.tar", last modified: Tue Apr 16 22:32:39 2024, max compression
+gzip compressed data, was "hahomematic-2024.4.9b2.tar", last modified: Wed Apr 17 09:22:17 2024, max compression
```

## Comparing `hahomematic-2024.4.9b1.tar` & `hahomematic-2024.4.9b2.tar`

### file list

```diff
@@ -1,107 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:32:39.820950 hahomematic-2024.4.9b1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-16 22:32:39.820950 hahomematic-2024.4.9b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:32:39.804950 hahomematic-2024.4.9b1/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/async_support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:32:39.808950 hahomematic-2024.4.9b1/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18499 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)    27542 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/caches/visibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:32:39.808950 hahomematic-2024.4.9b1/hahomematic/central/
--rw-r--r--   0 runner    (1001) docker     (127)    54211 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/central/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/central/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/central/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:32:39.808950 hahomematic-2024.4.9b1/hahomematic/client/
--rw-r--r--   0 runner    (1001) docker     (127)    42079 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34886 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/client/json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/client/xml_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14753 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/performance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:32:39.808950 hahomematic-2024.4.9b1/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:32:39.812950 hahomematic-2024.4.9b1/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26219 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    25529 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (127)    30029 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12704 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    44592 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    33530 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    29231 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:32:39.812950 hahomematic-2024.4.9b1/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:32:39.812950 hahomematic-2024.4.9b1/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (127)    14073 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:32:39.816950 hahomematic-2024.4.9b1/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic/support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:32:39.820950 hahomematic-2024.4.9b1/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-16 22:32:39.000000 hahomematic-2024.4.9b1/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-16 22:32:39.000000 hahomematic-2024.4.9b1/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:32:39.000000 hahomematic-2024.4.9b1/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:32:39.000000 hahomematic-2024.4.9b1/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-16 22:32:39.000000 hahomematic-2024.4.9b1/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-16 22:32:39.000000 hahomematic-2024.4.9b1/hahomematic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:32:39.816950 hahomematic-2024.4.9b1/hahomematic_support/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10649 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/hahomematic_support/client_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    18953 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-16 22:32:39.820950 hahomematic-2024.4.9b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:32:39.820950 hahomematic-2024.4.9b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/tests/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/tests/test_binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (127)    26329 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/tests/test_central.py
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/tests/test_central_pydevccu.py
--rw-r--r--   0 runner    (1001) docker     (127)    14900 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/tests/test_climate.py
--rw-r--r--   0 runner    (1001) docker     (127)    26891 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/tests/test_cover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/tests/test_json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    32422 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/tests/test_siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    14347 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/tests/test_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/tests/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-16 22:32:16.000000 hahomematic-2024.4.9b1/tests/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.706777 hahomematic-2024.4.9b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-17 09:22:17.706777 hahomematic-2024.4.9b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.690777 hahomematic-2024.4.9b2/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/async_support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.694777 hahomematic-2024.4.9b2/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18623 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27542 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/caches/visibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.694777 hahomematic-2024.4.9b2/hahomematic/central/
+-rw-r--r--   0 runner    (1001) docker     (127)    54211 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/central/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/central/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/central/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.694777 hahomematic-2024.4.9b2/hahomematic/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    42079 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34886 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/client/json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/client/xml_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14686 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/performance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.694777 hahomematic-2024.4.9b2/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.698777 hahomematic-2024.4.9b2/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26219 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25593 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30029 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12704 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44592 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33530 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29231 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.698777 hahomematic-2024.4.9b2/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.698777 hahomematic-2024.4.9b2/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14073 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.702777 hahomematic-2024.4.9b2/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     9533 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic/support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.706777 hahomematic-2024.4.9b2/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-17 09:22:17.000000 hahomematic-2024.4.9b2/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-17 09:22:17.000000 hahomematic-2024.4.9b2/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:22:17.000000 hahomematic-2024.4.9b2/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:22:17.000000 hahomematic-2024.4.9b2/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-17 09:22:17.000000 hahomematic-2024.4.9b2/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 09:22:17.000000 hahomematic-2024.4.9b2/hahomematic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.702777 hahomematic-2024.4.9b2/hahomematic_support/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10649 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/hahomematic_support/client_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18953 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-17 09:22:17.706777 hahomematic-2024.4.9b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:17.706777 hahomematic-2024.4.9b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26329 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_central.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_central_pydevccu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14900 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26891 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32422 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15478 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-17 09:21:54.000000 hahomematic-2024.4.9b2/tests/test_text.py
```

### Comparing `hahomematic-2024.4.9b1/LICENSE` & `hahomematic-2024.4.9b2/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/PKG-INFO` & `hahomematic-2024.4.9b2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.4.9b1
+Version: 2024.4.9b2
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.4.9b1/README.md` & `hahomematic-2024.4.9b2/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/__init__.py` & `hahomematic-2024.4.9b2/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/async_support.py` & `hahomematic-2024.4.9b2/hahomematic/async_support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/caches/dynamic.py` & `hahomematic-2024.4.9b2/hahomematic/caches/dynamic.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,24 +22,19 @@
     INIT_DATETIME,
     MAX_CACHE_AGE,
     NO_CACHE_ENTRY,
     CallSource,
     EventType,
     InterfaceEventType,
     InterfaceName,
-    Parameter,
     ParamsetKey,
 )
+from hahomematic.converter import CONVERTABLE_PARAMETERS, convert_combined_parameter_to_paramset
 from hahomematic.platforms.device import HmDevice
-from hahomematic.support import (
-    changed_within_seconds,
-    convert_combined_parameter_to_paramset,
-    get_channel_no,
-    get_device_address,
-)
+from hahomematic.support import changed_within_seconds, get_channel_no, get_device_address
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 
 class CommandCache:
     """Cache for send commands."""
 
@@ -54,16 +49,18 @@
     def add_set_value(
         self,
         channel_address: str,
         parameter: str,
         value: Any,
     ) -> None:
         """Add data from set value command."""
-        if parameter == Parameter.COMBINED_PARAMETER:
-            self.add_combined_parameter(channel_address=channel_address, combined_parameter=value)
+        if parameter in CONVERTABLE_PARAMETERS:
+            self.add_combined_parameter(
+                parameter=parameter, channel_address=channel_address, combined_parameter=value
+            )
             return
 
         key = (
             ParamsetKey.VALUES.value,
             get_device_address(channel_address),
             get_channel_no(channel_address),
             parameter,
@@ -83,17 +80,21 @@
                 paramset_key,
                 get_device_address(channel_address),
                 get_channel_no(channel_address),
                 parameter,
             )
             self._last_send_command[key] = (value, datetime.now())
 
-    def add_combined_parameter(self, channel_address: str, combined_parameter: str) -> None:
+    def add_combined_parameter(
+        self, parameter: str, channel_address: str, combined_parameter: str
+    ) -> None:
         """Add data from combined parameter."""
-        if values := convert_combined_parameter_to_paramset(combined_parameter=combined_parameter):
+        if values := convert_combined_parameter_to_paramset(
+            parameter=parameter, cpv=combined_parameter
+        ):
             self.add_put_paramset(
                 channel_address=channel_address,
                 paramset_key=ParamsetKey.VALUES.value,
                 values=values,
             )
 
     def get_last_value_send(
```

### Comparing `hahomematic-2024.4.9b1/hahomematic/caches/persistent.py` & `hahomematic-2024.4.9b2/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/caches/visibility.py` & `hahomematic-2024.4.9b2/hahomematic/caches/visibility.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/central/__init__.py` & `hahomematic-2024.4.9b2/hahomematic/central/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/central/decorators.py` & `hahomematic-2024.4.9b2/hahomematic/central/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/central/xml_rpc_server.py` & `hahomematic-2024.4.9b2/hahomematic/central/xml_rpc_server.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/client/__init__.py` & `hahomematic-2024.4.9b2/hahomematic/client/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/client/json_rpc.py` & `hahomematic-2024.4.9b2/hahomematic/client/json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/client/xml_rpc.py` & `hahomematic-2024.4.9b2/hahomematic/client/xml_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/config.py` & `hahomematic-2024.4.9b2/hahomematic/config.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/const.py` & `hahomematic-2024.4.9b2/hahomematic/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -407,17 +407,14 @@
     BOOL = "BOOL"
     ENUM = "ENUM"
     FLOAT = "FLOAT"
     INTEGER = "INTEGER"
     STRING = "STRING"
 
 
-COMBINED_PARAMETER_NAMES: Final = {"L": "LEVEL", "L2": "LEVEL2"}
-
-
 CLICK_EVENTS: Final[tuple[Parameter, ...]] = (
     Parameter.PRESS,
     Parameter.PRESS_CONT,
     Parameter.PRESS_LOCK,
     Parameter.PRESS_LONG,
     Parameter.PRESS_LONG_RELEASE,
     Parameter.PRESS_LONG_START,
```

### Comparing `hahomematic-2024.4.9b1/hahomematic/exceptions.py` & `hahomematic-2024.4.9b2/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/hmcli.py` & `hahomematic-2024.4.9b2/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/performance.py` & `hahomematic-2024.4.9b2/hahomematic/performance.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/__init__.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/custom/__init__.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/custom/climate.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/custom/const.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/custom/cover.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/custom/cover.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from collections.abc import Mapping
 from enum import IntEnum, StrEnum
 import logging
 from typing import Any, Final
 
 from hahomematic.const import EntityUsage, HmPlatform, Parameter
+from hahomematic.converter import convert_hm_level_to_cpv
 from hahomematic.platforms import device as hmd
 from hahomematic.platforms.custom import definition as hmed
 from hahomematic.platforms.custom.const import DeviceProfile, Field
 from hahomematic.platforms.custom.entity import CustomEntity
 from hahomematic.platforms.custom.support import CustomConfig, ExtendedConfig
 from hahomematic.platforms.decorators import value_property
 from hahomematic.platforms.entity import CallParameterCollector, bind_collector
@@ -360,17 +361,17 @@
     ) -> str | None:
         """Return the combined parameter."""
         if level is None and tilt_level is None:
             return None
         levels: list[str] = []
         # the resulting hex value is based on the doubled position
         if level is not None:
-            levels.append(format(int(level * 100 * 2), "#04x"))
+            levels.append(convert_hm_level_to_cpv(hm_level=level))
         if tilt_level is not None:
-            levels.append(format(int(tilt_level * 100 * 2), "#04x"))
+            levels.append(convert_hm_level_to_cpv(hm_level=tilt_level))
 
         if levels:
             return ",".join(levels)
         return None
 
 
 class CeIpBlind(CeBlind):
```

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/custom/definition.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/custom/entity.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/custom/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/custom/light.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/custom/light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/custom/lock.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/custom/siren.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/custom/support.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/custom/switch.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/decorators.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/device.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/entity.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/event.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/generic/__init__.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/generic/action.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/generic/button.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/generic/entity.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/generic/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/generic/number.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/generic/select.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/generic/sensor.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/generic/switch.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/hub/__init__.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/hub/button.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/hub/entity.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/hub/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/hub/number.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/hub/select.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/hub/sensor.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/hub/text.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/support.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/platforms/update.py` & `hahomematic-2024.4.9b2/hahomematic/platforms/update.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2024.4.9b2/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2024.4.9b2/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2024.4.9b2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/hahomematic/support.py` & `hahomematic-2024.4.9b2/hahomematic/support.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import socket
 import ssl
 import sys
 from typing import Any, Final
 
 from hahomematic.const import (
     CCU_PASSWORD_PATTERN,
-    COMBINED_PARAMETER_NAMES,
     FILE_DEVICES,
     FILE_PARAMSETS,
     IDENTIFIER_SEPARATOR,
     INIT_DATETIME,
     MAX_CACHE_AGE,
     NO_CACHE_ENTRY,
     SysvarType,
@@ -289,24 +288,14 @@
     def is_valid(self) -> bool:
         """Return if entry is valid."""
         if self.value == NO_CACHE_ENTRY:
             return False
         return changed_within_seconds(last_change=self.last_refresh)
 
 
-def convert_combined_parameter_to_paramset(combined_parameter: str) -> dict[str, Any]:
-    """Convert combined parameter to paramset."""
-    paramset: dict[str, Any] = {}
-    for cp_param_value in combined_parameter.split(","):
-        cp_param, value = cp_param_value.split("=")
-        if parameter := COMBINED_PARAMETER_NAMES.get(cp_param):
-            paramset[parameter] = value
-    return paramset
-
-
 def debug_enabled() -> bool:
     """Check if debug mode is enabled."""
     try:
         if sys.gettrace() is not None:
             return True
     except AttributeError:
         pass
```

### Comparing `hahomematic-2024.4.9b1/hahomematic.egg-info/PKG-INFO` & `hahomematic-2024.4.9b2/hahomematic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.4.9b1
+Version: 2024.4.9b2
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.4.9b1/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2024.4.9b2/hahomematic.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 setup.cfg
 hahomematic/__init__.py
 hahomematic/async_support.py
 hahomematic/config.py
 hahomematic/const.py
+hahomematic/converter.py
 hahomematic/exceptions.py
 hahomematic/hmcli.py
 hahomematic/performance.py
 hahomematic/py.typed
 hahomematic/support.py
 hahomematic.egg-info/PKG-INFO
 hahomematic.egg-info/SOURCES.txt
```

### Comparing `hahomematic-2024.4.9b1/hahomematic_support/client_local.py` & `hahomematic-2024.4.9b2/hahomematic_support/client_local.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/pyproject.toml` & `hahomematic-2024.4.9b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=69.2.0", "wheel~=0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2024.4.9b1"
+version     = "2024.4.9b2"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
```

### Comparing `hahomematic-2024.4.9b1/tests/test_action.py` & `hahomematic-2024.4.9b2/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/tests/test_binary_sensor.py` & `hahomematic-2024.4.9b2/tests/test_binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/tests/test_button.py` & `hahomematic-2024.4.9b2/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/tests/test_central.py` & `hahomematic-2024.4.9b2/tests/test_central.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/tests/test_central_pydevccu.py` & `hahomematic-2024.4.9b2/tests/test_central_pydevccu.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/tests/test_climate.py` & `hahomematic-2024.4.9b2/tests/test_climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/tests/test_cover.py` & `hahomematic-2024.4.9b2/tests/test_cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/tests/test_decorator.py` & `hahomematic-2024.4.9b2/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/tests/test_device.py` & `hahomematic-2024.4.9b2/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/tests/test_entity.py` & `hahomematic-2024.4.9b2/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/tests/test_event.py` & `hahomematic-2024.4.9b2/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/tests/test_json_rpc.py` & `hahomematic-2024.4.9b2/tests/test_json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/tests/test_light.py` & `hahomematic-2024.4.9b2/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/tests/test_lock.py` & `hahomematic-2024.4.9b2/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/tests/test_number.py` & `hahomematic-2024.4.9b2/tests/test_number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/tests/test_select.py` & `hahomematic-2024.4.9b2/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/tests/test_sensor.py` & `hahomematic-2024.4.9b2/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/tests/test_siren.py` & `hahomematic-2024.4.9b2/tests/test_siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/tests/test_support.py` & `hahomematic-2024.4.9b2/tests/test_support.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Tests for switch entities of hahomematic."""
 
 from __future__ import annotations
 
+from collections.abc import Callable
 from datetime import datetime, timedelta
+from typing import Any
 from unittest.mock import patch
 
 import pytest
 
 from hahomematic.caches.visibility import _get_value_from_dict_by_wildcard_key
 from hahomematic.const import INIT_DATETIME, EntityUsage, ParameterType, SysvarType
+from hahomematic.converter import _COMBINED_PARAMETER_TO_HM_CONVERTER, convert_hm_level_to_cpv
 from hahomematic.exceptions import HaHomematicException
 from hahomematic.platforms.support import (
     _check_channel_name_with_channel_no,
     convert_value,
     generate_unique_id,
     get_custom_entity_name,
     get_device_name,
@@ -417,7 +420,50 @@
     assert check_password("t") is True
     assert check_password("test") is True
     assert check_password("TEST") is True
     assert check_password("1234") is True
     assert check_password("test123TEST") is True
     assert check_password("test.!$():;#-") is True
     assert check_password("test%") is False
+
+
+@pytest.mark.parametrize(
+    ("parameter", "input_value", "converter", "result_value"),
+    [
+        (
+            "LEVEL_COMBINED",
+            0,
+            convert_hm_level_to_cpv,
+            "0x00",
+        ),
+        (
+            "LEVEL_COMBINED",
+            0.17,
+            convert_hm_level_to_cpv,
+            "0x22",
+        ),
+        (
+            "LEVEL_COMBINED",
+            0.81,
+            convert_hm_level_to_cpv,
+            "0xa2",
+        ),
+        (
+            "LEVEL_COMBINED",
+            1,
+            convert_hm_level_to_cpv,
+            "0xc8",
+        ),
+    ],
+)
+def test_converter(
+    parameter: str,
+    input_value: Any,
+    converter: Callable,
+    result_value: Any,
+) -> None:
+    """Test device un ignore."""
+
+    assert input_value is not None
+    assert converter(input_value) == result_value
+    if re_converter := _COMBINED_PARAMETER_TO_HM_CONVERTER.get(parameter):
+        assert re_converter(result_value) == input_value
```

### Comparing `hahomematic-2024.4.9b1/tests/test_switch.py` & `hahomematic-2024.4.9b2/tests/test_switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.9b1/tests/test_text.py` & `hahomematic-2024.4.9b2/tests/test_text.py`

 * *Files identical despite different names*

