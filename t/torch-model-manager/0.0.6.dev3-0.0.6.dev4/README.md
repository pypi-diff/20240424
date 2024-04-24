# Comparing `tmp/torch_model_manager-0.0.6.dev3.tar.gz` & `tmp/torch_model_manager-0.0.6.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.0.6.dev3.tar", last modified: Wed Apr 24 10:57:22 2024, max compression
+gzip compressed data, was "torch_model_manager-0.0.6.dev4.tar", last modified: Wed Apr 24 11:02:09 2024, max compression
```

## Comparing `torch_model_manager-0.0.6.dev3.tar` & `torch_model_manager-0.0.6.dev4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 10:57:22.230338 torch_model_manager-0.0.6.dev3/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 10:57:22.226338 torch_model_manager-0.0.6.dev3/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev3/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-24 10:57:22.230338 torch_model_manager-0.0.6.dev3/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)      976 2024-04-24 10:57:15.000000 torch_model_manager-0.0.6.dev3/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 10:57:22.218337 torch_model_manager-0.0.6.dev3/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 10:57:22.222338 torch_model_manager-0.0.6.dev3/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev3/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev3/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 10:57:22.222338 torch_model_manager-0.0.6.dev3/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev3/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev3/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 10:57:22.226338 torch_model_manager-0.0.6.dev3/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev3/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3580 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev3/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16400 2024-04-24 10:52:24.000000 torch_model_manager-0.0.6.dev3/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 10:57:22.226338 torch_model_manager-0.0.6.dev3/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 10:57:22.000000 torch_model_manager-0.0.6.dev3/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-04-24 10:57:22.000000 torch_model_manager-0.0.6.dev3/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-24 10:57:22.000000 torch_model_manager-0.0.6.dev3/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-24 10:57:22.000000 torch_model_manager-0.0.6.dev3/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-24 10:57:22.000000 torch_model_manager-0.0.6.dev3/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 10:57:22.226338 torch_model_manager-0.0.6.dev3/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev3/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     5834 2024-04-24 10:50:30.000000 torch_model_manager-0.0.6.dev3/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:02:09.715074 torch_model_manager-0.0.6.dev4/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 11:02:09.715074 torch_model_manager-0.0.6.dev4/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev4/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-24 11:02:09.715074 torch_model_manager-0.0.6.dev4/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)      976 2024-04-24 11:02:06.000000 torch_model_manager-0.0.6.dev4/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:02:09.707074 torch_model_manager-0.0.6.dev4/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:02:09.707074 torch_model_manager-0.0.6.dev4/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev4/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev4/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:02:09.707074 torch_model_manager-0.0.6.dev4/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev4/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev4/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:02:09.711074 torch_model_manager-0.0.6.dev4/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev4/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3580 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev4/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16394 2024-04-24 11:01:59.000000 torch_model_manager-0.0.6.dev4/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:02:09.715074 torch_model_manager-0.0.6.dev4/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 11:02:09.000000 torch_model_manager-0.0.6.dev4/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-04-24 11:02:09.000000 torch_model_manager-0.0.6.dev4/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-24 11:02:09.000000 torch_model_manager-0.0.6.dev4/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-24 11:02:09.000000 torch_model_manager-0.0.6.dev4/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-24 11:02:09.000000 torch_model_manager-0.0.6.dev4/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:02:09.715074 torch_model_manager-0.0.6.dev4/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev4/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     5834 2024-04-24 10:50:30.000000 torch_model_manager-0.0.6.dev4/utils/helpers.py
```

### Comparing `torch_model_manager-0.0.6.dev3/PKG-INFO` & `torch_model_manager-0.0.6.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.6.dev3
+Version: 0.0.6.dev4
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.0.6.dev3/README.md` & `torch_model_manager-0.0.6.dev4/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev3/setup.py` & `torch_model_manager-0.0.6.dev4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.0.6.dev3',
+    version='0.0.6.dev4',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 'docs', 'build.sh', 'requirements.sh', 'resources.md']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Billal-MOKHTARI/torch-model-manager',
```

### Comparing `torch_model_manager-0.0.6.dev3/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.0.6.dev4/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev3/tests/test_utils/test_helpers.py` & `torch_model_manager-0.0.6.dev4/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev3/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.0.6.dev4/torch_model_manager/neptune_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev3/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.0.6.dev4/torch_model_manager/torch_model_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,13 +438,13 @@
 
         if run is not None:
             assert image_workspace is not None, "Please provide a workspace name for the images"
             for res_row, row_ind in zip(result, row_index):
                 neptune_manager.log_tensors(run, 
                                             res_row, 
                                             workspace = helpers.concatenate_with_character(col_index, f"{row_ind} -> ", mode='pre'), 
-                                            image_workspace=image_workspace, 
+                                            workspace=image_workspace, 
                                             on_series=True)
                 
 
         return result, row_index, col_index
```

### Comparing `torch_model_manager-0.0.6.dev3/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.0.6.dev4/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.6.dev3
+Version: 0.0.6.dev4
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.0.6.dev3/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.0.6.dev4/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev3/utils/helpers.py` & `torch_model_manager-0.0.6.dev4/utils/helpers.py`

 * *Files identical despite different names*

