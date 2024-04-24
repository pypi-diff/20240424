# Comparing `tmp/tensorrt_lean_cu12_libs-10.0.0b6.tar.gz` & `tmp/tensorrt_lean_cu12_libs-10.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorrt_lean_cu12_libs-10.0.0b6.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
+gzip compressed data, was "tensorrt_lean_cu12_libs-10.0.1.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `tensorrt_lean_cu12_libs-10.0.0b6.tar` & `tensorrt_lean_cu12_libs-10.0.1.tar`

### file list

```diff
@@ -1,2 +1,2 @@
 -rw-r--r--   0        0        0      217 1993-04-05 07:00:00.000000 pyproject.toml
--rw-r--r--   0        0        0      525 1993-04-05 07:00:00.000000 PKG-INFO
+-rw-r--r--   0        0        0      523 1993-04-05 07:00:00.000000 PKG-INFO
```

### PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorrt_lean-cu12_libs
-Version: 10.0.0b6
+Version: 10.0.1
 Summary: TensorRT Libraries
 Home-page: https://developer.nvidia.com/tensorrt
 Download-URL: https://github.com/nvidia/tensorrt/tags
 Author: NVIDIA Corporation
 License: Proprietary
 Keywords: nvidia tensorrt deeplearning inference
 Classifier: License :: Other/Proprietary License
```

