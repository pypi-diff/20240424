# Comparing `tmp/zalo_sdk-0.2.5-py3-none-any.whl.zip` & `tmp/zalo_sdk-0.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,21 @@
-Zip file size: 10329 bytes, number of entries: 14
+Zip file size: 15143 bytes, number of entries: 19
+-rw-r--r--  2.0 unx       34 b- defN 24-Apr-10 19:09 test/__init__.py
+-rw-r--r--  2.0 unx      259 b- defN 24-Apr-10 19:09 test/base.py
+-rw-r--r--  2.0 unx     1779 b- defN 24-Apr-10 19:09 test/test_create_request_header.py
+-rw-r--r--  2.0 unx      522 b- defN 24-Apr-24 14:59 test/test_get_user_detail.py
+-rw-r--r--  2.0 unx    22718 b- defN 24-Apr-10 19:09 test/test_oa_create_request_body.py
 -rw-r--r--  2.0 unx     7275 b- defN 24-Apr-10 19:25 zalo_sdk/BaseClient.py
 -rw-r--r--  2.0 unx      345 b- defN 23-May-16 15:21 zalo_sdk/ZaloException.py
 -rw-r--r--  2.0 unx     2527 b- defN 24-Apr-10 19:09 zalo_sdk/ZaloOAException.py
 -rw-r--r--  2.0 unx      106 b- defN 23-May-16 15:21 zalo_sdk/__init__.py
--rw-r--r--  2.0 unx     3437 b- defN 24-Apr-10 19:25 zalo_sdk/oa/Client.py
+-rw-r--r--  2.0 unx     3827 b- defN 24-Apr-24 14:59 zalo_sdk/oa/Client.py
 -rw-r--r--  2.0 unx     5485 b- defN 24-Apr-10 19:09 zalo_sdk/oa/ZaloMessage.py
 -rw-r--r--  2.0 unx       48 b- defN 23-May-16 15:21 zalo_sdk/oa/__init__.py
 -rw-r--r--  2.0 unx     2083 b- defN 24-Apr-10 19:25 zalo_sdk/zns/Client.py
 -rw-r--r--  2.0 unx       21 b- defN 23-May-16 15:21 zalo_sdk/zns/__init__.py
--rw-r--r--  2.0 unx     1064 b- defN 24-Apr-10 19:33 zalo_sdk-0.2.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     1779 b- defN 24-Apr-10 19:33 zalo_sdk-0.2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 19:33 zalo_sdk-0.2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Apr-10 19:33 zalo_sdk-0.2.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1107 b- defN 24-Apr-10 19:33 zalo_sdk-0.2.5.dist-info/RECORD
-14 files, 25378 bytes uncompressed, 8495 bytes compressed:  66.5%
+-rw-r--r--  2.0 unx     1064 b- defN 24-Apr-24 15:00 zalo_sdk-0.2.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1779 b- defN 24-Apr-24 15:00 zalo_sdk-0.2.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 15:00 zalo_sdk-0.2.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 24-Apr-24 15:00 zalo_sdk-0.2.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1515 b- defN 24-Apr-24 15:00 zalo_sdk-0.2.6.dist-info/RECORD
+19 files, 51493 bytes uncompressed, 12679 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -1,7 +1,22 @@
+Filename: test/__init__.py
+Comment: 
+
+Filename: test/base.py
+Comment: 
+
+Filename: test/test_create_request_header.py
+Comment: 
+
+Filename: test/test_get_user_detail.py
+Comment: 
+
+Filename: test/test_oa_create_request_body.py
+Comment: 
+
 Filename: zalo_sdk/BaseClient.py
 Comment: 
 
 Filename: zalo_sdk/ZaloException.py
 Comment: 
 
 Filename: zalo_sdk/ZaloOAException.py
@@ -21,23 +36,23 @@
 
 Filename: zalo_sdk/zns/Client.py
 Comment: 
 
 Filename: zalo_sdk/zns/__init__.py
 Comment: 
 
-Filename: zalo_sdk-0.2.5.dist-info/LICENSE
+Filename: zalo_sdk-0.2.6.dist-info/LICENSE
 Comment: 
 
-Filename: zalo_sdk-0.2.5.dist-info/METADATA
+Filename: zalo_sdk-0.2.6.dist-info/METADATA
 Comment: 
 
-Filename: zalo_sdk-0.2.5.dist-info/WHEEL
+Filename: zalo_sdk-0.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: zalo_sdk-0.2.5.dist-info/top_level.txt
+Filename: zalo_sdk-0.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: zalo_sdk-0.2.5.dist-info/RECORD
+Filename: zalo_sdk-0.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zalo_sdk/oa/Client.py

```diff
@@ -71,14 +71,25 @@
         }
         url = f"{self.endpoint_prefix}/v2.0/oa/getprofile"
         response = self.send_request(
             method="GET", url=url, body=params, headers=headers
         )
         return self._validate_zalo_response(response)
     
+    def get_user_detail(self, user_id):
+        headers = self.create_request_header(method="GET")
+        params = {
+            "user_id": user_id
+        }
+        url = f"{self.endpoint_prefix}/v3.0/oa/user/detail"
+        response = self.send_request(
+            method="GET", url=url, body=params, headers=headers
+        )
+        return self._validate_zalo_response(response)
+    
     def _validate_zalo_response(self, response):
         self.check_http_error(response)
 
         zalo_response = response.json()
         self.check_zalo_oa_error(zalo_response)
         return zalo_response
```

## Comparing `zalo_sdk-0.2.5.dist-info/LICENSE` & `zalo_sdk-0.2.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zalo_sdk-0.2.5.dist-info/METADATA` & `zalo_sdk-0.2.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zalo_sdk
-Version: 0.2.5
+Version: 0.2.6
 Summary: Zalo SDK
 Home-page: https://github.com/connext-biz/zalo_integration
 Author: Khoa Tran
 Author-email: khoa@connext.biz
 License: MIT License
         
         Copyright (c) 2023 Connext
```

