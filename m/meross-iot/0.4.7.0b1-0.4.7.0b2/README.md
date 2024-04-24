# Comparing `tmp/meross_iot-0.4.7.0b1.tar.gz` & `tmp/meross_iot-0.4.7.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meross_iot-0.4.7.0b1.tar", last modified: Tue Apr 16 22:16:34 2024, max compression
+gzip compressed data, was "meross_iot-0.4.7.0b2.tar", last modified: Wed Apr 17 22:25:46 2024, max compression
```

## Comparing `meross_iot-0.4.7.0b1.tar` & `meross_iot-0.4.7.0b2.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.177346 meross_iot-0.4.7.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/.version
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19192 2024-04-16 22:16:34.177346 meross_iot-0.4.7.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.161346 meross_iot-0.4.7.0b1/meross_iot/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.165346 meross_iot-0.4.7.0b1/meross_iot/controller/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21400 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.165346 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/consumption.py
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/diffuser_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/diffuser_spray.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/dnd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/electricity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/garage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     9288 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/roller_shutter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/spray.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     9564 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/mixins/toggle.py
--rw-r--r--   0 runner    (1001) docker     (127)    18079 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/controller/subdevice.py
--rw-r--r--   0 runner    (1001) docker     (127)    10889 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/device_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/error_budget.py
--rw-r--r--   0 runner    (1001) docker     (127)    31385 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/http_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    54525 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.169346 meross_iot-0.4.7.0b1/meross_iot/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.169346 meross_iot-0.4.7.0b1/meross_iot/model/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/http/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/http/error_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/http/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/http/subdevice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.169346 meross_iot-0.4.7.0b1/meross_iot/model/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/plugin/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/plugin/light.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/plugin/power.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.169346 meross_iot-0.4.7.0b1/meross_iot/model/push/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/push/bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/push/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/push/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/push/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/push/online.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/push/unbind.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/model/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.173346 meross_iot-0.4.7.0b1/meross_iot/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/utilities/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/utilities/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/utilities/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/utilities/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    12305 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/meross_iot/utilities/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.177346 meross_iot-0.4.7.0b1/meross_iot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19192 2024-04-16 22:16:34.000000 meross_iot-0.4.7.0b1/meross_iot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-16 22:16:34.000000 meross_iot-0.4.7.0b1/meross_iot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:16:34.000000 meross_iot-0.4.7.0b1/meross_iot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-16 22:16:34.000000 meross_iot-0.4.7.0b1/meross_iot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-16 22:16:34.000000 meross_iot-0.4.7.0b1/meross_iot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-16 22:16:34.000000 meross_iot-0.4.7.0b1/meross_iot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 22:16:34.177346 meross_iot-0.4.7.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.173346 meross_iot-0.4.7.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_consumptionx.py
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_diffuser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_disconnection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_dnd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_electricity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_garage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_push_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_roller_shutter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_spray.py
--rw-r--r--   0 runner    (1001) docker     (127)    10419 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_thermostat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_toggle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_togglex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_transport_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/tests/test_valve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:34.177346 meross_iot-0.4.7.0b1/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/utilities/meross_fake_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/utilities/meross_fake_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/utilities/meross_sniffer.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-16 22:16:21.000000 meross_iot-0.4.7.0b1/utilities/mixedqueue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:25:46.650717 meross_iot-0.4.7.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/.version
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19214 2024-04-17 22:25:46.646717 meross_iot-0.4.7.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17957 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:25:46.634717 meross_iot-0.4.7.0b2/meross_iot/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:25:46.634717 meross_iot-0.4.7.0b2/meross_iot/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21400 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/controller/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:25:46.638717 meross_iot-0.4.7.0b2/meross_iot/controller/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/controller/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/controller/mixins/consumption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/controller/mixins/diffuser_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/controller/mixins/diffuser_spray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/controller/mixins/dnd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/controller/mixins/electricity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/controller/mixins/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/controller/mixins/garage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/controller/mixins/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/controller/mixins/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9288 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/controller/mixins/roller_shutter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/controller/mixins/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/controller/mixins/spray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/controller/mixins/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9564 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/controller/mixins/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/controller/mixins/toggle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18079 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/controller/subdevice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10889 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/device_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/error_budget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31385 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/http_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54530 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:25:46.638717 meross_iot-0.4.7.0b2/meross_iot/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/model/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/model/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/model/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:25:46.638717 meross_iot-0.4.7.0b2/meross_iot/model/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/model/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/model/http/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/model/http/error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/model/http/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/model/http/subdevice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:25:46.638717 meross_iot-0.4.7.0b2/meross_iot/model/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/model/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/model/plugin/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/model/plugin/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/model/plugin/power.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:25:46.642717 meross_iot-0.4.7.0b2/meross_iot/model/push/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/model/push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/model/push/bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/model/push/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/model/push/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/model/push/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/model/push/online.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/model/push/unbind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/model/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/model/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:25:46.642717 meross_iot-0.4.7.0b2/meross_iot/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/utilities/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/utilities/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/utilities/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/utilities/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12305 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/meross_iot/utilities/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:25:46.646717 meross_iot-0.4.7.0b2/meross_iot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19214 2024-04-17 22:25:46.000000 meross_iot-0.4.7.0b2/meross_iot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-17 22:25:46.000000 meross_iot-0.4.7.0b2/meross_iot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 22:25:46.000000 meross_iot-0.4.7.0b2/meross_iot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-17 22:25:46.000000 meross_iot-0.4.7.0b2/meross_iot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-17 22:25:46.000000 meross_iot-0.4.7.0b2/meross_iot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 22:25:46.000000 meross_iot-0.4.7.0b2/meross_iot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 22:25:46.650717 meross_iot-0.4.7.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:25:46.646717 meross_iot-0.4.7.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/tests/test_consumptionx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/tests/test_diffuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/tests/test_disconnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/tests/test_dnd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/tests/test_electricity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/tests/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/tests/test_garage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/tests/test_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/tests/test_push_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/tests/test_roller_shutter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/tests/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/tests/test_spray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10419 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/tests/test_thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/tests/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/tests/test_toggle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/tests/test_togglex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/tests/test_transport_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/tests/test_valve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:25:46.646717 meross_iot-0.4.7.0b2/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/utilities/meross_fake_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/utilities/meross_fake_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/utilities/meross_sniffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-17 22:25:29.000000 meross_iot-0.4.7.0b2/utilities/mixedqueue.py
```

### Comparing `meross_iot-0.4.7.0b1/LICENSE` & `meross_iot-0.4.7.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/PKG-INFO` & `meross_iot-0.4.7.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meross_iot
-Version: 0.4.7.0b1
+Version: 0.4.7.0b2
 Summary: A simple library to deal with Meross devices. At the moment MSS110, MSS210, MSS310, MSS310H smart plugs and the MSS425E power strip. Other meross device might work out of the box with limited functionality. Give it a try and, in case of problems, let the developer know by opening an issue on Github.
 Home-page: https://github.com/albertogeniola/MerossIot
 Author: Alberto Geniola
 Author-email: albertogeniola@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/albertogeniola/MerossIot
 Project-URL: Funding, https://donate.pypi.org
@@ -210,17 +210,18 @@
 the pipeline will issue on/off commands against real devices, that are dedicated 24/7 to the tests.
 Such devices have been bought by myself (with contributions received by donors).
 However, keeping such devices connected 24/7 has a cost, which I sustain happily due to the success of the library.
 Anyway, feel free to contribute via donations!
 </p>
 
 ## Changelog
-#### 0.4.7.0b1
+#### 0.4.7.0b2
 - Added local-lan encryption capabilities to support newest Meross devices
 - Fixed roller shutter mixin not updating initial position after a full async_update() invocation
+- Attempt to fix #352
 
 <details>
     <summary>Older</summary>
 #### 0.4.6.2
 - Fix dependency specification for paho-mqtt and other libraries
 
 #### 0.4.6.0
```

### Comparing `meross_iot-0.4.7.0b1/README.md` & `meross_iot-0.4.7.0b2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -187,17 +187,18 @@
 the pipeline will issue on/off commands against real devices, that are dedicated 24/7 to the tests.
 Such devices have been bought by myself (with contributions received by donors).
 However, keeping such devices connected 24/7 has a cost, which I sustain happily due to the success of the library.
 Anyway, feel free to contribute via donations!
 </p>
 
 ## Changelog
-#### 0.4.7.0b1
+#### 0.4.7.0b2
 - Added local-lan encryption capabilities to support newest Meross devices
 - Fixed roller shutter mixin not updating initial position after a full async_update() invocation
+- Attempt to fix #352
 
 <details>
     <summary>Older</summary>
 #### 0.4.6.2
 - Fix dependency specification for paho-mqtt and other libraries
 
 #### 0.4.6.0
```

### Comparing `meross_iot-0.4.7.0b1/meross_iot/controller/device.py` & `meross_iot-0.4.7.0b2/meross_iot/controller/device.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/consumption.py` & `meross_iot-0.4.7.0b2/meross_iot/controller/mixins/consumption.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/diffuser_light.py` & `meross_iot-0.4.7.0b2/meross_iot/controller/mixins/diffuser_light.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/diffuser_spray.py` & `meross_iot-0.4.7.0b2/meross_iot/controller/mixins/diffuser_spray.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/dnd.py` & `meross_iot-0.4.7.0b2/meross_iot/controller/mixins/dnd.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/electricity.py` & `meross_iot-0.4.7.0b2/meross_iot/controller/mixins/electricity.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/encryption.py` & `meross_iot-0.4.7.0b2/meross_iot/controller/mixins/encryption.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/garage.py` & `meross_iot-0.4.7.0b2/meross_iot/controller/mixins/garage.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/hub.py` & `meross_iot-0.4.7.0b2/meross_iot/controller/mixins/hub.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/light.py` & `meross_iot-0.4.7.0b2/meross_iot/controller/mixins/light.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/roller_shutter.py` & `meross_iot-0.4.7.0b2/meross_iot/controller/mixins/roller_shutter.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/runtime.py` & `meross_iot-0.4.7.0b2/meross_iot/controller/mixins/runtime.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/spray.py` & `meross_iot-0.4.7.0b2/meross_iot/controller/mixins/spray.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/system.py` & `meross_iot-0.4.7.0b2/meross_iot/controller/mixins/system.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/thermostat.py` & `meross_iot-0.4.7.0b2/meross_iot/controller/mixins/thermostat.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/controller/mixins/toggle.py` & `meross_iot-0.4.7.0b2/meross_iot/controller/mixins/toggle.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/controller/subdevice.py` & `meross_iot-0.4.7.0b2/meross_iot/controller/subdevice.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/device_factory.py` & `meross_iot-0.4.7.0b2/meross_iot/device_factory.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/error_budget.py` & `meross_iot-0.4.7.0b2/meross_iot/error_budget.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/http_api.py` & `meross_iot-0.4.7.0b2/meross_iot/http_api.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/manager.py` & `meross_iot-0.4.7.0b2/meross_iot/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import functools
 import json
 import logging
 import random
 import ssl
 import string
 import sys
 from asyncio import Future, AbstractEventLoop
@@ -1149,21 +1150,22 @@
             _LOGGER.debug("Skipping set_result for cancelled future.")
         elif future.done():
             _LOGGER.error("This future is already done: cannot set result.")
         else:
             future.set_result(result)
 
 
-def set_future_done(future):
+def set_future_done(coroutine, future):
+    coroutine.close()
     if future in _PENDING_FUTURES:
         _PENDING_FUTURES.remove(future)
 
 
-def _schedule_later(coroutine, start_delay, loop):
-    async def delayed_execution(coro, delay, loop):
-        await asyncio.sleep(delay=delay)
-        await coro
+async def delayed_execution(coro, delay):
+    await asyncio.sleep(delay=delay)
+    await coro
+
 
-    future = asyncio.run_coroutine_threadsafe(coro=delayed_execution(coro=coroutine, delay=start_delay, loop=loop),
-                                              loop=loop)
+def _schedule_later(coroutine, start_delay, loop):
+    future = asyncio.run_coroutine_threadsafe(coro=delayed_execution(coro=coroutine, delay=start_delay), loop=loop)
     _PENDING_FUTURES.append(future)
-    future.add_done_callback(set_future_done)
+    future.add_done_callback(functools.partial(set_future_done,coroutine))
```

### Comparing `meross_iot-0.4.7.0b1/meross_iot/model/credentials.py` & `meross_iot-0.4.7.0b2/meross_iot/model/credentials.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/model/enums.py` & `meross_iot-0.4.7.0b2/meross_iot/model/enums.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/model/exception.py` & `meross_iot-0.4.7.0b2/meross_iot/model/exception.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/model/http/device.py` & `meross_iot-0.4.7.0b2/meross_iot/model/http/device.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/model/http/error_codes.py` & `meross_iot-0.4.7.0b2/meross_iot/model/http/error_codes.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/model/http/exception.py` & `meross_iot-0.4.7.0b2/meross_iot/model/http/exception.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/model/http/subdevice.py` & `meross_iot-0.4.7.0b2/meross_iot/model/http/subdevice.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/model/plugin/hub.py` & `meross_iot-0.4.7.0b2/meross_iot/model/plugin/hub.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/model/plugin/light.py` & `meross_iot-0.4.7.0b2/meross_iot/model/plugin/light.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/model/plugin/power.py` & `meross_iot-0.4.7.0b2/meross_iot/model/plugin/power.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/model/push/bind.py` & `meross_iot-0.4.7.0b2/meross_iot/model/push/bind.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/model/push/common.py` & `meross_iot-0.4.7.0b2/meross_iot/model/push/common.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/model/push/factory.py` & `meross_iot-0.4.7.0b2/meross_iot/model/push/factory.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/model/push/online.py` & `meross_iot-0.4.7.0b2/meross_iot/model/push/online.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/model/shared.py` & `meross_iot-0.4.7.0b2/meross_iot/model/shared.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/utilities/conversion.py` & `meross_iot-0.4.7.0b2/meross_iot/utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/utilities/mqtt.py` & `meross_iot-0.4.7.0b2/meross_iot/utilities/mqtt.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot/utilities/stats.py` & `meross_iot-0.4.7.0b2/meross_iot/utilities/stats.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/meross_iot.egg-info/PKG-INFO` & `meross_iot-0.4.7.0b2/meross_iot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meross_iot
-Version: 0.4.7.0b1
+Version: 0.4.7.0b2
 Summary: A simple library to deal with Meross devices. At the moment MSS110, MSS210, MSS310, MSS310H smart plugs and the MSS425E power strip. Other meross device might work out of the box with limited functionality. Give it a try and, in case of problems, let the developer know by opening an issue on Github.
 Home-page: https://github.com/albertogeniola/MerossIot
 Author: Alberto Geniola
 Author-email: albertogeniola@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/albertogeniola/MerossIot
 Project-URL: Funding, https://donate.pypi.org
@@ -210,17 +210,18 @@
 the pipeline will issue on/off commands against real devices, that are dedicated 24/7 to the tests.
 Such devices have been bought by myself (with contributions received by donors).
 However, keeping such devices connected 24/7 has a cost, which I sustain happily due to the success of the library.
 Anyway, feel free to contribute via donations!
 </p>
 
 ## Changelog
-#### 0.4.7.0b1
+#### 0.4.7.0b2
 - Added local-lan encryption capabilities to support newest Meross devices
 - Fixed roller shutter mixin not updating initial position after a full async_update() invocation
+- Attempt to fix #352
 
 <details>
     <summary>Older</summary>
 #### 0.4.6.2
 - Fix dependency specification for paho-mqtt and other libraries
 
 #### 0.4.6.0
```

### Comparing `meross_iot-0.4.7.0b1/meross_iot.egg-info/SOURCES.txt` & `meross_iot-0.4.7.0b2/meross_iot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/setup.py` & `meross_iot-0.4.7.0b2/setup.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/tests/test_consumptionx.py` & `meross_iot-0.4.7.0b2/tests/test_consumptionx.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/tests/test_diffuser.py` & `meross_iot-0.4.7.0b2/tests/test_diffuser.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/tests/test_disconnection.py` & `meross_iot-0.4.7.0b2/tests/test_disconnection.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/tests/test_dnd.py` & `meross_iot-0.4.7.0b2/tests/test_dnd.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/tests/test_electricity.py` & `meross_iot-0.4.7.0b2/tests/test_electricity.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/tests/test_error.py` & `meross_iot-0.4.7.0b2/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/tests/test_garage.py` & `meross_iot-0.4.7.0b2/tests/test_garage.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/tests/test_http.py` & `meross_iot-0.4.7.0b2/tests/test_http.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         assert devices is not None
         assert len(devices) > 0
 
 
     @unittest_run_loop
     async def test_bad_domain(self):
         with self.assertRaises(BadDomainException):
-            return await MerossHttpClient.async_from_user_password(api_base_url="iot.meross.com", email=_TEST_EMAIL, password=_TEST_PASSWORD, auto_retry_on_bad_domain=False)
+            return await MerossHttpClient.async_from_user_password(api_base_url="iotx-ap.meross.com", email=_TEST_EMAIL, password=_TEST_PASSWORD, auto_retry_on_bad_domain=False)
 
 
     @unittest_run_loop
     async def test_subdevice_listing(self):
         devices = await self.meross_client.async_list_devices()
         # look for a msxh0 hub
         hub = None
```

### Comparing `meross_iot-0.4.7.0b1/tests/test_hub.py` & `meross_iot-0.4.7.0b2/tests/test_hub.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/tests/test_light.py` & `meross_iot-0.4.7.0b2/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/tests/test_push_handler.py` & `meross_iot-0.4.7.0b2/tests/test_push_handler.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/tests/test_roller_shutter.py` & `meross_iot-0.4.7.0b2/tests/test_roller_shutter.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/tests/test_runtime.py` & `meross_iot-0.4.7.0b2/tests/test_runtime.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/tests/test_sensor.py` & `meross_iot-0.4.7.0b2/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/tests/test_spray.py` & `meross_iot-0.4.7.0b2/tests/test_spray.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/tests/test_thermostat.py` & `meross_iot-0.4.7.0b2/tests/test_thermostat.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/tests/test_timeout.py` & `meross_iot-0.4.7.0b2/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/tests/test_toggle.py` & `meross_iot-0.4.7.0b2/tests/test_toggle.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/tests/test_togglex.py` & `meross_iot-0.4.7.0b2/tests/test_togglex.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/tests/test_transport_mode.py` & `meross_iot-0.4.7.0b2/tests/test_transport_mode.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/tests/test_update.py` & `meross_iot-0.4.7.0b2/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/tests/test_valve.py` & `meross_iot-0.4.7.0b2/tests/test_valve.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/utilities/meross_fake_app.py` & `meross_iot-0.4.7.0b2/utilities/meross_fake_app.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/utilities/meross_fake_device.py` & `meross_iot-0.4.7.0b2/utilities/meross_fake_device.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/utilities/meross_sniffer.py` & `meross_iot-0.4.7.0b2/utilities/meross_sniffer.py`

 * *Files identical despite different names*

### Comparing `meross_iot-0.4.7.0b1/utilities/mixedqueue.py` & `meross_iot-0.4.7.0b2/utilities/mixedqueue.py`

 * *Files identical despite different names*

