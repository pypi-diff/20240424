# Comparing `tmp/torch_model_manager-0.0.6.dev8.tar.gz` & `tmp/torch_model_manager-0.0.6.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.0.6.dev8.tar", last modified: Wed Apr 24 16:53:00 2024, max compression
+gzip compressed data, was "torch_model_manager-0.0.6.dev9.tar", last modified: Wed Apr 24 17:04:20 2024, max compression
```

## Comparing `torch_model_manager-0.0.6.dev8.tar` & `torch_model_manager-0.0.6.dev9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 16:53:00.362551 torch_model_manager-0.0.6.dev8/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 16:53:00.362551 torch_model_manager-0.0.6.dev8/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev8/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-24 16:53:00.362551 torch_model_manager-0.0.6.dev8/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)      976 2024-04-24 16:52:54.000000 torch_model_manager-0.0.6.dev8/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 16:53:00.354551 torch_model_manager-0.0.6.dev8/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 16:53:00.358551 torch_model_manager-0.0.6.dev8/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev8/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev8/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 16:53:00.358551 torch_model_manager-0.0.6.dev8/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev8/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev8/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 16:53:00.358551 torch_model_manager-0.0.6.dev8/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev8/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     4030 2024-04-24 16:47:30.000000 torch_model_manager-0.0.6.dev8/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16969 2024-04-24 16:47:11.000000 torch_model_manager-0.0.6.dev8/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 16:53:00.362551 torch_model_manager-0.0.6.dev8/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 16:53:00.000000 torch_model_manager-0.0.6.dev8/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-04-24 16:53:00.000000 torch_model_manager-0.0.6.dev8/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-24 16:53:00.000000 torch_model_manager-0.0.6.dev8/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-24 16:53:00.000000 torch_model_manager-0.0.6.dev8/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-24 16:53:00.000000 torch_model_manager-0.0.6.dev8/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 16:53:00.362551 torch_model_manager-0.0.6.dev8/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev8/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     5834 2024-04-24 10:50:30.000000 torch_model_manager-0.0.6.dev8/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 17:04:20.324792 torch_model_manager-0.0.6.dev9/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 17:04:20.320792 torch_model_manager-0.0.6.dev9/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev9/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-24 17:04:20.324792 torch_model_manager-0.0.6.dev9/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)      976 2024-04-24 17:03:55.000000 torch_model_manager-0.0.6.dev9/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 17:04:20.316792 torch_model_manager-0.0.6.dev9/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 17:04:20.320792 torch_model_manager-0.0.6.dev9/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev9/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev9/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 17:04:20.320792 torch_model_manager-0.0.6.dev9/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev9/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev9/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 17:04:20.320792 torch_model_manager-0.0.6.dev9/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev9/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     4067 2024-04-24 17:04:15.000000 torch_model_manager-0.0.6.dev9/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16969 2024-04-24 16:47:11.000000 torch_model_manager-0.0.6.dev9/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 17:04:20.320792 torch_model_manager-0.0.6.dev9/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 17:04:20.000000 torch_model_manager-0.0.6.dev9/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-04-24 17:04:20.000000 torch_model_manager-0.0.6.dev9/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-24 17:04:20.000000 torch_model_manager-0.0.6.dev9/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-24 17:04:20.000000 torch_model_manager-0.0.6.dev9/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-24 17:04:20.000000 torch_model_manager-0.0.6.dev9/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 17:04:20.320792 torch_model_manager-0.0.6.dev9/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev9/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     5834 2024-04-24 10:50:30.000000 torch_model_manager-0.0.6.dev9/utils/helpers.py
```

### Comparing `torch_model_manager-0.0.6.dev8/PKG-INFO` & `torch_model_manager-0.0.6.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.6.dev8
+Version: 0.0.6.dev9
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.0.6.dev8/README.md` & `torch_model_manager-0.0.6.dev9/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev8/setup.py` & `torch_model_manager-0.0.6.dev9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.0.6.dev8',
+    version='0.0.6.dev9',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 'docs', 'build.sh', 'requirements.sh', 'resources.md']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Billal-MOKHTARI/torch-model-manager',
```

### Comparing `torch_model_manager-0.0.6.dev8/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.0.6.dev9/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev8/tests/test_utils/test_helpers.py` & `torch_model_manager-0.0.6.dev9/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev8/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.0.6.dev9/torch_model_manager/neptune_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,13 +93,14 @@
                 for name, tensor in zip(names, tensors):
                     run[workspace].append(File.as_image(to_pil(tensor)), name = name)
 
     def delete_data(self, run, workspaces):
         for workspace in workspaces:
             run.pop(workspace)
             
-    def log_artifacts(self, run, data, path, workspace):
+    def log_artifacts(self, run, data, path, workspace, keep=False):
         with open(path, 'wb') as f:
             pkl.dump(data, f)
         run[workspace].track_files(path)
-        os.remove(path)
+        if not keep:
+            os.remove(path)
```

### Comparing `torch_model_manager-0.0.6.dev8/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.0.6.dev9/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev8/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.0.6.dev9/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.6.dev8
+Version: 0.0.6.dev9
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.0.6.dev8/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.0.6.dev9/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev8/utils/helpers.py` & `torch_model_manager-0.0.6.dev9/utils/helpers.py`

 * *Files identical despite different names*

