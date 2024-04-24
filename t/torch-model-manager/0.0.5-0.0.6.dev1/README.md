# Comparing `tmp/torch-model-manager-0.0.5.tar.gz` & `tmp/torch_model_manager-0.0.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-model-manager-0.0.5.tar", last modified: Wed Apr  3 00:46:10 2024, max compression
+gzip compressed data, was "torch_model_manager-0.0.6.dev1.tar", last modified: Wed Apr 24 08:51:21 2024, max compression
```

## Comparing `torch-model-manager-0.0.5.tar` & `torch_model_manager-0.0.6.dev1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:46:10.155179 torch-model-manager-0.0.5/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8694 2024-04-03 00:46:10.155179 torch-model-manager-0.0.5/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-03 00:37:24.000000 torch-model-manager-0.0.5/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-03 00:46:10.155179 torch-model-manager-0.0.5/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)      936 2024-04-03 00:43:00.000000 torch-model-manager-0.0.5/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:46:10.123179 torch-model-manager-0.0.5/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:46:10.127179 torch-model-manager-0.0.5/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.5/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-02 21:24:16.000000 torch-model-manager-0.0.5/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:46:10.127179 torch-model-manager-0.0.5/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.5/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-02 16:34:05.000000 torch-model-manager-0.0.5/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:46:10.127179 torch-model-manager-0.0.5/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       50 2024-04-02 21:41:02.000000 torch-model-manager-0.0.5/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    11669 2024-04-02 16:34:05.000000 torch-model-manager-0.0.5/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:46:10.155179 torch-model-manager-0.0.5/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8694 2024-04-03 00:46:10.000000 torch-model-manager-0.0.5/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      506 2024-04-03 00:46:10.000000 torch-model-manager-0.0.5/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-03 00:46:10.000000 torch-model-manager-0.0.5/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-03 00:46:10.000000 torch-model-manager-0.0.5/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-03 00:46:10.000000 torch-model-manager-0.0.5/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-03 00:46:10.151179 torch-model-manager-0.0.5/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.5/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1585 2024-04-02 16:34:05.000000 torch-model-manager-0.0.5/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:51:21.755025 torch_model_manager-0.0.6.dev1/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 08:51:21.755025 torch_model_manager-0.0.6.dev1/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev1/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-24 08:51:21.755025 torch_model_manager-0.0.6.dev1/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)      976 2024-04-24 08:50:56.000000 torch_model_manager-0.0.6.dev1/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:51:21.747024 torch_model_manager-0.0.6.dev1/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:51:21.751025 torch_model_manager-0.0.6.dev1/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev1/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev1/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:51:21.751025 torch_model_manager-0.0.6.dev1/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev1/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev1/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:51:21.751025 torch_model_manager-0.0.6.dev1/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev1/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3580 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev1/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16038 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev1/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:51:21.755025 torch_model_manager-0.0.6.dev1/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 08:51:21.000000 torch_model_manager-0.0.6.dev1/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-04-24 08:51:21.000000 torch_model_manager-0.0.6.dev1/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-24 08:51:21.000000 torch_model_manager-0.0.6.dev1/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-24 08:51:21.000000 torch_model_manager-0.0.6.dev1/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-24 08:51:21.000000 torch_model_manager-0.0.6.dev1/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:51:21.755025 torch_model_manager-0.0.6.dev1/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev1/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     5503 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev1/utils/helpers.py
```

### Comparing `torch-model-manager-0.0.5/PKG-INFO` & `torch_model_manager-0.0.6.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.5
+Version: 0.0.6.dev1
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch-model-manager-0.0.5/README.md` & `torch_model_manager-0.0.6.dev1/README.md`

 * *Files identical despite different names*

### Comparing `torch-model-manager-0.0.5/setup.py` & `torch_model_manager-0.0.6.dev1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.0.5',
+    version='0.0.6.dev1',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
-    packages=find_packages(exclude=['tests', 'docs', 'build.sh']),
+    packages=find_packages(exclude=['tests', 'docs', 'build.sh', 'requirements.sh', 'resources.md']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Billal-MOKHTARI/torch-model-manager',
     keywords=['PyTorch', 'Deep Learning', 'Machine Learning', 'High Level Programming'],
     install_requires=[
         'torch',
         'numpy',
```

### Comparing `torch-model-manager-0.0.5/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.0.6.dev1/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch-model-manager-0.0.5/tests/test_utils/test_helpers.py` & `torch_model_manager-0.0.6.dev1/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch-model-manager-0.0.5/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.0.6.dev1/torch_model_manager/torch_model_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,20 @@
-import torchvision.models as models
+
 from torch import nn
 import os
 import sys
 import numpy as np
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '../')))
 from utils import helpers
+from typing import List
+from torchviz import make_dot
+import torch
+from torchvision import transforms
+from torchcam.methods import LayerCAM
+import neptune_manager as nm
 
 class TorchModelManager:
     """
     A class for managing PyTorch models.
 
     Attributes:
         model: The PyTorch model to manage.
@@ -19,16 +25,17 @@
         """
         Initialize PyModelManager with a given PyTorch model.
 
         Args:
             model (nn.Module): The PyTorch model to manage.
         """
         self.model = model
-        self.named_layers = dict()
-    
+        self.named_layers = self.get_named_layers()
+        self.model_depth = self.get_model_depth()
+
     def get_named_layers(self) -> dict:
         """
         Recursively fetch and store all named layers of the model.
 
         Returns:
             dict: A dictionary containing the named layers of the model.
         """
@@ -48,14 +55,23 @@
                 else:
                     model_children[name] = layer
             self.named_layers = model_children
             return self.named_layers
         
         return get_layers_recursive(dict(self.model.named_children()))
 
+    def get_model_depth(self):
+
+        def dict_depth(dictionary):
+            if not isinstance(dictionary, dict) or not dictionary:
+                return 0
+            return 1 + max(dict_depth(value) for value in dictionary.values())
+        
+        return dict_depth(self.named_layers)
+
     def get_attribute(self, layer: nn.Module, attribute: str) -> any:
         """
         Get a specific attribute of a layer.
 
         Args:
             layer (nn.Module): The layer.
             attribute (str): The attribute name.
@@ -203,15 +219,15 @@
                         tmp_statement_result = search_result
                         first_iter = False
                     else:
                         tmp_statement_result = helpers.union_dicts(tmp_statement_result, search_result)
             result = helpers.union_dicts(result, tmp_statement_result)
         return result
                     
-    def get_layer_by_instance(self, instance_type: type) -> dict:
+    def get_layer_by_instance(self, instance_type: List[type]) -> dict:
         """
         Search for layers in the model by their instance type.
 
         Args:
             instance_type (type): The instance type of the layers to search for.
 
         Returns:
@@ -219,15 +235,15 @@
         """
         def dfs(self, model, instance_type, layers, indexes, tmp=None, depth=0):
             if tmp is None:
                 tmp = []
 
             for name, layer in model.named_children():
                 tmp.append(name)
-                if isinstance(layer, instance_type):
+                if helpers.is_instance_of(layer, instance_type):
                     layers.append(layer)
                     indexes.append(tmp.copy())
 
                 # Recursive call
                 dfs(self, layer, instance_type, layers, indexes, tmp, depth + 1)
 
                 # Pop the last element to backtrack
@@ -236,14 +252,47 @@
         layers = []
         indexes = []
 
         dfs(self, self.model, instance_type, layers, indexes)
 
         return helpers.create_dictionary(helpers.convert_to_int(indexes), layers)    
 
+    def get_layer_by_depth(self, depth: int) -> dict:
+        """
+        Retrieves layers from the model that are at a specific depth.
+
+        Args:
+            depth (int): The depth at which the layers are located.
+
+        Returns:
+            dict: A dictionary mapping the indexes of the layers to the corresponding layer objects.
+        """
+        def dfs(self, model, depth, layers, indexes, tmp=None, current_depth=0):
+            if tmp is None:
+                tmp = []
+
+            for name, layer in model.named_children():
+                tmp.append(name)
+                if current_depth == depth:
+                    layers.append(layer)
+                    indexes.append(tmp.copy())
+                else:
+                    dfs(self, layer, depth, layers, indexes, tmp, current_depth + 1)
+
+                # Pop the last element to backtrack
+                tmp.pop()
+
+        layers = []
+        indexes = []
+
+        dfs(self, self.model, depth, layers, indexes)
+
+        return helpers.create_dictionary(helpers.convert_to_int(indexes), layers)
+
+
     def delete_layer_by_index(self, index: list) -> None:
         """
         Delete a layer from the model using its index.
 
         Args:
             index (list): The index path of the layer in the model.
         """
@@ -295,19 +344,102 @@
         search_res = self.get_layer_by_attributes(conditions)
 
         while list(search_res.keys()) != []:
             self.delete_layer_by_index(list(search_res.keys())[0])
             search_res = self.get_layer_by_attributes(conditions)
 
 
-    def delete_layer_by_instance(self, instance_type: type) -> None:
+    def delete_layer_by_instance(self, instance_types: List[type]) -> None:
         """
         Delete layers from the model by their instance type.
 
         Args:
             instance_type (type): The instance type of the layers to delete.
         """
-        search_res = self.get_layer_by_instance(instance_type)
+        search_res = self.get_layer_by_instance(instance_types)
  
         while list(search_res.keys()) != []:
             self.delete_layer_by_index(list(search_res.keys())[0])
-            search_res = self.get_layer_by_instance(instance_type)
+            search_res = self.get_layer_by_instance(instance_types)
+
+    def get_layers_by_indexes(self, indexes: List[list]) -> List:
+        """
+        Get layers from the model using their indexes.
+
+        Args:
+            indexes (List[list]): A list of indexes of the layers in the model.
+
+        Returns:
+            dict: A dictionary containing the layers from the model.
+        """
+        layers = []
+        for index in indexes:
+            layers.append(self.get_layer_by_index(index))
+        return layers
+
+    def delete_layers_by_indexes(self, indexes: List[list]) -> None:
+        """
+        Delete layers from the model using their indexes.
+
+        Args:
+            indexes (List[list]): A list of indexes of the layers in the model.
+        """
+        for index in indexes:
+            self.delete_layer_by_index(index)
+
+    def visualize(self, shape, show_attrs: bool = True, show_saved: bool = True, **kwargs) -> None:
+        x = torch.randn(shape)
+        make_dot(self.model(x), 
+                 params=dict(self.model.named_parameters()), 
+                 show_attrs=show_attrs, show_saved=show_saved).render(kwargs)
+        
+
+
+    def show_hidden_layers(self, 
+                           input_data: torch.Tensor, 
+                           indexes, 
+                           row_index: List[str] = None, 
+                           show_figure: bool = True, 
+                           figure_factor: float = 1.0,
+                           save_path = None,
+                           run = None,
+                           image_workspace = None) :
+        result = []
+        layers = self.get_layers_by_indexes(indexes)
+
+        for im in input_data:
+            tmp_model = self.model.eval()
+
+            layer_extractor = LayerCAM(tmp_model, layers)
+            out = tmp_model(im.unsqueeze(0))
+ 
+            cams = layer_extractor(out.squeeze(0).argmax().item(), out)
+            
+            result.append(cams)
+
+        if row_index is None:
+            row_index = np.arange(input_data.shape[0])
+        
+        col_index = [helpers.parse_list(index, joiner='->') for index in indexes]
+
+
+        if show_figure:
+            helpers.show_images_with_indices(result, row_index, col_index, figure_factor=figure_factor)
+
+
+
+        figure = helpers.resize_and_concat_images(result)
+        if save_path is not None:
+            to_pil = transforms.ToPILImage()
+            pil_image = to_pil(figure)
+
+            # Save the PIL image to disk
+            pil_image.save(save_path)
+
+        if run is not None:
+            assert image_workspace is not None, "Please provide a workspace name for the images"
+            for res_row in result:
+                nm.log_tensors(run, res_row, workspace = image_workspace, on_series=True)
+                
+
+        return result, row_index, col_index
+
```

### Comparing `torch-model-manager-0.0.5/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.0.6.dev1/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.5
+Version: 0.0.6.dev1
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

