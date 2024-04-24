# Comparing `tmp/torch_model_manager-0.0.6.dev5.tar.gz` & `tmp/torch_model_manager-0.0.6.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.0.6.dev5.tar", last modified: Wed Apr 24 11:04:16 2024, max compression
+gzip compressed data, was "torch_model_manager-0.0.6.dev6.tar", last modified: Wed Apr 24 11:07:36 2024, max compression
```

## Comparing `torch_model_manager-0.0.6.dev5.tar` & `torch_model_manager-0.0.6.dev6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:04:16.749353 torch_model_manager-0.0.6.dev5/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 11:04:16.749353 torch_model_manager-0.0.6.dev5/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev5/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-24 11:04:16.749353 torch_model_manager-0.0.6.dev5/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)      976 2024-04-24 11:04:11.000000 torch_model_manager-0.0.6.dev5/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:04:16.741353 torch_model_manager-0.0.6.dev5/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:04:16.745353 torch_model_manager-0.0.6.dev5/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev5/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev5/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:04:16.745353 torch_model_manager-0.0.6.dev5/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev5/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev5/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:04:16.745353 torch_model_manager-0.0.6.dev5/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev5/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3580 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev5/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16323 2024-04-24 11:03:35.000000 torch_model_manager-0.0.6.dev5/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:04:16.749353 torch_model_manager-0.0.6.dev5/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 11:04:16.000000 torch_model_manager-0.0.6.dev5/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-04-24 11:04:16.000000 torch_model_manager-0.0.6.dev5/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-24 11:04:16.000000 torch_model_manager-0.0.6.dev5/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-24 11:04:16.000000 torch_model_manager-0.0.6.dev5/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-24 11:04:16.000000 torch_model_manager-0.0.6.dev5/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:04:16.749353 torch_model_manager-0.0.6.dev5/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev5/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     5834 2024-04-24 10:50:30.000000 torch_model_manager-0.0.6.dev5/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:07:36.958859 torch_model_manager-0.0.6.dev6/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 11:07:36.958859 torch_model_manager-0.0.6.dev6/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev6/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-24 11:07:36.958859 torch_model_manager-0.0.6.dev6/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)      976 2024-04-24 11:07:14.000000 torch_model_manager-0.0.6.dev6/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:07:36.950858 torch_model_manager-0.0.6.dev6/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:07:36.954858 torch_model_manager-0.0.6.dev6/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev6/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev6/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:07:36.954858 torch_model_manager-0.0.6.dev6/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev6/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev6/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:07:36.954858 torch_model_manager-0.0.6.dev6/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev6/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3790 2024-04-24 11:07:08.000000 torch_model_manager-0.0.6.dev6/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16323 2024-04-24 11:03:35.000000 torch_model_manager-0.0.6.dev6/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:07:36.958859 torch_model_manager-0.0.6.dev6/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8699 2024-04-24 11:07:36.000000 torch_model_manager-0.0.6.dev6/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-04-24 11:07:36.000000 torch_model_manager-0.0.6.dev6/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-24 11:07:36.000000 torch_model_manager-0.0.6.dev6/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-24 11:07:36.000000 torch_model_manager-0.0.6.dev6/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-24 11:07:36.000000 torch_model_manager-0.0.6.dev6/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 11:07:36.958859 torch_model_manager-0.0.6.dev6/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.0.6.dev6/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     5834 2024-04-24 10:50:30.000000 torch_model_manager-0.0.6.dev6/utils/helpers.py
```

### Comparing `torch_model_manager-0.0.6.dev5/PKG-INFO` & `torch_model_manager-0.0.6.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.6.dev5
+Version: 0.0.6.dev6
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.0.6.dev5/README.md` & `torch_model_manager-0.0.6.dev6/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev5/setup.py` & `torch_model_manager-0.0.6.dev6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.0.6.dev5',
+    version='0.0.6.dev6',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 'docs', 'build.sh', 'requirements.sh', 'resources.md']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Billal-MOKHTARI/torch-model-manager',
```

### Comparing `torch_model_manager-0.0.6.dev5/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.0.6.dev6/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev5/tests/test_utils/test_helpers.py` & `torch_model_manager-0.0.6.dev6/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev5/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.0.6.dev6/torch_model_manager/neptune_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,13 +81,17 @@
     
     def log_tensors(self, run, tensors, descriptions = None, names = None, paths = None, workspace = None, on_series = False):
         to_pil = transforms.ToPILImage()
         if not on_series:
             for path, tensor in zip(paths, tensors) :
                 run[path].upload(File.as_image(to_pil(tensor)))
         else:
-            for name, description, tensor in zip(names, descriptions, tensors):
-                run[workspace].append(File.as_image(to_pil(tensor)), name = name, description = description)
+            if descriptions is not None:
+                for name, description, tensor in zip(names, descriptions, tensors):
+                    run[workspace].append(File.as_image(to_pil(tensor)), name = name, description = description)
+            else:
+                for name, tensor in zip(names, tensors):
+                    run[workspace].append(File.as_image(to_pil(tensor)), name = name)
 
     def delete_data(self, run, workspaces):
         for workspace in workspaces:
             run.pop(workspace)
```

### Comparing `torch_model_manager-0.0.6.dev5/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.0.6.dev6/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev5/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.0.6.dev6/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.6.dev5
+Version: 0.0.6.dev6
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.0.6.dev5/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.0.6.dev6/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.0.6.dev5/utils/helpers.py` & `torch_model_manager-0.0.6.dev6/utils/helpers.py`

 * *Files identical despite different names*

