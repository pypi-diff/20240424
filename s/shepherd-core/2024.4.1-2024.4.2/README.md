# Comparing `tmp/shepherd_core-2024.4.1.tar.gz` & `tmp/shepherd_core-2024.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shepherd_core-2024.4.1.tar", last modified: Thu Apr 18 13:25:03 2024, max compression
+gzip compressed data, was "shepherd_core-2024.4.2.tar", last modified: Wed Apr 24 19:38:56 2024, max compression
```

## Comparing `shepherd_core-2024.4.1.tar` & `shepherd_core-2024.4.2.tar`

### file list

```diff
@@ -1,89 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.188937 shepherd_core-2024.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-04-18 13:25:03.188937 shepherd_core-2024.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:25:03.188937 shepherd_core-2024.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.176937 shepherd_core-2024.4.1/shepherd_core/
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/calibration_hw_def.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.176937 shepherd_core-2024.4.1/shepherd_core/data_models/
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.176937 shepherd_core-2024.4.1/shepherd_core/data_models/base/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/base/cal_measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/base/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/base/content.py
--rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/base/shepherd.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/base/timezone.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/base/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.180937 shepherd_core-2024.4.1/shepherd_core/data_models/content/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/content/energy_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/content/firmware.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/content/firmware_datatype.py
--rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/content/virtual_harvester.py
--rw-r--r--   0 runner    (1001) docker     (127)    13958 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/content/virtual_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/doc_virtual_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.180937 shepherd_core-2024.4.1/shepherd_core/data_models/experiment/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/experiment/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/experiment/observer_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/experiment/target_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.180937 shepherd_core-2024.4.1/shepherd_core/data_models/task/
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/task/emulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/task/firmware_mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/task/harvest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/task/observer_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/task/programming.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/task/testbed_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.180937 shepherd_core-2024.4.1/shepherd_core/data_models/testbed/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/testbed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/testbed/cape.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/testbed/gpio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/testbed/mcu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/testbed/observer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/testbed/target.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/testbed/testbed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.184937 shepherd_core-2024.4.1/shepherd_core/decoder_waveform/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/decoder_waveform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10672 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/decoder_waveform/uart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.184937 shepherd_core-2024.4.1/shepherd_core/fw_tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/fw_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/fw_tools/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/fw_tools/converter_elf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/fw_tools/patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/fw_tools/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.184937 shepherd_core-2024.4.1/shepherd_core/inventory/
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/inventory/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/inventory/system.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/inventory/target.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    26082 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.184937 shepherd_core-2024.4.1/shepherd_core/testbed_client/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/testbed_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/testbed_client/cache_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/testbed_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/testbed_client/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/testbed_client/user_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.184937 shepherd_core-2024.4.1/shepherd_core/vsource/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/vsource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10332 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/vsource/virtual_converter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7764 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/vsource/virtual_harvester_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/vsource/virtual_source_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14355 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.188937 shepherd_core-2024.4.1/shepherd_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-04-18 13:25:03.000000 shepherd_core-2024.4.1/shepherd_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-18 13:25:03.000000 shepherd_core-2024.4.1/shepherd_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:25:03.000000 shepherd_core-2024.4.1/shepherd_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-18 13:25:03.000000 shepherd_core-2024.4.1/shepherd_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 13:25:03.000000 shepherd_core-2024.4.1/shepherd_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:25:02.000000 shepherd_core-2024.4.1/shepherd_core.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.188937 shepherd_core-2024.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/tests/test_cal_hw.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     9560 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.229001 shepherd_core-2024.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-04-24 19:38:56.229001 shepherd_core-2024.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.205001 shepherd_core-2024.4.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/examples/experiment_from_yaml.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/examples/experiment_generic_var1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/examples/experiment_generic_var2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/examples/experiment_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/examples/firmware_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/examples/firmware_modification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/examples/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/examples/uart_decode_waveform.py
+-rw-r--r--   0 runner    (1001) docker     (127)   229877 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/examples/uart_raw2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/examples/vharvester_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/examples/vsource_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:38:56.229001 shepherd_core-2024.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.205001 shepherd_core-2024.4.2/shepherd_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/calibration_hw_def.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.209001 shepherd_core-2024.4.2/shepherd_core/data_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.209001 shepherd_core-2024.4.2/shepherd_core/data_models/base/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/base/cal_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10320 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/base/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/base/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/base/shepherd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/base/timezone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/base/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.209001 shepherd_core-2024.4.2/shepherd_core/data_models/content/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12259 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/content/_external_fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/content/energy_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/content/energy_environment_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/content/firmware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/content/firmware_datatype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9448 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/content/virtual_harvester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/content/virtual_harvester_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14142 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/content/virtual_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/content/virtual_source_fixture.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.209001 shepherd_core-2024.4.2/shepherd_core/data_models/experiment/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/experiment/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/experiment/observer_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/experiment/target_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.213001 shepherd_core-2024.4.2/shepherd_core/data_models/task/
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/task/emulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/task/firmware_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/task/harvest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/task/observer_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/task/programming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/task/testbed_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.213001 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/cape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/cape_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/gpio_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/mcu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/mcu_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/observer_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/target_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/testbed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/testbed/testbed_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/data_models/virtual_source_doc.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.213001 shepherd_core-2024.4.2/shepherd_core/decoder_waveform/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/decoder_waveform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/decoder_waveform/uart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.217001 shepherd_core-2024.4.2/shepherd_core/fw_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/fw_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/fw_tools/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/fw_tools/converter_elf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/fw_tools/patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/fw_tools/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.217001 shepherd_core-2024.4.2/shepherd_core/inventory/
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/inventory/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/inventory/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/inventory/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26245 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.217001 shepherd_core-2024.4.2/shepherd_core/testbed_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/testbed_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/testbed_client/cache_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/testbed_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/testbed_client/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/testbed_client/user_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.217001 shepherd_core-2024.4.2/shepherd_core/vsource/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/vsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/vsource/virtual_converter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/vsource/virtual_harvester_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/vsource/virtual_source_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14482 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/shepherd_core/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.229001 shepherd_core-2024.4.2/shepherd_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-04-24 19:38:56.000000 shepherd_core-2024.4.2/shepherd_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-24 19:38:56.000000 shepherd_core-2024.4.2/shepherd_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:38:56.000000 shepherd_core-2024.4.2/shepherd_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-24 19:38:56.000000 shepherd_core-2024.4.2/shepherd_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 19:38:56.000000 shepherd_core-2024.4.2/shepherd_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:38:55.000000 shepherd_core-2024.4.2/shepherd_core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.217001 shepherd_core-2024.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.221001 shepherd_core-2024.4.2/tests/data_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/example_cal_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/example_cal_data_faulty.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/example_cal_meas.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/example_cal_meas_faulty1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/example_cal_meas_faulty2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/example_config_emulator.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/example_config_experiment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/example_config_experiment_alternative.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/example_config_harvester.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/example_config_testbed.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/example_config_virtsource.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/test_base_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/test_content_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/test_content_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/test_experiment_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/test_task_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/test_task_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/test_testbed_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/data_models/test_testbed_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.225001 shepherd_core-2024.4.2/tests/decoder_waveform/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/decoder_waveform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/decoder_waveform/test_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.225001 shepherd_core-2024.4.2/tests/fw_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/fw_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   345592 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/fw_tools/build_msp.elf
+-rw-r--r--   0 runner    (1001) docker     (127)   887576 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/fw_tools/build_nrf.elf
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/fw_tools/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/fw_tools/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/fw_tools/test_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/fw_tools/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.225001 shepherd_core-2024.4.2/tests/inventory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/inventory/test_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/test_cal_hw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9560 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.225001 shepherd_core-2024.4.2/tests/testbed_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/testbed_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:56.229001 shepherd_core-2024.4.2/tests/vsource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/vsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/vsource/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/vsource/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/vsource/test_harvester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 19:38:51.000000 shepherd_core-2024.4.2/tests/vsource/test_z.py
```

### Comparing `shepherd_core-2024.4.1/PKG-INFO` & `shepherd_core-2024.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd_core
-Version: 2024.4.1
+Version: 2024.4.2
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Author-email: Ingmar Splitt <ingmar.splitt@tu-dresden.de>
 Maintainer-email: Ingmar Splitt <ingmar.splitt@tu-dresden.de>
 Project-URL: Documentation, https://github.com/orgua/shepherd-datalib/blob/main/README.md
 Project-URL: Issues, https://github.com/orgua/shepherd-datalib/issues
 Project-URL: Source, https://pypi.org/project/shepherd-core/
 Keywords: testbed,beaglebone,pru,batteryless,energyharvesting,solar
@@ -35,14 +35,15 @@
 Requires-Dist: pydantic[email]>2.0.0
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Requires-Dist: intelhex
 Requires-Dist: requests
 Requires-Dist: pyelftools
 Requires-Dist: zstandard
+Requires-Dist: typing-extensions
 Provides-Extra: elf
 Requires-Dist: pwntools-elf-only; extra == "elf"
 Provides-Extra: inventory
 Requires-Dist: psutil; extra == "inventory"
 Provides-Extra: dev
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
```

### Comparing `shepherd_core-2024.4.1/README.md` & `shepherd_core-2024.4.2/README.md`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.1/pyproject.toml` & `shepherd_core-2024.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     "pydantic[email]>2.0.0",
     "scipy",
     "tqdm",
     "intelhex",
     "requests",
     "pyelftools",
     "zstandard",
+    "typing-extensions",
 ]
 
 [project.optional-dependencies]
 elf = [
     "pwntools-elf-only",
     # TODO: still separate because of missing windows-compat
     # modified package for reading ELF-files with fw_tools
@@ -70,15 +71,15 @@
 
 [project.urls]
 Documentation = "https://github.com/orgua/shepherd-datalib/blob/main/README.md"
 Issues = "https://github.com/orgua/shepherd-datalib/issues"
 Source = "https://pypi.org/project/shepherd-core/"
 
 [build-system]
-requires = ["setuptools"]
+requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 platforms = ["unix", "linux", "osx", "cygwin", "win32", "win64"]
 zip-safe = true
 include-package-data = true
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/__init__.py` & `shepherd_core-2024.4.2/shepherd_core/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-"""shepherd.core
-~~~~~
+"""Bundled core features used by several systems.
+
 Provides classes for storing and retrieving sampled IV data to/from
 HDF5 files.
 
 """
 
 from .data_models.base.calibration import Calc_t
 from .data_models.base.calibration import CalibrationCape
@@ -19,15 +19,15 @@
 from .logger import increase_verbose_level
 from .logger import logger
 from .reader import Reader
 from .testbed_client.client import TestbedClient
 from .testbed_client.client import tb_client
 from .writer import Writer
 
-__version__ = "2024.04.1"
+__version__ = "2024.4.2"
 
 __all__ = [
     "Reader",
     "Writer",
     "get_verbose_level",
     "increase_verbose_level",
     "logger",
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/calibration_hw_def.py` & `shepherd_core-2024.4.2/shepherd_core/calibration_hw_def.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-"""Contains some info about the hardware configuration on the shepherd
+"""parametrized math models for converting between raw- and si-values.
+
+Contains some info about the hardware configuration on the shepherd
 cape. Based on these values, one can derive the expected adc readings given
 an input voltage/current or, for emulation, the expected voltage and current
 given the digital code in the DAC.
 
 currently configured for cape v2.4c
 
 """
@@ -27,42 +29,48 @@
 M_DAC = 16  # [bit]
 # DERIVED VARIABLES
 RAW_MAX_ADC = 2**M_ADC - 1
 RAW_MAX_DAC = 2**M_DAC - 1
 
 
 def adc_current_to_raw(current: float) -> int:
+    """Convert back a current [A] to raw ADC value."""
     # voltage on input of adc
     val_adc = G_INST_AMP * R_SHT * current
     # digital value according to ADC gain
     val_raw = int(val_adc * (2**M_ADC) / (G_ADC_I * V_REF_ADC))
     return min(max(val_raw, 0), 2**M_ADC - 1)
 
 
 def adc_raw_to_current(value: int) -> float:
+    """Convert a raw ADC value to a current [A]."""
     value = min(max(value, 0), 2**M_ADC - 1)
     # voltage on input of adc
     val_adc = float(value) * (G_ADC_I * V_REF_ADC) / (2**M_ADC)
     # current according to adc value
     return val_adc / (R_SHT * G_INST_AMP)
 
 
 def adc_voltage_to_raw(voltage: float) -> int:
+    """Convert back a voltage [V] to raw ADC value."""
     # digital value according to ADC gain
     val_raw = int(voltage * (2**M_ADC) / (G_ADC_V * V_REF_ADC))
     return min(max(val_raw, 0), 2**M_ADC - 1)
 
 
 def adc_raw_to_voltage(value: int) -> float:
+    """Convert a raw ADC value to a voltage [V]."""
     value = min(max(value, 0), 2**M_ADC - 1)
     # voltage according to ADC value
     return float(value) * (G_ADC_V * V_REF_ADC) / (2**M_ADC)
 
 
 def dac_raw_to_voltage(value: int) -> float:
+    """Convert back a raw DAC value to a voltage [V]."""
     value = min(max(value, 0), 2**M_DAC - 1)
     return float(value) * (V_REF_DAC * G_DAC) / (2**M_DAC)
 
 
 def dac_voltage_to_raw(voltage: float) -> int:
+    """Convert a voltage [V] to raw DAC value."""
     val_raw = int(voltage * (2**M_DAC) / (V_REF_DAC * G_DAC))
     return min(max(val_raw, 0), 2**M_DAC - 1)
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/__init__.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+"""Container for shepherds data-models.
+
+Public models are directly referenced here and are usable like:
+
+'''python
+from shepherd-core import data_models
+
+cdata = data_models.CapeData(serial_number="A123")
+'''
+"""
+
 from .base.calibration import CalibrationCape
 from .base.calibration import CalibrationEmulator
 from .base.calibration import CalibrationHarvester
 from .base.calibration import CalibrationPair
 from .base.calibration import CalibrationSeries
 from .base.calibration import CapeData
 from .base.content import ContentModel
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/base/cal_measurement.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/base/cal_measurement.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,85 +1,97 @@
+"""Models for the process of calibration a device by measurements."""
+
 from typing import List
 from typing import Optional
 
 import numpy as np
 from pydantic import Field
 from pydantic import PositiveFloat
 from pydantic import validate_call
 from typing_extensions import Annotated
 
-from .. import CalibrationCape
-from .. import CalibrationEmulator
-from .. import CalibrationHarvester
-from .. import CalibrationPair
+from .calibration import CalibrationCape
+from .calibration import CalibrationEmulator
+from .calibration import CalibrationHarvester
+from .calibration import CalibrationPair
 from .calibration import CapeData
 from .shepherd import ShpModel
 
 # TODO: move to shepherd_data to remove scipy-dependency from _core
 
 
 class CalMeasurementPair(ShpModel):
+    """Value-container for a calibration-measurement."""
+
     shepherd_raw: PositiveFloat
     reference_si: float = 0
 
 
 CalMeasPairs = Annotated[List[CalMeasurementPair], Field(min_length=2)]
 
 
 @validate_call
 def meas_to_cal(data: CalMeasPairs, component: str) -> CalibrationPair:
-    from scipy import stats  # here due to massive delay
+    """Convert values from calibration-measurement to the calibration itself."""
+    from scipy import stats  # placed here due to massive delay
 
     x = np.empty(len(data))
     y = np.empty(len(data))
     for i, pair in enumerate(data):
         x[i] = pair.shepherd_raw
         y[i] = pair.reference_si
     result = stats.linregress(x, y)
     offset = float(result.intercept)
     gain = float(result.slope)
     rval = result.rvalue  # test quality of regression
 
     if rval < 0.999:
-        raise ValueError(
+        msg = (
             "Calibration faulty -> Correlation coefficient "
             f"(rvalue) = {rval}:.6f is too low for '{component}'"
         )
+        raise ValueError(msg)
     return CalibrationPair(offset=offset, gain=gain)
 
 
 class CalMeasurementHarvester(ShpModel):
+    """Container for the values of the calibration-measurement."""
+
     dac_V_Hrv: CalMeasPairs
     dac_V_Sim: CalMeasPairs
     adc_V_Sense: CalMeasPairs
     adc_C_Hrv: CalMeasPairs
 
     def to_cal(self) -> CalibrationHarvester:
         dv = self.model_dump()
         dcal = CalibrationHarvester().model_dump()
         for key in dv:
             dcal[key] = meas_to_cal(self[key], f"hrv_{key}")
         return CalibrationHarvester(**dcal)
 
 
 class CalMeasurementEmulator(ShpModel):
+    """Container for the values of the calibration-measurement."""
+
     dac_V_A: CalMeasPairs  # TODO: why not V_dac_A or V_dac_a
     dac_V_B: CalMeasPairs
     adc_C_A: CalMeasPairs
     adc_C_B: CalMeasPairs
 
     def to_cal(self) -> CalibrationEmulator:
         dv = self.model_dump()
         dcal = CalibrationEmulator().model_dump()
         for key in dv:
             dcal[key] = meas_to_cal(self[key], f"emu_{key}")
         return CalibrationEmulator(**dcal)
 
 
 class CalMeasurementCape(ShpModel):
+    """Container for the values of the calibration-measurement."""
+
     cape: Optional[CapeData] = None
     host: Optional[str] = None
 
     harvester: Optional[CalMeasurementHarvester] = None
     emulator: Optional[CalMeasurementEmulator] = None
 
     def to_cal(self) -> CalibrationCape:
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/base/calibration.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/base/calibration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Models for the calibration-data to convert between raw & SI-Values."""
+
 import struct
 from typing import Callable
 from typing import Generator
 from typing import Optional
 from typing import TypeVar
 from typing import Union
 
@@ -22,14 +24,18 @@
 
 Calc_t = TypeVar("Calc_t", NDArray[np.float64], float)
 
 
 def dict_generator(
     in_dict: Union[dict, list], pre: Optional[list] = None
 ) -> Generator[list, None, None]:
+    """Recursive helper-function to generate a 1D-List(or not?).
+
+    TODO: isn't that a 1D-List generator?
+    """
     pre = pre[:] if pre else []
     if isinstance(in_dict, dict):
         for key, value in in_dict.items():
             if isinstance(value, dict):
                 yield from dict_generator(value, [*pre, key])
             elif isinstance(value, (list, tuple)):
                 for v in value:
@@ -37,44 +43,45 @@
             else:
                 yield [*pre, key, value]
     else:
         yield [*pre, in_dict]
 
 
 class CalibrationPair(ShpModel):
-    """SI-value [SI-Unit] = raw-value * gain + offset"""
+    """SI-value [SI-Unit] = raw-value * gain + offset."""
 
     gain: PositiveFloat
     offset: float = 0
 
     def raw_to_si(self, values_raw: Calc_t, *, allow_negative: bool = True) -> Calc_t:
-        """Convert between physical units and raw unsigned integers"""
+        """Convert between physical units and raw unsigned integers."""
         values_si = values_raw * self.gain + self.offset
         if not allow_negative:
             if isinstance(values_si, np.ndarray):
                 values_si[values_si < 0.0] = 0.0
                 # if pyright still complains, cast with .astype(float)
             else:
                 values_si = float(max(values_si, 0.0))
         elif not isinstance(values_si, np.ndarray):
             values_si = float(values_si)
         return values_si
 
     def si_to_raw(self, values_si: Calc_t) -> Calc_t:
-        """Convert between physical units and raw unsigned integers"""
+        """Convert between physical units and raw unsigned integers."""
         values_raw = (values_si - self.offset) / self.gain
         if isinstance(values_raw, np.ndarray):
             values_raw[values_raw < 0.0] = 0.0
             values_raw = np.around(values_raw)
         else:
             values_raw = round(max(values_raw, 0.0))
         return values_raw
 
     @classmethod
     def from_fn(cls, fn: Callable) -> Self:
+        """Probe linear function to determine scaling values."""
         offset = fn(0)
         gain_inv = fn(1.0) - offset
         return cls(
             gain=1.0 / float(gain_inv),
             offset=-float(offset) / gain_inv,
         )
 
@@ -84,21 +91,25 @@
     "dac_voltage_b": "dac_V_Hrv",
     "adc_current": "adc_C_Hrv",  # datalog current
     "adc_voltage": "adc_V_Sense",  # datalog voltage
 }
 
 
 class CalibrationHarvester(ShpModel):
+    """Container for all calibration-pairs for that device."""
+
     dac_V_Hrv: CalibrationPair = CalibrationPair.from_fn(dac_voltage_to_raw)
     dac_V_Sim: CalibrationPair = CalibrationPair.from_fn(dac_voltage_to_raw)
     adc_V_Sense: CalibrationPair = CalibrationPair.from_fn(adc_voltage_to_raw)
     adc_C_Hrv: CalibrationPair = CalibrationPair.from_fn(adc_current_to_raw)
 
     def export_for_sysfs(self) -> dict:
-        """[scaling according to commons.h]
+        """Convert and write the essential data.
+
+        [scaling according to commons.h]
         # ADC-C is handled in nA (nano-ampere), gain is shifted by 8 bit
         # ADC-V is handled in uV (micro-volt), gain is shifted by 8 bit
         # DAC-V is handled in uV (micro-volt), gain is shifted by 20 bit
         """
         cal_set = {
             "adc_current_gain": round(1e9 * (2**8) * self.adc_C_Hrv.gain),
             "adc_current_offset": round(1e9 * (2**0) * self.adc_C_Hrv.offset),
@@ -107,36 +118,42 @@
             "dac_voltage_gain": round((2**20) / (1e6 * self.dac_V_Hrv.gain)),
             "dac_voltage_offset": round(1e6 * (2**0) * self.dac_V_Hrv.offset),
         }
         for key, value in cal_set.items():
             if (("gain" in key) and not (0 <= value < 2**32)) or (
                 ("offset" in key) and not (-(2**31) <= value < 2**31)
             ):
-                raise ValueError(f"Value ({key}={value}) exceeds uint32-container")
+                msg = f"Value ({key}={value}) exceeds uint32-container"
+                raise ValueError(msg)
         return cal_set
 
 
 cal_emu_legacy = {  # legacy translator
     "dac_voltage_a": "dac_V_A",
     "dac_voltage_b": "dac_V_B",  # datalog voltage
     "adc_current": "adc_C_A",  # datalog current
     "adc_voltage": "adc_C_B",
 }
 
 
 class CalibrationEmulator(ShpModel):
-    """Cal-Data for both Target-Ports A/B"""
+    """Container for all calibration-pairs for that device.
+
+    Differentiates between both target-ports A/B.
+    """
 
     dac_V_A: CalibrationPair = CalibrationPair.from_fn(dac_voltage_to_raw)
     dac_V_B: CalibrationPair = CalibrationPair.from_fn(dac_voltage_to_raw)
     adc_C_A: CalibrationPair = CalibrationPair.from_fn(adc_current_to_raw)
     adc_C_B: CalibrationPair = CalibrationPair.from_fn(adc_current_to_raw)
 
     def export_for_sysfs(self) -> dict:
-        """[scaling according to commons.h]
+        """Convert and write the essential data.
+
+        [scaling according to commons.h]
         # ADC-C is handled in nA (nano-ampere), gain is shifted by 8 bit
         # ADC-V -> unused by vsrc / emu
         # DAC-V is handled in uV (micro-volt), gain is shifted by 20 bit
         TODO: current impl does not distinguish target_ports for DAC
         """
         cal_set = {
             "adc_current_gain": round(1e9 * (2**8) * self.adc_C_A.gain),
@@ -146,21 +163,23 @@
             "dac_voltage_gain": round((2**20) / (1e6 * self.dac_V_A.gain)),
             "dac_voltage_offset": round(1e6 * (2**0) * self.dac_V_A.offset),
         }
         for key, value in cal_set.items():
             if (("gain" in key) and not (0 <= value < 2**32)) or (
                 ("offset" in key) and not (-(2**31) <= value < 2**31)
             ):
-                raise ValueError(f"Value ({key}={value}) exceeds uint32-container")
+                msg = f"Value ({key}={value}) exceeds uint32-container"
+                raise ValueError(msg)
         return cal_set
 
 
 class CapeData(ShpModel):
-    """Representation of Beaglebone Cape information
-        -> just provide serial-number on creation
+    """Representation of Beaglebone Cape information.
+
+    User must at least provide serial-number on creation.
 
     According to BeagleBone specifications, each cape should host an EEPROM
     that contains some standardized information about the type of cape,
     manufacturer, version etc.
 
     `See<https://github.com/beagleboard/beaglebone-black/wiki/System-Reference-Manual#824_EEPROM_Data_Format>`_
     """
@@ -174,35 +193,37 @@
 
     serial_number: constr(max_length=12)
 
     cal_date: constr(max_length=12) = Field(default_factory=local_iso_date)
     # ⤷ produces something like '2023-01-01'
 
     def __repr__(self) -> str:  # TODO: override useful?
-        """string-representation allows print(model)"""
+        """string-representation allows print(model)."""
         return str(self.model_dump())
 
 
 class CalibrationCape(ShpModel):
     """Represents calibration data of shepherd cape.
+
     Defines the format of calibration data and provides convenient functions
     to read and write calibration data.
 
     YAML: .to_file() and .from_file() already in ShpModel
     """
 
     cape: Optional[CapeData] = None
     host: Optional[str] = None
 
     harvester: CalibrationHarvester = CalibrationHarvester()
     emulator: CalibrationEmulator = CalibrationEmulator()
 
     @classmethod
     def from_bytestr(cls, data: bytes, cape: Optional[CapeData] = None) -> Self:
-        """Instantiates calibration data based on byte string.
+        """Instantiate calibration data based on byte string.
+
         This is mainly used to deserialize data read from an EEPROM memory.
 
         Args:
         ----
             data: Byte string containing calibration data.
             cape: data can be supplied
         Returns:
@@ -216,28 +237,30 @@
         for _i, walk in enumerate(lw):
             # hardcoded fixed depth ... bad but easy
             dv[walk[0]][walk[1]][walk[2]] = float(values[_i])
         dv["cape"] = cape
         return cls(**dv)
 
     def to_bytestr(self) -> bytes:
-        """Serializes calibration data to byte string.
+        """Serialize calibration data to byte string.
+
         Used to prepare data for writing it to EEPROM.
 
-        Returns
-        -------
+        Returns:
             Byte string representation of calibration values.
 
         """
         lw = list(dict_generator(self.model_dump(include={"harvester", "emulator"})))
         values = [walk[-1] for walk in lw]
         return struct.pack(">" + len(lw) * "d", *values)
 
 
 class CalibrationSeries(ShpModel):
+    """Cal-Data for a typical recording of a testbed experiment."""
+
     voltage: CalibrationPair = CalibrationPair(gain=3 * 1e-9)
     # ⤷ default allows 0 - 12 V in 3 nV-Steps
     current: CalibrationPair = CalibrationPair(gain=250 * 1e-12)
     # ⤷ default allows 0 - 1 A in 250 pA - Steps
     time: CalibrationPair = CalibrationPair(gain=1e-9)
     # ⤷ default = nanoseconds
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/base/content.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/base/content.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,49 @@
+"""Base-Model for all content."""
+
 import hashlib
 from datetime import datetime
 from typing import Optional
 from typing import Union
 from uuid import uuid4
 
 from pydantic import UUID4
 from pydantic import Field
 from pydantic import StringConstraints
 from pydantic import model_validator
 from typing_extensions import Annotated
 from typing_extensions import Self
+from typing_extensions import deprecated
 
 from .shepherd import ShpModel
 from .timezone import local_now
 
 # constr -> to_lower=True, max_length=16, regex=r"^[\w]+$"
 # ⤷ Regex = AlphaNum
 IdInt = Annotated[int, Field(ge=0, lt=2**128)]
 NameStr = Annotated[str, StringConstraints(max_length=32, pattern=r"^[^<>:;,?\"\*|\/\\]+$")]
 # ⤷ Regex = FileSystem-Compatible ASCII
 SafeStr = Annotated[str, StringConstraints(pattern=r"^[ -~]+$")]
 # ⤷ Regex = All Printable ASCII-Characters with Space
 
 
+@deprecated("use UUID4 instead")
 def id_default() -> int:
-    # note: IdInt has space for 128 bit, so 128/4 = 32 hex-chars
+    """Generate a unique ID - usable as default value.
+
+    Note: IdInt has space for 128 bit, so 128/4 = 32 hex-chars
+    """
     time_stamp = str(local_now()).encode("utf-8")
     time_hash = hashlib.sha3_224(time_stamp).hexdigest()[-32:]
     return int(time_hash, 16)
 
 
 class ContentModel(ShpModel):
-    # General Properties
+    """Base-Model for content with generalized properties."""
+
     # id: UUID4 = Field(  # TODO: db-migration - temp fix for documentation
     id: Union[UUID4, int] = Field(
         description="Unique ID",
         default_factory=uuid4,
     )
     name: NameStr
     description: Annotated[Optional[SafeStr], Field(description="Required when public")] = None
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/base/shepherd.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/base/shepherd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Shepherds base-model that brings a lot of default functionality."""
+
 import hashlib
 import pathlib
 from datetime import timedelta
 from ipaddress import IPv4Address
 from pathlib import Path
 from typing import Any
 from typing import Generator
@@ -20,35 +22,38 @@
 from .timezone import local_now
 from .wrapper import Wrapper
 
 
 def path2str(
     dumper: Dumper, data: Union[pathlib.Path, pathlib.WindowsPath, pathlib.PosixPath]
 ) -> ScalarNode:
+    """Add a yaml-representation for a specific datatype."""
     return dumper.represent_scalar("tag:yaml.org,2002:str", str(data.as_posix()))
 
 
 def time2int(dumper: Dumper, data: timedelta) -> ScalarNode:
+    """Add a yaml-representation for a specific datatype."""
     return dumper.represent_scalar("tag:yaml.org,2002:int", str(int(data.total_seconds())))
 
 
 def generic2str(dumper: Dumper, data: Any) -> ScalarNode:
+    """Add a yaml-representation for a specific datatype."""
     return dumper.represent_scalar("tag:yaml.org,2002:str", str(data))
 
 
 yaml.add_representer(pathlib.PosixPath, path2str, SafeDumper)
 yaml.add_representer(pathlib.WindowsPath, path2str, SafeDumper)
 yaml.add_representer(pathlib.Path, path2str, SafeDumper)
 yaml.add_representer(timedelta, time2int, SafeDumper)
 yaml.add_representer(IPv4Address, generic2str, SafeDumper)
 yaml.add_representer(UUID, generic2str, SafeDumper)
 
 
 class ShpModel(BaseModel):
-    """Pre-configured Pydantic Base-Model (specifically for shepherd)
+    """Pre-configured Pydantic Base-Model (specifically for shepherd).
 
     Inheritable Features:
     - constant / frozen, hashable .get_hash()
     - safe / limited custom types
     - string-representation str(ShpModel)
     - accessible as class (model.var) and dict (model[var])
     - yaml-support with type-safe .from_file() & .to_file()
@@ -65,68 +70,72 @@
         # ⤷ TODO: was 4 but localizing constraints works different with pydantic2
         #       - might be solvable with "use_enum_values=True"
         str_max_length=512,
         # ⤷ local str-length constraints overrule global ones!
         str_strip_whitespace=True,  # strip leading & trailing whitespaces
         use_enum_values=True,  # cleaner export of enum-parameters
         allow_inf_nan=False,  # float without +-inf or NaN
-        # defer_build, possible speedup -> but it triggers a bug
+        # defer_build=True, possible speedup -> but it triggers a bug
     )
 
     def __repr__(self) -> str:
-        """string-representation allows print(model)"""
+        """string-representation allows print(model)."""
         name = type(self).__name__
         content = self.model_dump(exclude_unset=True, exclude_defaults=True)
         return f"{name}({content})"
 
     def __str__(self) -> str:
-        """string-representation allows str(model)"""
+        """string-representation allows str(model)."""
         content = yaml.safe_dump(
             self.model_dump(exclude_unset=True, exclude_defaults=True),
             default_flow_style=False,
             sort_keys=False,
         )
         return str(content)
 
     def __getitem__(self, key: str) -> Any:
-        """Allows dict access -> model["key"], in addition to model.key"""
+        """Allow dict access like model["key"].
+
+        in addition to model.key.
+        """
         return self.__getattribute__(key)
 
     def __contains__(self, item: str) -> bool:
-        """Allows checks like 'x in YClass'"""
+        """Allow checks like 'x in YClass'."""
         return item in self.model_dump().keys()  # noqa: SIM118
         # more correct, but probably slower than hasattr
 
     def keys(self):  # noqa: ANN201
-        """Fn of dict"""
+        """Fn of dict."""
         return self.model_dump().keys()
 
     def items(self) -> Generator[tuple, None, None]:
-        """Fn of dict"""
+        """Fn of dict."""
         for key in self.keys():
             yield key, self[key]
 
     @classmethod
     def schema_to_file(cls, path: Union[str, Path]) -> None:
-        """Store schema to yaml (for frontend-generators)"""
+        """Store schema to yaml (for frontend-generators)."""
         model_dict = cls.model_json_schema()
         model_yaml = yaml.safe_dump(model_dict, default_flow_style=False, sort_keys=False)
         with Path(path).resolve().with_suffix(".yaml").open("w") as f:
             f.write(model_yaml)
 
     def to_file(
         self,
         path: Union[str, Path],
         comment: Optional[str] = None,
         *,
         minimal: bool = True,
     ) -> Path:
-        """Store data to yaml in a wrapper
+        """Store data to yaml in a wrapper.
+
         minimal: stores minimal set (filters out unset & default parameters)
-        comment: documentation
+        comment: documentation.
         """
         model_dict = self.model_dump(exclude_unset=minimal)
         model_wrap = Wrapper(
             datatype=type(self).__name__,
             comment=comment,
             created=local_now(),
             parameters=model_dict,
@@ -142,15 +151,15 @@
             model_path.parent.mkdir(parents=True)
         with model_path.open("w") as f:
             f.write(model_yaml)
         return model_path
 
     @classmethod
     def from_file(cls, path: Union[str, Path]) -> Self:
-        """Load from yaml"""
+        """Load from yaml."""
         with Path(path).open() as shp_file:
             shp_dict = yaml.safe_load(shp_file)
         shp_wrap = Wrapper(**shp_dict)
         if shp_wrap.datatype != cls.__name__:
             raise ValueError("Model in file does not match the requirement")
         return cls(**shp_wrap.parameters)
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/base/wrapper.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/base/wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
+"""Wrapper-related ecosystem for transferring models."""
+
 from datetime import datetime
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import StringConstraints
 from typing_extensions import Annotated
 
 SafeStrClone = Annotated[str, StringConstraints(pattern=r"^[ -~]+$")]
 # ⤷ copy avoids circular import
 
 
 class Wrapper(BaseModel):
-    """Prototype for enabling one web- & file-interface for
-    all models with dynamic typecasting
-    """
+    """Generalized web- & file-interface for all models with dynamic typecasting."""
 
     datatype: str
     # ⤷ model-name
     comment: Optional[SafeStrClone] = None
     created: Optional[datetime] = None
     # ⤷ Optional metadata
     parameters: dict
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/content/__init__.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/content/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+"""Module for content-type data-models.
+
+These models import externally from: /base, /testbed.
+"""
+
 from .energy_environment import EnergyDType
 from .energy_environment import EnergyEnvironment
 from .firmware import Firmware
 from .firmware_datatype import FirmwareDType
 from .virtual_harvester import VirtualHarvesterConfig
 from .virtual_source import VirtualSourceConfig
 
-# these models import externally from: /base, /testbed
-
 __all__ = [
     "EnergyEnvironment",
     "VirtualSourceConfig",
     "VirtualHarvesterConfig",
     "Firmware",
     # Enums
     "EnergyDType",
     "FirmwareDType",
 ]
-
-# TODO: include models for end-users on root-level
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/content/energy_environment.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/content/energy_environment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,30 @@
+"""Data-model for recorded eEnvs."""
+
 from enum import Enum
 from pathlib import Path
 from typing import Optional
 
 from pydantic import PositiveFloat
 from pydantic import model_validator
 
 from ...testbed_client import tb_client
 from ..base.content import ContentModel
 
 
 class EnergyDType(str, Enum):
-    ivsample = "ivsample"
-    ivsamples = "ivsample"
-    ivcurve = "ivcurve"
-    ivcurves = "ivcurve"  # a stream could also be called iv-surface
+    """Data-Type-Options for energy environments."""
+
+    ivsample = ivsamples = "ivsample"
+    ivcurve = ivcurves = ivsurface = "ivcurve"
     isc_voc = "isc_voc"
 
 
 class EnergyEnvironment(ContentModel):
-    """Recording of meta-data representation of a testbed-component"""
+    """Recording of meta-data representation of a testbed-component."""
 
     # General Metadata & Ownership -> ContentModel
 
     data_path: Path
     data_type: EnergyDType
     data_local: bool = True
     # ⤷ signals that file has to be copied to testbed
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/content/firmware.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/content/firmware.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""Handling firmware for targets.
+
+TODO: should be more generalized - currently only supports msp & nRF
+"""
+
 from pathlib import Path
 from typing import Optional
 from typing import TypedDict
 from typing import Union
 
 from pydantic import StringConstraints
 from pydantic import model_validator
@@ -41,15 +46,15 @@
     "nrf52": {"name": "nrf52"},
 }
 
 FirmwareStr = Annotated[str, StringConstraints(min_length=3, max_length=8_000_000)]
 
 
 class Firmware(ContentModel, title="Firmware of Target"):
-    """meta-data representation of a data-component"""
+    """meta-data representation of a data-component."""
 
     # General Metadata & Ownership -> ContentModel
 
     mcu: MCU
 
     data: Union[FirmwareStr, Path]
     data_type: FirmwareDType
@@ -87,17 +92,18 @@
     def from_firmware(
         cls,
         file: Path,
         *,
         embed: bool = True,
         **kwargs: Unpack[TypedDict],
     ) -> Self:
-        """Embeds firmware and tries to fill parameters
+        """Embeds firmware and tries to fill parameters.
+
         ELF -> mcu und data_type are deducted
-        HEX -> must supply mcu manually
+        HEX -> must supply mcu manually.
         """
         # TODO: use new determine_type() & determine_arch() and also allow to not embed
         kwargs["data_hash"] = fw_tools.file_to_hash(file)
         if embed:
             kwargs["data"] = fw_tools.file_to_base64(file)
             kwargs["data_local"] = False
         else:
@@ -109,15 +115,15 @@
 
         if kwargs["data_type"] == FirmwareDType.base64_hex:
             if fw_tools.is_hex_msp430(file):
                 arch = "msp430"
             elif fw_tools.is_hex_nrf52(file):
                 arch = "nrf52"
             else:
-                raise ValueError("File is not a HEX for the Testbed")
+                raise ValueError("File is not a suitable HEX for the Testbed")
             if "mcu" not in kwargs:
                 kwargs["mcu"] = arch_to_mcu[arch]
 
         if kwargs["data_type"] == FirmwareDType.base64_elf:
             arch = fw_tools.read_arch(file)
             if "msp430" in arch and not fw_tools.is_elf_msp430(file):
                 raise ValueError("File is not a ELF for msp430")
@@ -146,15 +152,16 @@
 
         if not match:
             logger.warning("FW-Hash does not match with stored value!")
         return match
 
     @validate_call
     def extract_firmware(self, file: Path) -> Path:
-        """Stores embedded data in file
+        """Store embedded fw-data in file.
+
         - file-suffix is derived from data-type and adapted
         - if provided path is a directory, the firmware-name is used
         """
         if file.is_dir():
             file = file / self.name
         file_new = fw_tools.extract_firmware(self.data, self.data_type, file)
         self.compare_hash(file_new)
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/content/virtual_harvester.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/content/virtual_harvester.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Generalized energy harvester data models."""
+
 from enum import Enum
 from typing import Optional
 from typing import Tuple
 
 from pydantic import Field
 from pydantic import model_validator
 from typing_extensions import Annotated
@@ -13,30 +15,30 @@
 from ..base.calibration import CalibrationHarvester
 from ..base.content import ContentModel
 from ..base.shepherd import ShpModel
 from .energy_environment import EnergyDType
 
 
 class AlgorithmDType(str, Enum):
+    """Options for choosing a harvesting algorithm."""
+
     isc_voc = "isc_voc"
-    ivcurve = ("ivcurve",)
-    ivcurves = ("ivcurve",)
-    cv = "cv"
-    constant = "cv"
+    ivcurve = ivcurves = ("ivcurve",)
+    constant = cv = "cv"
     # ci .. constant current -> is this desired?
     mppt_voc = "mppt_voc"
-    mppt_po = "mppt_po"
-    perturb_observe = "mppt_po"
-    mppt_opt = "mppt_opt"
-    optimal = "mppt_opt"
+    mppt_po = perturb_observe = "mppt_po"
+    mppt_opt = optimal = "mppt_opt"
 
 
 class VirtualHarvesterConfig(ContentModel, title="Config for the Harvester"):
-    """A Harvester is needed when the file-based energy environment
-    of the virtual source is not already supplied as ivsample
+    """A vHrv makes a source-characterization (i.e. ivcurve) usable for the vSrc.
+
+    Mostly used when the file-based energy environment of the virtual source
+    is not already supplied as pre-harvested ivsample-stream.
     """
 
     # General Metadata & Ownership -> ContentModel
 
     algorithm: AlgorithmDType
     # ⤷ used to harvest energy
 
@@ -106,27 +108,29 @@
 
     def calc_hrv_mode(self, *, for_emu: bool) -> int:
         return 1 * int(for_emu) + 2 * self.rising
 
     def calc_algorithm_num(self, *, for_emu: bool) -> int:
         num = algo_to_num.get(self.algorithm)
         if for_emu and self.get_datatype() != EnergyDType.ivsample:
-            raise ValueError(
+            msg = (
                 f"[{self.name}] Select valid harvest-algorithm for emulator, "
-                f"current usage = {self.algorithm}",
+                f"current usage = {self.algorithm}"
             )
+            raise ValueError(msg)
         if num < algo_to_num["isc_voc"]:
-            raise ValueError(
+            msg = (
                 f"[{self.name}] Select valid harvest-algorithm for harvester, "
-                f"current usage = {self.algorithm}",
+                f"current usage = {self.algorithm}"
             )
+            raise ValueError(msg)
         return num
 
     def calc_timings_ms(self, *, for_emu: bool) -> Tuple[float, float]:
-        """factor-in model-internal timing-constraints"""
+        """factor-in model-internal timing-constraints."""
         window_length = self.samples_n * (1 + self.wait_cycles)
         time_min_ms = (1 + self.wait_cycles) * 1_000 / samplerate_sps_default
         if for_emu:
             window_ms = window_length * 1_000 / samplerate_sps_default
             time_min_ms = max(time_min_ms, window_ms)
 
         interval_ms = min(max(self.interval_ms, time_min_ms), 1_000_000)
@@ -151,15 +155,15 @@
     ) -> int:
         if for_emu:
             if dtype_in == EnergyDType.ivcurve:
                 return self.samples_n * (1 + self.wait_cycles)
             if dtype_in == EnergyDType.ivsample:
                 return 0
             # isc_voc: 2 * (1 + wait_cycles), noqa
-            raise ValueError("Not Implemented")
+            raise NotImplementedError
 
         # only used by ivcurve algo (in ADC-Mode)
         return self.samples_n
 
 
 u32 = Annotated[int, Field(ge=0, lt=2**32)]
 
@@ -187,19 +191,20 @@
     "mppt_voc": EnergyDType.ivsample,
     "mppt_po": EnergyDType.ivsample,
     "mppt_opt": EnergyDType.ivsample,
 }
 
 
 class HarvesterPRUConfig(ShpModel):
-    """Map settings-list to internal state-vars struct HarvesterConfig
+    """Map settings-list to internal state-vars struct HarvesterConfig for PRU.
+
     NOTE:
       - yaml is based on si-units like nA, mV, ms, uF
       - c-code and py-copy is using nA, uV, ns, nF, fW, raw
-      - ordering is intentional and in sync with shepherd/commons.h
+      - ordering is intentional and in sync with shepherd/commons.h.
     """
 
     algorithm: u32
     hrv_mode: u32
     window_size: u32
     voltage_uV: u32
     voltage_min_uV: u32
@@ -224,15 +229,15 @@
         window_size: Optional[u32] = None,
         *,
         for_emu: bool = False,
     ) -> Self:
         if isinstance(dtype_in, str):
             dtype_in = EnergyDType[dtype_in]
         if for_emu and dtype_in not in {EnergyDType.ivsample, EnergyDType.ivcurve}:
-            raise ValueError("Not Implemented")
+            raise NotImplementedError
         # TODO: use dtype properly in shepherd
         interval_ms, duration_ms = data.calc_timings_ms(for_emu=for_emu)
         return cls(
             algorithm=data.calc_algorithm_num(for_emu=for_emu),
             hrv_mode=data.calc_hrv_mode(for_emu=for_emu),
             window_size=window_size
             if window_size is not None
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/content/virtual_source.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/content/virtual_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
+"""Generalized virtual source data models."""
+
 from typing import List
 
 from pydantic import Field
 from pydantic import model_validator
 from typing_extensions import Annotated
 from typing_extensions import Self
 
 from ...commons import samplerate_sps_default
 from ...logger import logger
 from ...testbed_client import tb_client
-from .. import ShpModel
 from ..base.content import ContentModel
+from ..base.shepherd import ShpModel
 from .virtual_harvester import HarvesterPRUConfig
 from .virtual_harvester import VirtualHarvesterConfig
 
 # Custom Types
 LUT_SIZE: int = 12
 NormedNum = Annotated[float, Field(ge=0.0, le=1.0)]
 LUT1D = Annotated[List[NormedNum], Field(min_length=LUT_SIZE, max_length=LUT_SIZE)]
 LUT2D = Annotated[List[LUT1D], Field(min_length=LUT_SIZE, max_length=LUT_SIZE)]
 
 
 class VirtualSourceConfig(ContentModel, title="Config for the virtual Source"):
-    """The virtual Source uses the energy environment (file)
-    for supplying the Target Node during the experiment.
-    If not already done, the energy will be harvested and then converted.
+    """The vSrc uses the energy environment (file) for supplying the Target Node.
+
+    If not already done, the energy will be harvested and
+    then converted during the experiment.
+
     The converter-stage is software defined and offers:
     - buck-boost-combinations,
     - a simple diode + resistor and
     - an intermediate buffer capacitor.
     """
 
     # TODO: I,V,R should be in regular unit (V, A, Ohm)
@@ -113,17 +117,23 @@
     @model_validator(mode="after")
     def post_validation(self) -> Self:
         # trigger stricter test of harv-parameters
         HarvesterPRUConfig.from_vhrv(self.harvester, for_emu=True)
         return self
 
     def calc_internal_states(self) -> dict:
-        """Compensate for (hard to detect) current-surge of real capacitors
-        when converter gets turned on -> this can be const value, because
-        the converter always turns on with "V_storage_enable_threshold_uV"
+        """Update the model-states for the capacitor and other elements.
+
+        This also compensates for current-surge of real capacitors
+        when the converter gets turned on:
+
+        - surges are hard to detect & record
+        - this can be const value, because
+        - the converter always turns on with "V_storage_enable_threshold_uV".
+
         TODO: currently neglecting delay after disabling converter, boost
         only has simpler formula, second enabling when V_Cap >= V_out
 
         Math behind this calculation:
 
         - Energy-Change Storage Cap ->  E_new = E_old - E_output
         - with Energy of a Cap 	    -> 	E_x = C_x * V_x^2 / 2
@@ -185,30 +195,31 @@
         else:
             values["dV_enable_output_mV"] = dV_output_en_thrs_mV
             values["V_enable_output_threshold_mV"] = self.V_intermediate_enable_threshold_mV
             values["V_disable_output_threshold_mV"] = self.V_intermediate_disable_threshold_mV
         return values
 
     def calc_converter_mode(self, *, log_intermediate_node: bool) -> int:
-        """Assembles bitmask from discrete values
+        """Assembles bitmask from discrete values.
 
         log_intermediate_node: record / log virtual intermediate (cap-)voltage and
         -current (out) instead of output-voltage and -current
         """
         enable_storage = self.C_intermediate_uF > 0
         enable_boost = self.enable_boost and enable_storage
         return (
             1 * int(enable_storage)
             + 2 * int(enable_boost)
             + 4 * int(self.enable_buck)
             + 8 * int(log_intermediate_node)
         )
 
     def calc_cap_constant_us_per_nF_n28(self) -> int:
-        """Calc constant to convert capacitor-current to Voltage-delta
+        """Calc constant to convert capacitor-current to Voltage-delta.
+
         dV[uV] = constant[us/nF] * current[nA] = constant[us*V/nAs] * current[nA]
         """
         C_cap_uF = max(self.C_intermediate_uF, 0.001)
         return int((10**3 * (2**28)) // (C_cap_uF * samplerate_sps_default))
 
 
 u32 = Annotated[int, Field(ge=0, lt=2**32)]
@@ -220,15 +231,16 @@
         max_length=LUT_SIZE,
     ),
 ]
 lut_o = Annotated[List[u32], Field(min_length=LUT_SIZE, max_length=LUT_SIZE)]
 
 
 class ConverterPRUConfig(ShpModel):
-    """Map settings-list to internal state-vars struct ConverterConfig
+    """Map settings-list to internal state-vars struct ConverterConfig.
+
     NOTE:
       - yaml is based on si-units like nA, mV, ms, uF
       - c-code and py-copy is using nA, uV, ns, nF, fW, raw
       - ordering is intentional and in sync with shepherd/commons.h
     """
 
     converter_mode: u32
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/doc_virtual_source.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/virtual_source_doc.txt`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/experiment/__init__.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/experiment/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-from ..testbed.cape import TargetPort
+"""Module for experiment related data-models.
+
+These models import externally from: /base, /content, /testbed.
+"""
+
 from .experiment import Experiment
 from .observer_features import GpioActuation
 from .observer_features import GpioEvent
 from .observer_features import GpioLevel
 from .observer_features import GpioTracing
 from .observer_features import PowerTracing
 from .observer_features import SystemLogging
 from .target_config import TargetConfig
 
-# these models import externally from: /base, /content, /testbed
-
 __all__ = [
     "Experiment",
     "TargetConfig",
     # Features
     "PowerTracing",
     "GpioTracing",
     "GpioActuation",
     "GpioEvent",
     "SystemLogging",
     # Enums
     "GpioLevel",
-    "TargetPort",
 ]
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/experiment/experiment.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/experiment/experiment.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Config for testbed experiments."""
+
 from datetime import datetime
 from datetime import timedelta
 from typing import List
 from typing import Optional
 from typing import Union
 from uuid import uuid4
 
@@ -18,20 +20,18 @@
 from ..testbed.target import Target
 from ..testbed.testbed import Testbed
 from .observer_features import SystemLogging
 from .target_config import TargetConfig
 
 
 class Experiment(ShpModel, title="Config of an Experiment"):
-    """Configuration for Experiments on the Shepherd-Testbed
-    emulating Energy Environments for Target Nodes
-    """
+    """Config for experiments on the testbed emulating energy environments for target nodes."""
 
     # General Properties
-    # id: UUID4 ... # TODO db-migration - temp fix for documentation
+    # id: UUID4 ... # TODO: db-migration - temp fix for documentation
     id: Union[UUID4, int] = Field(default_factory=uuid4)
     # ⤷ TODO: automatic ID is problematic for identification by hash
 
     name: NameStr
     description: Annotated[
         Optional[SafeStr], Field(description="Required for public instances")
     ] = None
@@ -86,19 +86,20 @@
     def validate_observers(configs: List[TargetConfig]) -> None:
         target_ids = [_id for _config in configs for _id in _config.target_IDs]
 
         testbed = Testbed(name="shepherd_tud_nes")
         obs_ids = [testbed.get_observer(_id).id for _id in target_ids]
         if len(target_ids) > len(set(obs_ids)):
             raise ValueError(
-                "Observer used more than once in Experiment -> only 1 target per observer!"
+                "Observer is used more than once in Experiment -> only 1 target per observer!"
             )
 
     def get_target_ids(self) -> list:
         return [_id for _config in self.target_configs for _id in _config.target_IDs]
 
     def get_target_config(self, target_id: int) -> TargetConfig:
         for _config in self.target_configs:
             if target_id in _config.target_IDs:
                 return _config
         # gets already caught in target_config - but keep:
-        raise ValueError(f"Target-ID {target_id} was not found in Experiment '{self.name}'")
+        msg = f"Target-ID {target_id} was not found in Experiment '{self.name}'"
+        raise ValueError(msg)
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/experiment/observer_features.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/experiment/observer_features.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Configs for observer features like gpio- & power-tracing."""
+
 from datetime import timedelta
 from enum import Enum
 from typing import List
 from typing import Optional
 
 import numpy as np
 from pydantic import Field
@@ -11,15 +13,16 @@
 from typing_extensions import Self
 
 from ..base.shepherd import ShpModel
 from ..testbed.gpio import GPIO
 
 
 class PowerTracing(ShpModel, title="Config for Power-Tracing"):
-    """Configuration for recording the Power-Consumption of the Target Nodes
+    """Configuration for recording the Power-Consumption of the Target Nodes.
+
     TODO: postprocessing not implemented ATM
     """
 
     intermediate_voltage: bool = False
     # ⤷ for EMU: record buffer capacitor instead of output (good for V_out = const)
     #            this also includes current!
 
@@ -41,20 +44,21 @@
         if self.duration and self.duration.total_seconds() < 0:
             raise ValueError("Duration can't be negative.")
 
         discard_all = self.discard_current and self.discard_voltage
         if not self.calculate_power and discard_all:
             raise ValueError("Error in config -> tracing enabled, but output gets discarded")
         if self.calculate_power:
-            raise ValueError("postprocessing not implemented ATM")
+            raise NotImplementedError("postprocessing not implemented ATM")
         return self
 
 
 class GpioTracing(ShpModel, title="Config for GPIO-Tracing"):
-    """Configuration for recording the GPIO-Output of the Target Nodes
+    """Configuration for recording the GPIO-Output of the Target Nodes.
+
     TODO: postprocessing not implemented ATM
     """
 
     # initial recording
     mask: Annotated[int, Field(ge=0, lt=2**10)] = 0b11_1111_1111  # all
     # ⤷ TODO: custom mask not implemented in PRU, ATM
     gpios: Optional[Annotated[List[GPIO], Field(min_length=1, max_length=10)]] = None  # = all
@@ -80,56 +84,59 @@
             raise ValueError("Delay can't be negative.")
         if self.duration and self.duration.total_seconds() < 0:
             raise ValueError("Duration can't be negative.")
         return self
 
 
 class GpioLevel(str, Enum):
+    """Options for setting the gpio-level or state."""
+
     low = "L"
     high = "H"
     toggle = "X"  # TODO: not the smartest decision for writing a converter
 
 
 class GpioEvent(ShpModel, title="Config for a GPIO-Event"):
-    """Configuration for a single GPIO-Event (Actuation)"""
+    """Configuration for a single GPIO-Event (Actuation)."""
 
     delay: PositiveFloat
     # ⤷ from start_time
     # ⤷ resolution 10 us (guaranteed, but finer steps are possible)
     gpio: GPIO
     level: GpioLevel
     period: Annotated[float, Field(ge=10e-6)] = 1
     # ⤷ time base of periodicity in s
     count: Annotated[int, Field(ge=1, le=4096)] = 1
 
     @model_validator(mode="after")
     def post_validation(self) -> Self:
         if not self.gpio.user_controllable():
-            raise ValueError(f"GPIO '{self.gpio.name}' in actuation-event not controllable by user")
+            msg = f"GPIO '{self.gpio.name}' in actuation-event not controllable by user"
+            raise ValueError(msg)
         return self
 
     def get_events(self) -> np.ndarray:
         stop = self.delay + self.count * self.period
         return np.arange(self.delay, stop, self.period)
 
 
 class GpioActuation(ShpModel, title="Config for GPIO-Actuation"):
-    """Configuration for a GPIO-Actuation-Sequence"""
+    """Configuration for a GPIO-Actuation-Sequence."""
 
     # TODO: not implemented ATM - decide if pru control sys-gpio or
     # TODO: not implemented ATM - reverses pru-gpio (preferred if possible)
 
     events: Annotated[List[GpioEvent], Field(min_length=1, max_length=1024)]
 
     def get_gpios(self) -> set:
         return {_ev.gpio for _ev in self.events}
 
 
 class SystemLogging(ShpModel, title="Config for System-Logging"):
-    """Configuration for recording Debug-Output of the Observers System-Services"""
+    """Configuration for recording Debug-Output of the Observers System-Services."""
 
     dmesg: bool = True
     ptp: bool = True
     shepherd: bool = True
     # TODO: rename to kernel, timesync, sheep
     # TODO: add utilization as option
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/experiment/target_config.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/experiment/target_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Configuration related to Target Nodes (DuT)."""
+
 from typing import List
 from typing import Optional
 
 from pydantic import Field
 from pydantic import model_validator
 from typing_extensions import Annotated
 from typing_extensions import Self
@@ -15,15 +17,15 @@
 from ..testbed.target import Target
 from .observer_features import GpioActuation
 from .observer_features import GpioTracing
 from .observer_features import PowerTracing
 
 
 class TargetConfig(ShpModel, title="Target Config"):
-    """Configuration for Target Nodes (DuT)"""
+    """Configuration related to Target Nodes (DuT)."""
 
     target_IDs: Annotated[List[IdInt], Field(min_length=1, max_length=128)]
     custom_IDs: Optional[Annotated[List[IdInt16], Field(min_length=1, max_length=128)]] = None
     # ⤷ will replace 'const uint16_t SHEPHERD_NODE_ID' in firmware
     #   if no custom ID is provided, the original ID of target is used
 
     energy_env: EnergyEnvironment  # alias: input
@@ -40,44 +42,46 @@
     power_tracing: Optional[PowerTracing] = None
     gpio_tracing: Optional[GpioTracing] = None
     gpio_actuation: Optional[GpioActuation] = None
 
     @model_validator(mode="after")
     def post_validation(self) -> Self:
         if not self.energy_env.valid:
-            raise ValueError(f"EnergyEnv '{self.energy_env.name}' for target must be valid")
+            msg = f"EnergyEnv '{self.energy_env.name}' for target must be valid"
+            raise ValueError(msg)
         for _id in self.target_IDs:
             target = Target(id=_id)
             for mcu_num in [1, 2]:
                 val_fw = getattr(self, f"firmware{mcu_num}")
                 has_fw = val_fw is not None
                 tgt_mcu = target[f"mcu{mcu_num}"]
                 has_mcu = tgt_mcu is not None
                 if not has_fw and has_mcu:
                     fw_def = Firmware(name=tgt_mcu.fw_name_default)
                     # ⤷ this will raise if default is faulty
                     if tgt_mcu.id != fw_def.mcu.id:
-                        raise ValueError(
+                        msg = (
                             f"Default-Firmware for MCU{mcu_num} of Target-ID '{target.id}' "
                             f"(={fw_def.mcu.name}) "
                             f"is incompatible (={tgt_mcu.name})"
                         )
+                        raise ValueError(msg)
                 if has_fw and has_mcu and val_fw.mcu.id != tgt_mcu.id:
-                    raise ValueError(
+                    msg = (
                         f"Firmware{mcu_num} for MCU of Target-ID '{target.id}' "
                         f"(={val_fw.mcu.name}) "
                         f"is incompatible (={tgt_mcu.name})"
                     )
+                    raise ValueError(msg)
 
         c_ids = self.custom_IDs
         t_ids = self.target_IDs
         if c_ids is not None and (len(set(c_ids)) < len(set(t_ids))):
-            raise ValueError(
-                f"Provided custom IDs {c_ids} not enough to cover target range {t_ids}"
-            )
+            msg = f"Provided custom IDs {c_ids} not enough to cover target range {t_ids}"
+            raise ValueError(msg)
         # TODO: if custom ids present, firmware must be ELF
         return self
 
     def get_custom_id(self, target_id: int) -> Optional[int]:
         if self.custom_IDs is not None and target_id in self.target_IDs:
             return self.custom_IDs[self.target_IDs.index(target_id)]
         return None
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/task/__init__.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/task/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""Module for task-related data-modules.
+
+These models import externally from all other model-modules!
+"""
+
 from pathlib import Path
 from typing import List
 from typing import Optional
 from typing import Union
 
 import yaml
 
@@ -29,15 +34,17 @@
     # helper functions
     "prepare_task",
     "extract_tasks",
 ]
 
 
 def prepare_task(config: Union[ShpModel, Path, str], observer: Optional[str] = None) -> Wrapper:
-    """- Opens file (from Path or str of Path)
+    """Open file and extract tasks.
+
+    - Open file (from Path or str of Path)
     - wraps task-model
     - and if it's an TestbedTasks it will extract the correct ObserverTask
     """
     if isinstance(config, str):
         config = Path(config)
 
     if isinstance(config, Path):
@@ -46,15 +53,15 @@
         shp_wrap = Wrapper(**shp_dict)
     elif isinstance(config, ShpModel):
         shp_wrap = Wrapper(
             datatype=type(config).__name__,
             parameters=config.model_dump(),
         )
     else:
-        raise ValueError("had unknown input: %s", type(config))
+        raise TypeError("had unknown input: %s", type(config))
 
     if shp_wrap.datatype == TestbedTasks.__name__:
         if observer is None:
             logger.debug(
                 "Task-Set contained TestbedTasks & no observer was provided "
                 "-> will return TB-Tasks"
             )
@@ -68,15 +75,15 @@
             datatype=type(obt).__name__,
             parameters=obt.model_dump(),
         )
     return shp_wrap
 
 
 def extract_tasks(shp_wrap: Wrapper, *, no_task_sets: bool = True) -> List[ShpModel]:
-    """ """
+    """Make the individual task-sets usable for each observer."""
     if shp_wrap.datatype == ObserverTasks.__name__:
         obt = ObserverTasks(**shp_wrap.parameters)
         content = obt.get_tasks()
     elif shp_wrap.datatype == EmulationTask.__name__:
         content = [EmulationTask(**shp_wrap.parameters)]
     elif shp_wrap.datatype == HarvestTask.__name__:
         content = [HarvestTask(**shp_wrap.parameters)]
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/task/emulation.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/task/emulation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Configuration for the Observer in Emulation-Mode."""
+
 import copy
 from datetime import datetime
 from datetime import timedelta
 from enum import Enum
 from pathlib import Path
 from typing import Optional
 from typing import Union
@@ -22,28 +24,28 @@
 from ..experiment.observer_features import PowerTracing
 from ..experiment.observer_features import SystemLogging
 from ..testbed import Testbed
 from ..testbed.cape import TargetPort
 
 
 class Compression(str, Enum):
-    lzf = "lzf"  # not native hdf5
-    gzip1 = 1  # higher compr & load
-    gzip = 1
-    default = "lzf"
+    """Options for choosing a dataset-compression."""
+
+    lzf = default = "lzf"  # not native hdf5
+    gzip1 = gzip = 1  # higher compr & load
     null = None
     # NOTE: changed to lzf as BBB needs every straw it can get
 
 
 compressions_allowed: list = [None, "lzf", 1]
 c_translate = {"lzf": "lzf", "1": 1, "None": None, None: None}
 
 
 class EmulationTask(ShpModel):
-    """Configuration for the Observer in Emulation-Mode"""
+    """Configuration for the Observer in Emulation-Mode."""
 
     # General config
     input_path: Path
     # ⤷ hdf5 file containing harvesting data
     output_path: Optional[Path] = None
     # ⤷ dir- or file-path for storing the recorded data:
     #   - providing a directory -> file is named emu_timestamp.h5
@@ -107,18 +109,19 @@
 
     @model_validator(mode="after")
     def post_validation(self) -> Self:
         # TODO: limit paths
         has_time = self.time_start is not None
         time_now = datetime.now().astimezone()
         if has_time and self.time_start < time_now:
-            raise ValueError(
+            msg = (
                 "Start-Time for Emulation can't be in the past "
                 f"('{self.time_start}' vs '{time_now}'."
             )
+            raise ValueError(msg)
         if self.duration and self.duration.total_seconds() < 0:
             raise ValueError("Task-Duration can't be negative.")
         if isinstance(self.voltage_aux, str) and self.voltage_aux not in {
             "main",
             "buffer",
         }:
             raise ValueError("Voltage Aux must be in float (0 - 4.5) or string 'main' / 'mid'.")
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/task/firmware_mod.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/task/firmware_mod.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Config for Task that adds the custom ID to the firmware & stores it into a file."""
+
 import copy
 from pathlib import Path
 from typing import Optional
 from typing import TypedDict
 from typing import Union
 
 from pydantic import Field
@@ -20,15 +22,15 @@
 from ..experiment.experiment import Experiment
 from ..testbed import Testbed
 from ..testbed.target import IdInt16
 from ..testbed.target import MCUPort
 
 
 class FirmwareModTask(ShpModel):
-    """Config for Task that adds the custom ID to the firmware & stores it into a file"""
+    """Config for Task that adds the custom ID to the firmware & stores it into a file."""
 
     data: Union[FirmwareStr, Path]
     data_type: FirmwareDType
     custom_id: Optional[IdInt16] = None
     firmware_file: Path
 
     verbose: Annotated[int, Field(ge=0, le=4)] = 2
@@ -75,15 +77,15 @@
     @classmethod
     def from_firmware(
         cls,
         fw: Firmware,
         **kwargs: Unpack[TypedDict],
     ) -> Self:
         if not isinstance(fw, Firmware):
-            raise ValueError("fw-argument must be of type Firmware")
+            raise TypeError("fw-argument must be of type Firmware")
         kwargs["data"] = fw.data
         kwargs["data_type"] = fw.data_type
         fw.compare_hash()
         path = kwargs.get("firmware_file")
         if path is not None and path.is_dir():
             path_new: Path = path / fw.name
             kwargs["firmware_file"] = path_new.with_suffix(".hex")
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/task/harvest.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/task/harvest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Config for the Observer in Harvest-Mode to record IV data from a harvesting-source."""
+
 from datetime import datetime
 from datetime import timedelta
 from pathlib import Path
 from typing import Optional
 
 from pydantic import Field
 from pydantic import model_validator
@@ -13,17 +15,15 @@
 from ..content.virtual_harvester import VirtualHarvesterConfig
 from ..experiment.observer_features import PowerTracing
 from ..experiment.observer_features import SystemLogging
 from .emulation import Compression
 
 
 class HarvestTask(ShpModel):
-    """Configuration for the Observer in Harvest-Mode
-    Record IV data from a harvest-source
-    """
+    """Config for the Observer in Harvest-Mode to record IV data from a harvesting-source."""
 
     # General config
     output_path: Path
     # ⤷ dir- or file-path for storing the recorded data:
     #   - providing a directory -> file is named hrv_timestamp.h5
     #   - for a complete path the filename is not changed except it exists and
     #     overwrite is disabled -> name#num.h5
@@ -69,14 +69,15 @@
 
     @model_validator(mode="after")
     def post_validation(self) -> Self:
         # TODO: limit paths
         has_time = self.time_start is not None
         time_now = datetime.now().astimezone()
         if has_time and self.time_start < time_now:
-            raise ValueError(
+            msg = (
                 "Start-Time for Emulation can't be in the past "
                 f"('{self.time_start}' vs '{time_now}'."
             )
+            raise ValueError(msg)
         if self.duration and self.duration.total_seconds() < 0:
             raise ValueError("Task-Duration can't be negative.")
         return self
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/task/observer_tasks.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/task/observer_tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Collection of tasks for selected observer included in experiment."""
+
 from datetime import datetime
 from datetime import timedelta
 from pathlib import Path
 from typing import List
 from typing import Optional
 
 from pydantic import validate_call
@@ -14,15 +16,15 @@
 from ..testbed.testbed import Testbed
 from .emulation import EmulationTask
 from .firmware_mod import FirmwareModTask
 from .programming import ProgrammingTask
 
 
 class ObserverTasks(ShpModel):
-    """Collection of tasks for selected observer included in experiment"""
+    """Collection of tasks for selected observer included in experiment."""
 
     observer: NameStr
     owner_id: Optional[IdInt]  # TODO: set to optional for now, shouldn't be
 
     # PRE PROCESS
     time_prep: datetime  # TODO: should be optional
     root_path: Path
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/task/programming.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/task/programming.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Config for a Task programming the selected target."""
+
 import copy
 from pathlib import Path
 from typing import Optional
 
 from pydantic import Field
 from pydantic import model_validator
 from pydantic import validate_call
@@ -17,15 +19,15 @@
 from ..testbed.cape import TargetPort
 from ..testbed.mcu import ProgrammerProtocol
 from ..testbed.target import MCUPort
 from ..testbed.testbed import Testbed
 
 
 class ProgrammingTask(ShpModel):
-    """Config for Task programming the target selected"""
+    """Config for a Task programming the selected target."""
 
     firmware_file: Path
     target_port: TargetPort = TargetPort.A
     mcu_port: MCUPort = 1
     mcu_type: SafeStr
     # ⤷ must be either "nrf52" or "msp430" ATM, TODO: clean xp to tasks
     voltage: Annotated[float, Field(ge=1, lt=5)] = 3
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/task/testbed_tasks.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/task/testbed_tasks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Collection of tasks for all observers included in experiment."""
+
 from typing import List
 from typing import Optional
 
 from pydantic import Field
 from pydantic import validate_call
 from typing_extensions import Annotated
 from typing_extensions import Self
@@ -11,15 +13,15 @@
 from ..base.shepherd import ShpModel
 from ..experiment.experiment import Experiment
 from ..testbed.testbed import Testbed
 from .observer_tasks import ObserverTasks
 
 
 class TestbedTasks(ShpModel):
-    """Collection of tasks for all observers included in experiment"""
+    """Collection of tasks for all observers included in experiment."""
 
     name: NameStr
     observer_tasks: Annotated[List[ObserverTasks], Field(min_length=1, max_length=128)]
 
     # POST PROCESS
     email_results: bool = False
     owner_id: Optional[IdInt]
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/testbed/__init__.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/testbed/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+"""Module for testbed-related data-models.
+
+These models import externally from: /base
+"""
+
 from .cape import Cape
 from .cape import TargetPort
 from .gpio import GPIO
 from .gpio import Direction
 from .mcu import MCU
 from .mcu import ProgrammerProtocol
 from .observer import MACStr
 from .observer import Observer
 from .target import IdInt16
 from .target import Target
 from .testbed import Testbed
 
-# these models import externally from: /base
-
 __all__ = [
     "Testbed",
     "Observer",
     "Cape",
     "Target",
     "MCU",
     "GPIO",
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/testbed/cape.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/testbed/target.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,61 @@
-from datetime import date
+"""meta-data representation of a testbed-component (physical object)."""
+
 from datetime import datetime
-from enum import Enum
 from typing import Optional
 from typing import Union
 
 from pydantic import Field
 from pydantic import model_validator
+from typing_extensions import Annotated
 
 from ...testbed_client import tb_client
 from ..base.content import IdInt
 from ..base.content import NameStr
 from ..base.content import SafeStr
 from ..base.shepherd import ShpModel
+from .mcu import MCU
 
+IdInt16 = Annotated[int, Field(ge=0, lt=2**16)]
 
-class TargetPort(str, Enum):
-    A = "A"
-    B = "B"
-    a = "A"
-    b = "B"
+MCUPort = Annotated[int, Field(ge=1, le=2)]
 
 
-class Cape(ShpModel, title="Shepherd-Cape"):
-    """meta-data representation of a testbed-component (physical object)"""
+class Target(ShpModel, title="Target Node (DuT)"):
+    """meta-data representation of a testbed-component (physical object)."""
 
     id: IdInt
     name: NameStr
     version: NameStr
     description: SafeStr
+
     comment: Optional[SafeStr] = None
-    # TODO: wake_interval, calibration
 
     active: bool = True
-    created: Union[date, datetime] = Field(default_factory=datetime.now)
-    calibrated: Union[date, datetime, None] = None
+    created: datetime = Field(default_factory=datetime.now)
+
+    testbed_id: Optional[IdInt16] = None
+    # ⤷ is derived from ID (targets are still selected by id!)
+    mcu1: Union[MCU, NameStr]
+    mcu2: Union[MCU, NameStr, None] = None
+
+    # TODO: programming pins per mcu should be here (or better in Cape)
 
     def __str__(self) -> str:
         return self.name
 
     @model_validator(mode="before")
     @classmethod
     def query_database(cls, values: dict) -> dict:
         values, _ = tb_client.try_completing_model(cls.__name__, values)
+
+        # post correction
+        for _mcu in ["mcu1", "mcu2"]:
+            if isinstance(values.get(_mcu), str):
+                values[_mcu] = MCU(name=values[_mcu])
+                # ⤷ this will raise if default is faulty
+            elif isinstance(values.get(_mcu), dict):
+                values[_mcu] = MCU(**values[_mcu])
+        if values.get("testbed_id") is None:
+            values["testbed_id"] = values.get("id") % 2**16
+
         return values
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/testbed/gpio.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/testbed/gpio.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""meta-data representation of a testbed-component (physical object)."""
+
 from enum import Enum
 from typing import Optional
 
 from pydantic import Field
 from pydantic import StringConstraints
 from pydantic import model_validator
 from typing_extensions import Annotated
@@ -11,24 +13,23 @@
 from ..base.content import IdInt
 from ..base.content import NameStr
 from ..base.content import SafeStr
 from ..base.shepherd import ShpModel
 
 
 class Direction(str, Enum):
-    Input = "IN"
-    IN = "IN"
-    Output = "OUT"
-    OUT = "OUT"
-    Bidirectional = "IO"
-    IO = "IO"
+    """Options for pin-direction."""
+
+    Input = IN = "IN"
+    Output = OUT = "OUT"
+    Bidirectional = IO = "IO"
 
 
 class GPIO(ShpModel, title="GPIO of Observer Node"):
-    """meta-data representation of a testbed-component"""
+    """meta-data representation of a testbed-component."""
 
     id: IdInt
     name: NameStr
     description: Optional[SafeStr] = None
     comment: Optional[SafeStr] = None
 
     direction: Direction = Direction.Input
@@ -50,15 +51,16 @@
 
     @model_validator(mode="after")
     def post_validation(self) -> Self:
         # ensure that either pru or sys is used, otherwise instance is considered faulty
         no_pru = (self.reg_pru is None) or (self.pin_pru is None)
         no_sys = (self.reg_sys is None) or (self.pin_sys is None)
         if no_pru and no_sys:
-            raise ValueError(
+            msg = (
                 "GPIO-Instance is faulty -> "
                 f"it needs to use pru or sys, content: {self.model_dump()}"
             )
+            raise ValueError(msg)
         return self
 
     def user_controllable(self) -> bool:
         return ("gpio" in self.name.lower()) and (self.direction in {"IO", "OUT"})
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/testbed/mcu.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/testbed/mcu.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""meta-data representation of a testbed-component (physical object)."""
+
 from enum import Enum
 from typing import Optional
 
 from pydantic import Field
 from pydantic import model_validator
 from typing_extensions import Annotated
 
@@ -9,26 +11,24 @@
 from ..base.content import IdInt
 from ..base.content import NameStr
 from ..base.content import SafeStr
 from ..base.shepherd import ShpModel
 
 
 class ProgrammerProtocol(str, Enum):
-    SWD = "SWD"
-    swd = "SWD"
-    SBW = "SBW"
-    sbw = "SBW"
-    JTAG = "JTAG"
-    jtag = "JTAG"
-    UART = "UART"
-    uart = "UART"
+    """Options regarding the programming-protocol."""
+
+    SWD = swd = "SWD"
+    SBW = sbw = "SBW"
+    JTAG = jtag = "JTAG"
+    UART = uart = "UART"
 
 
 class MCU(ShpModel, title="Microcontroller of the Target Node"):
-    """meta-data representation of a testbed-component (physical object)"""
+    """meta-data representation of a testbed-component (physical object)."""
 
     id: IdInt
     name: NameStr
     description: SafeStr
     comment: Optional[SafeStr] = None
 
     platform: NameStr
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/testbed/observer.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/testbed/observer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""meta-data representation of a testbed-component (physical object)."""
+
 from datetime import datetime
 from typing import Optional
 
 from pydantic import Field
 from pydantic import IPvAnyAddress
 from pydantic import StringConstraints
 from pydantic import model_validator
@@ -20,15 +22,15 @@
 MACStr = Annotated[
     str,
     StringConstraints(max_length=17, pattern=r"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$"),
 ]
 
 
 class Observer(ShpModel, title="Shepherd-Sheep"):
-    """meta-data representation of a testbed-component (physical object)"""
+    """meta-data representation of a testbed-component (physical object)."""
 
     id: IdInt
     name: NameStr
     description: SafeStr
     comment: Optional[SafeStr] = None
 
     ip: IPvAnyAddress
@@ -59,15 +61,16 @@
         return values
 
     @model_validator(mode="after")
     def post_validation(self) -> Self:
         has_cape = self.cape is not None
         has_target = (self.target_a is not None) or (self.target_b is not None)
         if not has_cape and has_target:
-            raise ValueError(f"Observer '{self.name}' is faulty -> has targets but no cape")
+            msg = f"Observer '{self.name}' is faulty -> has targets but no cape"
+            raise ValueError(msg)
         return self
 
     def has_target(self, target_id: int) -> bool:
         if self.target_a is not None and target_id == self.target_a.id and self.target_a.active:
             return True
         if self.target_b is not None and target_id == self.target_b.id and self.target_b.active:
             return True
@@ -75,16 +78,18 @@
 
     def get_target_port(self, target_id: int) -> TargetPort:
         if self.has_target(target_id):
             if self.target_a is not None and target_id == self.target_a.id:
                 return TargetPort.A
             if self.target_b is not None and target_id == self.target_b.id:
                 return TargetPort.B
-        raise ValueError(f"Target-ID {target_id} was not found in Observer '{self.name}'")
+        msg = f"Target-ID {target_id} was not found in Observer '{self.name}'"
+        raise KeyError(msg)
 
     def get_target(self, target_id: int) -> Target:
         if self.has_target(target_id):
             if self.target_a is not None and target_id == self.target_a.id:
                 return self.target_a
             if self.target_b is not None and target_id == self.target_b.id:
                 return self.target_b
-        raise ValueError(f"Target-ID {target_id} was not found in Observer '{self.name}'")
+        msg = f"Target-ID {target_id} was not found in Observer '{self.name}'"
+        raise KeyError(msg)
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/testbed/target.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/testbed/cape.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,47 @@
+"""meta-data representation of a testbed-component (physical object)."""
+
+from datetime import date
 from datetime import datetime
+from enum import Enum
 from typing import Optional
 from typing import Union
 
 from pydantic import Field
 from pydantic import model_validator
-from typing_extensions import Annotated
 
 from ...testbed_client import tb_client
 from ..base.content import IdInt
 from ..base.content import NameStr
 from ..base.content import SafeStr
 from ..base.shepherd import ShpModel
-from .mcu import MCU
 
-IdInt16 = Annotated[int, Field(ge=0, lt=2**16)]
 
-MCUPort = Annotated[int, Field(ge=1, le=2)]
+class TargetPort(str, Enum):
+    """Options for choosing a target-port."""
+
+    A = a = "A"
+    B = b = "B"
 
 
-class Target(ShpModel, title="Target Node (DuT)"):
-    """meta-data representation of a testbed-component (physical object)"""
+class Cape(ShpModel, title="Shepherd-Cape"):
+    """meta-data representation of a testbed-component (physical object)."""
 
     id: IdInt
     name: NameStr
     version: NameStr
     description: SafeStr
-
     comment: Optional[SafeStr] = None
+    # TODO: wake_interval, calibration
 
     active: bool = True
-    created: datetime = Field(default_factory=datetime.now)
-
-    testbed_id: Optional[IdInt16] = None
-    # ⤷ is derived from ID (targets are still selected by id!)
-    mcu1: Union[MCU, NameStr]
-    mcu2: Union[MCU, NameStr, None] = None
-
-    # TODO programming pins per mcu should be here (or better in Cape)
+    created: Union[date, datetime] = Field(default_factory=datetime.now)
+    calibrated: Union[date, datetime, None] = None
 
     def __str__(self) -> str:
         return self.name
 
     @model_validator(mode="before")
     @classmethod
     def query_database(cls, values: dict) -> dict:
         values, _ = tb_client.try_completing_model(cls.__name__, values)
-
-        # post correction
-        for _mcu in ["mcu1", "mcu2"]:
-            if isinstance(values.get(_mcu), str):
-                values[_mcu] = MCU(name=values[_mcu])
-                # ⤷ this will raise if default is faulty
-            elif isinstance(values.get(_mcu), dict):
-                values[_mcu] = MCU(**values[_mcu])
-        if values.get("testbed_id") is None:
-            values["testbed_id"] = values.get("id") % 2**16
-
         return values
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/data_models/testbed/testbed.py` & `shepherd_core-2024.4.2/shepherd_core/data_models/testbed/testbed.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""meta-data representation of a testbed-component (physical object)."""
+
 from datetime import timedelta
 from pathlib import Path
 from typing import List
 from typing import Optional
 
 from pydantic import Field
 from pydantic import HttpUrl
@@ -14,15 +16,15 @@
 from ..base.content import NameStr
 from ..base.content import SafeStr
 from ..base.shepherd import ShpModel
 from .observer import Observer
 
 
 class Testbed(ShpModel):
-    """meta-data representation of a testbed-component (physical object)"""
+    """meta-data representation of a testbed-component (physical object)."""
 
     id: IdInt
     name: NameStr
     description: SafeStr
     comment: Optional[SafeStr] = None
 
     url: Optional[HttpUrl] = None
@@ -83,8 +85,9 @@
     def get_observer(self, target_id: int) -> Observer:
         for _observer in self.observers:
             if not _observer.active or not _observer.cape.active:
                 # skip decommissioned setups
                 continue
             if _observer.has_target(target_id):
                 return _observer
-        raise ValueError(f"Target-ID {target_id} was not found in Testbed '{self.name}'")
+        msg = f"Target-ID {target_id} was not found in Testbed '{self.name}'"
+        raise ValueError(msg)
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/decoder_waveform/uart.py` & `shepherd_core-2024.4.2/shepherd_core/decoder_waveform/uart.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-"""UART - Decoder - Features:
+"""UART - Decoder.
+
+Features:
+
 - 1 bit Start (LOW)
 - 1 .. **8** .. 64 bit data-frame
 - **1**, 1.5, 2 bit stop (HIGH) - don't care?
 - **no**, even, odd parity bit (there are more, see sigrok-link) - TODO
 - **LSB** / MSB first - detectable with dict-compare - TODO
 - **no** inversion
 
 Todo:
-----
-  - detect bitOrder
-  - detect dataframe length
-  - detect parity
+- detect bitOrder
+- detect dataframe length
+- detect parity
 
 More Info:
+
 https://en.wikipedia.org/wiki/Universal_asynchronous_receiver-transmitter
 https://sigrok.org/wiki/Protocol_decoder:Uart
 
 """
 
 from enum import Enum
 from pathlib import Path
@@ -25,40 +28,48 @@
 
 import numpy as np
 
 from ..logger import logger
 
 
 class Parity(str, Enum):
+    """Options for parity-property of UART data-frame."""
+
     no = "no"
     even = "odd"
     odd = "even"
 
 
 class BitOrder(str, Enum):
-    msb = "msb"
-    msb_first = "msb"
-    lsb = "lsb"
-    lsb_first = "lsb"
+    """Options for bit-order-property of UART data-frame."""
+
+    msb = msb_first = "msb"
+    lsb = lsb_first = "lsb"
 
 
 class Uart:
+    """Specialized UART decoder."""
+
     def __init__(
         self,
         content: Union[Path, np.ndarray],
         baud_rate: Optional[int] = None,
         frame_length: Optional[int] = 8,
         inversion: Optional[bool] = None,
         parity: Optional[Parity] = Parity.no,
         bit_order: Optional[BitOrder] = BitOrder.lsb_first,
     ) -> None:
-        """Provide a file with two columns:
-        - timestamp (seconds with fraction) and signal (can be analog).
-        - class-parameters that are None (above) get auto-detected
-          (some detectors still missing)
+        """Provide a file with two columns: TS & Signal.
+
+        Constraints:
+        - timestamp -> seconds with fraction
+        - signal -> can be analog or digital
+
+        Note: class-parameters that are None (above) get auto-detected
+          (some detectors still missing).
         """
         if isinstance(content, Path):
             self.events_sig: np.ndarray = np.loadtxt(content.as_posix(), delimiter=",", skiprows=1)
             # TODO: if float fails load as str -
             #  cast first col as np.datetime64 with ns-resolution, convert to delta
         else:
             self.events_sig = content
@@ -105,89 +116,96 @@
 
         # results
         self.events_symbols: Optional[np.ndarray] = None
         self.events_lines: Optional[np.ndarray] = None
         self.text: Optional[str] = None
 
     def _convert_analog2digital(self, *, invert: bool = False) -> None:
-        """Divide dimension in two, divided by mean-value"""
+        """Divide dimension in two, divided by mean-value."""
         data = self.events_sig[:, 1]
         mean = np.mean(data)
         if invert:
             self.events_sig[:, 1] = data <= mean
         else:
             self.events_sig[:, 1] = data >= mean
 
     def _filter_redundant_states(self) -> None:
-        """Sum of two sequential states is always 1 (True + False) if alternating"""
+        """Sum of two sequential states is always 1 (True + False) if alternating."""
         data_0 = self.events_sig[:, 1]
         data_1 = np.concatenate([[not data_0[0]], data_0[:-1]])
         data_f = data_0 + data_1
         self.events_sig = self.events_sig[data_f == 1]
 
         if len(data_0) > len(self.events_sig):
             logger.debug(
                 "filtered out %d/%d events (redundant)",
                 len(data_0) - len(self.events_sig),
                 len(data_0),
             )
 
     def _add_duration(self) -> None:
-        """Calculate third column -> duration of state in [baud-ticks]"""
+        """Calculate third column -> duration of state in [baud-ticks]."""
         if self.events_sig.shape[1] > 2:
             logger.warning("Tried to add state-duration, but it seems already present")
             return
         if not hasattr(self, "dur_tick"):
             raise ValueError("Make sure that baud-rate was calculated before running add_dur()")
         dur_steps = self.events_sig[1:, 0] - self.events_sig[:-1, 0]
         dur_steps = np.reshape(dur_steps, (dur_steps.size, 1))
         self.events_sig = np.append(self.events_sig[:-1, :], dur_steps / self.dur_tick, axis=1)
 
     def detect_inversion(self) -> bool:
-        """Analyze bit-state during long pauses (unchanged states)
+        """Analyze bit-state during long pauses (unchanged states).
+
         - pause should be HIGH for non-inverted mode (default)
         - assumes max frame size of 64 bit + x for safety
         """
         events = self.events_sig[:1000, :]  # speedup for large datasets
         pauses = events[:, 2] > 80
         states_1 = events[:, 1]
         pause_states = states_1[pauses]
         mean_state = pause_states.mean()
         if 0.1 < mean_state < 0.9:
             raise ValueError("Inversion in pauses could not be detected")
         return mean_state < 0.5
 
     def detect_baud_rate(self) -> int:
-        """Analyze the smallest step"""
+        """Analyze the smallest step."""
         events = self.events_sig[:1000, :]  # speedup for large datasets
         dur_steps = events[1:, 0] - events[:-1, 0]
         def_step = np.percentile(dur_steps[dur_steps > 0], 10)
         mean_tick = dur_steps[
             (dur_steps >= 0.66 * def_step) & (dur_steps <= 1.33 * def_step)
         ].mean()
         return round(1 / mean_tick)
 
     def detect_half_stop(self) -> bool:
-        """Looks into the spacing between time-steps"""
+        """Look into the spacing between time-steps to determine use of half stop."""
         events = self.events_sig[:1000, :]  # speedup for large datasets
         return np.sum((events > 1.333 * self.dur_tick) & (events < 1.667 * self.dur_tick)) > 0
 
     def detect_dataframe_length(self) -> int:
-        """Look after longest pauses
-        - accumulate steps until a state with uneven step-size is found
+        """Try to determine length of dataframe.
+
+        Algo will look for longest pauses & accumulate steps until
+        a state with uneven step-size is found.
         """
+        raise NotImplementedError
 
     def get_symbols(self, *, force_redo: bool = False) -> np.ndarray:
-        """Ways to detect EOF:
+        """Extract symbols from events.
+
+        Ways to detect EOF:
         - long pause on HIGH
         - off_tick pause on high
         - bit_pos > max
+
         # TODO:
             - slowest FN -> speedup with numba or parallelization?
-            - dset could be divided (long pauses) and threaded for speedup
+            - dset could be divided (long pauses) and threaded for speedup.
         """
         if force_redo:
             self.events_symbols = None
         if self.events_symbols is not None:
             return self.events_symbols
 
         pos_df = None
@@ -231,15 +249,15 @@
         self.events_symbols = np.concatenate(content).reshape((len(content), 2))
         # TODO: numpy is converting timestamp to string -> must be added as tuple (ts, symbol)
         # symbol_events[:, 0] = symbol_events[:, 0].astype(float)  # noqa: ERA001
         # ⤷ does not work
         return self.events_symbols
 
     def get_lines(self, *, force_redo: bool = False) -> np.ndarray:
-        """Timestamped symbols to line, cut at \r, \r\n or \n"""
+        r"""Timestamped symbols to line, cut at \r, \r\n or \n."""
         if force_redo:
             self.events_lines = None
         if self.events_lines is not None:
             return self.events_lines
         if self.events_symbols is None:
             self.get_symbols()
 
@@ -263,15 +281,15 @@
             if t_start is None:
                 t_start = time
             line += symbol
         self.events_lines = np.concatenate(content).reshape((len(content), 2))
         return self.events_lines
 
     def get_text(self, *, force_redo: bool = False) -> str:
-        """Remove timestamps and just return the whole string"""
+        """Remove timestamps and just return the whole string."""
         if force_redo:
             self.text = None
         if self.text is not None:
             return self.text
         if self.events_lines is None:
             self.get_lines()
         self.text = "".join(self.events_lines[:, 1])
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/fw_tools/__init__.py` & `shepherd_core-2024.4.2/shepherd_core/fw_tools/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Helper-functions for handling firmware around the testbed."""
+
 from typing import Any
 
 try:
     from importlib.util import find_spec
 
     find_spec("pwnlib.elf.ELF")
 except ImportError:
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/fw_tools/converter.py` & `shepherd_core-2024.4.2/shepherd_core/fw_tools/converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Content-Converters for firmwares."""
+
 import base64
 import hashlib
 import shutil
 from pathlib import Path
 from typing import Union
 
 import zstandard as zstd
@@ -11,72 +13,81 @@
 from .converter_elf import elf_to_hex
 from .validation import is_elf
 from .validation import is_hex
 
 
 @validate_call
 def firmware_to_hex(file_path: Path) -> Path:
-    """Generic converter that handles ELF & HEX"""
+    """Convert ELF-Files to HEX.
+
+    Generic converter that handles ELF & HEX.
+    """
     if not file_path.is_file():
-        raise ValueError("Fn needs an existing file as input")
+        raise FileNotFoundError("Fn needs an existing file as input")
     if is_elf(file_path):
         return elf_to_hex(file_path)
     if is_hex(file_path):
         return file_path
-    raise ValueError("FW2Hex: unknown file '%s', it should be ELF or HEX", file_path.name)
+    raise FileNotFoundError("FW2Hex: unknown file '%s', it should be ELF or HEX", file_path.name)
 
 
 @validate_call
 def file_to_base64(file_path: Path) -> str:
-    """Compress and encode content of file
+    """Compress and encode content of file.
+
     - base64 adds ~33 % overhead
-    - zstd compression ~ 1:3
+    - zstd compression reduces to ~ 1:3
     """
     if not file_path.is_file():
         raise ValueError("Fn needs an existing file as input")
     with file_path.resolve().open("rb") as file:
         file_content = file.read()
     file_cmpress = zstd.ZstdCompressor(level=20).compress(file_content)
     return base64.b64encode(file_cmpress).decode("ascii")
 
 
 @validate_call
 def base64_to_file(content: str, file_path: Path) -> None:
-    """DeCompress and decode Content of file
+    """DeCompress and decode Content of file.
+
     - base64 adds ~33 % overhead
-    - zstd compression ~ 1:3
+    - zstd compression reduces to ~ 1:3
     """
     file_cmpress = base64.b64decode(content)
     file_content = zstd.ZstdDecompressor().decompress(file_cmpress)
     if not file_path.parent.exists():
         file_path.parent.mkdir(parents=True)
     with file_path.resolve().open("wb") as file:
         file.write(file_content)
 
 
 @validate_call
 def file_to_hash(file_path: Path) -> str:
+    """Convert file-content to hash-value."""
     if not file_path.is_file():
         raise ValueError("Fn needs an existing file as input")
     with file_path.resolve().open("rb") as file:
         file_content = file.read()
     return hashlib.sha3_224(file_content).hexdigest()
 
 
 @validate_call
 def base64_to_hash(content: str) -> str:
+    """Convert base64-content to hash-value."""
     file_cmpress = base64.b64decode(content)
     file_content = zstd.ZstdDecompressor().decompress(file_cmpress)
     return hashlib.sha3_224(file_content).hexdigest()
 
 
 @validate_call
 def extract_firmware(data: Union[str, Path], data_type: FirmwareDType, file_path: Path) -> Path:
-    """- base64-string will be transformed into file
-    - if data is a path the file will be copied to the destination
+    """Make embedded firmware-data usable in filesystem.
+
+    - base64-string will be transformed to file
+    - if data is a path the file will be copied to the destination.
     """
     if data_type == FirmwareDType.base64_elf:
         file = file_path.with_suffix(".elf")
         base64_to_file(data, file)
     elif data_type == FirmwareDType.base64_hex:
         file = file_path.with_suffix(".hex")
         base64_to_file(data, file)
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/fw_tools/converter_elf.py` & `shepherd_core-2024.4.2/shepherd_core/fw_tools/converter_elf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+"""Converter for ELF-files."""
+
 import subprocess
 from pathlib import Path
 from typing import Optional
 
 from pydantic import validate_call
 
 # extra src-file necessary to prevent circular import
 
 
 @validate_call
 def elf_to_hex(file_elf: Path, file_hex: Optional[Path] = None) -> Path:
+    """Convert ELF to hex file using objcopy."""
     if not file_elf.is_file():
         raise ValueError("Fn needs an existing file as input")
     if not file_hex:
         file_hex = file_elf.resolve().with_suffix(".hex")
     cmd = ["objcopy", "-O", "ihex", file_elf.resolve().as_posix(), file_hex.as_posix()]
     # TODO: observe - maybe $ARCH-Versions of objcopy are needed
     #  (hex of nRF / msp identical between the 3 $arch-versions)
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/fw_tools/patcher.py` & `shepherd_core-2024.4.2/shepherd_core/fw_tools/patcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Read and modify symbols in ELF-files."""
+
 from pathlib import Path
 from typing import Optional
 
 from pydantic import Field
 from pydantic import validate_call
 from typing_extensions import Annotated
 
@@ -18,14 +20,15 @@
         "Please install functionality with 'pip install shepherd_core[elf] -U' first, "
         f"underlying exception: {e.msg}"
     )
 
 
 @validate_call
 def find_symbol(file_elf: Path, symbol: str) -> bool:
+    """Find a symbol in the ELF file."""
     if symbol is None or not is_elf(file_elf):
         return False
     if ELF is None:
         raise RuntimeError(elf_error_text)
     elf = ELF(path=file_elf)
     try:
         addr = elf.symbols[symbol]
@@ -43,31 +46,36 @@
     )
     elf.close()
     return True
 
 
 @validate_call
 def read_symbol(file_elf: Path, symbol: str, length: int = uid_len_default) -> Optional[int]:
-    """Interpreted as int"""
+    """Read value of symbol in ELF-File.
+
+    Will be interpreted as int.
+    """
     if not find_symbol(file_elf, symbol):
         return None
     if ELF is None:
         raise RuntimeError(elf_error_text)
     elf = ELF(path=file_elf)
     addr = elf.symbols[symbol]
     value_raw = elf.read(address=addr, count=length)[-length:]
     elf.close()
     return int.from_bytes(bytes=value_raw, byteorder=elf.endian, signed=False)
 
 
 def read_uid(file_elf: Path) -> Optional[int]:
+    """Read value of UID-symbol for shepherd testbed."""
     return read_symbol(file_elf, symbol=uid_str_default, length=uid_len_default)
 
 
 def read_arch(file_elf: Path) -> Optional[str]:
+    """Determine chip-architecture from elf-metadata."""
     if not is_elf(file_elf):
         return None
     if ELF is None:
         raise RuntimeError(elf_error_text)
     elf = ELF(path=file_elf)
     if "exec" in elf.elftype.lower():
         return elf.arch.lower()
@@ -79,17 +87,20 @@
 def modify_symbol_value(
     file_elf: Path,
     symbol: str,
     value: Annotated[int, Field(ge=0, lt=2 ** (8 * uid_len_default))],
     *,
     overwrite: bool = False,
 ) -> Optional[Path]:
-    """Replaces value of symbol in ELF-File, hardcoded for uint16_t (2 byte)
-    testbed uses FN to patch firmware with custom target-ID
-    NOTE: can overwrite provided file
+    """Replace value of uint16-symbol in ELF-File.
+
+    Hardcoded for uint16_t (2 byte).
+    The testbed uses this to patch firmware with custom target-ID.
+
+    NOTE: can overwrite provided file.
 
     """
     if not find_symbol(file_elf, symbol):
         return None
     if ELF is None:
         raise RuntimeError(elf_error_text)
     elf = ELF(path=file_elf)
@@ -117,8 +128,9 @@
         hex(value),
         hex(addr),
     )
     return file_new
 
 
 def modify_uid(file_elf: Path, value: int) -> Optional[Path]:
+    """Replace value of UID-symbol for shepherd testbed."""
     return modify_symbol_value(file_elf, symbol=uid_str_default, value=value, overwrite=True)
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/fw_tools/validation.py` & `shepherd_core-2024.4.2/shepherd_core/fw_tools/validation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-"""TODO: Work in Progress"""
+"""Helper-functions for firmware-validation.
+
+TODO: Work in Progress.
+    - Each arch should have its own file and
+    - detection-functions that register in main validator.
+"""
 
 import tempfile
 from pathlib import Path
 
 from intelhex import IntelHex
 from intelhex import IntelHexError
 from pydantic import validate_call
@@ -21,25 +26,28 @@
         "Please install functionality with 'pip install shepherd_core[elf] -U' first, "
         f"underlying exception: {e.msg}"
     )
 
 
 @validate_call
 def is_hex(file: Path) -> bool:
+    """Check if file is containing intel-hex data."""
     try:
         _ = IntelHex(file.as_posix())
     except ValueError:  # parsing
         return False
     except IntelHexError:  # structural errors
         return False
     return True
 
 
 def is_hex_msp430(file: Path) -> bool:
-    """Observations:
+    """Try to detect specifics for that MCU.
+
+    Observations:
     - addresses begin at 0x4000
     - value @0xFFFE (IVT) is start_address (of pgm-code)
     """
     if is_hex(file):
         ih = IntelHex(file.as_posix())
         if ih.minaddr() != 0x4000:
             return False
@@ -52,15 +60,17 @@
             # conservative test for now - should be well below 128 kB + 8kB for msp430fr5962
             return False
         return True
     return False
 
 
 def is_hex_nrf52(file: Path) -> bool:
-    """Observations:
+    """Try to detect specifics for that MCU.
+
+    Observations:
     - addresses begin at 0x0
     - only one segment (.get_segments), todo
     """
     if is_hex(file):
         ih = IntelHex(file.as_posix())
         if ih.minaddr() != 0x0000:
             return False
@@ -75,59 +85,70 @@
 #  - remove conversion to hex
 #  - use elftools to verify magic-bytes and similar things done for the hex
 #  https://github.com/eliben/pyelftools/wiki/User's-guide
 
 
 @validate_call
 def is_elf(file: Path) -> bool:
+    """Check if file is an ELF file."""
     if ELF is None:
         raise RuntimeError(elf_error_text)
     if not file.is_file():
         return False
     try:
         _ = ELF(path=file)
     except ELFError:
         logger.debug("File %s is not ELF - Magic number does not match", file.name)
         return False
     return True
 
 
-def is_elf_msp430(file: Path) -> bool:  # TODO: allow detection without conversion
+def is_elf_msp430(file: Path) -> bool:
+    """Check if file is an ELF for that MCU.
+
+    TODO: allow detection without conversion
+    """
     if is_elf(file):
         with tempfile.TemporaryDirectory() as path:
             file_hex = Path(path) / "file.hex"
             file_hex = elf_to_hex(file, file_hex)
             if is_hex_msp430(file_hex):
                 return True
         return False
     return False
 
 
-def is_elf_nrf52(file: Path) -> bool:  # TODO: allow detection without conversion
+def is_elf_nrf52(file: Path) -> bool:
+    """Check if file is an ELF for that MCU.
+
+    TODO: allow detection without conversion
+    """
     if is_elf(file):
         with tempfile.TemporaryDirectory() as path:
             file_hex = Path(path) / "file.hex"
             file_hex = elf_to_hex(file, file_hex)
             if is_hex_nrf52(file_hex):
                 return True
         return False
     return False
 
 
 def determine_type(file: Path) -> FirmwareDType:
+    """Figure out file-type (hex or elf)."""
     if not file.is_file():
         raise ValueError("Fn needs an existing file as input")
     if is_hex(file):
         return FirmwareDType.path_hex
     if is_elf(file):
         return FirmwareDType.path_elf
     raise ValueError("Type of file '%s' could not be determined", file.name)
 
 
 def determine_arch(file: Path) -> str:
+    """Figure out arch (msp430 or nrf52)."""
     file_t = determine_type(file)
     if file_t == FirmwareDType.path_elf:
         if is_elf_nrf52(file):
             return "nrf52"
         if is_elf_msp430(file):
             return "msp430"
         raise ValueError("Arch of ELF '%s' could not be determined", file.name)
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/inventory/__init__.py` & `shepherd_core-2024.4.2/shepherd_core/inventory/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-"""Creates an overview for shepherd-host-machines with:
+"""Creates an overview for shepherd-host-machines.
+
+This will collect:
 - relevant software-versions
 - system-parameters
-- hardware-config
+- hardware-config.
 """
 
 from datetime import datetime
 from datetime import timedelta
 from pathlib import Path
 from typing import List
 
@@ -24,15 +26,19 @@
     "PythonInventory",
     "SystemInventory",
     "TargetInventory",
 ]
 
 
 class Inventory(PythonInventory, SystemInventory, TargetInventory):
-    # has all child-parameters
+    """Complete inventory for one device.
+
+    Has all child-parameters.
+    """
+
     hostname: str
     created: datetime
 
     @classmethod
     def collect(cls) -> Self:
         # one by one for more precise error messages
         # NOTE: system is first, as it must take a precise timestamp
@@ -43,20 +49,24 @@
         # make important metadata available at root level
         model["created"] = sid["timestamp"]
         model["hostname"] = sid["hostname"]
         return cls(**model)
 
 
 class InventoryList(ShpModel):
+    """Collection of inventories for several devices."""
+
     elements: Annotated[List[Inventory], Field(min_length=1)]
 
     def to_csv(self, path: Path) -> None:
-        """TODO: pretty messed up (raw lists and dicts for sub-elements)
+        """Generate a CSV.
+
+        TODO: pretty messed up (raw lists and dicts for sub-elements)
         numpy.savetxt -> too basic
-        np.concatenate(content).reshape((len(content), len(content[0])))
+        np.concatenate(content).reshape((len(content), len(content[0]))).
         """
         if path.is_dir():
             path = path / "inventory.yaml"
         with path.resolve().open("w") as fd:
             fd.write(", ".join(self.elements[0].model_dump().keys()) + "\r\n")
             for item in self.elements:
                 content = list(item.model_dump().values())
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/inventory/python.py` & `shepherd_core-2024.4.2/shepherd_core/inventory/python.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+"""Python related inventory model."""
+
 import platform
 from contextlib import suppress
 from importlib import import_module
 from typing import Optional
 
 from pydantic import ConfigDict
 from typing_extensions import Self
 
 from ..data_models import ShpModel
 
 
 class PythonInventory(ShpModel):
+    """Python related inventory model."""
+
     # program versions
     h5py: Optional[str] = None
     numpy: Optional[str] = None
     pydantic: Optional[str] = None
     python: Optional[str] = None
     shepherd_core: Optional[str] = None
     shepherd_sheep: Optional[str] = None
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/inventory/system.py` & `shepherd_core-2024.4.2/shepherd_core/inventory/system.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,35 @@
+"""System / OS related inventory model."""
+
 import platform
 import subprocess
 import time
 from contextlib import suppress
 from datetime import datetime
 from typing import Optional
 
 from typing_extensions import Self
 
-from .. import local_now
-from .. import logger
+from ..data_models.base.timezone import local_now
+from ..logger import logger
 
 try:
     import psutil
 except ImportError:
     psutil = None
 
 from pydantic import ConfigDict
 from pydantic.types import PositiveInt
 
 from ..data_models import ShpModel
 
 
 class SystemInventory(ShpModel):
+    """System / OS related inventory model."""
+
     uptime: PositiveInt
     # ⤷ seconds
     timestamp: datetime
     # time_delta: timedelta = timedelta(0)  # noqa: ERA001
     # ⤷ lag behind earliest observer, TODO: wrong place
 
     system: str
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/logger.py` & `shepherd_core-2024.4.2/shepherd_core/logger.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+"""Log handler of shepherd."""
+
 import logging
 import logging.handlers
 from typing import Union
 
 import chromalog
 
 chromalog.basicConfig(format="%(message)s")
 logger = logging.getLogger("SHPCore")
 logger.addHandler(logging.NullHandler())
 
 verbose_level: int = 2
 
 
 def get_verbose_level() -> int:
+    """Get log level of shepherd."""
     return verbose_level
 
 
 def set_log_verbose_level(log_: Union[logging.Logger, logging.Handler], verbose: int) -> None:
+    """Set log level of shepherd."""
     if verbose == 0:
         log_.setLevel(logging.ERROR)
         logging.basicConfig(level=logging.ERROR)
     elif verbose == 1:
         log_.setLevel(logging.WARNING)
     elif verbose == 2:
         log_.setLevel(logging.INFO)
@@ -35,14 +39,15 @@
     if verbose > 2:
         chromalog.basicConfig(format="%(name)s %(levelname)s: %(message)s")
     else:
         chromalog.basicConfig(format="%(message)s")  # reduce internals
 
 
 def increase_verbose_level(verbose: int) -> None:
+    """Increase log level of shepherd."""
     global verbose_level  # noqa: PLW0603
     if verbose >= verbose_level:
         verbose_level = min(max(verbose, 0), 3)
         set_log_verbose_level(logger, verbose_level)
 
 
 increase_verbose_level(2)
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/reader.py` & `shepherd_core-2024.4.2/shepherd_core/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-"""Reader-Baseclass"""
+"""Reader-Baseclass."""
+
+from __future__ import annotations
 
 import contextlib
 import errno
 import logging
 import math
 import os
 from itertools import product
 from pathlib import Path
-from types import TracebackType
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import ClassVar
 from typing import Dict
 from typing import Generator
 from typing import List
 from typing import Optional
 from typing import Type
@@ -26,14 +28,17 @@
 
 from .commons import samplerate_sps_default
 from .data_models.base.calibration import CalibrationPair
 from .data_models.base.calibration import CalibrationSeries
 from .data_models.content.energy_environment import EnergyDType
 from .decoder_waveform import Uart
 
+if TYPE_CHECKING:
+    from types import TracebackType
+
 
 class Reader:
     """Sequentially Reads shepherd-data from HDF5 file.
 
     Args:
     ----
         file_path: Path of hdf5 file containing shepherd data with iv-samples, iv-curves or isc&voc
@@ -92,15 +97,16 @@
                     errno.ENOENT, os.strerror(errno.ENOENT), self.file_path.name
                 )
 
             try:
                 self.h5file = h5py.File(self.file_path, "r")  # = readonly
                 self._reader_opened = True
             except OSError as _xcp:
-                raise TypeError(f"Unable to open HDF5-File '{self.file_path.name}'") from _xcp
+                msg = f"Unable to open HDF5-File '{self.file_path.name}'"
+                raise TypeError(msg) from _xcp
 
             if self.is_valid():
                 self._logger.debug("File is available now")
             else:
                 self._logger.error(
                     "[FileValidation] File is faulty! "
                     "Will try to open but there might be dragons, for '%s'",
@@ -155,15 +161,15 @@
 
     def __repr__(self) -> str:
         return yaml.safe_dump(
             self.get_metadata(minimal=True), default_flow_style=False, sort_keys=False
         )
 
     def _refresh_file_stats(self) -> None:
-        """Update internal states, helpful after resampling or other changes in data-group"""
+        """Update internal states, helpful after resampling or other changes in data-group."""
         self.h5file.flush()
         if (self.ds_time.shape[0] > 1) and (self.ds_time[1] != self.ds_time[0]):
             # this assumes isochronal sampling
             self.sample_interval_s = self._cal.time.raw_to_si(self.ds_time[1] - self.ds_time[0])
             self.sample_interval_ns = int(10**9 * self.sample_interval_s)
             self.samplerate_sps = max(int(10**9 // self.sample_interval_ns), 1)
         self.runtime_s = round(self.ds_voltage.shape[0] / self.samplerate_sps, 1)
@@ -177,18 +183,19 @@
         self,
         start_n: int = 0,
         end_n: Optional[int] = None,
         *,
         is_raw: bool = False,
         omit_ts: bool = False,
     ) -> Generator[tuple, None, None]:
-        """Generator that reads the specified range of buffers from the hdf5 file.
-        can be configured on first call
+        """Read the specified range of buffers from the hdf5 file.
+
+        Generator - can be configured on first call
         TODO: reconstruct - start/end mark samples &
-         each call can request a certain number of samples
+         each call can request a certain number of samples.
 
         Args:
         ----
             :param start_n: (int) Index of first buffer to be read
             :param end_n: (int) Index of last buffer to be read
             :param is_raw: (bool) output original data, not transformed to SI-Units
             :param omit_ts: (bool) optimize reading if timestamp is never used
@@ -214,15 +221,15 @@
                 yield (
                     self._cal.time.raw_to_si(self.ds_time[idx_start:idx_end]) if _wts else None,
                     self._cal.voltage.raw_to_si(self.ds_voltage[idx_start:idx_end]),
                     self._cal.current.raw_to_si(self.ds_current[idx_start:idx_end]),
                 )
 
     def get_calibration_data(self) -> CalibrationSeries:
-        """Reads calibration-data from hdf5 file.
+        """Read calibration-data from hdf5 file.
 
         :return: Calibration data as CalibrationSeries object
         """
         return self._cal
 
     def get_window_samples(self) -> int:
         if "window_samples" in self.h5file["data"].attrs:
@@ -244,29 +251,31 @@
             return self.h5file.attrs["hostname"]
         return "unknown"
 
     def get_datatype(self) -> Optional[EnergyDType]:
         try:
             if "datatype" in self.h5file["data"].attrs:
                 return EnergyDType[self.h5file["data"].attrs["datatype"]]
-            return None
         except KeyError:
             return None
+        else:
+            return None
 
     def get_hrv_config(self) -> dict:
-        """Essential info for harvester
+        """Essential info for harvester.
+
         :return: config-dict directly for vHarvester to be used during emulation
         """
         return {
             "datatype": self.get_datatype(),
             "window_samples": self.get_window_samples(),
         }
 
     def is_valid(self) -> bool:
-        """Checks file for plausibility
+        """Check file for plausibility, validity / correctness.
 
         :return: state of validity
         """
         # hard criteria
         if "data" not in self.h5file:
             self._logger.error(
                 "[FileValidation] root data-group not found in '%s'",
@@ -386,29 +395,30 @@
                 "[FileValidation] Sheep reported %d errors during execution -> check logs in '%s'",
                 _err,
                 self.file_path.name,
             )
         return True
 
     def __getitem__(self, key: str) -> Any:
-        """Returns attribute or (if none found) a handle for a group or dataset (if found)
+        """Query attribute or (if none found) a handle for a group or dataset (if found).
 
         :param key: attribute, group, dataset
         :return: value of that key, or handle of object
         """
         if key in self.h5file.attrs:
             return self.h5file.attrs.__getitem__(key)
         if key in self.h5file:
             return self.h5file.__getitem__(key)
         raise KeyError
 
     def energy(self) -> float:
-        """Determine the recorded energy of the trace
+        """Determine the recorded energy of the trace.
+
         # multiprocessing: https://stackoverflow.com/a/71898911
-        # -> failed with multiprocessing.pool and pathos.multiprocessing.ProcessPool
+        # -> failed with multiprocessing.pool and pathos.multiprocessing.ProcessPool.
 
         :return: sampled energy in Ws (watt-seconds)
         """
         iterations = math.ceil(self.ds_voltage.shape[0] / self.max_elements)
         job_iter = trange(
             0,
             self.ds_voltage.shape[0],
@@ -426,15 +436,16 @@
 
         energy_ws = [_calc_energy(i) for i in job_iter]
         return float(sum(energy_ws))
 
     def _dset_statistics(
         self, dset: h5py.Dataset, cal: Optional[CalibrationPair] = None
     ) -> Dict[str, float]:
-        """Some basic stats for a provided dataset
+        """Create basic stats for a provided dataset.
+
         :param dset: dataset to evaluate
         :param cal: calibration (if wanted)
         :return: dict with entries for mean, min, max, std
         """
         si_converted = True
         if not isinstance(cal, CalibrationPair):
             if "gain" in dset.attrs and "offset" in dset.attrs:
@@ -468,16 +479,17 @@
             "max": float(stats_nd[:, 2].max()),
             "std": float(stats_nd[:, 3].mean()),  # TODO: sooo wrong :)
             "si_converted": si_converted,
         }
         return stats
 
     def _data_timediffs(self) -> List[float]:
-        """Calculate list of (unique) time-deltas between buffers [s]
-            -> optimized version that only looks at the start of each buffer
+        """Calculate list of unique time-deltas [s] between buffers.
+
+        Optimized version that only looks at the start of each buffer.
 
         :return: list of (unique) time-deltas between buffers [s]
         """
         iterations = math.ceil(self.ds_time.shape[0] / self.max_elements)
         job_iter = trange(
             0,
             self.h5file["data"]["time"].shape[0],
@@ -499,16 +511,17 @@
             round(self._cal.time.raw_to_si(j) / self.samples_per_buffer, 6)
             for i in diffs_ll
             for j in i
         }
         return list(diffs)
 
     def check_timediffs(self) -> bool:
-        """Validate equal time-deltas
-        -> unexpected time-jumps hint at a corrupted file or faulty measurement
+        """Validate equal time-deltas.
+
+        Unexpected time-jumps hint at a corrupted file or faulty measurement.
 
         :return: True if OK
         """
         diffs = self._data_timediffs()
         if len(diffs) > 1:
             self._logger.warning(
                 "Time-jumps detected -> expected equal steps, but got: %s s", diffs
@@ -528,15 +541,16 @@
 
     def get_metadata(
         self,
         node: Union[h5py.Dataset, h5py.Group, None] = None,
         *,
         minimal: bool = False,
     ) -> Dict[str, dict]:
-        """Recursive FN to capture the structure of the file
+        """Recursive FN to capture the structure of the file.
+
         :param node: starting node, leave free to go through whole file
         :param minimal: just provide a bare tree (much faster)
         :return: structure of that node with everything inside it
         """
         if node is None:
             self._refresh_file_stats()
             return self.get_metadata(self.h5file, minimal=minimal)
@@ -579,15 +593,15 @@
                 }
             for item in node:
                 metadata[item] = self.get_metadata(node[item], minimal=minimal)
 
         return metadata
 
     def save_metadata(self, node: Union[h5py.Dataset, h5py.Group, None] = None) -> dict:
-        """Get structure of file and dump content to yaml-file with same name as original
+        """Get structure of file and dump content to yaml-file with same name as original.
 
         :param node: starting node, leave free to go through whole file
         :return: structure of that node with everything inside it
         """
         if isinstance(self.file_path, Path):
             yaml_path = Path(self.file_path).resolve().with_suffix(".yaml")
             if yaml_path.exists():
@@ -608,16 +622,17 @@
         for desc_name, desc in descriptions.items():
             if name in desc["name"]:
                 return int(desc_name)
         return None
 
     @staticmethod
     def get_filter_for_redundant_states(data: np.ndarray) -> np.ndarray:
-        """Input is 1D state-vector, kep only first from identical & sequential states
-        algo: create an offset-by-one vector and compare against original
+        """Input is 1D state-vector, kep only first from identical & sequential states.
+
+        Algo: create an offset-by-one vector and compare against original.
         """
         if len(data.shape) > 1:
             ValueError("Array must be 1D")
         data_1 = np.concatenate(([not data[0]], data[:-1]))
         return data != data_1
 
     def gpio_to_waveforms(self, name: Optional[str] = None) -> dict:
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/testbed_client/client.py` & `shepherd_core-2024.4.2/shepherd_core/testbed_client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Client-Class to access a testbed instance."""
+
 from importlib import import_module
 from pathlib import Path
 from typing import Optional
 from typing import TypedDict
 from typing import Union
 
 from pydantic import validate_call
@@ -12,14 +14,16 @@
 from ..data_models.base.shepherd import ShpModel
 from ..data_models.base.wrapper import Wrapper
 from .fixtures import Fixtures
 from .user_model import User
 
 
 class TestbedClient:
+    """Client-Class to access a testbed instance."""
+
     _instance: Optional[Self] = None
 
     def __init__(self, server: Optional[str] = None, token: Union[str, Path, None] = None) -> None:
         if not hasattr(self, "_token"):
             self._token: str = "null"
             self._server: Optional[str] = testbed_server_default
             self._user: Optional[User] = None
@@ -37,16 +41,18 @@
         return cls._instance
 
     def __del__(self) -> None:
         TestbedClient._instance = None
 
     @validate_call
     def connect(self, server: Optional[str] = None, token: Union[str, Path, None] = None) -> bool:
-        """server: either "local" to use demo-fixtures or something like "https://HOST:PORT"
-        token: your account validation
+        """Establish connection to testbed-server.
+
+        server: either "local" to use demo-fixtures or something like "https://HOST:PORT"
+        token: your account validation.
         """
         if isinstance(token, Path):
             with token.resolve().open() as file:
                 self._token = file.read()
         elif isinstance(token, str):
             self._token = token
 
@@ -73,27 +79,27 @@
             r.raise_for_status()
         else:
             self._fixtures.insert_model(wrap)
         return True
 
     def query_ids(self, model_type: str) -> list:
         if self._connected:
-            raise RuntimeError("Not Implemented, TODO")
+            raise NotImplementedError("TODO")
         return list(self._fixtures[model_type].elements_by_id.keys())
 
     def query_names(self, model_type: str) -> list:
         if self._connected:
-            raise RuntimeError("Not Implemented, TODO")
+            raise NotImplementedError("TODO")
         return list(self._fixtures[model_type].elements_by_name.keys())
 
     def query_item(
         self, model_type: str, uid: Optional[int] = None, name: Optional[str] = None
     ) -> dict:
         if self._connected:
-            raise RuntimeError("Not Implemented, TODO")
+            raise NotImplementedError("TODO")
         if uid is not None:
             return self._fixtures[model_type].query_id(uid)
         if name is not None:
             return self._fixtures[model_type].query_name(name)
         raise ValueError("Query needs either uid or name of object")
 
     def _query_session_key(self) -> bool:
@@ -111,31 +117,32 @@
             r.raise_for_status()
             self._user = User(**r.json())
             return True
         return False
 
     def try_inheritance(self, model_type: str, values: dict) -> (dict, list):
         if self._connected:
-            raise RuntimeError("Not Implemented, TODO")
+            raise NotImplementedError("TODO")
         return self._fixtures[model_type].inheritance(values)
 
     def try_completing_model(self, model_type: str, values: dict) -> (dict, list):
-        """Init by name/id, for none existing instances raise Exception"""
+        """Init by name/id, for none existing instances raise Exception."""
         if len(values) == 1 and next(iter(values.keys())) in {"id", "name"}:
             value = next(iter(values.values()))
             if (
                 isinstance(value, str)
                 and value.lower() in self._fixtures[model_type].elements_by_name
             ):
                 values = self.query_item(model_type, name=value)
             elif isinstance(value, int) and value in self._fixtures[model_type].elements_by_id:
                 # TODO: still depending on _fixture
                 values = self.query_item(model_type, uid=value)
             else:
-                raise ValueError(f"Query {model_type} by name / ID failed - {values} is unknown!")
+                msg = f"Query {model_type} by name / ID failed - {values} is unknown!"
+                raise ValueError(msg)
         return self.try_inheritance(model_type, values)
 
     def fill_in_user_data(self, values: dict) -> dict:
         if self._user:
             # TODO: this looks wrong, should have "is None", why not always overwrite?
             if values.get("owner"):
                 values["owner"] = self._user.name
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/testbed_client/fixtures.py` & `shepherd_core-2024.4.2/shepherd_core/testbed_client/fixtures.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Current implementation of a file-based database."""
+
 import copy
 import os
 import pickle
 from datetime import datetime
 from datetime import timedelta
 from pathlib import Path
 from typing import Any
@@ -25,15 +27,15 @@
 # - inherit_from  <-- current choice
 # - inheritor
 # - hereditary
 # - based_on
 
 
 class Fixture:
-    """Current implementation of a file-based database"""
+    """Current implementation of a file-based database."""
 
     def __init__(self, model_type: str) -> None:
         self.model_type: str = model_type.lower()
         self.elements_by_name: Dict[str, dict] = {}
         self.elements_by_id: Dict[int, dict] = {}
         # Iterator reset
         self._iter_index: int = 0
@@ -59,15 +61,16 @@
         if isinstance(key, str):
             key = key.lower()
             if key in self.elements_by_name:
                 return self.elements_by_name[key]
             key = int(key) if key.isdigit() else None
         if key in self.elements_by_id:
             return self.elements_by_id[int(key)]
-        raise ValueError(f"{self.model_type} '{key}' not found!")
+        msg = f"{self.model_type} '{key}' not found!"
+        raise ValueError(msg)
 
     def __iter__(self) -> Self:
         self._iter_index = 0
         self._iter_list = list(self.elements_by_name.values())
         return self
 
     def __next__(self) -> Any:
@@ -91,20 +94,22 @@
         fixture_base: dict = {}
         if "inherit_from" in values:
             fixture_name = values.pop("inherit_from")
             # ⤷ will also remove entry from dict
             if "name" in values and len(chain) < 1:
                 base_name = values.get("name")
                 if base_name in chain:
+                    msg = f"Inheritance-Circle detected ({base_name} already in {chain})"
                     raise ValueError(
-                        f"Inheritance-Circle detected ({base_name} already in {chain})",
+                        msg,
                     )
                 if base_name == fixture_name:
+                    msg = f"Inheritance-Circle detected ({base_name} == {fixture_name})"
                     raise ValueError(
-                        f"Inheritance-Circle detected ({base_name} == {fixture_name})",
+                        msg,
                     )
                 chain.append(base_name)
             fixture_base = copy.copy(self[fixture_name])
             logger.debug("'%s' will inherit from '%s'", self.model_type, fixture_name)
             fixture_base["name"] = fixture_name
             chain.append(fixture_name)
             base_dict, chain = self.inheritance(values=fixture_base, chain=chain)
@@ -145,31 +150,36 @@
             # keep previous entries
             base[key] = value
         return base
 
     def query_id(self, _id: int) -> dict:
         if isinstance(_id, int) and _id in self.elements_by_id:
             return self.elements_by_id[_id]
-        raise ValueError(f"Initialization of {self.model_type} by ID failed - {_id} is unknown!")
+        msg = f"Initialization of {self.model_type} by ID failed - {_id} is unknown!"
+        raise ValueError(msg)
 
     def query_name(self, name: str) -> dict:
         if isinstance(name, str) and name.lower() in self.elements_by_name:
             return self.elements_by_name[name.lower()]
-        raise ValueError(f"Initialization of {self.model_type} by name failed - {name} is unknown!")
+        msg = f"Initialization of {self.model_type} by name failed - {name} is unknown!"
+        raise ValueError(msg)
 
 
 def file_older_than(file: Path, delta: timedelta) -> bool:
+    """Decide if file is older than a specific duration of time."""
     cutoff = local_now() - delta
     mtime = datetime.fromtimestamp(file.stat().st_mtime, tz=local_tz())
     if mtime < cutoff:
         return True
     return False
 
 
 class Fixtures:
+    """A collection of individual fixture-elements."""
+
     suffix = ".yaml"
 
     @validate_call
     def __init__(self, file_path: Optional[Path] = None, *, reset: bool = False) -> None:
         if file_path is None:
             self.file_path = Path(__file__).parent.parent.resolve() / "data_models"
         else:
@@ -190,17 +200,20 @@
                 files = get_files(self.file_path, self.suffix)
             else:
                 raise ValueError("Path must either be file or directory (or empty)")
 
             for file in files:
                 self.insert_file(file)
 
-            save_path.parent.mkdir(parents=True, exist_ok=True)
-            with save_path.open("wb", buffering=-1) as fd:
-                pickle.dump(self.components, fd)
+            if len(self.components) < 1:
+                logger.error(f"No fixture-components found at {self.file_path.as_posix()}")
+            else:
+                save_path.parent.mkdir(parents=True, exist_ok=True)
+                with save_path.open("wb", buffering=-1) as fd:
+                    pickle.dump(self.components, fd)
 
     @validate_call
     def insert_file(self, file: Path) -> None:
         with file.open() as fd:
             fixtures = yaml.safe_load(fd)
             for fixture in fixtures:
                 if not isinstance(fixture, dict):
@@ -214,25 +227,28 @@
             self.components[fix_type] = Fixture(model_type=fix_type)
         self.components[fix_type].insert(data)
 
     def __getitem__(self, key: str) -> Fixture:
         key = key.lower()
         if key in self.components:
             return self.components[key]
-        raise ValueError(f"Component '{key}' not found!")
+        msg = f"Component '{key}' not found!"
+        raise ValueError(msg)
 
     def keys(self):  # noqa: ANN201
         return self.components.keys()
 
     @staticmethod
     def to_file(file: Path) -> None:
-        raise RuntimeError(f"Not Implemented, TODO (val={file})")
+        msg = f"TODO (val={file})"
+        raise NotImplementedError(msg)
 
 
 def get_files(start_path: Path, suffix: str, recursion_depth: int = 0) -> List[Path]:
+    """Generate a recursive list of all files in a directory."""
     if recursion_depth == 0:
         suffix = suffix.lower().split(".")[-1]
     dir_items = os.scandir(start_path)
     recursion_depth += 1
     files = []
 
     for item in dir_items:
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/testbed_client/user_model.py` & `shepherd_core-2024.4.2/shepherd_core/testbed_client/user_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Model for user-management."""
+
 import secrets
 from hashlib import pbkdf2_hmac
 from typing import Optional
 from typing import Union
 from uuid import uuid4
 
 from pydantic import UUID4
@@ -17,29 +19,32 @@
 from ..data_models.base.content import NameStr
 from ..data_models.base.content import SafeStr
 from ..data_models.base.shepherd import ShpModel
 
 
 @validate_call
 def hash_password(pw: Annotated[str, StringConstraints(min_length=20, max_length=100)]) -> bytes:
-    # TODO: add salt of testbed -> this fn should be part of Testbed-Object
+    """Generate a hash of a string.
+
     # NOTE: 1M Iterations need 25s on beaglebone
+    # TODO: add salt of testbed -> this fn should be part of Testbed-Object
+    """
     return pbkdf2_hmac(
         "sha512",
         password=pw.encode("utf-8"),
         salt=b"testbed_salt_TODO",
         iterations=1_000_000,
         dklen=128,
     )
 
 
 class User(ShpModel):
-    """meta-data representation of a testbed-component (physical object)"""
+    """meta-data representation of a testbed-component (physical object)."""
 
-    # id: UUID4 = Field(  # TODO db-migration - temp fix for documentation
+    # id: UUID4 = Field(  # TODO: db-migration - temp fix for documentation
     id: Union[UUID4, int] = Field(
         description="Unique ID",
         default_factory=uuid4,
     )
     name: NameStr
     description: Optional[SafeStr] = None
     comment: Optional[SafeStr] = None
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/vsource/virtual_converter_model.py` & `shepherd_core-2024.4.2/shepherd_core/vsource/virtual_converter_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,49 +1,56 @@
-"""this is ported py-version of the pru-code, goals:
+"""This is ported py-version of the pru-code.
+
+Goals:
+
 - stay close to original code-base
 - offer a comparison for the tests
 - step 1 to a virtualization of emulation
 
 NOTE: DO NOT OPTIMIZE -> stay close to original code-base
 
 Compromises:
+
 - bitshifted values (i.e. _n28) are converted to float without shift
 
 """
 
 import math
 from typing import Optional
 
 from ..data_models import CalibrationEmulator
 from ..data_models.content.virtual_source import LUT_SIZE
 from ..data_models.content.virtual_source import ConverterPRUConfig
 
 
 class PruCalibration:
-    """part of calibration.h"""
+    """part of calibration.h."""
 
     def __init__(self, cal_emu: Optional[CalibrationEmulator] = None) -> None:
         self.cal = cal_emu if cal_emu else CalibrationEmulator()
 
     def conv_adc_raw_to_nA(self, current_raw: int) -> float:
         return self.cal.adc_C_A.raw_to_si(current_raw) * (10**9)
         # TODO: add feature "negative residue compensation" to here
 
     @staticmethod
     def conv_adc_raw_to_uV(voltage_raw: int) -> float:
-        raise RuntimeError(f"This Fn should not been used (val={voltage_raw})")
+        msg = f"This Fn should not been used (val={voltage_raw})"
+        raise RuntimeError(msg)
 
     def conv_uV_to_dac_raw(self, voltage_uV: float) -> int:
         dac_raw = self.cal.dac_V_A.si_to_raw(float(voltage_uV) / (10**6))
         if dac_raw > (2**16) - 1:
             dac_raw = (2**16) - 1
         return dac_raw
 
 
 class VirtualConverterModel:
+    """Ported python version of the pru vCnv."""
+
     def __init__(self, cfg: ConverterPRUConfig, cal: PruCalibration) -> None:
         self._cal: PruCalibration = cal
         self._cfg: ConverterPRUConfig = cfg
 
         # simplifications for python
         self.R_input_kOhm = float(self._cfg.R_input_kOhm_n22) / 2**22
         self.Constant_us_per_nF = float(self._cfg.Constant_us_per_nF_n28) / 2**28
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/vsource/virtual_harvester_model.py` & `shepherd_core-2024.4.2/shepherd_core/vsource/virtual_harvester_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,33 @@
-"""this is ported py-version of the pru-code, goals:
+"""this is ported py-version of the pru-code.
+
+Goals:
+
 - stay close to original code-base
 - offer a comparison for the tests
 - step 1 to a virtualization of emulation
 
 NOTE1: DO NOT OPTIMIZE -> stay close to original c-code-base
 NOTE2: adc-harvest-routines are not part of this model (virtual_harvester lines 66:289)
 
 Compromises:
+
 - Py has to map the settings-list to internal vars -> is kernel-task
 - Python has no static vars -> FName_reset is handling the class-vars
 
 """
 
 from typing import Tuple
 
 from ..data_models.content.virtual_harvester import HarvesterPRUConfig
 
 
 class VirtualHarvesterModel:
+    """Ported python version of the pru vHrv."""
+
     HRV_IVCURVE: int = 2**4
     HRV_CV: int = 2**8
     HRV_MPPT_VOC: int = 2**12
     HRV_MPPT_PO: int = 2**13
     HRV_MPPT_OPT: int = 2**14
 
     def __init__(self, cfg: HarvesterPRUConfig) -> None:
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/vsource/virtual_source_model.py` & `shepherd_core-2024.4.2/shepherd_core/vsource/virtual_source_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-"""this is ported py-version of the pru-code, goals:
+"""This is ported py-version of the pru-code.
+
+Goals:
+
 - stay close to original code-base
 - offer a comparison for the tests
-- step 1 to a virtualization of emulation
+- step 1 to a virtualization of emulation.
 
 NOTE: DO NOT OPTIMIZE -> stay close to original code-base
 
 """
 
 from typing import Optional
 
@@ -16,15 +19,15 @@
 from ..data_models.content.virtual_source import ConverterPRUConfig
 from .virtual_converter_model import PruCalibration
 from .virtual_converter_model import VirtualConverterModel
 from .virtual_harvester_model import VirtualHarvesterModel
 
 
 class VirtualSourceModel:
-    """part of sampling.c"""
+    """part of sampling.c."""
 
     def __init__(
         self,
         vsrc: Optional[VirtualSourceConfig],
         cal_emu: CalibrationEmulator,
         dtype_in: EnergyDType = EnergyDType.ivsample,
         window_size: Optional[int] = None,
@@ -49,16 +52,17 @@
 
         self.hrv: VirtualHarvesterModel = VirtualHarvesterModel(hrv_config)
 
         self.W_inp_fWs: float = 0.0
         self.W_out_fWs: float = 0.0
 
     def iterate_sampling(self, V_inp_uV: int = 0, I_inp_nA: int = 0, I_out_nA: int = 0) -> int:
-        """TEST-SIMPLIFICATION - code below is not part of pru-code,
-        but in part sample_emulator() in sampling.c
+        """TEST-SIMPLIFICATION - code below is not part of pru-code.
+
+        It originates from sample_emulator() in sampling.c.
 
         :param V_inp_uV:
         :param I_inp_nA:
         :param I_out_nA:
         :return:
         """
         V_inp_uV, I_inp_nA = self.hrv.ivcurve_sample(V_inp_uV, I_inp_nA)
```

### Comparing `shepherd_core-2024.4.1/shepherd_core/writer.py` & `shepherd_core-2024.4.2/shepherd_core/writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Writer that inherits from Reader-Baseclass"""
+"""Writer that inherits from Reader-Baseclass."""
 
 import logging
 import math
 import pathlib
 from datetime import timedelta
 from itertools import product
 from pathlib import Path
@@ -31,44 +31,46 @@
 from .reader import Reader
 
 
 # copy of core/models/base/shepherd - needed also here
 def path2str(
     dumper: Dumper, data: Union[pathlib.Path, pathlib.WindowsPath, pathlib.PosixPath]
 ) -> ScalarNode:
+    """Add a yaml-representation for a specific datatype."""
     return dumper.represent_scalar("tag:yaml.org,2002:str", str(data.as_posix()))
 
 
 def time2int(dumper: Dumper, data: timedelta) -> ScalarNode:
+    """Add a yaml-representation for a specific datatype."""
     return dumper.represent_scalar("tag:yaml.org,2002:int", str(int(data.total_seconds())))
 
 
 yaml.add_representer(pathlib.PosixPath, path2str, SafeDumper)
 yaml.add_representer(pathlib.WindowsPath, path2str, SafeDumper)
 yaml.add_representer(pathlib.Path, path2str, SafeDumper)
 yaml.add_representer(timedelta, time2int, SafeDumper)
 
 
 def unique_path(base_path: Union[str, Path], suffix: str) -> Path:
-    """Finds an unused filename in case it already exists
+    """Find an unused filename in case it already exists.
 
     :param base_path: file-path to test
     :param suffix: file-suffix
     :return: new non-existing path
     """
     counter = 0
     while True:
         path = Path(base_path).with_suffix(f".{counter}{suffix}")
         if not path.exists():
             return path
         counter += 1
 
 
 class Writer(Reader):
-    """Stores data for Shepherd in HDF5 format
+    """Stores data for Shepherd in HDF5 format.
 
     Choose lossless compression filter
      - lzf:  low to moderate compression, VERY fast, no options
              -> 20 % cpu overhead for half the filesize
      - gzip: good compression, moderate speed, select level from 1-9, default is 4
              -> lower levels seem fine
              -> _algo=number instead of "gzip" is read as compression level for gzip
@@ -120,34 +122,35 @@
             self._logger: logging.Logger = logging.getLogger("SHPCore.Writer")
         # -> logger gets configured in reader()
 
         if self._modify or force_overwrite or not file_path.exists():
             self.file_path: Path = file_path.resolve()
             self._logger.info("Storing data to   '%s'", self.file_path)
         elif file_path.exists() and not file_path.is_file():
-            raise TypeError(f"Path is not a file ({file_path})")
+            msg = f"Path is not a file ({file_path})"
+            raise TypeError(msg)
         else:
             base_dir = file_path.resolve().parents[0]
             self.file_path = unique_path(base_dir / file_path.stem, file_path.suffix)
             self._logger.warning(
                 "File '%s' already exists -> storing under '%s' instead",
                 file_path,
                 self.file_path.name,
             )
 
         if isinstance(mode, str) and mode not in self.mode_dtype_dict:
-            raise ValueError(f"Can't handle mode '{mode}' (choose one of {self.mode_dtype_dict})")
+            msg = f"Can't handle mode '{mode}' (choose one of {self.mode_dtype_dict})"
+            raise ValueError(msg)
 
-        _dtypes = self.mode_dtype_dict[mode if mode else self.mode_default]
+        _dtypes = self.mode_dtype_dict[mode or self.mode_default]
         if isinstance(datatype, str):
             datatype = EnergyDType[datatype]
         if isinstance(datatype, EnergyDType) and datatype not in _dtypes:
-            raise ValueError(
-                f"Can't handle value '{datatype}' of datatype (choose one of {_dtypes})"
-            )
+            msg = f"Can't handle value '{datatype}' of datatype (choose one of {_dtypes})"
+            raise ValueError(msg)
 
         if self._modify:
             self._mode = mode
             self._datatype = datatype
             self._window_samples = window_samples
         else:
             self._mode = mode if isinstance(mode, str) else self.mode_default
@@ -219,15 +222,15 @@
             self.file_size / 2**20,
             self.data_rate / 2**10,
         )
         self.is_valid()
         self.h5file.close()
 
     def _create_skeleton(self) -> None:
-        """Initializes the structure of the HDF5 file
+        """Initialize the structure of the HDF5 file.
 
         HDF5 is hierarchically structured and before writing data, we have to
         setup this structure, i.e. creating the right groups with corresponding
         data types. We will store 3 types of data in a database: The
         actual IV samples recorded either from the harvester (during recording)
         or the target (during emulation). Any log messages, that can be used to
         store relevant events or tag some parts of the recorded data.
@@ -275,15 +278,15 @@
 
     def append_iv_data_raw(
         self,
         timestamp: Union[np.ndarray, float, int],  # noqa: PYI041
         voltage: np.ndarray,
         current: np.ndarray,
     ) -> None:
-        """Writes raw data to database
+        """Write raw data to database.
 
         Args:
         ----
             timestamp: just start of buffer or whole ndarray
             voltage: ndarray as raw unsigned integers
             current: ndarray as raw unsigned integers
 
@@ -294,15 +297,15 @@
             timestamp = int(timestamp)
         if isinstance(timestamp, int):
             time_series_ns = self.sample_interval_ns * np.arange(len_new).astype("u8")
             timestamp = timestamp + time_series_ns
         if isinstance(timestamp, np.ndarray):
             len_new = min(len_new, timestamp.size)
         else:
-            raise ValueError("timestamp-data was not usable")
+            raise TypeError("timestamp-data was not usable")
 
         len_old = self.ds_voltage.shape[0]
 
         # resize dataset
         self.ds_time.resize((len_old + len_new,))
         self.ds_voltage.resize((len_old + len_new,))
         self.ds_current.resize((len_old + len_new,))
@@ -314,15 +317,17 @@
 
     def append_iv_data_si(
         self,
         timestamp: Union[np.ndarray, float],
         voltage: np.ndarray,
         current: np.ndarray,
     ) -> None:
-        """Writes data (in SI / physical unit) to file, but converts it to raw-data first
+        """Write data (provided in SI / physical unit) to file.
+
+        This will convert it to raw-data first.
 
            SI-value [SI-Unit] = raw-value * gain + offset,
 
         Args:
         ----
             timestamp: python timestamp (time.time()) in seconds (si-unit)
                        -> provide start of buffer or whole ndarray
@@ -332,15 +337,15 @@
         """
         timestamp = self._cal.time.si_to_raw(timestamp)
         voltage = self._cal.voltage.si_to_raw(voltage)
         current = self._cal.current.si_to_raw(current)
         self.append_iv_data_raw(timestamp, voltage, current)
 
     def _align(self) -> None:
-        """Align datasets with buffer-size of shepherd"""
+        """Align datasets with buffer-size of shepherd."""
         self._refresh_file_stats()
         n_buff = self.ds_voltage.size / self.samples_per_buffer
         size_new = int(math.floor(n_buff) * self.samples_per_buffer)
         if size_new < self.ds_voltage.size:
             if self.samplerate_sps != samplerate_sps_default:
                 self._logger.debug("skipped alignment due to altered samplerate")
                 return
@@ -349,26 +354,26 @@
                 self.ds_voltage.size - size_new,
             )
             self.ds_time.resize((size_new,))
             self.ds_voltage.resize((size_new,))
             self.ds_current.resize((size_new,))
 
     def __setitem__(self, key: str, item: Any) -> None:
-        """A convenient interface to store relevant key-value data (attribute) if H5-structure"""
+        """Conveniently store relevant key-value data (attribute) in H5-structure."""
         self.h5file.attrs.__setitem__(key, item)
 
     def store_config(self, data: dict) -> None:
-        """Important Step to get a self-describing Output-File
+        """Get a better self-describing Output-File.
+
         TODO: use data-model?
-        :param data: from virtual harvester or converter / source
+        :param data: from virtual harvester or converter / source.
         """
         self.h5file["data"].attrs["config"] = yaml.safe_dump(
             data, default_flow_style=False, sort_keys=False
         )
 
     def store_hostname(self, name: str) -> None:
-        """Option to distinguish the host, target or data-source in the testbed
-            -> perfect for plotting later
+        """Option to distinguish the host, target or data-source -> perfect for plotting later.
 
         :param name: something unique, or "artificial" in case of generated content
         """
         self.h5file.attrs["hostname"] = name
```

### Comparing `shepherd_core-2024.4.1/shepherd_core.egg-info/PKG-INFO` & `shepherd_core-2024.4.2/shepherd_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd_core
-Version: 2024.4.1
+Version: 2024.4.2
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Author-email: Ingmar Splitt <ingmar.splitt@tu-dresden.de>
 Maintainer-email: Ingmar Splitt <ingmar.splitt@tu-dresden.de>
 Project-URL: Documentation, https://github.com/orgua/shepherd-datalib/blob/main/README.md
 Project-URL: Issues, https://github.com/orgua/shepherd-datalib/issues
 Project-URL: Source, https://pypi.org/project/shepherd-core/
 Keywords: testbed,beaglebone,pru,batteryless,energyharvesting,solar
@@ -35,14 +35,15 @@
 Requires-Dist: pydantic[email]>2.0.0
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Requires-Dist: intelhex
 Requires-Dist: requests
 Requires-Dist: pyelftools
 Requires-Dist: zstandard
+Requires-Dist: typing-extensions
 Provides-Extra: elf
 Requires-Dist: pwntools-elf-only; extra == "elf"
 Provides-Extra: inventory
 Requires-Dist: psutil; extra == "inventory"
 Provides-Extra: dev
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
```

### Comparing `shepherd_core-2024.4.1/tests/test_cal_hw.py` & `shepherd_core-2024.4.2/tests/test_cal_hw.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.1/tests/test_examples.py` & `shepherd_core-2024.4.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.1/tests/test_reader.py` & `shepherd_core-2024.4.2/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2024.4.1/tests/test_writer.py` & `shepherd_core-2024.4.2/tests/test_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,20 +72,20 @@
 
 def test_writer_unique_path(h5_file: Path) -> None:
     with Writer(h5_file) as sfw:
         assert sfw.file_path != h5_path
 
 
 def test_writer_faulty_mode(h5_path: Path) -> None:
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError):  # noqa: PT011
         generate_shp_file(h5_path, mode="excavator", datatype="ivcurve")
 
 
 def test_writer_faulty_datatype(h5_path: Path) -> None:
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError):  # noqa: PT011
         generate_shp_file(h5_path, mode="emulator", datatype="ivcurve")
 
 
 def test_writer_faulty_path(tmp_path: Path) -> None:
     with pytest.raises(TypeError):
         generate_shp_file(tmp_path)
 
@@ -105,17 +105,17 @@
 
 def test_writer_init_cal_series(h5_path: Path) -> None:
     cs = CalSeries.from_cal(CalHrv())
     generate_shp_file(h5_path, cal_data=cs)
 
 
 def test_writer_faulty_window(h5_path: Path) -> None:
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError):  # noqa: PT011
         generate_shp_file(h5_path, mode="harvester", datatype="ivcurve")
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError):  # noqa: PT011
         generate_shp_file(
             h5_path,
             mode="harvester",
             datatype="ivcurve",
             window_samples=0,
         )
 
@@ -125,15 +125,15 @@
         data_nd = np.zeros((sfw.samples_per_buffer,))
         time_float = 5.5
         time_int = 3
         time_nd = 3 + data_nd
         sfw.append_iv_data_raw(time_float, data_nd, data_nd)
         sfw.append_iv_data_raw(time_int, data_nd, data_nd)
         sfw.append_iv_data_raw(time_nd, data_nd, data_nd)
-        with pytest.raises(ValueError):
+        with pytest.raises(TypeError):
             sfw.append_iv_data_raw(None, data_nd, data_nd)
 
 
 def test_writer_align(h5_path: Path) -> None:
     with Writer(h5_path) as sfw:
         length = int(5.5 * sfw.samples_per_buffer)
         time_nd = np.arange(0, length * sfw.sample_interval_ns, sfw.sample_interval_ns)
```

