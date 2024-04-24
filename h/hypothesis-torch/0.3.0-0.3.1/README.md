# Comparing `tmp/hypothesis_torch-0.3.0.tar.gz` & `tmp/hypothesis_torch-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypothesis_torch-0.3.0.tar", last modified: Wed Apr 24 03:17:47 2024, max compression
+gzip compressed data, was "hypothesis_torch-0.3.1.tar", last modified: Wed Apr 24 03:25:11 2024, max compression
```

## Comparing `hypothesis_torch-0.3.0.tar` & `hypothesis_torch-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 03:17:47.842120 hypothesis_torch-0.3.0/
--rw-r--r--   0 root         (0) root         (0)     1070 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8094 2024-04-24 03:17:47.842120 hypothesis_torch-0.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5282 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 03:17:47.842120 hypothesis_torch-0.3.0/hypothesis_torch/
--rw-r--r--   0 root         (0) root         (0)     1240 2024-04-24 03:17:44.000000 hypothesis_torch-0.3.0/hypothesis_torch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1408 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/hypothesis_torch/device.py
--rw-r--r--   0 root         (0) root         (0)     2491 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/hypothesis_torch/dtype.py
--rw-r--r--   0 root         (0) root         (0)     3922 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/hypothesis_torch/huggingface.py
--rw-r--r--   0 root         (0) root         (0)     1977 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/hypothesis_torch/inspection_util.py
--rw-r--r--   0 root         (0) root         (0)      735 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/hypothesis_torch/layout.py
--rw-r--r--   0 root         (0) root         (0)      846 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/hypothesis_torch/memory_format.py
--rw-r--r--   0 root         (0) root         (0)    10903 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/hypothesis_torch/module.py
--rw-r--r--   0 root         (0) root         (0)     7873 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/hypothesis_torch/tensor.py
--rw-r--r--   0 root         (0) root         (0)     1325 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/hypothesis_torch/test_memory_format.py
--rw-r--r--   0 root         (0) root         (0)     1422 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/hypothesis_torch/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 03:17:47.842120 hypothesis_torch-0.3.0/hypothesis_torch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8094 2024-04-24 03:17:47.000000 hypothesis_torch-0.3.0/hypothesis_torch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      561 2024-04-24 03:17:47.000000 hypothesis_torch-0.3.0/hypothesis_torch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 03:17:47.000000 hypothesis_torch-0.3.0/hypothesis_torch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       96 2024-04-24 03:17:47.000000 hypothesis_torch-0.3.0/hypothesis_torch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-24 03:17:47.000000 hypothesis_torch-0.3.0/hypothesis_torch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2099 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 03:17:47.842120 hypothesis_torch-0.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 03:25:11.333052 hypothesis_torch-0.3.1/
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8094 2024-04-24 03:25:11.333052 hypothesis_torch-0.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5282 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 03:25:11.333052 hypothesis_torch-0.3.1/hypothesis_torch/
+-rw-r--r--   0 root         (0) root         (0)     1240 2024-04-24 03:25:08.000000 hypothesis_torch-0.3.1/hypothesis_torch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/hypothesis_torch/device.py
+-rw-r--r--   0 root         (0) root         (0)     2491 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/hypothesis_torch/dtype.py
+-rw-r--r--   0 root         (0) root         (0)     3922 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/hypothesis_torch/huggingface.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/hypothesis_torch/inspection_util.py
+-rw-r--r--   0 root         (0) root         (0)      735 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/hypothesis_torch/layout.py
+-rw-r--r--   0 root         (0) root         (0)      846 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/hypothesis_torch/memory_format.py
+-rw-r--r--   0 root         (0) root         (0)    10903 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/hypothesis_torch/module.py
+-rw-r--r--   0 root         (0) root         (0)     7873 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/hypothesis_torch/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/hypothesis_torch/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 03:25:11.333052 hypothesis_torch-0.3.1/hypothesis_torch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8094 2024-04-24 03:25:11.000000 hypothesis_torch-0.3.1/hypothesis_torch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      522 2024-04-24 03:25:11.000000 hypothesis_torch-0.3.1/hypothesis_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 03:25:11.000000 hypothesis_torch-0.3.1/hypothesis_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2024-04-24 03:25:11.000000 hypothesis_torch-0.3.1/hypothesis_torch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-24 03:25:11.000000 hypothesis_torch-0.3.1/hypothesis_torch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2099 2024-04-24 03:24:28.000000 hypothesis_torch-0.3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 03:25:11.333052 hypothesis_torch-0.3.1/setup.cfg
```

### Comparing `hypothesis_torch-0.3.0/LICENSE` & `hypothesis_torch-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.3.0/PKG-INFO` & `hypothesis_torch-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.3.0
+Version: 0.3.1
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `hypothesis_torch-0.3.0/README.md` & `hypothesis_torch-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.3.0/hypothesis_torch/__init__.py` & `hypothesis_torch-0.3.1/hypothesis_torch/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Hypothesis strategies for various Pytorch structures (including tensors and modules).
 
 [Hypothesis](https://hypothesis.readthedocs.io/en/latest/) is a powerful property-based testing library for Python. It
 lacks built-in support for Pytorch tensors and modules, so this library provides strategies for generating them.
 """
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 import importlib.util
 
 from hypothesis_torch.device import (
     device_strategy,
     AVAILABLE_CPU_DEVICES,
     AVAILABLE_CUDA_DEVICES,
     AVAILABLE_MPS_DEVICES,
```

### Comparing `hypothesis_torch-0.3.0/hypothesis_torch/device.py` & `hypothesis_torch-0.3.1/hypothesis_torch/device.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.3.0/hypothesis_torch/dtype.py` & `hypothesis_torch-0.3.1/hypothesis_torch/dtype.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.3.0/hypothesis_torch/huggingface.py` & `hypothesis_torch-0.3.1/hypothesis_torch/huggingface.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.3.0/hypothesis_torch/inspection_util.py` & `hypothesis_torch-0.3.1/hypothesis_torch/inspection_util.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.3.0/hypothesis_torch/layout.py` & `hypothesis_torch-0.3.1/hypothesis_torch/layout.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.3.0/hypothesis_torch/memory_format.py` & `hypothesis_torch-0.3.1/hypothesis_torch/memory_format.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.3.0/hypothesis_torch/module.py` & `hypothesis_torch-0.3.1/hypothesis_torch/module.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.3.0/hypothesis_torch/tensor.py` & `hypothesis_torch-0.3.1/hypothesis_torch/tensor.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.3.0/hypothesis_torch/utils.py` & `hypothesis_torch-0.3.1/hypothesis_torch/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import TypeVar
 
 T = TypeVar("T")
 T_co = TypeVar("T_co", covariant=True)
 
 if sys.version_info < (3, 10):
 
-    def pairwise(iterable: Iterable[T]) -> Iterable[tuple[T, T]]:
+    def pairwise(iterable: Iterable[T]) -> Iterable[tuple[T, T]]:  # pragma: no cover
         """Iterate over pairs of consecutive elements in an iterable.
 
         Note:
             This is a backport of the `pairwise` function from Python 3.10 (for older versions of Python).
 
         Args:
             iterable: The iterable to iterate over.
```

### Comparing `hypothesis_torch-0.3.0/hypothesis_torch.egg-info/PKG-INFO` & `hypothesis_torch-0.3.1/hypothesis_torch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.3.0
+Version: 0.3.1
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `hypothesis_torch-0.3.0/hypothesis_torch.egg-info/SOURCES.txt` & `hypothesis_torch-0.3.1/hypothesis_torch.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,13 @@
 hypothesis_torch/dtype.py
 hypothesis_torch/huggingface.py
 hypothesis_torch/inspection_util.py
 hypothesis_torch/layout.py
 hypothesis_torch/memory_format.py
 hypothesis_torch/module.py
 hypothesis_torch/tensor.py
-hypothesis_torch/test_memory_format.py
 hypothesis_torch/utils.py
 hypothesis_torch.egg-info/PKG-INFO
 hypothesis_torch.egg-info/SOURCES.txt
 hypothesis_torch.egg-info/dependency_links.txt
 hypothesis_torch.egg-info/requires.txt
 hypothesis_torch.egg-info/top_level.txt
```

### Comparing `hypothesis_torch-0.3.0/pyproject.toml` & `hypothesis_torch-0.3.1/pyproject.toml`

 * *Files identical despite different names*

