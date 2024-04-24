# Comparing `tmp/cnn2snn-2.7.0.tar.gz` & `tmp/cnn2snn-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnn2snn-2.7.0.tar", last modified: Wed Feb  7 14:29:55 2024, max compression
+gzip compressed data, was "cnn2snn-2.7.2.tar", last modified: Wed Apr 24 15:30:28 2024, max compression
```

## Comparing `cnn2snn-2.7.0.tar` & `cnn2snn-2.7.2.tar`

### file list

```diff
@@ -1,94 +1,95 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:29:55.753460 cnn2snn-2.7.0/
--rw-r--r--   0 root         (0) root         (0)    11358 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       16 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      665 2024-02-07 14:29:55.753460 cnn2snn-2.7.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      252 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:29:55.741460 cnn2snn-2.7.0/cnn2snn/
--rw-r--r--   0 root         (0) root         (0)     1517 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2149 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/akida_versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:29:55.745460 cnn2snn-2.7.0/cnn2snn/calibration/
--rw-r--r--   0 root         (0) root         (0)      958 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/calibration/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17761 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/calibration/adaround.py
--rw-r--r--   0 root         (0) root         (0)     6564 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/calibration/bias_correction.py
--rw-r--r--   0 root         (0) root         (0)    12381 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/calibration/calibration.py
--rw-r--r--   0 root         (0) root         (0)    10525 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/cli.py
--rw-r--r--   0 root         (0) root         (0)     1701 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/cnn2snn_objects.py
--rw-r--r--   0 root         (0) root         (0)    16610 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/compatibility_checks.py
--rw-r--r--   0 root         (0) root         (0)    10888 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/converter.py
--rw-r--r--   0 root         (0) root         (0)     1440 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/min_value_constraint.py
--rw-r--r--   0 root         (0) root         (0)    13473 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/model_generator.py
--rw-r--r--   0 root         (0) root         (0)    13749 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantization.py
--rw-r--r--   0 root         (0) root         (0)    25908 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantization_layers.py
--rw-r--r--   0 root         (0) root         (0)    12977 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantization_ops.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:29:55.749460 cnn2snn-2.7.0/cnn2snn/quantizeml/
--rw-r--r--   0 root         (0) root         (0)     1446 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3602 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/activations.py
--rw-r--r--   0 root         (0) root         (0)     4203 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/add.py
--rw-r--r--   0 root         (0) root         (0)     5321 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/attention.py
--rw-r--r--   0 root         (0) root         (0)     5503 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/batchnorm.py
--rw-r--r--   0 root         (0) root         (0)     2924 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/block_converter.py
--rw-r--r--   0 root         (0) root         (0)     9596 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/block_converters_generator.py
--rw-r--r--   0 root         (0) root         (0)     8323 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/blocks.py
--rw-r--r--   0 root         (0) root         (0)     5045 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/btc_common.py
--rw-r--r--   0 root         (0) root         (0)     3165 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/buffer_temp_conv.py
--rw-r--r--   0 root         (0) root         (0)     2450 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/concatenate.py
--rw-r--r--   0 root         (0) root         (0)     3915 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/conv2d_transpose.py
--rw-r--r--   0 root         (0) root         (0)    15062 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/conv_common.py
--rw-r--r--   0 root         (0) root         (0)     8048 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/convolution.py
--rw-r--r--   0 root         (0) root         (0)    12257 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/dense.py
--rw-r--r--   0 root         (0) root         (0)     3360 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/depthwise_buffer_temp_conv.py
--rw-r--r--   0 root         (0) root         (0)     6567 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/depthwise_conv2d.py
--rw-r--r--   0 root         (0) root         (0)     4240 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/depthwise_conv2d_transpose.py
--rw-r--r--   0 root         (0) root         (0)     5502 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/dequantizer.py
--rw-r--r--   0 root         (0) root         (0)     4175 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/extract_token.py
--rw-r--r--   0 root         (0) root         (0)     7278 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/input_conv.py
--rw-r--r--   0 root         (0) root         (0)     4142 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/input_data.py
--rw-r--r--   0 root         (0) root         (0)     2416 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/layer_utils.py
--rw-r--r--   0 root         (0) root         (0)     5782 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/madnorm.py
--rw-r--r--   0 root         (0) root         (0)     3584 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/model_generator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:29:55.753460 cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/
--rw-r--r--   0 root         (0) root         (0)      327 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1634 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/activation.py
--rw-r--r--   0 root         (0) root         (0)     2956 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/add.py
--rw-r--r--   0 root         (0) root         (0)     5050 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/base_converter.py
--rw-r--r--   0 root         (0) root         (0)     2716 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/check_compatibility.py
--rw-r--r--   0 root         (0) root         (0)     3499 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/conv2d.py
--rw-r--r--   0 root         (0) root         (0)     4604 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/conv_commons.py
--rw-r--r--   0 root         (0) root         (0)     3815 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/dense.py
--rw-r--r--   0 root         (0) root         (0)     2985 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/depthwise2d.py
--rw-r--r--   0 root         (0) root         (0)     1463 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/dequantizer.py
--rw-r--r--   0 root         (0) root         (0)     2513 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/input_data.py
--rw-r--r--   0 root         (0) root         (0)     1860 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/layer_bounds.py
--rw-r--r--   0 root         (0) root         (0)     4444 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/model_generator.py
--rw-r--r--   0 root         (0) root         (0)     3614 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/padding.py
--rw-r--r--   0 root         (0) root         (0)     2665 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/register.py
--rw-r--r--   0 root         (0) root         (0)     2076 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/scale_out.py
--rw-r--r--   0 root         (0) root         (0)     4535 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/weights.py
--rw-r--r--   0 root         (0) root         (0)     4644 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/outputs.py
--rw-r--r--   0 root         (0) root         (0)     3663 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/padding.py
--rw-r--r--   0 root         (0) root         (0)     4258 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/pooling.py
--rw-r--r--   0 root         (0) root         (0)     6331 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/separable_convolution.py
--rw-r--r--   0 root         (0) root         (0)     3572 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/shiftmax.py
--rw-r--r--   0 root         (0) root         (0)     8596 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/stateful_recurrent.py
--rw-r--r--   0 root         (0) root         (0)     8605 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/stem.py
--rw-r--r--   0 root         (0) root         (0)     1914 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/quantizeml/weights.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:29:55.753460 cnn2snn-2.7.0/cnn2snn/transforms/
--rw-r--r--   0 root         (0) root         (0)     1126 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/transforms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4525 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/transforms/act_step_equalization.py
--rw-r--r--   0 root         (0) root         (0)     8089 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/transforms/batch_normalization.py
--rw-r--r--   0 root         (0) root         (0)     2492 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/transforms/clone.py
--rw-r--r--   0 root         (0) root         (0)     6288 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/transforms/equalization.py
--rw-r--r--   0 root         (0) root         (0)     1670 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/transforms/reshape.py
--rw-r--r--   0 root         (0) root         (0)    15274 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/transforms/sequential.py
--rw-r--r--   0 root         (0) root         (0)     1734 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/utils.py
--rw-r--r--   0 root         (0) root         (0)       99 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/version.py
--rw-r--r--   0 root         (0) root         (0)    11223 2024-02-07 14:29:54.000000 cnn2snn-2.7.0/cnn2snn/weights_ops.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:29:55.753460 cnn2snn-2.7.0/cnn2snn.egg-info/
--rw-r--r--   0 root         (0) root         (0)      665 2024-02-07 14:29:55.000000 cnn2snn-2.7.0/cnn2snn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2926 2024-02-07 14:29:55.000000 cnn2snn-2.7.0/cnn2snn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-07 14:29:55.000000 cnn2snn-2.7.0/cnn2snn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-02-07 14:29:55.000000 cnn2snn-2.7.0/cnn2snn.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       80 2024-02-07 14:29:55.000000 cnn2snn-2.7.0/cnn2snn.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-02-07 14:29:55.000000 cnn2snn-2.7.0/cnn2snn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-07 14:29:55.753460 cnn2snn-2.7.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1154 2024-02-07 14:28:48.000000 cnn2snn-2.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:30:28.359943 cnn2snn-2.7.2/
+-rw-r--r--   0 root         (0) root         (0)    11358 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      665 2024-04-24 15:30:28.359943 cnn2snn-2.7.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      252 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:30:28.351943 cnn2snn-2.7.2/cnn2snn/
+-rw-r--r--   0 root         (0) root         (0)     1517 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2149 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/akida_versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:30:28.351943 cnn2snn-2.7.2/cnn2snn/calibration/
+-rw-r--r--   0 root         (0) root         (0)      958 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/calibration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17761 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/calibration/adaround.py
+-rw-r--r--   0 root         (0) root         (0)     6564 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/calibration/bias_correction.py
+-rw-r--r--   0 root         (0) root         (0)    12381 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/calibration/calibration.py
+-rw-r--r--   0 root         (0) root         (0)    10525 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/cnn2snn_objects.py
+-rw-r--r--   0 root         (0) root         (0)    16610 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/compatibility_checks.py
+-rw-r--r--   0 root         (0) root         (0)    11571 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/converter.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/min_value_constraint.py
+-rw-r--r--   0 root         (0) root         (0)    13473 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/model_generator.py
+-rw-r--r--   0 root         (0) root         (0)    13749 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantization.py
+-rw-r--r--   0 root         (0) root         (0)    25908 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantization_layers.py
+-rw-r--r--   0 root         (0) root         (0)    12977 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantization_ops.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:30:28.355943 cnn2snn-2.7.2/cnn2snn/quantizeml/
+-rw-r--r--   0 root         (0) root         (0)     1479 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/activations.py
+-rw-r--r--   0 root         (0) root         (0)     4203 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/add.py
+-rw-r--r--   0 root         (0) root         (0)     5321 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/attention.py
+-rw-r--r--   0 root         (0) root         (0)     5503 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/batchnorm.py
+-rw-r--r--   0 root         (0) root         (0)     2924 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/block_converter.py
+-rw-r--r--   0 root         (0) root         (0)     9596 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/block_converters_generator.py
+-rw-r--r--   0 root         (0) root         (0)     8323 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/blocks.py
+-rw-r--r--   0 root         (0) root         (0)     5045 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/btc_common.py
+-rw-r--r--   0 root         (0) root         (0)     3165 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/buffer_temp_conv.py
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/concatenate.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/conv2d_transpose.py
+-rw-r--r--   0 root         (0) root         (0)    15062 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/conv_common.py
+-rw-r--r--   0 root         (0) root         (0)     8048 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/convolution.py
+-rw-r--r--   0 root         (0) root         (0)    12257 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/dense.py
+-rw-r--r--   0 root         (0) root         (0)     3360 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/depthwise_buffer_temp_conv.py
+-rw-r--r--   0 root         (0) root         (0)     6567 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/depthwise_conv2d.py
+-rw-r--r--   0 root         (0) root         (0)     4240 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/depthwise_conv2d_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     5502 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/dequantizer.py
+-rw-r--r--   0 root         (0) root         (0)     4175 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/extract_token.py
+-rw-r--r--   0 root         (0) root         (0)     7278 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/input_conv.py
+-rw-r--r--   0 root         (0) root         (0)     4142 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/input_data.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/layer_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5782 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/madnorm.py
+-rw-r--r--   0 root         (0) root         (0)     3584 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/model_generator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:30:28.359943 cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/
+-rw-r--r--   0 root         (0) root         (0)      327 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/activation.py
+-rw-r--r--   0 root         (0) root         (0)     2956 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/add.py
+-rw-r--r--   0 root         (0) root         (0)     5050 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/base_converter.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/check_compatibility.py
+-rw-r--r--   0 root         (0) root         (0)     3499 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/conv2d.py
+-rw-r--r--   0 root         (0) root         (0)     4604 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/conv_commons.py
+-rw-r--r--   0 root         (0) root         (0)     3815 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/dense.py
+-rw-r--r--   0 root         (0) root         (0)     2985 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/depthwise2d.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/dequantizer.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/input_data.py
+-rw-r--r--   0 root         (0) root         (0)     1860 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/layer_bounds.py
+-rw-r--r--   0 root         (0) root         (0)     4444 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/model_generator.py
+-rw-r--r--   0 root         (0) root         (0)     4231 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/padding.py
+-rw-r--r--   0 root         (0) root         (0)     2665 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/register.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/scale_out.py
+-rw-r--r--   0 root         (0) root         (0)     4535 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/weights.py
+-rw-r--r--   0 root         (0) root         (0)     4644 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/outputs.py
+-rw-r--r--   0 root         (0) root         (0)     3663 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/padding.py
+-rw-r--r--   0 root         (0) root         (0)     4258 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/pooling.py
+-rw-r--r--   0 root         (0) root         (0)     6331 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/separable_convolution.py
+-rw-r--r--   0 root         (0) root         (0)     3572 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/shiftmax.py
+-rw-r--r--   0 root         (0) root         (0)     8369 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/stateful_recurrent.py
+-rw-r--r--   0 root         (0) root         (0)     9236 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/stem.py
+-rw-r--r--   0 root         (0) root         (0)    18917 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/vit_encoder_block.py
+-rw-r--r--   0 root         (0) root         (0)     1914 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/quantizeml/weights.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:30:28.359943 cnn2snn-2.7.2/cnn2snn/transforms/
+-rw-r--r--   0 root         (0) root         (0)     1126 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/transforms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4525 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/transforms/act_step_equalization.py
+-rw-r--r--   0 root         (0) root         (0)     8089 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/transforms/batch_normalization.py
+-rw-r--r--   0 root         (0) root         (0)     2492 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/transforms/clone.py
+-rw-r--r--   0 root         (0) root         (0)     6288 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/transforms/equalization.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/transforms/reshape.py
+-rw-r--r--   0 root         (0) root         (0)    15274 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/transforms/sequential.py
+-rw-r--r--   0 root         (0) root         (0)     1734 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/utils.py
+-rw-r--r--   0 root         (0) root         (0)       99 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/version.py
+-rw-r--r--   0 root         (0) root         (0)    11223 2024-04-24 15:30:27.000000 cnn2snn-2.7.2/cnn2snn/weights_ops.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:30:28.359943 cnn2snn-2.7.2/cnn2snn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      665 2024-04-24 15:30:28.000000 cnn2snn-2.7.2/cnn2snn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2966 2024-04-24 15:30:28.000000 cnn2snn-2.7.2/cnn2snn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 15:30:28.000000 cnn2snn-2.7.2/cnn2snn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-04-24 15:30:28.000000 cnn2snn-2.7.2/cnn2snn.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-24 15:30:28.000000 cnn2snn-2.7.2/cnn2snn.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-24 15:30:28.000000 cnn2snn-2.7.2/cnn2snn.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 15:30:28.359943 cnn2snn-2.7.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1154 2024-04-24 15:29:26.000000 cnn2snn-2.7.2/setup.py
```

### Comparing `cnn2snn-2.7.0/LICENSE` & `cnn2snn-2.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/PKG-INFO` & `cnn2snn-2.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: cnn2snn
-Version: 2.7.0
+Version: 2.7.2
 Summary: Keras to Akida CNN Converter
 Home-page: https://doc.brainchipinc.com
 Author: Nezar Lheimeur
 Author-email: nlheimeur@brainchip.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tensorflow<2.13.0,>=2.10.0
 Requires-Dist: keras<2.13.0,>=2.10.0
-Requires-Dist: akida==2.7.0
+Requires-Dist: akida==2.7.2
 Requires-Dist: quantizeml~=0.8.1
 
 # CNN2SNN toolkit
 
 The Brainchip CNN2SNN toolkit provides a means to convert Convolutional Neural
 Networks (CNN) that were trained using Deep Learning methods to a low-latency 
 and low-power Spiking Neural Network (SNN) for use with the Akida Runtime.
```

### Comparing `cnn2snn-2.7.0/cnn2snn/__init__.py` & `cnn2snn-2.7.2/cnn2snn/__init__.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/akida_versions.py` & `cnn2snn-2.7.2/cnn2snn/akida_versions.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/calibration/__init__.py` & `cnn2snn-2.7.2/cnn2snn/calibration/__init__.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/calibration/adaround.py` & `cnn2snn-2.7.2/cnn2snn/calibration/adaround.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/calibration/bias_correction.py` & `cnn2snn-2.7.2/cnn2snn/calibration/bias_correction.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/calibration/calibration.py` & `cnn2snn-2.7.2/cnn2snn/calibration/calibration.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/cli.py` & `cnn2snn-2.7.2/cnn2snn/cli.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/cnn2snn_objects.py` & `cnn2snn-2.7.2/cnn2snn/cnn2snn_objects.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/compatibility_checks.py` & `cnn2snn-2.7.2/cnn2snn/compatibility_checks.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/converter.py` & `cnn2snn-2.7.2/cnn2snn/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 
 import os
 import warnings
 import tensorflow as tf
 from onnx import ModelProto
 from .model_generator import generate_model as cnn2snn_generate_model
 from .quantizeml import generate_model as qml_generate_model
+from .quantizeml.vit_encoder_block import fold_vitencoderblock
 
+import akida
 from .akida_versions import get_akida_version, AkidaVersion
 from .transforms import fix_v1_activation_variables, prepare_to_convert
 from .compatibility_checks import check_sequential_compatibility
 from quantizeml.models import QuantizationParams, quantize as quantize_qml
 
 
 def check_model_compatibility(model, device=None):
@@ -46,15 +48,15 @@
     Raises:
         ValueError: if model type is incompatbile with Akida version context.
         ValueError: if device is incompatibile with Akida version context.
         Exception: if an incompatibility is encountered on quantization/conversion/mapping steps.
     """
     # Preliminary checks:
     # Onnx models are not supported on Akida v1
-    if (get_akida_version() == AkidaVersion.v1) and (type(model) == ModelProto):
+    if (get_akida_version() == AkidaVersion.v1) and (isinstance(model, ModelProto)):
         raise ValueError("Akida v1 does not support ONNX models. Use Akida v2 instead.")
 
     # if a device is provided, it should be consistent with the Akida version used.
     if device is not None and device.version.product_id in [0, 0xa1] \
             and (get_akida_version() != AkidaVersion.v1):
         raise ValueError(f"The device {device} is inconsistent with the Akida version used.")
 
@@ -119,17 +121,16 @@
         ak_model = _convert_cnn2snn(model, input_scaling)
     else:
         if input_scaling:
             warnings.warn(UserWarning("Cannot use input_scaling parameter when converting"
                                       " quantizeml models to akida."))
         ak_model = _convert_quantizeml(model)
 
-    # check if the akida v1 model has an unvalid act_step, that prevents the model
-    # to map on HW. If so equalize the Akida model activation variables.
-    fix_v1_activation_variables(ak_model)
+    # Perform post conversion checks on the model
+    ak_model = _post_conversion_checks(ak_model)
 
     # Save model if file_path is given
     if file_path:
         # Create directories
         dir_name, base_name = os.path.split(file_path)
         if base_name:
             file_root, file_ext = os.path.splitext(base_name)
@@ -275,7 +276,25 @@
     """
 
     Rescaling = tf.keras.layers.Rescaling
     for layer in model.layers[:2]:
         if isinstance(layer, Rescaling):
             return (1 / layer.scale, -layer.offset / layer.scale)
     return None
+
+
+def _post_conversion_checks(model):
+    """ Perform post-conversion checks on an akida model.
+
+    The model is not necessarily changed and can be the original one.
+
+    Args:
+        model (Model): the model to check
+    """
+    if model.ip_version == akida.core.IpVersion.v1:
+        # check if the akida v1 model has an unvalid act_step, that prevents the model
+        # to map on HW. If so equalize the Akida model activation variables.
+        fix_v1_activation_variables(model)
+    elif model.ip_version == akida.core.IpVersion.v2:
+        # look for attention and group constitutive layers into VitEncoderBlock layer when possible
+        model = fold_vitencoderblock(model)
+    return model
```

### Comparing `cnn2snn-2.7.0/cnn2snn/min_value_constraint.py` & `cnn2snn-2.7.2/cnn2snn/min_value_constraint.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/model_generator.py` & `cnn2snn-2.7.2/cnn2snn/model_generator.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantization.py` & `cnn2snn-2.7.2/cnn2snn/quantization.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantization_layers.py` & `cnn2snn-2.7.2/cnn2snn/quantization_layers.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantization_ops.py` & `cnn2snn-2.7.2/cnn2snn/quantization_ops.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/__init__.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,7 +30,8 @@
 from .madnorm import *
 from .concatenate import *
 from .extract_token import *
 from .dequantizer import *
 from .buffer_temp_conv import *
 from .depthwise_buffer_temp_conv import *
 from .stateful_recurrent import *
+from .vit_encoder_block import *
```

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/activations.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/activations.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/add.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/add.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/attention.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/attention.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/batchnorm.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/batchnorm.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/block_converter.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/block_converter.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/block_converters_generator.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/block_converters_generator.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/blocks.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/blocks.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/btc_common.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/btc_common.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/buffer_temp_conv.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/buffer_temp_conv.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/concatenate.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/concatenate.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/conv2d_transpose.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/conv_common.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/conv_common.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/convolution.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/convolution.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/dense.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/dense.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/depthwise_buffer_temp_conv.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/depthwise_buffer_temp_conv.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/depthwise_conv2d.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/depthwise_conv2d_transpose.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/depthwise_conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/dequantizer.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/dequantizer.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/extract_token.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/extract_token.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/input_conv.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/input_conv.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/input_data.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/input_data.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/layer_utils.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/layer_utils.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/madnorm.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/madnorm.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/model_generator.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/model_generator.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/activation.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/activation.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/add.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/add.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/base_converter.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/base_converter.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/check_compatibility.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/check_compatibility.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/conv2d.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/conv2d.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/conv_commons.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/conv_commons.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/dense.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/dense.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/depthwise2d.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/depthwise2d.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/dequantizer.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/dequantizer.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/input_data.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/input_data.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/layer_bounds.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/layer_bounds.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/model_generator.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/model_generator.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/padding.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/padding.py`

 * *Files 13% similar despite different names*

```diff
@@ -57,36 +57,46 @@
         converter (OnnxConverter): the converter to extract the padding.
 
     Returns:
         akida.Padding: the padding
     """
     # Check pads are compatible with akida.Padding.Same
     kernel_shapes = converter.weights["W"].shape[-2:]
-    if any(x for x in converter.pads):
-        exp_pads = compute_same_pads(converter.input_shape[:2], kernel_shapes, converter.strides)
-        ak_padding = akida.Padding.Same
-    else:
-        exp_pads = [0] * 2 * len(kernel_shapes)
-        ak_padding = akida.Padding.Valid
+    # Initially assume padding corresponds to akida.Padding.Same
+    exp_pads = compute_same_pads(converter.input_shape[:2], kernel_shapes, converter.strides)
+    ak_padding = akida.Padding.Same
     # Pads in FC dimensions have to be zero
     fc_pads = converter.pads[:2] + converter.pads[4:6]
     if any(fc_pads):
         raise ValueError(f"Unrecognized {converter.pads} pads in {converter.name}.")
     # Compare if convolutional padding produces same behavior than Akida
     convert_pads = converter.pads[2:4] + converter.pads[6:]
     if convert_pads != exp_pads:
-        raise ValueError(f"Expect pads {exp_pads} (found {convert_pads}) in {converter.name}.")
+        if all(x == 0 for x in convert_pads):
+            # Force ak_padding to Valid, because no padding is supported as Valid in akida HW
+            ak_padding = akida.Padding.Valid
+            exp_pads = [0] * 2 * len(kernel_shapes)
+        else:
+            raise ValueError(f"Expect pads {exp_pads} (found {convert_pads}) in {converter.name}.")
 
     # Compare if max pool padding produces same behavior than Akida
     if converter.pool_type == akida.PoolType.Max:
         # Calculate convolutional output shape
         out_shape = compute_conv_output(converter.input_shape[:2],
                                         kernel_shapes,
                                         converter.strides,
                                         convert_pads)
         if ak_padding == akida.Padding.Same:
-            exp_pads = compute_same_pads(out_shape, converter.pool_size, converter.pool_strides)
+            exp_pool_pads = compute_same_pads(out_shape,
+                                              converter.pool_size,
+                                              converter.pool_strides)
+            if converter.pool_pads != exp_pool_pads and all(x == 0 for x in exp_pads):
+                # Mismatch when padding Same. Try once again with a valid one,
+                # given in this condition both padding are exchangable.
+                ak_padding = akida.Padding.Valid
+            else:
+                exp_pads = exp_pool_pads
         if converter.pool_pads != exp_pads:
             raise ValueError(f"Expect pads {exp_pads} (found {converter.pool_pads}) "
                              f"in {converter.name} maxpool.")
 
     return ak_padding
```

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/register.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/register.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/scale_out.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/scale_out.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/onnx_conversion/weights.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/onnx_conversion/weights.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/outputs.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/outputs.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/padding.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/padding.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/pooling.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/pooling.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/separable_convolution.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/separable_convolution.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/shiftmax.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/shiftmax.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/stateful_recurrent.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/stateful_recurrent.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,22 +86,17 @@
     A_real_ak = stateful_rec.a_quantizer(stateful_rec.A_real).values.numpy()
     variables_ak["A_real"] = A_real_ak.astype(np.int16)
     A_imag_ak = stateful_rec.a_quantizer(stateful_rec.A_imag).values.numpy()
     variables_ak["A_imag"] = A_imag_ak.astype(np.int16)
 
     # Set intermediate stateful_outputs_shift
     internal_state_shift = stateful_rec.out_quantizer.shift.value[0]
+    assert np.all(internal_state_shift <= 0), "shift values should be negative"
     broadcast_and_set_variable(variables_ak, "internal_state_outputs_shift",
-                               internal_state_shift.numpy().astype(np.int8))
-
-    # Set out_projection input_shift
-    out_proj_inputs_shift = getattr(out_proj_dense, 'input_shift', None)
-    if out_proj_inputs_shift is not None:
-        broadcast_and_set_variable(variables_ak, "out_proj_inputs_shift",
-                                   out_proj_inputs_shift.value.numpy().astype(np.uint8))
+                               np.abs(internal_state_shift.numpy()).astype(np.uint8))
 
     # Set out_proj dense kernel variable
     out_proj_ak = out_proj_dense.weight_quantizer.qweights.value.fp.values.numpy()
     variables_ak["out_proj"] = out_proj_ak.astype(np.int8)
 
     if out_proj_dense.use_bias:
         bias_quantizer = out_proj_dense.bias_quantizer
```

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/stem.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/stem.py`

 * *Files 8% similar despite different names*

```diff
@@ -199,11 +199,21 @@
         # Stem handles only square kernels.
         if (kernel_size[0] != kernel_size[1]):
             raise ValueError("input should have square kernels. Receives: "
                              f"k_x={kernel_size[0]} and k_y={kernel_size[1]}")
         # Stem input size must be a multiple of kernel size.
         if (input_shape[0] % kernel_size[0] != 0):
             raise ValueError("Input spatial dimension size must be a multiple of kernel size")
+        stride_x = embedding.strides[0]
+        stride_y = embedding.strides[1]
+        # Stem handles only same strides along its spatial dims
+        if (stride_x != stride_y):
+            raise ValueError("Input should have the same strides along its spatial dims. "
+                             f"Receives: x_stride={stride_x} and y_stride={stride_y}")
+        # Stem kernel size should be equal kernel stride.
+        if (kernel_size[0] != stride_x):
+            raise ValueError("Input kernel size should be equal kernel stride. "
+                             f"Received: kernel_size={kernel_size[0]} and stride={stride_x}")
 
 
 # Register the valid stem block pattern for Akida v2
 register_conversion_patterns(AkidaVersion.v2, _PATTERNS, StemBlockConverter, input_pattern=True)
```

### Comparing `cnn2snn-2.7.0/cnn2snn/quantizeml/weights.py` & `cnn2snn-2.7.2/cnn2snn/quantizeml/weights.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/transforms/__init__.py` & `cnn2snn-2.7.2/cnn2snn/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/transforms/act_step_equalization.py` & `cnn2snn-2.7.2/cnn2snn/transforms/act_step_equalization.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/transforms/batch_normalization.py` & `cnn2snn-2.7.2/cnn2snn/transforms/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/transforms/clone.py` & `cnn2snn-2.7.2/cnn2snn/transforms/clone.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/transforms/equalization.py` & `cnn2snn-2.7.2/cnn2snn/transforms/equalization.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/transforms/reshape.py` & `cnn2snn-2.7.2/cnn2snn/transforms/reshape.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/transforms/sequential.py` & `cnn2snn-2.7.2/cnn2snn/transforms/sequential.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/utils.py` & `cnn2snn-2.7.2/cnn2snn/utils.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn/weights_ops.py` & `cnn2snn-2.7.2/cnn2snn/weights_ops.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.7.0/cnn2snn.egg-info/PKG-INFO` & `cnn2snn-2.7.2/cnn2snn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: cnn2snn
-Version: 2.7.0
+Version: 2.7.2
 Summary: Keras to Akida CNN Converter
 Home-page: https://doc.brainchipinc.com
 Author: Nezar Lheimeur
 Author-email: nlheimeur@brainchip.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tensorflow<2.13.0,>=2.10.0
 Requires-Dist: keras<2.13.0,>=2.10.0
-Requires-Dist: akida==2.7.0
+Requires-Dist: akida==2.7.2
 Requires-Dist: quantizeml~=0.8.1
 
 # CNN2SNN toolkit
 
 The Brainchip CNN2SNN toolkit provides a means to convert Convolutional Neural
 Networks (CNN) that were trained using Deep Learning methods to a low-latency 
 and low-power Spiking Neural Network (SNN) for use with the Akida Runtime.
```

### Comparing `cnn2snn-2.7.0/cnn2snn.egg-info/SOURCES.txt` & `cnn2snn-2.7.2/cnn2snn.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 cnn2snn/quantizeml/outputs.py
 cnn2snn/quantizeml/padding.py
 cnn2snn/quantizeml/pooling.py
 cnn2snn/quantizeml/separable_convolution.py
 cnn2snn/quantizeml/shiftmax.py
 cnn2snn/quantizeml/stateful_recurrent.py
 cnn2snn/quantizeml/stem.py
+cnn2snn/quantizeml/vit_encoder_block.py
 cnn2snn/quantizeml/weights.py
 cnn2snn/quantizeml/onnx_conversion/__init__.py
 cnn2snn/quantizeml/onnx_conversion/activation.py
 cnn2snn/quantizeml/onnx_conversion/add.py
 cnn2snn/quantizeml/onnx_conversion/base_converter.py
 cnn2snn/quantizeml/onnx_conversion/check_compatibility.py
 cnn2snn/quantizeml/onnx_conversion/conv2d.py
```

### Comparing `cnn2snn-2.7.0/setup.py` & `cnn2snn-2.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 # Read the contents of the README file
 directory = path.abspath(path.dirname(__file__))
 with open(path.join(directory, 'README'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='cnn2snn',
-    version='2.7.0',
+    version='2.7.2',
     description='Keras to Akida CNN Converter',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Nezar Lheimeur',
     author_email='nlheimeur@brainchip.com',
     url='https://doc.brainchipinc.com',
     license='Apache 2.0',
     packages=['cnn2snn', 'cnn2snn.transforms', 'cnn2snn.calibration', 'cnn2snn.quantizeml',
               'cnn2snn.quantizeml.onnx_conversion'],
     entry_points={
         'console_scripts': [ 'cnn2snn = cnn2snn.cli:main' ]
     },
     install_requires=[get_tf_dep(), 'keras>=2.10.0,<2.13.0',
-        'akida==2.7.0', 'quantizeml~=0.8.1'],
+        'akida==2.7.2', 'quantizeml~=0.8.1'],
 )
```

