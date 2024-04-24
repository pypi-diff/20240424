# Comparing `tmp/waylay_ml_adapter_numpy-0.0.2.tar.gz` & `tmp/waylay_ml_adapter_numpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_ml_adapter_numpy-0.0.2.tar", last modified: Wed Apr 17 09:14:45 2024, max compression
+gzip compressed data, was "waylay_ml_adapter_numpy-0.0.3.tar", last modified: Wed Apr 24 15:24:51 2024, max compression
```

## Comparing `waylay_ml_adapter_numpy-0.0.2.tar` & `waylay_ml_adapter_numpy-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:45.271979 waylay_ml_adapter_numpy-0.0.2/
--rw-r--r--   0 thomas     (502) staff       (20)      281 2024-04-17 09:14:45.271356 waylay_ml_adapter_numpy-0.0.2/PKG-INFO
--rw-r--r--   0 thomas     (502) staff       (20)      912 2024-04-17 08:27:35.000000 waylay_ml_adapter_numpy-0.0.2/pyproject.toml
--rw-r--r--   0 thomas     (502) staff       (20)       38 2024-04-17 09:14:45.272058 waylay_ml_adapter_numpy-0.0.2/setup.cfg
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:45.264570 waylay_ml_adapter_numpy-0.0.2/src/
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:45.264396 waylay_ml_adapter_numpy-0.0.2/src/ml_adapter/
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:45.266319 waylay_ml_adapter_numpy-0.0.2/src/ml_adapter/numpy/
--rw-r--r--   0 thomas     (502) staff       (20)      166 2024-03-19 07:45:20.000000 waylay_ml_adapter_numpy-0.0.2/src/ml_adapter/numpy/__init__.py
--rw-r--r--   0 thomas     (502) staff       (20)     1210 2024-04-17 08:27:35.000000 waylay_ml_adapter_numpy-0.0.2/src/ml_adapter/numpy/adapter.py
--rw-r--r--   0 thomas     (502) staff       (20)     4944 2024-04-17 08:27:35.000000 waylay_ml_adapter_numpy-0.0.2/src/ml_adapter/numpy/marshall.py
--rw-r--r--   0 thomas     (502) staff       (20)        0 2023-12-05 09:35:32.000000 waylay_ml_adapter_numpy-0.0.2/src/ml_adapter/numpy/py.typed
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:45.270850 waylay_ml_adapter_numpy-0.0.2/src/waylay_ml_adapter_numpy.egg-info/
--rw-r--r--   0 thomas     (502) staff       (20)      281 2024-04-17 09:14:45.000000 waylay_ml_adapter_numpy-0.0.2/src/waylay_ml_adapter_numpy.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (502) staff       (20)      396 2024-04-17 09:14:45.000000 waylay_ml_adapter_numpy-0.0.2/src/waylay_ml_adapter_numpy.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (502) staff       (20)        1 2024-04-17 09:14:45.000000 waylay_ml_adapter_numpy-0.0.2/src/waylay_ml_adapter_numpy.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (502) staff       (20)       71 2024-04-17 09:14:45.000000 waylay_ml_adapter_numpy-0.0.2/src/waylay_ml_adapter_numpy.egg-info/requires.txt
--rw-r--r--   0 thomas     (502) staff       (20)       11 2024-04-17 09:14:45.000000 waylay_ml_adapter_numpy-0.0.2/src/waylay_ml_adapter_numpy.egg-info/top_level.txt
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:24:51.873968 waylay_ml_adapter_numpy-0.0.3/
+-rw-r--r--   0 thomas     (502) staff       (20)      746 2024-04-24 15:21:52.000000 waylay_ml_adapter_numpy-0.0.3/LICENCE.txt
+-rw-r--r--   0 thomas     (502) staff       (20)     1026 2024-04-24 15:24:51.873383 waylay_ml_adapter_numpy-0.0.3/PKG-INFO
+-rw-r--r--   0 thomas     (502) staff       (20)      654 2024-04-24 11:51:39.000000 waylay_ml_adapter_numpy-0.0.3/README.md
+-rw-r--r--   0 thomas     (502) staff       (20)     1095 2024-04-24 15:21:52.000000 waylay_ml_adapter_numpy-0.0.3/pyproject.toml
+-rw-r--r--   0 thomas     (502) staff       (20)       38 2024-04-24 15:24:51.874019 waylay_ml_adapter_numpy-0.0.3/setup.cfg
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:24:51.864650 waylay_ml_adapter_numpy-0.0.3/src/
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:24:51.864365 waylay_ml_adapter_numpy-0.0.3/src/ml_adapter/
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:24:51.868954 waylay_ml_adapter_numpy-0.0.3/src/ml_adapter/numpy/
+-rw-r--r--   0 thomas     (502) staff       (20)      166 2024-04-22 08:55:37.000000 waylay_ml_adapter_numpy-0.0.3/src/ml_adapter/numpy/__init__.py
+-rw-r--r--   0 thomas     (502) staff       (20)     1102 2024-04-24 10:44:07.000000 waylay_ml_adapter_numpy-0.0.3/src/ml_adapter/numpy/adapter.py
+-rw-r--r--   0 thomas     (502) staff       (20)     4924 2024-04-24 15:21:52.000000 waylay_ml_adapter_numpy-0.0.3/src/ml_adapter/numpy/marshall.py
+-rw-r--r--   0 thomas     (502) staff       (20)        0 2023-12-05 09:35:32.000000 waylay_ml_adapter_numpy-0.0.3/src/ml_adapter/numpy/py.typed
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:24:51.872733 waylay_ml_adapter_numpy-0.0.3/src/waylay_ml_adapter_numpy.egg-info/
+-rw-r--r--   0 thomas     (502) staff       (20)     1026 2024-04-24 15:24:51.000000 waylay_ml_adapter_numpy-0.0.3/src/waylay_ml_adapter_numpy.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (502) staff       (20)      418 2024-04-24 15:24:51.000000 waylay_ml_adapter_numpy-0.0.3/src/waylay_ml_adapter_numpy.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (502) staff       (20)        1 2024-04-24 15:24:51.000000 waylay_ml_adapter_numpy-0.0.3/src/waylay_ml_adapter_numpy.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (502) staff       (20)       71 2024-04-24 15:24:51.000000 waylay_ml_adapter_numpy-0.0.3/src/waylay_ml_adapter_numpy.egg-info/requires.txt
+-rw-r--r--   0 thomas     (502) staff       (20)       11 2024-04-24 15:24:51.000000 waylay_ml_adapter_numpy-0.0.3/src/waylay_ml_adapter_numpy.egg-info/top_level.txt
```

### Comparing `waylay_ml_adapter_numpy-0.0.2/pyproject.toml` & `waylay_ml_adapter_numpy-0.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 
 [tool.setuptools-git-versioning]
 enabled = true
 
 [project]
 name = "waylay-ml-adapter-numpy"
 description = "ML_adapter for numpy."
-requires-python = ">=3.9"
-authors = [{name = "Waylay"}]
+requires-python = ">=3.11"
+authors = [{name = "Waylay", email = "info@waylay.io"}]
+license={file = "LICENSE.txt"}
+readme = "README.md"
 dependencies = [
   "numpy>=1.25.0",
   "waylay-ml-adapter-base"
 ]
 dynamic = ["version"]
 
 
@@ -37,8 +39,11 @@
 [tool.ruff.lint]
 select = ["E", "F", "UP",  "B", "SIM", "I", "D1", "D4"]
 
 [tool.ruff.lint.per-file-ignores]
 "**/*test.py" = ["D"] # no docstyle required
 
 [tool.pytest.ini_options]
-asyncio_mode = "auto"
+asyncio_mode = "auto"
+markers = [
+    "exclude_ci: marks tests to exclude for ci (unstable or requires additional config)"
+]
```

### Comparing `waylay_ml_adapter_numpy-0.0.2/src/ml_adapter/numpy/adapter.py` & `waylay_ml_adapter_numpy-0.0.3/src/ml_adapter/numpy/adapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,12 +38,10 @@
 ):
     """Adapts a callable with numpy arrays as input and output."""
 
     DEFAULT_MARSHALLER = V1NumpyMarshaller
     PROTOCOL = V1_PROTOCOL
     DEFAULT_REQUIREMENTS = NUMPY_REQUIREMENTS
     DEFAULT_SCRIPT = {
-        "webscript": default_webscript_script(
-            "ml_adapter.numpy", "V1NumpyModelAdapter"
-        ),
-        "plug": default_plug_v1_script("ml_adapter.numpy", "V1NumpyModelAdapter"),
+        "webscript": default_webscript_script,
+        "plug": default_plug_v1_script,
     }
```

### Comparing `waylay_ml_adapter_numpy-0.0.2/src/ml_adapter/numpy/marshall.py` & `waylay_ml_adapter_numpy-0.0.3/src/ml_adapter/numpy/marshall.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Numpy ML Marshaller."""
 
 from collections.abc import Iterator, Mapping
-from typing import Any, Optional, cast
+from typing import Any, cast
 
 import ml_adapter.base.marshall.v1.base as V1B
 from ml_adapter.api import types as T
 from ml_adapter.api.data import common as C
 from ml_adapter.api.data import v1 as V1
 from ml_adapter.base.marshall.v1 import list as V1L
 
@@ -36,46 +36,46 @@
 
 def iter_decode_binary(value: Any) -> Iterator[bytes]:
     """Decode a base64 binary value."""
     if not isinstance(value, list):
         yield V1L.decode_binary(value)
         return
     evidence = value[0]
-    if isinstance(evidence, (str, dict)):
+    if isinstance(evidence, str | dict):
         for v in value:
             yield V1L.decode_binary(v)
         return
     if isinstance(evidence, list):
         for v in value:
             yield from iter_decode_binary(v)
         return
     yield from value
 
 
 def iter_flattened(value: C.Tensor) -> Iterator[C.Scalar]:
     """Iterate over a lists of lists."""
-    if isinstance(value, (list, Iterator)):
+    if isinstance(value, list | Iterator):
         for v in value:
             yield from iter_flattened(v)
         return
     yield value
 
 
-def _get_request_dtype(**kwargs) -> Optional[npt.DTypeLike]:
+def _get_request_dtype(**kwargs) -> npt.DTypeLike | None:
     datatype = kwargs.get("datatype", "_")
     return NUMPY_DATA_TYPES.get(datatype)
 
 
 class V1NumpyEncoding(V1B.WithV1TensorEncoding[npt.ArrayLike]):
     """Encoding and decoding of v1 tensors to numpy arrays."""
 
     def decode(
         self,
         value: V1.ValueOrTensor,
-        dtype: Optional[npt.DTypeLike] = None,
+        dtype: npt.DTypeLike | None = None,
         datatype: str = C.DataTypes.DEFAULT,
     ) -> npt.ArrayLike:
         """Map a value tensor, decoding binary data."""
         if V1.is_binary(value, datatype):
             dtype = dtype or np.object_
             return np.fromiter(iter_decode_binary(value), dtype=dtype).reshape(
                 np.shape(value)
@@ -92,15 +92,15 @@
 
 
 class V1NumpyMarshaller(
     V1B.V1ValueOrDictRequestMarshallerBase[npt.ArrayLike],
     V1B.V1ValueOrDictResponseMarshallerBase[npt.ArrayLike],
     V1NumpyEncoding,
 ):
-    """Convert v1 payload from and to numpy arrays."""
+    """Converts v1 payload from and to numpy arrays."""
 
     def map_decoding_kwargs(
         self, parameters: C.Parameters, **kwargs
     ) -> Mapping[str, Any]:
         """Provide default for dtype."""
         dtype = kwargs.pop("dtype", _get_request_dtype(**kwargs))
         return super().map_decoding_kwargs(parameters, dtype=dtype, **kwargs)
@@ -115,15 +115,15 @@
         self, response: ArraysOrNamedArrays, /, **kwargs
     ) -> V1.NamedValues:
         """Map model response to named values."""
         return self.encode_as_named(response, **kwargs)
 
     def decode_response(
         self, response: V1.V1PredictionResponse, /, **kwargs
-    ) -> tuple[ArraysOrNamedArrays, Optional[T.Parameters]]:
+    ) -> tuple[ArraysOrNamedArrays, T.Parameters | None]:
         """Decode a v1 inference response."""
         dtype = kwargs.pop("dtype", _get_request_dtype(**kwargs))
         return super().decode_response(response, dtype=dtype, **kwargs)
 
     def decode_named_values(
         self, response: list[V1.NamedValues], /, **kwargs
     ) -> ArraysOrNamedArrays:
```

