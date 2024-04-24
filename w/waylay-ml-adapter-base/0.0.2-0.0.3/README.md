# Comparing `tmp/waylay_ml_adapter_base-0.0.2.tar.gz` & `tmp/waylay_ml_adapter_base-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_ml_adapter_base-0.0.2.tar", last modified: Wed Apr 17 09:14:32 2024, max compression
+gzip compressed data, was "waylay_ml_adapter_base-0.0.3.tar", last modified: Wed Apr 24 15:23:29 2024, max compression
```

## Comparing `waylay_ml_adapter_base-0.0.2.tar` & `waylay_ml_adapter_base-0.0.3.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:32.071910 waylay_ml_adapter_base-0.0.2/
--rw-r--r--   0 thomas     (502) staff       (20)      681 2024-04-17 09:14:32.071312 waylay_ml_adapter_base-0.0.2/PKG-INFO
--rw-r--r--   0 thomas     (502) staff       (20)       65 2023-11-28 14:22:50.000000 waylay_ml_adapter_base-0.0.2/README.md
--rw-r--r--   0 thomas     (502) staff       (20)     1035 2024-03-19 07:45:20.000000 waylay_ml_adapter_base-0.0.2/pyproject.toml
--rw-r--r--   0 thomas     (502) staff       (20)       38 2024-04-17 09:14:32.071981 waylay_ml_adapter_base-0.0.2/setup.cfg
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:32.051876 waylay_ml_adapter_base-0.0.2/src/
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:32.051021 waylay_ml_adapter_base-0.0.2/src/ml_adapter/
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:32.054946 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/
--rw-r--r--   0 thomas     (502) staff       (20)      557 2024-03-19 07:45:20.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/__init__.py
--rw-r--r--   0 thomas     (502) staff       (20)     5819 2024-04-17 08:27:35.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/adapter.py
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:32.063538 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/
--rw-r--r--   0 thomas     (502) staff       (20)      872 2024-03-19 07:45:20.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/__init__.py
--rw-r--r--   0 thomas     (502) staff       (20)      655 2024-03-19 07:45:20.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/_err.py
--rw-r--r--   0 thomas     (502) staff       (20)    18404 2024-03-19 07:45:20.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/base.py
--rw-r--r--   0 thomas     (502) staff       (20)     1756 2024-03-19 07:45:20.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/cached.py
--rw-r--r--   0 thomas     (502) staff       (20)     1525 2024-04-17 08:27:35.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/default.v1.plug.json
--rw-r--r--   0 thomas     (502) staff       (20)      171 2024-01-29 09:33:59.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/default.v1.webscript.json
--rw-r--r--   0 thomas     (502) staff       (20)     2920 2024-04-16 15:58:38.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/default.v2.plug.json
--rw-r--r--   0 thomas     (502) staff       (20)      966 2024-03-19 07:45:20.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/json.py
--rw-r--r--   0 thomas     (502) staff       (20)     9636 2024-04-17 08:27:35.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/manifest.py
--rw-r--r--   0 thomas     (502) staff       (20)     1204 2024-03-19 07:45:20.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/mixin.py
--rw-r--r--   0 thomas     (502) staff       (20)     3521 2024-03-19 07:45:20.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/openapi.py
--rw-r--r--   0 thomas     (502) staff       (20)     7438 2024-04-15 14:44:44.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/python.py
--rw-r--r--   0 thomas     (502) staff       (20)      803 2024-03-19 07:45:20.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/root.py
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:32.064187 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/marshall/
--rw-r--r--   0 thomas     (502) staff       (20)      110 2024-03-19 07:45:20.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/marshall/__init__.py
--rw-r--r--   0 thomas     (502) staff       (20)     2534 2024-04-17 08:27:35.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/marshall/base.py
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:32.065318 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/marshall/v1/
--rw-r--r--   0 thomas     (502) staff       (20)      128 2024-03-19 07:45:20.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/marshall/v1/__init__.py
--rw-r--r--   0 thomas     (502) staff       (20)    18208 2024-04-17 08:27:35.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/marshall/v1/base.py
--rw-r--r--   0 thomas     (502) staff       (20)     2671 2024-03-19 07:45:20.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/marshall/v1/list.py
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:32.067249 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/model/
--rw-r--r--   0 thomas     (502) staff       (20)      335 2024-03-19 07:45:20.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/model/__init__.py
--rw-r--r--   0 thomas     (502) staff       (20)     3058 2024-04-17 08:27:35.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/model/access.py
--rw-r--r--   0 thomas     (502) staff       (20)      624 2024-04-17 08:27:35.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/model/base.py
--rw-r--r--   0 thomas     (502) staff       (20)      875 2024-03-19 07:45:20.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/model/dill.py
--rw-r--r--   0 thomas     (502) staff       (20)     1075 2024-03-19 07:45:20.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/model/joblib.py
--rw-r--r--   0 thomas     (502) staff       (20)     1526 2024-04-17 08:27:35.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/model/serialize.py
--rw-r--r--   0 thomas     (502) staff       (20)        0 2023-11-24 15:37:37.000000 waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/py.typed
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:32.070081 waylay_ml_adapter_base-0.0.2/src/waylay_ml_adapter_base.egg-info/
--rw-r--r--   0 thomas     (502) staff       (20)      681 2024-04-17 09:14:32.000000 waylay_ml_adapter_base-0.0.2/src/waylay_ml_adapter_base.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (502) staff       (20)     1299 2024-04-17 09:14:32.000000 waylay_ml_adapter_base-0.0.2/src/waylay_ml_adapter_base.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (502) staff       (20)        1 2024-04-17 09:14:32.000000 waylay_ml_adapter_base-0.0.2/src/waylay_ml_adapter_base.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (502) staff       (20)      166 2024-04-17 09:14:32.000000 waylay_ml_adapter_base-0.0.2/src/waylay_ml_adapter_base.egg-info/requires.txt
--rw-r--r--   0 thomas     (502) staff       (20)       11 2024-04-17 09:14:32.000000 waylay_ml_adapter_base-0.0.2/src/waylay_ml_adapter_base.egg-info/top_level.txt
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:23:29.845263 waylay_ml_adapter_base-0.0.3/
+-rw-r--r--   0 thomas     (502) staff       (20)      746 2024-04-24 15:21:52.000000 waylay_ml_adapter_base-0.0.3/LICENCE.txt
+-rw-r--r--   0 thomas     (502) staff       (20)     5887 2024-04-24 15:23:29.844814 waylay_ml_adapter_base-0.0.3/PKG-INFO
+-rw-r--r--   0 thomas     (502) staff       (20)     5115 2024-04-24 11:51:38.000000 waylay_ml_adapter_base-0.0.3/README.md
+-rw-r--r--   0 thomas     (502) staff       (20)     1114 2024-04-24 15:21:52.000000 waylay_ml_adapter_base-0.0.3/pyproject.toml
+-rw-r--r--   0 thomas     (502) staff       (20)       38 2024-04-24 15:23:29.845310 waylay_ml_adapter_base-0.0.3/setup.cfg
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:23:29.819767 waylay_ml_adapter_base-0.0.3/src/
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:23:29.819063 waylay_ml_adapter_base-0.0.3/src/ml_adapter/
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:23:29.821412 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/
+-rw-r--r--   0 thomas     (502) staff       (20)      557 2024-03-19 07:45:20.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/__init__.py
+-rw-r--r--   0 thomas     (502) staff       (20)     6368 2024-04-24 15:21:52.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/adapter.py
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:23:29.832446 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/
+-rw-r--r--   0 thomas     (502) staff       (20)      872 2024-03-19 07:45:20.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/__init__.py
+-rw-r--r--   0 thomas     (502) staff       (20)      655 2024-03-19 07:45:20.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/_err.py
+-rw-r--r--   0 thomas     (502) staff       (20)    19987 2024-04-24 15:21:52.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/base.py
+-rw-r--r--   0 thomas     (502) staff       (20)     1743 2024-04-24 15:21:52.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/cached.py
+-rw-r--r--   0 thomas     (502) staff       (20)     1525 2024-04-17 08:27:35.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/default.v1.plug.json
+-rw-r--r--   0 thomas     (502) staff       (20)      171 2024-01-29 09:33:59.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/default.v1.webscript.json
+-rw-r--r--   0 thomas     (502) staff       (20)     2920 2024-04-16 15:58:38.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/default.v2.plug.json
+-rw-r--r--   0 thomas     (502) staff       (20)      966 2024-04-22 08:55:37.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/json.py
+-rw-r--r--   0 thomas     (502) staff       (20)    11144 2024-04-24 15:21:52.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/manifest.py
+-rw-r--r--   0 thomas     (502) staff       (20)     1429 2024-04-24 15:21:52.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/mixin.py
+-rw-r--r--   0 thomas     (502) staff       (20)     3714 2024-04-24 15:21:52.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/openapi.py
+-rw-r--r--   0 thomas     (502) staff       (20)     8028 2024-04-24 15:21:52.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/python.py
+-rw-r--r--   0 thomas     (502) staff       (20)      803 2024-03-19 07:45:20.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/root.py
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:23:29.833059 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/marshall/
+-rw-r--r--   0 thomas     (502) staff       (20)      110 2024-03-19 07:45:20.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/marshall/__init__.py
+-rw-r--r--   0 thomas     (502) staff       (20)     3081 2024-04-24 15:21:52.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/marshall/base.py
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:23:29.836938 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/marshall/v1/
+-rw-r--r--   0 thomas     (502) staff       (20)      128 2024-03-19 07:45:20.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/marshall/v1/__init__.py
+-rw-r--r--   0 thomas     (502) staff       (20)    18161 2024-04-24 15:21:52.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/marshall/v1/base.py
+-rw-r--r--   0 thomas     (502) staff       (20)     2671 2024-03-19 07:45:20.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/marshall/v1/list.py
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:23:29.840197 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/model/
+-rw-r--r--   0 thomas     (502) staff       (20)      365 2024-04-24 10:44:07.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/model/__init__.py
+-rw-r--r--   0 thomas     (502) staff       (20)     4168 2024-04-24 15:21:52.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/model/access.py
+-rw-r--r--   0 thomas     (502) staff       (20)      624 2024-04-22 08:55:37.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/model/base.py
+-rw-r--r--   0 thomas     (502) staff       (20)     1050 2024-04-22 08:55:37.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/model/dill.py
+-rw-r--r--   0 thomas     (502) staff       (20)     1209 2024-04-22 08:55:37.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/model/joblib.py
+-rw-r--r--   0 thomas     (502) staff       (20)     1644 2024-04-24 15:21:52.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/model/serialize.py
+-rw-r--r--   0 thomas     (502) staff       (20)        0 2023-11-24 15:37:37.000000 waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/py.typed
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:23:29.844026 waylay_ml_adapter_base-0.0.3/src/waylay_ml_adapter_base.egg-info/
+-rw-r--r--   0 thomas     (502) staff       (20)     5887 2024-04-24 15:23:29.000000 waylay_ml_adapter_base-0.0.3/src/waylay_ml_adapter_base.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (502) staff       (20)     1311 2024-04-24 15:23:29.000000 waylay_ml_adapter_base-0.0.3/src/waylay_ml_adapter_base.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (502) staff       (20)        1 2024-04-24 15:23:29.000000 waylay_ml_adapter_base-0.0.3/src/waylay_ml_adapter_base.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (502) staff       (20)      166 2024-04-24 15:23:29.000000 waylay_ml_adapter_base-0.0.3/src/waylay_ml_adapter_base.egg-info/requires.txt
+-rw-r--r--   0 thomas     (502) staff       (20)       11 2024-04-24 15:23:29.000000 waylay_ml_adapter_base-0.0.3/src/waylay_ml_adapter_base.egg-info/top_level.txt
```

### Comparing `waylay_ml_adapter_base-0.0.2/pyproject.toml` & `waylay_ml_adapter_base-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 
 [tool.setuptools-git-versioning]
 enabled = true
 
 [project]
 name = "waylay-ml-adapter-base"
 description = "ml-adapter base classes."
-requires-python = ">=3.9"
-authors = [{name = "Waylay"}]
+requires-python = ">=3.11"
+authors = [{name = "Waylay", email = "info@waylay.io"}]
+license={file = "LICENSE.txt"}
+readme = "README.md"
 dependencies = [
   "waylay-ml-adapter-api",
   "openapi-spec-validator",
 ]
 dynamic = ["version"]
```

### Comparing `waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/__init__.py` & `waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/__init__.py`

 * *Files identical despite different names*

### Comparing `waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/adapter.py` & `waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/adapter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 """Base Model Adapter."""
 
 import inspect
-from typing import Generic, Optional
+from typing import Generic
 
 import ml_adapter.api.types as T
 from ml_adapter.api.data.common import NO_PROTOCOL
 from ml_adapter.base.model.access import WithModel
 
 from .marshall import Marshaller, NoMarshaller
 
 
 class ModelAdapter(Generic[T.MREQ, T.MRES, T.RREQ, T.RRES]):
-    """Model Adapter base."""
+    """Model Adapter base.
+
+    Provides the basic contract for exposing
+    a model to a waylay _plugin_ or _webscript_.
+    * delegates to a `marshaller` to map the remote,
+      json-compatible python data structures
+      from and to the native tensor data structures for the ML framework.
+    * delegates to a `invoker` to find the model method to be called
+    * the `call` method maps remote requests and invokes the model method
+    * the `call_remote` method tests the round trip serialization, encoding
+      native data request to remotable and back before invoking `call`
+    """
 
     DEFAULT_MARSHALLER = NoMarshaller
     PROTOCOL = NO_PROTOCOL
 
     model_method = ""
     _invoker: T.ModelInvoker[T.MREQ, T.MRES] | None
 
@@ -65,15 +76,15 @@
             await self.model_asset.load()
 
     async def __call__(self, request: T.RREQ, /, **kwargs) -> T.RRES:
         """Invoke the model with a remote inference request."""
         return await self.call(request, **kwargs)
 
     async def call_remote(
-        self, request: T.MREQ, parameters: Optional[T.Parameters] = None, **kwargs
+        self, request: T.MREQ, parameters: T.Parameters | None = None, **kwargs
     ) -> tuple[T.MRES, T.Parameters]:
         """Test invoke a model with marshalled request and response data."""
         remote_request = self.marshaller.encode_request(request, parameters, **kwargs)
         remote_resp = await self.call(remote_request)
         return self.marshaller.decode_response(remote_resp, **kwargs)
```

### Comparing `waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/__init__.py` & `waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/_err.py` & `waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/_err.py`

 * *Files identical despite different names*

### Comparing `waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/base.py` & `waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 """Utility functions for accessing assets."""
 
 import abc
 import fnmatch
 import io
+import logging
 import shutil
 import tarfile
 from collections.abc import Iterator
 from pathlib import Path
-from typing import Optional, Self, TypeVar, cast
+from typing import Self, TypeVar, cast
 
 from ml_adapter.api.types import AssetLocation, AssetSource, as_location
 
 from . import _err
 
+LOG = logging.getLogger(__name__)
 A = TypeVar("A", bound="Asset")
 
+PathFilter = str | list[str] | None
+
 
 class Asset(abc.ABC):
     """Item(s) that can be saved/loaded as asset(s) for a waylay function."""
 
     parent: "AssetsFolder"
     path: str
 
-    PATH_PATTERNS: list[str] = ["*"]
+    PATH_INCLUDES: list[str] = ["*"]
+    PATH_EXCLUDES: list[str] = [".*"]
     DEFAULT_PATH: str = "?"
 
-    def __init__(self, parent: "AssetsFolder", path: Optional[str] = None, **_kwargs):
+    def __init__(self, parent: "AssetsFolder", path: str | None = None, **_kwargs):
         """Create an asset in the given assets directory."""
         self.parent = parent
         self.path = path or self.DEFAULT_PATH
 
     @property
     def full_path(self) -> str:
         """Full path in an assets archive."""
@@ -70,50 +75,60 @@
     def is_empty(self):
         """Check that no content is present."""
         return not self.has_content()
 
     def iter_locations(
         self,
         /,
-        relative_to: Optional[AssetLocation | str] = None,
+        relative_to: AssetLocation | str | None = None,
         exclude_empty=False,
         **_kwargs,
     ):
         """Iterate the paths for the assets."""
         if exclude_empty and self.is_empty():
             return
         if relative_to:
             yield self.location.relative_to(as_location(relative_to))
         else:
             yield self.location
 
     def iter(
         self,
         /,
-        asset_type: Optional[type[A]] = None,
-        path_pattern: Optional[str] = None,
+        asset_type: type[A] | None = None,
+        path_includes: PathFilter = None,
+        path_excludes: PathFilter = None,
         exclude_empty=False,
         **_kwargs,
     ) -> Iterator[A]:
         """Iterate the assets."""
         if exclude_empty and self.is_empty():
             return
         if not (asset_type is None or isinstance(self, asset_type)):
             return
-        if not (path_pattern is None or fnmatch.fnmatch(self.path, path_pattern)):
+        if not self._path_matches(self.path, path_includes, path_excludes):
             return
         yield cast(A, self)
 
     @classmethod
+    def _path_matches(
+        cls,
+        path: str,
+        includes: str | list[str] | None = None,
+        excludes: str | list[str] | None = None,
+    ) -> bool:
+        excluded = _matches(path, excludes, cls.PATH_EXCLUDES)
+        default_includes = [] if excluded else cls.PATH_INCLUDES
+        return _matches(path, includes, default_includes)
+
+    @classmethod
     def supports_path(cls, path: str, is_dir: bool) -> bool:
         """Check whether this asset class can load the given class."""
         assert isinstance(is_dir, bool)
-        return not cls.PATH_PATTERNS or any(
-            fnmatch.fnmatch(path, pattern) for pattern in cls.PATH_PATTERNS
-        )
+        return cls._path_matches(path)
 
     async def load_from(self, source: AssetSource):
         """Copy external data to this asse, replacing existing data."""
         if source == self.location:
             pass
         elif isinstance(source, io.TextIOBase):
             with open(self.location, "w", encoding="utf-8") as target:
@@ -126,14 +141,22 @@
             if source.is_dir():
                 shutil.copytree(source, self.location)
             else:
                 self.location.parent.mkdir(parents=True, exist_ok=True)
                 shutil.copyfile(source, self.location)
         await self.load()
 
+    def __iter__(self):
+        """Iterate over assets."""
+        return self.iter()
+
+    def __repr__(self):
+        """Get a string representation."""
+        return f"{self.path} <{self.__class__.__module__}.{self.__class__.__name__}>"
+
 
 class FileAsset(Asset):
     """A file asset."""
 
     @property
     def synced(self) -> bool:
         """True when the storage existence is in sync with the content."""
@@ -216,38 +239,43 @@
     def supports_path(cls, path: str, is_dir: bool = False) -> bool:
         """Check whether this asset class can load the given class."""
         return is_dir and super().supports_path(path, is_dir=is_dir)
 
     def iter_locations(
         self,
         /,
-        relative_to: Optional[AssetLocation | str] = None,
+        relative_to: AssetLocation | str | None = None,
         exclude_empty=False,
         include_dir=False,
         **kwargs,
     ):
         """Iterate the paths for the assets."""
         if include_dir:
             yield from super().iter_locations(
                 relative_to=relative_to, exclude_empty=exclude_empty, **kwargs
             )
 
     def iter(
         self,
         /,
-        asset_type: Optional[type[A]] = None,
-        path_pattern: Optional[str] = None,
+        asset_type: type[A] | None = None,
+        path_includes: PathFilter = None,
+        path_excludes: PathFilter = None,
         exclude_empty=False,
         include_dir=False,
         **kwargs,
     ) -> Iterator[A]:
         """Iterate the assets."""
         if include_dir:
             yield from super().iter(
-                asset_type, path_pattern, exclude_empty=exclude_empty, **kwargs
+                asset_type,
+                path_includes=path_includes,
+                path_excludes=path_excludes,
+                exclude_empty=exclude_empty,
+                **kwargs,
             )
 
 
 AssetType = type[Asset]
 
 
 class PlainFileAsset(FileAsset):
@@ -260,23 +288,22 @@
 
 class AssetsFolder(DirAsset):
     """A container of assets in a separate folder."""
 
     DEFAULT_ASSET_CLASSES: list[AssetType] = []
     DEFAULT_FILE_ASSET_CLASS = PlainFileAsset
     DEFAULT_DIR_ASSET_CLASS = PlainDirAsset
-    PATH_PATTERNS = ["*"]
 
     children: list[Asset]
     asset_classes: list[AssetType]
 
     def __init__(
         self,
         parent: "AssetsFolder",
-        asset_classes: Optional[list[AssetType]] = None,
+        asset_classes: list[AssetType] | None = None,
         **kwargs,
     ):
         """Create an assets directory."""
         is_dir = kwargs.pop("is_dir", True)
         super().__init__(parent, is_dir=is_dir, **kwargs)
         self.asset_classes = list(asset_classes or self.DEFAULT_ASSET_CLASSES)
         self.children = []
@@ -285,30 +312,30 @@
     def full_path(self) -> str:
         """Full path in an assets archive."""
         return self.parent.full_path + self.path + "/"
 
     def add(
         self,
         child_class: type[A],
-        path: Optional[str] = None,
+        path: str | None = None,
         is_dir: bool = False,
         **kwargs,
     ) -> A:
         """Add (or get) child asset."""
-        child = self.get(asset_type=child_class, path_pattern=path, is_dir=is_dir)
+        child = self.get(asset_type=child_class, path_includes=path, is_dir=is_dir)
         if not child:
             child = child_class(self, path=path, is_dir=is_dir, **kwargs)
             self.children.append(child)
         return child
 
     async def add_from(
         self,
         child_class: type[A],
         source: AssetSource,
-        path: Optional[str] = None,
+        path: str | None = None,
         **kwargs,
     ) -> A:
         """Add a child asset from an external location."""
         is_dir = False
         if isinstance(source, Path):
             is_dir = source.is_dir()
             path = path or source.name
@@ -331,31 +358,29 @@
             await child_asset.add_from_dir(source, recursive=True)
         else:
             await child_asset.load_from(source)
         return child_asset
 
     def asset_class_for(
         self, path: str, *asset_classes: AssetType, is_dir: bool = False
-    ) -> type[Asset]:
+    ) -> type[Asset] | None:
         """Get the asset class for the given path."""
         for asset_class in list(asset_classes) or self.asset_classes:
             if asset_class.supports_path(path, is_dir=is_dir):
                 return asset_class
-        raise TypeError(f"No supported asset class found for {path}")
+        return None
 
     async def save(self, **kwargs) -> Self:
         """Save the current assets when accessed."""
         await super().save(**kwargs)
         for child in self.children:
             await child.save(**kwargs)
         return self
 
-    async def save_archive(
-        self, target: Optional[AssetLocation | str] = None, **_kwargs
-    ):
+    async def save_archive(self, target: AssetLocation | str | None = None, **_kwargs):
         """Create a compressed tar archive.
 
         By default as a file in the parent folder."""
         await self.save()
         path = self.location.absolute().name
         target = Path(target or self.location.parent.joinpath(f"{path}.tar.gz"))
         with tarfile.open(target, "w:gz") as tar:
@@ -371,15 +396,15 @@
             self.location, *asset_classes, recursive=recursive, **kwargs
         )
 
     async def load_from(
         self,
         source: AssetSource,
         *asset_classes: AssetType,
-        path: Optional[str] = None,
+        path: str | None = None,
         **kwargs,
     ) -> Self:
         """Load an asset from an external location."""
         is_dir = False
         if isinstance(source, Path):
             is_dir = source.is_dir()
             path = path or source.name
@@ -391,90 +416,96 @@
             )
         _asset_classes = asset_classes or [
             *self.asset_classes,
             self.DEFAULT_DIR_ASSET_CLASS,
             self.DEFAULT_FILE_ASSET_CLASS,
         ]
         asset_class = self.asset_class_for(path, *_asset_classes, is_dir=is_dir)
+        if asset_class is None:
+            raise TypeError(f"No supported asset class found for {path}")
         asset = await self.add_from(asset_class, source, path, **kwargs)
         await asset.load()
         return self
 
     async def load_from_dir(
         self,
         from_location: AssetLocation,
         *asset_classes: type["Asset"],
+        path_includes: PathFilter = None,
+        path_excludes: PathFilter = None,
         recursive=True,
-        path_pattern: Optional[str] = None,
         **kwargs,
     ) -> Self:
         """Discover and load assets from an external location."""
         _asset_classes = asset_classes or self.asset_classes
         await self.add_from_dir(
             from_location,
             *_asset_classes,
             recursive=recursive,
-            path_pattern=path_pattern,
+            path_includes=path_includes,
+            path_excludes=path_excludes,
             **kwargs,
         )
         for child in self.children:
             await child.load()
         return self
 
     async def add_from_dir(
         self,
         from_location: AssetLocation,
         *asset_classes: type["Asset"],
         recursive=True,
-        path_pattern: Optional[str] = None,
         path_prefix: str = "",
+        path_includes: PathFilter = None,
+        path_excludes: PathFilter = None,
         **kwargs,
     ) -> Self:
         """Copy asset(s) (without loading) from an other location."""
         target_location = self.location / path_prefix
         target_location.mkdir(parents=True, exist_ok=True)
         if not from_location.exists():
             raise _err.not_found(from_location)
         if not from_location.is_dir():
             raise _err.not_dir(from_location)
         _asset_classes = asset_classes or self.asset_classes
         for child_location in from_location.iterdir():
             child_path = child_location.relative_to(from_location)
             target_path = f"{path_prefix}{child_path}"
-            path_matches = path_pattern is None or fnmatch.fnmatch(
-                child_location.name, path_pattern
-            )
             asset_class = self.asset_class_for(
                 target_path,
                 *_asset_classes,
                 self.DEFAULT_DIR_ASSET_CLASS,
                 self.DEFAULT_FILE_ASSET_CLASS,
                 is_dir=child_location.is_dir(),
             )
             if asset_class == self.DEFAULT_DIR_ASSET_CLASS and recursive:
                 await self.add_from_dir(
                     child_location,
                     *_asset_classes,
                     recursive=recursive,
                     path_prefix=f"{path_prefix}{child_location.name}/",
-                    path_pattern=path_pattern,
+                    path_includes=path_includes,
+                    path_excludes=path_excludes,
                     **kwargs,
                 )
-            elif path_matches:
+                continue
+            if asset_class is not None and asset_class._path_matches(
+                child_location.name, path_includes, path_excludes
+            ):
                 await self.add_from(asset_class, child_location, target_path, **kwargs)
         return self
 
     def is_empty(self):
         """Check that no child asset are present."""
         return all(child.is_empty() for child in self.children)
 
     def iter_locations(
         self,
         /,
-        relative_to: Optional[AssetLocation | str] = None,
+        relative_to: AssetLocation | str | None = None,
         exclude_empty=False,
         include_dir=False,
         recursive=True,
         **kwargs,
     ) -> Iterator[AssetLocation]:
         """List the asset locations."""
         relative_to = relative_to or self.location
@@ -495,53 +526,58 @@
                     recursive=recursive,
                     **kwargs,
                 )
 
     def iter(
         self,
         /,
-        asset_type: Optional[type[A]] = Asset,
-        path_pattern: Optional[str] = None,
+        asset_type: type[A] | None = Asset,
+        path_includes: PathFilter = None,
+        path_excludes: PathFilter = None,
         exclude_empty=False,
         include_dir=False,
         recursive=True,
         **kwargs,
     ) -> Iterator[A]:
         """List the assets."""
         if exclude_empty and self.is_empty():
             return
         yield from super().iter(
             asset_type=asset_type,
             include_dir=include_dir,
             exclude_empty=exclude_empty,
-            path_pattern=path_pattern,
+            path_includes=path_includes,
+            path_excludes=path_excludes,
             **kwargs,
         )
         if recursive:
             for child in self.children:
                 yield from child.iter(
                     asset_type=asset_type,
                     include_dir=include_dir,
                     exclude_empty=exclude_empty,
-                    path_pattern=path_pattern,
+                    path_includes=path_includes,
+                    path_excludes=path_excludes,
                     recursive=recursive,
                     **kwargs,
                 )
 
     def get(
         self,
         asset_type: type[A],
-        path_pattern: Optional[str] = None,
+        path_includes: PathFilter = None,
+        path_excludes: PathFilter = None,
         recursive=True,
         **kwargs,
-    ) -> Optional[A]:
+    ) -> A | None:
         """Get the asset of the given type, if it exists."""
         asset_it = self.iter(
             asset_type=asset_type,
-            path_pattern=path_pattern,
+            path_includes=path_includes,
+            path_excludes=path_excludes,
             recursive=recursive,
             include_dir=True,
             **kwargs,
         )
         asset = next(asset_it, None)
         if asset is None:
             return None
@@ -551,16 +587,28 @@
                 f"Multiple assets of type {asset_type} found:" f" {[asset, asset_2]}"
             )
         return asset
 
     def get_or_fail(
         self,
         asset_type: type[A],
-        path_pattern: Optional[str] = None,
+        path_includes: PathFilter = None,
+        path_excludes: PathFilter = None,
         recursive=True,
         **kwargs,
     ) -> A:
         """Get the asset of the given type, fail if it not exists."""
-        asset = self.get(asset_type, path_pattern, recursive, **kwargs)
+        asset = self.get(asset_type, path_includes, path_excludes, recursive, **kwargs)
         if asset is None:
-            raise _err.not_found(path_pattern)
+            raise _err.not_found(path_includes)
         return asset
+
+
+def _matches(path: str, patterns: str | list[str] | None, default_patterns: list[str]):
+    patterns = (
+        default_patterns
+        if patterns is None
+        else [patterns]
+        if isinstance(patterns, str)
+        else patterns
+    )
+    return any(fnmatch.fnmatch(path, pattern) for pattern in patterns)
```

### Comparing `waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/cached.py` & `waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/cached.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Assets that have a local edit cache."""
 
 import abc
-from typing import Generic, Optional, TypeVar
+from typing import Generic, TypeVar
 
 from . import _err
 from .base import FileAsset
 
 C = TypeVar("C")
 
 
 class CachedFileAsset(FileAsset, abc.ABC, Generic[C]):
     """Accessor to a file with local caching."""
 
-    content: Optional[C] = None
+    content: C | None = None
 
     def has_content(self) -> bool:
         """Check that cached content is not empty."""
         return self.content is not None
 
     def get_or_fail(self) -> C:
         """Get the content or fail if not set."""
```

### Comparing `waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/default.v1.plug.json` & `waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/default.v1.plug.json`

 * *Files identical despite different names*

### Comparing `waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/default.v2.plug.json` & `waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/default.v2.plug.json`

 * *Files identical despite different names*

### Comparing `waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/json.py` & `waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/json.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .cached import C, CachedFileAsset
 
 
 class JsonAsset(CachedFileAsset[C], Generic[C]):
     """An asset that loads json content."""
 
     JSON_INDENT = 2
-    PATH_PATTERNS: list[str] = ["*.json"]
+    PATH_INCLUDES: list[str] = ["*.json"]
 
     @property
     def json(self) -> C:
         """The cached json-serializable content."""
         # None can be valid (`null` as json)
         return cast(C, self.content)
```

### Comparing `waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/manifest.py` & `waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/manifest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Utility functions for accessing a function manifest."""
 
 import json
+from collections.abc import Callable
 from pathlib import Path
-from typing import Any, Literal, Optional, Self, Union
+from typing import Any, Literal, Self, Union
 
 from .base import AssetsFolder
 from .cached import CachedFileAsset
 from .json import JsonAsset
 from .mixin import WithAssets
 from .python import PythonRequirementsAsset
 
@@ -35,21 +36,21 @@
 
 FunctionType = Literal["webscript"] | Literal["plug"]
 
 
 class FunctionManifestAsset(JsonAsset):
     """An asset that represents a function manifest."""
 
-    PATH_PATTERNS = []
+    PATH_INCLUDES = []
     DEFAULT_MANIFEST: ManifestSpec = {"version": "0.0.1"}
     FUNCTION_TYPE: FunctionType
     MERGE_SPEC: ManifestMergeSpec = {}
 
     def __init__(
-        self, parent: AssetsFolder, manifest: Optional[ManifestSpec] = None, **kwargs
+        self, parent: AssetsFolder, manifest: ManifestSpec | None = None, **kwargs
     ):
         """Create the function manifest asset."""
         super().__init__(parent, **kwargs)
         manifest = manifest or {**self.DEFAULT_MANIFEST}
         self.json = manifest
 
     def merge(self, manifest: ManifestSpec) -> ManifestSpec:
@@ -70,70 +71,85 @@
 
 
 class WebscriptManifestAsset(FunctionManifestAsset):
     """An asset that represents the webscript manifest."""
 
     FUNCTION_TYPE = "webscript"
     DEFAULT_PATH = WEBSCRIPT_MANIFEST_NAME
-    PATH_PATTERNS = [DEFAULT_PATH]
+    PATH_INCLUDES = [DEFAULT_PATH]
 
 
 class PlugManifestAsset(FunctionManifestAsset):
     """An asset that represents the webscript manifest."""
 
     FUNCTION_TYPE = "plug"
     DEFAULT_PATH = PLUG_MANIFEST_NAME
-    PATH_PATTERNS = [DEFAULT_PATH]
+    PATH_INCLUDES = [DEFAULT_PATH]
     MERGE_SPEC: ManifestMergeSpec = PLUG_MERGE_SPEC
 
 
-NO_SCRIPT = """
+def no_script(adapter: type, **kwargs):
+    """Produce a placeholder script."""
+    return """
 # Script not provided, please use the correct ML Adapter.
 """
 
 
 class WithManifest(WithAssets):
-    """Mixin for a configuration that has a waylay function manifest."""
+    """Mixin for a configuration that has a waylay _function_ manifest file and script.
+
+    Adds methods to a `WithAssets` adapter to manage the function _manifest_ of
+    waylay _plugin_ or _webscript_.
+
+    * `manifest` returns the manifest asset of the function archive
+        at `plug.json` or `webscript.json`.
+    * `as_webscript()` initializes the manifest
+        and script for a _webscript_ that uses an ML Adapter.
+    * `as_plug()` initializes the manifest and script for
+        a rule _plugin_ that uses an ML Adapter.
+    """
 
     MANIFEST_ASSET_CLASSES = [WebscriptManifestAsset, PlugManifestAsset]
     DEFAULT_MANIFEST_CLASS = WebscriptManifestAsset
     DEFAULT_REQUIREMENTS = ["starlette"]
-    DEFAULT_SCRIPT: dict[FunctionType, str] = {
-        "webscript": NO_SCRIPT,
-        "plug": NO_SCRIPT,
+    DEFAULT_SCRIPT: dict[FunctionType, Callable] = {
+        "webscript": no_script,
+        "plug": no_script,
     }
     DEFAULT_MANIFEST: dict[FunctionType, ManifestSpec] = {
         "webscript": DEFAULT_WEBSCRIPT_MANIFEST_V1,
         "plug": DEFAULT_PLUG_MANIFEST_V1,
     }
 
-    def default_script(self, function_type: FunctionType = "plug") -> str:
+    def default_script(self, function_type: FunctionType = "plug") -> Callable:
         """Get a default main.py script for a webscript."""
         return self.DEFAULT_SCRIPT[function_type]
 
     def default_requirements(self) -> list[str]:
         """Get the default requirements for this archive."""
         return self.DEFAULT_REQUIREMENTS
 
     def default_manifest(self, function_type: FunctionType = "plug") -> ManifestSpec:
         """Get a default manifest for this archive."""
         return self.DEFAULT_MANIFEST[function_type]
 
     def __init__(
         self,
-        manifest_path: Optional[str] = None,
-        manifest: Optional[ManifestSpec] = None,
+        manifest_path: str | None = None,
+        manifest: ManifestSpec | None = None,
         **kwargs,
     ):
         """Register the manifest asset classes."""
         super().__init__(**kwargs)
         self.assets.asset_classes.extend(self.MANIFEST_ASSET_CLASSES)
         asset_class = WebscriptManifestAsset
         if manifest_path:
-            asset_class = self.assets.asset_class_for(manifest_path, is_dir=False)
+            asset_class = (
+                self.assets.asset_class_for(manifest_path, is_dir=False) or asset_class
+            )
         self.assets.add(asset_class, manifest_path, manifest=manifest, **kwargs)
 
     @property
     def manifest(self) -> FunctionManifestAsset:
         """The manifest of the function that uses this adapter."""
         return self.assets.get_or_fail(asset_type=FunctionManifestAsset)
 
@@ -153,16 +169,27 @@
             if function_type == "webscript"
             else PlugManifestAsset
         )
         manifest_asset.merge(self.default_manifest(function_type))
         manifest_asset.merge(manifest)
         # default script (no not overwrite existing script)
         script_asset = self.assets.get_or_fail(CachedFileAsset, "main.py")
+        model_path = None
+        model_class = None
+        from ..model import WithModel
+
+        if isinstance(self, WithModel):
+            model_path = self.model_path
+            model_class = self.model_class
         if not script_asset.content:
-            script_asset.content = self.default_script(function_type)
+            script_asset.content = self.default_script(function_type)(
+                self.__class__,
+                model_path=model_path,
+                model_class=model_class,
+            )
         # update default requirements (do not overwrite existing deps)
         requirements_asset = self.assets.get_or_fail(PythonRequirementsAsset)
         requirements_asset.add_default(*self.default_requirements())
         return self
 
     def as_webscript(self, manifest: ManifestSpec, **_kwargs) -> Self:
         """Make sure a webscript manifest is present."""
@@ -170,32 +197,37 @@
 
     def as_plug(self, manifest: ManifestSpec, **_kwargs) -> Self:
         """Make sure that a plug manifest is present."""
         return self._as_function(manifest, "plug")
 
 
 def default_webscript_script(
-    adapter_module, adapter_class, model_location="model.dill"
+    adapter_class: type, model_path=None, model_class=None
 ) -> str:
     """Get a default model loading script for webscripts."""
+    adapter_fqn = f"{adapter_class.__module__}.{adapter_class.__name__}"
+    model_class_ref = (
+        f"'{model_class.__module__}.{model_class.__name__}'" if model_class else "None"
+    )
+    model_path_ref = f"'{model_path}'" if model_path else "None"
     return f"""
-# {adapter_module}.{adapter_class} model adapter
+# {adapter_fqn} model adapter
 import os
 from starlette.requests import Request
 from starlette.responses import JSONResponse
 from starlette.exceptions import HTTPException
-from {adapter_module} import {adapter_class}
+from {adapter_class.__module__} import {adapter_class.__name__}
 
-MODEL_LOCATION = os.environ.get('MODEL_LOCATION', '{model_location}')
-MODEL_CLASS = os.environ.get('MODEL_CLASS', None)
+MODEL_PATH = os.environ.get('MODEL_PATH', {model_path_ref})
+MODEL_CLASS = os.environ.get('MODEL_CLASS', {model_class_ref})
 
 # Initialize the model adapter.
 # Provide a `model` argument if you want to create/load the model yourself.
-adapter = {adapter_class}(
-    model_location=MODEL_LOCATION, model_class=MODEL_CLASS
+adapter = {adapter_class.__name__}(
+    model_path=MODEL_PATH, model_class=MODEL_CLASS
 )
 
 # Webscript handler
 async def execute(request: Request):
     if request.method == 'GET':
         return JSONResponse(adapter.openapi)
     if request.method != 'POST':
@@ -208,40 +240,45 @@
     # call the model adapter using the V1
     response_json = await adapter.call(request_json)
     return JSONResponse(response_json)
 """
 
 
 def default_plug_v1_script(
-    adapter_module,
-    adapter_class,
-    model_location="model.dill",
+    adapter_class: type,
+    model_path: str | None = None,
+    model_class: type | None = None,
     state_ok="PREDICTED",
     state_nok="FAILED",
 ) -> str:
     """Get a default model loading script for plugs."""
+    adapter_fqn = f"{adapter_class.__module__}.{adapter_class.__name__}"
+    model_class_ref = (
+        f"'{model_class.__module__}.{model_class.__name__}'" if model_class else "None"
+    )
+    model_path_ref = f"'{model_path}'" if model_path else "None"
     return f"""
-# {adapter_module}.{adapter_class} model adapter
+# {adapter_fqn} model adapter
 import os
 from ml_adapter.api.data import v1 as V1
-from {adapter_module} import {adapter_class}
+from {adapter_class.__module__} import {adapter_class.__name__}
 
 # optional type alias for plug response
 StatusAndRawData = tuple[str, V1.V1PredictionResponse|V1.V1ErrorResponse]
 
 STATE_OK = '{state_ok}'
 STATE_NOK = '{state_nok}'
 
-MODEL_LOCATION = os.environ.get('MODEL_LOCATION', '{model_location}')
-MODEL_CLASS = os.environ.get('MODEL_CLASS', None)
+MODEL_PATH = os.environ.get('MODEL_PATH', {model_path_ref})
+MODEL_CLASS = os.environ.get('MODEL_CLASS', {model_class_ref})
 
 # Initialize the model adapter.
 # Provide a `model` argument if you want to create/load the model yourself.
-adapter = {adapter_class}(
-    model_location=MODEL_LOCATION, model_class=MODEL_CLASS
+adapter = {adapter_class.__name__}(
+    model_path=MODEL_PATH, model_class=MODEL_CLASS
 )
 
 async def execute(properties: V1.V1Request, console, logger) -> StatusAndRawData:
     try:
         result = await adapter.call(properties)
         return (STATE_OK, result)
     except Exception as err:
```

### Comparing `waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/mixin.py` & `waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/root.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,29 @@
-"""ML Adapter mixing providing access to assets."""
-
-from typing import Optional, Self
+"""Asset folder and root asset folder."""
 
 from ml_adapter.api.types import AssetLocation, as_location
 
-from .base import Asset
-from .root import AssetsRoot
-
+from .base import AssetsFolder
 
-class WithAssets:
-    """Mixin for a configuration backed by assets."""
 
-    assets: AssetsRoot
+class AssetsRoot(AssetsFolder):
+    """Root of the assets storage."""
 
-    def __init__(self, location: Optional[AssetLocation | str] = None, **kwargs):
-        """Create assets support."""
-        self.assets = AssetsRoot(location=as_location(location), **kwargs)
-
-    async def save(self, **kwargs) -> Self:
-        """Save the current assets when accessed."""
-        await self.assets.save(**kwargs)
-        return self
-
-    async def load(self, *asset_classes: type["Asset"], **kwargs) -> Self:
-        """Load all assets."""
-        await self.assets.load(*asset_classes, **kwargs)
-        return self
-
-    async def save_archive(
-        self, target: Optional[AssetLocation | str] = None, **kwargs
-    ) -> AssetLocation:
-        """Save the archive."""
-        return await self.assets.save_archive(target, **kwargs)
+    _location: AssetLocation
 
     @property
     def location(self) -> AssetLocation:
-        """Return the location of the stored assets."""
-        return self.assets.location
+        """Path of asset(s)."""
+        return self._location
+
+    @property
+    def full_path(self) -> str:
+        """Full path in an assets archive."""
+        return ""
+
+    def __init__(self, location: AssetLocation | str = ".", **kwargs):
+        """Create an assets root."""
+        super().__init__(parent=self, path=".", **kwargs)
+        location = as_location(location)
+        if location.exists() and not location.is_dir():
+            location = location.parent
+        self._location = location
```

### Comparing `waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/openapi.py` & `waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/openapi.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Utilities for the openapi description of the adapter."""
 
-from typing import Any, Optional
+from typing import Any
 
 import openapi_spec_validator
 from jsonschema.protocols import Validator
 from jsonschema_path import SchemaPath
 from ml_adapter.api.types import AssetLocation
 from openapi_schema_validator import OAS31Validator
 from openapi_spec_validator.validation.validators import SpecValidator
@@ -16,26 +16,26 @@
 SchemaSpec = bool | dict
 OpenapiSpec = dict
 
 
 class SchemaAsset(JsonAsset[SchemaSpec]):
     """The assets containing the json spec."""
 
-    PATH_PATTERNS = ["*.schema.json"]
+    PATH_INCLUDES = ["*.schema.json"]
     SCHEMA_VALIDATOR: Validator = OAS31Validator
 
     @property
-    def schema(self) -> Optional[SchemaSpec]:
+    def schema(self) -> SchemaSpec | None:
         """Get and validate the schema spec."""
         if self.json is None:
             return None
         return self.validate_schema(self.json)
 
     @schema.setter
-    def schema(self, schema: Optional[SchemaSpec] | AssetLocation):
+    def schema(self, schema: SchemaSpec | None | AssetLocation):
         """Validate and set schema definition."""
         if isinstance(schema, AssetLocation):
             schema = SchemaPath.from_file_path(schema).content()
         if schema is not None:
             schema = self.validate_schema(schema)
         self.json = schema
 
@@ -49,15 +49,15 @@
         self.json = self.validate_schema(self.content)
         return await super().save_content(**kwargs)
 
 
 class OpenApiAsset(SchemaAsset):
     """Asset for an openapi specification."""
 
-    PATH_PATTERNS = ["*openapi.json"]
+    PATH_INCLUDES = ["*openapi.json"]
     DEFAULT_PATH = "openapi.json"
 
     OPENAPI_VALIDATOR: SpecValidator = openapi_spec_validator
 
     def validate_schema(self, schema: dict) -> dict:
         """Validate the schema."""
         schema = self.update_with_manifest(schema)
@@ -72,15 +72,22 @@
         manifest = manifest_asset.json
         if not manifest:
             return schema
         return _update_openapi_with_manifest(schema, manifest)
 
 
 class WithOpenapi(WithAssets):
-    """Mixin for a configuration that has an openapi description."""
+    """Mixin for a configuration that has an openapi description.
+
+    Adds methods to a `WithAssets` adapter to manage the
+    openapi description of waylay _plugin_ or _webscript_.
+
+    * `openapi` returns an asset of type `OpenApiAsset` (normally at `openapi.json`)
+
+    """
 
     def __init__(self, **kwargs):
         """Register the openapi asset classes."""
         super().__init__(**kwargs)
         self.assets.asset_classes.extend([OpenApiAsset, SchemaAsset])
         self.assets.add(OpenApiAsset)
```

### Comparing `waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/assets/python.py` & `waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/assets/python.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Python dependencies as a function asset."""
 
 import re
 from collections import namedtuple
 from collections.abc import Iterator, Mapping
-from typing import Optional
+from pathlib import Path
 
 from .base import AssetsFolder, AssetSource, FileAsset
 from .cached import CachedFileAsset, RequiredCachedFileAsset
 from .mixin import WithAssets
 
 
 class PythonRequirementsAsset(RequiredCachedFileAsset[list[str]]):
     """The python requirements.txt."""
 
-    PATH_PATTERNS = ["requirements.txt"]
+    PATH_INCLUDES = ["requirements.txt"]
     DEFAULT_PATH = "requirements.txt"
 
     def __init__(self, *args, **kwargs):
         """Create a requirements asset, with empty list as default."""
         super().__init__(*args, **kwargs)
         self.content = []
 
@@ -76,21 +76,21 @@
         )
         return self.requirements
 
 
 class PythonLibraryAsset(FileAsset):
     """An installable python library."""
 
-    PATH_PATTERNS = ["*.tar.gz"]
+    PATH_INCLUDES = ["*.tar.gz"]
 
 
 class PythonScriptAsset(CachedFileAsset):
     """A python script."""
 
-    PATH_PATTERNS = ["*.py"]
+    PATH_INCLUDES = ["*.py"]
     DEFAULT_PATH = "main.py"
 
     async def load_content(self, **_kwargs):
         """Cache the content."""
         with open(self.location, encoding="utf-8") as f:
             self.content = "".join(f.readlines())
 
@@ -101,36 +101,43 @@
                 f.write(self.content)
 
 
 class PythonLibAssetDir(AssetsFolder):
     """Default location for packaged libraries."""
 
     DEFAULT_PATH = "lib"
-    PATH_PATTERNS = [DEFAULT_PATH]
+    PATH_INCLUDES = [DEFAULT_PATH]
     DEFAULT_ASSET_CLASSES = [PythonLibraryAsset]
 
     async def add_library(
         self,
         source: AssetSource,
-        path: Optional[str] = None,
-        requirement: Optional[str] = None,
+        path: str | None = None,
+        requirement: str | None = None,
     ):
         """Add a library as a asset and as requirement."""
         library = await self.add_from(PythonLibraryAsset, source, path=path)
         requirements = self.parent.get_or_fail(PythonRequirementsAsset)
         if requirement:
             requirements.add(f"--find-links {library.parent.full_path}")
             requirements.add(requirement)
         else:
             requirements.add(library.full_path)
         return library
 
 
 class WithPython(WithAssets):
-    """Handles requirements.txt, scripts and libraries as function assets."""
+    """Handles assets specific to python-based functions.
+
+    * `requirements` handles the dependency file (at `requirements.txt`)
+    * `lib` handles the libraries that are uploaded with
+       the function archive itself. (at `lib/*.tar.gz`)
+    * `main_script` handles the main script of the function (`main.py`)
+    * `scripts` handles other utility scripts of the function (`*.py`)
+    """
 
     def __init__(self, **kwargs):
         """Register the requirements asset classes."""
         super().__init__(**kwargs)
         self.assets.asset_classes.extend(
             [
                 PythonRequirementsAsset,
@@ -151,24 +158,31 @@
     def lib(self) -> PythonLibAssetDir:
         """The lib dir holding python libraries."""
         return self.assets.get_or_fail(
             PythonLibAssetDir, PythonLibAssetDir.DEFAULT_PATH
         )
 
     async def add_script(
-        self, source: AssetSource, path="main.py"
+        self, source: AssetSource, path: str | None = None
     ) -> PythonScriptAsset:
         """Add a (main) python script."""
+        if path is None:
+            if not isinstance(source, str | Path):
+                raise AttributeError(
+                    "Please specify a `path` when the source is not a filename."
+                )
+            source = Path(source)
+            path = source.name
         return await self.assets.add_from(PythonScriptAsset, source=source, path=path)
 
     async def add_library(
         self,
         source: AssetSource,
-        path: Optional[str] = None,
-        requirement: Optional[str] = None,
+        path: str | None = None,
+        requirement: str | None = None,
     ) -> PythonLibraryAsset:
         """Add a (main) python script."""
         return await self.lib.add_library(
             source=source, path=path, requirement=requirement
         )
 
     @property
```

### Comparing `waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/marshall/base.py` & `waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/marshall/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,72 @@
 """Mapping and validation of remote data to and from model inference."""
 
 import abc
 from abc import ABC
-from typing import Any, Generic, Optional
+from typing import Any, Generic
 
 import ml_adapter.api.types as T
 
 
 class RequestMarshaller(Generic[T.MREQ, T.RREQ], ABC):
     """Base class to marshall inference requests."""
 
     @abc.abstractmethod
     def map_request(self, request: T.RREQ, /, **kwargs) -> T.MREQ:
         """Convert a remote request to an model inference request."""
 
     @abc.abstractmethod
     def encode_request(
-        self, request: T.MREQ, parameters: Optional[T.Parameters] = None, **kwargs
+        self, request: T.MREQ, parameters: T.Parameters | None = None, **kwargs
     ) -> T.RREQ:
         """Convert a model inference request to the remote protocol."""
 
 
 class ResponseMarshaller(Generic[T.MRES, T.RREQ, T.RRES], ABC):
     """Base class to marshall inference responses."""
 
     @abc.abstractmethod
     def map_response(
         self,
         request: T.RREQ,
         response: T.MRES,
-        output_params: Optional[dict[str, Any]] = None,
+        output_params: dict[str, Any] | None = None,
         /,
         **kwargs,
     ) -> T.RRES:
         """Convert a model inference response to the remote protocol."""
 
     @abc.abstractmethod
     def decode_response(
         self, response: T.RRES, /, **kwargs
-    ) -> (T.MRES, Optional[T.Parameters]):
+    ) -> (T.MRES, T.Parameters | None):
         """Decode a remote model inference response."""
 
 
 class Marshaller(
     RequestMarshaller[T.MREQ, T.RREQ],
     ResponseMarshaller[T.MRES, T.RREQ, T.RRES],
     Generic[T.MREQ, T.MRES, T.RREQ, T.RRES],
     ABC,
 ):
-    """Base class to marshall inference requests and responses."""
+    """Abstract base class to marshall inference requests and responses.
+
+    Methods used to invoke the model in a _plugin_ or _webscript_:
+    * `map_request()` maps remote requests (generic type `RREQ`)
+    to native requests (generic type `MREQ`)
+    * `map_response()` maps native responses (generic type `MRES`)
+    to remote a response (generic type `RRES`)
+
+    Methods used to test roundtrip encoding in a client:
+    * `encode_request()` encodes a native request
+    to a remote request that can be sent to a waylay function.
+    * `decode_response()` decodes a remote response from a function
+    to native a response.
+
+    """
 
 
 class NoMarshaller(
     RequestMarshaller[T.MREQ, T.MREQ],
     ResponseMarshaller[T.MRES, T.MREQ, T.MREQ],
     Generic[T.MREQ, T.MRES],
 ):
@@ -66,21 +80,21 @@
         self, request: T.MREQ, parameters: T.Parameters | None = None, **kwargs
     ) -> T.MREQ:
         """Encode a tensor request with default input name."""
         return request
 
     def decode_response(
         self, response: T.MRES, /, **kwargs
-    ) -> (T.MRES, Optional[T.Parameters]):
+    ) -> (T.MRES, T.Parameters | None):
         """Decode the default tensor from a V1 response."""
         return response, {}
 
     def map_response(
         self,
         request: T.MREQ,
         response: T.MRES,
-        output_params: Optional[dict[str, Any]] = None,
+        output_params: dict[str, Any] | None = None,
         /,
         **kwargs,
     ) -> T.MRES:
         """Convert a model inference response to the remote protocol."""
         return response
```

### Comparing `waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/marshall/v1/base.py` & `waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/marshall/v1/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """V1 marshaller base."""
 
 import abc
 from collections import defaultdict
 from collections.abc import Iterable, Mapping
-from typing import Any, Generic, Optional, Union, cast
+from typing import Any, Generic, cast
 
 from ml_adapter.api import types as T
 from ml_adapter.api.data import common as C
 from ml_adapter.api.data import v1 as V1
 
 from ..base import Marshaller, RequestMarshaller, ResponseMarshaller
 
@@ -34,23 +34,23 @@
     SINGLE_MAIN_AS_VALUE = True
     DEFAULT_INPUT_NAME = "main"
     DEFAULT_INPUT_DATA_TYPE = C.DataTypes.DEFAULT
     DEFAULT_OUTPUT_NAME = "main"
     DEFAULT_OUTPUT_DATA_TYPE = C.DataTypes.DEFAULT
 
     def map_decoding_kwargs(
-        self, parameters: Optional[C.Parameters], **kwargs
+        self, parameters: C.Parameters | None, **kwargs
     ) -> Mapping[str, Any]:
         """Extract arguments for mapping V1 requests."""
         if parameters:
             return {**kwargs, **parameters}
         return kwargs
 
     def map_encoding_kwargs(
-        self, parameters: Optional[C.Parameters], **kwargs
+        self, parameters: C.Parameters | None, **kwargs
     ) -> Mapping[str, Any]:
         """Extract arguments for mapping V1 requests."""
         if parameters:
             kwargs = {**kwargs, **parameters}
         return kwargs
 
     def as_single_main_input(self, named_tensors: V1.NamedValues):
@@ -124,16 +124,16 @@
     @abc.abstractmethod
     def encode_as_named(self, request: T.MREQ, **kwargs) -> V1.NamedValues:
         """Encode an inference request as a dict of V1 tensors."""
 
     def encode_request(
         self,
         request: T.MREQ,
-        parameters: Optional[C.Parameters] = None,
-        as_instances: Optional[bool] = None,
+        parameters: C.Parameters | None = None,
+        as_instances: bool | None = None,
         **kwargs,
     ) -> V1.V1Request:
         """Encode a V1 inference request."""
         req: V1.V1Request = {}
         if parameters is not None:
             req["parameters"] = parameters
             kwargs = self.map_encoding_kwargs(parameters, **kwargs)
@@ -170,26 +170,26 @@
 
 class V1ResponseMarshallerBase(
     V1ResponseMarshaller[T.MRES], WithV1Encoding, Generic[T.MRES], abc.ABC
 ):
     """Base Marshaller from/to the V1 protocol."""
 
     def map_response_parameters(
-        self, output_params: Optional[C.Parameters], /, **kwargs
+        self, output_params: C.Parameters | None, /, **kwargs
     ) -> C.Parameters:
         """Extract all request params."""
         if output_params:
             return {**output_params, **kwargs}
         return kwargs
 
     def map_response(
         self,
         request: V1.V1Request,
         response: T.MRES,
-        output_params: Optional[C.Parameters] = None,
+        output_params: C.Parameters | None = None,
         /,
         **kwargs,
     ) -> V1.V1PredictionResponse:
         """Convert a model inference response to the remote protocol."""
         kwargs = self.map_encoding_kwargs(request.get("parameters"), **kwargs)
         kwargs = self.map_encoding_kwargs(output_params, **kwargs)
 
@@ -256,15 +256,15 @@
             return self.decode_named_values(
                 cast(list[V1.NamedValues], response), **kwargs
             )
         return self.decode_response_value(cast(V1.ValueOrTensor, response), **kwargs)
 
     def decode_response(
         self, response: V1.V1PredictionResponse, /, **kwargs
-    ) -> (T.MRES, Optional[T.Parameters]):
+    ) -> (T.MRES, T.Parameters | None):
         """Decode a V1 inference response."""
         response_params = self.decode_response_parameters(
             response.get("parameters"), **kwargs
         )
         kwargs = self.map_decoding_kwargs(response_params, **kwargs)
         if "predictions" in response:
             decoded = self.decode_predictions(response["predictions"], **kwargs)
@@ -272,15 +272,15 @@
             decoded = self.decode_output_response(response["outputs"], **kwargs)
         else:
             decoded = self.decode_empty_response(**kwargs)
 
         return decoded, response_params
 
     def decode_response_parameters(
-        self, parameters: Optional[C.Parameters], **_kwargs
+        self, parameters: C.Parameters | None, **_kwargs
     ) -> T.Parameters:
         """Decode V1 response parameters."""
         return parameters or {}
 
 
 class WithV1TensorEncoding(Generic[T.V], abc.ABC):
     """Provides encoding and decoding of V1 tensors."""
@@ -321,15 +321,15 @@
 
     def encode_as_named(self, request: T.VDict, **kwargs) -> V1.NamedValues:
         """Encode a tensor dict to a v1 dict."""
         return {name: self.encode(value, **kwargs) for name, value in request.items()}
 
 
 class V1ValueOrDictRequestMarshallerBase(
-    V1RequestMarshallerBase[Union[T.V, T.VDict]],
+    V1RequestMarshallerBase[T.V | T.VDict],
     WithV1TensorEncoding[T.V],
     Generic[T.V],
     abc.ABC,
 ):
     """V1 Request Marshaller all requests to a tensor or Dict of tensors."""
 
     def map_named_inputs(self, data: V1.NamedValues, /, **kwargs) -> T.VorDict:
```

### Comparing `waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/marshall/v1/list.py` & `waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/marshall/v1/list.py`

 * *Files identical despite different names*

### Comparing `waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/model/base.py` & `waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/model/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from ..assets import RequiredCachedFileAsset, _err
 
 
 class ModelAsset(RequiredCachedFileAsset[T.MI], Generic[T.MI]):
     """Asset for the ml model storage."""
 
-    PATH_PATTERNS = ["model.*"]
+    PATH_INCLUDES = ["model.*"]
     PATH_SUFFIXES = []
 
     @property
     def model(self) -> T.MI:
         """The model instance."""
         if self.content is None:
             raise _err.not_found(location=self.location)
```

### Comparing `waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/model/dill.py` & `waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/model/dill.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,17 +13,22 @@
     """Load and cache the dill module."""
     import dill as dill_loaded  # pylint:disable=import-outside-toplevel
 
     return dill_loaded
 
 
 class DillModelAsset(ModelAsset[T.MI], Generic[T.MI]):
-    """Model asset for dill-serialized models."""
+    """Model asset for dill-serialized models.
 
-    PATH_PATTERNS = ["model.dill", "model.pkl", "model.pickle"]
+    Reads/writes the model from paths like `model.dill`, `model.pkl`, `model.pickle`
+    using [dill](https://pypi.org/project/dill/) serialisation.
+    """
+
+    PATH_INCLUDES = ["*.dill", "*.pkl", "*.pickle"]
+    DEFAULT_PATH = "model.dill"
 
     async def load_content(self, **kwargs):
         """Load a dill model."""
         with open(self.location, "rb") as f:
             self.content = dill().load(f, **kwargs)  # type: ignore
 
     async def save_content(self, **kwargs):
```

### Comparing `waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/model/joblib.py` & `waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/model/joblib.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,17 +13,21 @@
     """Load and cache the joblib module."""
     import joblib as joblib_loaded  # pylint:disable=import-outside-toplevel
 
     return joblib_loaded
 
 
 class JoblibModelAsset(ModelAsset[T.MI], Generic[T.MI]):
-    """Model asset with joblib serialization."""
+    """Model asset with joblib serialization.
 
-    PATH_PATTERNS = ["model.joblib", "model.joblib.gz"]
+    Reads/writes the model from `model.joblib` or `model.joblib.gz`
+    using [joblib](https://pypi.org/project/joblib/) serialisation.
+    """
+
+    PATH_INCLUDES = ["*.joblib", "*.joblib.gz"]
     DEFAULT_PATH = "model.joblib"
 
     joblib_serialization_defaults = {"compress": ("gzip", 3)}
 
     async def load_content(self, **kwargs):
         """Load joblib a model."""
         with open(self.location, "rb") as f:
```

### Comparing `waylay_ml_adapter_base-0.0.2/src/ml_adapter/base/model/serialize.py` & `waylay_ml_adapter_base-0.0.3/src/ml_adapter/base/model/serialize.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 """Serialization of models with pickling libraries (dill, joblib)."""
 
 import inspect
-from typing import Generic, Optional, TypeVar
+from typing import Generic, TypeVar
 
 import ml_adapter.api.types as T
 
 from ..assets import AssetsFolder
 from .base import ModelAsset
 
 SMI = TypeVar("SMI", bound=T.SerializableModel)
 
 
 class SelfSerializingModelAsset(ModelAsset[SMI], Generic[SMI]):
-    """Model asset with own serialization methods."""
+    """Model asset with own serialization methods.
 
-    PATH_PATTERNS = ["model.sav"]
+    Reads/writes the model from `model.sav` using the `save` and `load` methods
+    defined on the `model_class`.
+    """
+
+    PATH_INCLUDES = ["*.sav"]
     DEFAULT_PATH = "model.sav"
-    MODEL_CLASS: Optional[type[SMI]] = None
+    MODEL_CLASS: type[SMI] | None = None
 
     model_class: type[SMI]
 
     def __init__(
-        self, parent: AssetsFolder, model_class: Optional[type[SMI]] = None, **kwargs
+        self, parent: AssetsFolder, model_class: type[SMI] | None = None, **kwargs
     ):
         """Create a self-serializing model asset."""
         super().__init__(parent, **kwargs)
         model_class = model_class or self.MODEL_CLASS
-        if not model_class:
+        if not isinstance(model_class, type):
             raise TypeError(
                 f'Loading a self-serializing model using "{self.__class__.__name__}"'
                 ' requires a "model_class" argument.'
             )
         self.model_class = model_class
 
     async def load_content(self, **kwargs):
```

### Comparing `waylay_ml_adapter_base-0.0.2/src/waylay_ml_adapter_base.egg-info/SOURCES.txt` & `waylay_ml_adapter_base-0.0.3/src/waylay_ml_adapter_base.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENCE.txt
 README.md
 pyproject.toml
 src/ml_adapter/base/__init__.py
 src/ml_adapter/base/adapter.py
 src/ml_adapter/base/py.typed
 src/ml_adapter/base/assets/__init__.py
 src/ml_adapter/base/assets/_err.py
```

