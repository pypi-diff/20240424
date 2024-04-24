# Comparing `tmp/codeproject_ai_sdk-0.0.2-py3-none-any.whl.zip` & `tmp/codeproject_ai_sdk-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 40992 bytes, number of entries: 16
+Zip file size: 41000 bytes, number of entries: 16
 -rw-rw-rw-  2.0 fat      337 b- defN 24-Apr-23 16:11 codeproject_ai_sdk/__init__.py
 -rw-rw-rw-  2.0 fat     4745 b- defN 24-Mar-19 15:28 codeproject_ai_sdk/common.py
 -rw-rw-rw-  2.0 fat    14191 b- defN 24-Apr-23 15:10 codeproject_ai_sdk/module_logging.py
 -rw-rw-rw-  2.0 fat     5209 b- defN 24-Apr-23 14:59 codeproject_ai_sdk/module_options.py
 -rw-rw-rw-  2.0 fat    61486 b- defN 24-Apr-23 14:59 codeproject_ai_sdk/module_runner.py
 -rw-rw-rw-  2.0 fat     9686 b- defN 24-Apr-23 14:55 codeproject_ai_sdk/request_data.py
 -rw-rw-rw-  2.0 fat    14686 b- defN 24-Apr-22 15:48 codeproject_ai_sdk/system_info.py
 -rw-rw-rw-  2.0 fat     8344 b- defN 24-Mar-19 15:28 codeproject_ai_sdk/training/augmentation.py
 -rw-rw-rw-  2.0 fat      328 b- defN 24-Apr-23 16:30 codeproject_ai_sdk/utils/__init__.py
 -rw-rw-rw-  2.0 fat    26205 b- defN 24-Mar-19 15:28 codeproject_ai_sdk/utils/cpuinfo.py
 -rw-rw-rw-  2.0 fat     2746 b- defN 24-Mar-19 15:28 codeproject_ai_sdk/utils/environment_check.py
 -rw-rw-rw-  2.0 fat     1419 b- defN 24-Mar-19 15:28 codeproject_ai_sdk/utils/image_utils.py
--rw-rw-rw-  2.0 fat      934 b- defN 24-Apr-23 19:41 codeproject_ai_sdk-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-23 19:41 codeproject_ai_sdk-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       19 b- defN 24-Apr-23 19:41 codeproject_ai_sdk-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1457 b- defN 24-Apr-23 19:41 codeproject_ai_sdk-0.0.2.dist-info/RECORD
-16 files, 151884 bytes uncompressed, 38550 bytes compressed:  74.6%
+-rw-rw-rw-  2.0 fat      985 b- defN 24-Apr-23 21:30 codeproject_ai_sdk-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-23 21:30 codeproject_ai_sdk-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       19 b- defN 24-Apr-23 21:30 codeproject_ai_sdk-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1457 b- defN 24-Apr-23 21:30 codeproject_ai_sdk-0.0.3.dist-info/RECORD
+16 files, 151935 bytes uncompressed, 38558 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: codeproject_ai_sdk/utils/environment_check.py
 Comment: 
 
 Filename: codeproject_ai_sdk/utils/image_utils.py
 Comment: 
 
-Filename: codeproject_ai_sdk-0.0.2.dist-info/METADATA
+Filename: codeproject_ai_sdk-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: codeproject_ai_sdk-0.0.2.dist-info/WHEEL
+Filename: codeproject_ai_sdk-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: codeproject_ai_sdk-0.0.2.dist-info/top_level.txt
+Filename: codeproject_ai_sdk-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: codeproject_ai_sdk-0.0.2.dist-info/RECORD
+Filename: codeproject_ai_sdk-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `codeproject_ai_sdk-0.0.2.dist-info/METADATA` & `codeproject_ai_sdk-0.0.3.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: codeproject-ai-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python SDK for writing Modules for CodeProject AI Server
 Author: Chris Maunder, Matthew Dennis
 License: SSPL
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: Pillow
 Requires-Dist: charset-normalizer
 Requires-Dist: aiohttp
 Requires-Dist: aiofiles
 Requires-Dist: py-cpuinfo
 Requires-Dist: GPUtil
```

## Comparing `codeproject_ai_sdk-0.0.2.dist-info/RECORD` & `codeproject_ai_sdk-0.0.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 codeproject_ai_sdk/request_data.py,sha256=qjfG4bIK53itOhV_fC2iGM6sZQp5eURjArUife_15lg,9686
 codeproject_ai_sdk/system_info.py,sha256=_dJ3VeDItdN2yz-j_1uCARnz-A1N3SKN0-lsrzxGWQ0,14686
 codeproject_ai_sdk/training/augmentation.py,sha256=owzuW0FtAJikU2nfRFhO9TLDdNjJtN57FL-1ka5ilnI,8344
 codeproject_ai_sdk/utils/__init__.py,sha256=iJxF8ROEpDlnUDMb61p3LFPWyHx1NR3ix1nzv3_umKo,328
 codeproject_ai_sdk/utils/cpuinfo.py,sha256=Y2_khkb6FPiqzVoFy1olM-Kz8kDhc7CwKXyYohAU7PI,26205
 codeproject_ai_sdk/utils/environment_check.py,sha256=dLEnaXX5AlMNGRnSPRWlLniHqiyF1VJZSJAnLE6TxsE,2746
 codeproject_ai_sdk/utils/image_utils.py,sha256=IVa7x8u22VV89XJoYKR-iXMXqATDzNiDQEGV46MqSrc,1419
-codeproject_ai_sdk-0.0.2.dist-info/METADATA,sha256=RpPLoAxLOyk_M4IaoNAvEB4R-07gLDq4K8I4TZfXpug,934
-codeproject_ai_sdk-0.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-codeproject_ai_sdk-0.0.2.dist-info/top_level.txt,sha256=Nv5ufBe4VOyLmSTbCJjYnM6L-0bnqnSlpxtqG0GE064,19
-codeproject_ai_sdk-0.0.2.dist-info/RECORD,,
+codeproject_ai_sdk-0.0.3.dist-info/METADATA,sha256=_75lywopI3HBNvHFCoBPuri_7SVYSHh1CXVEXAv7plY,985
+codeproject_ai_sdk-0.0.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+codeproject_ai_sdk-0.0.3.dist-info/top_level.txt,sha256=Nv5ufBe4VOyLmSTbCJjYnM6L-0bnqnSlpxtqG0GE064,19
+codeproject_ai_sdk-0.0.3.dist-info/RECORD,,
```

