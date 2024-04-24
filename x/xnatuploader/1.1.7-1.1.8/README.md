# Comparing `tmp/xnatuploader-1.1.7.tar.gz` & `tmp/xnatuploader-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnatuploader-1.1.7.tar", last modified: Mon Apr 15 06:04:17 2024, max compression
+gzip compressed data, was "xnatuploader-1.1.8.tar", last modified: Wed Apr 24 04:19:01 2024, max compression
```

## Comparing `xnatuploader-1.1.7.tar` & `xnatuploader-1.1.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-04-15 06:04:17.357443 xnatuploader-1.1.7/
--rw-r--r--   0 mike       (501) staff       (20)    14656 2024-04-15 06:04:17.356798 xnatuploader-1.1.7/PKG-INFO
--rw-r--r--   0 mike       (501) staff       (20)    13805 2023-08-21 06:36:43.000000 xnatuploader-1.1.7/README.md
--rw-r--r--   0 mike       (501) staff       (20)       93 2022-06-16 06:56:16.000000 xnatuploader-1.1.7/pyproject.toml
--rw-r--r--   0 mike       (501) staff       (20)     1104 2024-04-15 06:04:17.358771 xnatuploader-1.1.7/setup.cfg
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-04-15 06:04:17.332955 xnatuploader-1.1.7/src/
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-04-15 06:04:17.344589 xnatuploader-1.1.7/src/xnatuploader/
--rw-r--r--   0 mike       (501) staff       (20)       72 2022-06-16 06:56:16.000000 xnatuploader-1.1.7/src/xnatuploader/__init__.py
--rw-r--r--   0 mike       (501) staff       (20)      283 2023-05-25 02:08:09.000000 xnatuploader-1.1.7/src/xnatuploader/dataclass.py
--rw-r--r--   0 mike       (501) staff       (20)     3420 2024-04-15 05:45:59.000000 xnatuploader-1.1.7/src/xnatuploader/dicoms.py
--rw-r--r--   0 mike       (501) staff       (20)    14733 2024-04-15 05:45:59.000000 xnatuploader-1.1.7/src/xnatuploader/matcher.py
--rw-r--r--   0 mike       (501) staff       (20)     8947 2023-03-15 03:09:46.000000 xnatuploader-1.1.7/src/xnatuploader/put.py
--rw-r--r--   0 mike       (501) staff       (20)     8483 2024-04-15 05:45:59.000000 xnatuploader-1.1.7/src/xnatuploader/upload.py
--rw-r--r--   0 mike       (501) staff       (20)      203 2023-04-05 06:48:06.000000 xnatuploader-1.1.7/src/xnatuploader/userdict.py
--rw-r--r--   0 mike       (501) staff       (20)     4131 2023-12-20 05:46:20.000000 xnatuploader-1.1.7/src/xnatuploader/workbook.py
--rwxr-xr-x   0 mike       (501) staff       (20)    19103 2024-04-15 05:45:59.000000 xnatuploader-1.1.7/src/xnatuploader/xnatuploader.py
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-04-15 06:04:17.354949 xnatuploader-1.1.7/src/xnatuploader.egg-info/
--rw-r--r--   0 mike       (501) staff       (20)    14656 2024-04-15 06:04:17.000000 xnatuploader-1.1.7/src/xnatuploader.egg-info/PKG-INFO
--rw-r--r--   0 mike       (501) staff       (20)      615 2024-04-15 06:04:17.000000 xnatuploader-1.1.7/src/xnatuploader.egg-info/SOURCES.txt
--rw-r--r--   0 mike       (501) staff       (20)        1 2024-04-15 06:04:17.000000 xnatuploader-1.1.7/src/xnatuploader.egg-info/dependency_links.txt
--rw-r--r--   0 mike       (501) staff       (20)       64 2024-04-15 06:04:17.000000 xnatuploader-1.1.7/src/xnatuploader.egg-info/entry_points.txt
--rw-r--r--   0 mike       (501) staff       (20)      123 2024-04-15 06:04:17.000000 xnatuploader-1.1.7/src/xnatuploader.egg-info/requires.txt
--rw-r--r--   0 mike       (501) staff       (20)       13 2024-04-15 06:04:17.000000 xnatuploader-1.1.7/src/xnatuploader.egg-info/top_level.txt
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-04-15 06:04:17.353873 xnatuploader-1.1.7/tests/
--rw-r--r--   0 mike       (501) staff       (20)      289 2022-11-17 02:49:16.000000 xnatuploader-1.1.7/tests/test_config.py
--rw-r--r--   0 mike       (501) staff       (20)     3117 2024-02-06 22:21:42.000000 xnatuploader-1.1.7/tests/test_matcher.py
--rw-r--r--   0 mike       (501) staff       (20)     5937 2024-04-15 05:45:59.000000 xnatuploader-1.1.7/tests/test_scan.py
--rw-r--r--   0 mike       (501) staff       (20)     5938 2024-04-15 05:45:59.000000 xnatuploader-1.1.7/tests/test_upload.py
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-04-24 04:19:01.692525 xnatuploader-1.1.8/
+-rw-r--r--   0 mike       (501) staff       (20)    14656 2024-04-24 04:19:01.691738 xnatuploader-1.1.8/PKG-INFO
+-rw-r--r--   0 mike       (501) staff       (20)    13805 2023-08-21 06:36:43.000000 xnatuploader-1.1.8/README.md
+-rw-r--r--   0 mike       (501) staff       (20)       93 2022-06-16 06:56:16.000000 xnatuploader-1.1.8/pyproject.toml
+-rw-r--r--   0 mike       (501) staff       (20)     1104 2024-04-24 04:19:01.694121 xnatuploader-1.1.8/setup.cfg
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-04-24 04:19:01.662026 xnatuploader-1.1.8/src/
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-04-24 04:19:01.675654 xnatuploader-1.1.8/src/xnatuploader/
+-rw-r--r--   0 mike       (501) staff       (20)       72 2022-06-16 06:56:16.000000 xnatuploader-1.1.8/src/xnatuploader/__init__.py
+-rw-r--r--   0 mike       (501) staff       (20)      283 2023-05-25 02:08:09.000000 xnatuploader-1.1.8/src/xnatuploader/dataclass.py
+-rw-r--r--   0 mike       (501) staff       (20)     3456 2024-04-24 04:18:10.000000 xnatuploader-1.1.8/src/xnatuploader/dicoms.py
+-rw-r--r--   0 mike       (501) staff       (20)    14733 2024-04-15 05:45:59.000000 xnatuploader-1.1.8/src/xnatuploader/matcher.py
+-rw-r--r--   0 mike       (501) staff       (20)     8947 2023-03-15 03:09:46.000000 xnatuploader-1.1.8/src/xnatuploader/put.py
+-rw-r--r--   0 mike       (501) staff       (20)     8483 2024-04-15 05:45:59.000000 xnatuploader-1.1.8/src/xnatuploader/upload.py
+-rw-r--r--   0 mike       (501) staff       (20)      203 2023-04-05 06:48:06.000000 xnatuploader-1.1.8/src/xnatuploader/userdict.py
+-rw-r--r--   0 mike       (501) staff       (20)     4131 2023-12-20 05:46:20.000000 xnatuploader-1.1.8/src/xnatuploader/workbook.py
+-rwxr-xr-x   0 mike       (501) staff       (20)    19103 2024-04-15 05:45:59.000000 xnatuploader-1.1.8/src/xnatuploader/xnatuploader.py
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-04-24 04:19:01.689615 xnatuploader-1.1.8/src/xnatuploader.egg-info/
+-rw-r--r--   0 mike       (501) staff       (20)    14656 2024-04-24 04:19:01.000000 xnatuploader-1.1.8/src/xnatuploader.egg-info/PKG-INFO
+-rw-r--r--   0 mike       (501) staff       (20)      615 2024-04-24 04:19:01.000000 xnatuploader-1.1.8/src/xnatuploader.egg-info/SOURCES.txt
+-rw-r--r--   0 mike       (501) staff       (20)        1 2024-04-24 04:19:01.000000 xnatuploader-1.1.8/src/xnatuploader.egg-info/dependency_links.txt
+-rw-r--r--   0 mike       (501) staff       (20)       64 2024-04-24 04:19:01.000000 xnatuploader-1.1.8/src/xnatuploader.egg-info/entry_points.txt
+-rw-r--r--   0 mike       (501) staff       (20)      123 2024-04-24 04:19:01.000000 xnatuploader-1.1.8/src/xnatuploader.egg-info/requires.txt
+-rw-r--r--   0 mike       (501) staff       (20)       13 2024-04-24 04:19:01.000000 xnatuploader-1.1.8/src/xnatuploader.egg-info/top_level.txt
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-04-24 04:19:01.687763 xnatuploader-1.1.8/tests/
+-rw-r--r--   0 mike       (501) staff       (20)      289 2022-11-17 02:49:16.000000 xnatuploader-1.1.8/tests/test_config.py
+-rw-r--r--   0 mike       (501) staff       (20)     3117 2024-02-06 22:21:42.000000 xnatuploader-1.1.8/tests/test_matcher.py
+-rw-r--r--   0 mike       (501) staff       (20)     5937 2024-04-15 05:45:59.000000 xnatuploader-1.1.8/tests/test_scan.py
+-rw-r--r--   0 mike       (501) staff       (20)     5938 2024-04-15 05:45:59.000000 xnatuploader-1.1.8/tests/test_upload.py
```

### Comparing `xnatuploader-1.1.7/PKG-INFO` & `xnatuploader-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnatuploader
-Version: 1.1.7
+Version: 1.1.8
 Summary: CLI tool for uploading multiple files to XNAT
 Home-page: https://github.com/SydneyInformaticsHub/xnatuploader
 Author: Mike Lynch
 Author-email: m.lynch@sydney.edu.au
 Project-URL: Bug Tracker, https://github.com/SydneyInformaticsHub/xnatuploader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `xnatuploader-1.1.7/README.md` & `xnatuploader-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.7/setup.cfg` & `xnatuploader-1.1.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = xnatuploader
-version = 1.1.7
+version = 1.1.8
 author = Mike Lynch
 author_email = m.lynch@sydney.edu.au
 description = CLI tool for uploading multiple files to XNAT
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/SydneyInformaticsHub/xnatuploader
 project_urls =
```

### Comparing `xnatuploader-1.1.7/src/xnatuploader/dicoms.py` & `xnatuploader-1.1.8/src/xnatuploader/dicoms.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,17 @@
         raise ExtractException("DICOM is an encapsulated report")
     values = {f"DICOM:{p}": dc_meta.get(p) for p in DICOM_PARAMS}
     if "DICOM:Modality" not in values:
         raise ExtractException("DICOM has no modality")
     if values["DICOM:Modality"] == "SR":
         raise ExtractException("DICOM is an SR (structured report)")
     image_type = dc_meta.get("ImageType")
-    if image_type[2] == "DOSE_INFO":
-        raise ExtractException("DICOM has ImageType DOSE_INFO")
+    if len(image_type) > 2:
+        if image_type[2] == "DOSE_INFO":
+            raise ExtractException("DICOM has ImageType DOSE_INFO")
     return values
 
 
 class XNATFileMatch(FileMatch):
     """
     Sublass of FileMatch which provides getters and setters for xnat-specific
     metadata.
```

### Comparing `xnatuploader-1.1.7/src/xnatuploader/matcher.py` & `xnatuploader-1.1.8/src/xnatuploader/matcher.py`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.7/src/xnatuploader/put.py` & `xnatuploader-1.1.8/src/xnatuploader/put.py`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.7/src/xnatuploader/upload.py` & `xnatuploader-1.1.8/src/xnatuploader/upload.py`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.7/src/xnatuploader/workbook.py` & `xnatuploader-1.1.8/src/xnatuploader/workbook.py`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.7/src/xnatuploader/xnatuploader.py` & `xnatuploader-1.1.8/src/xnatuploader/xnatuploader.py`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.7/src/xnatuploader.egg-info/PKG-INFO` & `xnatuploader-1.1.8/src/xnatuploader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnatuploader
-Version: 1.1.7
+Version: 1.1.8
 Summary: CLI tool for uploading multiple files to XNAT
 Home-page: https://github.com/SydneyInformaticsHub/xnatuploader
 Author: Mike Lynch
 Author-email: m.lynch@sydney.edu.au
 Project-URL: Bug Tracker, https://github.com/SydneyInformaticsHub/xnatuploader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `xnatuploader-1.1.7/src/xnatuploader.egg-info/SOURCES.txt` & `xnatuploader-1.1.8/src/xnatuploader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.7/tests/test_matcher.py` & `xnatuploader-1.1.8/tests/test_matcher.py`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.7/tests/test_scan.py` & `xnatuploader-1.1.8/tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.7/tests/test_upload.py` & `xnatuploader-1.1.8/tests/test_upload.py`

 * *Files identical despite different names*

