# Comparing `tmp/tensorrt_lean_cu11_bindings-10.0.0b6-cp39-none-win_amd64.whl.zip` & `tmp/tensorrt_lean_cu11_bindings-10.0.1-cp311-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,12 @@
-Zip file size: 503837 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat     5895 b- defN 24-Mar-14 05:07 tensorrt_lean_bindings/__init__.py
--rw-rw-rw-  2.0 fat  1313792 b- defN 24-Mar-14 05:07 tensorrt_lean_bindings/tensorrt_lean.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    47141 b- defN 24-Mar-14 05:07 tensorrt_lean_cu11_bindings-10.0.0b6.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      615 b- defN 24-Mar-14 05:07 tensorrt_lean_cu11_bindings-10.0.0b6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       99 b- defN 24-Mar-14 05:07 tensorrt_lean_cu11_bindings-10.0.0b6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 24-Mar-14 05:07 tensorrt_lean_cu11_bindings-10.0.0b6.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 24-Mar-14 05:07 tensorrt_lean_cu11_bindings-10.0.0b6.dist-info/zip-safe
-?rw-rw-r--  2.0 fat      820 b- defN 24-Mar-14 05:07 tensorrt_lean_cu11_bindings-10.0.0b6.dist-info/RECORD
-8 files, 1368387 bytes uncompressed, 502363 bytes compressed:  63.3%
+Zip file size: 535574 bytes, number of entries: 10
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-17 02:19 tensorrt_lean_bindings/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-17 02:19 tensorrt_lean_cu11_bindings-10.0.1.dist-info/
+-rw-r--r--  2.0 unx      613 b- defN 24-Apr-17 02:19 tensorrt_lean_cu11_bindings-10.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx        2 b- defN 24-Apr-17 02:19 tensorrt_lean_cu11_bindings-10.0.1.dist-info/zip-safe
+-rw-r--r--  2.0 unx       23 b- defN 24-Apr-17 02:19 tensorrt_lean_cu11_bindings-10.0.1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      100 b- defN 24-Apr-17 02:19 tensorrt_lean_cu11_bindings-10.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      810 b- defN 24-Apr-17 02:19 tensorrt_lean_cu11_bindings-10.0.1.dist-info/RECORD
+-rw-r--r--  2.0 unx    47141 b- defN 24-Apr-17 02:19 tensorrt_lean_cu11_bindings-10.0.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx  1480704 b- defN 24-Apr-17 02:19 tensorrt_lean_bindings/tensorrt_lean.cp311-win_amd64.pyd
+-rw-r--r--  2.0 unx     5908 b- defN 24-Apr-17 02:19 tensorrt_lean_bindings/__init__.py
+10 files, 1535301 bytes uncompressed, 533834 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -1,25 +1,31 @@
-Filename: tensorrt_lean_bindings/__init__.py
+Filename: tensorrt_lean_bindings/
+Comment: 
+
+Filename: tensorrt_lean_cu11_bindings-10.0.1.dist-info/
 Comment: 
 
-Filename: tensorrt_lean_bindings/tensorrt_lean.cp39-win_amd64.pyd
+Filename: tensorrt_lean_cu11_bindings-10.0.1.dist-info/METADATA
 Comment: 
 
-Filename: tensorrt_lean_cu11_bindings-10.0.0b6.dist-info/LICENSE.txt
+Filename: tensorrt_lean_cu11_bindings-10.0.1.dist-info/zip-safe
 Comment: 
 
-Filename: tensorrt_lean_cu11_bindings-10.0.0b6.dist-info/METADATA
+Filename: tensorrt_lean_cu11_bindings-10.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: tensorrt_lean_cu11_bindings-10.0.0b6.dist-info/WHEEL
+Filename: tensorrt_lean_cu11_bindings-10.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: tensorrt_lean_cu11_bindings-10.0.0b6.dist-info/top_level.txt
+Filename: tensorrt_lean_cu11_bindings-10.0.1.dist-info/RECORD
 Comment: 
 
-Filename: tensorrt_lean_cu11_bindings-10.0.0b6.dist-info/zip-safe
+Filename: tensorrt_lean_cu11_bindings-10.0.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: tensorrt_lean_cu11_bindings-10.0.0b6.dist-info/RECORD
+Filename: tensorrt_lean_bindings/tensorrt_lean.cp311-win_amd64.pyd
+Comment: 
+
+Filename: tensorrt_lean_bindings/__init__.py
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## tensorrt_lean_bindings/__init__.py

```diff
@@ -47,39 +47,39 @@
         raise FileNotFoundError(
             "Could not find: {:}. Is it on your PATH?\nNote: Paths searched were:\n{:}".format(name, paths)
         )
 
     # Order matters here because of dependencies
     LIBRARIES = {
         "tensorrt": [
-            "nvinfer.dll",
+            "nvinfer_10.dll",
             "cublas64_11.dll",
             "cublasLt64_11.dll",
             "cudnn64_##CUDNN_MAJOR##.dll",
-            "nvinfer_plugin.dll",
-            "nvonnxparser.dll",
+            "nvinfer_plugin_10.dll",
+            "nvonnxparser_10.dll",
         ],
         "tensorrt_dispatch": [
-            "nvinfer_dispatch.dll",
+            "nvinfer_dispatch_10.dll",
         ],
         "tensorrt_lean": [
-            "nvinfer_lean.dll",
+            "nvinfer_lean_10.dll",
         ],
     }["tensorrt_lean"]
 
     for lib in LIBRARIES:
         lib_path = find_lib(lib)
         if lib_path != "":
             ctypes.CDLL(lib_path)
 
 del _libs_wheel_imported
 
 from .tensorrt_lean import *
 
-__version__ = "10.0.0b6"
+__version__ = "10.0.1"
 
 
 # Provides Python's `with` syntax
 def common_enter(this):
     warnings.warn(
         "Context managers for TensorRT types are deprecated. "
         "Memory will be freed automatically when the reference count reaches 0.",
```

## Comparing `tensorrt_lean_cu11_bindings-10.0.0b6.dist-info/LICENSE.txt` & `tensorrt_lean_cu11_bindings-10.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `tensorrt_lean_cu11_bindings-10.0.0b6.dist-info/METADATA` & `tensorrt_lean_cu11_bindings-10.0.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorrt_lean-cu11_bindings
-Version: 10.0.0b6
+Version: 10.0.1
 Summary: A high performance deep learning inference library
 Home-page: https://developer.nvidia.com/tensorrt
 Download-URL: https://github.com/nvidia/tensorrt/tags
 Author: NVIDIA Corporation
 License: Proprietary
 Keywords: nvidia tensorrt deeplearning inference
 Classifier: License :: Other/Proprietary License
```

