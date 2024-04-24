# Comparing `tmp/np-upload-validation-0.1.8.tar.gz` & `tmp/np-upload-validation-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np-upload-validation-0.1.8.tar", last modified: Fri Feb 16 18:36:43 2024, max compression
+gzip compressed data, was "np-upload-validation-0.1.9.tar", last modified: Fri Feb 16 19:11:15 2024, max compression
```

## Comparing `np-upload-validation-0.1.8.tar` & `np-upload-validation-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:43.335984 np-upload-validation-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-02-16 18:35:49.000000 np-upload-validation-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-02-16 18:36:43.335984 np-upload-validation-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-02-16 18:35:49.000000 np-upload-validation-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-02-16 18:36:39.000000 np-upload-validation-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 18:36:43.335984 np-upload-validation-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:43.331984 np-upload-validation-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:43.335984 np-upload-validation-0.1.8/src/np_upload_validation/
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-02-16 18:35:49.000000 np-upload-validation-0.1.8/src/np_upload_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-02-16 18:35:49.000000 np-upload-validation-0.1.8/src/np_upload_validation/checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-16 18:35:49.000000 np-upload-validation-0.1.8/src/np_upload_validation/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-02-16 18:36:35.000000 np-upload-validation-0.1.8/src/np_upload_validation/hpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-16 18:35:49.000000 np-upload-validation-0.1.8/src/np_upload_validation/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-02-16 18:36:35.000000 np-upload-validation-0.1.8/src/np_upload_validation/npc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:35:49.000000 np-upload-validation-0.1.8/src/np_upload_validation/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:43.335984 np-upload-validation-0.1.8/src/np_upload_validation/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-02-16 18:35:49.000000 np-upload-validation-0.1.8/src/np_upload_validation/scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-02-16 18:35:49.000000 np-upload-validation-0.1.8/src/np_upload_validation/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:43.335984 np-upload-validation-0.1.8/src/np_upload_validation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-02-16 18:36:43.000000 np-upload-validation-0.1.8/src/np_upload_validation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-02-16 18:36:43.000000 np-upload-validation-0.1.8/src/np_upload_validation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 18:36:43.000000 np-upload-validation-0.1.8/src/np_upload_validation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-16 18:36:43.000000 np-upload-validation-0.1.8/src/np_upload_validation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-16 18:36:43.000000 np-upload-validation-0.1.8/src/np_upload_validation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-16 18:36:43.000000 np-upload-validation-0.1.8/src/np_upload_validation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:36:43.335984 np-upload-validation-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-02-16 18:35:49.000000 np-upload-validation-0.1.8/tests/test_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-16 18:35:49.000000 np-upload-validation-0.1.8/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-16 18:35:49.000000 np-upload-validation-0.1.8/tests/test_hpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-02-16 18:35:49.000000 np-upload-validation-0.1.8/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:11:14.995609 np-upload-validation-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-02-16 19:10:26.000000 np-upload-validation-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-02-16 19:11:14.995609 np-upload-validation-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-02-16 19:10:26.000000 np-upload-validation-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-02-16 19:11:10.000000 np-upload-validation-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 19:11:14.995609 np-upload-validation-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:11:14.991609 np-upload-validation-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:11:14.995609 np-upload-validation-0.1.9/src/np_upload_validation/
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-02-16 19:10:26.000000 np-upload-validation-0.1.9/src/np_upload_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-02-16 19:10:26.000000 np-upload-validation-0.1.9/src/np_upload_validation/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-16 19:10:26.000000 np-upload-validation-0.1.9/src/np_upload_validation/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-02-16 19:10:26.000000 np-upload-validation-0.1.9/src/np_upload_validation/hpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-16 19:10:26.000000 np-upload-validation-0.1.9/src/np_upload_validation/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-02-16 19:10:26.000000 np-upload-validation-0.1.9/src/np_upload_validation/npc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 19:10:26.000000 np-upload-validation-0.1.9/src/np_upload_validation/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:11:14.995609 np-upload-validation-0.1.9/src/np_upload_validation/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-02-16 19:10:26.000000 np-upload-validation-0.1.9/src/np_upload_validation/scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-02-16 19:10:26.000000 np-upload-validation-0.1.9/src/np_upload_validation/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:11:14.995609 np-upload-validation-0.1.9/src/np_upload_validation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-02-16 19:11:14.000000 np-upload-validation-0.1.9/src/np_upload_validation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-02-16 19:11:14.000000 np-upload-validation-0.1.9/src/np_upload_validation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 19:11:14.000000 np-upload-validation-0.1.9/src/np_upload_validation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-16 19:11:14.000000 np-upload-validation-0.1.9/src/np_upload_validation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-16 19:11:14.000000 np-upload-validation-0.1.9/src/np_upload_validation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-16 19:11:14.000000 np-upload-validation-0.1.9/src/np_upload_validation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:11:14.995609 np-upload-validation-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-02-16 19:10:26.000000 np-upload-validation-0.1.9/tests/test_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-16 19:10:26.000000 np-upload-validation-0.1.9/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-16 19:10:26.000000 np-upload-validation-0.1.9/tests/test_hpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-02-16 19:10:26.000000 np-upload-validation-0.1.9/tests/test_validation.py
```

### Comparing `np-upload-validation-0.1.8/LICENSE` & `np-upload-validation-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `np-upload-validation-0.1.8/PKG-INFO` & `np-upload-validation-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-upload-validation
-Version: 0.1.8
+Version: 0.1.9
 Summary: AWS upload validation
 Author-email: Christopher Mochizuki <chrism@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/np-upload-validation
 Project-URL: Issues, https://github.com/AllenInstitute/np-upload-validation/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `np-upload-validation-0.1.8/README.md` & `np-upload-validation-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `np-upload-validation-0.1.8/pyproject.toml` & `np-upload-validation-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "fabric>=3.2.2",
     "npc-lims==0.1.110",
     "npc-sessions==0.0.179",
     "numpy>=1.26.4",
     "click>=8.1.7",
     "python-dotenv>=1.0.1",
 ]
-version = "0.1.8"
+version = "0.1.9"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
```

### Comparing `np-upload-validation-0.1.8/src/np_upload_validation/__init__.py` & `np-upload-validation-0.1.9/src/np_upload_validation/__init__.py`

 * *Files identical despite different names*

### Comparing `np-upload-validation-0.1.8/src/np_upload_validation/checksum.py` & `np-upload-validation-0.1.9/src/np_upload_validation/checksum.py`

 * *Files identical despite different names*

### Comparing `np-upload-validation-0.1.8/src/np_upload_validation/hpc.py` & `np-upload-validation-0.1.9/src/np_upload_validation/hpc.py`

 * *Files identical despite different names*

### Comparing `np-upload-validation-0.1.8/src/np_upload_validation/npc.py` & `np-upload-validation-0.1.9/src/np_upload_validation/npc.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,18 +45,17 @@
     if not info.is_uploaded:
         raise exceptions.ValidationException("Data not yet uploaded.")
 
     s3 = npc_sessions.Session(info)
     logger.debug("s3 session id: %s" % s3.id)
     isilon = npc_sessions.Session(info.allen_path)
     logger.debug("isilon session id: %s" % isilon.id)
-    if s3.id == isilon.id:
-        raise exceptions.ValidationException(
-            "Fetched s3 and isilon sessions are the same."
-        )
+    # if s3.id == isilon.id:
+    #     raise exceptions.ValidationException(
+    #         "Fetched s3 and isilon sessions are the same.")
 
     for timing_data in isilon.ephys_timing_data:
         try:
             logger.debug("isilon device name: %s" % timing_data.device.name)
             isilon_timing_data = _get_timing_data(timing_data.device)
             s3_device = next(
                 d.device
```

### Comparing `np-upload-validation-0.1.8/src/np_upload_validation/scripts/main.py` & `np-upload-validation-0.1.9/src/np_upload_validation/scripts/main.py`

 * *Files identical despite different names*

### Comparing `np-upload-validation-0.1.8/src/np_upload_validation/validation.py` & `np-upload-validation-0.1.9/src/np_upload_validation/validation.py`

 * *Files identical despite different names*

### Comparing `np-upload-validation-0.1.8/src/np_upload_validation.egg-info/PKG-INFO` & `np-upload-validation-0.1.9/src/np_upload_validation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-upload-validation
-Version: 0.1.8
+Version: 0.1.9
 Summary: AWS upload validation
 Author-email: Christopher Mochizuki <chrism@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/np-upload-validation
 Project-URL: Issues, https://github.com/AllenInstitute/np-upload-validation/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `np-upload-validation-0.1.8/src/np_upload_validation.egg-info/SOURCES.txt` & `np-upload-validation-0.1.9/src/np_upload_validation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `np-upload-validation-0.1.8/tests/test_checksum.py` & `np-upload-validation-0.1.9/tests/test_checksum.py`

 * *Files identical despite different names*

### Comparing `np-upload-validation-0.1.8/tests/test_validation.py` & `np-upload-validation-0.1.9/tests/test_validation.py`

 * *Files identical despite different names*

