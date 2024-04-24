# Comparing `tmp/sml2mqtt-2.2.tar.gz` & `tmp/sml2mqtt-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sml2mqtt-2.2.tar", last modified: Fri Mar 31 05:13:02 2023, max compression
+gzip compressed data, was "sml2mqtt-3.0.tar", last modified: Wed Apr 24 04:53:23 2024, max compression
```

## Comparing `sml2mqtt-2.2.tar` & `sml2mqtt-3.0.tar`

### file list

```diff
@@ -1,65 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:13:02.288910 sml2mqtt-2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-31 05:12:48.000000 sml2mqtt-2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-31 05:12:48.000000 sml2mqtt-2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-03-31 05:13:02.288910 sml2mqtt-2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-31 05:12:48.000000 sml2mqtt-2.2/requirements_setup.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 05:13:02.288910 sml2mqtt-2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-03-31 05:12:48.000000 sml2mqtt-2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:13:02.280910 sml2mqtt-2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:13:02.284910 sml2mqtt-2.2/src/sml2mqtt/
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/__args__.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/__log__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/__shutdown__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:13:02.284910 sml2mqtt-2.2/src/sml2mqtt/config/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/config/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/config/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/config/mqtt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:13:02.284910 sml2mqtt-2.2/src/sml2mqtt/device/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/device/sml_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/device/sml_device_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/device/sml_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/device/sml_value_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/device/watchdog.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:13:02.284910 sml2mqtt-2.2/src/sml2mqtt/mqtt/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/mqtt/connect_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/mqtt/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/mqtt/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/mqtt/mqtt_obj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:13:02.288910 sml2mqtt-2.2/src/sml2mqtt/sml_value/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/sml_value/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/sml_value/__types__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/sml_value/enum_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:13:02.288910 sml2mqtt-2.2/src/sml2mqtt/sml_value/filter/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/sml_value/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/sml_value/filter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/sml_value/filter/change.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/sml_value/filter/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/sml_value/filter/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/sml_value/sml_value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:13:02.288910 sml2mqtt-2.2/src/sml2mqtt/sml_value/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/sml_value/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/sml_value/transformations/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/sml_value/transformations/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:13:02.288910 sml2mqtt-2.2/src/sml2mqtt/sml_value/workarounds/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/sml_value/workarounds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/sml_value/workarounds/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-03-31 05:12:48.000000 sml2mqtt-2.2/src/sml2mqtt/sml_value/workarounds/negative_on_energy_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:13:02.284910 sml2mqtt-2.2/src/sml2mqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-03-31 05:13:02.000000 sml2mqtt-2.2/src/sml2mqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-31 05:13:02.000000 sml2mqtt-2.2/src/sml2mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 05:13:02.000000 sml2mqtt-2.2/src/sml2mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-31 05:13:02.000000 sml2mqtt-2.2/src/sml2mqtt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-31 05:13:02.000000 sml2mqtt-2.2/src/sml2mqtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-31 05:13:02.000000 sml2mqtt-2.2/src/sml2mqtt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:13:02.288910 sml2mqtt-2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-03-31 05:12:48.000000 sml2mqtt-2.2/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-03-31 05:12:48.000000 sml2mqtt-2.2/tests/test_mqtt_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-31 05:12:48.000000 sml2mqtt-2.2/tests/test_readme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:23.820391 sml2mqtt-3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 04:53:10.000000 sml2mqtt-3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 04:53:10.000000 sml2mqtt-3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-24 04:53:23.820391 sml2mqtt-3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-24 04:53:10.000000 sml2mqtt-3.0/requirements_setup.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 04:53:23.820391 sml2mqtt-3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-24 04:53:10.000000 sml2mqtt-3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:23.808391 sml2mqtt-3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:23.812391 sml2mqtt-3.0/src/sml2mqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/__args__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/__log__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:23.812391 sml2mqtt-3.0/src/sml2mqtt/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/config/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/config/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/config/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/config/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/config/mqtt_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11404 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/config/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/config/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:23.816391 sml2mqtt-3.0/src/sml2mqtt/const/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/const/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/const/date_time_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/const/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/const/sml_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/const/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/const/time_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:23.816391 sml2mqtt-3.0/src/sml2mqtt/mqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/mqtt/connect_delay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/mqtt/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/mqtt/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/mqtt/mqtt_obj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:23.816391 sml2mqtt-3.0/src/sml2mqtt/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/runtime/shutdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:23.816391 sml2mqtt-3.0/src/sml2mqtt/sml_device/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_device/device_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_device/setup_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_device/sml_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_device/sml_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_device/watchdog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:23.816391 sml2mqtt-3.0/src/sml2mqtt/sml_source/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_source/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_source/serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_source/setup_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:23.816391 sml2mqtt-3.0/src/sml2mqtt/sml_value/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_value/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_value/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:23.820391 sml2mqtt-3.0/src/sml2mqtt/sml_value/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_value/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_value/operations/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_value/operations/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_value/operations/date_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_value/operations/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_value/operations/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_value/operations/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_value/operations/time_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_value/operations/workarounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_value/setup_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_value/sml_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-24 04:53:10.000000 sml2mqtt-3.0/src/sml2mqtt/sml_value/sml_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:23.820391 sml2mqtt-3.0/src/sml2mqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-24 04:53:23.000000 sml2mqtt-3.0/src/sml2mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-24 04:53:23.000000 sml2mqtt-3.0/src/sml2mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 04:53:23.000000 sml2mqtt-3.0/src/sml2mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-24 04:53:23.000000 sml2mqtt-3.0/src/sml2mqtt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-24 04:53:23.000000 sml2mqtt-3.0/src/sml2mqtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 04:53:23.000000 sml2mqtt-3.0/src/sml2mqtt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:23.820391 sml2mqtt-3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-24 04:53:10.000000 sml2mqtt-3.0/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-24 04:53:10.000000 sml2mqtt-3.0/tests/test_mqtt_obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-24 04:53:10.000000 sml2mqtt-3.0/tests/test_readme.py
```

### Comparing `sml2mqtt-2.2/LICENSE` & `sml2mqtt-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sml2mqtt-2.2/setup.py` & `sml2mqtt-3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-import typing
+from __future__ import annotations
+
 from pathlib import Path
 
 import setuptools  # type: ignore
 
 
 # Load version number without importing HABApp
 def load_version() -> str:
-    version: typing.Dict[str, str] = {}
+    version: dict[str, str] = {}
     with open("src/sml2mqtt/__version__.py") as fp:
         exec(fp.read(), version)
     assert version['__version__'], version
     return version['__version__']
 
 
-def load_req() -> typing.List[str]:
+def load_req() -> list[str]:
     req_file = Path(__file__).with_name('requirements_setup.txt')
     with req_file.open() as f:
         return f.readlines()
 
 
 __version__ = load_version()
 
@@ -32,39 +33,41 @@
         long_description = fh.read()
 
 setuptools.setup(
     name="sml2mqtt",
     version=__version__,
     author="spaceman_spiff",
     # author_email="",
-    description="A sml (Smart Message Language) to MQTT bridge",
+    description="A sml (Smart Message Language) energy meter to MQTT bridge. "
+                "Can read from serial ports or http (e.g. Tibber Pulse).",
     keywords=[
         'mqtt',
         'sml',
         'Smart Message Language',
-        'energy meter'
+        'energy meter',
+        'tibber'
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/spacemanspiff2007/sml2mqtt",
     project_urls={
         'GitHub': 'https://github.com/spacemanspiff2007/sml2mqtt',
     },
     packages=setuptools.find_packages(where='src', exclude=['tests*']),
     package_dir={'': 'src'},
-    python_requires='>=3.8',
+    python_requires='>=3.10',
     install_requires=load_req(),
     classifiers=[
         "Development Status :: 4 - Beta",
         "Framework :: AsyncIO",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Home Automation"
     ],
     entry_points={
         'console_scripts': [
             'sml2mqtt = sml2mqtt.__main__:main'
         ]
```

### Comparing `sml2mqtt-2.2/src/sml2mqtt/__args__.py` & `sml2mqtt-3.0/src/sml2mqtt/__args__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 import argparse
 import os
 import sys
 from pathlib import Path
-from typing import Final, Optional, Type
+from typing import Final
 
 
 class CommandArgs:
-    config: Optional[Path] = None
+    config: Path | None = None
     analyze: bool = False
 
 
 CMD_ARGS: Final = CommandArgs
 
 
-def get_command_line_args(args=None) -> Type[CommandArgs]:
+def get_command_line_args(args=None) -> type[CommandArgs]:
+
+    env_var_name = 'SML2MQTT_ANALYZE'
 
     parser = argparse.ArgumentParser(description='SML to MQTT bridge')
     parser.add_argument(
         '-c',
         '--config',
         help='Path to configuration file',
         default=None
     )
     parser.add_argument(
         '-a',
         '--analyze',
-        help='Process exactly one sml message, shows the values of the message and what will be reported',
+        help='Process exactly one sml message, shows the values of the message and what will be reported. '
+             f'Can also be set by setting the environment variable "{env_var_name:s}" to an arbitrary value',
         action='store_true',
         default=False
     )
     args = parser.parse_args(args)
     CMD_ARGS.config = find_config_folder(args.config)
-    CMD_ARGS.analyze = args.analyze
+    CMD_ARGS.analyze = args.analyze or bool(os.environ.get(env_var_name, ''))
+
     return CMD_ARGS
 
 
-def find_config_folder(config_file_str: Optional[str]) -> Path:
+def find_config_folder(config_file_str: str | None) -> Path:
     check_path = []
 
     if config_file_str is None:
         # Nothing is specified, we try to find the config automatically
         try:
-            working_dir = Path(os.getcwd())
+            working_dir = Path.cwd()
             check_path.append(working_dir / 'sml2mqtt')
             check_path.append(working_dir.with_name('sml2mqtt'))
             check_path.append(working_dir.parent.with_name('sml2mqtt'))
         except ValueError:
             # the ValueError gets raised if the working_dir or its parent is empty (e.g. c:\ or /)
             pass
```

### Comparing `sml2mqtt-2.2/src/sml2mqtt/__log__.py` & `sml2mqtt-3.0/src/sml2mqtt/__log__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
 import sys
 from datetime import date, datetime
 from logging.handlers import RotatingFileHandler
+from pathlib import Path
 
 import sml2mqtt
 
+
 log = logging.getLogger('sml')
 
 
 def get_logger(suffix: str) -> logging.Logger:
     if not suffix:
         return log
     return log.getChild(suffix)
@@ -16,40 +18,45 @@
 
 class MidnightRotatingFileHandler(RotatingFileHandler):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.last_check: date = datetime.now().date()
 
-    def shouldRollover(self, record):   # noqa: N802
-        date = datetime.now().date()
-        if date == self.last_check:
+    def shouldRollover(self, record) -> int:
+        if (date_now := datetime.now().date()) == self.last_check:
             return 0
-        self.last_check = date
+        self.last_check = date_now
         return super().shouldRollover(record)
 
 
 def setup_log():
     level = sml2mqtt.CONFIG.logging.set_log_level()
 
     # This is the longest logger name str
     chars = 0
-    for device in sml2mqtt.CONFIG.ports:
-        chars = max(len(f'sml.device.{device.url}'), chars)
+    for device in sml2mqtt.CONFIG.inputs:
+        # Name of the longest logger, should be the device status
+        chars = max(len(get_logger(device.get_device_name()).getChild('status').name), chars)
     log_format = logging.Formatter("[{asctime:s}] [{name:" + str(chars) + "s}] {levelname:8s} | {message:s}", style='{')
 
     # File Handler
-    log_file = sml2mqtt.CONFIG.logging.file
-    if not log_file.is_absolute():
-        log_file = sml2mqtt.CMD_ARGS.config.parent / log_file
-        log_file.resolve()
-
-    handler = MidnightRotatingFileHandler(
-        str(log_file), maxBytes=1024 * 1024, backupCount=3, encoding='utf-8'
-    )
+    file_path = sml2mqtt.CONFIG.logging.file
+    if file_path.lower() == 'stdout':
+        handler = logging.StreamHandler(sys.stdout)
+    else:
+        log_file = Path(file_path)
+        if not log_file.is_absolute():
+            log_file = sml2mqtt.CMD_ARGS.config.parent / log_file
+            log_file.resolve()
+
+        handler = MidnightRotatingFileHandler(
+            str(log_file), maxBytes=1024 * 1024, backupCount=3, encoding='utf-8'
+        )
+
     handler.setFormatter(log_format)
     handler.setLevel(logging.DEBUG)
 
     # Bind handler to logger
     root_log = logging.getLogger()
     root_log.addHandler(handler)
```

### Comparing `sml2mqtt-2.2/src/sml2mqtt/config/config.py` & `sml2mqtt-3.0/src/sml2mqtt/config/inputs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,107 +1,114 @@
-from typing import Dict, List, Union
+from typing import Literal
 
 import serial
-from easyconfig import AppBaseModel, BaseModel, create_app_config
-from pydantic import constr, Field, StrictFloat, StrictInt, StrictStr, validator
+from aiohttp import ClientTimeout
+from easyconfig import BaseModel
+from pydantic import (
+    AnyHttpUrl,
+    Field,
+    StrictFloat,
+    StrictInt,
+    constr,
+    field_validator,
+    model_validator,
+)
+from typing_extensions import override
+
+from sml2mqtt.config.types import log
+
+
+class SmlSourceSettingsBase(BaseModel):
+    def get_device_name(self) -> str:
+        raise NotImplementedError()
 
-from .device import REPUBLISH_ALIAS, SmlDeviceConfig, SmlValueConfig
-from .logging import LoggingSettings
-from .mqtt import MqttConfig, OptionalMqttPublishConfig
 
+class SerialSourceSettings(SmlSourceSettingsBase):
+    type: Literal['serial']
 
-class PortSettings(BaseModel):
     url: constr(strip_whitespace=True, min_length=1, strict=True) = Field(..., description='Device path')
-    timeout: Union[int, float] = Field(
-        default=3, description='Seconds after which a timeout will be detected (default=3)')
+    timeout: StrictInt | StrictFloat = Field(
+        default=6, description='Seconds after which a timeout will be detected (default=6)')
 
     baudrate: int = Field(9600, in_file=False)
     parity: str = Field('None', in_file=False)
-    stopbits: Union[StrictInt, StrictFloat] = Field(serial.STOPBITS_ONE, in_file=False, alias='stop bits')
+    stopbits: StrictInt | StrictFloat = Field(serial.STOPBITS_ONE, in_file=False, alias='stop bits')
     bytesize: int = Field(serial.EIGHTBITS, in_file=False, alias='byte size')
 
-    @validator('baudrate')
+    @field_validator('baudrate')
     def _val_baudrate(cls, v):
         if v not in serial.Serial.BAUDRATES:
-            raise ValueError(f'must be one of {list(serial.Serial.BAUDRATES)}')
+            msg = f'must be one of {list(serial.Serial.BAUDRATES)}'
+            raise ValueError(msg)
         return v
 
-    @validator('parity')
+    @field_validator('parity')
     def _val_parity(cls, v):
         # Short name
         if v in serial.PARITY_NAMES:
             return v
 
         # Name -> Short name
         parity_values = {_n: _v for _v, _n in serial.PARITY_NAMES.items()}
         if v not in parity_values:
-            raise ValueError(f'must be one of {list(parity_values)}')
+            msg = f'must be one of {list(parity_values)}'
+            raise ValueError(msg)
         return parity_values[v]
 
-    @validator('stopbits')
+    @field_validator('stopbits')
     def _val_stopbits(cls, v):
         if v not in serial.Serial.STOPBITS:
-            raise ValueError(f'must be one of {list(serial.Serial.STOPBITS)}')
+            msg = f'must be one of {list(serial.Serial.STOPBITS)}'
+            raise ValueError(msg)
         return v
 
-    @validator('bytesize')
+    @field_validator('bytesize')
     def _val_bytesize(cls, v):
         if v not in serial.Serial.BYTESIZES:
-            raise ValueError(f'must be one of {list(serial.Serial.BYTESIZES)}')
+            msg = f'must be one of {list(serial.Serial.BYTESIZES)}'
+            raise ValueError(msg)
         return v
 
+    @override
+    def get_device_name(self) -> str:
+        return self.url.split("/")[-1]
 
-class GeneralSettings(BaseModel):
-    wh_in_kwh: bool = Field(True, description='Automatically convert Wh to kWh', alias='Wh in kWh')
-    republish_after: int = Field(
-        120, description='Republish automatically after this time (if no other filter configured)',
-        alias=REPUBLISH_ALIAS,
-    )
-    report_blank_energy_meters: bool = Field(
-        False, description='Report blank energy meters (where the value is 0kwh)',
-        alias='report blank energy meters', in_file=False
-    )
-    report_device_id: bool = Field(
-        False, description='Report the device id even though it does never change',
-        alias='report device id', in_file=False
-    )
-    device_id_obis: List[StrictStr] = Field(
-        # 0100000009ff (1-0:0.0.9*255) : Geräteeinzelidentifikation
-        # 0100600100ff (1-0:96.1.0*255): Produktionsnummer
-        ['0100000009ff', '0100600100ff'],
-        description='Additional OBIS fields for the serial number to configuration matching',
-        alias='device id obis', in_file=False
-    )
 
+class HttpSourceSettings(SmlSourceSettingsBase):
+    type: Literal['http']
 
-class Settings(AppBaseModel):
-    logging: LoggingSettings = Field(default_factory=LoggingSettings)
-    mqtt: MqttConfig = Field(default_factory=MqttConfig)
-    general: GeneralSettings = Field(default_factory=GeneralSettings)
-    ports: List[PortSettings] = []
-    devices: Dict[str, SmlDeviceConfig] = Field({}, description='Device configuration by ID or url',)
-
-
-def default_config() -> Settings:
-    # File defaults
-    s = Settings(
-        ports=[PortSettings(url='COM1', timeout=3), PortSettings(url='/dev/ttyS0', timeout=3), ],
-        devices={
-            'DEVICE_ID_HEX': SmlDeviceConfig(
-                mqtt=OptionalMqttPublishConfig(topic='DEVICE_BASE_TOPIC'),
-                status=OptionalMqttPublishConfig(topic='status'),
-                skip=['OBIS'],
-                values={
-                    'OBIS': SmlValueConfig(
-                        mqtt=OptionalMqttPublishConfig(topic='OBIS'),
-                        workarounds=[{'negative on energy meter status': True}],
-                        transformations=[{'factor': 3}, {'offset': 100}, {'round': 2}],
-                        filters=[{'diff': 10}, {'perc': 10}, {'every': 120}],
-                    )
-                }
-            )
-        }
-    )
-    return s
+    url: AnyHttpUrl = Field(..., description='Url')
+    timeout: StrictInt | StrictFloat = Field(
+        default=6, description='Seconds after which a timeout will be detected (default=6)')
+
+    interval: StrictInt | StrictFloat = Field(default=2, description='Delay between requests', ge=0.1)
+    user: str = Field(default='', description='User (if needed)')
+    password: str = Field(default='', description='Password (if needed)')
 
+    request_timeout: StrictInt | StrictFloat | None = Field(
+        default=None, alias='request timeout', description='Dedicated timeout for the http request',
+        in_file=False
+    )
 
-CONFIG: Settings = create_app_config(Settings(), default_config)
+    @override
+    def get_device_name(self) -> str:
+        return self.url.host
+
+    @model_validator(mode='after')
+    def check_timeout_gt_interval(self):
+        if self.interval * 2 > self.timeout:
+            msg = 'Timeout must be greater equal than 2 * interval'
+            raise ValueError(msg)
+
+        # Timeout is interval, and we automatically retry 3 times before we fail
+        if self.interval * 3 > self.timeout:
+            log.warning(f'The recommendation for timeout is at least 3 * interval '
+                        f'({self.interval * 3:.0f})! Currently: {self.timeout}')
+
+        return self
+
+    def get_request_timeout(self) -> ClientTimeout:
+        value = self.interval if self.request_timeout is None else self.request_timeout
+        if value is None:
+            msg = 'No value for ClientTimeout'
+            raise ValueError(msg)
+        return ClientTimeout(total=value)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sml2mqtt-2.2/src/sml2mqtt/config/mqtt.py` & `sml2mqtt-3.0/src/sml2mqtt/config/mqtt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,67 @@
+import random
+import string
+
 from easyconfig import BaseModel
-from pydantic import conint, constr, Field, StrictBool, validator
+from pydantic import Field, StrictBool, field_validator, model_validator
 
-QOS = conint(ge=0, le=2)
-TOPIC_STR = constr(strip_whitespace=True, min_length=1)
-STRIPPED_STR = constr(strip_whitespace=True)
+from sml2mqtt.config.mqtt_tls import MqttTlsOptions
+from sml2mqtt.config.types import MqttQosInt, MqttTopicStr, StrippedStr
 
 
 class MqttDefaultPublishConfig(BaseModel):
-    qos: QOS = Field(
-        0, description='Default value for QOS if no other QOS value in the config entry is set')
+    qos: MqttQosInt = Field(
+        0, description='Default value for QoS if no other QoS value in the config entry is set')
     retain: StrictBool = Field(
         False, description='Default value for retain if no other retain value in the config entry is set')
 
 
 class OptionalMqttPublishConfig(BaseModel):
-    topic: TOPIC_STR = Field(None, description='Topic fragment for building this topic with the parent topic')
-    full_topic: TOPIC_STR = Field(
+    topic: MqttTopicStr | None = Field(
+        None, description='Topic fragment for building this topic with the parent topic')
+    full_topic: MqttTopicStr | None = Field(
         None, alias='full topic', description='Full topic - will ignore the parent topic parts')
-    qos: QOS = Field(None, description='QoS for publishing this value (if set - otherwise use parent)')
-    retain: StrictBool = Field(None, description='Retain for publishing this value (if set - otherwise use parent)')
+    qos: MqttQosInt | None = Field(
+        None, description='QoS for publishing this value (if set - otherwise use parent)')
+    retain: StrictBool | None = Field(
+        None, description='Retain for publishing this value (if set - otherwise use parent)')
 
-    @validator('topic', 'full_topic')
+    @field_validator('topic', 'full_topic')
     def validate_topic(cls, value):
         if value is None:
             return None
 
         if value.endswith('/'):
-            raise ValueError('Topic must not end with "/"')
+            msg = 'Topic must not end with "/"'
+            raise ValueError(msg)
         if value.startswith('/'):
-            raise ValueError('Topic must not start with "/"')
+            msg = 'Topic must not start with "/"'
+            raise ValueError(msg)
         return value
 
-    @validator('full_topic')
-    def check_full_or_partial(cls, v, values):
-        if v is None:
-            return None
-
-        if values.get('topic') is not None:
-            raise ValueError('Topic and full_topic can not be used at the same time!')
-        return v
+    @model_validator(mode='after')
+    def check_full_or_partial(self):
+        if self.topic is not None and self.full_topic is not None:
+            msg = 'Topic and full_topic can not be used at the same time!'
+            raise ValueError(msg)
+        return self
 
 
 class MqttConnection(BaseModel):
-    client_id: STRIPPED_STR = Field('sml2mqtt', alias='client id')
-    host: STRIPPED_STR = 'localhost'
-    port: conint(gt=0) = 1883
-    user: STRIPPED_STR = ''
-    password: STRIPPED_STR = ''
-    tls: StrictBool = False
-    tls_insecure: StrictBool = Field(False, alias='tls insecure')
+    identifier: StrippedStr = Field('sml2mqtt-' + ''.join(random.choices(string.ascii_letters, k=13)),)
+    host: StrippedStr = 'localhost'
+    port: int = Field(1883, ge=0)
+    user: StrippedStr = ''
+    password: StrippedStr = ''
+
+    tls: MqttTlsOptions | None = Field(None)
 
 
 class MqttConfig(BaseModel):
-    connection: MqttConnection = Field(default_factory=MqttConnection)
-    topic: TOPIC_STR = Field('sml2mqtt', alias='topic prefix')
-    defaults: MqttDefaultPublishConfig = Field(default_factory=MqttDefaultPublishConfig)
+    connection: MqttConnection = Field(
+        default_factory=MqttConnection)
+    topic: StrippedStr = Field(
+        'sml2mqtt', alias='topic prefix', description='Prefix for all topics. Set to empty string to disable')
+    defaults: MqttDefaultPublishConfig = Field(
+        default_factory=MqttDefaultPublishConfig)
     last_will: OptionalMqttPublishConfig = Field(
         default_factory=lambda: OptionalMqttPublishConfig(topic='status'), alias='last will')
```

### Comparing `sml2mqtt-2.2/src/sml2mqtt/mqtt/connect_delay.py` & `sml2mqtt-3.0/src/sml2mqtt/mqtt/connect_delay.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from asyncio import sleep
-from typing import Optional
 
 
 class DynDelay:
-    def __init__(self, min_delay: float, max_delay: float, start_delay: Optional[float] = None):
+    def __init__(self, min_delay: float, max_delay: float, start_delay: float | None = None):
         if min_delay < 0:
-            raise ValueError(f'min_delay must be >= 0: {min_delay}')
+            msg = f'min_delay must be >= 0: {min_delay}'
+            raise ValueError(msg)
         if max_delay <= min_delay:
-            raise ValueError(f'max_delay must be >= min_delay: {max_delay}')
+            msg = f'max_delay must be >= min_delay: {max_delay}'
+            raise ValueError(msg)
 
         self.min = min_delay
         self.max = max_delay
 
         if start_delay is None:
             start_delay = min_delay
```

### Comparing `sml2mqtt-2.2/src/sml2mqtt/mqtt/mqtt.py` & `sml2mqtt-3.0/src/sml2mqtt/mqtt/mqtt.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,134 +1,131 @@
 import traceback
-from asyncio import CancelledError, create_task, Event, Queue, Task, TimeoutError, wait_for
-from typing import Final, Optional, Union
+from asyncio import CancelledError, Event, Queue, TimeoutError, wait_for
+from typing import Final
 
-from asyncio_mqtt import Client, MqttError, Will
+from aiomqtt import Client, MqttError, Will
 
 import sml2mqtt
 from sml2mqtt.__log__ import log as _parent_logger
+from sml2mqtt.const import Task
 from sml2mqtt.errors import InitialMqttConnectionFailedError
 from sml2mqtt.mqtt import DynDelay
+from sml2mqtt.runtime import on_shutdown
 
-log = _parent_logger.getChild('mqtt')
 
+log = _parent_logger.getChild('mqtt')
 
-TASK: Optional[Task] = None
-IS_CONNECTED: Optional[Event] = None
 
+TASK: Task | None = None
+IS_CONNECTED: Event | None = None
 
-def start():
-    global TASK, IS_CONNECTED
 
-    IS_CONNECTED = Event()
+async def start():
+    global IS_CONNECTED, TASK
 
     assert TASK is None
-    TASK = create_task(mqtt_task(), name='MQTT Task')
 
+    IS_CONNECTED = Event()
+    TASK = Task(_mqtt_task, name='MQTT Task')
 
-def cancel():
-    global TASK
-    if TASK is not None:
-        TASK.cancel()
-        TASK = None
+    on_shutdown(TASK.cancel_and_wait, 'Shutdown mqtt')
+    TASK.start()
 
 
 async def wait_for_connect(timeout: float):
     if IS_CONNECTED is None:
-        return None
+        raise ValueError()
 
     try:
         await wait_for(IS_CONNECTED.wait(), timeout)
     except TimeoutError:
         log.error('Initial mqtt connection failed!')
         raise InitialMqttConnectionFailedError() from None
 
     return None
 
 
-async def wait_for_disconnect():
-    if TASK is None:
-        return None
-
-    await TASK
-
-
-QUEUE: Optional[Queue] = None
-
-
-async def mqtt_task():
-    try:
-        await _mqtt_task()
-    finally:
-        log.debug('Task finished')
+QUEUE: Queue[tuple[str, int | float | str | bytes, int, bool]] | None = None
 
 
-async def _mqtt_task():
+async def _mqtt_task() -> None:
     global QUEUE
 
     from .mqtt_obj import BASE_TOPIC
     config = sml2mqtt.config.CONFIG
 
     cfg_connection = config.mqtt.connection
 
     delay = DynDelay(0, 300)
 
-    payload_offline: Final = 'OFFLINE'
     payload_online: Final = 'ONLINE'
+    payload_offline: Final = 'OFFLINE'
 
     shutdown = False
 
     while not shutdown:
         await delay.wait()
 
         try:
             # since we just pass this into the mqtt wrapper we do not link it to the base topic
-            will_topic = BASE_TOPIC.create_child(
-                topic_fragment=config.mqtt.last_will.topic).set_config(config.mqtt.last_will)
+            will_topic = BASE_TOPIC.create_child(topic_fragment='status').set_config(config.mqtt.last_will)
+
+            will = Will(
+                topic=will_topic.topic, payload=payload_offline,
+                qos=will_topic.qos, retain=will_topic.retain
+            )
+
+            tls_kwargs = {} if cfg_connection.tls is None else cfg_connection.tls.get_client_kwargs(log)
 
             client = Client(
-                hostname=cfg_connection.host,
-                port=cfg_connection.port,
+                hostname=cfg_connection.host, port=cfg_connection.port,
+
                 username=cfg_connection.user if cfg_connection.user else None,
                 password=cfg_connection.password if cfg_connection.password else None,
-                will=Will(will_topic.topic, payload=payload_offline, qos=will_topic.qos, retain=will_topic.retain),
-                client_id=cfg_connection.client_id
+                will=will,
+                identifier=cfg_connection.identifier,
+
+                **tls_kwargs
             )
 
             log.debug(f'Connecting to {cfg_connection.host}:{cfg_connection.port}')
 
             async with client:
                 log.debug('Success!')
                 delay.reset()
                 QUEUE = Queue()
                 IS_CONNECTED.set()
 
                 try:
                     # signal that we are online
-                    await client.publish(will_topic.topic, payload_online, will_topic.qos, will_topic.retain)
+                    await client.publish(will.topic, payload_online, will.qos, will.retain)
 
                     # worker to publish things
                     while True:
                         topic, value, qos, retain = await QUEUE.get()
                         await client.publish(topic, value, qos, retain)
                         QUEUE.task_done()
+
                 except CancelledError:
                     # The last will testament only gets sent on abnormal disconnect
                     # Since we disconnect gracefully we have to manually sent the offline status
-                    await client.publish(will_topic.topic, payload_offline, will_topic.qos, will_topic.retain)
+                    await client.publish(will.topic, will.payload, will.qos, will.retain)
                     shutdown = True
+                    log.debug('Disconnecting')
 
         except MqttError as e:
             delay.increase()
             log.error(f'{e} ({e.__class__.__name__})')
+
         except Exception:
             delay.increase()
             for line in traceback.format_exc().splitlines():
                 log.error(line)
+
         finally:
             QUEUE = None
             IS_CONNECTED.clear()
 
 
-def publish(topic: str, value: Union[int, float, str], qos: int, retain: bool):
+def publish(topic: str, value: int | float | str | bytes, qos: int, retain: bool):
     if QUEUE is not None:
         QUEUE.put_nowait((topic, value, qos, retain))
```

### Comparing `sml2mqtt-2.2/src/sml2mqtt/mqtt/mqtt_obj.py` & `sml2mqtt-3.0/src/sml2mqtt/mqtt/mqtt_obj.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,60 @@
 import dataclasses
-from typing import Any, Callable, Final, List, Optional, Union
+from collections.abc import Callable, Generator
+from typing import Any, Final
 
 from sml2mqtt.__log__ import get_logger
 from sml2mqtt.config import OptionalMqttPublishConfig
 from sml2mqtt.mqtt import publish
 
-from .errors import MqttConfigValuesMissingError, TopicFragmentExpectedError
+from .errors import MqttConfigValuesMissingError, MqttTopicEmpty, TopicFragmentExpectedError
 
-pub_func: Callable[[str, Union[int, float, str], int, bool], Any] = publish
 
+pub_func: Callable[[str, int | float | str, int, bool], Any] = publish
 
-def publish_analyze(topic: str, value: Union[int, float, str], qos: int, retain: bool):
+
+def publish_analyze(topic: str, value: int | float | str, qos: int, retain: bool):
     get_logger('mqtt.pub').info(f'{topic}: {value} (QOS: {qos}, retain: {retain})')
 
 
+def patch_analyze():
+    global pub_func
+
+    pub_func = publish_analyze
+
+
 @dataclasses.dataclass
 class MqttCfg:
-    topic_full: Optional[str] = None
-    topic_fragment: Optional[str] = None
-    qos: Optional[int] = None
-    retain: Optional[bool] = None
+    topic_full: str | None = None
+    topic_fragment: str | None = None
+    qos: int | None = None
+    retain: bool | None = None
 
-    def set_config(self, config: Optional[OptionalMqttPublishConfig]):
+    def set_config(self, config: OptionalMqttPublishConfig):
         self.topic_full = config.full_topic
         self.topic_fragment = config.topic
         self.qos = config.qos
         self.retain = config.retain
 
 
 class MqttObj:
-    def __init__(self, topic_fragment: Optional[str] = None, qos: Optional[int] = None, retain: Optional[bool] = None):
+    def __init__(self, topic_fragment: str | None = None, qos: int | None = None, retain: bool | None = None):
 
         # Configured parts
         self.cfg = MqttCfg(topic_fragment=topic_fragment, qos=qos, retain=retain)
 
         # Effective config
         self.qos: int = 0
         self.retain: bool = False
         self.topic: str = ''
 
-        self.parent: Optional[MqttObj] = None
-        self.children: List[MqttObj] = []
+        self.parent: MqttObj | None = None
+        self.children: list[MqttObj] = []
 
-    def publish(self, value: Union[str, int, float, bytes]):
+    def publish(self, value: str | int | float):
         pub_func(self.topic, value, self.qos, self.retain)
 
     def update(self) -> 'MqttObj':
         self._merge_values()
         for c in self.children:
             c.update()
         return self
@@ -65,56 +73,75 @@
 
         # effective topic
         if self.cfg.topic_full:
             self.topic = self.cfg.topic_full
         else:
             if not self.cfg.topic_fragment:
                 raise TopicFragmentExpectedError()
-            self.topic = f'{self.parent.topic}/{self.cfg.topic_fragment}'
+
+            # The topmost topic may be empty
+            parts = []
+            if self.parent.topic:
+                parts.append(self.parent.topic)
+            if self.cfg.topic_fragment:
+                parts.append(self.cfg.topic_fragment)
+            self.topic = '/'.join(parts)
+
+            if not self.topic:
+                raise MqttTopicEmpty()
 
         # effective QOS
         self.qos = self.cfg.qos
         if self.qos is None:
             self.qos = self.parent.qos
 
         # effective retain
         self.retain = self.cfg.retain
         if self.retain is None:
             self.retain = self.parent.retain
         return self
 
-    def set_topic(self, topic: str) -> 'MqttObj':
+    def set_topic(self, topic: str | None) -> 'MqttObj':
         self.cfg.topic_fragment = topic
         self.update()
         return self
 
-    def set_config(self, cfg: Optional[OptionalMqttPublishConfig]) -> 'MqttObj':
+    def set_config(self, cfg: OptionalMqttPublishConfig | None) -> 'MqttObj':
         if cfg is None:
             return self
 
         self.cfg.set_config(cfg)
         self.update()
         return self
 
-    def create_child(self, topic_fragment: Optional[str] = None, qos: Optional[int] = None,
-                     retain: Optional[bool] = None) -> 'MqttObj':
+    def create_child(self, topic_fragment: str | None = None, qos: int | None = None,
+                     retain: bool | None = None) -> 'MqttObj':
         child = self.__class__(topic_fragment=topic_fragment, qos=qos, retain=retain)
         child.parent = self
         self.children.append(child)
         child.update()
         return child
 
+    def iter_objs(self) -> Generator['MqttObj', Any, None]:
+        yield self
+        for child in self.children:
+            yield from child.iter_objs()
+
 
 BASE_TOPIC: Final = MqttObj()
 
 
 def setup_base_topic(topic: str, qos: int, retain: bool):
     BASE_TOPIC.cfg.topic_fragment = topic
     BASE_TOPIC.cfg.qos = qos
     BASE_TOPIC.cfg.retain = retain
     BASE_TOPIC.update()
 
 
-def patch_analyze():
-    global pub_func
+def check_for_duplicate_topics(obj: MqttObj):
+    log = get_logger('mqtt')
 
-    pub_func = publish_analyze
+    topics: set[str] = set()
+    for o in obj.iter_objs():
+        if (topic := o.topic) in topics:
+            log.warning(f'Topic "{topic:s}" is already configured!')
+        topics.add(topic)
```

### Comparing `sml2mqtt-2.2/src/sml2mqtt/sml_value/filter/diff.py` & `sml2mqtt-3.0/src/sml2mqtt/sml_value/operations/operations.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,43 @@
-from typing import Final, Union
+from collections.abc import Generator
 
-from .base import FilterBase, VALUE_TYPE
+from typing_extensions import override
 
+from sml2mqtt.sml_value.base import OperationContainerBase, SmlValueInfo, ValueOperationBase
 
-class DiffFilterBase(FilterBase):
-    def __init__(self, min_diff: Union[int, float]):
-        if min_diff < 0:
-            raise ValueError('min diff must be >= 0')
-        self.min_diff: Final = min_diff
-        self.last_value: VALUE_TYPE = None
 
-    def required(self, value: VALUE_TYPE) -> VALUE_TYPE:
-        if value is None:
-            return False
-        if self.last_value is None:
-            return True
-        return self.diff(value)
+class OrOperation(ValueOperationBase, OperationContainerBase):
 
-    def done(self, value):
-        self.last_value = value
+    @override
+    def process_value(self, value: float | None, info: SmlValueInfo) -> float | None:
+        ret: float | None = None
+        for op in self.operations:
+            if (call := op.process_value(value, info)) is not None and ret is None:
+                ret = call
 
-    def diff(self, value: Union[int, float]) -> VALUE_TYPE:
-        raise NotImplementedError()
-
-
-class DiffAbsFilter(DiffFilterBase):
-    def diff(self, value: Union[int, float]) -> VALUE_TYPE:
-        if abs(value - self.last_value) < self.min_diff:
-            return False
-        return True
+        return ret
 
     def __repr__(self):
-        return f'<AbsDiff: {self.min_diff}>'
+        return f'<Or at 0x{id(self):x}>'
 
+    @override
+    def describe(self, indent: str = '') -> Generator[str, None, None]:
+        yield f'{indent:s}- Or:'
+        for o in self.operations:
+            yield from o.describe(indent + '  ')
 
-class DiffPercFilter(DiffFilterBase):
-    def diff(self, value: Union[int, float]) -> VALUE_TYPE:
-        if not self.last_value:
-            return False
-
-        perc = abs(1 - value / self.last_value) * 100
-        if perc < self.min_diff:
-            return False
-        return True
+
+class SequenceOperation(ValueOperationBase, OperationContainerBase):
+    @override
+    def process_value(self, value: float | None, info: SmlValueInfo) -> float | None:
+        for op in self.operations:
+            value = op.process_value(value, info)
+        return value
 
     def __repr__(self):
-        return f'<PercDiff: {self.min_diff}>'
+        return f'<Sequence at 0x{id(self):x}>'
+
+    @override
+    def describe(self, indent: str = '') -> Generator[str, None, None]:
+        yield f'{indent:s}- Sequence:'
+        for o in self.operations:
+            yield from o.describe(indent + '  ')
```

### Comparing `sml2mqtt-2.2/src/sml2mqtt.egg-info/SOURCES.txt` & `sml2mqtt-3.0/src/sml2mqtt.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -2,50 +2,64 @@
 MANIFEST.in
 requirements_setup.txt
 setup.py
 src/sml2mqtt/__args__.py
 src/sml2mqtt/__init__.py
 src/sml2mqtt/__log__.py
 src/sml2mqtt/__main__.py
-src/sml2mqtt/__shutdown__.py
 src/sml2mqtt/__version__.py
 src/sml2mqtt/errors.py
 src/sml2mqtt.egg-info/PKG-INFO
 src/sml2mqtt.egg-info/SOURCES.txt
 src/sml2mqtt.egg-info/dependency_links.txt
 src/sml2mqtt.egg-info/entry_points.txt
 src/sml2mqtt.egg-info/requires.txt
 src/sml2mqtt.egg-info/top_level.txt
 src/sml2mqtt/config/__init__.py
 src/sml2mqtt/config/config.py
 src/sml2mqtt/config/device.py
+src/sml2mqtt/config/inputs.py
 src/sml2mqtt/config/logging.py
 src/sml2mqtt/config/mqtt.py
-src/sml2mqtt/device/__init__.py
-src/sml2mqtt/device/sml_device.py
-src/sml2mqtt/device/sml_device_status.py
-src/sml2mqtt/device/sml_serial.py
-src/sml2mqtt/device/sml_value_group.py
-src/sml2mqtt/device/watchdog.py
+src/sml2mqtt/config/mqtt_tls.py
+src/sml2mqtt/config/operations.py
+src/sml2mqtt/config/types.py
+src/sml2mqtt/const/__init__.py
+src/sml2mqtt/const/date_time_finder.py
+src/sml2mqtt/const/protocols.py
+src/sml2mqtt/const/sml_helpers.py
+src/sml2mqtt/const/task.py
+src/sml2mqtt/const/time_series.py
 src/sml2mqtt/mqtt/__init__.py
 src/sml2mqtt/mqtt/connect_delay.py
 src/sml2mqtt/mqtt/errors.py
 src/sml2mqtt/mqtt/mqtt.py
 src/sml2mqtt/mqtt/mqtt_obj.py
+src/sml2mqtt/runtime/__init__.py
+src/sml2mqtt/runtime/shutdown.py
+src/sml2mqtt/sml_device/__init__.py
+src/sml2mqtt/sml_device/device_status.py
+src/sml2mqtt/sml_device/setup_device.py
+src/sml2mqtt/sml_device/sml_device.py
+src/sml2mqtt/sml_device/sml_devices.py
+src/sml2mqtt/sml_device/watchdog.py
+src/sml2mqtt/sml_source/__init__.py
+src/sml2mqtt/sml_source/http.py
+src/sml2mqtt/sml_source/serial.py
+src/sml2mqtt/sml_source/setup_source.py
 src/sml2mqtt/sml_value/__init__.py
-src/sml2mqtt/sml_value/__types__.py
-src/sml2mqtt/sml_value/enum_builder.py
+src/sml2mqtt/sml_value/base.py
+src/sml2mqtt/sml_value/setup_operations.py
 src/sml2mqtt/sml_value/sml_value.py
-src/sml2mqtt/sml_value/filter/__init__.py
-src/sml2mqtt/sml_value/filter/base.py
-src/sml2mqtt/sml_value/filter/change.py
-src/sml2mqtt/sml_value/filter/diff.py
-src/sml2mqtt/sml_value/filter/time.py
-src/sml2mqtt/sml_value/transformations/__init__.py
-src/sml2mqtt/sml_value/transformations/base.py
-src/sml2mqtt/sml_value/transformations/math.py
-src/sml2mqtt/sml_value/workarounds/__init__.py
-src/sml2mqtt/sml_value/workarounds/base.py
-src/sml2mqtt/sml_value/workarounds/negative_on_energy_status.py
+src/sml2mqtt/sml_value/sml_values.py
+src/sml2mqtt/sml_value/operations/__init__.py
+src/sml2mqtt/sml_value/operations/_helper.py
+src/sml2mqtt/sml_value/operations/actions.py
+src/sml2mqtt/sml_value/operations/date_time.py
+src/sml2mqtt/sml_value/operations/filter.py
+src/sml2mqtt/sml_value/operations/math.py
+src/sml2mqtt/sml_value/operations/operations.py
+src/sml2mqtt/sml_value/operations/time_series.py
+src/sml2mqtt/sml_value/operations/workarounds.py
 tests/test_docs.py
 tests/test_mqtt_obj.py
 tests/test_readme.py
```

