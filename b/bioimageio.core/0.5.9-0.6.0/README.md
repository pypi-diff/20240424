# Comparing `tmp/bioimageio.core-0.5.9.tar.gz` & `tmp/bioimageio.core-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioimageio.core-0.5.9.tar", last modified: Tue May 16 10:11:41 2023, max compression
+gzip compressed data, was "bioimageio.core-0.6.0.tar", last modified: Tue Apr 23 23:21:59 2024, max compression
```

## Comparing `bioimageio.core-0.5.9.tar` & `bioimageio.core-0.6.0.tar`

### file list

```diff
@@ -1,90 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.069888 bioimageio.core-0.5.9/bioimageio/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.069888 bioimageio.core-0.5.9/bioimageio/core/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-16 10:11:38.000000 bioimageio.core-0.5.9/bioimageio/core/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.069888 bioimageio.core-0.5.9/bioimageio/core/build_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/build_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/build_spec/add_weights.py
--rw-r--r--   0 runner    (1001) docker     (123)    36794 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/build_spec/build_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/image_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    20458 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.069888 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_combined_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_measure_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/_keras_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/_onnx_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/_pytorch_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/_tensorflow_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/_torchscript_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_prediction_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_stat_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/bioimageio/core/resource_io/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/resource_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/resource_io/io_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/resource_io/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/resource_io/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13163 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/resource_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/statistical_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/bioimageio/core/weight_converter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/weight_converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/bioimageio/core/weight_converter/keras/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/weight_converter/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/weight_converter/keras/tensorflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/bioimageio/core/weight_converter/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/weight_converter/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/weight_converter/torch/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/weight_converter/torch/torchscript.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/weight_converter/torch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.069888 bioimageio.core-0.5.9/bioimageio.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-16 10:11:40.000000 bioimageio.core-0.5.9/bioimageio.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-16 10:11:41.000000 bioimageio.core-0.5.9/bioimageio.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 10:11:40.000000 bioimageio.core-0.5.9/bioimageio.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-16 10:11:40.000000 bioimageio.core-0.5.9/bioimageio.core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 10:11:40.000000 bioimageio.core-0.5.9/bioimageio.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-16 10:11:40.000000 bioimageio.core-0.5.9/bioimageio.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/tests/build_spec/
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/build_spec/test_add_weights.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/build_spec/test_build_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/tests/prediction_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/prediction_pipeline/test_combined_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/prediction_pipeline/test_device_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/prediction_pipeline/test_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/prediction_pipeline/test_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/prediction_pipeline/test_prediction_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/prediction_pipeline/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/prediction_pipeline/test_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/tests/resource_io/
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/resource_io/test_load_rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/resource_io/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/test_bioimageio_spec_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/test_export_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/test_image_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/test_prediction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/tests/test_resource_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/test_resource_tests/test_test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.069888 bioimageio.core-0.5.9/tests/weight_converter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/tests/weight_converter/keras/
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/weight_converter/keras/test_tensorflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/tests/weight_converter/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/weight_converter/torch/test_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/weight_converter/torch/test_torchscript.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.273630 bioimageio.core-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-23 23:21:21.000000 bioimageio.core-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-23 23:21:59.273630 bioimageio.core-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.257630 bioimageio.core-0.6.0/bioimageio/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.265630 bioimageio.core-0.6.0/bioimageio/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/_magic_tensor_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/_op_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/_prediction_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/_resource_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/block_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12475 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/digest_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.265630 bioimageio.core-0.6.0/bioimageio/core/model_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/model_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/model_adapters/_keras_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/model_adapters/_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/model_adapters/_onnx_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/model_adapters/_pytorch_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/model_adapters/_tensorflow_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/model_adapters/_torchscript_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21626 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/proc_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/proc_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20495 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/stat_calculators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/stat_measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16351 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.265630 bioimageio.core-0.6.0/bioimageio/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.269630 bioimageio.core-0.6.0/bioimageio/core/weight_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/weight_converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.269630 bioimageio.core-0.6.0/bioimageio/core/weight_converter/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/weight_converter/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/weight_converter/keras/_tensorflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.269630 bioimageio.core-0.6.0/bioimageio/core/weight_converter/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/weight_converter/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/weight_converter/torch/_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/weight_converter/torch/_torchscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/bioimageio/core/weight_converter/torch/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.261630 bioimageio.core-0.6.0/bioimageio.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-23 23:21:59.000000 bioimageio.core-0.6.0/bioimageio.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-23 23:21:59.000000 bioimageio.core-0.6.0/bioimageio.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 23:21:59.000000 bioimageio.core-0.6.0/bioimageio.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 23:21:59.000000 bioimageio.core-0.6.0/bioimageio.core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-23 23:21:59.000000 bioimageio.core-0.6.0/bioimageio.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-23 23:21:59.000000 bioimageio.core-0.6.0/bioimageio.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.269630 bioimageio.core-0.6.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/scripts/setup_dev_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/scripts/show_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 23:21:59.273630 bioimageio.core-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.269630 bioimageio.core-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_any_model_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_bioimageio_spec_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_digest_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_prediction_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_prediction_pipeline_device_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12513 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_proc_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_resource_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_stat_calculators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_stat_measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/test_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.269630 bioimageio.core-0.6.0/tests/weight_converter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.269630 bioimageio.core-0.6.0/tests/weight_converter/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/weight_converter/keras/test_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/weight_converter/test_add_weights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:59.273630 bioimageio.core-0.6.0/tests/weight_converter/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/weight_converter/torch/test_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-23 23:21:56.000000 bioimageio.core-0.6.0/tests/weight_converter/torch/test_torchscript.py
```

### Comparing `bioimageio.core-0.5.9/LICENSE` & `bioimageio.core-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.9/PKG-INFO` & `bioimageio.core-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,117 +1,147 @@
 Metadata-Version: 2.1
 Name: bioimageio.core
-Version: 0.5.9
+Version: 0.6.0
 Summary: Python functionality for the bioimage model zoo
 Home-page: https://github.com/bioimage-io/core-bioimage-io-python
 Author: Bioimage Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/core-bioimage-io-python/issues
 Project-URL: Source, https://github.com/bioimage-io/core-bioimage-io-python
 Description: # core-bioimage-io-python
         
         Python specific core utilities for running models in the [BioImage Model Zoo](https://bioimage.io).
         
         ## Installation
         
-        ### Via Conda
+        ### Via Mamba/Conda
         
         The `bioimageio.core` package can be installed from conda-forge via
+        
+        ```console
+        mamba install -c conda-forge bioimageio.core
         ```
-        conda install -c conda-forge bioimageio.core
-        ```
-        if you don't install any additional deep learning libraries, you will only be able to use general convenience functionality, but not any functionality for model prediction.
+        
+        If you do not install any additional deep learning libraries, you will only be able to use general convenience
+        functionality, but not any functionality for model prediction.
         To install additional deep learning libraries use:
         
         * Pytorch/Torchscript:
-          ```bash
-          # cpu installation (if you don't have an nvidia graphics card)
-          conda install -c pytorch -c conda-forge bioimageio.core pytorch torchvision cpuonly
         
-          # gpu installation (for cuda 11.6, please choose the appropriate cuda version for your system)
-          conda install -c pytorch -c nvidia -c conda-forge bioimageio.core pytorch torchvision pytorch-cuda=11.6 
+          CPU installation (if you don't have an nvidia graphics card):
+        
+          ```console
+          mamba install -c pytorch -c conda-forge bioimageio.core pytorch torchvision cpuonly
           ```
-          Note that the pytorch installation instructions may change in the future. For the latest instructions please refer to [pytorch.org](https://pytorch.org/).
         
+          GPU installation (for cuda 11.6, please choose the appropriate cuda version for your system):
+        
+          ```console
+          mamba install -c pytorch -c nvidia -c conda-forge bioimageio.core pytorch torchvision pytorch-cuda=11.8
+          ```
+        
+          Note that the pytorch installation instructions may change in the future. For the latest instructions please refer to [pytorch.org](https://pytorch.org/).
         
         * Tensorflow
-          ```bash
-          # currently only cpu version supported
-          conda install -c conda-forge bioimageio.core tensorflow
+        
+          Currently only CPU version supported
+        
+          ```console
+          mamba install -c conda-forge bioimageio.core tensorflow
           ```
         
         * ONNXRuntime
-          ```bash
-          # currently only cpu version supported
-          conda install -c conda-forge bioimageio.core onnxruntime
+        
+          Currently only cpu version supported
+        
+          ```console
+          mamba install -c conda-forge bioimageio.core onnxruntime
           ```
-          
+        
         ### Via pip
         
-        The package is also available via pip:
-        ```
-        pip install bioimageio.core
+        The package is also available via pip
+        (e.g. with recommended extras `onnx` and `pytorch`):
+        
+        ```console
+        pip install bioimageio.core[onnx,pytorch]
         ```
         
         ### Set up Development Environment
         
         To set up a development conda environment run the following commands:
-        ```
-        conda env create -f dev/environment-base.yaml
-        conda activate bio-core-dev
+        
+        ```console
+        mamba env create -f dev/env.yaml
+        mamba activate core
         pip install -e . --no-deps
         ```
         
         There are different environment files that only install tensorflow or pytorch as dependencies available.
         
-        ## Command Line
+        ## 💻 Command Line
         
-        `bioimageio.core` installs a command line interface for testing models and other functionality. You can list all the available commands via:
-        ```
+        `bioimageio.core` installs a command line interface (CLI) for testing models and other functionality.
+        You can list all the available commands via:
+        
+        ```console
         bioimageio
         ```
         
         Check that a model adheres to the model spec:
-        ```
+        
+        ```console
         bioimageio validate <MODEL>
         ```
         
         Test a model (including prediction for the test input):
-        ```
+        
+        ```console
         bioimageio test-model <MODEL>
         ```
         
         Run prediction for an image stored on disc:
-        ```
-        bioimageio predict-image -m <MODEL> -i <INPUT> -o <OUTPUT>
+        
+        ```console
+        bioimageio predict-image <MODEL> --inputs <INPUT> --outputs <OUTPUT>
         ```
         
         Run prediction for multiple images stored on disc:
-        ```
+        
+        ```console
         bioimagei predict-images -m <MODEL> -i <INPUT_PATTERN> - o <OUTPUT_FOLDER>
         ```
-        `<INPUT_PATTERN>` is a `glob` pattern to select the desired images, e.g. `/path/to/my/images/*.tif`.
         
+        `<INPUT_PATTERN>` is a `glob` pattern to select the desired images, e.g. `/path/to/my/images/*.tif`.
         
         ## From python
         
         `bioimageio.core` is a python library that implements loading models, running prediction with them and more.
         To get an overview of this functionality, check out the example notebooks:
-        - [example/model_usage](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/model_usage.ipynb) for how to load models and run prediction with them
-        - [example/model_creation](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/model_creation.ipynb) for how to create bioimage.io compatible model packages
-        - [example/dataset_statistics_demo](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/dataset_statistics_demo.ipynb) for how to use the dataset statistics for advanced pre-and-postprocessing
+        
+        * [example/model_usage](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/model_usage.ipynb) for how to load models and run prediction with them
+        * [example/model_creation](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/model_creation.ipynb) for how to create bioimage.io compatible model packages
+        * [example/dataset_statistics_demo](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/dataset_statistics_demo.ipynb) for how to use the dataset statistics for advanced pre-and-postprocessing
         
         ## Model Specification
         
-        The model specification and its validation tools can be found at https://github.com/bioimage-io/spec-bioimage-io.
+        The model specification and its validation tools can be found at <https://github.com/bioimage-io/spec-bioimage-io>.
+        
+        ## Changelog
+        
+        ### 0.5.10
+        
+        * [Fix critical bug in predict with tiling](https://github.com/bioimage-io/core-bioimage-io-python/pull/359)
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: dev
 Provides-Extra: pytorch
 Provides-Extra: tensorflow
 Provides-Extra: onnx
+Provides-Extra: dev
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bioimageio.core-0.5.9/README.md` & `bioimageio.core-0.6.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,96 +1,124 @@
 # core-bioimage-io-python
 
 Python specific core utilities for running models in the [BioImage Model Zoo](https://bioimage.io).
 
 ## Installation
 
-### Via Conda
+### Via Mamba/Conda
 
 The `bioimageio.core` package can be installed from conda-forge via
+
+```console
+mamba install -c conda-forge bioimageio.core
 ```
-conda install -c conda-forge bioimageio.core
-```
-if you don't install any additional deep learning libraries, you will only be able to use general convenience functionality, but not any functionality for model prediction.
+
+If you do not install any additional deep learning libraries, you will only be able to use general convenience
+functionality, but not any functionality for model prediction.
 To install additional deep learning libraries use:
 
 * Pytorch/Torchscript:
-  ```bash
-  # cpu installation (if you don't have an nvidia graphics card)
-  conda install -c pytorch -c conda-forge bioimageio.core pytorch torchvision cpuonly
 
-  # gpu installation (for cuda 11.6, please choose the appropriate cuda version for your system)
-  conda install -c pytorch -c nvidia -c conda-forge bioimageio.core pytorch torchvision pytorch-cuda=11.6 
+  CPU installation (if you don't have an nvidia graphics card):
+
+  ```console
+  mamba install -c pytorch -c conda-forge bioimageio.core pytorch torchvision cpuonly
   ```
-  Note that the pytorch installation instructions may change in the future. For the latest instructions please refer to [pytorch.org](https://pytorch.org/).
 
+  GPU installation (for cuda 11.6, please choose the appropriate cuda version for your system):
+
+  ```console
+  mamba install -c pytorch -c nvidia -c conda-forge bioimageio.core pytorch torchvision pytorch-cuda=11.8
+  ```
+
+  Note that the pytorch installation instructions may change in the future. For the latest instructions please refer to [pytorch.org](https://pytorch.org/).
 
 * Tensorflow
-  ```bash
-  # currently only cpu version supported
-  conda install -c conda-forge bioimageio.core tensorflow
+
+  Currently only CPU version supported
+
+  ```console
+  mamba install -c conda-forge bioimageio.core tensorflow
   ```
 
 * ONNXRuntime
-  ```bash
-  # currently only cpu version supported
-  conda install -c conda-forge bioimageio.core onnxruntime
+
+  Currently only cpu version supported
+
+  ```console
+  mamba install -c conda-forge bioimageio.core onnxruntime
   ```
-  
+
 ### Via pip
 
-The package is also available via pip:
-```
-pip install bioimageio.core
+The package is also available via pip
+(e.g. with recommended extras `onnx` and `pytorch`):
+
+```console
+pip install bioimageio.core[onnx,pytorch]
 ```
 
 ### Set up Development Environment
 
 To set up a development conda environment run the following commands:
-```
-conda env create -f dev/environment-base.yaml
-conda activate bio-core-dev
+
+```console
+mamba env create -f dev/env.yaml
+mamba activate core
 pip install -e . --no-deps
 ```
 
 There are different environment files that only install tensorflow or pytorch as dependencies available.
 
-## Command Line
+## 💻 Command Line
 
-`bioimageio.core` installs a command line interface for testing models and other functionality. You can list all the available commands via:
-```
+`bioimageio.core` installs a command line interface (CLI) for testing models and other functionality.
+You can list all the available commands via:
+
+```console
 bioimageio
 ```
 
 Check that a model adheres to the model spec:
-```
+
+```console
 bioimageio validate <MODEL>
 ```
 
 Test a model (including prediction for the test input):
-```
+
+```console
 bioimageio test-model <MODEL>
 ```
 
 Run prediction for an image stored on disc:
-```
-bioimageio predict-image -m <MODEL> -i <INPUT> -o <OUTPUT>
+
+```console
+bioimageio predict-image <MODEL> --inputs <INPUT> --outputs <OUTPUT>
 ```
 
 Run prediction for multiple images stored on disc:
-```
+
+```console
 bioimagei predict-images -m <MODEL> -i <INPUT_PATTERN> - o <OUTPUT_FOLDER>
 ```
-`<INPUT_PATTERN>` is a `glob` pattern to select the desired images, e.g. `/path/to/my/images/*.tif`.
 
+`<INPUT_PATTERN>` is a `glob` pattern to select the desired images, e.g. `/path/to/my/images/*.tif`.
 
 ## From python
 
 `bioimageio.core` is a python library that implements loading models, running prediction with them and more.
 To get an overview of this functionality, check out the example notebooks:
-- [example/model_usage](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/model_usage.ipynb) for how to load models and run prediction with them
-- [example/model_creation](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/model_creation.ipynb) for how to create bioimage.io compatible model packages
-- [example/dataset_statistics_demo](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/dataset_statistics_demo.ipynb) for how to use the dataset statistics for advanced pre-and-postprocessing
+
+* [example/model_usage](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/model_usage.ipynb) for how to load models and run prediction with them
+* [example/model_creation](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/model_creation.ipynb) for how to create bioimage.io compatible model packages
+* [example/dataset_statistics_demo](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/dataset_statistics_demo.ipynb) for how to use the dataset statistics for advanced pre-and-postprocessing
 
 ## Model Specification
 
-The model specification and its validation tools can be found at https://github.com/bioimage-io/spec-bioimage-io.
+The model specification and its validation tools can be found at <https://github.com/bioimage-io/spec-bioimage-io>.
+
+## Changelog
+
+### 0.5.10
+
+* [Fix critical bug in predict with tiling](https://github.com/bioimage-io/core-bioimage-io-python/pull/359)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/_model_adapter.py` & `bioimageio.core-0.6.0/bioimageio/core/model_adapters/_model_adapter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,178 +1,163 @@
-import abc
-from typing import List, Optional, Sequence, Type, Union
+import warnings
+from abc import ABC, abstractmethod
+from typing import List, Optional, Sequence, Tuple, Union, final
 
-import xarray as xr
+from bioimageio.spec.model import v0_4, v0_5
 
-from bioimageio.core import load_resource_description
-from bioimageio.core.resource_io import nodes
+from ..tensor import Tensor
 
-#: Known weight formats in order of priority
-#: First match wins
-from bioimageio.spec.model import raw_nodes
+WeightsFormat = Union[v0_4.WeightsFormat, v0_5.WeightsFormat]
 
-_WEIGHT_FORMATS = ["pytorch_state_dict", "tensorflow_saved_model_bundle", "torchscript", "onnx", "keras_hdf5"]
+# Known weight formats in order of priority
+# First match wins
+DEFAULT_WEIGHT_FORMAT_PRIORITY_ORDER: Tuple[WeightsFormat, ...] = (
+    "pytorch_state_dict",
+    "tensorflow_saved_model_bundle",
+    "torchscript",
+    "onnx",
+    "keras_hdf5",
+)
 
 
-class ModelAdapter(abc.ABC):
-    """
-    Represents model *without* any preprocessing and postprocessing
+class ModelAdapter(ABC):
     """
+    Represents model *without* any preprocessing or postprocessing.
 
-    def __init__(
-        self, *, bioimageio_model: Union[nodes.Model, raw_nodes.Model], devices: Optional[Sequence[str]] = None
-    ):
-        self.bioimageio_model = self._prepare_model(bioimageio_model)
-        self.default_devices = devices
-        self.loaded = False
-
-    @staticmethod
-    def _prepare_model(bioimageio_model):
-        """the (raw) model node is prepared (here: loaded as non-raw model node) for the model adapter to be ready
-        for operation.
-        Note: To write a model adapter that uses the raw model node one can overwrite this method.
-        """
-        if isinstance(bioimageio_model, nodes.Model):
-            return bioimageio_model
-        else:
-            return load_resource_description(bioimageio_model)
-
-    def __enter__(self):
-        """load on entering context"""
-        assert not self.loaded
-        self.load()  # using default_devices
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        """unload on exiting context"""
-        assert self.loaded
-        self.unload()
-        return False
+    ```
+    from bioimageio.core import load_description
 
-    def load(self, *, devices: Optional[Sequence[str]] = None) -> None:
-        """
-        Note: Use ModelAdapter as context to not worry about calling unload()!
-        Load model onto devices. If devices is None, self.default_devices are chosen
-        (which may be None as well, in which case a framework dependent default is chosen)
-        """
-        self._load(devices=devices or self.default_devices)
-        self.loaded = True
+    model = load_description(...)
 
-    @abc.abstractmethod
-    def _load(self, *, devices: Optional[Sequence[str]] = None) -> None:
-        """
-        Load model onto devices. If devices is None a framework dependent default is chosen
-        """
-        ...
+    # option 1:
+    adapter = ModelAdapter.create(model)
+    adapter.forward(...)
+    adapter.unload()
 
-    def forward(self, *input_tensors: xr.DataArray) -> List[xr.DataArray]:
-        """
-        Load model if unloaded/outside context; then run forward pass of model to get model predictions
+    # option 2:
+    with ModelAdapter.create(model) as adapter:
+        adapter.forward(...)
+    ```
+    """
+
+    @final
+    @classmethod
+    def create(
+        cls,
+        model_description: Union[v0_4.ModelDescr, v0_5.ModelDescr],
+        *,
+        devices: Optional[Sequence[str]] = None,
+        weight_format_priority_order: Optional[Sequence[WeightsFormat]] = None,
+    ):
         """
-        if not self.loaded:
-            self.load()
+        Creates model adapter based on the passed spec
+        Note: All specific adapters should happen inside this function to prevent different framework
+        initializations interfering with each other
+        """
+        if not isinstance(model_description, (v0_4.ModelDescr, v0_5.ModelDescr)):
+            raise TypeError(
+                f"expected v0_4.ModelDescr or v0_5.ModelDescr, but got {type(model_description)}"
+            )
+
+        weights = model_description.weights
+        errors: List[str] = []
+        weight_format_priority_order = (
+            DEFAULT_WEIGHT_FORMAT_PRIORITY_ORDER
+            if weight_format_priority_order is None
+            else weight_format_priority_order
+        )
+        for wf in weight_format_priority_order:
+            if wf == "pytorch_state_dict" and weights.pytorch_state_dict is not None:
+                try:
+                    from ._pytorch_model_adapter import PytorchModelAdapter
+
+                    return PytorchModelAdapter(
+                        outputs=model_description.outputs,
+                        weights=weights.pytorch_state_dict,
+                        devices=devices,
+                    )
+                except Exception as e:
+                    errors.append(f"{wf}: {e}")
+            elif (
+                wf == "tensorflow_saved_model_bundle"
+                and weights.tensorflow_saved_model_bundle is not None
+            ):
+                try:
+                    from ._tensorflow_model_adapter import TensorflowModelAdapter
+
+                    return TensorflowModelAdapter(
+                        model_description=model_description, devices=devices
+                    )
+                except Exception as e:
+                    errors.append(f"{wf}: {e}")
+            elif wf == "onnx" and weights.onnx is not None:
+                try:
+                    from ._onnx_model_adapter import ONNXModelAdapter
+
+                    return ONNXModelAdapter(
+                        model_description=model_description, devices=devices
+                    )
+                except Exception as e:
+                    errors.append(f"{wf}: {e}")
+            elif wf == "torchscript" and weights.torchscript is not None:
+                try:
+                    from ._torchscript_model_adapter import TorchscriptModelAdapter
+
+                    return TorchscriptModelAdapter(
+                        model_description=model_description, devices=devices
+                    )
+                except Exception as e:
+                    errors.append(f"{wf}: {e}")
+            elif wf == "keras_hdf5" and weights.keras_hdf5 is not None:
+                # keras can either be installed as a separate package or used as part of tensorflow
+                # we try to first import the keras model adapter using the separate package and,
+                # if it is not available, try to load the one using tf
+                try:
+                    from ._keras_model_adapter import (
+                        KerasModelAdapter,
+                        keras,  # type: ignore
+                    )
+
+                    if keras is None:
+                        from ._tensorflow_model_adapter import KerasModelAdapter
+
+                    return KerasModelAdapter(
+                        model_description=model_description, devices=devices
+                    )
+                except Exception as e:
+                    errors.append(f"{wf}: {e}")
+
+        assert errors
+        error_list = "\n - ".join(errors)
+        raise ValueError(
+            "None of the weight format specific model adapters could be created for"
+            + f" '{model_description.id or model_description.name}'"
+            + f" in this environment. Errors are:\n\n{error_list}.\n\n"
+        )
 
-        assert self.loaded
-        return self._forward(*input_tensors)
+    @final
+    def load(self, *, devices: Optional[Sequence[str]] = None) -> None:
+        warnings.warn("Deprecated. ModelAdapter is loaded on initialization")
 
-    @abc.abstractmethod
-    def _forward(self, *input_tensors: xr.DataArray) -> List[xr.DataArray]:
+    @abstractmethod
+    def forward(self, *input_tensors: Optional[Tensor]) -> List[Optional[Tensor]]:
         """
         Run forward pass of model to get model predictions
-        Note: model is responsible converting it's data representation to
-        xarray.DataArray
         """
-        ...
+        # TODO: handle tensor.transpose in here and make _forward_impl the abstract impl
 
+    @abstractmethod
     def unload(self):
         """
         Unload model from any devices, freeing their memory.
-        Note: Use ModelAdapter as context to not worry about calling unload()!
+        The moder adapter should be considered unusable afterwards.
         """
-        # implementation of non-state-machine logic in _unload()
-        assert self.loaded
-        self._unload()
-        self.loaded = False
-
-    @abc.abstractmethod
-    def _unload(self) -> None:
-        """
-        Unload model from any devices, freeing their memory.
-        """
-        ...
 
 
 def get_weight_formats() -> List[str]:
     """
     Return list of supported weight types
     """
-    return _WEIGHT_FORMATS.copy()
-
-
-def create_model_adapter(
-    *,
-    bioimageio_model: Union[nodes.Model, raw_nodes.Model],
-    devices=Optional[Sequence[str]],
-    weight_format: Optional[str] = None,
-) -> ModelAdapter:
-    """
-    Creates model adapter based on the passed spec
-    Note: All specific adapters should happen inside this function to prevent different framework
-    initializations interfering with each other
-    """
-    weights = bioimageio_model.weights
-    weight_formats = get_weight_formats()
-
-    if weight_format is not None:
-        if weight_format not in weight_formats:
-            raise ValueError(f"Weight format {weight_format} is not in supported formats {weight_formats}")
-        weight_formats = [weight_format]
-
-    for weight in weight_formats:
-        if weight in weights:
-            adapter_cls = _get_model_adapter(weight)
-            return adapter_cls(bioimageio_model=bioimageio_model, devices=devices)
-
-    raise RuntimeError(
-        f"weight format {weight_format} not among formats listed in model: {list(bioimageio_model.weights.keys())}"
-    )
-
-
-def _get_model_adapter(weight_format: str) -> Type[ModelAdapter]:
-    """
-    Return adapter class based on the weight format
-    Note: All specific adapters should happen inside this function to prevent different framework
-    initializations interfering with each other
-    """
-    if weight_format == "pytorch_state_dict":
-        from ._pytorch_model_adapter import PytorchModelAdapter
-
-        return PytorchModelAdapter
-
-    elif weight_format == "tensorflow_saved_model_bundle":
-        from ._tensorflow_model_adapter import TensorflowModelAdapter
-
-        return TensorflowModelAdapter
-
-    elif weight_format == "onnx":
-        from ._onnx_model_adapter import ONNXModelAdapter
-
-        return ONNXModelAdapter
-
-    elif weight_format == "torchscript":
-        from ._torchscript_model_adapter import TorchscriptModelAdapter
-
-        return TorchscriptModelAdapter
-
-    elif weight_format == "keras_hdf5":
-        # keras can either be installed as a separate package or used as part of tensorflow
-        # we try to first import the keras model adapter using the separate package and,
-        # if it is not available, try to load the one using tf
-        try:
-            from ._keras_model_adapter import KerasModelAdapter
-        except ImportError:
-            from ._tensorflow_model_adapter import KerasModelAdapter
+    return list(DEFAULT_WEIGHT_FORMAT_PRIORITY_ORDER)
 
-        return KerasModelAdapter
 
-    else:
-        raise ValueError(f"Weight format {weight_format} is not supported.")
+create_model_adapter = ModelAdapter.create
```

### Comparing `bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/_onnx_model_adapter.py` & `bioimageio.core-0.6.0/bioimageio/core/model_adapters/_onnx_model_adapter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,68 @@
-import logging
 import warnings
-from typing import List, Optional
+from typing import Any, List, Optional, Sequence, Union
 
-import onnxruntime as rt
-import xarray as xr
+from numpy.typing import NDArray
 
+from bioimageio.spec.model import v0_4, v0_5
+from bioimageio.spec.utils import download
+
+from ..digest_spec import get_axes_infos
+from ..tensor import Tensor
 from ._model_adapter import ModelAdapter
 
-logger = logging.getLogger(__name__)
+try:
+    import onnxruntime as rt
+except Exception:
+    rt = None
 
 
 class ONNXModelAdapter(ModelAdapter):
-    def _load(self, *, devices: Optional[List[str]] = None):
-        self._internal_output_axes = [tuple(out.axes) for out in self.bioimageio_model.outputs]
-
-        self._session = rt.InferenceSession(str(self.bioimageio_model.weights["onnx"].source))
-        onnx_inputs = self._session.get_inputs()
-        self._input_names = [ipt.name for ipt in onnx_inputs]
+    def __init__(
+        self,
+        *,
+        model_description: Union[v0_4.ModelDescr, v0_5.ModelDescr],
+        devices: Optional[Sequence[str]] = None,
+    ):
+        if rt is None:
+            raise ImportError("onnxruntime")
+
+        super().__init__()
+        self._internal_output_axes = [
+            tuple(a.id for a in get_axes_infos(out))
+            for out in model_description.outputs
+        ]
+        if model_description.weights.onnx is None:
+            raise ValueError("No ONNX weights specified for {model_description.name}")
+
+        self._session = rt.InferenceSession(
+            str(download(model_description.weights.onnx.source).path)
+        )
+        onnx_inputs = self._session.get_inputs()  # type: ignore
+        self._input_names: List[str] = [ipt.name for ipt in onnx_inputs]  # type: ignore
 
         if devices is not None:
-            warnings.warn(f"Device management is not implemented for onnx yet, ignoring the devices {devices}")
+            warnings.warn(
+                f"Device management is not implemented for onnx yet, ignoring the devices {devices}"
+            )
 
-    def _forward(self, *input_tensors: xr.DataArray) -> List[xr.DataArray]:
+    def forward(self, *input_tensors: Optional[Tensor]) -> List[Optional[Tensor]]:
         assert len(input_tensors) == len(self._input_names)
-        input_arrays = [ipt.data for ipt in input_tensors]
-        result = self._session.run(None, dict(zip(self._input_names, input_arrays)))
-        if not isinstance(result, (list, tuple)):
-            result = []
-
-        return [xr.DataArray(r, dims=axes) for r, axes in zip(result, self._internal_output_axes)]
-
-    def _unload(self) -> None:
-        warnings.warn("Device management is not implemented for onnx yet, cannot unload model")
+        input_arrays = [None if ipt is None else ipt.data.data for ipt in input_tensors]
+        result: Union[Sequence[Optional[NDArray[Any]]], Optional[NDArray[Any]]]
+        result = self._session.run(  # pyright: ignore[reportUnknownVariableType]
+            None, dict(zip(self._input_names, input_arrays))
+        )
+        if isinstance(result, (list, tuple)):
+            result_seq: Sequence[Optional[NDArray[Any]]] = result
+        else:
+            result_seq = [result]  # type: ignore
+
+        return [
+            None if r is None else Tensor(r, dims=axes)
+            for r, axes in zip(result_seq, self._internal_output_axes)
+        ]
+
+    def unload(self) -> None:
+        warnings.warn(
+            "Device management is not implemented for onnx yet, cannot unload model"
+        )
```

### Comparing `bioimageio.core-0.5.9/bioimageio/core/resource_tests.py` & `bioimageio.core-0.6.0/bioimageio/core/_resource_tests.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,333 +1,420 @@
-import os
-import re
 import traceback
 import warnings
-from copy import deepcopy
-from pathlib import Path
-from typing import List, Optional, Tuple, Union
+from typing import Dict, Hashable, List, Literal, Optional, Set, Tuple, Union
 
-import numpy
 import numpy as np
-import xarray as xr
-from marshmallow import ValidationError
 
-from bioimageio.core import __version__ as bioimageio_core_version, load_resource_description
-from bioimageio.core.common import TestSummary
-from bioimageio.core.prediction import predict
-from bioimageio.core.prediction_pipeline import create_prediction_pipeline
-from bioimageio.core.resource_io.nodes import (
-    ImplicitOutputShape,
-    Model,
-    ParametrizedInputShape,
-    ResourceDescription,
-    URI,
+from bioimageio.core.sample import Sample
+from bioimageio.spec import (
+    InvalidDescr,
+    ResourceDescr,
+    build_description,
+    dump_description,
+    load_description,
 )
-from bioimageio.core.resource_io.utils import SourceNodeChecker
-from bioimageio.spec import __version__ as bioimageio_spec_version
-from bioimageio.spec.model.raw_nodes import WeightsFormat
-from bioimageio.spec.shared import resolve_source
-from bioimageio.spec.shared.common import ValidationWarning
-from bioimageio.spec.shared.raw_nodes import ResourceDescription as RawResourceDescription
+from bioimageio.spec._internal.common_nodes import ResourceDescrBase
+from bioimageio.spec.common import BioimageioYamlContent, PermissiveFileSource
+from bioimageio.spec.model import v0_4, v0_5
+from bioimageio.spec.model.v0_5 import WeightsFormat
+from bioimageio.spec.summary import (
+    ErrorEntry,
+    InstalledPackage,
+    ValidationDetail,
+    ValidationSummary,
+)
+
+from ._prediction_pipeline import create_prediction_pipeline
+from .axis import AxisId, BatchSize
+from .digest_spec import get_test_inputs, get_test_outputs
+from .utils import VERSION
 
 
 def test_model(
-    model_rdf: Union[URI, Path, str],
+    source: Union[v0_5.ModelDescr, PermissiveFileSource],
     weight_format: Optional[WeightsFormat] = None,
     devices: Optional[List[str]] = None,
     decimal: int = 4,
-) -> List[TestSummary]:
-    """Test whether the test output(s) of a model can be reproduced."""
-    return test_resource(
-        model_rdf, weight_format=weight_format, devices=devices, decimal=decimal, expected_type="model"
+) -> ValidationSummary:
+    """Test model inference"""
+    return test_description(
+        source,
+        weight_format=weight_format,
+        devices=devices,
+        decimal=decimal,
+        expected_type="model",
     )
 
 
-def check_input_shape(shape: Tuple[int, ...], shape_spec) -> bool:
-    if isinstance(shape_spec, list):
-        if shape != tuple(shape_spec):
-            return False
-    elif isinstance(shape_spec, ParametrizedInputShape):
-        assert len(shape_spec.min) == len(shape_spec.step)
-        if len(shape) != len(shape_spec.min):
-            return False
-        min_shape = shape_spec.min
-        step = shape_spec.step
-        # check if the shape is valid for all dimension by seeing if it can be reached with an integer number of steps
-        # NOTE we allow that the valid shape is reached using a different number of steps for each axis here
-        # this is usually valid because dimensions are independent in neural networks
-        is_valid = [(sh - minsh) % st == 0 if st > 0 else sh == minsh for sh, st, minsh in zip(shape, step, min_shape)]
-        return all(is_valid)
-    else:
-        raise TypeError(f"Encountered unexpected shape description of type {type(shape_spec)}")
-
-    return True
+def test_description(
+    source: Union[ResourceDescr, PermissiveFileSource, BioimageioYamlContent],
+    *,
+    format_version: Union[Literal["discover", "latest"], str] = "discover",
+    weight_format: Optional[WeightsFormat] = None,
+    devices: Optional[List[str]] = None,
+    decimal: int = 4,
+    expected_type: Optional[str] = None,
+) -> ValidationSummary:
+    """Test a bioimage.io resource dynamically, e.g. prediction of test tensors for models"""
+    rd = load_description_and_test(
+        source,
+        format_version=format_version,
+        weight_format=weight_format,
+        devices=devices,
+        decimal=decimal,
+        expected_type=expected_type,
+    )
+    return rd.validation_summary
 
 
-def check_output_shape(shape: Tuple[int, ...], shape_spec, input_shapes) -> bool:
-    if isinstance(shape_spec, list):
-        return shape == tuple(shape_spec)
-    elif isinstance(shape_spec, ImplicitOutputShape):
-        ref_tensor = shape_spec.reference_tensor
-        if ref_tensor not in input_shapes:
-            raise ValidationError(f"The reference tensor name {ref_tensor} is not in {input_shapes}")
-        ipt_shape = numpy.array(input_shapes[ref_tensor])
-        scale = numpy.array([0.0 if sc is None else sc for sc in shape_spec.scale])
-        offset = numpy.array(shape_spec.offset)
-        exp_shape = numpy.round_(ipt_shape * scale) + 2 * offset
+def load_description_and_test(
+    source: Union[ResourceDescr, PermissiveFileSource, BioimageioYamlContent],
+    *,
+    format_version: Union[Literal["discover", "latest"], str] = "discover",
+    weight_format: Optional[WeightsFormat] = None,
+    devices: Optional[List[str]] = None,
+    decimal: int = 4,
+    expected_type: Optional[str] = None,
+) -> Union[ResourceDescr, InvalidDescr]:
+    """Test RDF dynamically, e.g. model inference of test inputs"""
+    if (
+        isinstance(source, ResourceDescrBase)
+        and format_version != "discover"
+        and source.format_version != format_version
+    ):
+        warnings.warn(
+            f"deserializing source to ensure we validate and test using format {format_version}"
+        )
+        source = dump_description(source)
 
-        return shape == tuple(exp_shape)
+    if isinstance(source, ResourceDescrBase):
+        rd = source
+    elif isinstance(source, dict):
+        rd = build_description(source, format_version=format_version)
     else:
-        raise TypeError(f"Encountered unexpected shape description of type {type(shape_spec)}")
-
-
-def _test_resource_urls(rd: ResourceDescription) -> TestSummary:
-    assert isinstance(rd, ResourceDescription)
-    with warnings.catch_warnings(record=True) as all_warnings:
-        try:
-            SourceNodeChecker(root_path=rd.root_path).visit(rd)
-        except FileNotFoundError as e:
-            error = str(e)
-            tb = traceback.format_tb(e.__traceback__)
-        else:
-            error = None
-            tb = None
+        rd = load_description(source, format_version=format_version)
 
-    return dict(
-        name="All URLs and paths available",
-        status="passed" if error is None else "failed",
-        error=error,
-        traceback=tb,
-        bioimageio_spec_version=bioimageio_spec_version,
-        bioimageio_core_version=bioimageio_core_version,
-        nested_errors=None,
-        source_name=rd.id or rd.id or rd.name if hasattr(rd, "id") else rd.name,
-        warnings={"SourceNodeChecker": [str(w.message) for w in all_warnings]} if all_warnings else {},
+    rd.validation_summary.env.append(
+        InstalledPackage(name="bioimageio.core", version=VERSION)
     )
 
+    if expected_type is not None:
+        _test_expected_resource_type(rd, expected_type)
 
-def _test_model_documentation(rd: ResourceDescription) -> TestSummary:
-    assert isinstance(rd, Model)
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore")
-        doc_path: Path = resolve_source(rd.documentation, root_path=rd.root_path)
-        doc = doc_path.read_text()
-        wrn = ""
-        if not re.match("#.*[vV]alidation", doc):
-            wrn = "No '# Validation' (sub)section found."
-
-        return dict(
-            name="Test documentation completeness.",
-            status="passed",
-            error=None,
-            traceback=None,
-            bioimageio_spec_version=bioimageio_spec_version,
-            bioimageio_core_version=bioimageio_core_version,
-            source_name=rd.id or rd.name if hasattr(rd, "id") else rd.name,
-            warnings={"documentation": wrn} if wrn else {},
-        )
+    if isinstance(rd, (v0_4.ModelDescr, v0_5.ModelDescr)):
+        _test_model_inference(rd, weight_format, devices, decimal)
+        if not isinstance(rd, v0_4.ModelDescr):
+            _test_model_inference_parametrized(rd, weight_format, devices)
+
+    # TODO: add execution of jupyter notebooks
+    # TODO: add more tests
+
+    return rd
+
+
+def _test_model_inference(
+    model: Union[v0_4.ModelDescr, v0_5.ModelDescr],
+    weight_format: Optional[WeightsFormat],
+    devices: Optional[List[str]],
+    decimal: int,
+) -> None:
+    error: Optional[str] = None
+    tb: List[str] = []
+    try:
+        inputs = get_test_inputs(model)
+        expected = get_test_outputs(model)
 
+        with create_prediction_pipeline(
+            bioimageio_model=model, devices=devices, weight_format=weight_format
+        ) as prediction_pipeline:
+            results = prediction_pipeline.predict_sample_without_blocking(inputs)
 
-def _test_model_inference(model: Model, weight_format: str, devices: Optional[List[str]], decimal: int) -> TestSummary:
-    error: Optional[str] = None
-    tb: Optional = None
-    with warnings.catch_warnings(record=True) as all_warnings:
-        try:
-            inputs = [np.load(str(in_path)) for in_path in model.test_inputs]
-            expected = [np.load(str(out_path)) for out_path in model.test_outputs]
-
-            assert len(inputs) == len(model.inputs)  # should be checked by validation
-            input_shapes = {}
-            for idx, (ipt, ipt_spec) in enumerate(zip(inputs, model.inputs)):
-                if not check_input_shape(tuple(ipt.shape), ipt_spec.shape):
-                    raise ValidationError(
-                        f"Shape {tuple(ipt.shape)} of test input {idx} '{ipt_spec.name}' does not match "
-                        f"input shape description: {ipt_spec.shape}."
-                    )
-                input_shapes[ipt_spec.name] = ipt.shape
+        if len(results.members) != len(expected.members):
+            error = f"Expected {len(expected.members)} outputs, but got {len(results.members)}"
 
-            assert len(expected) == len(model.outputs)  # should be checked by validation
-            for idx, (out, out_spec) in enumerate(zip(expected, model.outputs)):
-                if not check_output_shape(tuple(out.shape), out_spec.shape, input_shapes):
-                    error = (error or "") + (
-                        f"Shape {tuple(out.shape)} of test output {idx} '{out_spec.name}' does not match "
-                        f"output shape description: {out_spec.shape}."
+        else:
+            for m, exp in expected.members.items():
+                res = results.members.get(m)
+                if res is None:
+                    error = "Output tensors for test case may not be None"
+                    break
+                try:
+                    np.testing.assert_array_almost_equal(
+                        res.data, exp.data, decimal=decimal
                     )
+                except AssertionError as e:
+                    error = f"Output and expected output disagree:\n {e}"
+                    break
+    except Exception as e:
+        error = str(e)
+        tb = traceback.format_tb(e.__traceback__)
 
-            with create_prediction_pipeline(
-                bioimageio_model=model, devices=devices, weight_format=weight_format
-            ) as prediction_pipeline:
-                results = predict(prediction_pipeline, inputs)
-
-            if len(results) != len(expected):
-                error = (error or "") + (
-                    f"Number of outputs and number of expected outputs disagree: {len(results)} != {len(expected)}"
-                )
-            else:
-                for res, exp in zip(results, expected):
-                    try:
-                        np.testing.assert_array_almost_equal(res, exp, decimal=decimal)
-                    except AssertionError as e:
-                        error = (error or "") + f"Output and expected output disagree:\n {e}"
-        except Exception as e:
-            error = str(e)
-            tb = traceback.format_tb(e.__traceback__)
-
-    return dict(
-        name=f"reproduce test outputs from test inputs (bioimageio.core {bioimageio_core_version})",
-        status="passed" if error is None else "failed",
-        error=error,
-        traceback=tb,
-        bioimageio_spec_version=bioimageio_spec_version,
-        bioimageio_core_version=bioimageio_core_version,
-        warnings=ValidationWarning.get_warning_summary(all_warnings),
-        source_name=model.id or model.name,
+    model.validation_summary.add_detail(
+        ValidationDetail(
+            name="Reproduce test outputs from test inputs",
+            status="passed" if error is None else "failed",
+            errors=(
+                []
+                if error is None
+                else [
+                    ErrorEntry(
+                        loc=(
+                            ("weights",)
+                            if weight_format is None
+                            else ("weights", weight_format)
+                        ),
+                        msg=error,
+                        type="bioimageio.core",
+                        traceback=tb,
+                    )
+                ]
+            ),
+        )
     )
 
 
-def _test_load_resource(
-    rdf: Union[RawResourceDescription, ResourceDescription, URI, Path, str],
-    weight_format: Optional[WeightsFormat] = None,
-) -> Tuple[Optional[ResourceDescription], TestSummary]:
-    if isinstance(rdf, (URI, os.PathLike)):
-        source_name = str(rdf)
-    elif isinstance(rdf, str):
-        source_name = rdf[:120]
-    else:
-        source_name = rdf.id if hasattr(rdf, "id") else rdf.name
+def _test_model_inference_parametrized(
+    model: v0_5.ModelDescr,
+    weight_format: Optional[WeightsFormat],
+    devices: Optional[List[str]],
+    test_cases: Set[Tuple[v0_5.ParameterizedSize.N, BatchSize]] = {
+        (0, 2),
+        (1, 3),
+        (2, 1),
+        (3, 2),
+    },
+) -> None:
+    if not test_cases:
+        return
+
+    if not any(
+        isinstance(a.size, v0_5.ParameterizedSize)
+        for ipt in model.inputs
+        for a in ipt.axes
+    ):
+        # no parameterized sizes => set n=0
+        test_cases = {(0, b) for _n, b in test_cases}
+
+    if not any(isinstance(a, v0_5.BatchAxis) for ipt in model.inputs for a in ipt.axes):
+        # no batch axis => set b=1
+        test_cases = {(n, 1) for n, _b in test_cases}
+
+    def generate_test_cases():
+        tested: Set[Hashable] = set()
+
+        def get_ns(n: int):
+            return {
+                (t.id, a.id): n
+                for t in model.inputs
+                for a in t.axes
+                if isinstance(a.size, v0_5.ParameterizedSize)
+            }
+
+        for n, batch_size in sorted(test_cases):
+            input_target_sizes, expected_output_sizes = model.get_axis_sizes(
+                get_ns(n), batch_size=batch_size
+            )
+            hashable_target_size = tuple(
+                (k, input_target_sizes[k]) for k in sorted(input_target_sizes)
+            )
+            if hashable_target_size in tested:
+                continue
+            else:
+                tested.add(hashable_target_size)
 
-    main_test_warnings = []
-    try:
-        with warnings.catch_warnings(record=True) as all_warnings:
-            rd: Optional[ResourceDescription] = load_resource_description(
-                rdf, weights_priority_order=None if weight_format is None else [weight_format]
+            resized_test_inputs = Sample(
+                members={
+                    t.id: test_inputs.members[t.id].resize_to(
+                        {
+                            aid: s
+                            for (tid, aid), s in input_target_sizes.items()
+                            if tid == t.id
+                        },
+                    )
+                    for t in model.inputs
+                },
+                stat=test_inputs.stat,
+                id=test_inputs.id,
             )
+            expected_output_shapes = {
+                t.id: {
+                    aid: s
+                    for (tid, aid), s in expected_output_sizes.items()
+                    if tid == t.id
+                }
+                for t in model.outputs
+            }
+            yield n, batch_size, resized_test_inputs, expected_output_shapes
 
-            main_test_warnings += list(all_warnings)
-    except Exception as e:
-        rd = None
-        error: Optional[str] = str(e)
-        tb: Optional = traceback.format_tb(e.__traceback__)
-    else:
-        error = None
-        tb = None
+    try:
+        test_inputs = get_test_inputs(model)
 
-    load_summary = TestSummary(
-        name="load resource description",
-        status="passed" if error is None else "failed",
-        error=error,
-        nested_errors=None,
-        traceback=tb,
-        bioimageio_spec_version=bioimageio_spec_version,
-        bioimageio_core_version=bioimageio_core_version,
-        warnings={},
-        source_name=source_name,
-    )
+        with create_prediction_pipeline(
+            bioimageio_model=model, devices=devices, weight_format=weight_format
+        ) as prediction_pipeline:
+            for n, batch_size, inputs, exptected_output_shape in generate_test_cases():
+                error: Optional[str] = None
+                result = prediction_pipeline.predict_sample_with_blocking(inputs)
+                if len(result.members) != len(exptected_output_shape):
+                    error = (
+                        f"Expected {len(exptected_output_shape)} outputs,"
+                        + f" but got {len(result.members)}"
+                    )
 
-    return rd, load_summary
+                else:
+                    for m, exp in exptected_output_shape.items():
+                        res = result.members.get(m)
+                        if res is None:
+                            error = "Output tensors may not be None for test case"
+                            break
+
+                        diff: Dict[AxisId, int] = {}
+                        for a, s in res.sizes.items():
+                            if isinstance((e_aid := exp[AxisId(a)]), int):
+                                if s != e_aid:
+                                    diff[AxisId(a)] = s
+                            elif (
+                                s < e_aid.min or e_aid.max is not None and s > e_aid.max
+                            ):
+                                diff[AxisId(a)] = s
+                        if diff:
+                            error = (
+                                f"(n={n}) Expected output shape {exp},"
+                                + f" but got {res.sizes} (diff: {diff})"
+                            )
+                            break
+
+                model.validation_summary.add_detail(
+                    ValidationDetail(
+                        name="Run inference for inputs with batch_size:"
+                        + f" {batch_size} and size parameter n: {n}",
+                        status="passed" if error is None else "failed",
+                        errors=(
+                            []
+                            if error is None
+                            else [
+                                ErrorEntry(
+                                    loc=(
+                                        ("weights",)
+                                        if weight_format is None
+                                        else ("weights", weight_format)
+                                    ),
+                                    msg=error,
+                                    type="bioimageio.core",
+                                )
+                            ]
+                        ),
+                    )
+                )
+    except Exception as e:
+        error = str(e)
+        tb = traceback.format_tb(e.__traceback__)
+        model.validation_summary.add_detail(
+            ValidationDetail(
+                name="Run inference for parametrized inputs",
+                status="failed",
+                errors=[
+                    ErrorEntry(
+                        loc=(
+                            ("weights",)
+                            if weight_format is None
+                            else ("weights", weight_format)
+                        ),
+                        msg=error,
+                        type="bioimageio.core",
+                        traceback=tb,
+                    )
+                ],
+            )
+        )
 
 
-def _test_expected_resource_type(rd: ResourceDescription, expected_type: str) -> TestSummary:
+def _test_expected_resource_type(
+    rd: Union[InvalidDescr, ResourceDescr], expected_type: str
+):
     has_expected_type = rd.type == expected_type
-    return dict(
-        name="has expected resource type",
-        status="passed" if has_expected_type else "failed",
-        error=None if has_expected_type else f"expected type {expected_type}, found {rd.type}",
-        traceback=None,
-        source_name=rd.id or rd.name if hasattr(rd, "id") else rd.name,
+    rd.validation_summary.details.append(
+        ValidationDetail(
+            name="Has expected resource type",
+            status="passed" if has_expected_type else "failed",
+            errors=(
+                []
+                if has_expected_type
+                else [
+                    ErrorEntry(
+                        loc=("type",),
+                        type="type",
+                        msg=f"expected type {expected_type}, found {rd.type}",
+                    )
+                ]
+            ),
+        )
     )
 
 
-def test_resource(
-    rdf: Union[RawResourceDescription, ResourceDescription, URI, Path, str],
-    *,
-    weight_format: Optional[WeightsFormat] = None,
-    devices: Optional[List[str]] = None,
-    decimal: int = 4,
-    expected_type: Optional[str] = None,
-) -> List[TestSummary]:
-    """Test RDF dynamically
-
-    Returns: summary dict with keys: name, status, error, traceback, bioimageio_spec_version, bioimageio_core_version
-    """
-    rd, load_test = _test_load_resource(rdf, weight_format)
-    tests: List[TestSummary] = [load_test]
-    if rd is not None:
-        if expected_type is not None:
-            tests.append(_test_expected_resource_type(rd, expected_type))
-
-        tests.append(_test_resource_urls(rd))
-
-    if isinstance(rd, Model):
-        tests.append(_test_model_documentation(rd))
-        tests.append(_test_model_inference(rd, weight_format, devices, decimal))
-
-    return tests
-
-
-def debug_model(
-    model_rdf: Union[RawResourceDescription, ResourceDescription, URI, Path, str],
-    *,
-    weight_format: Optional[WeightsFormat] = None,
-    devices: Optional[List[str]] = None,
-):
-    """Run the model test and return dict with inputs, results, expected results and intermediates.
-
-    Returns dict with tensors "inputs", "inputs_processed", "outputs_raw", "outputs", "expected" and "diff".
-    """
-    inputs_raw: Optional = None
-    inputs_processed: Optional = None
-    outputs_raw: Optional = None
-    outputs: Optional = None
-    expected: Optional = None
-    diff: Optional = None
-
-    model = load_resource_description(
-        model_rdf, weights_priority_order=None if weight_format is None else [weight_format]
-    )
-    if not isinstance(model, Model):
-        raise ValueError(f"Not a bioimageio.model: {model_rdf}")
-
-    prediction_pipeline = create_prediction_pipeline(
-        bioimageio_model=model, devices=devices, weight_format=weight_format
-    )
-    inputs = [
-        xr.DataArray(np.load(str(in_path)), dims=input_spec.axes)
-        for in_path, input_spec in zip(model.test_inputs, model.inputs)
-    ]
-    input_dict = {input_spec.name: input for input_spec, input in zip(model.inputs, inputs)}
-
-    # keep track of the non-processed inputs
-    inputs_raw = [deepcopy(input) for input in inputs]
-
-    computed_measures = {}
-
-    prediction_pipeline.apply_preprocessing(input_dict, computed_measures)
-    inputs_processed = list(input_dict.values())
-    outputs_raw = prediction_pipeline.predict(*inputs_processed)
-    output_dict = {output_spec.name: deepcopy(output) for output_spec, output in zip(model.outputs, outputs_raw)}
-    prediction_pipeline.apply_postprocessing(output_dict, computed_measures)
-    outputs = list(output_dict.values())
-
-    if isinstance(outputs, (np.ndarray, xr.DataArray)):
-        outputs = [outputs]
-
-    expected = [
-        xr.DataArray(np.load(str(out_path)), dims=output_spec.axes)
-        for out_path, output_spec in zip(model.test_outputs, model.outputs)
-    ]
-    if len(outputs) != len(expected):
-        error = f"Number of outputs and number of expected outputs disagree: {len(outputs)} != {len(expected)}"
-        print(error)
-    else:
-        diff = []
-        for res, exp in zip(outputs, expected):
-            diff.append(res - exp)
-
-    return {
-        "inputs": inputs_raw,
-        "inputs_processed": inputs_processed,
-        "outputs_raw": outputs_raw,
-        "outputs": outputs,
-        "expected": expected,
-        "diff": diff,
-    }
+# def debug_model(
+#     model_rdf: Union[RawResourceDescr, ResourceDescr, URI, Path, str],
+#     *,
+#     weight_format: Optional[WeightsFormat] = None,
+#     devices: Optional[List[str]] = None,
+# ):
+#     """Run the model test and return dict with inputs, results, expected results and intermediates.
+
+#     Returns dict with tensors "inputs", "inputs_processed", "outputs_raw", "outputs", "expected" and "diff".
+#     """
+#     inputs_raw: Optional = None
+#     inputs_processed: Optional = None
+#     outputs_raw: Optional = None
+#     outputs: Optional = None
+#     expected: Optional = None
+#     diff: Optional = None
+
+#     model = load_description(
+#         model_rdf, weights_priority_order=None if weight_format is None else [weight_format]
+#     )
+#     if not isinstance(model, Model):
+#         raise ValueError(f"Not a bioimageio.model: {model_rdf}")
+
+#     prediction_pipeline = create_prediction_pipeline(
+#         bioimageio_model=model, devices=devices, weight_format=weight_format
+#     )
+#     inputs = [
+#         xr.DataArray(load_array(str(in_path)), dims=input_spec.axes)
+#         for in_path, input_spec in zip(model.test_inputs, model.inputs)
+#     ]
+#     input_dict = {input_spec.name: input for input_spec, input in zip(model.inputs, inputs)}
+
+#     # keep track of the non-processed inputs
+#     inputs_raw = [deepcopy(input) for input in inputs]
+
+#     computed_measures = {}
+
+#     prediction_pipeline.apply_preprocessing(input_dict, computed_measures)
+#     inputs_processed = list(input_dict.values())
+#     outputs_raw = prediction_pipeline.predict(*inputs_processed)
+#     output_dict = {output_spec.name: deepcopy(output) for output_spec, output in zip(model.outputs, outputs_raw)}
+#     prediction_pipeline.apply_postprocessing(output_dict, computed_measures)
+#     outputs = list(output_dict.values())
+
+#     if isinstance(outputs, (np.ndarray, xr.DataArray)):
+#         outputs = [outputs]
+
+#     expected = [
+#         xr.DataArray(load_array(str(out_path)), dims=output_spec.axes)
+#         for out_path, output_spec in zip(model.test_outputs, model.outputs)
+#     ]
+#     if len(outputs) != len(expected):
+#         error = f"Number of outputs and number of expected outputs disagree: {len(outputs)} != {len(expected)}"
+#         print(error)
+#     else:
+#         diff = []
+#         for res, exp in zip(outputs, expected):
+#             diff.append(res - exp)
+
+#     return {
+#         "inputs": inputs_raw,
+#         "inputs_processed": inputs_processed,
+#         "outputs_raw": outputs_raw,
+#         "outputs": outputs,
+#         "expected": expected,
+#         "diff": diff,
+#     }
```

### Comparing `bioimageio.core-0.5.9/bioimageio/core/weight_converter/keras/tensorflow.py` & `bioimageio.core-0.6.0/bioimageio/core/weight_converter/keras/_tensorflow.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,130 +1,151 @@
+# type: ignore  # TODO: type
 import os
 import shutil
 from pathlib import Path
-from typing import Union
+from typing import no_type_check
 from zipfile import ZipFile
 
-import bioimageio.spec as spec
-from bioimageio.core import load_resource_description
-
-import tensorflow
-from tensorflow import saved_model
-
-
-def _zip_weights(output_path):
-    zipped_model = f"{output_path}.zip"
-    # zip the weights
-    file_paths = []
-    for folder_names, subfolder, filenames in os.walk(os.path.join(output_path)):
-        for filename in filenames:
-            # create complete filepath of file in directory
-            file_paths.append(os.path.join(folder_names, filename))
-
-    with ZipFile(zipped_model, "w") as zip_obj:
-        for f in file_paths:
-            # Add file to zip
-            zip_obj.write(f, os.path.relpath(f, output_path))
+try:
+    import tensorflow.saved_model
+except Exception:
+    tensorflow = None
+
+from bioimageio.spec._internal.io_utils import download
+from bioimageio.spec.model.v0_5 import ModelDescr
+
+
+def _zip_model_bundle(model_bundle_folder: Path):
+    zipped_model_bundle = model_bundle_folder.with_suffix(".zip")
+
+    with ZipFile(zipped_model_bundle, "w") as zip_obj:
+        for root, _, files in os.walk(model_bundle_folder):
+            for filename in files:
+                src = os.path.join(root, filename)
+                zip_obj.write(src, os.path.relpath(src, model_bundle_folder))
 
     try:
-        shutil.rmtree(output_path)
+        shutil.rmtree(model_bundle_folder)
     except Exception:
         print("TensorFlow bundled model was not removed after compression")
 
-    return zipped_model
+    return zipped_model_bundle
 
 
 # adapted from
 # https://github.com/deepimagej/pydeepimagej/blob/master/pydeepimagej/yaml/create_config.py#L236
-def _convert_tf1(keras_weight_path, output_path, input_name, output_name, zip_weights):
+def _convert_tf1(
+    keras_weight_path: Path,
+    output_path: Path,
+    input_name: str,
+    output_name: str,
+    zip_weights: bool,
+):
+    try:
+        # try to build the tf model with the keras import from tensorflow
+        from bioimageio.core.weight_converter.keras._tensorflow import (
+            keras,  # type: ignore
+        )
+
+    except Exception:
+        # if the above fails try to export with the standalone keras
+        import keras
+
+    @no_type_check
     def build_tf_model():
         keras_model = keras.models.load_model(keras_weight_path)
-
-        builder = saved_model.builder.SavedModelBuilder(output_path)
-        signature = saved_model.signature_def_utils.predict_signature_def(
-            inputs={input_name: keras_model.input}, outputs={output_name: keras_model.output}
+        assert tensorflow is not None
+        builder = tensorflow.saved_model.builder.SavedModelBuilder(output_path)
+        signature = tensorflow.saved_model.signature_def_utils.predict_signature_def(
+            inputs={input_name: keras_model.input},
+            outputs={output_name: keras_model.output},
         )
 
-        signature_def_map = {saved_model.signature_constants.DEFAULT_SERVING_SIGNATURE_DEF_KEY: signature}
+        signature_def_map = {
+            tensorflow.saved_model.signature_constants.DEFAULT_SERVING_SIGNATURE_DEF_KEY: signature
+        }
 
         builder.add_meta_graph_and_variables(
-            keras.backend.get_session(), [saved_model.tag_constants.SERVING], signature_def_map=signature_def_map
+            keras.backend.get_session(),
+            [tensorflow.saved_model.tag_constants.SERVING],
+            signature_def_map=signature_def_map,
         )
         builder.save()
 
-    try:
-        # try to build the tf model with the keras import from tensorflow
-        from tensorflow import keras
-        build_tf_model()
-    except Exception:
-        # if the above fails try to export with the standalone keras
-        import keras
-
-        build_tf_model()
+    build_tf_model()
 
     if zip_weights:
-        output_path = _zip_weights(output_path)
+        output_path = _zip_model_bundle(output_path)
     print("TensorFlow model exported to", output_path)
 
     return 0
 
 
-def _convert_tf2(keras_weight_path, output_path, zip_weights):
+def _convert_tf2(keras_weight_path: Path, output_path: Path, zip_weights: bool):
     try:
         # try to build the tf model with the keras import from tensorflow
-        from tensorflow import keras
+        from bioimageio.core.weight_converter.keras._tensorflow import keras
     except Exception:
         # if the above fails try to export with the standalone keras
         import keras
 
     model = keras.models.load_model(keras_weight_path)
     keras.models.save_model(model, output_path)
 
     if zip_weights:
-        output_path = _zip_weights(output_path)
+        output_path = _zip_model_bundle(output_path)
     print("TensorFlow model exported to", output_path)
 
     return 0
 
 
 def convert_weights_to_tensorflow_saved_model_bundle(
-    model_spec: Union[str, Path, spec.model.raw_nodes.Model], output_path: Union[str, Path]
+    model: ModelDescr, output_path: Path
 ):
     """Convert model weights from format 'keras_hdf5' to 'tensorflow_saved_model_bundle'.
 
     Adapted from
     https://github.com/deepimagej/pydeepimagej/blob/5aaf0e71f9b04df591d5ca596f0af633a7e024f5/pydeepimagej/yaml/create_config.py
 
     Args:
-        model_spec: location of the resource for the input bioimageio model
+        model: The bioimageio model description
         output_path: where to save the tensorflow weights. This path must not exist yet.
     """
+    assert tensorflow is not None
     tf_major_ver = int(tensorflow.__version__.split(".")[0])
 
-    path_ = Path(output_path)
-    if path_.suffix == ".zip":
-        path_ = Path(os.path.splitext(path_)[0])
+    if output_path.suffix == ".zip":
+        output_path = output_path.with_suffix("")
         zip_weights = True
     else:
         zip_weights = False
 
-    if path_.exists():
-        raise ValueError(f"The ouptut directory at {path_} must not exist.")
+    if output_path.exists():
+        raise ValueError(f"The ouptut directory at {output_path} must not exist.")
+
+    if model.weights.keras_hdf5 is None:
+        raise ValueError("Missing Keras Hdf5 weights to convert from.")
 
-    model = load_resource_description(model_spec)
-    assert "keras_hdf5" in model.weights
-    weight_spec = model.weights["keras_hdf5"]
-    weight_path = str(weight_spec.source)
+    weight_spec = model.weights.keras_hdf5
+    weight_path = download(weight_spec.source).path
 
     if weight_spec.tensorflow_version:
         model_tf_major_ver = int(weight_spec.tensorflow_version.major)
         if model_tf_major_ver != tf_major_ver:
-            raise RuntimeError(f"Tensorflow major versions of model {model_tf_major_ver} is not {tf_major_ver}")
+            raise RuntimeError(
+                f"Tensorflow major versions of model {model_tf_major_ver} is not {tf_major_ver}"
+            )
 
     if tf_major_ver == 1:
         if len(model.inputs) != 1 or len(model.outputs) != 1:
             raise NotImplementedError(
                 "Weight conversion for models with multiple inputs or outputs is not yet implemented."
             )
-        return _convert_tf1(weight_path, str(path_), model.inputs[0].name, model.outputs[0].name, zip_weights)
+        return _convert_tf1(
+            weight_path,
+            output_path,
+            model.inputs[0].id,
+            model.outputs[0].id,
+            zip_weights,
+        )
     else:
-        return _convert_tf2(weight_path, str(path_), zip_weights)
+        return _convert_tf2(weight_path, output_path, zip_weights)
```

### Comparing `bioimageio.core-0.5.9/bioimageio/core/weight_converter/torch/onnx.py` & `bioimageio.core-0.6.0/bioimageio/core/weight_converter/torch/_onnx.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,80 +1,106 @@
+# type: ignore  # TODO: type
 import warnings
 from pathlib import Path
-from typing import Union, Optional
+from typing import Any, List, Sequence, cast
 
 import numpy as np
-import torch
 from numpy.testing import assert_array_almost_equal
 
-import bioimageio.spec as spec
-from bioimageio.core import load_resource_description
-from bioimageio.core.resource_io import nodes
-from .utils import load_model
+from bioimageio.spec import load_description
+from bioimageio.spec.common import InvalidDescr
+from bioimageio.spec.model import v0_4, v0_5
+
+from ...digest_spec import get_member_id, get_test_inputs
+from ...weight_converter.torch._utils import load_torch_model
 
 try:
-    import onnxruntime as rt
+    import torch
 except ImportError:
-    rt = None
+    torch = None
 
 
-def convert_weights_to_onnx(
-    model_spec: Union[str, Path, spec.model.raw_nodes.Model],
-    output_path: Union[str, Path],
-    opset_version: Optional[int] = 12,
+def add_onnx_weights(
+    model_spec: "str | Path | v0_4.ModelDescr | v0_5.ModelDescr",
+    *,
+    output_path: Path,
     use_tracing: bool = True,
-    verbose: bool = True,
-    test_decimal: int = 4
+    test_decimal: int = 4,
+    verbose: bool = False,
+    opset_version: "int | None" = None,
 ):
     """Convert model weights from format 'pytorch_state_dict' to 'onnx'.
 
     Args:
-        model_spec: location of the resource for the input bioimageio model
-        output_path: where to save the onnx weights
+        source_model: model without onnx weights
         opset_version: onnx opset version
         use_tracing: whether to use tracing or scripting to export the onnx format
-        verbose: be verbose during the onnx export
         test_decimal: precision for testing whether the results agree
     """
     if isinstance(model_spec, (str, Path)):
-        model_spec = load_resource_description(Path(model_spec))
+        loaded_spec = load_description(Path(model_spec))
+        if isinstance(loaded_spec, InvalidDescr):
+            raise ValueError(f"Bad resource description: {loaded_spec}")
+        if not isinstance(loaded_spec, (v0_4.ModelDescr, v0_5.ModelDescr)):
+            raise TypeError(
+                f"Path {model_spec} is a {loaded_spec.__class__.__name__}, expected a v0_4.ModelDescr or v0_5.ModelDescr"
+            )
+        model_spec = loaded_spec
+
+    state_dict_weights_descr = model_spec.weights.pytorch_state_dict
+    if state_dict_weights_descr is None:
+        raise ValueError(
+            "The provided model does not have weights in the pytorch state dict format"
+        )
 
-    assert isinstance(model_spec, nodes.Model)
+    assert torch is not None
     with torch.no_grad():
-        # load input and expected output data
-        input_data = [np.load(inp).astype("float32") for inp in model_spec.test_inputs]
-        input_tensors = [torch.from_numpy(inp) for inp in input_data]
-
-        # instantiate and generate the expected output
-        model = load_model(model_spec)
-        expected_outputs = model(*input_tensors)
-        if isinstance(expected_outputs, torch.Tensor):
-            expected_outputs = [expected_outputs]
-        expected_outputs = [out.numpy() for out in expected_outputs]
+
+        sample = get_test_inputs(model_spec)
+        input_data = [sample[get_member_id(ipt)].data.data for ipt in model_spec.inputs]
+        input_tensors = [torch.from_numpy(ipt) for ipt in input_data]
+        model = load_torch_model(state_dict_weights_descr)
+
+        expected_tensors = model(*input_tensors)
+        if isinstance(expected_tensors, torch.Tensor):
+            expected_tensors = [expected_tensors]
+        expected_outputs: List[np.ndarray[Any, Any]] = [
+            out.numpy() for out in expected_tensors
+        ]
 
         if use_tracing:
             torch.onnx.export(
                 model,
-                input_tensors if len(input_tensors) > 1 else input_tensors[0],
-                output_path,
+                tuple(input_tensors) if len(input_tensors) > 1 else input_tensors[0],
+                str(output_path),
                 verbose=verbose,
                 opset_version=opset_version,
             )
         else:
             raise NotImplementedError
 
-    if rt is None:
+    try:
+        import onnxruntime as rt  # pyright: ignore [reportMissingTypeStubs]
+    except ImportError:
         msg = "The onnx weights were exported, but onnx rt is not available and weights cannot be checked."
         warnings.warn(msg)
-        return 1
+        return
 
     # check the onnx model
-    sess = rt.InferenceSession(str(output_path))  # does not support Path, so need to cast to str
-    onnx_inputs = {input_name.name: inp for input_name, inp in zip(sess.get_inputs(), input_data)}
-    outputs = sess.run(None, onnx_inputs)
+    sess = rt.InferenceSession(str(output_path))
+    onnx_input_node_args = cast(
+        List[Any], sess.get_inputs()
+    )  # fixme: remove cast, try using rt.NodeArg instead of Any
+    onnx_inputs = {
+        input_name.name: inp
+        for input_name, inp in zip(onnx_input_node_args, input_data)
+    }
+    outputs = cast(
+        Sequence[np.ndarray[Any, Any]], sess.run(None, onnx_inputs)
+    )  # FIXME: remove cast
 
     try:
         for exp, out in zip(expected_outputs, outputs):
             assert_array_almost_equal(exp, out, decimal=test_decimal)
         return 0
     except AssertionError as e:
         msg = f"The onnx weights were exported, but results before and after conversion do not agree:\n {str(e)}"
```

### Comparing `bioimageio.core-0.5.9/bioimageio.core.egg-info/PKG-INFO` & `bioimageio.core-0.6.0/bioimageio.core.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,117 +1,147 @@
 Metadata-Version: 2.1
 Name: bioimageio.core
-Version: 0.5.9
+Version: 0.6.0
 Summary: Python functionality for the bioimage model zoo
 Home-page: https://github.com/bioimage-io/core-bioimage-io-python
 Author: Bioimage Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/core-bioimage-io-python/issues
 Project-URL: Source, https://github.com/bioimage-io/core-bioimage-io-python
 Description: # core-bioimage-io-python
         
         Python specific core utilities for running models in the [BioImage Model Zoo](https://bioimage.io).
         
         ## Installation
         
-        ### Via Conda
+        ### Via Mamba/Conda
         
         The `bioimageio.core` package can be installed from conda-forge via
+        
+        ```console
+        mamba install -c conda-forge bioimageio.core
         ```
-        conda install -c conda-forge bioimageio.core
-        ```
-        if you don't install any additional deep learning libraries, you will only be able to use general convenience functionality, but not any functionality for model prediction.
+        
+        If you do not install any additional deep learning libraries, you will only be able to use general convenience
+        functionality, but not any functionality for model prediction.
         To install additional deep learning libraries use:
         
         * Pytorch/Torchscript:
-          ```bash
-          # cpu installation (if you don't have an nvidia graphics card)
-          conda install -c pytorch -c conda-forge bioimageio.core pytorch torchvision cpuonly
         
-          # gpu installation (for cuda 11.6, please choose the appropriate cuda version for your system)
-          conda install -c pytorch -c nvidia -c conda-forge bioimageio.core pytorch torchvision pytorch-cuda=11.6 
+          CPU installation (if you don't have an nvidia graphics card):
+        
+          ```console
+          mamba install -c pytorch -c conda-forge bioimageio.core pytorch torchvision cpuonly
           ```
-          Note that the pytorch installation instructions may change in the future. For the latest instructions please refer to [pytorch.org](https://pytorch.org/).
         
+          GPU installation (for cuda 11.6, please choose the appropriate cuda version for your system):
+        
+          ```console
+          mamba install -c pytorch -c nvidia -c conda-forge bioimageio.core pytorch torchvision pytorch-cuda=11.8
+          ```
+        
+          Note that the pytorch installation instructions may change in the future. For the latest instructions please refer to [pytorch.org](https://pytorch.org/).
         
         * Tensorflow
-          ```bash
-          # currently only cpu version supported
-          conda install -c conda-forge bioimageio.core tensorflow
+        
+          Currently only CPU version supported
+        
+          ```console
+          mamba install -c conda-forge bioimageio.core tensorflow
           ```
         
         * ONNXRuntime
-          ```bash
-          # currently only cpu version supported
-          conda install -c conda-forge bioimageio.core onnxruntime
+        
+          Currently only cpu version supported
+        
+          ```console
+          mamba install -c conda-forge bioimageio.core onnxruntime
           ```
-          
+        
         ### Via pip
         
-        The package is also available via pip:
-        ```
-        pip install bioimageio.core
+        The package is also available via pip
+        (e.g. with recommended extras `onnx` and `pytorch`):
+        
+        ```console
+        pip install bioimageio.core[onnx,pytorch]
         ```
         
         ### Set up Development Environment
         
         To set up a development conda environment run the following commands:
-        ```
-        conda env create -f dev/environment-base.yaml
-        conda activate bio-core-dev
+        
+        ```console
+        mamba env create -f dev/env.yaml
+        mamba activate core
         pip install -e . --no-deps
         ```
         
         There are different environment files that only install tensorflow or pytorch as dependencies available.
         
-        ## Command Line
+        ## 💻 Command Line
         
-        `bioimageio.core` installs a command line interface for testing models and other functionality. You can list all the available commands via:
-        ```
+        `bioimageio.core` installs a command line interface (CLI) for testing models and other functionality.
+        You can list all the available commands via:
+        
+        ```console
         bioimageio
         ```
         
         Check that a model adheres to the model spec:
-        ```
+        
+        ```console
         bioimageio validate <MODEL>
         ```
         
         Test a model (including prediction for the test input):
-        ```
+        
+        ```console
         bioimageio test-model <MODEL>
         ```
         
         Run prediction for an image stored on disc:
-        ```
-        bioimageio predict-image -m <MODEL> -i <INPUT> -o <OUTPUT>
+        
+        ```console
+        bioimageio predict-image <MODEL> --inputs <INPUT> --outputs <OUTPUT>
         ```
         
         Run prediction for multiple images stored on disc:
-        ```
+        
+        ```console
         bioimagei predict-images -m <MODEL> -i <INPUT_PATTERN> - o <OUTPUT_FOLDER>
         ```
-        `<INPUT_PATTERN>` is a `glob` pattern to select the desired images, e.g. `/path/to/my/images/*.tif`.
         
+        `<INPUT_PATTERN>` is a `glob` pattern to select the desired images, e.g. `/path/to/my/images/*.tif`.
         
         ## From python
         
         `bioimageio.core` is a python library that implements loading models, running prediction with them and more.
         To get an overview of this functionality, check out the example notebooks:
-        - [example/model_usage](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/model_usage.ipynb) for how to load models and run prediction with them
-        - [example/model_creation](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/model_creation.ipynb) for how to create bioimage.io compatible model packages
-        - [example/dataset_statistics_demo](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/dataset_statistics_demo.ipynb) for how to use the dataset statistics for advanced pre-and-postprocessing
+        
+        * [example/model_usage](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/model_usage.ipynb) for how to load models and run prediction with them
+        * [example/model_creation](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/model_creation.ipynb) for how to create bioimage.io compatible model packages
+        * [example/dataset_statistics_demo](https://github.com/bioimage-io/core-bioimage-io-python/blob/main/example/dataset_statistics_demo.ipynb) for how to use the dataset statistics for advanced pre-and-postprocessing
         
         ## Model Specification
         
-        The model specification and its validation tools can be found at https://github.com/bioimage-io/spec-bioimage-io.
+        The model specification and its validation tools can be found at <https://github.com/bioimage-io/spec-bioimage-io>.
+        
+        ## Changelog
+        
+        ### 0.5.10
+        
+        * [Fix critical bug in predict with tiling](https://github.com/bioimage-io/core-bioimage-io-python/pull/359)
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: dev
 Provides-Extra: pytorch
 Provides-Extra: tensorflow
 Provides-Extra: onnx
+Provides-Extra: dev
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bioimageio.core-0.5.9/setup.py` & `bioimageio.core-0.6.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,45 +6,68 @@
 # Get the long description from the README file
 ROOT_DIR = Path(__file__).parent.resolve()
 long_description = (ROOT_DIR / "README.md").read_text(encoding="utf-8")
 VERSION_FILE = ROOT_DIR / "bioimageio" / "core" / "VERSION"
 VERSION = json.loads(VERSION_FILE.read_text())["version"]
 
 
-setup(
+_ = setup(
     name="bioimageio.core",
     version=VERSION,
     description="Python functionality for the bioimage model zoo",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bioimage-io/core-bioimage-io-python",
     author="Bioimage Team",
-    classifiers=[  # Optional
+    classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
-    packages=find_namespace_packages(exclude=["tests"]),  # Required
+    packages=find_namespace_packages(exclude=["tests"]),
     install_requires=[
-        "bioimageio.spec==0.4.9.*",
+        "bioimageio.spec==0.5.2.*",
+        "fire",
         "imageio>=2.5",
+        "loguru",
         "numpy",
-        "ruamel.yaml",
+        "pydantic-settings",
+        "pydantic",
+        "python-dotenv",
+        "ruyaml",
         "tqdm",
+        "typing-extensions",
         "xarray",
-        "tifffile",
     ],
     include_package_data=True,
     extras_require={
-        "test": ["pytest", "black", "mypy"],
-        "dev": ["pre-commit"],
-        "pytorch": ["torch>=1.6", "torchvision"],
-        "tensorflow": ["tensorflow"],
+        "pytorch": ["torch>=1.6", "torchvision", "keras>=3.0"],
+        "tensorflow": ["tensorflow", "keras>=2.15"],
         "onnx": ["onnxruntime"],
+        "dev": [
+            "black",
+            # "crick",  # currently requires python<=3.9
+            "filelock",
+            "jupyter",
+            "jupyter-black",
+            "keras>=3.0",
+            "onnxruntime",
+            "packaging>=17.0",
+            "pre-commit",
+            "psutil",  # parallel pytest with 'pytest -n auto'
+            "pyright",
+            "pytest-xdist",  # parallel pytest
+            "pytest",
+            "torch>=1.6",
+            "torchvision",
+        ],
     },
-    project_urls={  # Optional
+    project_urls={
         "Bug Reports": "https://github.com/bioimage-io/core-bioimage-io-python/issues",
         "Source": "https://github.com/bioimage-io/core-bioimage-io-python",
     },
-    entry_points={"console_scripts": ["bioimageio = bioimageio.core.__main__:app"]},
+    entry_points={"console_scripts": ["bioimageio = bioimageio.core.__main__:main"]},
 )
```

### Comparing `bioimageio.core-0.5.9/tests/build_spec/test_add_weights.py` & `bioimageio.core-0.6.0/tests/weight_converter/test_add_weights.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,48 @@
-import os
-from bioimageio.core import export_resource_package, load_raw_resource_description, load_resource_description
-from bioimageio.core.resource_tests import test_model as _test_model
+# TODO: update add weights tests
+# import os
 
 
-def _test_add_weights(model, tmp_path, base_weights, added_weights, **kwargs):
-    from bioimageio.core.build_spec import add_weights
+# def _test_add_weights(model, tmp_path, base_weights, added_weights, **kwargs):
+#     from bioimageio.core.build_spec import add_weights
 
-    rdf = load_raw_resource_description(model)
-    assert base_weights in rdf.weights
-    assert added_weights in rdf.weights
+#     rdf = load_raw_resource_description(model)
+#     assert base_weights in rdf.weights
+#     assert added_weights in rdf.weights
 
-    weight_path = load_resource_description(model).weights[added_weights].source
-    assert weight_path.exists()
+#     weight_path = load_description(model).weights[added_weights].source
+#     assert weight_path.exists()
 
-    drop_weights = set(rdf.weights.keys()) - {base_weights}
-    for drop in drop_weights:
-        rdf.weights.pop(drop)
-    assert tuple(rdf.weights.keys()) == (base_weights,)
+#     drop_weights = set(rdf.weights.keys()) - {base_weights}
+#     for drop in drop_weights:
+#         rdf.weights.pop(drop)
+#     assert tuple(rdf.weights.keys()) == (base_weights,)
 
-    in_path = tmp_path / "model1.zip"
-    export_resource_package(rdf, output_path=in_path)
+#     in_path = tmp_path / "model1.zip"
+#     export_resource_package(rdf, output_path=in_path)
 
-    out_path = tmp_path / "model2.zip"
-    add_weights(in_path, weight_path, weight_type=added_weights, output_path=out_path, **kwargs)
+#     out_path = tmp_path / "model2.zip"
+#     add_weights(in_path, weight_path, weight_type=added_weights, output_path=out_path, **kwargs)
 
-    assert out_path.exists()
-    new_rdf = load_resource_description(out_path)
-    assert set(new_rdf.weights.keys()) == {base_weights, added_weights}
-    for weight in new_rdf.weights.values():
-        assert weight.source.exists()
+#     assert out_path.exists()
+#     new_rdf = load_description(out_path)
+#     assert set(new_rdf.weights.keys()) == {base_weights, added_weights}
+#     for weight in new_rdf.weights.values():
+#         assert weight.source.exists()
 
-    test_res = _test_model(out_path, added_weights)
-    failed = [s for s in test_res if s["status"] != "passed"]
-    assert not failed, failed
-    test_res = _test_model(out_path)
-    failed = [s for s in test_res if s["status"] != "passed"]
-    assert not failed, failed
+#     test_res = _test_model(out_path, added_weights)
+#     failed = [s for s in test_res if s["status"] != "passed"]
+#     assert not failed, failed
+#     test_res = _test_model(out_path)
+#     failed = [s for s in test_res if s["status"] != "passed"]
+#     assert not failed, failed
 
-    # make sure the weights were cleaned from the cwd
-    assert not os.path.exists(os.path.split(weight_path)[1])
+#     # make sure the weights were cleaned from the cwd
+#     assert not os.path.exists(os.path.split(weight_path)[1])
 
 
-def test_add_torchscript(unet2d_nuclei_broad_model, tmp_path):
-    _test_add_weights(unet2d_nuclei_broad_model, tmp_path, "pytorch_state_dict", "torchscript")
+# def test_add_torchscript(unet2d_nuclei_broad_model, tmp_path):
+#     _test_add_weights(unet2d_nuclei_broad_model, tmp_path, "pytorch_state_dict", "torchscript")
 
 
-def test_add_onnx(unet2d_nuclei_broad_model, tmp_path):
-    _test_add_weights(unet2d_nuclei_broad_model, tmp_path, "pytorch_state_dict", "onnx", opset_version=12)
+# def test_add_onnx(unet2d_nuclei_broad_model, tmp_path):
+#     _test_add_weights(unet2d_nuclei_broad_model, tmp_path, "pytorch_state_dict", "onnx", opset_version=12)
```

### Comparing `bioimageio.core-0.5.9/tests/prediction_pipeline/test_device_management.py` & `bioimageio.core-0.6.0/tests/test_prediction_pipeline_device_management.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,79 +1,87 @@
-import numpy as np
-import pytest
-import xarray as xr
+from pathlib import Path
+
 from numpy.testing import assert_array_almost_equal
 
-from bioimageio.core import load_resource_description
-from bioimageio.core.resource_io.nodes import Model
-from bioimageio.core.utils import skip_on
+from bioimageio.core.utils.testing import skip_on
+from bioimageio.spec.model.v0_4 import ModelDescr as ModelDescr04
+from bioimageio.spec.model.v0_5 import ModelDescr, WeightsFormat
 
 
 class TooFewDevicesException(Exception):
     pass
 
 
-def _test_device_management(model_package, weight_format):
+def _test_device_management(model_package: Path, weight_format: WeightsFormat):
     import torch
 
-    if torch.cuda.device_count() == 0:
+    from bioimageio.core import load_description
+    from bioimageio.core._prediction_pipeline import create_prediction_pipeline
+    from bioimageio.core.digest_spec import get_test_inputs, get_test_outputs
+
+    if not hasattr(torch, "cuda") or torch.cuda.device_count() == 0:
         raise TooFewDevicesException("Need at least one cuda device for this test")
 
-    from bioimageio.core.prediction_pipeline import create_prediction_pipeline
+    bio_model = load_description(model_package)
+    assert isinstance(bio_model, (ModelDescr, ModelDescr04))
+    pred_pipe = create_prediction_pipeline(
+        bioimageio_model=bio_model, weight_format=weight_format, devices=["cuda:0"]
+    )
 
-    bio_model = load_resource_description(model_package)
-    assert isinstance(bio_model, Model)
-    pred_pipe = create_prediction_pipeline(bioimageio_model=bio_model, weight_format=weight_format, devices=["cuda:0"])
-
-    inputs = [
-        xr.DataArray(np.load(str(test_tensor)), dims=tuple(spec.axes))
-        for test_tensor, spec in zip(bio_model.test_inputs, bio_model.inputs)
-    ]
+    inputs = get_test_inputs(bio_model)
     with pred_pipe as pp:
-        outputs = pp.forward(*inputs)
-
-    assert isinstance(outputs, list)
+        outputs = pp.predict_sample_without_blocking(inputs)
 
-    expected_outputs = [
-        xr.DataArray(np.load(str(test_tensor)), dims=tuple(spec.axes))
-        for test_tensor, spec in zip(bio_model.test_outputs, bio_model.outputs)
-    ]
+    expected_outputs = get_test_outputs(bio_model)
 
-    assert len(outputs) == len(expected_outputs)
-    for out, exp in zip(outputs, expected_outputs):
+    assert len(outputs.shape) == len(expected_outputs.shape)
+    for m in expected_outputs.members:
+        out = outputs.members[m].data
+        assert out is not None
+        exp = expected_outputs.members[m].data
         assert_array_almost_equal(out, exp, decimal=4)
 
-    # repeat inference with context manager to test load/unload/load/forward
+    # repeat inference with context manager to test load/predict/unload/load/predict
     with pred_pipe as pp:
-        outputs = pp.forward(*inputs)
+        outputs = pp.predict_sample_without_blocking(inputs)
 
-    assert len(outputs) == len(expected_outputs)
-    for out, exp in zip(outputs, expected_outputs):
+    assert len(outputs.shape) == len(expected_outputs.shape)
+    for m in expected_outputs.members:
+        out = outputs.members[m].data
+        assert out is not None
+        exp = expected_outputs.members[m].data
         assert_array_almost_equal(out, exp, decimal=4)
 
 
-@skip_on(TooFewDevicesException, reason="Too few devices")
-def test_device_management_torch(any_torch_model):
+@skip_on(
+    TooFewDevicesException, reason="Too few devices"
+)  # pyright: ignore[reportArgumentType]
+def test_device_management_torch(any_torch_model: Path):
     _test_device_management(any_torch_model, "pytorch_state_dict")
 
 
-@skip_on(TooFewDevicesException, reason="Too few devices")
-def test_device_management_torchscript(any_torchscript_model):
+@skip_on(
+    TooFewDevicesException, reason="Too few devices"
+)  # pyright: ignore[reportArgumentType]
+def test_device_management_torchscript(any_torchscript_model: Path):
     _test_device_management(any_torchscript_model, "torchscript")
 
 
-@pytest.mark.skipif(pytest.skip_torch, reason="requires torch for device discovery")
-@skip_on(TooFewDevicesException, reason="Too few devices")
-def test_device_management_onnx(any_onnx_model):
+@skip_on(
+    TooFewDevicesException, reason="Too few devices"
+)  # pyright: ignore[reportArgumentType]
+def test_device_management_onnx(any_onnx_model: Path):
     _test_device_management(any_onnx_model, "onnx")
 
 
-@pytest.mark.skipif(pytest.skip_torch, reason="requires torch for device discovery")
-@skip_on(TooFewDevicesException, reason="Too few devices")
-def test_device_management_tensorflow(any_tensorflow_model):
+@skip_on(
+    TooFewDevicesException, reason="Too few devices"
+)  # pyright: ignore[reportArgumentType]
+def test_device_management_tensorflow(any_tensorflow_model: Path):
     _test_device_management(any_tensorflow_model, "tensorflow_saved_model_bundle")
 
 
-@pytest.mark.skipif(pytest.skip_torch, reason="requires torch for device discovery")
-@skip_on(TooFewDevicesException, reason="Too few devices")
-def test_device_management_keras(any_keras_model):
+@skip_on(
+    TooFewDevicesException, reason="Too few devices"
+)  # pyright: ignore[reportArgumentType]
+def test_device_management_keras(any_keras_model: Path):
     _test_device_management(any_keras_model, "keras_hdf5")
```

### Comparing `bioimageio.core-0.5.9/tests/prediction_pipeline/test_prediction_pipeline.py` & `bioimageio.core-0.6.0/tests/test_prediction_pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,51 @@
-import numpy as np
-import xarray as xr
-from numpy.testing import assert_array_almost_equal
-
-from bioimageio.core import load_resource_description
-from bioimageio.core.resource_io.nodes import Model
-
+from pathlib import Path
 
-def _test_prediction_pipeline(model_package, weight_format):
-    from bioimageio.core.prediction_pipeline import create_prediction_pipeline
-
-    bio_model = load_resource_description(model_package)
-    assert isinstance(bio_model, Model)
-    pp = create_prediction_pipeline(bioimageio_model=bio_model, weight_format=weight_format)
-
-    inputs = [
-        xr.DataArray(np.load(str(test_tensor)), dims=tuple(spec.axes))
-        for test_tensor, spec in zip(bio_model.test_inputs, bio_model.inputs)
-    ]
-    outputs = pp.forward(*inputs)
-    assert isinstance(outputs, list)
-
-    expected_outputs = [
-        xr.DataArray(np.load(str(test_tensor)), dims=tuple(spec.axes))
-        for test_tensor, spec in zip(bio_model.test_outputs, bio_model.outputs)
-    ]
-    assert len(outputs) == len(expected_outputs)
+from numpy.testing import assert_array_almost_equal
 
-    for out, exp in zip(outputs, expected_outputs):
+from bioimageio.spec import load_description
+from bioimageio.spec.model.v0_4 import ModelDescr as ModelDescr04
+from bioimageio.spec.model.v0_5 import ModelDescr, WeightsFormat
+
+
+def _test_prediction_pipeline(model_package: Path, weights_format: WeightsFormat):
+    from bioimageio.core._prediction_pipeline import create_prediction_pipeline
+    from bioimageio.core.digest_spec import get_test_inputs, get_test_outputs
+
+    bio_model = load_description(model_package)
+    assert isinstance(
+        bio_model, (ModelDescr, ModelDescr04)
+    ), bio_model.validation_summary.format()
+    pp = create_prediction_pipeline(
+        bioimageio_model=bio_model, weight_format=weights_format
+    )
+
+    inputs = get_test_inputs(bio_model)
+    outputs = pp.predict_sample_without_blocking(inputs)
+
+    expected_outputs = get_test_outputs(bio_model)
+    assert len(outputs.shape) == len(expected_outputs.shape)
+    for m in expected_outputs.members:
+        out = outputs.members[m].data
+        assert out is not None
+        exp = expected_outputs.members[m].data
         assert_array_almost_equal(out, exp, decimal=4)
 
 
-def test_prediction_pipeline_torch(any_torch_model):
+def test_prediction_pipeline_torch(any_torch_model: Path):
     _test_prediction_pipeline(any_torch_model, "pytorch_state_dict")
 
 
-def test_prediction_pipeline_torchscript(any_torchscript_model):
+def test_prediction_pipeline_torchscript(any_torchscript_model: Path):
     _test_prediction_pipeline(any_torchscript_model, "torchscript")
 
 
-def test_prediction_pipeline_onnx(any_onnx_model):
+def test_prediction_pipeline_onnx(any_onnx_model: Path):
     _test_prediction_pipeline(any_onnx_model, "onnx")
 
 
-def test_prediction_pipeline_tensorflow(any_tensorflow_model):
+def test_prediction_pipeline_tensorflow(any_tensorflow_model: Path):
     _test_prediction_pipeline(any_tensorflow_model, "tensorflow_saved_model_bundle")
 
 
-def test_prediction_pipeline_keras(any_keras_model):
+def test_prediction_pipeline_keras(any_keras_model: Path):
     _test_prediction_pipeline(any_keras_model, "keras_hdf5")
```

### Comparing `bioimageio.core-0.5.9/tests/test_cli.py` & `bioimageio.core-0.6.0/tests/test_cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,141 +1,137 @@
-import os
 import subprocess
-from typing import Sequence
+from typing import Any, List, Sequence
 
-import numpy as np
 import pytest
+from pydantic import FilePath
 
-from bioimageio.core import load_resource_description
 
-
-def run_subprocess(commands: Sequence[str], **kwargs) -> subprocess.CompletedProcess:
-    return subprocess.run(commands, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, encoding="utf-8", **kwargs)
-
-
-def test_validate_model(unet2d_nuclei_broad_model):
-    ret = run_subprocess(["bioimageio", "validate", unet2d_nuclei_broad_model])
-    assert ret.returncode == 0, ret.stdout
-
-
-def test_cli_package(unet2d_nuclei_broad_model, tmp_path):
-    out_path = tmp_path / "model.zip"
-    ret = run_subprocess(["bioimageio", "package", unet2d_nuclei_broad_model, str(out_path)])
-    assert ret.returncode == 0, ret.stdout
-    assert out_path.exists()
-
-
-def test_cli_package_wo_cache(unet2d_nuclei_broad_model):
-    env = os.environ.copy()
-    env["BIOIMAGEIO_USE_CACHE"] = "false"
-    ret = run_subprocess(["bioimageio", "package", unet2d_nuclei_broad_model], env=env)
-    assert ret.returncode == 0, ret.stdout
-
-
-def test_cli_test_model(unet2d_nuclei_broad_model):
-    ret = run_subprocess(["bioimageio", "test-model", unet2d_nuclei_broad_model])
-    assert ret.returncode == 0, ret.stdout
-
-
-def test_cli_test_model_fail(stardist_wrong_shape):
-    ret = run_subprocess(["bioimageio", "test-model", stardist_wrong_shape])
-    assert ret.returncode == 1
-
-
-def test_cli_test_model_with_weight_format(unet2d_nuclei_broad_model):
-    ret = run_subprocess(
-        ["bioimageio", "test-model", unet2d_nuclei_broad_model, "--weight-format", "pytorch_state_dict"]
+def run_subprocess(
+    commands: Sequence[str], **kwargs: Any
+) -> "subprocess.CompletedProcess[str]":
+    return subprocess.run(
+        commands,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.STDOUT,
+        encoding="utf-8",
+        **kwargs,
     )
-    assert ret.returncode == 0, ret.stdout
-
 
-def test_cli_test_resource(unet2d_nuclei_broad_model):
-    ret = run_subprocess(["bioimageio", "test-resource", unet2d_nuclei_broad_model])
-    assert ret.returncode == 0, ret.stdout
 
-
-def test_cli_test_resource_with_weight_format(unet2d_nuclei_broad_model):
-    ret = run_subprocess(
-        ["bioimageio", "test-resource", unet2d_nuclei_broad_model, "--weight-format", "pytorch_state_dict"]
-    )
-    assert ret.returncode == 0, ret.stdout
-
-
-def _test_cli_predict_image(model, tmp_path, extra_kwargs=None):
-    spec = load_resource_description(model)
-    in_path = spec.test_inputs[0]
-    out_path = tmp_path.with_suffix(".npy")
-    cmd = ["bioimageio", "predict-image", model, "--inputs", str(in_path), "--outputs", str(out_path)]
-    if extra_kwargs is not None:
-        cmd.extend(extra_kwargs)
-    ret = run_subprocess(cmd)
-    assert ret.returncode == 0, ret.stdout
-    assert out_path.exists()
-
-
-def test_cli_predict_image(unet2d_nuclei_broad_model, tmp_path):
-    _test_cli_predict_image(unet2d_nuclei_broad_model, tmp_path)
-
-
-def test_cli_predict_image_with_weight_format(unet2d_nuclei_broad_model, tmp_path):
-    _test_cli_predict_image(unet2d_nuclei_broad_model, tmp_path, ["--weight-format", "pytorch_state_dict"])
-
-
-def _test_cli_predict_images(model, tmp_path, extra_kwargs=None):
-    n_images = 3
-    shape = (1, 1, 128, 128)
-    expected_shape = (1, 1, 128, 128)
-
-    in_folder = tmp_path / "inputs"
-    in_folder.mkdir()
-    out_folder = tmp_path / "outputs"
-    out_folder.mkdir()
-
-    expected_outputs = []
-    for i in range(n_images):
-        path = in_folder / f"im-{i}.npy"
-        im = np.random.randint(0, 255, size=shape).astype("uint8")
-        np.save(path, im)
-        expected_outputs.append(out_folder / f"im-{i}.npy")
-
-    input_pattern = str(in_folder / "*.npy")
-    cmd = ["bioimageio", "predict-images", model, input_pattern, str(out_folder)]
-    if extra_kwargs is not None:
-        cmd.extend(extra_kwargs)
-    ret = run_subprocess(cmd)
-    assert ret.returncode == 0, ret.stdout
-
-    for out_path in expected_outputs:
-        assert out_path.exists()
-        assert np.load(out_path).shape == expected_shape
-
-
-def test_cli_predict_images(unet2d_nuclei_broad_model, tmp_path):
-    _test_cli_predict_images(unet2d_nuclei_broad_model, tmp_path)
-
-
-def test_cli_predict_images_with_weight_format(unet2d_nuclei_broad_model, tmp_path):
-    _test_cli_predict_images(unet2d_nuclei_broad_model, tmp_path, ["--weight-format", "pytorch_state_dict"])
-
-
-def test_torch_to_torchscript(unet2d_nuclei_broad_model, tmp_path):
-    out_path = tmp_path.with_suffix(".pt")
-    ret = run_subprocess(
-        ["bioimageio", "convert-torch-weights-to-torchscript", str(unet2d_nuclei_broad_model), str(out_path)]
-    )
-    assert ret.returncode == 0, ret.stdout
-    assert out_path.exists()
-
-
-@pytest.mark.skipif(pytest.skip_onnx, reason="requires torch and onnx")
-def test_torch_to_onnx(unet2d_nuclei_broad_model, tmp_path):
-    out_path = tmp_path.with_suffix(".onnx")
-    ret = run_subprocess(["bioimageio", "convert-torch-weights-to-onnx", str(unet2d_nuclei_broad_model), str(out_path)])
-    assert ret.returncode == 0, ret.stdout
-    assert out_path.exists()
-
-
-def test_keras_to_tf(unet2d_keras, tmp_path):
-    out_path = tmp_path / "weights.zip"
-    ret = run_subprocess(["bioimageio", "convert-keras-weights-to-tensorflow", str(unet2d_keras), str(out_path)])
-    assert ret.returncode == 0, ret.stdout
-    assert out_path.exists()
+@pytest.mark.parametrize(
+    "args",
+    [
+        [
+            "package",
+            "unet2d_nuclei_broad_model",
+            "--weight-format",
+            "pytorch_state_dict",
+        ],
+        ["package", "unet2d_nuclei_broad_model"],
+        [
+            "test",
+            "unet2d_nuclei_broad_model",
+            "--weight-format",
+            "pytorch_state_dict",
+        ],
+        ["test", "unet2d_nuclei_broad_model"],
+    ],
+)
+def test_cli(args: List[str], unet2d_nuclei_broad_model: str):
+    resolved_args = [
+        str(unet2d_nuclei_broad_model) if arg == "unet2d_nuclei_broad_model" else arg
+        for arg in args
+    ]
+    ret = run_subprocess(["bioimageio", *resolved_args])
+    assert ret.returncode == 0, ret.stdout
+
+
+@pytest.mark.parametrize("args", [["test", "stardist_wrong_shape"]])
+def test_cli_fails(args: List[str], stardist_wrong_shape: FilePath):
+    resolved_args = [
+        str(stardist_wrong_shape) if arg == "stardist_wrong_shape" else arg
+        for arg in args
+    ]
+    ret = run_subprocess(["bioimageio", *resolved_args])
+    assert ret.returncode == 1, ret.stdout
+
+
+# TODO: update CLI test
+# def _test_cli_predict_image(model: Path, tmp_path: Path, extra_cmd_args: Optional[List[str]] = None):
+#     spec = load_description(model)
+#     in_path = spec.test_inputs[0]
+
+#     out_path = tmp_path.with_suffix(".npy")
+#     cmd = ["bioimageio", "predict-image", model, "--input", str(in_path), "--output", str(out_path)]
+#     if extra_cmd_args is not None:
+#         cmd.extend(extra_cmd_args)
+#     ret = run_subprocess(cmd)
+#     assert ret.returncode == 0, ret.stdout
+#     assert out_path.exists()
+
+
+# def test_cli_predict_image(unet2d_nuclei_broad_model: Path, tmp_path: Path):
+#     _test_cli_predict_image(unet2d_nuclei_broad_model, tmp_path)
+
+
+# def test_cli_predict_image_with_weight_format(unet2d_nuclei_broad_model: Path, tmp_path: Path):
+#     _test_cli_predict_image(unet2d_nuclei_broad_model, tmp_path, ["--weight-format", "pytorch_state_dict"])
+
+
+# def _test_cli_predict_images(model: Path, tmp_path: Path, extra_cmd_args: Optional[List[str]] = None):
+#     n_images = 3
+#     shape = (1, 1, 128, 128)
+#     expected_shape = (1, 1, 128, 128)
+
+#     in_folder = tmp_path / "inputs"
+#     in_folder.mkdir()
+#     out_folder = tmp_path / "outputs"
+#     out_folder.mkdir()
+
+#     expected_outputs: List[Path] = []
+#     for i in range(n_images):
+#         path = in_folder / f"im-{i}.npy"
+#         im = np.random.randint(0, 255, size=shape).astype("uint8")
+#         np.save(path, im)
+#         expected_outputs.append(out_folder / f"im-{i}.npy")
+
+#     input_pattern = str(in_folder / "*.npy")
+#     cmd = ["bioimageio", "predict-images", str(model), input_pattern, str(out_folder)]
+#     if extra_cmd_args is not None:
+#         cmd.extend(extra_cmd_args)
+#     ret = run_subprocess(cmd)
+#     assert ret.returncode == 0, ret.stdout
+
+#     for out_path in expected_outputs:
+#         assert out_path.exists()
+#         assert np.load(out_path).shape == expected_shape
+
+
+# def test_cli_predict_images(unet2d_nuclei_broad_model: Path, tmp_path: Path):
+#     _test_cli_predict_images(unet2d_nuclei_broad_model, tmp_path)
+
+
+# def test_cli_predict_images_with_weight_format(unet2d_nuclei_broad_model: Path, tmp_path: Path):
+#     _test_cli_predict_images(unet2d_nuclei_broad_model, tmp_path, ["--weight-format", "pytorch_state_dict"])
+
+
+# def test_torch_to_torchscript(unet2d_nuclei_broad_model: Path, tmp_path: Path):
+#     out_path = tmp_path.with_suffix(".pt")
+#     ret = run_subprocess(
+#         ["bioimageio", "convert-torch-weights-to-torchscript", str(unet2d_nuclei_broad_model), str(out_path)]
+#     )
+#     assert ret.returncode == 0, ret.stdout
+#     assert out_path.exists()
+
+
+# def test_torch_to_onnx(convert_to_onnx: Path, tmp_path: Path):
+#     out_path = tmp_path.with_suffix(".onnx")
+#     ret = run_subprocess(["bioimageio", "convert-torch-weights-to-onnx", str(convert_to_onnx), str(out_path)])
+#     assert ret.returncode == 0, ret.stdout
+#     assert out_path.exists()
+
+
+# def test_keras_to_tf(unet2d_keras: Path, tmp_path: Path):
+#     out_path = tmp_path / "weights.zip"
+#     ret = run_subprocess(["bioimageio", "convert-keras-weights-to-tensorflow", str(unet2d_keras), str(out_path)])
+#     assert ret.returncode == 0, ret.stdout
+#     assert out_path.exists()
```

### Comparing `bioimageio.core-0.5.9/tests/test_prediction.py` & `bioimageio.core-0.6.0/tests/test_prediction.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,210 +1,228 @@
-from pathlib import Path
+# TODO: update
+# from pathlib import Path
 
-import imageio
-import numpy as np
-from numpy.testing import assert_array_almost_equal
-
-from bioimageio.core import load_resource_description
-from bioimageio.core.resource_io.nodes import Model
-
-
-def test_predict_image(any_model, tmpdir):
-    from bioimageio.core.prediction import predict_image
-
-    spec = load_resource_description(any_model)
-    assert isinstance(spec, Model)
-    inputs = spec.test_inputs
-
-    outputs = [Path(tmpdir) / f"out{i}.npy" for i in range(len(spec.test_outputs))]
-    predict_image(any_model, inputs, outputs)
-    for out_path in outputs:
-        assert out_path.exists()
-
-    result = [np.load(str(p)) for p in outputs]
-    expected = [np.load(str(p)) for p in spec.test_outputs]
-    for res, exp in zip(result, expected):
-        assert_array_almost_equal(res, exp, decimal=4)
-
-
-def test_predict_image_with_weight_format(unet2d_fixed_shape_or_not, tmpdir):
-    from bioimageio.core.prediction import predict_image
-
-    spec = load_resource_description(unet2d_fixed_shape_or_not)
-    assert isinstance(spec, Model)
-    inputs = spec.test_inputs
-
-    outputs = [Path(tmpdir) / f"out{i}.npy" for i in range(len(spec.test_outputs))]
-    predict_image(unet2d_fixed_shape_or_not, inputs, outputs, weight_format="pytorch_state_dict")
-    for out_path in outputs:
-        assert out_path.exists()
-
-    result = [np.load(str(p)) for p in outputs]
-    expected = [np.load(str(p)) for p in spec.test_outputs]
-    for res, exp in zip(result, expected):
-        assert_array_almost_equal(res, exp, decimal=4)
-
-
-def _test_predict_with_padding(model, tmp_path):
-    from bioimageio.core.prediction import predict_image
-
-    spec = load_resource_description(model)
-    assert isinstance(spec, Model)
-
-    input_spec, output_spec = spec.inputs[0], spec.outputs[0]
-    channel_axis = input_spec.axes.index("c")
-    channel_first = channel_axis == 1
-
-    image = np.load(str(spec.test_inputs[0]))
-    assert image.shape[channel_axis] == 1
-    if channel_first:
-        image = image[0, 0]
-    else:
-        image = image[0, ..., 0]
-    original_shape = image.shape
-    assert image.ndim == 2
-
-    if isinstance(output_spec.shape, list):
-        n_channels = output_spec.shape[channel_axis]
-    else:
-        scale = output_spec.shape.scale[channel_axis]
-        offset = output_spec.shape.offset[channel_axis]
-        in_channels = 1
-        n_channels = int(2 * offset + scale * in_channels)
-
-    # write the padded image
-    image = image[3:-2, 1:-12]
-    in_path = tmp_path / "in.tif"
-    out_path = tmp_path / "out.tif"
-    imageio.imwrite(in_path, image)
-
-    if hasattr(output_spec.shape, "scale"):
-        scale = dict(zip(output_spec.axes, output_spec.shape.scale))
-        offset = dict(zip(output_spec.axes, output_spec.shape.offset))
-        spatial_axes = [ax for ax in output_spec.axes if ax in "xyz"]
-        network_resizes = any(sc != 1 for ax, sc in scale.items() if ax in spatial_axes) or any(
-            off != 0 for ax, off in offset.items() if ax in spatial_axes
-        )
-    else:
-        network_resizes = False
-
-    if network_resizes:
-        exp_shape = tuple(int(sh * scale[ax] + 2 * offset[ax]) for sh, ax in zip(image.shape, spatial_axes))
-    else:
-        exp_shape = image.shape
-
-    def check_result():
-        if n_channels == 1:
-            assert out_path.exists()
-            res = imageio.imread(out_path)
-            assert res.shape == exp_shape
-        else:
-            path = str(out_path)
-            for c in range(n_channels):
-                channel_out_path = Path(path.replace(".tif", f"-c{c}.tif"))
-                assert channel_out_path.exists()
-                res = imageio.imread(channel_out_path)
-                assert res.shape == exp_shape
-
-    # test with dynamic padding
-    predict_image(model, in_path, out_path, padding={"x": 16, "y": 16, "mode": "dynamic"})
-    check_result()
-
-    # test with fixed padding
-    predict_image(
-        model, in_path, out_path, padding={"x": original_shape[0], "y": original_shape[1], "mode": "fixed"}
-    )
-    check_result()
-
-    # test with automated padding
-    predict_image(model, in_path, out_path, padding=True)
-    check_result()
-
-
-# prediction with padding with the parameters above may not be suited for any model
-# so we only run it for the pytorch unet2d here
-def test_predict_image_with_padding(unet2d_fixed_shape_or_not, tmp_path):
-    _test_predict_with_padding(unet2d_fixed_shape_or_not, tmp_path)
-
-
-# and with different output shape
-def test_predict_image_with_padding_diff_output_shape(unet2d_diff_output_shape, tmp_path):
-    _test_predict_with_padding(unet2d_diff_output_shape, tmp_path)
-
-
-def test_predict_image_with_padding_channel_last(stardist, tmp_path):
-    _test_predict_with_padding(stardist, tmp_path)
-
-
-def _test_predict_image_with_tiling(model, tmp_path, exp_mean_deviation):
-    from bioimageio.core.prediction import predict_image
-
-    spec = load_resource_description(model)
-    assert isinstance(spec, Model)
-    inputs = spec.test_inputs
-    assert len(inputs) == 1
-    exp = np.load(str(spec.test_outputs[0]))
-
-    out_path = tmp_path.with_suffix(".npy")
-
-    def check_result():
-        assert out_path.exists()
-        res = np.load(out_path)
-        assert res.shape == exp.shape
-        # check that the mean deviation is smaller than the expected value
-        # note that we can't use array_almost_equal here, because the numerical differences
-        # between tiled and normal prediction are too large
-        mean_deviation = np.abs(res - exp).mean()
-        assert mean_deviation <= exp_mean_deviation
-
-    # with tiling config
-    tiling = {"halo": {"x": 32, "y": 32}, "tile": {"x": 256, "y": 256}}
-    predict_image(model, inputs, [out_path], tiling=tiling)
-    check_result()
-
-    # with tiling determined from spec
-    predict_image(model, inputs, [out_path], tiling=True)
-    check_result()
-
-
-# prediction with tiling with the parameters above may not be suited for any model
-# so we only run it for the pytorch unet2d here
-def test_predict_image_with_tiling_1(unet2d_nuclei_broad_model, tmp_path):
-    _test_predict_image_with_tiling(unet2d_nuclei_broad_model, tmp_path, 0.012)
-
-
-def test_predict_image_with_tiling_2(unet2d_diff_output_shape, tmp_path):
-    _test_predict_image_with_tiling(unet2d_diff_output_shape, tmp_path, 0.012)
-
-
-def test_predict_image_with_tiling_3(shape_change_model, tmp_path):
-    _test_predict_image_with_tiling(shape_change_model, tmp_path, 0.012)
-
-
-def test_predict_image_with_tiling_channel_last(stardist, tmp_path):
-    _test_predict_image_with_tiling(stardist, tmp_path, 0.13)
-
-
-def test_predict_image_with_tiling_fixed_output_shape(unet2d_fixed_shape, tmp_path):
-    _test_predict_image_with_tiling(unet2d_fixed_shape, tmp_path, 0.025)
-
-
-def test_predict_images(unet2d_nuclei_broad_model, tmp_path):
-    from bioimageio.core.prediction import predict_images
-
-    n_images = 5
-    shape = (256, 256)
-
-    in_paths = []
-    out_paths = []
-    for i in range(n_images):
-        in_path = tmp_path / f"in{i}.tif"
-        im = np.random.randint(0, 255, size=shape).astype("uint8")
-        imageio.imwrite(in_path, im)
-        in_paths.append(in_path)
-        out_paths.append(tmp_path / f"out{i}.tif")
-    predict_images(unet2d_nuclei_broad_model, in_paths, out_paths)
-
-    for outp in out_paths:
-        assert outp.exists()
-        out = imageio.imread(outp)
-        assert out.shape == shape
+# import imageio
+# import numpy as np
+# from numpy.testing import assert_array_almost_equal
+
+# from bioimageio.spec import load_description
+# from bioimageio.spec.model.v0_4 import InputTensorDescr as InputTensorDescr_v0_4
+# from bioimageio.spec.model.v0_4 import ModelDescr as ModelDescr_v0_4
+# from bioimageio.spec.model.v0_5 import ModelDescr
+
+
+# def test_predict_image(any_model: Path, tmpdir: Path):
+#     from bioimageio.core.prediction import predict_image
+
+#     spec = load_description(any_model)
+#     assert isinstance(spec, ModelDescr)
+#     inputs = spec.test_inputs
+
+#     outputs = [Path(tmpdir) / f"out{i}.npy" for i in range(len(spec.test_outputs))]
+#     predict_image(any_model, inputs, outputs)
+#     for out_path in outputs:
+#         assert out_path.exists()
+
+#     result = [np.load(str(p)) for p in outputs]
+#     expected = [np.load(str(p)) for p in spec.test_outputs]
+#     for res, exp in zip(result, expected):
+#         assert_array_almost_equal(res, exp, decimal=4)
+
+
+# def test_predict_image_with_weight_format(
+#     unet2d_fixed_shape_or_not: Path, tmpdir: Path
+# ):
+#     from bioimageio.core.prediction import predict_image
+
+#     spec = load_description(unet2d_fixed_shape_or_not)
+#     assert isinstance(spec, Model)
+#     inputs = spec.test_inputs
+
+#     outputs = [Path(tmpdir) / f"out{i}.npy" for i in range(len(spec.test_outputs))]
+#     predict_image(
+#         unet2d_fixed_shape_or_not, inputs, outputs, weight_format="pytorch_state_dict"
+#     )
+#     for out_path in outputs:
+#         assert out_path.exists()
+
+#     result = [np.load(str(p)) for p in outputs]
+#     expected = [np.load(str(p)) for p in spec.test_outputs]
+#     for res, exp in zip(result, expected):
+#         assert_array_almost_equal(res, exp, decimal=4)
+
+
+# def _test_predict_with_padding(any_model: Path, tmp_path: Path):
+#     from bioimageio.core.digest_spec import get_test_inputs
+#     from bioimageio.core.prediction import predict_image
+
+#     model = load_description(any_model)
+#     assert isinstance(model, (ModelDescr_v0_4, ModelDescr))
+
+#     input_spec, output_spec = model.inputs[0], model.outputs[0]
+#     channel_axis = (
+#         "c"
+#         if isinstance(input_spec, InputTensorDescr_v0_4)
+#         else [a.id for a in input_spec.axes][0]
+#     )
+#     channel_first = channel_axis == 1
+
+#     # TODO: check more tensors
+#     image = get_test_inputs(model)[0]
+
+#     if isinstance(output_spec.shape, list):
+#         n_channels = output_spec.shape[channel_axis]
+#     else:
+#         scale = output_spec.shape.scale[channel_axis]
+#         offset = output_spec.shape.offset[channel_axis]
+#         in_channels = 1
+#         n_channels = int(2 * offset + scale * in_channels)
+
+#     # write the padded image
+#     image = image[3:-2, 1:-12]
+#     in_path = tmp_path / "in.tif"
+#     out_path = tmp_path / "out.tif"
+#     imageio.imwrite(in_path, image)
+
+#     if hasattr(output_spec.shape, "scale"):
+#         scale = dict(zip(output_spec.axes, output_spec.shape.scale))
+#         offset = dict(zip(output_spec.axes, output_spec.shape.offset))
+#         spatial_axes = [ax for ax in output_spec.axes if ax in "xyz"]
+#         network_resizes = any(
+#             sc != 1 for ax, sc in scale.items() if ax in spatial_axes
+#         ) or any(off != 0 for ax, off in offset.items() if ax in spatial_axes)
+#     else:
+#         network_resizes = False
+
+#     if network_resizes:
+#         exp_shape = tuple(
+#             int(sh * scale[ax] + 2 * offset[ax])
+#             for sh, ax in zip(image.shape, spatial_axes)
+#         )
+#     else:
+#         exp_shape = image.shape
+
+#     def check_result():
+#         if n_channels == 1:
+#             assert out_path.exists()
+#             res = imageio.imread(out_path)
+#             assert res.shape == exp_shape
+#         else:
+#             path = str(out_path)
+#             for c in range(n_channels):
+#                 channel_out_path = Path(path.replace(".tif", f"-c{c}.tif"))
+#                 assert channel_out_path.exists()
+#                 res = imageio.imread(channel_out_path)
+#                 assert res.shape == exp_shape
+
+#     # test with dynamic padding
+#     predict_image(
+#         any_model, in_path, out_path, padding={"x": 16, "y": 16, "mode": "dynamic"}
+#     )
+#     check_result()
+
+#     # test with fixed padding
+#     predict_image(
+#         any_model,
+#         in_path,
+#         out_path,
+#         padding={"x": original_shape[0], "y": original_shape[1], "mode": "fixed"},
+#     )
+#     check_result()
+
+#     # test with automated padding
+#     predict_image(any_model, in_path, out_path, padding=True)
+#     check_result()
+
+
+# # prediction with padding with the parameters above may not be suited for any model
+# # so we only run it for the pytorch unet2d here
+# def test_predict_image_with_padding(unet2d_fixed_shape_or_not, tmp_path):
+#     _test_predict_with_padding(unet2d_fixed_shape_or_not, tmp_path)
+
+
+# # and with different output shape
+# def test_predict_image_with_padding_diff_output_shape(
+#     unet2d_diff_output_shape, tmp_path
+# ):
+#     _test_predict_with_padding(unet2d_diff_output_shape, tmp_path)
+
+
+# def test_predict_image_with_padding_channel_last(stardist, tmp_path):
+#     _test_predict_with_padding(stardist, tmp_path)
+
+
+# def _test_predict_image_with_tiling(model: Path, tmp_path: Path, exp_mean_deviation):
+#     from bioimageio.core.prediction import predict_image
+
+#     spec = load_description(model)
+#     assert isinstance(spec, Model)
+#     inputs = spec.test_inputs
+#     assert len(inputs) == 1
+#     exp = np.load(str(spec.test_outputs[0]))
+
+#     out_path = tmp_path.with_suffix(".npy")
+
+#     def check_result():
+#         assert out_path.exists()
+#         res = np.load(out_path)
+#         assert res.shape == exp.shape
+#         # check that the mean deviation is smaller than the expected value
+#         # note that we can't use array_almost_equal here, because the numerical differences
+#         # between tiled and normal prediction are too large
+#         mean_deviation = np.abs(res - exp).mean()
+#         assert mean_deviation <= exp_mean_deviation
+
+#     # with tiling config
+#     tiling = {"halo": {"x": 32, "y": 32}, "tile": {"x": 256, "y": 256}}
+#     predict_image(model, inputs, [out_path], tiling=tiling)
+#     check_result()
+
+#     # with tiling determined from spec
+#     predict_image(model, inputs, [out_path], tiling=True)
+#     check_result()
+
+
+# # prediction with tiling with the parameters above may not be suited for any model
+# # so we only run it for the pytorch unet2d here
+# def test_predict_image_with_tiling_1(unet2d_nuclei_broad_model: Path, tmp_path: Path):
+#     _test_predict_image_with_tiling(unet2d_nuclei_broad_model, tmp_path, 0.012)
+
+
+# def test_predict_image_with_tiling_2(unet2d_diff_output_shape: Path, tmp_path: Path):
+#     _test_predict_image_with_tiling(unet2d_diff_output_shape, tmp_path, 0.06)
+
+
+# def test_predict_image_with_tiling_3(shape_change_model: Path, tmp_path: Path):
+#     _test_predict_image_with_tiling(shape_change_model, tmp_path, 0.012)
+
+
+# def test_predict_image_with_tiling_channel_last(stardist: Path, tmp_path: Path):
+#     _test_predict_image_with_tiling(stardist, tmp_path, 0.13)
+
+
+# def test_predict_image_with_tiling_fixed_output_shape(
+#     unet2d_fixed_shape: Path, tmp_path: Path
+# ):
+#     _test_predict_image_with_tiling(unet2d_fixed_shape, tmp_path, 0.025)
+
+
+# def test_predict_images(unet2d_nuclei_broad_model: Path, tmp_path: Path):
+#     from bioimageio.core.prediction import predict_images
+
+#     n_images = 5
+#     shape = (256, 256)
+
+#     in_paths = []
+#     out_paths = []
+#     for i in range(n_images):
+#         in_path = tmp_path / f"in{i}.tif"
+#         im = np.random.randint(0, 255, size=shape).astype("uint8")
+#         imageio.imwrite(in_path, im)
+#         in_paths.append(in_path)
+#         out_paths.append(tmp_path / f"out{i}.tif")
+#     predict_images(unet2d_nuclei_broad_model, in_paths, out_paths)
+
+#     for outp in out_paths:
+#         assert outp.exists()
+#         out = imageio.imread(outp)
+#         assert out.shape == shape
```

