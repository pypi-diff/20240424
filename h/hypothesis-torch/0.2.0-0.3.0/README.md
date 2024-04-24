# Comparing `tmp/hypothesis_torch-0.2.0.tar.gz` & `tmp/hypothesis_torch-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypothesis_torch-0.2.0.tar", last modified: Tue Apr 23 15:02:47 2024, max compression
+gzip compressed data, was "hypothesis_torch-0.3.0.tar", last modified: Wed Apr 24 03:17:47 2024, max compression
```

## Comparing `hypothesis_torch-0.2.0.tar` & `hypothesis_torch-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 15:02:47.264539 hypothesis_torch-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     1070 2024-04-23 15:01:42.000000 hypothesis_torch-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8094 2024-04-23 15:02:47.260539 hypothesis_torch-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5282 2024-04-23 15:01:42.000000 hypothesis_torch-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 15:02:47.260539 hypothesis_torch-0.2.0/hypothesis_torch/
--rw-r--r--   0 root         (0) root         (0)     1122 2024-04-23 15:02:43.000000 hypothesis_torch-0.2.0/hypothesis_torch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1408 2024-04-23 15:01:42.000000 hypothesis_torch-0.2.0/hypothesis_torch/device.py
--rw-r--r--   0 root         (0) root         (0)     2116 2024-04-23 15:01:42.000000 hypothesis_torch-0.2.0/hypothesis_torch/dtype.py
--rw-r--r--   0 root         (0) root         (0)     3922 2024-04-23 15:01:42.000000 hypothesis_torch-0.2.0/hypothesis_torch/huggingface.py
--rw-r--r--   0 root         (0) root         (0)     1977 2024-04-23 15:01:42.000000 hypothesis_torch-0.2.0/hypothesis_torch/inspection_util.py
--rw-r--r--   0 root         (0) root         (0)    10903 2024-04-23 15:01:42.000000 hypothesis_torch-0.2.0/hypothesis_torch/module.py
--rw-r--r--   0 root         (0) root         (0)     3449 2024-04-23 15:01:42.000000 hypothesis_torch-0.2.0/hypothesis_torch/tensor.py
--rw-r--r--   0 root         (0) root         (0)     1422 2024-04-23 15:01:42.000000 hypothesis_torch-0.2.0/hypothesis_torch/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 15:02:47.260539 hypothesis_torch-0.2.0/hypothesis_torch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8094 2024-04-23 15:02:47.000000 hypothesis_torch-0.2.0/hypothesis_torch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      461 2024-04-23 15:02:47.000000 hypothesis_torch-0.2.0/hypothesis_torch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 15:02:47.000000 hypothesis_torch-0.2.0/hypothesis_torch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       96 2024-04-23 15:02:47.000000 hypothesis_torch-0.2.0/hypothesis_torch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-23 15:02:47.000000 hypothesis_torch-0.2.0/hypothesis_torch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2099 2024-04-23 15:01:42.000000 hypothesis_torch-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 15:02:47.264539 hypothesis_torch-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 03:17:47.842120 hypothesis_torch-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8094 2024-04-24 03:17:47.842120 hypothesis_torch-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5282 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 03:17:47.842120 hypothesis_torch-0.3.0/hypothesis_torch/
+-rw-r--r--   0 root         (0) root         (0)     1240 2024-04-24 03:17:44.000000 hypothesis_torch-0.3.0/hypothesis_torch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/hypothesis_torch/device.py
+-rw-r--r--   0 root         (0) root         (0)     2491 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/hypothesis_torch/dtype.py
+-rw-r--r--   0 root         (0) root         (0)     3922 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/hypothesis_torch/huggingface.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/hypothesis_torch/inspection_util.py
+-rw-r--r--   0 root         (0) root         (0)      735 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/hypothesis_torch/layout.py
+-rw-r--r--   0 root         (0) root         (0)      846 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/hypothesis_torch/memory_format.py
+-rw-r--r--   0 root         (0) root         (0)    10903 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/hypothesis_torch/module.py
+-rw-r--r--   0 root         (0) root         (0)     7873 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/hypothesis_torch/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     1325 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/hypothesis_torch/test_memory_format.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/hypothesis_torch/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 03:17:47.842120 hypothesis_torch-0.3.0/hypothesis_torch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8094 2024-04-24 03:17:47.000000 hypothesis_torch-0.3.0/hypothesis_torch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      561 2024-04-24 03:17:47.000000 hypothesis_torch-0.3.0/hypothesis_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 03:17:47.000000 hypothesis_torch-0.3.0/hypothesis_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2024-04-24 03:17:47.000000 hypothesis_torch-0.3.0/hypothesis_torch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-24 03:17:47.000000 hypothesis_torch-0.3.0/hypothesis_torch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2099 2024-04-24 03:17:13.000000 hypothesis_torch-0.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 03:17:47.842120 hypothesis_torch-0.3.0/setup.cfg
```

### Comparing `hypothesis_torch-0.2.0/LICENSE` & `hypothesis_torch-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.2.0/PKG-INFO` & `hypothesis_torch-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.2.0
+Version: 0.3.0
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `hypothesis_torch-0.2.0/README.md` & `hypothesis_torch-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.2.0/hypothesis_torch/__init__.py` & `hypothesis_torch-0.3.0/hypothesis_torch/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Hypothesis strategies for various Pytorch structures (including tensors and modules).
 
 [Hypothesis](https://hypothesis.readthedocs.io/en/latest/) is a powerful property-based testing library for Python. It
 lacks built-in support for Pytorch tensors and modules, so this library provides strategies for generating them.
 """
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 import importlib.util
 
 from hypothesis_torch.device import (
     device_strategy,
     AVAILABLE_CPU_DEVICES,
     AVAILABLE_CUDA_DEVICES,
     AVAILABLE_MPS_DEVICES,
@@ -22,13 +22,15 @@
     SIGNED_INT_DTYPES,
     UNSIGNED_INT_DTYPES,
     BFLOAT_DTYPES,
     COMPLEX_DTYPES,
     BOOL_DTYPES,
     ALL_DTYPES,
 )
+from hypothesis_torch.layout import layout_strategy
+from hypothesis_torch.memory_format import memory_format_strategy
 from hypothesis_torch.module import linear_network_strategy, same_shape_activation_strategy
 from hypothesis_torch.tensor import tensor_strategy
 
 if importlib.util.find_spec("transformers") is not None:
     # Import Hugging Face strategies if transformers is installed
     from hypothesis_torch.huggingface import transformer_strategy
```

### Comparing `hypothesis_torch-0.2.0/hypothesis_torch/device.py` & `hypothesis_torch-0.3.0/hypothesis_torch/device.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.2.0/hypothesis_torch/dtype.py` & `hypothesis_torch-0.3.0/hypothesis_torch/dtype.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,53 @@
 """Strategies for generating PyTorch dtypes."""
 
 from __future__ import annotations
 
 from collections.abc import Sequence
+from typing import Mapping
+
+from typing_extensions import Final
 
 import numpy as np
 import numpy.typing as npt
 import torch
 from hypothesis import strategies as st
 
-SIGNED_INT_DTYPES = [torch.int8, torch.int16, torch.int32, torch.int64]
+SIGNED_INT_DTYPES: Final[tuple[torch.dtype, ...]] = (
+    torch.int8,
+    torch.int16,
+    torch.int32,
+    torch.int64,
+)
 """All signed integer dtypes supported by PyTorch."""
-UNSIGNED_INT_DTYPES = [torch.uint8]
+UNSIGNED_INT_DTYPES: Final[tuple[torch.dtype, ...]] = (torch.uint8,)
 """All unsigned integer dtypes supported by PyTorch."""
-INT_DTYPES = SIGNED_INT_DTYPES + UNSIGNED_INT_DTYPES
+INT_DTYPES: Final[tuple[torch.dtype, ...]] = SIGNED_INT_DTYPES + UNSIGNED_INT_DTYPES
 """All integer (both signed and unsigned) dtypes supported by PyTorch."""
 
-FLOAT_DTYPES = [torch.float16, torch.float32, torch.float64]
+FLOAT_DTYPES: Final[tuple[torch.dtype, ...]] = (
+    torch.float16,
+    torch.float32,
+    torch.float64,
+)
 """All floating point dtypes supported by PyTorch."""
-BFLOAT_DTYPES = [torch.bfloat16]
+BFLOAT_DTYPES: Final[tuple[torch.dtype, ...]] = (torch.bfloat16,)
 """All brain-float dtypes supported by PyTorch."""
-COMPLEX_DTYPES = [torch.complex64, torch.complex128]
+COMPLEX_DTYPES: Final[tuple[torch.dtype, ...]] = (
+    torch.complex64,
+    torch.complex128,
+)
 """All complex dtypes supported by PyTorch."""
-BOOL_DTYPES = [torch.bool]
+BOOL_DTYPES: Final[tuple[torch.dtype, ...]] = (torch.bool,)
 """All boolean dtypes supported by PyTorch."""
 
-ALL_DTYPES = INT_DTYPES + FLOAT_DTYPES + BFLOAT_DTYPES + COMPLEX_DTYPES + BOOL_DTYPES
+ALL_DTYPES: Final[tuple[torch.dtype, ...]] = INT_DTYPES + FLOAT_DTYPES + BFLOAT_DTYPES + COMPLEX_DTYPES + BOOL_DTYPES
 """All dtypes supported by PyTorch."""
 
-numpy_dtype_map: dict[torch.dtype, npt.DTypeLike] = {
+numpy_dtype_map: Final[Mapping[torch.dtype, npt.DTypeLike]] = {
     torch.int8: np.int8,
     torch.int16: np.int16,
     torch.int32: np.int32,
     torch.int64: np.int64,
     torch.uint8: np.uint8,
     torch.float16: float,
     torch.float32: float,
@@ -44,15 +59,15 @@
 }
 """A mapping from torch dtypes to numpy dtypes. Useful for generating tensors of arbitrary dtypes from the builtin
 numpy strategies."""
 
 assert set(numpy_dtype_map.keys()) == set(ALL_DTYPES)
 
 
-def dtype_strategy(*, dtypes: Sequence[torch.dtype] | None = None) -> st.SearchStrategy[torch.dtype]:
+def dtype_strategy(dtypes: Sequence[torch.dtype] | None = None) -> st.SearchStrategy[torch.dtype]:
     """Strategy for generating torch dtypes.
 
     Args:
         dtypes: A strategy for generating elements of the dtype. If `None`, all dtypes are sampled.
 
     Returns:
         A strategy for generating torch dtypes.
```

### Comparing `hypothesis_torch-0.2.0/hypothesis_torch/huggingface.py` & `hypothesis_torch-0.3.0/hypothesis_torch/huggingface.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.2.0/hypothesis_torch/inspection_util.py` & `hypothesis_torch-0.3.0/hypothesis_torch/inspection_util.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.2.0/hypothesis_torch/module.py` & `hypothesis_torch-0.3.0/hypothesis_torch/module.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.2.0/hypothesis_torch/utils.py` & `hypothesis_torch-0.3.0/hypothesis_torch/utils.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.2.0/hypothesis_torch.egg-info/PKG-INFO` & `hypothesis_torch-0.3.0/hypothesis_torch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.2.0
+Version: 0.3.0
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `hypothesis_torch-0.2.0/pyproject.toml` & `hypothesis_torch-0.3.0/pyproject.toml`

 * *Files identical despite different names*

