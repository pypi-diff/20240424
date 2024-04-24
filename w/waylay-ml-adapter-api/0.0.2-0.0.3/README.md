# Comparing `tmp/waylay_ml_adapter_api-0.0.2.tar.gz` & `tmp/waylay_ml_adapter_api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_ml_adapter_api-0.0.2.tar", last modified: Wed Apr 17 09:14:25 2024, max compression
+gzip compressed data, was "waylay_ml_adapter_api-0.0.3.tar", last modified: Wed Apr 24 15:22:55 2024, max compression
```

## Comparing `waylay_ml_adapter_api-0.0.2.tar` & `waylay_ml_adapter_api-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:25.758282 waylay_ml_adapter_api-0.0.2/
--rw-r--r--   0 thomas     (502) staff       (20)      221 2024-04-17 09:14:25.757840 waylay_ml_adapter_api-0.0.2/PKG-INFO
--rw-r--r--   0 thomas     (502) staff       (20)       62 2023-11-28 14:22:50.000000 waylay_ml_adapter_api-0.0.2/README.md
--rw-r--r--   0 thomas     (502) staff       (20)      822 2024-03-19 07:45:20.000000 waylay_ml_adapter_api-0.0.2/pyproject.toml
--rw-r--r--   0 thomas     (502) staff       (20)       38 2024-04-17 09:14:25.758344 waylay_ml_adapter_api-0.0.2/setup.cfg
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:25.749961 waylay_ml_adapter_api-0.0.2/src/
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:25.749595 waylay_ml_adapter_api-0.0.2/src/ml_adapter/
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:25.752056 waylay_ml_adapter_api-0.0.2/src/ml_adapter/api/
--rw-r--r--   0 thomas     (502) staff       (20)       22 2023-11-28 14:21:53.000000 waylay_ml_adapter_api-0.0.2/src/ml_adapter/api/__init__.py
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:25.753273 waylay_ml_adapter_api-0.0.2/src/ml_adapter/api/data/
--rw-r--r--   0 thomas     (502) staff       (20)       92 2024-03-19 07:45:20.000000 waylay_ml_adapter_api-0.0.2/src/ml_adapter/api/data/__init__.py
--rw-r--r--   0 thomas     (502) staff       (20)     1022 2024-03-19 07:45:20.000000 waylay_ml_adapter_api-0.0.2/src/ml_adapter/api/data/common.py
--rw-r--r--   0 thomas     (502) staff       (20)     1776 2024-03-19 07:45:20.000000 waylay_ml_adapter_api-0.0.2/src/ml_adapter/api/data/v1.py
--rw-r--r--   0 thomas     (502) staff       (20)     1207 2024-03-19 07:45:20.000000 waylay_ml_adapter_api-0.0.2/src/ml_adapter/api/data/v2.py
--rw-r--r--   0 thomas     (502) staff       (20)       48 2023-12-07 15:05:11.000000 waylay_ml_adapter_api-0.0.2/src/ml_adapter/api/error.py
--rw-r--r--   0 thomas     (502) staff       (20)        0 2023-11-24 15:36:52.000000 waylay_ml_adapter_api-0.0.2/src/ml_adapter/api/py.typed
--rw-r--r--   0 thomas     (502) staff       (20)     2925 2024-03-19 07:45:20.000000 waylay_ml_adapter_api-0.0.2/src/ml_adapter/api/types.py
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:25.757116 waylay_ml_adapter_api-0.0.2/src/waylay_ml_adapter_api.egg-info/
--rw-r--r--   0 thomas     (502) staff       (20)      221 2024-04-17 09:14:25.000000 waylay_ml_adapter_api-0.0.2/src/waylay_ml_adapter_api.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (502) staff       (20)      513 2024-04-17 09:14:25.000000 waylay_ml_adapter_api-0.0.2/src/waylay_ml_adapter_api.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (502) staff       (20)        1 2024-04-17 09:14:25.000000 waylay_ml_adapter_api-0.0.2/src/waylay_ml_adapter_api.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (502) staff       (20)       34 2024-04-17 09:14:25.000000 waylay_ml_adapter_api-0.0.2/src/waylay_ml_adapter_api.egg-info/requires.txt
--rw-r--r--   0 thomas     (502) staff       (20)       11 2024-04-17 09:14:25.000000 waylay_ml_adapter_api-0.0.2/src/waylay_ml_adapter_api.egg-info/top_level.txt
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:22:55.682128 waylay_ml_adapter_api-0.0.3/
+-rw-r--r--   0 thomas     (502) staff       (20)      746 2024-04-24 15:21:52.000000 waylay_ml_adapter_api-0.0.3/LICENCE.txt
+-rw-r--r--   0 thomas     (502) staff       (20)     1934 2024-04-24 15:22:55.681314 waylay_ml_adapter_api-0.0.3/PKG-INFO
+-rw-r--r--   0 thomas     (502) staff       (20)     1622 2024-04-24 11:51:37.000000 waylay_ml_adapter_api-0.0.3/README.md
+-rw-r--r--   0 thomas     (502) staff       (20)      901 2024-04-24 15:21:52.000000 waylay_ml_adapter_api-0.0.3/pyproject.toml
+-rw-r--r--   0 thomas     (502) staff       (20)       38 2024-04-24 15:22:55.682218 waylay_ml_adapter_api-0.0.3/setup.cfg
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:22:55.674946 waylay_ml_adapter_api-0.0.3/src/
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:22:55.674664 waylay_ml_adapter_api-0.0.3/src/ml_adapter/
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:22:55.676074 waylay_ml_adapter_api-0.0.3/src/ml_adapter/api/
+-rw-r--r--   0 thomas     (502) staff       (20)       72 2024-04-22 08:55:37.000000 waylay_ml_adapter_api-0.0.3/src/ml_adapter/api/__init__.py
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:22:55.677236 waylay_ml_adapter_api-0.0.3/src/ml_adapter/api/data/
+-rw-r--r--   0 thomas     (502) staff       (20)       92 2024-03-19 07:45:20.000000 waylay_ml_adapter_api-0.0.3/src/ml_adapter/api/data/__init__.py
+-rw-r--r--   0 thomas     (502) staff       (20)     1017 2024-04-24 15:21:52.000000 waylay_ml_adapter_api-0.0.3/src/ml_adapter/api/data/common.py
+-rw-r--r--   0 thomas     (502) staff       (20)     1776 2024-03-19 07:45:20.000000 waylay_ml_adapter_api-0.0.3/src/ml_adapter/api/data/v1.py
+-rw-r--r--   0 thomas     (502) staff       (20)     1207 2024-03-19 07:45:20.000000 waylay_ml_adapter_api-0.0.3/src/ml_adapter/api/data/v2.py
+-rw-r--r--   0 thomas     (502) staff       (20)        0 2023-11-24 15:36:52.000000 waylay_ml_adapter_api-0.0.3/src/ml_adapter/api/py.typed
+-rw-r--r--   0 thomas     (502) staff       (20)     2896 2024-04-24 15:21:52.000000 waylay_ml_adapter_api-0.0.3/src/ml_adapter/api/types.py
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:22:55.680917 waylay_ml_adapter_api-0.0.3/src/waylay_ml_adapter_api.egg-info/
+-rw-r--r--   0 thomas     (502) staff       (20)     1934 2024-04-24 15:22:55.000000 waylay_ml_adapter_api-0.0.3/src/waylay_ml_adapter_api.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (502) staff       (20)      497 2024-04-24 15:22:55.000000 waylay_ml_adapter_api-0.0.3/src/waylay_ml_adapter_api.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (502) staff       (20)        1 2024-04-24 15:22:55.000000 waylay_ml_adapter_api-0.0.3/src/waylay_ml_adapter_api.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (502) staff       (20)       34 2024-04-24 15:22:55.000000 waylay_ml_adapter_api-0.0.3/src/waylay_ml_adapter_api.egg-info/requires.txt
+-rw-r--r--   0 thomas     (502) staff       (20)       11 2024-04-24 15:22:55.000000 waylay_ml_adapter_api-0.0.3/src/waylay_ml_adapter_api.egg-info/top_level.txt
```

### Comparing `waylay_ml_adapter_api-0.0.2/pyproject.toml` & `waylay_ml_adapter_api-0.0.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 
 [tool.setuptools-git-versioning]
 enabled = true
 
 [project]
 name = "waylay-ml-adapter-api"
 description = "API models for the ml-adapter."
-requires-python = ">=3.9"
-authors = [{name = "Waylay"}]
+requires-python = ">=3.11"
+authors = [{name = "Waylay", email = "info@waylay.io"}]
+license={file = "LICENSE.txt"}
+readme = "README.md"
 dependencies = [
 ]
 dynamic = ["version"]
 
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `waylay_ml_adapter_api-0.0.2/src/ml_adapter/api/data/common.py` & `waylay_ml_adapter_api-0.0.3/src/ml_adapter/api/data/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,12 +37,12 @@
 NamedTensors = dict[str, Tensor]
 
 ScalarTensorOrNamed = ScalarOrBytes | NamedScalarOrTensors
 
 BytesTensor = list[Union[bytes, "BytesTensor"]]
 BytesOrBytesTensor = bytes | BytesTensor
 
-InferenceProtocol = Union[Literal["KServe-1.0"], Literal["OIP-2.0"], Literal["N/A"]]
+InferenceProtocol = Literal["KServe-1.0"] | Literal["OIP-2.0"] | Literal["N/A"]
 
 V1_PROTOCOL: InferenceProtocol = "KServe-1.0"
 V2_PROTOCOL: InferenceProtocol = "OIP-2.0"
 NO_PROTOCOL: InferenceProtocol = "N/A"
```

### Comparing `waylay_ml_adapter_api-0.0.2/src/ml_adapter/api/data/v1.py` & `waylay_ml_adapter_api-0.0.3/src/ml_adapter/api/data/v1.py`

 * *Files identical despite different names*

### Comparing `waylay_ml_adapter_api-0.0.2/src/ml_adapter/api/data/v2.py` & `waylay_ml_adapter_api-0.0.3/src/ml_adapter/api/data/v2.py`

 * *Files identical despite different names*

### Comparing `waylay_ml_adapter_api-0.0.2/src/ml_adapter/api/types.py` & `waylay_ml_adapter_api-0.0.3/src/ml_adapter/api/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Types related to model loading."""
 
 import io
 from pathlib import Path
-from typing import Generic, Optional, Protocol, TypeVar, Union
+from typing import Generic, Protocol, TypeVar
 
 from .data.common import Parameters
 
 AssetLocation = Path
 AssetSource = AssetLocation | str | io.IOBase
 
 
-def as_location(location: Optional[AssetLocation | str]) -> AssetLocation:
+def as_location(location: AssetLocation | str | None) -> AssetLocation:
     """Parse a location specification as location path."""
     return Path(location or ".")
 
 
 #: Model Instance Type Variable
 MI = TypeVar("MI")
 #: Native Model Inference Request
@@ -82,15 +82,15 @@
         """Signature for save the model instance."""
 
     @classmethod
     def load(cls: type[MI], location: AssetLocation, **kwargs) -> MI:
         """Signature to load the model instance."""
 
 
-SerializableModel = Union[AsyncSerializableModel, SyncSerializableModel]
+SerializableModel = AsyncSerializableModel | SyncSerializableModel
 
-ModelInvoker = Union[
-    AsyncModelInvoker[MREQ, MRES],
-    AsyncModelInvokerWithParams[MREQ, MRES],
-    SyncModelInvoker[MREQ, MRES],
-    SyncModelInvokerWithParams[MREQ, MRES],
-]
+ModelInvoker = (
+    AsyncModelInvoker[MREQ, MRES]
+    | AsyncModelInvokerWithParams[MREQ, MRES]
+    | SyncModelInvoker[MREQ, MRES]
+    | SyncModelInvokerWithParams[MREQ, MRES]
+)
```

