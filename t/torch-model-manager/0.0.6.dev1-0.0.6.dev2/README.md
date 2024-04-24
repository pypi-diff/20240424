# Comparing `tmp/torch_model_manager-0.0.6.dev1.tar.gz` & `tmp/torch_model_manager-0.0.6.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.0.6.dev1.tar", last modified: Wed Apr 24 08:51:21 2024, max compression
+gzip compressed data, was "torch_model_manager-0.0.6.dev2.tar", last modified: Wed Apr 24 09:11:04 2024, max compression
```

## Comparing `torch_model_manager-0.0.6.dev1.tar` & `torch_model_manager-0.0.6.dev2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:51:21.755025 torch_model_manager-0.0.6.dev1/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 08:51:21.755025 torch_model_manager-0.0.6.dev1/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev1/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-24 08:51:21.755025 torch_model_manager-0.0.6.dev1/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)      976 2024-04-24 08:50:56.000000 torch_model_manager-0.0.6.dev1/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:51:21.747024 torch_model_manager-0.0.6.dev1/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:51:21.751025 torch_model_manager-0.0.6.dev1/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev1/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev1/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:51:21.751025 torch_model_manager-0.0.6.dev1/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev1/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev1/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:51:21.751025 torch_model_manager-0.0.6.dev1/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev1/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3580 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev1/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16038 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev1/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:51:21.755025 torch_model_manager-0.0.6.dev1/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 08:51:21.000000 torch_model_manager-0.0.6.dev1/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-04-24 08:51:21.000000 torch_model_manager-0.0.6.dev1/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-24 08:51:21.000000 torch_model_manager-0.0.6.dev1/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-24 08:51:21.000000 torch_model_manager-0.0.6.dev1/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-24 08:51:21.000000 torch_model_manager-0.0.6.dev1/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:51:21.755025 torch_model_manager-0.0.6.dev1/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev1/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     5503 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev1/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 09:11:04.691149 torch_model_manager-0.0.6.dev2/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 09:11:04.691149 torch_model_manager-0.0.6.dev2/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev2/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-24 09:11:04.691149 torch_model_manager-0.0.6.dev2/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)      976 2024-04-24 09:10:19.000000 torch_model_manager-0.0.6.dev2/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 09:11:04.683149 torch_model_manager-0.0.6.dev2/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 09:11:04.683149 torch_model_manager-0.0.6.dev2/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev2/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev2/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 09:11:04.683149 torch_model_manager-0.0.6.dev2/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev2/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev2/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 09:11:04.687149 torch_model_manager-0.0.6.dev2/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev2/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3580 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev2/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16073 2024-04-24 09:09:00.000000 torch_model_manager-0.0.6.dev2/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 09:11:04.691149 torch_model_manager-0.0.6.dev2/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 09:11:04.000000 torch_model_manager-0.0.6.dev2/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-04-24 09:11:04.000000 torch_model_manager-0.0.6.dev2/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-24 09:11:04.000000 torch_model_manager-0.0.6.dev2/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-24 09:11:04.000000 torch_model_manager-0.0.6.dev2/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-24 09:11:04.000000 torch_model_manager-0.0.6.dev2/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 09:11:04.687149 torch_model_manager-0.0.6.dev2/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev2/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     5503 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev2/utils/helpers.py
```

### Comparing `torch_model_manager-0.0.6.dev1/PKG-INFO` & `torch_model_manager-0.0.6.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.6.dev1
+Version: 0.0.6.dev2
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.0.6.dev1/README.md` & `torch_model_manager-0.0.6.dev2/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev1/setup.py` & `torch_model_manager-0.0.6.dev2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.0.6.dev1',
+    version='0.0.6.dev2',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 'docs', 'build.sh', 'requirements.sh', 'resources.md']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Billal-MOKHTARI/torch-model-manager',
```

### Comparing `torch_model_manager-0.0.6.dev1/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.0.6.dev2/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev1/tests/test_utils/test_helpers.py` & `torch_model_manager-0.0.6.dev2/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev1/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.0.6.dev2/torch_model_manager/neptune_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev1/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.0.6.dev2/torch_model_manager/torch_model_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '../')))
 from utils import helpers
 from typing import List
 from torchviz import make_dot
 import torch
 from torchvision import transforms
 from torchcam.methods import LayerCAM
-import neptune_manager as nm
 
 class TorchModelManager:
     """
     A class for managing PyTorch models.
 
     Attributes:
         model: The PyTorch model to manage.
@@ -397,14 +396,15 @@
     def show_hidden_layers(self, 
                            input_data: torch.Tensor, 
                            indexes, 
                            row_index: List[str] = None, 
                            show_figure: bool = True, 
                            figure_factor: float = 1.0,
                            save_path = None,
+                           neptune_manager = None,
                            run = None,
                            image_workspace = None) :
         result = []
         layers = self.get_layers_by_indexes(indexes)
 
         for im in input_data:
             tmp_model = self.model.eval()
@@ -434,12 +434,12 @@
 
             # Save the PIL image to disk
             pil_image.save(save_path)
 
         if run is not None:
             assert image_workspace is not None, "Please provide a workspace name for the images"
             for res_row in result:
-                nm.log_tensors(run, res_row, workspace = image_workspace, on_series=True)
+                neptune_manager.log_tensors(run, res_row, workspace = image_workspace, on_series=True)
                 
 
         return result, row_index, col_index
```

### Comparing `torch_model_manager-0.0.6.dev1/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.0.6.dev2/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.6.dev1
+Version: 0.0.6.dev2
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.0.6.dev1/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.0.6.dev2/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev1/utils/helpers.py` & `torch_model_manager-0.0.6.dev2/utils/helpers.py`

 * *Files identical despite different names*

