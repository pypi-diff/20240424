# Comparing `tmp/waylay_ml_adapter_torch-0.0.2.tar.gz` & `tmp/waylay_ml_adapter_torch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_ml_adapter_torch-0.0.2.tar", last modified: Wed Apr 17 09:14:58 2024, max compression
+gzip compressed data, was "waylay_ml_adapter_torch-0.0.3.tar", last modified: Wed Apr 24 15:26:47 2024, max compression
```

## Comparing `waylay_ml_adapter_torch-0.0.2.tar` & `waylay_ml_adapter_torch-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:58.221763 waylay_ml_adapter_torch-0.0.2/
--rw-r--r--   0 thomas     (502) staff       (20)      634 2024-04-17 09:14:58.221357 waylay_ml_adapter_torch-0.0.2/PKG-INFO
--rw-r--r--   0 thomas     (502) staff       (20)       56 2024-04-17 08:27:35.000000 waylay_ml_adapter_torch-0.0.2/README.md
--rw-r--r--   0 thomas     (502) staff       (20)     1126 2024-04-17 08:27:35.000000 waylay_ml_adapter_torch-0.0.2/pyproject.toml
--rw-r--r--   0 thomas     (502) staff       (20)       38 2024-04-17 09:14:58.221812 waylay_ml_adapter_torch-0.0.2/setup.cfg
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:58.215385 waylay_ml_adapter_torch-0.0.2/src/
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:58.215201 waylay_ml_adapter_torch-0.0.2/src/ml_adapter/
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:58.217922 waylay_ml_adapter_torch-0.0.2/src/ml_adapter/torch/
--rw-r--r--   0 thomas     (502) staff       (20)      156 2024-04-17 08:27:35.000000 waylay_ml_adapter_torch-0.0.2/src/ml_adapter/torch/__init__.py
--rw-r--r--   0 thomas     (502) staff       (20)     3668 2024-04-17 08:27:35.000000 waylay_ml_adapter_torch-0.0.2/src/ml_adapter/torch/adapter.py
--rw-r--r--   0 thomas     (502) staff       (20)     1511 2024-04-17 08:27:35.000000 waylay_ml_adapter_torch-0.0.2/src/ml_adapter/torch/marshall.py
--rw-r--r--   0 thomas     (502) staff       (20)        0 2024-04-17 08:27:35.000000 waylay_ml_adapter_torch-0.0.2/src/ml_adapter/torch/py.typed
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:58.220815 waylay_ml_adapter_torch-0.0.2/src/waylay_ml_adapter_torch.egg-info/
--rw-r--r--   0 thomas     (502) staff       (20)      634 2024-04-17 09:14:58.000000 waylay_ml_adapter_torch-0.0.2/src/waylay_ml_adapter_torch.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (502) staff       (20)      406 2024-04-17 09:14:58.000000 waylay_ml_adapter_torch-0.0.2/src/waylay_ml_adapter_torch.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (502) staff       (20)        1 2024-04-17 09:14:58.000000 waylay_ml_adapter_torch-0.0.2/src/waylay_ml_adapter_torch.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (502) staff       (20)      198 2024-04-17 09:14:58.000000 waylay_ml_adapter_torch-0.0.2/src/waylay_ml_adapter_torch.egg-info/requires.txt
--rw-r--r--   0 thomas     (502) staff       (20)       11 2024-04-17 09:14:58.000000 waylay_ml_adapter_torch-0.0.2/src/waylay_ml_adapter_torch.egg-info/top_level.txt
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:26:47.595452 waylay_ml_adapter_torch-0.0.3/
+-rw-r--r--   0 thomas     (502) staff       (20)      746 2024-04-24 15:21:52.000000 waylay_ml_adapter_torch-0.0.3/LICENCE.txt
+-rw-r--r--   0 thomas     (502) staff       (20)     4784 2024-04-24 15:26:47.595166 waylay_ml_adapter_torch-0.0.3/PKG-INFO
+-rw-r--r--   0 thomas     (502) staff       (20)     4059 2024-04-24 15:21:52.000000 waylay_ml_adapter_torch-0.0.3/README.md
+-rw-r--r--   0 thomas     (502) staff       (20)     1206 2024-04-24 15:21:52.000000 waylay_ml_adapter_torch-0.0.3/pyproject.toml
+-rw-r--r--   0 thomas     (502) staff       (20)       38 2024-04-24 15:26:47.595508 waylay_ml_adapter_torch-0.0.3/setup.cfg
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:26:47.589327 waylay_ml_adapter_torch-0.0.3/src/
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:26:47.589151 waylay_ml_adapter_torch-0.0.3/src/ml_adapter/
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:26:47.591400 waylay_ml_adapter_torch-0.0.3/src/ml_adapter/torch/
+-rw-r--r--   0 thomas     (502) staff       (20)      156 2024-04-24 10:44:07.000000 waylay_ml_adapter_torch-0.0.3/src/ml_adapter/torch/__init__.py
+-rw-r--r--   0 thomas     (502) staff       (20)     3588 2024-04-24 15:21:52.000000 waylay_ml_adapter_torch-0.0.3/src/ml_adapter/torch/adapter.py
+-rw-r--r--   0 thomas     (502) staff       (20)     1479 2024-04-24 15:21:52.000000 waylay_ml_adapter_torch-0.0.3/src/ml_adapter/torch/marshall.py
+-rw-r--r--   0 thomas     (502) staff       (20)        0 2024-04-17 08:27:35.000000 waylay_ml_adapter_torch-0.0.3/src/ml_adapter/torch/py.typed
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:26:47.594607 waylay_ml_adapter_torch-0.0.3/src/waylay_ml_adapter_torch.egg-info/
+-rw-r--r--   0 thomas     (502) staff       (20)     4784 2024-04-24 15:26:47.000000 waylay_ml_adapter_torch-0.0.3/src/waylay_ml_adapter_torch.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (502) staff       (20)      418 2024-04-24 15:26:47.000000 waylay_ml_adapter_torch-0.0.3/src/waylay_ml_adapter_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (502) staff       (20)        1 2024-04-24 15:26:47.000000 waylay_ml_adapter_torch-0.0.3/src/waylay_ml_adapter_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (502) staff       (20)      198 2024-04-24 15:26:47.000000 waylay_ml_adapter_torch-0.0.3/src/waylay_ml_adapter_torch.egg-info/requires.txt
+-rw-r--r--   0 thomas     (502) staff       (20)       11 2024-04-24 15:26:47.000000 waylay_ml_adapter_torch-0.0.3/src/waylay_ml_adapter_torch.egg-info/top_level.txt
```

### Comparing `waylay_ml_adapter_torch-0.0.2/pyproject.toml` & `waylay_ml_adapter_torch-0.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 
 [tool.setuptools-git-versioning]
 enabled = true
 
 [project]
 name = "waylay-ml-adapter-torch"
 description = "ML_adapter for torch."
-requires-python = ">=3.9"
-authors = [{name = "Waylay"}]
+requires-python = ">=3.11"
+authors = [{name = "Waylay", email = "info@waylay.io"}]
+license={file = "LICENSE.txt"}
+readme = "README.md"
 dependencies = [
   "waylay-ml-adapter-api",
   "waylay-ml-adapter-base",
   "waylay-ml-adapter-numpy",
   "torch"
 ]
 dynamic = ["version"]
@@ -43,9 +45,9 @@
 
 [tool.ruff.lint.per-file-ignores]
 "**/*test.py" = ["D"] # no docstyle required
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 markers = [
-    "exclude_ci: marks tests to exlude for ci (unstable or requires additional config)"
+    "exclude_ci: marks tests to exclude for ci (unstable or requires additional config)"
 ]
```

### Comparing `waylay_ml_adapter_torch-0.0.2/src/ml_adapter/torch/adapter.py` & `waylay_ml_adapter_torch-0.0.3/src/ml_adapter/torch/adapter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Torch ML adapter."""
 
-from typing import Optional
-
 import ml_adapter.api.types as T
 import ml_adapter.base as A
 import ml_adapter.base.model as M
 from ml_adapter.api.data import v1 as V1
 from ml_adapter.api.data.common import V1_PROTOCOL
 from ml_adapter.base.assets import AssetsFolder
 from ml_adapter.base.assets.manifest import (
@@ -28,15 +26,15 @@
 
 TORCH_DEVICE = "cuda" if torch.cuda.is_available() else "cpu"
 
 
 class TorchModelAsset(M.ModelAsset[nn.Module]):
     """Model asset for pytorch models (fully serialized)."""
 
-    PATH_PATTERNS = ["*.pt", "*.pth"]
+    PATH_INCLUDES = ["*.pt", "*.pth"]
     DEFAULT_PATH = "model.pt"
 
     async def load_content(self, **kwargs):
         """Load a dill model."""
         with open(self.location, "rb") as f:
             model = torch.load(f)  # type: ignore
             # torch evaluation mode
@@ -49,24 +47,24 @@
         with open(self.location, "wb") as f:
             torch.save(self.content, f)
 
 
 class TorchModelWeightsAsset(M.ModelAsset[nn.Module]):
     """Model asset for pytorch models (only weights serialized)."""
 
-    PATH_PATTERNS = ["*weights.pt", "*weights.pth"]
+    PATH_INCLUDES = ["*weights.pt", "*weights.pth", "*Weights.pt", "*Weights.pth"]
     DEFAULT_PATH = "model_weights.pt"
-    MODEL_CLASS: Optional[type[nn.Module]] = None
+    MODEL_CLASS: type[nn.Module] | None = None
 
     model_class: type[nn.Module]
 
     def __init__(
         self,
         parent: AssetsFolder,
-        model_class: Optional[type[nn.Module]] = None,
+        model_class: type[nn.Module] | None = None,
         **kwargs,
     ):
         """Create a model loading weights."""
         super().__init__(parent, **kwargs)
         model_class = model_class or self.MODEL_CLASS
         if not model_class:
             raise TypeError(
@@ -109,15 +107,15 @@
 
     DEFAULT_MARSHALLER = V1TorchMarshaller
     MODEL_ASSET_CLASSES = [TorchModelWeightsAsset, TorchModelAsset]
     DEFAULT_MODEL_PATH = "model.pt"
     PROTOCOL = V1_PROTOCOL
     DEFAULT_REQUIREMENTS = TORCH_REQUIREMENTS
     DEFAULT_SCRIPT = {
-        "webscript": default_webscript_script("ml_adapter.torch", "V1TorchAdapter"),
-        "plug": default_plug_v1_script("ml_adapter.torch", "V1TorchAdapter"),
+        "webscript": default_webscript_script,
+        "plug": default_plug_v1_script,
     }
 
     @property
     def invoker(self) -> T.ModelInvoker:
         """Natively invoke the torch model without gradients calculation."""
         return torch.no_grad(super().invoker)
```

### Comparing `waylay_ml_adapter_torch-0.0.2/src/ml_adapter/torch/marshall.py` & `waylay_ml_adapter_torch-0.0.3/src/ml_adapter/torch/marshall.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Pytorch ML Marshaller."""
 
-from typing import Optional
-
 import ml_adapter.base.marshall.v1.base as V1B
 import numpy.typing as npt
 from ml_adapter.api.data import common as C
 from ml_adapter.api.data import v1 as V1
 from ml_adapter.numpy.marshall import V1NumpyEncoding
 
 import torch
@@ -22,15 +20,15 @@
     """Encoding and decoding of v1 tensors to pytorch arrays."""
 
     _numpy = V1NumpyEncoding()
 
     def decode(
         self,
         value: V1.ValueOrTensor,
-        dtype: Optional[npt.DTypeLike] = TORCH_DEFAULT_DTYPE,
+        dtype: npt.DTypeLike | None = TORCH_DEFAULT_DTYPE,
         datatype: str = C.DataTypes.DEFAULT,
         **kwargs,
     ) -> TorchTensor:
         """Map a value tensor, decoding binary data."""
         return torch.from_numpy(self._numpy.decode(value, dtype, datatype)).to(
             TORCH_DEVICE
         )
```

