# Comparing `tmp/hypothesis_torch-0.3.1.tar.gz` & `tmp/hypothesis_torch-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypothesis_torch-0.3.1.tar", last modified: Wed Apr 24 03:25:11 2024, max compression
+gzip compressed data, was "hypothesis_torch-0.4.0.tar", last modified: Wed Apr 24 19:46:13 2024, max compression
```

## Comparing `hypothesis_torch-0.3.1.tar` & `hypothesis_torch-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 03:25:11.333052 hypothesis_torch-0.3.1/
--rw-r--r--   0 root         (0) root         (0)     1070 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8094 2024-04-24 03:25:11.333052 hypothesis_torch-0.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5282 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 03:25:11.333052 hypothesis_torch-0.3.1/hypothesis_torch/
--rw-r--r--   0 root         (0) root         (0)     1240 2024-04-24 03:25:08.000000 hypothesis_torch-0.3.1/hypothesis_torch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1408 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/hypothesis_torch/device.py
--rw-r--r--   0 root         (0) root         (0)     2491 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/hypothesis_torch/dtype.py
--rw-r--r--   0 root         (0) root         (0)     3922 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/hypothesis_torch/huggingface.py
--rw-r--r--   0 root         (0) root         (0)     1977 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/hypothesis_torch/inspection_util.py
--rw-r--r--   0 root         (0) root         (0)      735 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/hypothesis_torch/layout.py
--rw-r--r--   0 root         (0) root         (0)      846 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/hypothesis_torch/memory_format.py
--rw-r--r--   0 root         (0) root         (0)    10903 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/hypothesis_torch/module.py
--rw-r--r--   0 root         (0) root         (0)     7873 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/hypothesis_torch/tensor.py
--rw-r--r--   0 root         (0) root         (0)     1442 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/hypothesis_torch/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 03:25:11.333052 hypothesis_torch-0.3.1/hypothesis_torch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8094 2024-04-24 03:25:11.000000 hypothesis_torch-0.3.1/hypothesis_torch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      522 2024-04-24 03:25:11.000000 hypothesis_torch-0.3.1/hypothesis_torch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 03:25:11.000000 hypothesis_torch-0.3.1/hypothesis_torch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       96 2024-04-24 03:25:11.000000 hypothesis_torch-0.3.1/hypothesis_torch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-24 03:25:11.000000 hypothesis_torch-0.3.1/hypothesis_torch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2099 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 03:25:11.333052 hypothesis_torch-0.3.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:46:13.048545 hypothesis_torch-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-04-24 19:45:37.000000 hypothesis_torch-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8094 2024-04-24 19:46:13.048545 hypothesis_torch-0.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5282 2024-04-24 19:45:37.000000 hypothesis_torch-0.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:46:13.044545 hypothesis_torch-0.4.0/hypothesis_torch/
+-rw-r--r--   0 root         (0) root         (0)     1319 2024-04-24 19:46:09.000000 hypothesis_torch-0.4.0/hypothesis_torch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2024-04-24 19:45:37.000000 hypothesis_torch-0.4.0/hypothesis_torch/device.py
+-rw-r--r--   0 root         (0) root         (0)     2491 2024-04-24 19:45:37.000000 hypothesis_torch-0.4.0/hypothesis_torch/dtype.py
+-rw-r--r--   0 root         (0) root         (0)     3922 2024-04-24 19:45:37.000000 hypothesis_torch-0.4.0/hypothesis_torch/huggingface.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2024-04-24 19:45:37.000000 hypothesis_torch-0.4.0/hypothesis_torch/inspection_util.py
+-rw-r--r--   0 root         (0) root         (0)      735 2024-04-24 19:45:37.000000 hypothesis_torch-0.4.0/hypothesis_torch/layout.py
+-rw-r--r--   0 root         (0) root         (0)      846 2024-04-24 19:45:37.000000 hypothesis_torch-0.4.0/hypothesis_torch/memory_format.py
+-rw-r--r--   0 root         (0) root         (0)    10903 2024-04-24 19:45:37.000000 hypothesis_torch-0.4.0/hypothesis_torch/module.py
+-rw-r--r--   0 root         (0) root         (0)      866 2024-04-24 19:45:37.000000 hypothesis_torch-0.4.0/hypothesis_torch/register_random_torch_state.py
+-rw-r--r--   0 root         (0) root         (0)     7873 2024-04-24 19:45:37.000000 hypothesis_torch-0.4.0/hypothesis_torch/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2024-04-24 19:45:37.000000 hypothesis_torch-0.4.0/hypothesis_torch/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:46:13.048545 hypothesis_torch-0.4.0/hypothesis_torch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8094 2024-04-24 19:46:13.000000 hypothesis_torch-0.4.0/hypothesis_torch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      613 2024-04-24 19:46:13.000000 hypothesis_torch-0.4.0/hypothesis_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 19:46:13.000000 hypothesis_torch-0.4.0/hypothesis_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2024-04-24 19:46:13.000000 hypothesis_torch-0.4.0/hypothesis_torch.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2024-04-24 19:46:13.000000 hypothesis_torch-0.4.0/hypothesis_torch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-24 19:46:13.000000 hypothesis_torch-0.4.0/hypothesis_torch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2215 2024-04-24 19:45:37.000000 hypothesis_torch-0.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 19:46:13.048545 hypothesis_torch-0.4.0/setup.cfg
```

### Comparing `hypothesis_torch-0.3.1/LICENSE` & `hypothesis_torch-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.3.1/PKG-INFO` & `hypothesis_torch-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.3.1
+Version: 0.4.0
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `hypothesis_torch-0.3.1/README.md` & `hypothesis_torch-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.3.1/hypothesis_torch/__init__.py` & `hypothesis_torch-0.4.0/hypothesis_torch/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Hypothesis strategies for various Pytorch structures (including tensors and modules).
 
 [Hypothesis](https://hypothesis.readthedocs.io/en/latest/) is a powerful property-based testing library for Python. It
 lacks built-in support for Pytorch tensors and modules, so this library provides strategies for generating them.
 """
 
-__version__ = "0.3.1"
+__version__ = "0.4.0"
 import importlib.util
 
 from hypothesis_torch.device import (
     device_strategy,
     AVAILABLE_CPU_DEVICES,
     AVAILABLE_CUDA_DEVICES,
     AVAILABLE_MPS_DEVICES,
@@ -25,12 +25,14 @@
     COMPLEX_DTYPES,
     BOOL_DTYPES,
     ALL_DTYPES,
 )
 from hypothesis_torch.layout import layout_strategy
 from hypothesis_torch.memory_format import memory_format_strategy
 from hypothesis_torch.module import linear_network_strategy, same_shape_activation_strategy
+from hypothesis_torch.register_random_torch_state import TORCH_RANDOM_WRAPPER
 from hypothesis_torch.tensor import tensor_strategy
 
+
 if importlib.util.find_spec("transformers") is not None:
     # Import Hugging Face strategies if transformers is installed
     from hypothesis_torch.huggingface import transformer_strategy
```

### Comparing `hypothesis_torch-0.3.1/hypothesis_torch/device.py` & `hypothesis_torch-0.4.0/hypothesis_torch/device.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.3.1/hypothesis_torch/dtype.py` & `hypothesis_torch-0.4.0/hypothesis_torch/dtype.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.3.1/hypothesis_torch/huggingface.py` & `hypothesis_torch-0.4.0/hypothesis_torch/huggingface.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.3.1/hypothesis_torch/inspection_util.py` & `hypothesis_torch-0.4.0/hypothesis_torch/inspection_util.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.3.1/hypothesis_torch/layout.py` & `hypothesis_torch-0.4.0/hypothesis_torch/layout.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.3.1/hypothesis_torch/memory_format.py` & `hypothesis_torch-0.4.0/hypothesis_torch/memory_format.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.3.1/hypothesis_torch/module.py` & `hypothesis_torch-0.4.0/hypothesis_torch/module.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.3.1/hypothesis_torch/tensor.py` & `hypothesis_torch-0.4.0/hypothesis_torch/tensor.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.3.1/hypothesis_torch/utils.py` & `hypothesis_torch-0.4.0/hypothesis_torch/utils.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.3.1/hypothesis_torch.egg-info/PKG-INFO` & `hypothesis_torch-0.4.0/hypothesis_torch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.3.1
+Version: 0.4.0
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `hypothesis_torch-0.3.1/hypothesis_torch.egg-info/SOURCES.txt` & `hypothesis_torch-0.4.0/hypothesis_torch.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 hypothesis_torch/device.py
 hypothesis_torch/dtype.py
 hypothesis_torch/huggingface.py
 hypothesis_torch/inspection_util.py
 hypothesis_torch/layout.py
 hypothesis_torch/memory_format.py
 hypothesis_torch/module.py
+hypothesis_torch/register_random_torch_state.py
 hypothesis_torch/tensor.py
 hypothesis_torch/utils.py
 hypothesis_torch.egg-info/PKG-INFO
 hypothesis_torch.egg-info/SOURCES.txt
 hypothesis_torch.egg-info/dependency_links.txt
+hypothesis_torch.egg-info/entry_points.txt
 hypothesis_torch.egg-info/requires.txt
 hypothesis_torch.egg-info/top_level.txt
```

### Comparing `hypothesis_torch-0.3.1/pyproject.toml` & `hypothesis_torch-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Testing",
 ]
+[project.entry-points."hypothesis"]
+_ = "hypothesis_torch.register_random_torch_state:_register_random_torch_state"
 
 [project.optional-dependencies]
 huggingface = [
   "transformers",
 ]
 dev = [
   "ruff==0.4.1",
```

