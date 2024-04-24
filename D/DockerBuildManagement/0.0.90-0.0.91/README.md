# Comparing `tmp/DockerBuildManagement-0.0.90-py2.py3-none-any.whl.zip` & `tmp/DockerBuildManagement-0.0.91-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 19107 bytes, number of entries: 17
+Zip file size: 19105 bytes, number of entries: 17
 -rwxrwxrwx  2.0 unx     3057 b- defN 24-Feb-23 12:11 DockerBuildManagement/BuildManager.py
 -rwxrwxrwx  2.0 unx     3872 b- defN 24-Feb-23 12:11 DockerBuildManagement/BuildSelections.py
 -rwxrwxrwx  2.0 unx     4569 b- defN 24-Feb-23 12:11 DockerBuildManagement/BuildTools.py
 -rwxrwxrwx  2.0 unx     2193 b- defN 24-Feb-23 12:11 DockerBuildManagement/ChangelogSelections.py
 -rwxrwxrwx  2.0 unx     4235 b- defN 24-Feb-23 12:11 DockerBuildManagement/PromoteSelections.py
 -rwxrwxrwx  2.0 unx     5165 b- defN 24-Feb-23 12:11 DockerBuildManagement/PublishSelections.py
 -rwxrwxrwx  2.0 unx     3976 b- defN 24-Feb-23 12:11 DockerBuildManagement/RunSelections.py
 -rwxrwxrwx  2.0 unx     5288 b- defN 24-Feb-23 14:57 DockerBuildManagement/SwarmSelections.py
 -rwxrwxrwx  2.0 unx     3735 b- defN 24-Feb-23 12:11 DockerBuildManagement/TestSelections.py
 -rwxrwxrwx  2.0 unx      241 b- defN 24-Feb-23 12:11 DockerBuildManagement/__init__.py
 -rwxrwxrwx  2.0 unx      241 b- defN 24-Feb-23 12:11 DockerBuildManagement/__main__.py
--rwxrwxrwx  2.0 unx     1094 b- defN 24-Feb-23 14:58 DockerBuildManagement-0.0.90.dist-info/LICENSE
--rwxrwxrwx  2.0 unx    15291 b- defN 24-Feb-23 14:58 DockerBuildManagement-0.0.90.dist-info/METADATA
--rwxrwxrwx  2.0 unx      110 b- defN 24-Feb-23 14:58 DockerBuildManagement-0.0.90.dist-info/WHEEL
--rwxrwxrwx  2.0 unx      103 b- defN 24-Feb-23 14:58 DockerBuildManagement-0.0.90.dist-info/entry_points.txt
--rwxrwxrwx  2.0 unx       22 b- defN 24-Feb-23 14:58 DockerBuildManagement-0.0.90.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1622 b- defN 24-Feb-23 14:58 DockerBuildManagement-0.0.90.dist-info/RECORD
-17 files, 54814 bytes uncompressed, 16369 bytes compressed:  70.1%
+-rwxrwxrwx  2.0 unx     1094 b- defN 24-Apr-24 12:07 DockerBuildManagement-0.0.91.dist-info/LICENSE
+-rwxrwxrwx  2.0 unx    15291 b- defN 24-Apr-24 12:07 DockerBuildManagement-0.0.91.dist-info/METADATA
+-rwxrwxrwx  2.0 unx      110 b- defN 24-Apr-24 12:07 DockerBuildManagement-0.0.91.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx      103 b- defN 24-Apr-24 12:07 DockerBuildManagement-0.0.91.dist-info/entry_points.txt
+-rwxrwxrwx  2.0 unx       22 b- defN 24-Apr-24 12:07 DockerBuildManagement-0.0.91.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1622 b- defN 24-Apr-24 12:07 DockerBuildManagement-0.0.91.dist-info/RECORD
+17 files, 54814 bytes uncompressed, 16367 bytes compressed:  70.1%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: DockerBuildManagement/__init__.py
 Comment: 
 
 Filename: DockerBuildManagement/__main__.py
 Comment: 
 
-Filename: DockerBuildManagement-0.0.90.dist-info/LICENSE
+Filename: DockerBuildManagement-0.0.91.dist-info/LICENSE
 Comment: 
 
-Filename: DockerBuildManagement-0.0.90.dist-info/METADATA
+Filename: DockerBuildManagement-0.0.91.dist-info/METADATA
 Comment: 
 
-Filename: DockerBuildManagement-0.0.90.dist-info/WHEEL
+Filename: DockerBuildManagement-0.0.91.dist-info/WHEEL
 Comment: 
 
-Filename: DockerBuildManagement-0.0.90.dist-info/entry_points.txt
+Filename: DockerBuildManagement-0.0.91.dist-info/entry_points.txt
 Comment: 
 
-Filename: DockerBuildManagement-0.0.90.dist-info/top_level.txt
+Filename: DockerBuildManagement-0.0.91.dist-info/top_level.txt
 Comment: 
 
-Filename: DockerBuildManagement-0.0.90.dist-info/RECORD
+Filename: DockerBuildManagement-0.0.91.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `DockerBuildManagement-0.0.90.dist-info/LICENSE` & `DockerBuildManagement-0.0.91.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `DockerBuildManagement-0.0.90.dist-info/METADATA` & `DockerBuildManagement-0.0.91.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DockerBuildManagement
-Version: 0.0.90
+Version: 0.0.91
 Summary: A library for managing a build system with Docker.
 Home-page: https://github.com/hansehe/DockerBuildManagement
 Author: Hans Erik Heggem
 Author-email: hans.erik.heggem@gmail.com
 License: UNKNOWN
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, http://saythanks.io/to/example
@@ -19,16 +19,16 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: DockerBuildSystem (>=1.1.59)
-Requires-Dist: SwarmManagement (>=1.1.76)
+Requires-Dist: DockerBuildSystem (>=1.1.60)
+Requires-Dist: SwarmManagement (>=1.1.77)
 Provides-Extra: dev
 Requires-Dist: check-manifest ; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: coverage ; extra == 'test'
 
 # Docker Build Management
```

## Comparing `DockerBuildManagement-0.0.90.dist-info/RECORD` & `DockerBuildManagement-0.0.91.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -5,13 +5,13 @@
 DockerBuildManagement/PromoteSelections.py,sha256=sxlGkl2HKgX0wC1gCsr8P51s0PzXFfj6OZtKqOvX5xk,4235
 DockerBuildManagement/PublishSelections.py,sha256=oeECOtlPEvDTjI2IUZREoL35mf_MzSF_Z_T64Mn2OPw,5165
 DockerBuildManagement/RunSelections.py,sha256=pyEePrMwHWxZXk2fQ0G9LqOYBKjMVl748SXbGVd8Wsc,3976
 DockerBuildManagement/SwarmSelections.py,sha256=xGdn-nWVZ0KaHp-TQw7XHoBbcL8EzknhfnhiBhTEp_o,5288
 DockerBuildManagement/TestSelections.py,sha256=lg_3xVekGW-fVaOC-_f_X2Q9wfdU0RkZnNxu7e1UanI,3735
 DockerBuildManagement/__init__.py,sha256=4fwFlV6Y1n6k9vHc8j6OycOO8iB_IvM-NCi_pm9Yaec,241
 DockerBuildManagement/__main__.py,sha256=4fwFlV6Y1n6k9vHc8j6OycOO8iB_IvM-NCi_pm9Yaec,241
-DockerBuildManagement-0.0.90.dist-info/LICENSE,sha256=KSs7LHWHTRtrUpF081-excLTyptQFdFh2cQc-tNw_CI,1094
-DockerBuildManagement-0.0.90.dist-info/METADATA,sha256=qqwNDTNsfRTpCi5bXqWLZNwQN-BUhHjlG3XCpIKy9kI,15291
-DockerBuildManagement-0.0.90.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-DockerBuildManagement-0.0.90.dist-info/entry_points.txt,sha256=CG0PMIlKlBxBYYaicMgPZ3Q6eeFPlfUGrT7YpxcfzFU,103
-DockerBuildManagement-0.0.90.dist-info/top_level.txt,sha256=ouCn2WJqnE10AJtk80ukTFv6h_S2ydJ82juFz50nlk8,22
-DockerBuildManagement-0.0.90.dist-info/RECORD,,
+DockerBuildManagement-0.0.91.dist-info/LICENSE,sha256=KSs7LHWHTRtrUpF081-excLTyptQFdFh2cQc-tNw_CI,1094
+DockerBuildManagement-0.0.91.dist-info/METADATA,sha256=uIaFNXskzH2u_8tL6rb-kqjhE_sRwm3GH7_YcC_xFN4,15291
+DockerBuildManagement-0.0.91.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+DockerBuildManagement-0.0.91.dist-info/entry_points.txt,sha256=CG0PMIlKlBxBYYaicMgPZ3Q6eeFPlfUGrT7YpxcfzFU,103
+DockerBuildManagement-0.0.91.dist-info/top_level.txt,sha256=ouCn2WJqnE10AJtk80ukTFv6h_S2ydJ82juFz50nlk8,22
+DockerBuildManagement-0.0.91.dist-info/RECORD,,
```

