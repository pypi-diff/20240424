# Comparing `tmp/hypothesis_torch-0.1.9.tar.gz` & `tmp/hypothesis_torch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypothesis_torch-0.1.9.tar", last modified: Mon Apr 22 17:23:53 2024, max compression
+gzip compressed data, was "hypothesis_torch-0.2.0.tar", last modified: Tue Apr 23 15:02:47 2024, max compression
```

## Comparing `hypothesis_torch-0.1.9.tar` & `hypothesis_torch-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 17:23:53.231512 hypothesis_torch-0.1.9/
--rw-r--r--   0 root         (0) root         (0)     1070 2024-04-22 17:23:17.000000 hypothesis_torch-0.1.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8097 2024-04-22 17:23:53.231512 hypothesis_torch-0.1.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5285 2024-04-22 17:23:17.000000 hypothesis_torch-0.1.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 17:23:53.227512 hypothesis_torch-0.1.9/hypothesis_torch/
--rw-r--r--   0 root         (0) root         (0)      523 2024-04-22 17:23:49.000000 hypothesis_torch-0.1.9/hypothesis_torch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1454 2024-04-22 17:23:17.000000 hypothesis_torch-0.1.9/hypothesis_torch/device.py
--rw-r--r--   0 root         (0) root         (0)     2262 2024-04-22 17:23:17.000000 hypothesis_torch-0.1.9/hypothesis_torch/dtype.py
--rw-r--r--   0 root         (0) root         (0)     3922 2024-04-22 17:23:17.000000 hypothesis_torch-0.1.9/hypothesis_torch/huggingface.py
--rw-r--r--   0 root         (0) root         (0)     1977 2024-04-22 17:23:17.000000 hypothesis_torch-0.1.9/hypothesis_torch/inspection_util.py
--rw-r--r--   0 root         (0) root         (0)     9278 2024-04-22 17:23:17.000000 hypothesis_torch-0.1.9/hypothesis_torch/module.py
--rw-r--r--   0 root         (0) root         (0)     3116 2024-04-22 17:23:17.000000 hypothesis_torch-0.1.9/hypothesis_torch/tensor.py
--rw-r--r--   0 root         (0) root         (0)     1422 2024-04-22 17:23:17.000000 hypothesis_torch-0.1.9/hypothesis_torch/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 17:23:53.231512 hypothesis_torch-0.1.9/hypothesis_torch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8097 2024-04-22 17:23:53.000000 hypothesis_torch-0.1.9/hypothesis_torch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      461 2024-04-22 17:23:53.000000 hypothesis_torch-0.1.9/hypothesis_torch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 17:23:53.000000 hypothesis_torch-0.1.9/hypothesis_torch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       96 2024-04-22 17:23:53.000000 hypothesis_torch-0.1.9/hypothesis_torch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-22 17:23:53.000000 hypothesis_torch-0.1.9/hypothesis_torch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2090 2024-04-22 17:23:17.000000 hypothesis_torch-0.1.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-22 17:23:53.231512 hypothesis_torch-0.1.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 15:02:47.264539 hypothesis_torch-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-04-23 15:01:42.000000 hypothesis_torch-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8094 2024-04-23 15:02:47.260539 hypothesis_torch-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5282 2024-04-23 15:01:42.000000 hypothesis_torch-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 15:02:47.260539 hypothesis_torch-0.2.0/hypothesis_torch/
+-rw-r--r--   0 root         (0) root         (0)     1122 2024-04-23 15:02:43.000000 hypothesis_torch-0.2.0/hypothesis_torch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2024-04-23 15:01:42.000000 hypothesis_torch-0.2.0/hypothesis_torch/device.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2024-04-23 15:01:42.000000 hypothesis_torch-0.2.0/hypothesis_torch/dtype.py
+-rw-r--r--   0 root         (0) root         (0)     3922 2024-04-23 15:01:42.000000 hypothesis_torch-0.2.0/hypothesis_torch/huggingface.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2024-04-23 15:01:42.000000 hypothesis_torch-0.2.0/hypothesis_torch/inspection_util.py
+-rw-r--r--   0 root         (0) root         (0)    10903 2024-04-23 15:01:42.000000 hypothesis_torch-0.2.0/hypothesis_torch/module.py
+-rw-r--r--   0 root         (0) root         (0)     3449 2024-04-23 15:01:42.000000 hypothesis_torch-0.2.0/hypothesis_torch/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2024-04-23 15:01:42.000000 hypothesis_torch-0.2.0/hypothesis_torch/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 15:02:47.260539 hypothesis_torch-0.2.0/hypothesis_torch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8094 2024-04-23 15:02:47.000000 hypothesis_torch-0.2.0/hypothesis_torch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      461 2024-04-23 15:02:47.000000 hypothesis_torch-0.2.0/hypothesis_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 15:02:47.000000 hypothesis_torch-0.2.0/hypothesis_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2024-04-23 15:02:47.000000 hypothesis_torch-0.2.0/hypothesis_torch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-23 15:02:47.000000 hypothesis_torch-0.2.0/hypothesis_torch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2099 2024-04-23 15:01:42.000000 hypothesis_torch-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 15:02:47.264539 hypothesis_torch-0.2.0/setup.cfg
```

### Comparing `hypothesis_torch-0.1.9/LICENSE` & `hypothesis_torch-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.1.9/PKG-INFO` & `hypothesis_torch-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.1.9
+Version: 0.2.0
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -190,8 +190,8 @@
 import transformers
 from hypothesis import strategies as st
 hypothesis_torch.transformer_strategy(transformers.LlamaForCausalLM, hidden_size=st.integers(64, 128), vocab_size=1000)
 ```
 
 [! Note]
     Currently, the `transformer_strategy` only accepts `kwargs` that can be passed to the constructor of the model's 
-    config class. Thus, it cannot currently replicate all of the behavior of calling `from_pretrained` on a model class.
+    config class. Thus, it cannot currently replicate all the behavior of calling `from_pretrained` on a model class.
```

### Comparing `hypothesis_torch-0.1.9/README.md` & `hypothesis_torch-0.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -134,8 +134,8 @@
 import transformers
 from hypothesis import strategies as st
 hypothesis_torch.transformer_strategy(transformers.LlamaForCausalLM, hidden_size=st.integers(64, 128), vocab_size=1000)
 ```
 
 [! Note]
     Currently, the `transformer_strategy` only accepts `kwargs` that can be passed to the constructor of the model's 
-    config class. Thus, it cannot currently replicate all of the behavior of calling `from_pretrained` on a model class.
+    config class. Thus, it cannot currently replicate all the behavior of calling `from_pretrained` on a model class.
```

### Comparing `hypothesis_torch-0.1.9/hypothesis_torch/device.py` & `hypothesis_torch-0.2.0/hypothesis_torch/device.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,35 +11,33 @@
 AVAILABLE_CUDA_DEVICES = [torch.device("cuda", i) for i in range(torch.cuda.device_count())]
 AVAILABLE_MPS_DEVICES = [torch.device("mps")] if torch.backends.mps.is_available() else []
 AVAILABLE_META_DEVICES = [torch.device("meta")]
 
 AVAILABLE_PHYSICAL_DEVICES = AVAILABLE_CPU_DEVICES + AVAILABLE_CUDA_DEVICES + AVAILABLE_MPS_DEVICES
 
 
-@st.composite
 def device_strategy(
-    draw: st.DrawFn,
     *,
     devices: Sequence[torch.device] | None = None,
     allow_meta_device: bool = False,
-) -> torch.device:
+) -> st.SearchStrategy[torch.device]:
     """Strategy for generating torch devices.
 
     Args:
-        draw: The draw function provided by `hypothesis`.
         devices: A sequence of devices to sample from. If None, all available devices are sampled.
         allow_meta_device: Whether to allow the meta device.
 
     Returns:
         A strategy for generating torch devices.
 
     """
     if devices is None:
         devices = AVAILABLE_PHYSICAL_DEVICES
     if allow_meta_device:
         devices = list(devices) + AVAILABLE_META_DEVICES
     assert devices is not None
-    return draw(st.sampled_from(devices))
+    return st.sampled_from(devices)
 
 
 st.register_type_strategy(torch.device, device_strategy())
-st.register_type_strategy(torch.cuda.device, device_strategy(devices=AVAILABLE_CUDA_DEVICES))
+if torch.cuda.is_available():
+    st.register_type_strategy(torch.cuda.device, device_strategy(devices=AVAILABLE_CUDA_DEVICES))
```

### Comparing `hypothesis_torch-0.1.9/hypothesis_torch/dtype.py` & `hypothesis_torch-0.2.0/hypothesis_torch/dtype.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,39 +30,36 @@
 
 numpy_dtype_map: dict[torch.dtype, npt.DTypeLike] = {
     torch.int8: np.int8,
     torch.int16: np.int16,
     torch.int32: np.int32,
     torch.int64: np.int64,
     torch.uint8: np.uint8,
-    torch.float16: np.float16,
-    torch.float32: np.float32,
-    torch.float64: np.float64,
-    torch.bfloat16: np.float32,  # bfloat16 is not supported by numpy
-    torch.complex64: np.complex64,
-    torch.complex128: np.complex128,
+    torch.float16: float,
+    torch.float32: float,
+    torch.float64: float,
+    torch.bfloat16: float,
+    torch.complex64: complex,
+    torch.complex128: complex,
     torch.bool: np.bool_,
 }
 """A mapping from torch dtypes to numpy dtypes. Useful for generating tensors of arbitrary dtypes from the builtin
 numpy strategies."""
 
 assert set(numpy_dtype_map.keys()) == set(ALL_DTYPES)
 
 
-@st.composite
-def dtype_strategy(draw: st.DrawFn, *, dtypes: Sequence[torch.dtype] | None = None) -> torch.dtype:
+def dtype_strategy(*, dtypes: Sequence[torch.dtype] | None = None) -> st.SearchStrategy[torch.dtype]:
     """Strategy for generating torch dtypes.
 
     Args:
-        draw: The draw function provided by `hypothesis`. If `None`, all dtypes are sampled.
-        dtypes: A strategy for generating elements of the dtype.
+        dtypes: A strategy for generating elements of the dtype. If `None`, all dtypes are sampled.
 
     Returns:
         A strategy for generating torch dtypes.
-
     """
     if dtypes is None:
         dtypes = ALL_DTYPES
-    return draw(st.sampled_from(dtypes))
+    return st.sampled_from(dtypes)
 
 
 st.register_type_strategy(torch.dtype, dtype_strategy())
```

### Comparing `hypothesis_torch-0.1.9/hypothesis_torch/huggingface.py` & `hypothesis_torch-0.2.0/hypothesis_torch/huggingface.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.1.9/hypothesis_torch/inspection_util.py` & `hypothesis_torch-0.2.0/hypothesis_torch/inspection_util.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.1.9/hypothesis_torch/module.py` & `hypothesis_torch-0.2.0/hypothesis_torch/module.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 """Strategies for generating PyTorch Modules."""
 
 from __future__ import annotations
 
-from typing import TypeVar
+from typing import TypeVar, Sequence, Mapping
 
 import torch
 from hypothesis import strategies as st
 from torch import nn
 
 from hypothesis_torch import utils
 
-__all__ = [
-    "same_shape_activation_strategy",
-    "linear_network_strategy",
-]
-
 T = TypeVar("T")
 
 SENSIBLE_FLOATS = st.floats(
     min_value=-10,
     max_value=10,
     allow_nan=False,
     allow_infinity=False,
@@ -48,14 +43,22 @@
     lower = draw(SENSIBLE_FLOATS)
     upper = draw(SENSIBLE_FLOATS.filter(lambda x: x > lower))
     return lower, upper
 
 
 @st.composite
 def rrelu_strategy(draw: st.DrawFn) -> nn.RReLU:
+    """Strategy for generating instances of `nn.RReLU` by drawing values for its constructor.
+
+    Args:
+        draw: The draw function provided by `hypothesis`.
+
+    Returns:
+        An instance of `nn.RReLU`.
+    """
     lower, upper = draw(lower_upper_strategy())
     inplace = draw(st.booleans())
     return nn.RReLU(lower, upper, inplace)
 
 
 @st.composite
 def signature_to_strategy(draw: st.DrawFn, constructor: type[T], *args, **kwargs) -> T:
@@ -78,72 +81,93 @@
 
 
 @st.composite
 def hard_tanh_strategy(draw: st.DrawFn) -> nn.Hardtanh:
     """Strategy for generating instances of `nn.Hardtanh` by drawing values for its constructor.
 
     Args:
-    ----
         draw: The draw function provided by `hypothesis`.
 
     Returns:
-    -------
         An instance of `nn.Hardtanh`.
 
     """
     min_value = draw(SENSIBLE_FLOATS)
     max_value = draw(SENSIBLE_FLOATS.filter(lambda x: x > min_value))
     inplace = draw(st.booleans())
     return nn.Hardtanh(min_value, max_value, inplace)
 
 
-def same_shape_activation_strategy() -> st.SearchStrategy[nn.Module]:
+activation_strategies: dict[type[nn.Module], st.SearchStrategy[nn.Module]] = {
+    nn.Identity: signature_to_strategy(nn.Identity),
+    nn.ELU: signature_to_strategy(nn.ELU, alpha=SENSIBLE_FLOATS, inplace=st.booleans()),
+    nn.Hardshrink: signature_to_strategy(nn.Hardshrink, lambd=SENSIBLE_FLOATS),
+    nn.Hardsigmoid: signature_to_strategy(nn.Hardsigmoid, inplace=st.booleans()),
+    nn.Hardtanh: hard_tanh_strategy(),
+    nn.Hardswish: signature_to_strategy(nn.Hardswish, inplace=st.booleans()),
+    nn.LeakyReLU: signature_to_strategy(nn.LeakyReLU, negative_slope=SENSIBLE_FLOATS, inplace=st.booleans()),
+    nn.LogSigmoid: signature_to_strategy(nn.LogSigmoid),
+    # TODO: nn.MultiheadAttention, although in the `Non-linear activations` section, does not have the same shape
+    #  inside and outside
+    # TODO: nn.PReLU(num_parameters=1, init=0.25, device=None, dtype=None)
+    # TODO: PReLU might depend on the input shape
+    # TODO: num_parameters (int) – number of a to learn. Although it takes an int as input, there is only two
+    #  values are legitimate: 1, or the number of channels at input. Default: 1
+    nn.PReLU: signature_to_strategy(nn.PReLU, num_parameters=st.just(1), init=SENSIBLE_FLOATS),
+    nn.ReLU: signature_to_strategy(nn.ReLU, inplace=st.booleans()),
+    nn.ReLU6: signature_to_strategy(nn.ReLU6, inplace=st.booleans()),
+    nn.RReLU: rrelu_strategy(),
+    nn.SELU: signature_to_strategy(nn.SELU, inplace=st.booleans()),
+    nn.CELU: signature_to_strategy(
+        nn.CELU, alpha=SENSIBLE_FLOATS.filter(lambda x: abs(x) > 1e-5), inplace=st.booleans()
+    ),
+    nn.GELU: signature_to_strategy(nn.GELU, approximate=st.sampled_from(["none", "tanh"])),
+    nn.Sigmoid: signature_to_strategy(nn.Sigmoid),
+    nn.SiLU: signature_to_strategy(nn.SiLU, inplace=st.booleans()),
+    nn.Mish: signature_to_strategy(nn.Mish, inplace=st.booleans()),
+    nn.Softplus: signature_to_strategy(nn.Softplus, beta=SENSIBLE_FLOATS, threshold=SENSIBLE_POSITIVE_FLOATS),
+    nn.Softshrink: signature_to_strategy(nn.Softshrink, lambd=SENSIBLE_POSITIVE_FLOATS),
+    nn.Softsign: signature_to_strategy(nn.Softsign),
+    nn.Tanh: signature_to_strategy(nn.Tanh),
+    nn.Tanhshrink: signature_to_strategy(nn.Tanhshrink),
+    nn.Threshold: signature_to_strategy(
+        nn.Threshold, threshold=SENSIBLE_FLOATS, value=SENSIBLE_FLOATS, inplace=st.booleans()
+    ),
+    # TODO: nn.GLU depends on the input shape
+}
+
+
+def same_shape_activation_strategy(
+    allowed_activation_functions: Sequence[type[nn.Module]] | Sequence[st.SearchStrategy[nn.Module]] | None = None,
+) -> st.SearchStrategy[nn.Module]:
     """Strategy for generating activation functions that have the same shape input and output shape.
 
+    Args:
+        allowed_activation_functions: Activation functions to sample from.
+            - If a sequence of strategies is provided, only these strategies are sampled from.
+            - If a sequence of module types is provided, the elements are the activation functions to sample from.
+            - If `None`, all supported activation functions are sampled.
+            - For `None` or sequence of module type inputs, see complete list of supported activation functions in
+            `activation_strategies`.
+
     Returns:
         A strategy for generating activation functions that have the same shape input and output shape.
     """
-    return st.one_of(
-        signature_to_strategy(nn.Identity),
-        signature_to_strategy(nn.ELU, alpha=SENSIBLE_FLOATS, inplace=st.booleans()),
-        signature_to_strategy(nn.Hardshrink, lambd=SENSIBLE_FLOATS),
-        signature_to_strategy(nn.Hardsigmoid, inplace=st.booleans()),
-        hard_tanh_strategy(),
-        signature_to_strategy(nn.Hardswish, inplace=st.booleans()),
-        signature_to_strategy(nn.LeakyReLU, negative_slope=SENSIBLE_FLOATS, inplace=st.booleans()),
-        signature_to_strategy(nn.LogSigmoid),
-        # TODO: nn.MultiheadAttention, although in the `Non-linear activations` section, does not have the same shape
-        #  inside and outside
-        # TODO: nn.PReLU(num_parameters=1, init=0.25, device=None, dtype=None)
-        # TODO: PReLU might depend on the input shape
-        # TODO: num_parameters (int) – number of a to learn. Although it takes an int as input, there is only two
-        #  values are legitimate: 1, or the number of channels at input. Default: 1
-        signature_to_strategy(nn.PReLU, num_parameters=st.just(1), init=SENSIBLE_FLOATS),
-        signature_to_strategy(nn.ReLU, inplace=st.booleans()),
-        signature_to_strategy(nn.ReLU6, inplace=st.booleans()),
-        rrelu_strategy(),
-        signature_to_strategy(nn.SELU, inplace=st.booleans()),
-        signature_to_strategy(nn.CELU, alpha=SENSIBLE_FLOATS.filter(lambda x: abs(x) > 1e-5), inplace=st.booleans()),
-        signature_to_strategy(nn.GELU, approximate=st.sampled_from(["none", "tanh"])),
-        signature_to_strategy(nn.Sigmoid),
-        signature_to_strategy(nn.SiLU, inplace=st.booleans()),
-        signature_to_strategy(nn.Mish, inplace=st.booleans()),
-        signature_to_strategy(nn.Softplus, beta=SENSIBLE_FLOATS, threshold=SENSIBLE_POSITIVE_FLOATS),
-        signature_to_strategy(nn.Softshrink, lambd=SENSIBLE_POSITIVE_FLOATS),
-        signature_to_strategy(nn.Softsign),
-        signature_to_strategy(nn.Tanh),
-        signature_to_strategy(nn.Tanhshrink),
-        signature_to_strategy(
-            nn.Threshold,
-            threshold=SENSIBLE_FLOATS,
-            value=SENSIBLE_FLOATS,
-            inplace=st.booleans(),
-        ),
-        # TODO: nn.GLU depends on the input shape
-    )
+    if allowed_activation_functions is None:
+        allowed_activation_functions = list(activation_strategies.keys())
+    assert allowed_activation_functions is not None
+    strategies: list[st.SearchStrategy[nn.Module]] = []
+    for activation_function in allowed_activation_functions:
+        if isinstance(activation_function, st.SearchStrategy):
+            strategies.append(activation_function)
+        elif activation_function in activation_strategies:
+            strategies.append(activation_strategies[activation_function])
+        else:
+            raise ValueError(f"Unsupported activation function: {activation_function}")
+    return st.one_of(strategies)
 
 
 @st.composite
 def linear_network_strategy(
     draw: st.DrawFn,
     input_shape: tuple[int, ...] | torch.Size | st.SearchStrategy[tuple[int, ...]] | st.SearchStrategy[torch.Size],
     output_shape: tuple[int, ...] | torch.Size | st.SearchStrategy[tuple[int, ...]] | st.SearchStrategy[torch.Size],
```

### Comparing `hypothesis_torch-0.1.9/hypothesis_torch/tensor.py` & `hypothesis_torch-0.2.0/hypothesis_torch/tensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,16 +49,21 @@
         dtype = draw(dtype)
     numpy_dtype = dtype_module.numpy_dtype_map[dtype]
 
     # We will pre-sample the device so that we can cast it to a concrete torch device
     if isinstance(device, st.SearchStrategy):
         device = draw(device)
 
+    # INCOMPATIBILITY HANDLING
     # MPS devices do not support tensors with dtype torch.float64 and bfloat16
     hypothesis.assume(not (device is not None and device.type == "mps" and dtype in (torch.float64, torch.bfloat16)))
+    # If the dtype is an integer, we need to make sure that the elements are integers within the dtype's range
+    if dtype in dtype_module.INT_DTYPES and isinstance(elements, st.SearchStrategy):
+        info = torch.iinfo(dtype)
+        elements = elements.filter(lambda x: info.min <= x <= info.max)
 
     if isinstance(unique, st.SearchStrategy):
         unique = draw(unique)
 
     ndarray_strategy = numpy_st.arrays(numpy_dtype, shape, elements=elements, fill=fill, unique=unique)
     tensor = draw(ndarray_strategy.map(torch.from_numpy))
```

### Comparing `hypothesis_torch-0.1.9/hypothesis_torch/utils.py` & `hypothesis_torch-0.2.0/hypothesis_torch/utils.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.1.9/hypothesis_torch.egg-info/PKG-INFO` & `hypothesis_torch-0.2.0/hypothesis_torch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.1.9
+Version: 0.2.0
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -190,8 +190,8 @@
 import transformers
 from hypothesis import strategies as st
 hypothesis_torch.transformer_strategy(transformers.LlamaForCausalLM, hidden_size=st.integers(64, 128), vocab_size=1000)
 ```
 
 [! Note]
     Currently, the `transformer_strategy` only accepts `kwargs` that can be passed to the constructor of the model's 
-    config class. Thus, it cannot currently replicate all of the behavior of calling `from_pretrained` on a model class.
+    config class. Thus, it cannot currently replicate all the behavior of calling `from_pretrained` on a model class.
```

### Comparing `hypothesis_torch-0.1.9/pyproject.toml` & `hypothesis_torch-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -64,11 +64,11 @@
 build_command = "python -m pip install build && python -m build"
 
 [tool.setuptools.dynamic]
 version = {attr = "hypothesis_torch.__version__"}
 
 [tool.ruff.lint]
 select = ["D", "E", "F", "RUF100"]
-ignore = ["F401", "PT009", "S101"]
+ignore = ["D205", "F401", "PT009", "S101"]
 
 [tool.ruff.lint.pydocstyle]
-convention = "google"
+convention = "google"
```

