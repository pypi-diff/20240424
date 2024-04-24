# Comparing `tmp/tensorrt_cu12_bindings-10.0.0b6-cp39-none-win_amd64.whl.zip` & `tmp/tensorrt_cu12_bindings-10.0.1-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,12 @@
-Zip file size: 711165 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat     5875 b- defN 24-Mar-14 05:35 tensorrt_bindings/__init__.py
--rw-rw-rw-  2.0 fat  2113536 b- defN 24-Mar-14 05:35 tensorrt_bindings/tensorrt.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    47141 b- defN 24-Mar-14 05:35 tensorrt_cu12_bindings-10.0.0b6.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      610 b- defN 24-Mar-14 05:35 tensorrt_cu12_bindings-10.0.0b6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       99 b- defN 24-Mar-14 05:35 tensorrt_cu12_bindings-10.0.0b6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 24-Mar-14 05:35 tensorrt_cu12_bindings-10.0.0b6.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 24-Mar-14 05:35 tensorrt_cu12_bindings-10.0.0b6.dist-info/zip-safe
-?rw-rw-r--  2.0 fat      775 b- defN 24-Mar-14 05:35 tensorrt_cu12_bindings-10.0.0b6.dist-info/RECORD
-8 files, 2168056 bytes uncompressed, 709781 bytes compressed:  67.3%
+Zip file size: 712317 bytes, number of entries: 10
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-17 01:51 tensorrt_bindings/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-17 01:51 tensorrt_cu12_bindings-10.0.1.dist-info/
+-rw-r--r--  2.0 unx     5888 b- defN 24-Apr-17 01:51 tensorrt_bindings/__init__.py
+-rw-r--r--  2.0 unx  2115072 b- defN 24-Apr-17 01:51 tensorrt_bindings/tensorrt.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx      608 b- defN 24-Apr-17 01:51 tensorrt_cu12_bindings-10.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx        2 b- defN 24-Apr-17 01:51 tensorrt_cu12_bindings-10.0.1.dist-info/zip-safe
+-rw-r--r--  2.0 unx       18 b- defN 24-Apr-17 01:51 tensorrt_cu12_bindings-10.0.1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx       99 b- defN 24-Apr-17 01:51 tensorrt_cu12_bindings-10.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      763 b- defN 24-Apr-17 01:51 tensorrt_cu12_bindings-10.0.1.dist-info/RECORD
+-rw-r--r--  2.0 unx    47141 b- defN 24-Apr-17 01:51 tensorrt_cu12_bindings-10.0.1.dist-info/LICENSE.txt
+10 files, 2169591 bytes uncompressed, 710689 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -1,25 +1,31 @@
+Filename: tensorrt_bindings/
+Comment: 
+
+Filename: tensorrt_cu12_bindings-10.0.1.dist-info/
+Comment: 
+
 Filename: tensorrt_bindings/__init__.py
 Comment: 
 
 Filename: tensorrt_bindings/tensorrt.cp39-win_amd64.pyd
 Comment: 
 
-Filename: tensorrt_cu12_bindings-10.0.0b6.dist-info/LICENSE.txt
+Filename: tensorrt_cu12_bindings-10.0.1.dist-info/METADATA
 Comment: 
 
-Filename: tensorrt_cu12_bindings-10.0.0b6.dist-info/METADATA
+Filename: tensorrt_cu12_bindings-10.0.1.dist-info/zip-safe
 Comment: 
 
-Filename: tensorrt_cu12_bindings-10.0.0b6.dist-info/WHEEL
+Filename: tensorrt_cu12_bindings-10.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: tensorrt_cu12_bindings-10.0.0b6.dist-info/top_level.txt
+Filename: tensorrt_cu12_bindings-10.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: tensorrt_cu12_bindings-10.0.0b6.dist-info/zip-safe
+Filename: tensorrt_cu12_bindings-10.0.1.dist-info/RECORD
 Comment: 
 
-Filename: tensorrt_cu12_bindings-10.0.0b6.dist-info/RECORD
+Filename: tensorrt_cu12_bindings-10.0.1.dist-info/LICENSE.txt
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## tensorrt_bindings/__init__.py

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
             "cublas64_12.dll",
             "cublasLt64_12.dll",
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
     }["tensorrt"]
 
     for lib in LIBRARIES:
         lib_path = find_lib(lib)
         if lib_path != "":
             ctypes.CDLL(lib_path)
 
 del _libs_wheel_imported
 
 from .tensorrt import *
 
-__version__ = "10.0.0b6"
+__version__ = "10.0.1"
 
 
 # Provides Python's `with` syntax
 def common_enter(this):
     warnings.warn(
         "Context managers for TensorRT types are deprecated. "
         "Memory will be freed automatically when the reference count reaches 0.",
```

## Comparing `tensorrt_cu12_bindings-10.0.0b6.dist-info/LICENSE.txt` & `tensorrt_cu12_bindings-10.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `tensorrt_cu12_bindings-10.0.0b6.dist-info/METADATA` & `tensorrt_cu12_bindings-10.0.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorrt-cu12_bindings
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

## Comparing `tensorrt_cu12_bindings-10.0.0b6.dist-info/RECORD` & `tensorrt_cu12_bindings-10.0.1.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-tensorrt_bindings/__init__.py,sha256=6TB7xXC-FpiJYmFdfyabH7oKg7cG9KOX1VyHotq5V1A,5875
-tensorrt_bindings/tensorrt.cp39-win_amd64.pyd,sha256=n4-Oj3-XirYqD5viGWbKRPrymY9erBtvoluDFT6Zww8,2113536
-tensorrt_cu12_bindings-10.0.0b6.dist-info/LICENSE.txt,sha256=yGkV_ZW7773aMTWqzj5q1rRhKEbcvbxdL1o4sTndiLQ,47141
-tensorrt_cu12_bindings-10.0.0b6.dist-info/METADATA,sha256=a6fLte25IT6x6yxmIZAThydoTf8sx61LX7VxmJ34ZR8,610
-tensorrt_cu12_bindings-10.0.0b6.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-tensorrt_cu12_bindings-10.0.0b6.dist-info/top_level.txt,sha256=QuFeuaCbu20Zk7dFQs6JlSlk-ZLCkirage8XegBmyP0,18
-tensorrt_cu12_bindings-10.0.0b6.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-tensorrt_cu12_bindings-10.0.0b6.dist-info/RECORD,,
+tensorrt_bindings/__init__.py,sha256=YYWpJ67Z6hgxuYZhJ4epk-FxPhj1i41cgC-A5B74OH8,5888
+tensorrt_bindings/tensorrt.cp39-win_amd64.pyd,sha256=o2KhEDXn1l6xBzVsTvy_X5nru3so5MGx_dTn7PCqNUE,2115072
+tensorrt_cu12_bindings-10.0.1.dist-info/LICENSE.txt,sha256=yGkV_ZW7773aMTWqzj5q1rRhKEbcvbxdL1o4sTndiLQ,47141
+tensorrt_cu12_bindings-10.0.1.dist-info/METADATA,sha256=2h0yIo0YxHcY-x9TiWEx6se-GKNZwsI8LTfLYo7UH9Q,608
+tensorrt_cu12_bindings-10.0.1.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+tensorrt_cu12_bindings-10.0.1.dist-info/top_level.txt,sha256=QuFeuaCbu20Zk7dFQs6JlSlk-ZLCkirage8XegBmyP0,18
+tensorrt_cu12_bindings-10.0.1.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+tensorrt_cu12_bindings-10.0.1.dist-info/RECORD,,
```

