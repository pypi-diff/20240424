# Comparing `tmp/waylay_ml_adapter_sdk-0.0.2.tar.gz` & `tmp/waylay_ml_adapter_sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_ml_adapter_sdk-0.0.2.tar", last modified: Wed Apr 17 09:14:38 2024, max compression
+gzip compressed data, was "waylay_ml_adapter_sdk-0.0.3.tar", last modified: Wed Apr 24 15:24:08 2024, max compression
```

## Comparing `waylay_ml_adapter_sdk-0.0.2.tar` & `waylay_ml_adapter_sdk-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:38.836890 waylay_ml_adapter_sdk-0.0.2/
--rw-r--r--   0 thomas     (502) staff       (20)      494 2024-04-17 09:14:38.834613 waylay_ml_adapter_sdk-0.0.2/PKG-INFO
--rw-r--r--   0 thomas     (502) staff       (20)       66 2024-04-17 08:27:35.000000 waylay_ml_adapter_sdk-0.0.2/README.md
--rw-r--r--   0 thomas     (502) staff       (20)     1184 2024-04-17 08:27:35.000000 waylay_ml_adapter_sdk-0.0.2/pyproject.toml
--rw-r--r--   0 thomas     (502) staff       (20)       38 2024-04-17 09:14:38.837092 waylay_ml_adapter_sdk-0.0.2/setup.cfg
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:38.803837 waylay_ml_adapter_sdk-0.0.2/src/
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:38.803514 waylay_ml_adapter_sdk-0.0.2/src/ml_adapter/
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:38.813182 waylay_ml_adapter_sdk-0.0.2/src/ml_adapter/sdk/
--rw-r--r--   0 thomas     (502) staff       (20)       86 2024-04-17 08:27:35.000000 waylay_ml_adapter_sdk-0.0.2/src/ml_adapter/sdk/__init__.py
--rw-r--r--   0 thomas     (502) staff       (20)        0 2024-03-13 08:16:25.000000 waylay_ml_adapter_sdk-0.0.2/src/ml_adapter/sdk/py.typed
--rw-r--r--   0 thomas     (502) staff       (20)    12872 2024-04-17 08:27:35.000000 waylay_ml_adapter_sdk-0.0.2/src/ml_adapter/sdk/tool.py
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:38.830738 waylay_ml_adapter_sdk-0.0.2/src/waylay_ml_adapter_sdk.egg-info/
--rw-r--r--   0 thomas     (502) staff       (20)      494 2024-04-17 09:14:38.000000 waylay_ml_adapter_sdk-0.0.2/src/waylay_ml_adapter_sdk.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (502) staff       (20)      406 2024-04-17 09:14:38.000000 waylay_ml_adapter_sdk-0.0.2/src/waylay_ml_adapter_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (502) staff       (20)        1 2024-04-17 09:14:38.000000 waylay_ml_adapter_sdk-0.0.2/src/waylay_ml_adapter_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (502) staff       (20)       54 2024-04-17 09:14:38.000000 waylay_ml_adapter_sdk-0.0.2/src/waylay_ml_adapter_sdk.egg-info/entry_points.txt
--rw-r--r--   0 thomas     (502) staff       (20)      179 2024-04-17 09:14:38.000000 waylay_ml_adapter_sdk-0.0.2/src/waylay_ml_adapter_sdk.egg-info/requires.txt
--rw-r--r--   0 thomas     (502) staff       (20)       11 2024-04-17 09:14:38.000000 waylay_ml_adapter_sdk-0.0.2/src/waylay_ml_adapter_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:24:08.961491 waylay_ml_adapter_sdk-0.0.3/
+-rw-r--r--   0 thomas     (502) staff       (20)      746 2024-04-24 15:21:52.000000 waylay_ml_adapter_sdk-0.0.3/LICENCE.txt
+-rw-r--r--   0 thomas     (502) staff       (20)     2823 2024-04-24 15:24:08.961159 waylay_ml_adapter_sdk-0.0.3/PKG-INFO
+-rw-r--r--   0 thomas     (502) staff       (20)     2249 2024-04-24 11:51:38.000000 waylay_ml_adapter_sdk-0.0.3/README.md
+-rw-r--r--   0 thomas     (502) staff       (20)     1252 2024-04-24 15:21:52.000000 waylay_ml_adapter_sdk-0.0.3/pyproject.toml
+-rw-r--r--   0 thomas     (502) staff       (20)       38 2024-04-24 15:24:08.961536 waylay_ml_adapter_sdk-0.0.3/setup.cfg
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:24:08.954085 waylay_ml_adapter_sdk-0.0.3/src/
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:24:08.953940 waylay_ml_adapter_sdk-0.0.3/src/ml_adapter/
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:24:08.957524 waylay_ml_adapter_sdk-0.0.3/src/ml_adapter/sdk/
+-rw-r--r--   0 thomas     (502) staff       (20)      108 2024-04-22 08:55:37.000000 waylay_ml_adapter_sdk-0.0.3/src/ml_adapter/sdk/__init__.py
+-rw-r--r--   0 thomas     (502) staff       (20)        0 2024-03-13 08:16:25.000000 waylay_ml_adapter_sdk-0.0.3/src/ml_adapter/sdk/py.typed
+-rw-r--r--   0 thomas     (502) staff       (20)    13476 2024-04-24 15:21:52.000000 waylay_ml_adapter_sdk-0.0.3/src/ml_adapter/sdk/tool.py
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:24:08.960671 waylay_ml_adapter_sdk-0.0.3/src/waylay_ml_adapter_sdk.egg-info/
+-rw-r--r--   0 thomas     (502) staff       (20)     2823 2024-04-24 15:24:08.000000 waylay_ml_adapter_sdk-0.0.3/src/waylay_ml_adapter_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (502) staff       (20)      418 2024-04-24 15:24:08.000000 waylay_ml_adapter_sdk-0.0.3/src/waylay_ml_adapter_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (502) staff       (20)        1 2024-04-24 15:24:08.000000 waylay_ml_adapter_sdk-0.0.3/src/waylay_ml_adapter_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (502) staff       (20)       54 2024-04-24 15:24:08.000000 waylay_ml_adapter_sdk-0.0.3/src/waylay_ml_adapter_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 thomas     (502) staff       (20)      167 2024-04-24 15:24:08.000000 waylay_ml_adapter_sdk-0.0.3/src/waylay_ml_adapter_sdk.egg-info/requires.txt
+-rw-r--r--   0 thomas     (502) staff       (20)       11 2024-04-24 15:24:08.000000 waylay_ml_adapter_sdk-0.0.3/src/waylay_ml_adapter_sdk.egg-info/top_level.txt
```

### Comparing `waylay_ml_adapter_sdk-0.0.2/pyproject.toml` & `waylay_ml_adapter_sdk-0.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 
 [tool.setuptools-git-versioning]
 enabled = true
 
 [project]
 name = "waylay-ml-adapter-sdk"
 description = "ML_adapter plugin for waylay-sdk-py."
-requires-python = ">=3.9"
-authors = [{name = "Waylay"}]
+requires-python = ">=3.11"
+authors = [{name = "Waylay", email = "info@waylay.io"}]
+license={file = "LICENSE.txt"}
+readme = "README.md"
 dependencies = [
   "waylay-ml-adapter-base",
-  "waylay-sdk-registry-types==2.13.0b20240415",
-  "waylay-sdk-rules-types==6.5.0.20240415",
+  "waylay-sdk-registry==2.13.0b20240423",
+  "waylay-sdk-rules==6.5.0.20240423",
   "tenacity"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
   "waylay-ml-adapter-base",
@@ -34,15 +36,15 @@
 [project.entry-points.dynamic]
 "waylay_sdk_plugins"= "ml_adapter.sdk:PLUGINS"
 
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 markers = [
-    "exclude_ci: marks tests to exlude for ci (unstable or requires additional config)"
+    "exclude_ci: marks tests to exclude for ci (unstable or requires additional config)"
 ]
 
 [tool.ruff]
 include = ["pyproject.toml", "src/**/*.py", "test/**/*.py"]
 
 [tool.ruff.lint]
 select = ["E", "F", "UP",  "B", "SIM", "I", "D1", "D4"]
```

### Comparing `waylay_ml_adapter_sdk-0.0.2/src/ml_adapter/sdk/tool.py` & `waylay_ml_adapter_sdk-0.0.3/src/ml_adapter/sdk/tool.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,78 @@
 """Service tool for the ml-adapters."""
 
 import contextlib
 import logging
-from collections import namedtuple
 from collections.abc import AsyncIterator
 from functools import cached_property
-from types import SimpleNamespace
-from typing import Optional, TypeVar, Union, cast
+from typing import Any, cast
 
 from ml_adapter.api.data.common import V1_PROTOCOL
 from ml_adapter.base.assets.manifest import ManifestSpec, WithManifest
 from pydantic import TypeAdapter
 from tenacity import retry, stop_after_delay, wait_exponential
 from waylay.sdk import WaylayTool
 from waylay.sdk.exceptions import WaylayError
 from waylay.services.registry.api import PlugsApi, WebscriptsApi
-from waylay.services.registry.models import (
-    EventWithCloseSSE,
-    GetPlugResponseV2,
-    GetWebscriptResponseV2,
-    PostPlugJobAsyncResponseV2,
-    PostPlugJobSyncResponseV2,
-    PostWebscriptJobAsyncResponseV2,
-    PostWebscriptJobSyncResponseV2,
-)
-from waylay.services.registry.service.service import RegistryService
-from waylay.services.rules.service.service import RulesService
-
-WebscriptResponse = Union[
-    PostWebscriptJobAsyncResponseV2,
-    PostWebscriptJobSyncResponseV2,
-    GetWebscriptResponseV2,
-]
-
-T = TypeVar("T")
+from waylay.services.registry.service import RegistryService
+from waylay.services.rules.service import RulesService
 
 LOG = logging.getLogger(__name__)
 
+# unlimited read timeout
 STREAM_TIMEOUTS = (5.0, None, 5.0, 5.0)
 
-FunctionResponse = GetWebscriptResponseV2 | GetPlugResponseV2
-JobResponse = (
-    PostWebscriptJobAsyncResponseV2 | PostPlugJobAsyncResponseV2 | FunctionResponse
-)
-CreateResponse = (
-    PostWebscriptJobAsyncResponseV2
-    | PostWebscriptJobSyncResponseV2
-    | PostPlugJobAsyncResponseV2
-    | PostPlugJobSyncResponseV2
-)
 
-_FunctionRef = namedtuple("FunctionRef", ["name", "version"])
+class MLTool(WaylayTool):
+    """MLAdapter utility service for the waylay client.
 
+    Helps creating waylay webscripts and plugs that wrap a machine learning model.
 
-class MLTool(WaylayTool):
-    """MLAdapter utility service for the waylay client."""
+    Loaded as tool with name `ml_tool` in the python sdk.
+
+    #### Example
+    ```python
+    # create and test a simple model
+    import numpy as np
+    test_data = [1,2,3]
+    expected_result = [2,4,6]
+    doubler = lambda x: x*2
+    assert np.array_equal(
+        np.array(expected_result),
+        doubler(np.array(test_data))
+    )
+
+    # wrap in an adapter, test remoting
+    from ml_adapter.numpy import V1NumpyModelAdapter
+    adapter=V1NumpyModelAdapter(model=doubler)
+    test_resp == await adapter.call({"instances": test_data.tolist()})
+    assert test_resp['predictions'] = expected_result.tolist()
+
+    # use the ml_tool to deploy and test a webscript
+    # configure logging to see what is happening
+    import logging
+    logging.basicConfig(level='INFO')
+    from waylay.sdk import WaylayClient
+    client = WaylayClient.from_profile('demo')
+
+    ref = await client.ml_tool.create_webscript(
+        adapter, name='MyMLWebscript', draft=True
+    )
+    ref = await client.ml_tool.wait_until_ready(ref)
+    result = await client.ml_tool.test_webscript(ref, test_data)
+    if expected_result.to_list() == result:
+        await client.ml_tool.publish(ref)
+    else:
+        await client.ml_tool.remove(ref)
+    ```
+    """
 
     name = "ml_tool"
     title: str = "ML Adapter Tool"
-    description: Optional[str] = """
+    description: str | None = """
 Helps creating waylay webscripts and plugs that wrap a machine learning model.
 """
 
     @cached_property
     def registry(self) -> RegistryService:
         """Get the registry SDK."""
         return self._services.require(RegistryService)
@@ -81,29 +91,29 @@
     def plugs(self) -> PlugsApi:
         """Get the registry SDK."""
         return self.registry.plugs
 
     async def python_runtimes(self):
         """Check registry version."""
         resp = await self.registry.runtimes.list(
-            query={"archive_format": ["python"]}, select_path=""
+            query={"archiveFormat": ["python"]}, response_type=Any
         )
-        return SimpleNamespace(**{r.function_type: r for r in resp.runtimes})
+        return {r["functionType"]: r for r in resp["runtimes"]}
 
     async def create_webscript(
         self,
         adapter: WithManifest,
-        manifest: Optional[ManifestSpec] = None,
-        name: Optional[str] = None,
-        version: Optional[str] = None,
-        runtime: Optional[str] = None,
+        manifest: ManifestSpec | None = None,
+        name: str | None = None,
+        version: str | None = None,
+        runtime: str | None = None,
         comment: str = "",
         draft: bool = False,
         var_async: bool = True,
-    ) -> PostWebscriptJobAsyncResponseV2 | PostWebscriptJobSyncResponseV2:
+    ):
         """Create a webscript function from the given ml adapter."""
         manifest = manifest or {}
         if name:
             manifest = {**manifest, "name": name}
         if version:
             manifest = {**manifest, "version": version}
         if runtime:
@@ -119,54 +129,54 @@
                     include_dir=False,
                     exclude_empty=True,
                 )
             }
             result = await self.webscripts.create(
                 files=files,
                 query={"draft": draft, "comment": comment, "async": var_async},
-                select_path="",
+                response_type=Any,
             )
         return result
 
     async def create_plug(
         self,
         adapter: WithManifest,
-        manifest: Optional[ManifestSpec] = None,
-        states: Optional[list] = None,
-        inputs: Optional[dict] = None,
-        outputs: Optional[dict] = None,
-        name: Optional[str] = None,
-        version: Optional[str] = None,
-        runtime: Optional[str] = None,
+        manifest: ManifestSpec | None = None,
+        states: list | None = None,
+        inputs: dict | None = None,
+        outputs: dict | None = None,
+        name: str | None = None,
+        version: str | None = None,
+        runtime: str | None = None,
         comment: str = "",
         draft: bool = False,
         var_async: bool = True,
-    ) -> PostPlugJobAsyncResponseV2 | PostPlugJobSyncResponseV2:
+    ):
         """Create a plug function from the given ml adapter."""
         manifest = manifest or {}
         if name:
             manifest = {**manifest, "name": name}
         if version:
             manifest = {**manifest, "version": version}
         if runtime:
             manifest = {**manifest, "runtime": runtime}
         interface = manifest.get("interface") or {}
         interface_doc = manifest.get("metadata", {}).get("interface", {})
         if states:
             interface["states"] = states
             manifest["interface"] = interface
-            del interface_doc["states"]
+            interface_doc.pop("states", None)
         if inputs:
             interface["inputs"] = inputs
             manifest["interface"] = interface
-            del interface_doc["inputs"]
+            interface_doc.pop("inputs", None)
         if outputs:
             interface["outputs"] = outputs
             manifest["interface"] = interface
-            del interface_doc["outputs"]
+            interface_doc.pop("outputs", None)
         adapter = adapter.as_plug(manifest)
         await adapter.save()
         with contextlib.ExitStack() as stack:
             # uses ExitStack.enter_context to close files afterwards.
             files = {
                 asset.full_path: stack.enter_context(open(asset.location, "br"))
                 for asset in adapter.assets.iter(
@@ -174,168 +184,188 @@
                     include_dir=False,
                     exclude_empty=True,
                 )
             }
             result = await self.plugs.create(
                 files=files,
                 query={"draft": draft, "comment": comment, "async": var_async},
-                select_path="",
+                response_type=Any,
             )
         return result
 
     async def wait_until_ready(
         self,
-        resp: (CreateResponse | dict),
-        logger: Optional[logging.Logger] = None,
+        resp: dict,
+        logger: logging.Logger | None = None,
         success_states=("running",),
     ):
         """Wait for a webscript to be running."""
-        create_resp: CreateResponse = _as_model(resp, CreateResponse)
-        status = create_resp.entity.status
-        is_webscript = hasattr(create_resp.entity, "webscript")
-        ref = create_resp.entity.webscript if is_webscript else create_resp.entity.plug
+        entity = resp["entity"]
+        status = entity["status"]
+        as_webscript = entity.get("webscript", False)
+        as_plug = entity.get("plug", False)
+        event_href = resp.get("_links", {}).get("event", {}).get("href", None)
+        ref = as_webscript or as_plug
+        name = ref["name"]
+        version = ref["version"]
+        logger = logger or LOG
         if status not in success_states:
-            jobs_resp: JobResponse
-            if isinstance(create_resp, PostPlugJobSyncResponseV2):
-                jobs_resp = await self.plugs.get(ref.name, ref.version)
-            elif isinstance(create_resp, PostWebscriptJobSyncResponseV2):
-                jobs_resp = await self.webscripts.get(ref.name, ref.version)
-            else:
-                jobs_resp = create_resp
-            logger = logger or LOG
-            logger.info("Waiting for %s@%s to be ready:", ref.name, ref.version)
-            event_href: str
-            event_link = getattr(jobs_resp.links, "event", None)
-            if not event_link:
+            if not event_href:
+                if as_plug:
+                    jobs_resp = await self.plugs.get(name, version, response_type=Any)
+                else:
+                    jobs_resp = await self.webscripts.get(
+                        name, version, response_type=Any
+                    )
+                event_href = (
+                    jobs_resp.get("_links", {}).get("event", {}).get("href", None)
+                )
+            logger.info("Waiting for %s@%s to be ready:", name, version)
+            if not event_href:
                 raise WaylayError("no event link available")
-            event_href = event_link.href
             logger.info("listening on %s", event_href)
             _last_event = await self.log_events(event_href, logger)
-
-        if is_webscript:
-            result = await self.webscripts.get(ref.name, ref.version)
-        else:
-            result = await self.plugs.get(ref.name, ref.version)
-        status = result.entity.status
-        logger.info("function %s@%s has status %s", ref.name, ref.version, status)
+            result: dict[str, Any] = {}
+            if as_webscript:
+                result = await self.webscripts.get(name, version, response_type=Any)
+            else:
+                result = await self.plugs.get(name, version, response_type=Any)
+            status = result["entity"]["status"]
+        logger.info("function %s@%s has status %s", name, version, status)
         if status in success_states:
             return result
-        raise WaylayError(f"Deployment failed: {result.entity.failure_reason}")
+        raise WaylayError(
+            f"Deployment failed: {result['entity'].get('failureReason','')}"
+        )
 
-    def _log_event(
-        self, event: EventWithCloseSSE, logger: Optional[logging.Logger] = None
-    ):
+    def _log_event(self, event: dict, logger: logging.Logger | None = None):
         logger = logger or LOG
-        event_type = getattr(event, "event", None)
+        event_type = event.get("event")
         if event_type is None:
             logger.warning("%s", event)
+            return None
+        event_data = event.get("data", {})
+        event_info = event_data
+        if not isinstance(event_info, dict):
+            logger.info("%s: %s", event_type, event_info)
             return event_type
-        event_info = getattr(event, "data", None)
-        job = getattr(event_info, "job", "")
-        job_type = getattr(job, "type", "")
+        job = event_info.get("job", {})
+        job_type = job.get("type", "")
         if job_type == "":
-            logger.info("%s\n%s", event_type, event_info)
+            logger.info("%s: %s", event_type, event_info)
             return event_type
-        func = getattr(event_info, "function", "")
-        func_name = getattr(func, "name", "")
-        func_version = getattr(func, "version", "")
+        func = event_info.get("function", {})
+        func_name = func.get("name", "")
+        func_version = func.get("version", "")
         func_ref = f"{func_name}@{func_version}" if func else ""
         event_log = f"{func_ref} {job_type}: {event_type}"
         if event_type in ["completed", "failed"]:
             event_log += f"\n{event_info}"
         logger.info("%s", event_log)
         return event_type
 
     async def log_events(
         self,
-        query_or_url: Union[str, dict],
-        logger: Optional[logging.Logger] = None,
+        query_or_url: str | dict,
+        logger: logging.Logger | None = None,
         close_on_event: tuple[str] = ("close",),
     ):
         """Log job events for the given url or query."""
         iter_events = await self.iter_events(query_or_url)
         async for event in iter_events:
             event_type = self._log_event(event, logger)
             if event_type in close_on_event:
                 return event
 
-    async def iter_events(
-        self, query_or_url: Union[str, dict]
-    ) -> AsyncIterator[EventWithCloseSSE]:
+    async def iter_events(self, query_or_url: str | dict) -> AsyncIterator:
         """Iterate over job events."""
         if isinstance(query_or_url, str):
-            iterator = await self.registry.api_client.request(
-                "GET",
-                query_or_url,
-                stream=True,
-                timeout=STREAM_TIMEOUTS,
-                response_type=EventWithCloseSSE,
+            return cast(
+                AsyncIterator,
+                await self.registry.api_client.request(
+                    "GET",
+                    query_or_url,
+                    stream=True,
+                    timeout=STREAM_TIMEOUTS,
+                    response_type=Any,
+                ),
             )
-            return cast(AsyncIterator[EventWithCloseSSE], iterator)
         else:
             return await self.registry.jobs.events(
                 query=query_or_url,
                 stream=True,
                 timeout=STREAM_TIMEOUTS,
-                # TODO ,validate_query=False
+                validate_request=False,
+                response_type=Any,
             )
 
-    async def test_webscript(self, ref: GetWebscriptResponseV2 | dict, instances):
+    async def test_webscript(self, ref: dict, instances):
         """Test invocation of a deployed ml function."""
-        func_resp = _as_model(ref, GetWebscriptResponseV2)
-        invoke_link = func_resp.links.invoke
+        invoke_link = ref["_links"]["invoke"]
         if not invoke_link:
             raise WaylayError("No invocation link available")
         resp = await self.api_client.request(
-            "POST", invoke_link.href, json={"instances": instances}, raw_response=True
+            "POST",
+            invoke_link["href"],
+            json={"instances": instances},
+            raw_response=True,
+            response_type=Any,
         )
         data = resp.json()
         data = data.get("predictions", data)
         return data
 
-    async def test_plug(
-        self, ref: GetPlugResponseV2 | dict, data, protocol=V1_PROTOCOL
-    ):
+    async def test_plug(self, ref: dict, data, protocol=V1_PROTOCOL):
         """Test invocation of a deployed ml function."""
         if not isinstance(data, dict) or (
             "instances" not in data and "inputs" not in data
         ):
             key = "instances" if protocol == V1_PROTOCOL else "inputs"
             data = {key: data}
-        plug = _as_model(ref, GetPlugResponseV2).entity.plug
-        invoke_resp = await self.rules.plugs_execution.execute_sensor_version(
-            plug.name, plug.version, json={"properties": data}
+        plug = ref["entity"]["plug"]
+        invoke_resp: dict = await self.rules.plugs_execution.execute_sensor_version(
+            plug["name"], plug["version"], json={"properties": data}, response_type=Any
         )
-        resp_data = invoke_resp.raw_data or {}
+        resp_data = invoke_resp.get("rawData", {})
         for key in ["predictions", "outputs"]:
             if key in resp_data:
                 return resp_data[key]
         return resp_data
 
-    async def publish(self, ref: FunctionResponse | dict):
+    async def publish(self, ref: dict):
         """Publish a deployed function."""
-        ref = _as_model(ref, FunctionResponse)
-        ws_ref = getattr(ref.entity, "webscript", None)
-        if ws_ref:
-            return await self.webscripts.publish(ws_ref.name, ws_ref.version)
-        plug_ref = getattr(ref.entity, "plug", None)
-        if plug_ref:
-            return await self.plugs.publish(plug_ref.name, plug_ref.version)
+        entity = ref["entity"]
+        as_webscript = entity.get("webscript", False)
+        as_plug = entity.get("plug", False)
+        if as_webscript:
+            return await self.webscripts.publish(
+                as_webscript["name"], as_webscript["version"], response_type=Any
+            )
+        if as_plug:
+            return await self.plugs.publish(
+                as_plug["name"], as_plug["version"], response_type=Any
+            )
 
     @retry(reraise=True, stop=stop_after_delay(30), wait=wait_exponential(max=10))
-    async def remove(self, ref: FunctionResponse | dict, force=True):
+    async def remove(self, ref: dict, force=True):
         """Remove a deployed function."""
-        ref = _as_model(ref, FunctionResponse)
-        ws_ref = getattr(ref.entity, "webscript", None)
-        if ws_ref:
+        entity = ref["entity"]
+        as_webscript = entity.get("webscript", False)
+        as_plug = entity.get("plug", False)
+        if as_webscript:
             return await self.webscripts.remove_version(
-                ws_ref.name, ws_ref.version, query={"force": force}
+                as_webscript["name"],
+                as_webscript["version"],
+                query={"force": force},
+                response_type=Any,
             )
-        plug_ref = getattr(ref.entity, "plug", None)
-        if plug_ref:
+        if as_plug:
             return await self.plugs.remove_version(
-                plug_ref.name, plug_ref.version, query={"force": force}
+                as_plug["name"],
+                as_plug["version"],
+                query={"force": force},
+                response_type=Any,
             )
 
 
 def _as_model(ref, _type):
     return TypeAdapter(_type).validate_python(ref)
```

