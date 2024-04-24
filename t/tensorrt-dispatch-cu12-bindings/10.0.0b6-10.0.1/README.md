# Comparing `tmp/tensorrt_dispatch_cu12_bindings-10.0.0b6-cp39-none-win_amd64.whl.zip` & `tmp/tensorrt_dispatch_cu12_bindings-10.0.1-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,12 @@
-Zip file size: 503942 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat     5911 b- defN 24-Mar-14 05:35 tensorrt_dispatch_bindings/__init__.py
--rw-rw-rw-  2.0 fat  1313792 b- defN 24-Mar-14 05:35 tensorrt_dispatch_bindings/tensorrt_dispatch.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    47141 b- defN 24-Mar-14 05:35 tensorrt_dispatch_cu12_bindings-10.0.0b6.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      619 b- defN 24-Mar-14 05:35 tensorrt_dispatch_cu12_bindings-10.0.0b6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       99 b- defN 24-Mar-14 05:35 tensorrt_dispatch_cu12_bindings-10.0.0b6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       27 b- defN 24-Mar-14 05:35 tensorrt_dispatch_cu12_bindings-10.0.0b6.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 24-Mar-14 05:35 tensorrt_dispatch_cu12_bindings-10.0.0b6.dist-info/zip-safe
-?rw-rw-r--  2.0 fat      856 b- defN 24-Mar-14 05:35 tensorrt_dispatch_cu12_bindings-10.0.0b6.dist-info/RECORD
-8 files, 1368447 bytes uncompressed, 502396 bytes compressed:  63.3%
+Zip file size: 504871 bytes, number of entries: 10
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-17 01:51 tensorrt_dispatch_bindings/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-17 01:51 tensorrt_dispatch_cu12_bindings-10.0.1.dist-info/
+-rw-r--r--  2.0 unx  1315328 b- defN 24-Apr-17 01:51 tensorrt_dispatch_bindings/tensorrt_dispatch.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx     5924 b- defN 24-Apr-17 01:51 tensorrt_dispatch_bindings/__init__.py
+-rw-r--r--  2.0 unx      617 b- defN 24-Apr-17 01:51 tensorrt_dispatch_cu12_bindings-10.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx        2 b- defN 24-Apr-17 01:51 tensorrt_dispatch_cu12_bindings-10.0.1.dist-info/zip-safe
+-rw-r--r--  2.0 unx       27 b- defN 24-Apr-17 01:51 tensorrt_dispatch_cu12_bindings-10.0.1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx       99 b- defN 24-Apr-17 01:51 tensorrt_dispatch_cu12_bindings-10.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      844 b- defN 24-Apr-17 01:51 tensorrt_dispatch_cu12_bindings-10.0.1.dist-info/RECORD
+-rw-r--r--  2.0 unx    47141 b- defN 24-Apr-17 01:51 tensorrt_dispatch_cu12_bindings-10.0.1.dist-info/LICENSE.txt
+10 files, 1369982 bytes uncompressed, 503045 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -1,25 +1,31 @@
-Filename: tensorrt_dispatch_bindings/__init__.py
+Filename: tensorrt_dispatch_bindings/
+Comment: 
+
+Filename: tensorrt_dispatch_cu12_bindings-10.0.1.dist-info/
 Comment: 
 
 Filename: tensorrt_dispatch_bindings/tensorrt_dispatch.cp39-win_amd64.pyd
 Comment: 
 
-Filename: tensorrt_dispatch_cu12_bindings-10.0.0b6.dist-info/LICENSE.txt
+Filename: tensorrt_dispatch_bindings/__init__.py
+Comment: 
+
+Filename: tensorrt_dispatch_cu12_bindings-10.0.1.dist-info/METADATA
 Comment: 
 
-Filename: tensorrt_dispatch_cu12_bindings-10.0.0b6.dist-info/METADATA
+Filename: tensorrt_dispatch_cu12_bindings-10.0.1.dist-info/zip-safe
 Comment: 
 
-Filename: tensorrt_dispatch_cu12_bindings-10.0.0b6.dist-info/WHEEL
+Filename: tensorrt_dispatch_cu12_bindings-10.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: tensorrt_dispatch_cu12_bindings-10.0.0b6.dist-info/top_level.txt
+Filename: tensorrt_dispatch_cu12_bindings-10.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: tensorrt_dispatch_cu12_bindings-10.0.0b6.dist-info/zip-safe
+Filename: tensorrt_dispatch_cu12_bindings-10.0.1.dist-info/RECORD
 Comment: 
 
-Filename: tensorrt_dispatch_cu12_bindings-10.0.0b6.dist-info/RECORD
+Filename: tensorrt_dispatch_cu12_bindings-10.0.1.dist-info/LICENSE.txt
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## tensorrt_dispatch_bindings/__init__.py

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
     }["tensorrt_dispatch"]
 
     for lib in LIBRARIES:
         lib_path = find_lib(lib)
         if lib_path != "":
             ctypes.CDLL(lib_path)
 
 del _libs_wheel_imported
 
 from .tensorrt_dispatch import *
 
-__version__ = "10.0.0b6"
+__version__ = "10.0.1"
 
 
 # Provides Python's `with` syntax
 def common_enter(this):
     warnings.warn(
         "Context managers for TensorRT types are deprecated. "
         "Memory will be freed automatically when the reference count reaches 0.",
```

## Comparing `tensorrt_dispatch_cu12_bindings-10.0.0b6.dist-info/LICENSE.txt` & `tensorrt_dispatch_cu12_bindings-10.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `tensorrt_dispatch_cu12_bindings-10.0.0b6.dist-info/METADATA` & `tensorrt_dispatch_cu12_bindings-10.0.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorrt_dispatch-cu12_bindings
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

## Comparing `tensorrt_dispatch_cu12_bindings-10.0.0b6.dist-info/RECORD` & `tensorrt_dispatch_cu12_bindings-10.0.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-tensorrt_dispatch_bindings/__init__.py,sha256=0jwipyYqqqUnqeel-eiRxO2nlU52J6n0V-LFtCZHV9k,5911
-tensorrt_dispatch_bindings/tensorrt_dispatch.cp39-win_amd64.pyd,sha256=Yy6uMgt5YDi4JsnzlVz2rApwo7c0fbx8WRrjv3brNYY,1313792
-tensorrt_dispatch_cu12_bindings-10.0.0b6.dist-info/LICENSE.txt,sha256=yGkV_ZW7773aMTWqzj5q1rRhKEbcvbxdL1o4sTndiLQ,47141
-tensorrt_dispatch_cu12_bindings-10.0.0b6.dist-info/METADATA,sha256=ccywPrsP1Ick_Vh2afzQEWf7n7fMqxdq0ZeiAaJXHpY,619
-tensorrt_dispatch_cu12_bindings-10.0.0b6.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-tensorrt_dispatch_cu12_bindings-10.0.0b6.dist-info/top_level.txt,sha256=dIWegHwo5XlKMZXLvPtu3K6OsrpieEgAVIQea2uwBtw,27
-tensorrt_dispatch_cu12_bindings-10.0.0b6.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-tensorrt_dispatch_cu12_bindings-10.0.0b6.dist-info/RECORD,,
+tensorrt_dispatch_bindings/__init__.py,sha256=sJmwkX_Tvg2n3XBuOWuWticJiyAg21_Z6xOFyB2v_zg,5924
+tensorrt_dispatch_bindings/tensorrt_dispatch.cp39-win_amd64.pyd,sha256=QSMA0aIXfQeBMriZuAjcyWJLixIj-dGUiaEqmoebylQ,1315328
+tensorrt_dispatch_cu12_bindings-10.0.1.dist-info/LICENSE.txt,sha256=yGkV_ZW7773aMTWqzj5q1rRhKEbcvbxdL1o4sTndiLQ,47141
+tensorrt_dispatch_cu12_bindings-10.0.1.dist-info/METADATA,sha256=Ud9vGxx3W537nuag9-e8pBbQnAlj8CHEj1hJYo4XftQ,617
+tensorrt_dispatch_cu12_bindings-10.0.1.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+tensorrt_dispatch_cu12_bindings-10.0.1.dist-info/top_level.txt,sha256=dIWegHwo5XlKMZXLvPtu3K6OsrpieEgAVIQea2uwBtw,27
+tensorrt_dispatch_cu12_bindings-10.0.1.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+tensorrt_dispatch_cu12_bindings-10.0.1.dist-info/RECORD,,
```

