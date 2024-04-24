# Comparing `tmp/flowkit_jwt_generator-1.24.0.post0.dev65-py3-none-any.whl.zip` & `tmp/flowkit_jwt_generator-1.24.0.post0.dev77-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8544 bytes, number of entries: 10
--rw-r--r--  2.0 unx      507 b- defN 24-Apr-23 19:24 flowkit_jwt_generator/__init__.py
--rw-r--r--  2.0 unx      510 b- defN 24-Apr-23 19:24 flowkit_jwt_generator/_version.py
--rw-r--r--  2.0 unx     1591 b- defN 24-Apr-23 19:24 flowkit_jwt_generator/cli.py
--rw-r--r--  2.0 unx     3405 b- defN 24-Apr-23 19:24 flowkit_jwt_generator/fixtures.py
--rw-r--r--  2.0 unx     9215 b- defN 24-Apr-23 19:24 flowkit_jwt_generator/jwt.py
--rw-r--r--  2.0 unx     1334 b- defN 24-Apr-23 19:24 flowkit_jwt_generator-1.24.0.post0.dev65.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-23 19:24 flowkit_jwt_generator-1.24.0.post0.dev65.dist-info/WHEEL
--rw-r--r--  2.0 unx      138 b- defN 24-Apr-23 19:24 flowkit_jwt_generator-1.24.0.post0.dev65.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 24-Apr-23 19:24 flowkit_jwt_generator-1.24.0.post0.dev65.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      967 b- defN 24-Apr-23 19:24 flowkit_jwt_generator-1.24.0.post0.dev65.dist-info/RECORD
-10 files, 17781 bytes uncompressed, 6846 bytes compressed:  61.5%
+Zip file size: 8542 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      507 b- defN 24-Apr-24 11:12 flowkit_jwt_generator/__init__.py
+-rw-r--r--  2.0 unx      510 b- defN 24-Apr-24 11:12 flowkit_jwt_generator/_version.py
+-rw-r--r--  2.0 unx     1591 b- defN 24-Apr-24 11:12 flowkit_jwt_generator/cli.py
+-rw-r--r--  2.0 unx     3405 b- defN 24-Apr-24 11:12 flowkit_jwt_generator/fixtures.py
+-rw-r--r--  2.0 unx     9215 b- defN 24-Apr-24 11:12 flowkit_jwt_generator/jwt.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-Apr-24 11:12 flowkit_jwt_generator-1.24.0.post0.dev77.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 11:12 flowkit_jwt_generator-1.24.0.post0.dev77.dist-info/WHEEL
+-rw-r--r--  2.0 unx      138 b- defN 24-Apr-24 11:12 flowkit_jwt_generator-1.24.0.post0.dev77.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-24 11:12 flowkit_jwt_generator-1.24.0.post0.dev77.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      967 b- defN 24-Apr-24 11:12 flowkit_jwt_generator-1.24.0.post0.dev77.dist-info/RECORD
+10 files, 17781 bytes uncompressed, 6844 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: flowkit_jwt_generator/fixtures.py
 Comment: 
 
 Filename: flowkit_jwt_generator/jwt.py
 Comment: 
 
-Filename: flowkit_jwt_generator-1.24.0.post0.dev65.dist-info/METADATA
+Filename: flowkit_jwt_generator-1.24.0.post0.dev77.dist-info/METADATA
 Comment: 
 
-Filename: flowkit_jwt_generator-1.24.0.post0.dev65.dist-info/WHEEL
+Filename: flowkit_jwt_generator-1.24.0.post0.dev77.dist-info/WHEEL
 Comment: 
 
-Filename: flowkit_jwt_generator-1.24.0.post0.dev65.dist-info/entry_points.txt
+Filename: flowkit_jwt_generator-1.24.0.post0.dev77.dist-info/entry_points.txt
 Comment: 
 
-Filename: flowkit_jwt_generator-1.24.0.post0.dev65.dist-info/top_level.txt
+Filename: flowkit_jwt_generator-1.24.0.post0.dev77.dist-info/top_level.txt
 Comment: 
 
-Filename: flowkit_jwt_generator-1.24.0.post0.dev65.dist-info/RECORD
+Filename: flowkit_jwt_generator-1.24.0.post0.dev77.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flowkit_jwt_generator/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2024-04-23T19:21:46+0000",
+ "date": "2024-04-24T12:09:21+0100",
  "dirty": false,
  "error": null,
- "full-revisionid": "f4a51b42c21f8c197f5abdf9f029320c948b5d82",
- "version": "1.24.0.post0.dev65"
+ "full-revisionid": "aab8fa7c9f80317aab28c722c88940f2ea9e5a21",
+ "version": "1.24.0.post0.dev77"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## Comparing `flowkit_jwt_generator-1.24.0.post0.dev65.dist-info/METADATA` & `flowkit_jwt_generator-1.24.0.post0.dev77.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowkit_jwt_generator
-Version: 1.24.0.post0.dev65
+Version: 1.24.0.post0.dev77
 Summary: Common test JWT generator for FlowKit.
 Home-page: https://github.com/Flowminder/FlowKit
 Author: Flowminder Foundation
 Author-email: flowkit@flowminder.org
 Keywords: mobile telecommunications analysis
 Platform: MacOS X
 Platform: Linux
```

## Comparing `flowkit_jwt_generator-1.24.0.post0.dev65.dist-info/RECORD` & `flowkit_jwt_generator-1.24.0.post0.dev77.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 flowkit_jwt_generator/__init__.py,sha256=Vqa2vcGLH7wfO7GXFiSQX2QXctRgwUuM-QG9DJ0HQqk,507
-flowkit_jwt_generator/_version.py,sha256=_N3pZh9sc0GT7nQq00mFaiN1gkzIdVKhnZDnkbb_2j8,510
+flowkit_jwt_generator/_version.py,sha256=R-hujpRI26r8ghiYAQ8iUPCVVyEZF1S-O1T21elC9B8,510
 flowkit_jwt_generator/cli.py,sha256=hx88rA2O7sqhQ0EHQTCVrZpcdBLW-qssaaodnpXV1DQ,1591
 flowkit_jwt_generator/fixtures.py,sha256=jVDYkagDNtu_m94ns2F6sDtqMmq1kBygS6DBaMqBGoo,3405
 flowkit_jwt_generator/jwt.py,sha256=R_IjXQwtq3eYOmEVcHp7bOCtBgoGUyUpmrJRKsp1MMc,9215
-flowkit_jwt_generator-1.24.0.post0.dev65.dist-info/METADATA,sha256=lRrEqZCkLP6fHkcDsKNsJsMp5AJj76FWLzYZn3hCXd8,1334
-flowkit_jwt_generator-1.24.0.post0.dev65.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-flowkit_jwt_generator-1.24.0.post0.dev65.dist-info/entry_points.txt,sha256=dn2fWa3YIICO8NuUzecgAhZjHJqa_hCnJkRPdwdYW5I,138
-flowkit_jwt_generator-1.24.0.post0.dev65.dist-info/top_level.txt,sha256=qNfUi5RerckeRiSkJOlGGv5098vruKE2Ck_3TbYyci4,22
-flowkit_jwt_generator-1.24.0.post0.dev65.dist-info/RECORD,,
+flowkit_jwt_generator-1.24.0.post0.dev77.dist-info/METADATA,sha256=cfV49B4sTbtAI4furaSACriC1MsQ7MeWdAJ6bwXKYvU,1334
+flowkit_jwt_generator-1.24.0.post0.dev77.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+flowkit_jwt_generator-1.24.0.post0.dev77.dist-info/entry_points.txt,sha256=dn2fWa3YIICO8NuUzecgAhZjHJqa_hCnJkRPdwdYW5I,138
+flowkit_jwt_generator-1.24.0.post0.dev77.dist-info/top_level.txt,sha256=qNfUi5RerckeRiSkJOlGGv5098vruKE2Ck_3TbYyci4,22
+flowkit_jwt_generator-1.24.0.post0.dev77.dist-info/RECORD,,
```

