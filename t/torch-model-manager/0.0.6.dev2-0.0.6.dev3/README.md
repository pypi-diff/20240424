# Comparing `tmp/torch_model_manager-0.0.6.dev2.tar.gz` & `tmp/torch_model_manager-0.0.6.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.0.6.dev2.tar", last modified: Wed Apr 24 09:11:04 2024, max compression
+gzip compressed data, was "torch_model_manager-0.0.6.dev3.tar", last modified: Wed Apr 24 10:57:22 2024, max compression
```

## Comparing `torch_model_manager-0.0.6.dev2.tar` & `torch_model_manager-0.0.6.dev3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 09:11:04.691149 torch_model_manager-0.0.6.dev2/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 09:11:04.691149 torch_model_manager-0.0.6.dev2/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev2/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-24 09:11:04.691149 torch_model_manager-0.0.6.dev2/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)      976 2024-04-24 09:10:19.000000 torch_model_manager-0.0.6.dev2/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 09:11:04.683149 torch_model_manager-0.0.6.dev2/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 09:11:04.683149 torch_model_manager-0.0.6.dev2/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev2/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev2/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 09:11:04.683149 torch_model_manager-0.0.6.dev2/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev2/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev2/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 09:11:04.687149 torch_model_manager-0.0.6.dev2/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev2/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3580 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev2/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16073 2024-04-24 09:09:00.000000 torch_model_manager-0.0.6.dev2/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 09:11:04.691149 torch_model_manager-0.0.6.dev2/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 09:11:04.000000 torch_model_manager-0.0.6.dev2/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-04-24 09:11:04.000000 torch_model_manager-0.0.6.dev2/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-24 09:11:04.000000 torch_model_manager-0.0.6.dev2/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-24 09:11:04.000000 torch_model_manager-0.0.6.dev2/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-24 09:11:04.000000 torch_model_manager-0.0.6.dev2/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 09:11:04.687149 torch_model_manager-0.0.6.dev2/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev2/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     5503 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev2/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 10:57:22.230338 torch_model_manager-0.0.6.dev3/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 10:57:22.226338 torch_model_manager-0.0.6.dev3/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev3/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-24 10:57:22.230338 torch_model_manager-0.0.6.dev3/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)      976 2024-04-24 10:57:15.000000 torch_model_manager-0.0.6.dev3/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 10:57:22.218337 torch_model_manager-0.0.6.dev3/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 10:57:22.222338 torch_model_manager-0.0.6.dev3/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev3/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev3/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 10:57:22.222338 torch_model_manager-0.0.6.dev3/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev3/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev3/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 10:57:22.226338 torch_model_manager-0.0.6.dev3/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev3/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3580 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev3/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16400 2024-04-24 10:52:24.000000 torch_model_manager-0.0.6.dev3/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 10:57:22.226338 torch_model_manager-0.0.6.dev3/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 10:57:22.000000 torch_model_manager-0.0.6.dev3/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-04-24 10:57:22.000000 torch_model_manager-0.0.6.dev3/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-24 10:57:22.000000 torch_model_manager-0.0.6.dev3/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-24 10:57:22.000000 torch_model_manager-0.0.6.dev3/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-24 10:57:22.000000 torch_model_manager-0.0.6.dev3/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 10:57:22.226338 torch_model_manager-0.0.6.dev3/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev3/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     5834 2024-04-24 10:50:30.000000 torch_model_manager-0.0.6.dev3/utils/helpers.py
```

### Comparing `torch_model_manager-0.0.6.dev2/PKG-INFO` & `torch_model_manager-0.0.6.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.6.dev2
+Version: 0.0.6.dev3
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.0.6.dev2/README.md` & `torch_model_manager-0.0.6.dev3/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev2/setup.py` & `torch_model_manager-0.0.6.dev3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.0.6.dev2',
+    version='0.0.6.dev3',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 'docs', 'build.sh', 'requirements.sh', 'resources.md']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Billal-MOKHTARI/torch-model-manager',
```

### Comparing `torch_model_manager-0.0.6.dev2/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.0.6.dev3/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev2/tests/test_utils/test_helpers.py` & `torch_model_manager-0.0.6.dev3/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev2/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.0.6.dev3/torch_model_manager/neptune_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev2/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.0.6.dev3/torch_model_manager/torch_model_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -398,15 +398,16 @@
                            indexes, 
                            row_index: List[str] = None, 
                            show_figure: bool = True, 
                            figure_factor: float = 1.0,
                            save_path = None,
                            neptune_manager = None,
                            run = None,
-                           image_workspace = None) :
+                           image_workspace = None,
+                           ) :
         result = []
         layers = self.get_layers_by_indexes(indexes)
 
         for im in input_data:
             tmp_model = self.model.eval()
 
             layer_extractor = LayerCAM(tmp_model, layers)
@@ -433,13 +434,17 @@
             pil_image = to_pil(figure)
 
             # Save the PIL image to disk
             pil_image.save(save_path)
 
         if run is not None:
             assert image_workspace is not None, "Please provide a workspace name for the images"
-            for res_row in result:
-                neptune_manager.log_tensors(run, res_row, workspace = image_workspace, on_series=True)
+            for res_row, row_ind in zip(result, row_index):
+                neptune_manager.log_tensors(run, 
+                                            res_row, 
+                                            workspace = helpers.concatenate_with_character(col_index, f"{row_ind} -> ", mode='pre'), 
+                                            image_workspace=image_workspace, 
+                                            on_series=True)
                 
 
         return result, row_index, col_index
```

### Comparing `torch_model_manager-0.0.6.dev2/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.0.6.dev3/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.6.dev2
+Version: 0.0.6.dev3
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.0.6.dev2/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.0.6.dev3/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev2/utils/helpers.py` & `torch_model_manager-0.0.6.dev3/utils/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,7 +162,16 @@
         # Concatenate resized images horizontally
         concatenated_images.append(torch.cat(resized_images, dim=2))
     # Concatenate sublist images vertically
     final_image = torch.cat(concatenated_images, dim=1)
     
     return final_image
 
+def concatenate_with_character(lst, char, mode='post'):
+    if mode == 'pre':
+        concatenated_list = [char + str(item) for item in lst]
+    elif mode == 'post':
+        concatenated_list = [str(item) + char for item in lst]
+    else:
+        raise ValueError("Invalid mode. Use 'pre' or 'post'.")
+
+    return concatenated_list
```

