# Comparing `tmp/torch_model_manager-0.0.6.dev7.tar.gz` & `tmp/torch_model_manager-0.0.6.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.0.6.dev7.tar", last modified: Wed Apr 24 11:10:49 2024, max compression
+gzip compressed data, was "torch_model_manager-0.0.6.dev8.tar", last modified: Wed Apr 24 16:53:00 2024, max compression
```

## Comparing `torch_model_manager-0.0.6.dev7.tar` & `torch_model_manager-0.0.6.dev8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:10:49.381685 torch_model_manager-0.0.6.dev7/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 11:10:49.377685 torch_model_manager-0.0.6.dev7/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev7/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-24 11:10:49.381685 torch_model_manager-0.0.6.dev7/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)      976 2024-04-24 11:10:45.000000 torch_model_manager-0.0.6.dev7/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:10:49.373685 torch_model_manager-0.0.6.dev7/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:10:49.373685 torch_model_manager-0.0.6.dev7/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev7/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev7/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:10:49.373685 torch_model_manager-0.0.6.dev7/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev7/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev7/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:10:49.377685 torch_model_manager-0.0.6.dev7/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev7/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3790 2024-04-24 11:07:08.000000 torch_model_manager-0.0.6.dev7/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16397 2024-04-24 11:10:37.000000 torch_model_manager-0.0.6.dev7/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:10:49.377685 torch_model_manager-0.0.6.dev7/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 11:10:49.000000 torch_model_manager-0.0.6.dev7/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-04-24 11:10:49.000000 torch_model_manager-0.0.6.dev7/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-24 11:10:49.000000 torch_model_manager-0.0.6.dev7/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-24 11:10:49.000000 torch_model_manager-0.0.6.dev7/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-24 11:10:49.000000 torch_model_manager-0.0.6.dev7/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:10:49.377685 torch_model_manager-0.0.6.dev7/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev7/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     5834 2024-04-24 10:50:30.000000 torch_model_manager-0.0.6.dev7/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 16:53:00.362551 torch_model_manager-0.0.6.dev8/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 16:53:00.362551 torch_model_manager-0.0.6.dev8/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev8/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-24 16:53:00.362551 torch_model_manager-0.0.6.dev8/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)      976 2024-04-24 16:52:54.000000 torch_model_manager-0.0.6.dev8/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 16:53:00.354551 torch_model_manager-0.0.6.dev8/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 16:53:00.358551 torch_model_manager-0.0.6.dev8/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev8/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev8/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 16:53:00.358551 torch_model_manager-0.0.6.dev8/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev8/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev8/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 16:53:00.358551 torch_model_manager-0.0.6.dev8/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev8/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     4030 2024-04-24 16:47:30.000000 torch_model_manager-0.0.6.dev8/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16969 2024-04-24 16:47:11.000000 torch_model_manager-0.0.6.dev8/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 16:53:00.362551 torch_model_manager-0.0.6.dev8/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 16:53:00.000000 torch_model_manager-0.0.6.dev8/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-04-24 16:53:00.000000 torch_model_manager-0.0.6.dev8/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-24 16:53:00.000000 torch_model_manager-0.0.6.dev8/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-24 16:53:00.000000 torch_model_manager-0.0.6.dev8/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-24 16:53:00.000000 torch_model_manager-0.0.6.dev8/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 16:53:00.362551 torch_model_manager-0.0.6.dev8/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev8/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     5834 2024-04-24 10:50:30.000000 torch_model_manager-0.0.6.dev8/utils/helpers.py
```

### Comparing `torch_model_manager-0.0.6.dev7/PKG-INFO` & `torch_model_manager-0.0.6.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.6.dev7
+Version: 0.0.6.dev8
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.0.6.dev7/README.md` & `torch_model_manager-0.0.6.dev8/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev7/setup.py` & `torch_model_manager-0.0.6.dev8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.0.6.dev7',
+    version='0.0.6.dev8',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 'docs', 'build.sh', 'requirements.sh', 'resources.md']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Billal-MOKHTARI/torch-model-manager',
```

### Comparing `torch_model_manager-0.0.6.dev7/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.0.6.dev8/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev7/tests/test_utils/test_helpers.py` & `torch_model_manager-0.0.6.dev8/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev7/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.0.6.dev8/torch_model_manager/neptune_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import neptune
 from neptune import management
 from neptune.types import File
 import json
 import numpy as np
 from torchvision import transforms
-
+import pickle as pkl
+import os
 class NeptuneManager:
     def __init__(self, project, api_token, run_ids_path, visibility = None, workspace=None, description=None, key=None):
         self.project = project
         self.api_token = api_token
         self.run_ids_path = run_ids_path
 
         if project not in management.get_project_list(api_token=self.api_token):
@@ -90,8 +91,15 @@
                     run[workspace].append(File.as_image(to_pil(tensor)), name = name, description = description)
             else:
                 for name, tensor in zip(names, tensors):
                     run[workspace].append(File.as_image(to_pil(tensor)), name = name)
 
     def delete_data(self, run, workspaces):
         for workspace in workspaces:
-            run.pop(workspace)
+            run.pop(workspace)
+            
+    def log_artifacts(self, run, data, path, workspace):
+        with open(path, 'wb') as f:
+            pkl.dump(data, f)
+        run[workspace].track_files(path)
+        os.remove(path)
+
```

### Comparing `torch_model_manager-0.0.6.dev7/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.0.6.dev8/torch_model_manager/torch_model_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '../')))
 from utils import helpers
 from typing import List
 from torchviz import make_dot
 import torch
 from torchvision import transforms
 from torchcam.methods import LayerCAM
+from torchvision import models
 
 class TorchModelManager:
     """
     A class for managing PyTorch models.
 
     Attributes:
         model: The PyTorch model to manage.
@@ -283,15 +284,35 @@
         layers = []
         indexes = []
 
         dfs(self, self.model, depth, layers, indexes)
 
         return helpers.create_dictionary(helpers.convert_to_int(indexes), layers)
 
+    def get_indexes(self, indexes):
+        def dfs(self, model, indexes, tmp=None, depth=0):
+            if tmp is None:
+                tmp = []
+
+            for name, _ in model.named_children():
+                tmp.append(name)
+                indexes.append(tmp.copy())
 
+                # Recursive call
+                dfs(self, indexes, tmp, depth+1)
+
+                # Pop the last element to backtrack
+                tmp.pop()
+
+        indexes = []
+        dfs(self, self.model, indexes)
+        
+        return indexes
+    
+    
     def delete_layer_by_index(self, index: list) -> None:
         """
         Delete a layer from the model using its index.
 
         Args:
             index (list): The index path of the layer in the model.
         """
@@ -444,7 +465,9 @@
                                             names = helpers.concatenate_with_character(col_index, f"{row_ind} -> ", mode='pre'), 
                                             workspace=image_workspace,
                                             on_series=True)
                 
 
         return result, row_index, col_index
     
+
+
```

### Comparing `torch_model_manager-0.0.6.dev7/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.0.6.dev8/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.6.dev7
+Version: 0.0.6.dev8
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.0.6.dev7/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.0.6.dev8/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev7/utils/helpers.py` & `torch_model_manager-0.0.6.dev8/utils/helpers.py`

 * *Files identical despite different names*

