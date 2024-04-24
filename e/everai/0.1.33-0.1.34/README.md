# Comparing `tmp/everai-0.1.33-py3-none-any.whl.zip` & `tmp/everai-0.1.34-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 418127 bytes, number of entries: 400
+Zip file size: 418148 bytes, number of entries: 400
 -rw-r--r--  2.0 unx       66 b- defN 24-Apr-24 07:43 everai/__init__.py
--rw-r--r--  2.0 unx     1077 b- defN 24-Apr-17 09:14 everai/constants.py
--rw-r--r--  2.0 unx       22 b- defN 24-Apr-24 07:44 everai/version.py
+-rw-r--r--  2.0 unx     1111 b- defN 24-Apr-24 07:49 everai/constants.py
+-rw-r--r--  2.0 unx       23 b- defN 24-Apr-24 07:52 everai/version.py
 -rw-r--r--  2.0 unx       40 b- defN 24-Mar-15 10:09 everai/api/__init__.py
 -rw-r--r--  2.0 unx    14055 b- defN 24-Apr-23 15:30 everai/api/api.py
 -rw-r--r--  2.0 unx      208 b- defN 24-Apr-15 11:24 everai/app/__init__.py
 -rw-r--r--  2.0 unx     3667 b- defN 24-Apr-23 15:20 everai/app/app.py
--rw-r--r--  2.0 unx    11071 b- defN 24-Apr-24 07:42 everai/app/app_manager.py
+-rw-r--r--  2.0 unx    11070 b- defN 24-Apr-24 07:48 everai/app/app_manager.py
 -rw-r--r--  2.0 unx     1791 b- defN 24-Apr-24 07:37 everai/app/app_runner.py
 -rw-r--r--  2.0 unx     3223 b- defN 24-Apr-24 05:08 everai/app/app_runtime.py
 -rw-r--r--  2.0 unx     2568 b- defN 24-Apr-23 14:51 everai/app/app_setup.py
 -rw-r--r--  2.0 unx     1116 b- defN 24-Apr-24 04:14 everai/app/autocaling_handler.py
 -rw-r--r--  2.0 unx     2320 b- defN 24-Apr-23 14:26 everai/app/context.py
 -rw-r--r--  2.0 unx     2965 b- defN 24-Apr-23 09:42 everai/app/service.py
 -rw-r--r--  2.0 unx      210 b- defN 24-Mar-28 12:25 everai/app/typing.py
@@ -389,14 +389,14 @@
 -rw-r--r--  2.0 unx     1912 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_commit_file_body_file.py
 -rw-r--r--  2.0 unx     2548 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_commit_revision_body.py
 -rw-r--r--  2.0 unx     2233 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_complete_multipart_upload_body.py
 -rw-r--r--  2.0 unx     1624 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_create_body.py
 -rw-r--r--  2.0 unx     2149 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_initialize_multipart_upload_body.py
 -rw-r--r--  2.0 unx     1769 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_sign_multipart_upload_body.py
 -rw-r--r--  2.0 unx     1968 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_sign_upload_body.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 07:45 everai-0.1.33.dist-info/LICENSE
--rw-r--r--  2.0 unx     1951 b- defN 24-Apr-24 07:45 everai-0.1.33.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 07:45 everai-0.1.33.dist-info/WHEEL
--rw-r--r--  2.0 unx       98 b- defN 24-Apr-24 07:45 everai-0.1.33.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-24 07:45 everai-0.1.33.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    39817 b- defN 24-Apr-24 07:45 everai-0.1.33.dist-info/RECORD
-400 files, 1289055 bytes uncompressed, 353327 bytes compressed:  72.6%
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 07:53 everai-0.1.34.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1951 b- defN 24-Apr-24 07:53 everai-0.1.34.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 07:53 everai-0.1.34.dist-info/WHEEL
+-rw-r--r--  2.0 unx       98 b- defN 24-Apr-24 07:53 everai-0.1.34.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-24 07:53 everai-0.1.34.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    39817 b- defN 24-Apr-24 07:53 everai-0.1.34.dist-info/RECORD
+400 files, 1289089 bytes uncompressed, 353348 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -1176,26 +1176,26 @@
 
 Filename: generated/volumes/test/test_volume_service_sign_multipart_upload_body.py
 Comment: 
 
 Filename: generated/volumes/test/test_volume_service_sign_upload_body.py
 Comment: 
 
-Filename: everai-0.1.33.dist-info/LICENSE
+Filename: everai-0.1.34.dist-info/LICENSE
 Comment: 
 
-Filename: everai-0.1.33.dist-info/METADATA
+Filename: everai-0.1.34.dist-info/METADATA
 Comment: 
 
-Filename: everai-0.1.33.dist-info/WHEEL
+Filename: everai-0.1.34.dist-info/WHEEL
 Comment: 
 
-Filename: everai-0.1.33.dist-info/entry_points.txt
+Filename: everai-0.1.34.dist-info/entry_points.txt
 Comment: 
 
-Filename: everai-0.1.33.dist-info/top_level.txt
+Filename: everai-0.1.34.dist-info/top_level.txt
 Comment: 
 
-Filename: everai-0.1.33.dist-info/RECORD
+Filename: everai-0.1.34.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## everai/constants.py

```diff
@@ -2,15 +2,17 @@
 import sys
 
 from everai.utils.bool import str_to_bool
 from dotenv import load_dotenv
 
 load_dotenv('.env')
 
-EVERAI_ENDPOINT = os.getenv('EVERAI_ENDPOINT') or 'https://hub.everai.com'
+MAIN_SITE = 'everai.expvent.com'
+
+EVERAI_ENDPOINT = os.getenv('EVERAI_ENDPOINT') or f'https://{MAIN_SITE}'
 
 default_home = os.path.join(os.path.expanduser("~"), '.cache')
 
 EVERAI_HOME = os.path.expanduser(
     os.getenv(
         'EVERAI_HOME',
         os.path.join(
```

## everai/version.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.33"
+__version__ = "0.1.34"
```

## everai/app/app_manager.py

```diff
@@ -33,15 +33,15 @@
 from generated.volumes.exceptions import NotFoundException as VolumeNotFoundException
 
 autoscaling_warning = """
 You are deploying an app without autoscaling_policy, 
 that will cause the app to run only one worker and always one worker,
 if you want to setup an autoscaling_policy for this app after deploy,
 you cloud run command everai app upgrade <your app name> --autoscaling-policy,
-or setup in your dashboard, www.evermachine.com
+or setup in your dashboard, everai.expvent.com
 """
 
 
 class AppManager:
     def __init__(self):
         self.api = API()
         self.secret_manager = SecretManager()
```

## Comparing `everai-0.1.33.dist-info/METADATA` & `everai-0.1.34.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everai
-Version: 0.1.33
+Version: 0.1.34
 Summary: Client library to manage everai infrastructure
 Author-email: mc <mc@expvent.com>
 Maintainer-email: mc <mc@expvent.com>
 Project-URL: Homepage, https://everai.expvent.com
 Project-URL: Documentation, https://everai.expvent.com
 Project-URL: Repository, https://github.com/expvent/everai
 Project-URL: Issues, https://github.com/expvent/everai/issues
```

## Comparing `everai-0.1.33.dist-info/RECORD` & `everai-0.1.34.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 everai/__init__.py,sha256=AbgR3tVRy6TETgwXyJITEnET1TSFpEAEqQJJqzReYqQ,66
-everai/constants.py,sha256=GfhnCcPgJXJyTMWAuQWszwSxsrb3yYZiFFoQGvA5x7s,1077
-everai/version.py,sha256=-w_wSS_K7mBDaL2ciGoQ17Ab9V3-ElRGvc4UASK1hFI,22
+everai/constants.py,sha256=bZuLnYDxayThik9UU4eABKRjrp6fHw5vT14gNR2LpF8,1111
+everai/version.py,sha256=79r5jd-MqbhXLbIBDVBqUJvhvcucjkaId96r46KF18I,23
 everai/api/__init__.py,sha256=2WLrQ_PpJ35__yOVHC89MhILujyGioyaGir-5n6hxCc,40
 everai/api/api.py,sha256=HKMYo37SZxQo-aeqrIA5S0AKKoxGxkKhhejXBR3-y2o,14055
 everai/app/__init__.py,sha256=A-USWcj6TDAW_hxG6wT3Qb8m3d5Tq733WWC9McNhlGI,208
 everai/app/app.py,sha256=fweD6GNTR0vCCFvYDXSzZOIcphOEhM5nOlcXDA_kB3M,3667
-everai/app/app_manager.py,sha256=CxR8fGvgIaWlryiLUQltv1qScG5KARn9RclMLMfprio,11071
+everai/app/app_manager.py,sha256=SbDljStWdJSImjG6yIaA4KwUeU3G1NhfUmofrXXfRUE,11070
 everai/app/app_runner.py,sha256=HVlOLweFX-C2kBbgyVwuDz4vfGzQ6uzHpNVzikQhRfA,1791
 everai/app/app_runtime.py,sha256=zyj63A6VfM1P3WL7LVW_mcy9xmMwKueKzTcJduGMwSo,3223
 everai/app/app_setup.py,sha256=CLXAC83OyTqEjAEKNLHQaCT3UPhvw149mD1VQr-AEEg,2568
 everai/app/autocaling_handler.py,sha256=Exsdti0N16GlcqXIILJ1qa6_DN9cBwzWpahukDKiqEo,1116
 everai/app/context.py,sha256=BIZ0FOozDTVCZg-cWMUnpf9DEjKF2r5T1MRF8yWreG4,2320
 everai/app/service.py,sha256=tn202UvWjK3Zr34MTQB_XhrGwXYe-NqgQtdTFncrgYk,2965
 everai/app/typing.py,sha256=d7tPA7VoDY771u-v0DLwD6TTMfPotg8u_PAshDcHRQo,210
@@ -388,13 +388,13 @@
 generated/volumes/test/test_volume_service_commit_file_body_file.py,sha256=F4jWVTlpo82x5j68w3hYpaHvaUZhCiFrmBSo1SVZOu0,1912
 generated/volumes/test/test_volume_service_commit_revision_body.py,sha256=UizO6O0rY4b9isgc_d2lKBUwTlCn0kiefccAD86nCcs,2548
 generated/volumes/test/test_volume_service_complete_multipart_upload_body.py,sha256=Ek6ZP78kDn1ol-guEmhm2zA42c_6XkArQf8G-_L5MgI,2233
 generated/volumes/test/test_volume_service_create_body.py,sha256=2MA4PEVNwPpMGuvpwMu4qeYvDAjrZjyUaeuo9p3qJ1c,1624
 generated/volumes/test/test_volume_service_initialize_multipart_upload_body.py,sha256=G58739S9489bMEXfaefcWch_GqgV-PTw4QCewOzxhSs,2149
 generated/volumes/test/test_volume_service_sign_multipart_upload_body.py,sha256=3b5ULrWgH38nEWU0s_MISEyj4j6LV8doFAx3CfQ6XjY,1769
 generated/volumes/test/test_volume_service_sign_upload_body.py,sha256=xX2B1LCvIu0OHX0AkyL8dXPClBTDgmZwmgPJOjjz96g,1968
-everai-0.1.33.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-everai-0.1.33.dist-info/METADATA,sha256=-SQWRu8K_UjD5YeBrufESVWBSQ14jO3tZNfTLi6xQC8,1951
-everai-0.1.33.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-everai-0.1.33.dist-info/entry_points.txt,sha256=JB8rwg4N4ctezo4f9O0QbWJkivM_s-wUhOn0mPM9xug,98
-everai-0.1.33.dist-info/top_level.txt,sha256=UNE90t4nA-FVpeYLiqPcJVSFyaKbZ-ERHUNI0Qd6co8,17
-everai-0.1.33.dist-info/RECORD,,
+everai-0.1.34.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+everai-0.1.34.dist-info/METADATA,sha256=_qCbgJAsNzEKzgXkyEwseptWbbbL_GbfuY0wXJFzn1o,1951
+everai-0.1.34.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+everai-0.1.34.dist-info/entry_points.txt,sha256=JB8rwg4N4ctezo4f9O0QbWJkivM_s-wUhOn0mPM9xug,98
+everai-0.1.34.dist-info/top_level.txt,sha256=UNE90t4nA-FVpeYLiqPcJVSFyaKbZ-ERHUNI0Qd6co8,17
+everai-0.1.34.dist-info/RECORD,,
```

