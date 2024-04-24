# Comparing `tmp/cryptonets_python_sdk-1.2.2.tar.gz` & `tmp/cryptonets_python_sdk-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptonets_python_sdk-1.2.2.tar", last modified: Mon Apr 15 21:48:07 2024, max compression
+gzip compressed data, was "cryptonets_python_sdk-1.2.3.tar", last modified: Wed Apr 24 15:48:49 2024, max compression
```

## Comparing `cryptonets_python_sdk-1.2.2.tar` & `cryptonets_python_sdk-1.2.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2023-09-26 12:09:24.000000 cryptonets_python_sdk-1.2.2/LICENSE
--rw-rw-r--   0 azam      (1000) azam      (1000)       28 2023-09-26 12:09:24.000000 cryptonets_python_sdk-1.2.2/MANIFEST.in
--rw-rw-r--   0 azam      (1000) azam      (1000)     3625 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/PKG-INFO
--rw-rw-r--   0 azam      (1000) azam      (1000)     2511 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/README.md
--rw-rw-r--   0 azam      (1000) azam      (1000)       38 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/setup.cfg
--rw-rw-r--   0 azam      (1000) azam      (1000)     3798 2024-04-15 21:47:15.000000 cryptonets_python_sdk-1.2.2/setup.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-15 21:48:07.439253 cryptonets_python_sdk-1.2.2/src/
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)    31186 2024-04-08 11:43:05.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/factor.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/factor_modules/
--rw-rw-r--   0 azam      (1000) azam      (1000)    17344 2024-04-15 21:47:15.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/factor_modules/FaceModule.py
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/factor_modules/__init__.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/handler/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/handler/__init__.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/handler/lib/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/handler/lib/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)    44098 2024-04-15 21:47:15.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/handler/nativeMethods.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     3060 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/decorators.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     2964 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/messages.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     3293 2024-04-08 11:44:23.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/compareResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)      664 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/deleteResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     2946 2024-03-20 07:33:12.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/enrollPredictResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     1575 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/faceObjectResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     1463 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/faceValidationResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     2228 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/isoFaceResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     4641 2024-04-15 21:47:15.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/utils.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/settings/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/settings/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)      239 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/settings/cacheType.py
--rw-rw-r--   0 azam      (1000) azam      (1000)    16918 2024-04-12 17:30:20.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/settings/configuration.py
--rw-rw-r--   0 azam      (1000) azam      (1000)      298 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/settings/loggingLevel.py
--rw-rw-r--   0 azam      (1000) azam      (1000)      113 2024-04-12 17:30:20.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/settings/supportedPlatforms.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk.egg-info/
--rw-rw-r--   0 azam      (1000) azam      (1000)     3625 2024-04-15 21:48:07.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 azam      (1000) azam      (1000)     1544 2024-04-15 21:48:07.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 azam      (1000) azam      (1000)        1 2024-04-15 21:48:07.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 azam      (1000) azam      (1000)       48 2024-04-15 21:48:07.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk.egg-info/requires.txt
--rw-rw-r--   0 azam      (1000) azam      (1000)       22 2024-04-15 21:48:07.000000 cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-15 21:48:07.443253 cryptonets_python_sdk-1.2.2/tests/
--rw-rw-r--   0 azam      (1000) azam      (1000)    19957 2024-04-15 21:47:15.000000 cryptonets_python_sdk-1.2.2/tests/test.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     8913 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.2/tests/test_suite.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-24 15:48:49.137714 cryptonets_python_sdk-1.2.3/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2023-09-26 12:09:24.000000 cryptonets_python_sdk-1.2.3/LICENSE
+-rw-rw-r--   0 azam      (1000) azam      (1000)       28 2023-09-26 12:09:24.000000 cryptonets_python_sdk-1.2.3/MANIFEST.in
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3625 2024-04-24 15:48:49.137714 cryptonets_python_sdk-1.2.3/PKG-INFO
+-rw-rw-r--   0 azam      (1000) azam      (1000)     2511 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/README.md
+-rw-rw-r--   0 azam      (1000) azam      (1000)       38 2024-04-24 15:48:49.137714 cryptonets_python_sdk-1.2.3/setup.cfg
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3798 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.2.3/setup.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-24 15:48:49.133714 cryptonets_python_sdk-1.2.3/src/
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-24 15:48:49.133714 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)    31186 2024-04-08 11:43:05.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/factor.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-24 15:48:49.133714 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/factor_modules/
+-rw-rw-r--   0 azam      (1000) azam      (1000)    19933 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/factor_modules/FaceModule.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/factor_modules/__init__.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-24 15:48:49.137714 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/handler/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/handler/__init__.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-24 15:48:49.137714 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/handler/lib/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/handler/lib/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)    44485 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/handler/nativeMethods.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-24 15:48:49.137714 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3060 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/decorators.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3383 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/messages.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-24 15:48:49.137714 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3293 2024-04-08 11:44:23.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/compareResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)      664 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/deleteResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     2946 2024-03-20 07:33:12.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/enrollPredictResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     1575 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/faceObjectResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     1463 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/faceValidationResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     2228 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/isoFaceResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     4476 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/utils.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-24 15:48:49.137714 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/settings/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/settings/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)      239 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/settings/cacheType.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)    16918 2024-04-12 17:30:20.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/settings/configuration.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)      298 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/settings/loggingLevel.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)      113 2024-04-12 17:30:20.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/settings/supportedPlatforms.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-24 15:48:49.133714 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk.egg-info/
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3625 2024-04-24 15:48:48.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 azam      (1000) azam      (1000)     1544 2024-04-24 15:48:49.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 azam      (1000) azam      (1000)        1 2024-04-24 15:48:48.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 azam      (1000) azam      (1000)       48 2024-04-24 15:48:48.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk.egg-info/requires.txt
+-rw-rw-r--   0 azam      (1000) azam      (1000)       22 2024-04-24 15:48:48.000000 cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-04-24 15:48:49.137714 cryptonets_python_sdk-1.2.3/tests/
+-rw-rw-r--   0 azam      (1000) azam      (1000)    19957 2024-04-15 21:47:15.000000 cryptonets_python_sdk-1.2.3/tests/test.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     8913 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.2.3/tests/test_suite.py
```

### Comparing `cryptonets_python_sdk-1.2.2/PKG-INFO` & `cryptonets_python_sdk-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptonets_python_sdk
-Version: 1.2.2
+Version: 1.2.3
 Summary: Cryptonets SDK Library for Python
 Home-page: https://privateid.com/
 Author: Private Identity
 Author-email: support@private.id
 Project-URL: Bug Reports, https://github.com/prividentity/cryptonets-python-sdk/issues
 Project-URL: Source, https://github.com/prividentity/cryptonets-python-sdk
 Project-URL: Documentation, https://docs.private.id/cryptonets-python-sdk/index.html
```

### Comparing `cryptonets_python_sdk-1.2.2/README.md` & `cryptonets_python_sdk-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.2/setup.py` & `cryptonets_python_sdk-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 @author: Private Identity
 """
 NAME = "cryptonets_python_sdk"
 DESCRIPTION = "Cryptonets SDK Library for Python"
 AUTHOR = "Private Identity"
 AUTHOR_EMAIL = "support@private.id"
 URL = "https://privateid.com/"
-VERSION = "1.2.2"
+VERSION = "1.2.3"
 REQUIRES = ["numpy >= 1.21.0", "pillow >= 9.1.0","boto3","tqdm","exifread"]
 
 LONG_DESCRIPTION = ""
 if os.path.exists("./README.md"):
     with open("README.md", encoding="utf-8") as fp:
         LONG_DESCRIPTION = fp.read()
 setup(
```

### Comparing `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/factor.py` & `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/factor.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/factor_modules/FaceModule.py` & `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/factor_modules/FaceModule.py`

 * *Files 11% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                 return FaceEnrollPredictResult(
                 status=face_validation_data.get("face_validation_status",0),
                 enroll_level=json_data.get("enroll_level", None),
                 puid=api_response.get("puid", None),
                 guid=api_response.get("guid", None),
                 token=api_response.get("token", None),
                 score=api_response.get("score", None),
-                message=c_response.get("message", "something went wrong"),
+                message=self.message.get_message(int(face_validation_data.get("face_validation_status",0))),
                  )
             return FaceEnrollPredictResult(
                 status=call_status,
                 enroll_level=json_data.get("enroll_level", None),
                 puid=api_response.get("puid", None),
                 guid=api_response.get("guid", None),
                 token=api_response.get("token", None),
@@ -101,53 +101,74 @@
                 call_status = FaceEnrollPredictResult.CALL_STATUS_SUCCESS
 
             c_response=json_data.get("predict_onefa", {})
             api_response=c_response.get("api_response", {})
             face_validation_data=c_response.get("face_validation_data", {})
             if face_validation_data.get("face_validation_status",0)!=0:
                 if config_object and json.loads(config_object.get_config_param()).get("neighbors",0)>0:
-                        return [FaceEnrollPredictResult(
-                        status=face_validation_data.get("face_validation_status",0),
-                        enroll_level=json_data.get("enroll_level", None),
-                        puid=api_response.get("puid", None),
-                        guid=api_response.get("guid", None),
-                        token=api_response.get("token", None),
-                        score=api_response.get("score", None),
-                        message=c_response.get("message", "something went wrong"),
-                        )]
+                        if api_response.get("PI_list", []):
+                            return [FaceEnrollPredictResult(
+                            status=face_validation_data.get("face_validation_status",0),
+                            enroll_level=json_data.get("enroll_level", None),
+                            puid=api_response.get("puid", None),
+                            guid=api_response.get("guid", None),
+                            token=api_response.get("token", None),
+                            score=api_response.get("score", None),
+                            message=self.message.get_message(face_validation_data.get("face_validation_status", 0))
+                            )]
+                        else:
+                            return [FaceEnrollPredictResult(
+                                    status=api_response.get("status", "Something went wrong"),
+                                    enroll_level=json_data.get("enroll_level", None),
+                                    puid= None,
+                                    guid=None,
+                                    score= None,
+                                    message=api_response.get("message", "Something went wrong"))]
+                            
                 else:
                      return FaceEnrollPredictResult(
                         status=face_validation_data.get("face_validation_status",0),
                         enroll_level=json_data.get("enroll_level", None),
                         puid=api_response.get("puid", None),
                         guid=api_response.get("guid", None),
                         token=api_response.get("token", None),
                         score=api_response.get("score", None),
-                        message=c_response.get("message", "something went wrong"),
+                        message=self.message.get_message(int(face_validation_data.get("face_validation_status",0))),
                         )
+            if config_object and json.loads(config_object.get_config_param()).get("neighbors",0)>0:
+                if api_response.get("PI_list", []):
+                    return [FaceEnrollPredictResult(
+                        status=call_status,
+                        enroll_level=json_data.get("enroll_level", None),
+                        puid=person.get("puid", None),
+                        guid=person.get("guid", None),
+                        score=person.get("score", None),
+                        message=api_response.get("message", "Something went wrong"),
+                    ) for person in api_response.get("PI_list", [])]
+                else:
+                   return [FaceEnrollPredictResult(
+                        status=api_response.get("status", "Something went wrong"),
+                        enroll_level=json_data.get("enroll_level", None),
+                        puid= None,
+                        guid=None,
+                        score= None,
+                        message=api_response.get("message", "Something went wrong"))]
 
-            if not api_response.get("PI_list", []):
-                return FaceEnrollPredictResult(
+            
+               
+            else:
+                 return FaceEnrollPredictResult(
                     status=call_status,
                     enroll_level=json_data.get("enroll_level", None),
                     puid=api_response.get("puid", None),
                     guid=api_response.get("guid", None),
                     token=api_response.get("token", None),
                     score=api_response.get("score", None),
                     message=api_response.get("message", ""),
                 )
-            else:
-                return [FaceEnrollPredictResult(
-                    status=call_status,
-                    enroll_level=json_data.get("enroll_level", None),
-                    puid=person.get("puid", None),
-                    guid=person.get("guid", None),
-                    score=person.get("score", None),
-                    message=api_response.get("message", "Something went wrong"),
-                ) for person in api_response.get("PI_list", [])]
         except Exception as e:
             print(e, traceback.format_exc())
             return FaceEnrollPredictResult(message=self.message.EXCEPTION_ERROR_PREDICT)
 
     def delete(self, puid: str, config_object: ConfigObject = None,) -> FaceDeleteResult:
         try:
             json_response = self.face_factor_processor.delete(puid,config_object)
@@ -235,34 +256,52 @@
     def compare(
         self,
         image_data_1: np.array,
         image_data_2: np.array,
         config_object: ConfigObject = None,
     ) -> FaceCompareResult:
         try:
-            json_data = self.face_factor_processor.compare_files(
-                image_data_1, image_data_2, config_object=config_object
-            )
-            call_status = FaceCompareResult.CALL_STATUS_ERROR
-            if not json_data:
-                return FaceCompareResult(message=self.message.EXCEPTION_ERROR_COMPARE)
-            else:
-                # we received a json response and thus call is successful
-                call_status = FaceCompareResult.CALL_STATUS_SUCCESS
-
-            return FaceCompareResult(
-                result=json_data.get("result", None),
-                distance_min=json_data.get("distance_min", None),
-                first_validation_result=json_data.get("valid_flag_a", None),
-                second_validation_result=json_data.get("valid_flag_b", None),
-                distance_max=json_data.get("distance_max", None),
-                distance_mean=json_data.get("distance_mean", None),
-                status=call_status,
-                message=json_data.get("message", ""),
-            )
+            
+                face_compare_json_data_all = self.face_factor_processor.compare_files(
+                       image_data_1, image_data_2, config_object=config_object
+                )
+                call_status = FaceCompareResult.CALL_STATUS_ERROR
+                if not face_compare_json_data_all:
+                    return FaceCompareResult(message=self.message.EXCEPTION_ERROR_COMPARE)
+                else:
+                    call_status = FaceCompareResult.CALL_STATUS_SUCCESS
+                face_data=face_compare_json_data_all.get("face_compare",{})
+                call_status=face_compare_json_data_all.get("call_status",{}).get("return_status",-1)
+                if face_data.get("result", None)==1:
+                    return FaceCompareResult(
+                        result=face_data.get("result", None),
+                        distance=face_data.get("distance_min", None),
+                        first_validation_result=face_data.get("a_face_validation_status", None),
+                        second_validation_result=face_data.get("b_face_validation_status", None),
+                        status=face_data.get("result", None),
+                        message= "Same face",
+                    )
+                elif face_data.get("result", None)==-1:
+                    return FaceCompareResult(
+                        result=face_data.get("result", None),
+                        distance=face_data.get("distance_min", None),
+                        first_validation_result=face_data.get("a_face_validation_status", None),
+                        second_validation_result=face_data.get("b_face_validation_status", None),
+                        status=call_status,
+                        message= "Different face",
+                    )
+                else:
+                    return FaceCompareResult(
+                        result=face_data.get("result", None),
+                        distance=face_data.get("distance_min", None),
+                        first_validation_result=face_data.get("a_face_validation_status", None),
+                        second_validation_result=face_data.get("b_face_validation_status", None),
+                        status=call_status,
+                        message=self.message.EXCEPTION_ERROR_COMPARE,
+                    )
         except Exception as e:
             print(e, traceback.format_exc())
             return FaceCompareResult(message=self.message.EXCEPTION_ERROR_COMPARE)
 
     def is_valid(
         self, image_data: np.array, config_object: ConfigObject = None
     ) -> FaceValidationResult:
```

### Comparing `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/handler/nativeMethods.py` & `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/handler/nativeMethods.py`

 * *Files 4% similar despite different names*

```diff
@@ -651,15 +651,14 @@
         right_image: np.array,
         config_object: ConfigObject = None,
     ) -> Any:
         fudge_factor = 0.0
         try:
             left_img_data_buffer = left_image.flatten()
             right_img_data_buffer = right_image.flatten()
-            print(len(left_img_data_buffer),len(right_img_data_buffer))
             left_c_img_data_buffer = left_img_data_buffer.ctypes.data_as(
                 POINTER(c_uint8)
             )
             right_c_img_data_buffer = right_img_data_buffer.ctypes.data_as(
                 POINTER(c_uint8)
             )
 
@@ -668,15 +667,15 @@
 
             rim_height, rim_width, _ = right_image.shape
             rim_size = (
                 right_image.shape[1] * right_image.shape[0] * right_image.shape[2]
             )
             p_buffer_result = c_char_p()
             p_buffer_result_length = c_int()
-            config_object_default = {"face_thresholds_rem_bad_emb_default": 1.275, "face_thresholds_med": 1.275,"conf_score_thr_enroll":0.2,"conf_score_thr_enroll":0.2}
+            config_object_default = {"face_thresholds_rem_bad_emb_default": 1.275, "face_thresholds_med": 1.275,"conf_score_thr_enroll":0.2}
 
             if config_object and hasattr(config_object, 'get_config_param') and config_object.get_config_param():
                 config_param_str = config_object.get_config_param()
                 config_from_object = json.loads(config_param_str)
                 for key, value in config_object_default.items():
                     if key not in config_from_object:
                         config_from_object[key] = value
@@ -752,18 +751,19 @@
             )
 
             if config_object and config_object.get_config_param():
                 # Load existing config from the object
                 config_dict = json.loads(config_object.get_config_param())
                 # Ensure disable_enroll_mf is always added
                 config_dict["disable_enroll_mf"] = True
+                config_dict["conf_score_thr_enroll"]=0.2
                 config_json = json.dumps(config_dict)
             else:
                 # Create a new config dict with disable_enroll_mf set to True
-                config_dict = {"disable_enroll_mf": True}
+                config_dict = {"disable_enroll_mf": True,"conf_score_thr_enroll":0.2}
                 config_json = json.dumps(config_dict)
             # Common logic for converting the config dict to the required C types
             c_config_param = c_char_p(bytes(config_json, "utf-8"))
             c_config_param_len = c_int(len(config_json))
 
 
             best_input_out = c_uint8()  # uint8_t** best_input_out
@@ -803,23 +803,30 @@
             p_buffer_images_in = img_data
             c_p_buffer_images_in = p_buffer_images_in.ctypes.data_as(POINTER(c_uint8))
             im_size = im_height * im_width * im_channel
 
             c_result = c_char_p()
             result_out = np.zeros(1, dtype=np.int32)
             c_result_out = result_out.ctypes.data_as(POINTER(ctypes.c_int32))
-
+            
             if config_object and config_object.get_config_param():
-                c_config_param = c_char_p(
-                    bytes(config_object.get_config_param(), "utf-8")
-                )
-                c_config_param_len = c_int(len(config_object.get_config_param()))
+                # Load existing config from the object
+                config_dict = json.loads(config_object.get_config_param())
+                # Ensure disable_enroll_mf is always added
+                config_dict["disable_enroll_mf"] = True
+                config_dict["conf_score_thr_enroll"]=0.2
+                config_json = json.dumps(config_dict)
             else:
-                c_config_param = c_char_p(bytes("", "utf-8"))
-                c_config_param_len = c_int(0)
+                # Create a new config dict with disable_enroll_mf set to True
+                config_dict = {"disable_enroll_mf": True,"conf_score_thr_enroll":0.2}
+                config_json = json.dumps(config_dict)
+          
+            c_config_param = c_char_p(bytes(config_json, "utf-8"))
+            c_config_param_len = c_int(len(config_json))
+
 
             self._spl_so_face.privid_face_predict_onefa(
                 self._spl_so_face.handle,
                 c_config_param,
                 c_config_param_len,
                 c_p_buffer_images_in,
                 c_int(im_count),
```

### Comparing `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/decorators.py` & `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/decorators.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/compareResult.py` & `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/compareResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/deleteResult.py` & `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/deleteResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/enrollPredictResult.py` & `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/enrollPredictResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/faceObjectResult.py` & `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/faceObjectResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/faceValidationResult.py` & `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/faceValidationResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/result_objects/isoFaceResult.py` & `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/result_objects/isoFaceResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/helper/utils.py` & `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/helper/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,20 +129,17 @@
         return item in [v.value for v in cls.__members__.values()]
 
 
 class FaceValidationCode(Enum, metaclass=FaceValidationCodeMeta):
     InvalidImage = -100  # Err = -100
     NoFace = -1  # faceNotDetected = -1
     ValidBiometric = 0  # Ok = 0
-    ImageSpoof = (
-        1  # TODO Check  deprecated or new code? this does not exist in cpp core
-    )
-    VideoSpoof = (
-        2  # TODO Check  deprecated or new code? this does not exist in cpp core
-    )
+    ImageSpoof =  1
+
+    VideoSpoof = 2 
     TooClose = 3  # faceTooClose = 3
     TooFaraway = 4  # faceTooFar = 4
     TooFarToRight = 5  # faceRight = 5
     TooFarToLeft = 6  # faceLeft = 6
     TooFarUp = 7  # faceUp = 7
     TooFarDown = 8  # faceDown = 8
     TooBlurry = 9  # imageBlurr = 9
@@ -155,8 +152,10 @@
     FaceTooDark = 16  # FaceTooDark = 16
     FaceTooBright = 17  # FaceTooBright = 17
     FaceLowValConf = 18  # FaceLowValConf = 18
     InvalidFaceBackground = 19  # InvalidFaceBackground = 19
     EyeBlink = 20  # EyeBlink = 20
     МouthOpened = 21  # МouthOpened = 21
     faceRotatedRight = 22
-    faceRotatedLeft = 23
+    faceRotatedLeft = 23
+
+
```

### Comparing `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk/settings/configuration.py` & `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk/settings/configuration.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk.egg-info/PKG-INFO` & `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptonets-python-sdk
-Version: 1.2.2
+Version: 1.2.3
 Summary: Cryptonets SDK Library for Python
 Home-page: https://privateid.com/
 Author: Private Identity
 Author-email: support@private.id
 Project-URL: Bug Reports, https://github.com/prividentity/cryptonets-python-sdk/issues
 Project-URL: Source, https://github.com/prividentity/cryptonets-python-sdk
 Project-URL: Documentation, https://docs.private.id/cryptonets-python-sdk/index.html
```

### Comparing `cryptonets_python_sdk-1.2.2/src/cryptonets_python_sdk.egg-info/SOURCES.txt` & `cryptonets_python_sdk-1.2.3/src/cryptonets_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.2/tests/test.py` & `cryptonets_python_sdk-1.2.3/tests/test.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.2.2/tests/test_suite.py` & `cryptonets_python_sdk-1.2.3/tests/test_suite.py`

 * *Files identical despite different names*

