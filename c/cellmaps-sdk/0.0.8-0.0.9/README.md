# Comparing `tmp/cellmaps_sdk-0.0.8.tar.gz` & `tmp/cellmaps_sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellmaps_sdk-0.0.8.tar", last modified: Mon Apr 22 15:01:37 2024, max compression
+gzip compressed data, was "cellmaps_sdk-0.0.9.tar", last modified: Wed Apr 24 12:45:12 2024, max compression
```

## Comparing `cellmaps_sdk-0.0.8.tar` & `cellmaps_sdk-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-04-22 15:01:37.708274 cellmaps_sdk-0.0.8/
--rw-r--r--   0 colmbrandon   (501) staff       (20)        0 2024-01-26 12:59:01.000000 cellmaps_sdk-0.0.8/LICENSE.txt
--rw-r--r--   0 colmbrandon   (501) staff       (20)     1569 2024-04-22 15:01:37.708051 cellmaps_sdk-0.0.8/PKG-INFO
--rw-r--r--   0 colmbrandon   (501) staff       (20)      192 2024-01-26 12:59:01.000000 cellmaps_sdk-0.0.8/README.rst
--rw-r--r--   0 colmbrandon   (501) staff       (20)     1561 2024-04-22 15:00:50.000000 cellmaps_sdk-0.0.8/pyproject.toml
--rw-r--r--   0 colmbrandon   (501) staff       (20)       38 2024-04-22 15:01:37.708325 cellmaps_sdk-0.0.8/setup.cfg
-drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-04-22 15:01:37.700834 cellmaps_sdk-0.0.8/src/
-drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-04-22 15:01:37.706650 cellmaps_sdk-0.0.8/src/cellmaps_sdk/
--rw-r--r--   0 colmbrandon   (501) staff       (20)      282 2024-02-06 12:12:31.000000 cellmaps_sdk-0.0.8/src/cellmaps_sdk/__init__.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     2871 2024-03-07 12:05:00.000000 cellmaps_sdk-0.0.8/src/cellmaps_sdk/__main__.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)    36830 2024-02-23 16:16:31.000000 cellmaps_sdk-0.0.8/src/cellmaps_sdk/_cli_utils.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     1636 2024-03-14 11:43:19.000000 cellmaps_sdk-0.0.8/src/cellmaps_sdk/_config.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     9364 2024-04-22 14:53:12.000000 cellmaps_sdk-0.0.8/src/cellmaps_sdk/_raw_data.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     2657 2024-02-12 17:14:01.000000 cellmaps_sdk-0.0.8/src/cellmaps_sdk/_test_utils.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     1710 2024-04-22 15:00:37.000000 cellmaps_sdk-0.0.8/src/cellmaps_sdk/_utils.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)    35205 2024-04-18 12:00:14.000000 cellmaps_sdk-0.0.8/src/cellmaps_sdk/data.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     4461 2024-02-23 13:18:34.000000 cellmaps_sdk-0.0.8/src/cellmaps_sdk/data_utils.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)    29788 2024-03-06 12:03:46.000000 cellmaps_sdk-0.0.8/src/cellmaps_sdk/process.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)        0 2024-01-26 12:59:01.000000 cellmaps_sdk-0.0.8/src/cellmaps_sdk/py.typed
-drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-04-22 15:01:37.707573 cellmaps_sdk-0.0.8/src/cellmaps_sdk.egg-info/
--rw-r--r--   0 colmbrandon   (501) staff       (20)     1569 2024-04-22 15:01:37.000000 cellmaps_sdk-0.0.8/src/cellmaps_sdk.egg-info/PKG-INFO
--rw-r--r--   0 colmbrandon   (501) staff       (20)      595 2024-04-22 15:01:37.000000 cellmaps_sdk-0.0.8/src/cellmaps_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 colmbrandon   (501) staff       (20)        1 2024-04-22 15:01:37.000000 cellmaps_sdk-0.0.8/src/cellmaps_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 colmbrandon   (501) staff       (20)       55 2024-04-22 15:01:37.000000 cellmaps_sdk-0.0.8/src/cellmaps_sdk.egg-info/entry_points.txt
--rw-r--r--   0 colmbrandon   (501) staff       (20)      171 2024-04-22 15:01:37.000000 cellmaps_sdk-0.0.8/src/cellmaps_sdk.egg-info/requires.txt
--rw-r--r--   0 colmbrandon   (501) staff       (20)       13 2024-04-22 15:01:37.000000 cellmaps_sdk-0.0.8/src/cellmaps_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-04-24 12:45:12.957700 cellmaps_sdk-0.0.9/
+-rw-r--r--   0 colmbrandon   (501) staff       (20)        0 2024-01-26 12:59:01.000000 cellmaps_sdk-0.0.9/LICENSE.txt
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     1569 2024-04-24 12:45:12.957414 cellmaps_sdk-0.0.9/PKG-INFO
+-rw-r--r--   0 colmbrandon   (501) staff       (20)      192 2024-01-26 12:59:01.000000 cellmaps_sdk-0.0.9/README.rst
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     1561 2024-04-24 12:43:07.000000 cellmaps_sdk-0.0.9/pyproject.toml
+-rw-r--r--   0 colmbrandon   (501) staff       (20)       38 2024-04-24 12:45:12.957759 cellmaps_sdk-0.0.9/setup.cfg
+drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-04-24 12:45:12.948905 cellmaps_sdk-0.0.9/src/
+drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-04-24 12:45:12.955197 cellmaps_sdk-0.0.9/src/cellmaps_sdk/
+-rw-r--r--   0 colmbrandon   (501) staff       (20)      282 2024-02-06 12:12:31.000000 cellmaps_sdk-0.0.9/src/cellmaps_sdk/__init__.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     2871 2024-03-07 12:05:00.000000 cellmaps_sdk-0.0.9/src/cellmaps_sdk/__main__.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)    36830 2024-02-23 16:16:31.000000 cellmaps_sdk-0.0.9/src/cellmaps_sdk/_cli_utils.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     1636 2024-03-14 11:43:19.000000 cellmaps_sdk-0.0.9/src/cellmaps_sdk/_config.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     9359 2024-04-24 12:42:47.000000 cellmaps_sdk-0.0.9/src/cellmaps_sdk/_raw_data.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     2657 2024-02-12 17:14:01.000000 cellmaps_sdk-0.0.9/src/cellmaps_sdk/_test_utils.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     1710 2024-04-22 15:00:37.000000 cellmaps_sdk-0.0.9/src/cellmaps_sdk/_utils.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)    35205 2024-04-18 12:00:14.000000 cellmaps_sdk-0.0.9/src/cellmaps_sdk/data.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     4461 2024-02-23 13:18:34.000000 cellmaps_sdk-0.0.9/src/cellmaps_sdk/data_utils.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)    29788 2024-03-06 12:03:46.000000 cellmaps_sdk-0.0.9/src/cellmaps_sdk/process.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)        0 2024-01-26 12:59:01.000000 cellmaps_sdk-0.0.9/src/cellmaps_sdk/py.typed
+drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-04-24 12:45:12.956850 cellmaps_sdk-0.0.9/src/cellmaps_sdk.egg-info/
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     1569 2024-04-24 12:45:12.000000 cellmaps_sdk-0.0.9/src/cellmaps_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 colmbrandon   (501) staff       (20)      595 2024-04-24 12:45:12.000000 cellmaps_sdk-0.0.9/src/cellmaps_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 colmbrandon   (501) staff       (20)        1 2024-04-24 12:45:12.000000 cellmaps_sdk-0.0.9/src/cellmaps_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 colmbrandon   (501) staff       (20)       55 2024-04-24 12:45:12.000000 cellmaps_sdk-0.0.9/src/cellmaps_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 colmbrandon   (501) staff       (20)      171 2024-04-24 12:45:12.000000 cellmaps_sdk-0.0.9/src/cellmaps_sdk.egg-info/requires.txt
+-rw-r--r--   0 colmbrandon   (501) staff       (20)       13 2024-04-24 12:45:12.000000 cellmaps_sdk-0.0.9/src/cellmaps_sdk.egg-info/top_level.txt
```

### Comparing `cellmaps_sdk-0.0.8/PKG-INFO` & `cellmaps_sdk-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: The SDK for tool builders who wish to integrate their tool into the CellMaps Analysis Workflow IME
 Author-email: Colm Brandon <colm.brandon@ul.ie>
 Project-URL: Homepage, http://example.com
 Project-URL: Documentation, http://example.com
 Project-URL: Repository, http://example.com
 Project-URL: Bug Tracker, http://example.com
 Project-URL: Changelog, http://example.com
```

### Comparing `cellmaps_sdk-0.0.8/pyproject.toml` & `cellmaps_sdk-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "cellmaps-sdk"
 authors = [{name = "Colm Brandon", email = "colm.brandon@ul.ie"}]
-version = "0.0.8"
+version = "0.0.9"
 description = "The SDK for tool builders who wish to integrate their tool into the CellMaps Analysis Workflow IME"
 readme = "README.rst"
 license = {file = "LICENSE.txt"}
 keywords = ["Highly-plexed Tissue Imaging", "AI",]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python",
```

### Comparing `cellmaps_sdk-0.0.8/src/cellmaps_sdk/__main__.py` & `cellmaps_sdk-0.0.9/src/cellmaps_sdk/__main__.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.8/src/cellmaps_sdk/_cli_utils.py` & `cellmaps_sdk-0.0.9/src/cellmaps_sdk/_cli_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.8/src/cellmaps_sdk/_config.py` & `cellmaps_sdk-0.0.9/src/cellmaps_sdk/_config.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.8/src/cellmaps_sdk/_raw_data.py` & `cellmaps_sdk-0.0.9/src/cellmaps_sdk/_raw_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,16 +144,16 @@
             if obj.tags['cdb_experiment_type'] == ExperimentClass.experiment_tag:
                 # split the prefix and the file name (prefix is the experiment id)
                 prefix, file = obj.object_name.split('/')
                 # iterate over the files in the ExperimentClass (these are the files which should be present in the experiment prefix)
                 for f in ExperimentClass.files:
                     # prevent files with same regex to be overwritten
                     if f.cdb_file_tag not in all_experiments[prefix].keys():
-                        # check if the regex matches the file and the filetype matches the cdb_file_type
-                        if re.match(f.file_regex, file) and obj.tags['cdb_file_type'] == f.cdb_file_type:
+                        # check if the regex matches the file and the filetype matches the cdb_file_tag
+                        if re.match(f.file_regex, file) and obj.tags['cdb_file_tag'] == f.cdb_file_tag:
                             # add the file to the experiment dictionary for that prefix
                             if f.transformation_fn != None and use_transformations:
                                 # apply the transformation function to the file (typically reading the file and transforming it to a different format, as opposed to simply retrieving the file name)
                                 all_experiments[prefix][f.cdb_file_tag] = f.transformation_fn(obj)
                             else:
                                 all_experiments[prefix][f.cdb_file_tag] = file
                             break
@@ -186,16 +186,16 @@
     """
     client = _get_minio_client()
     urls = {}
     # iterate over the objects for a given experiment prefix
     for obj in client.list_objects(_Config._MINIO_EXPERIMENT_BUCKET,prefix_name,include_user_meta=True):
         # iterate over the files in the ExperimentClass
         for f in ExperimentClass.files:
-            # check if the regex matches the file and the filetype matches the cdb_file_type
-            if f.cdb_file_tag == obj.tags['cdb_file_type'] and re.match(f.file_regex, obj.object_name.split('/')[-1]):
+            # check if the regex matches the file and the filetype matches the cdb_file_tag
+            if f.cdb_file_tag == obj.tags['cdb_file_tag'] and re.match(f.file_regex, obj.object_name.split('/')[-1]):
                 urls[f.cdb_file_tag] = client.get_presigned_url('GET', bucket_name=_Config._MINIO_EXPERIMENT_BUCKET,object_name=obj.object_name)
                 break
     
     valid_file_tags = [f.cdb_file_tag for f in ExperimentClass.files] # get all the cdb_file_tags for the experiment class
     # check if all the required files are present (i.e. the experiment data is complete)
     if list(urls.keys()) == valid_file_tags:
         return urls
```

### Comparing `cellmaps_sdk-0.0.8/src/cellmaps_sdk/_test_utils.py` & `cellmaps_sdk-0.0.9/src/cellmaps_sdk/_test_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.8/src/cellmaps_sdk/_utils.py` & `cellmaps_sdk-0.0.9/src/cellmaps_sdk/_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.8/src/cellmaps_sdk/data.py` & `cellmaps_sdk-0.0.9/src/cellmaps_sdk/data.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.8/src/cellmaps_sdk/data_utils.py` & `cellmaps_sdk-0.0.9/src/cellmaps_sdk/data_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.8/src/cellmaps_sdk/process.py` & `cellmaps_sdk-0.0.9/src/cellmaps_sdk/process.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.8/src/cellmaps_sdk.egg-info/PKG-INFO` & `cellmaps_sdk-0.0.9/src/cellmaps_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: The SDK for tool builders who wish to integrate their tool into the CellMaps Analysis Workflow IME
 Author-email: Colm Brandon <colm.brandon@ul.ie>
 Project-URL: Homepage, http://example.com
 Project-URL: Documentation, http://example.com
 Project-URL: Repository, http://example.com
 Project-URL: Bug Tracker, http://example.com
 Project-URL: Changelog, http://example.com
```

### Comparing `cellmaps_sdk-0.0.8/src/cellmaps_sdk.egg-info/SOURCES.txt` & `cellmaps_sdk-0.0.9/src/cellmaps_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

