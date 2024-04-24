# Comparing `tmp/beta9-0.1.2.tar.gz` & `tmp/beta9-0.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beta9-0.1.2.tar", max compression
+gzip compressed data, was "beta9-0.1.2rc1.tar", max compression
```

## Comparing `beta9-0.1.2.tar` & `beta9-0.1.2rc1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1127 2024-04-24 16:12:32.840885 beta9-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      557 2024-04-21 16:36:14.953402 beta9-0.1.2/src/beta9/__init__.py
--rw-r--r--   0        0        0        0 2024-01-27 16:13:22.962074 beta9-0.1.2/src/beta9/abstractions/__init__.py
--rw-r--r--   0        0        0      606 2024-01-27 16:13:22.962265 beta9-0.1.2/src/beta9/abstractions/base/__init__.py
--rw-r--r--   0        0        0     8509 2024-04-21 16:36:14.953658 beta9-0.1.2/src/beta9/abstractions/base/runner.py
--rw-r--r--   0        0        0     3492 2024-04-21 16:36:14.953861 beta9-0.1.2/src/beta9/abstractions/container.py
--rw-r--r--   0        0        0     4432 2024-04-21 16:36:14.954028 beta9-0.1.2/src/beta9/abstractions/endpoint.py
--rw-r--r--   0        0        0     6595 2024-04-21 16:36:14.954181 beta9-0.1.2/src/beta9/abstractions/function.py
--rw-r--r--   0        0        0     4264 2024-04-21 16:36:14.954354 beta9-0.1.2/src/beta9/abstractions/image.py
--rw-r--r--   0        0        0     3237 2024-04-21 16:36:14.954512 beta9-0.1.2/src/beta9/abstractions/map.py
--rw-r--r--   0        0        0     3183 2024-04-21 16:36:14.955563 beta9-0.1.2/src/beta9/abstractions/queue.py
--rw-r--r--   0        0        0     8263 2024-04-21 16:36:14.956665 beta9-0.1.2/src/beta9/abstractions/taskqueue.py
--rw-r--r--   0        0        0     1605 2024-04-21 16:36:14.957214 beta9-0.1.2/src/beta9/abstractions/volume.py
--rw-r--r--   0        0        0      292 2024-01-27 16:13:22.963762 beta9-0.1.2/src/beta9/aio.py
--rw-r--r--   0        0        0        0 2024-01-27 16:13:22.963872 beta9-0.1.2/src/beta9/cli/__init__.py
--rw-r--r--   0        0        0      932 2024-04-21 16:36:14.959066 beta9-0.1.2/src/beta9/cli/config.py
--rw-r--r--   0        0        0      824 2024-04-21 16:36:14.962332 beta9-0.1.2/src/beta9/cli/contexts.py
--rw-r--r--   0        0        0     2422 2024-04-21 16:36:14.964463 beta9-0.1.2/src/beta9/cli/deployment.py
--rw-r--r--   0        0        0     3197 2024-04-21 16:36:14.964958 beta9-0.1.2/src/beta9/cli/extraclick.py
--rw-r--r--   0        0        0     1140 2024-04-21 16:36:14.966489 beta9-0.1.2/src/beta9/cli/main.py
--rw-r--r--   0        0        0     3738 2024-04-21 16:36:14.968025 beta9-0.1.2/src/beta9/cli/task.py
--rw-r--r--   0        0        0     8667 2024-04-21 16:36:14.970907 beta9-0.1.2/src/beta9/cli/volume.py
--rw-r--r--   0        0        0        0 2024-04-19 22:28:40.826909 beta9-0.1.2/src/beta9/clients/__init__.py
--rw-r--r--   0        0        0     2980 2024-04-21 16:36:14.973223 beta9-0.1.2/src/beta9/clients/container/__init__.py
--rw-r--r--   0        0        0     4275 2024-04-21 16:36:14.974260 beta9-0.1.2/src/beta9/clients/endpoint/__init__.py
--rw-r--r--   0        0        0     8023 2024-04-21 16:36:14.975351 beta9-0.1.2/src/beta9/clients/function/__init__.py
--rw-r--r--   0        0        0    21023 2024-04-21 16:36:14.977082 beta9-0.1.2/src/beta9/clients/gateway/__init__.py
--rw-r--r--   0        0        0     4773 2024-04-21 16:36:14.978808 beta9-0.1.2/src/beta9/clients/image/__init__.py
--rw-r--r--   0        0        0     8003 2024-04-21 16:36:14.979185 beta9-0.1.2/src/beta9/clients/map/__init__.py
--rw-r--r--   0        0        0     8687 2024-04-21 16:36:14.979353 beta9-0.1.2/src/beta9/clients/simplequeue/__init__.py
--rw-r--r--   0        0        0    13315 2024-04-21 16:36:14.979574 beta9-0.1.2/src/beta9/clients/taskqueue/__init__.py
--rw-r--r--   0        0        0     9482 2024-04-21 16:36:14.979799 beta9-0.1.2/src/beta9/clients/volume/__init__.py
--rw-r--r--   0        0        0     7301 2024-04-21 16:36:14.980146 beta9-0.1.2/src/beta9/config.py
--rw-r--r--   0        0        0      207 2024-01-27 16:13:22.966808 beta9-0.1.2/src/beta9/exceptions.py
--rw-r--r--   0        0        0      886 2024-04-21 16:36:14.980276 beta9-0.1.2/src/beta9/logging.py
--rw-r--r--   0        0        0        0 2024-01-27 16:13:22.966902 beta9-0.1.2/src/beta9/runner/__init__.py
--rw-r--r--   0        0        0     2618 2024-04-21 16:36:14.980451 beta9-0.1.2/src/beta9/runner/common.py
--rw-r--r--   0        0        0     2321 2024-04-21 16:36:14.980604 beta9-0.1.2/src/beta9/runner/container.py
--rw-r--r--   0        0        0     7210 2024-04-21 16:36:14.982122 beta9-0.1.2/src/beta9/runner/endpoint.py
--rw-r--r--   0        0        0     5906 2024-04-21 16:36:14.983323 beta9-0.1.2/src/beta9/runner/function.py
--rw-r--r--   0        0        0     3910 2024-04-21 16:36:14.986354 beta9-0.1.2/src/beta9/runner/serve.py
--rw-r--r--   0        0        0    10603 2024-04-21 16:36:14.989627 beta9-0.1.2/src/beta9/runner/taskqueue.py
--rw-r--r--   0        0        0     5593 2024-04-21 16:36:14.994797 beta9-0.1.2/src/beta9/sync.py
--rw-r--r--   0        0        0     2994 2024-04-21 16:36:14.997902 beta9-0.1.2/src/beta9/terminal.py
--rw-r--r--   0        0        0     1399 2024-01-27 16:13:22.968161 beta9-0.1.2/src/beta9/type.py
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 beta9-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1130 2024-04-17 13:23:37.995931 beta9-0.1.2rc1/pyproject.toml
+-rw-r--r--   0        0        0      557 2024-04-17 13:13:37.445495 beta9-0.1.2rc1/src/beta9/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-23 23:38:59.669351 beta9-0.1.2rc1/src/beta9/abstractions/__init__.py
+-rw-r--r--   0        0        0      606 2024-01-23 23:38:59.669478 beta9-0.1.2rc1/src/beta9/abstractions/base/__init__.py
+-rw-r--r--   0        0        0     8509 2024-04-17 13:14:18.140772 beta9-0.1.2rc1/src/beta9/abstractions/base/runner.py
+-rw-r--r--   0        0        0     3492 2024-04-17 13:14:18.141093 beta9-0.1.2rc1/src/beta9/abstractions/container.py
+-rw-r--r--   0        0        0     3977 2024-04-17 13:14:18.141399 beta9-0.1.2rc1/src/beta9/abstractions/endpoint.py
+-rw-r--r--   0        0        0     6175 2024-04-17 13:14:18.141584 beta9-0.1.2rc1/src/beta9/abstractions/function.py
+-rw-r--r--   0        0        0     4264 2024-04-17 13:14:18.141720 beta9-0.1.2rc1/src/beta9/abstractions/image.py
+-rw-r--r--   0        0        0     3237 2024-04-17 13:14:18.141834 beta9-0.1.2rc1/src/beta9/abstractions/map.py
+-rw-r--r--   0        0        0     3183 2024-04-17 13:14:18.141940 beta9-0.1.2rc1/src/beta9/abstractions/queue.py
+-rw-r--r--   0        0        0     6395 2024-04-17 13:14:18.142080 beta9-0.1.2rc1/src/beta9/abstractions/taskqueue.py
+-rw-r--r--   0        0        0     1605 2024-04-17 13:14:18.142367 beta9-0.1.2rc1/src/beta9/abstractions/volume.py
+-rw-r--r--   0        0        0      292 2024-04-15 21:13:39.880348 beta9-0.1.2rc1/src/beta9/aio.py
+-rw-r--r--   0        0        0        0 2024-01-23 23:38:59.670190 beta9-0.1.2rc1/src/beta9/cli/__init__.py
+-rw-r--r--   0        0        0      932 2024-04-17 13:14:18.142672 beta9-0.1.2rc1/src/beta9/cli/config.py
+-rw-r--r--   0        0        0      824 2024-04-17 13:14:18.143012 beta9-0.1.2rc1/src/beta9/cli/contexts.py
+-rw-r--r--   0        0        0     2422 2024-04-17 13:14:18.143206 beta9-0.1.2rc1/src/beta9/cli/deployment.py
+-rw-r--r--   0        0        0     3197 2024-04-17 13:14:18.143457 beta9-0.1.2rc1/src/beta9/cli/extraclick.py
+-rw-r--r--   0        0        0     1140 2024-04-17 13:14:18.143741 beta9-0.1.2rc1/src/beta9/cli/main.py
+-rw-r--r--   0        0        0     3738 2024-04-17 13:14:18.144016 beta9-0.1.2rc1/src/beta9/cli/task.py
+-rw-r--r--   0        0        0     8667 2024-04-17 13:14:18.144318 beta9-0.1.2rc1/src/beta9/cli/volume.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:32:37.403246 beta9-0.1.2rc1/src/beta9/clients/__init__.py
+-rw-r--r--   0        0        0     2980 2024-04-17 13:14:18.144448 beta9-0.1.2rc1/src/beta9/clients/container/__init__.py
+-rw-r--r--   0        0        0     2499 2024-04-17 13:14:18.144717 beta9-0.1.2rc1/src/beta9/clients/endpoint/__init__.py
+-rw-r--r--   0        0        0     8023 2024-04-17 13:14:18.144848 beta9-0.1.2rc1/src/beta9/clients/function/__init__.py
+-rw-r--r--   0        0        0    21023 2024-04-17 13:14:18.144938 beta9-0.1.2rc1/src/beta9/clients/gateway/__init__.py
+-rw-r--r--   0        0        0     4773 2024-04-17 13:14:18.145074 beta9-0.1.2rc1/src/beta9/clients/image/__init__.py
+-rw-r--r--   0        0        0     8003 2024-04-17 13:14:18.145188 beta9-0.1.2rc1/src/beta9/clients/map/__init__.py
+-rw-r--r--   0        0        0     8687 2024-04-17 13:14:18.145328 beta9-0.1.2rc1/src/beta9/clients/simplequeue/__init__.py
+-rw-r--r--   0        0        0     9665 2024-04-17 13:14:18.145458 beta9-0.1.2rc1/src/beta9/clients/taskqueue/__init__.py
+-rw-r--r--   0        0        0     9482 2024-04-17 13:14:18.145732 beta9-0.1.2rc1/src/beta9/clients/volume/__init__.py
+-rw-r--r--   0        0        0     7301 2024-04-17 13:14:18.145934 beta9-0.1.2rc1/src/beta9/config.py
+-rw-r--r--   0        0        0      207 2024-01-23 23:38:59.671504 beta9-0.1.2rc1/src/beta9/exceptions.py
+-rw-r--r--   0        0        0      886 2024-04-17 13:13:37.450038 beta9-0.1.2rc1/src/beta9/logging.py
+-rw-r--r--   0        0        0        0 2024-01-23 23:38:59.671565 beta9-0.1.2rc1/src/beta9/runner/__init__.py
+-rw-r--r--   0        0        0     2462 2024-04-17 13:14:18.146268 beta9-0.1.2rc1/src/beta9/runner/common.py
+-rw-r--r--   0        0        0     2321 2024-04-17 13:14:18.146631 beta9-0.1.2rc1/src/beta9/runner/container.py
+-rw-r--r--   0        0        0     4647 2024-04-17 13:14:18.146985 beta9-0.1.2rc1/src/beta9/runner/endpoint.py
+-rw-r--r--   0        0        0     5905 2024-04-17 13:14:18.147159 beta9-0.1.2rc1/src/beta9/runner/function.py
+-rw-r--r--   0        0        0     3910 2024-04-17 13:14:18.147410 beta9-0.1.2rc1/src/beta9/runner/serve.py
+-rw-r--r--   0        0        0    10259 2024-04-17 13:14:18.147724 beta9-0.1.2rc1/src/beta9/runner/taskqueue.py
+-rw-r--r--   0        0        0     5593 2024-04-17 13:14:18.148222 beta9-0.1.2rc1/src/beta9/sync.py
+-rw-r--r--   0        0        0     2994 2024-04-17 13:14:18.148560 beta9-0.1.2rc1/src/beta9/terminal.py
+-rw-r--r--   0        0        0     1399 2024-01-23 23:38:59.672017 beta9-0.1.2rc1/src/beta9/type.py
+-rw-r--r--   0        0        0      985 1970-01-01 00:00:00.000000 beta9-0.1.2rc1/PKG-INFO
```

### Comparing `beta9-0.1.2/pyproject.toml` & `beta9-0.1.2rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beta9"
-version = "0.1.2"
+version = "0.1.2rc1"
 description = ""
 authors = ["beam.cloud <support@beam.cloud>"]
 packages = [
     { include = "beta9", from = "src" },
     { include = "beta9/**/*.py", from = "src" },
 ]
```

### Comparing `beta9-0.1.2/src/beta9/__init__.py` & `beta9-0.1.2rc1/src/beta9/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/abstractions/base/__init__.py` & `beta9-0.1.2rc1/src/beta9/abstractions/base/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/abstractions/base/runner.py` & `beta9-0.1.2rc1/src/beta9/abstractions/base/runner.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/abstractions/container.py` & `beta9-0.1.2rc1/src/beta9/abstractions/container.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/abstractions/endpoint.py` & `beta9-0.1.2rc1/src/beta9/abstractions/endpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,15 @@
 from .. import terminal
 from ..abstractions.base.runner import (
     ENDPOINT_DEPLOYMENT_STUB_TYPE,
     ENDPOINT_SERVE_STUB_TYPE,
     RunnerAbstraction,
 )
 from ..abstractions.image import Image
-from ..clients.endpoint import (
-    EndpointServiceStub,
-    StartEndpointServeRequest,
-    StopEndpointServeRequest,
-)
+from ..clients.endpoint import EndpointServeRequest, EndpointServiceStub
 from ..clients.gateway import DeployStubRequest, DeployStubResponse
 from ..config import GatewayConfig, get_gateway_config
 
 
 class Endpoint(RunnerAbstraction):
     def __init__(
         self,
@@ -93,34 +89,23 @@
 
         try:
             with terminal.progress("Serving endpoint..."):
                 return self.parent.run_sync(
                     self._serve(dir=os.getcwd(), object_id=self.parent.object_id)
                 )
         except KeyboardInterrupt:
-            response = terminal.prompt(
-                text="Would you like to stop the container? (y/n)", default="y"
-            )
-            if response == "y":
-                terminal.header("Stopping serve container")
-                self.parent.run_sync(
-                    self.parent.endpoint_stub.stop_endpoint_serve(
-                        StopEndpointServeRequest(stub_id=self.parent.stub_id)
-                    )
-                )
-
-        terminal.print("Goodbye 👋")
+            terminal.prompt(text="Would you like to stop the container? (y/n)", default="y")
 
     async def _serve(self, *, dir: str, object_id: str):
         sync_task = self.parent.loop.create_task(
             self.parent.sync_dir_to_workspace(dir=dir, object_id=object_id)
         )
         try:
-            async for r in self.parent.endpoint_stub.start_endpoint_serve(
-                StartEndpointServeRequest(
+            async for r in self.parent.endpoint_stub.endpoint_serve(
+                EndpointServeRequest(
                     stub_id=self.parent.stub_id,
                 )
             ):
                 if r.output != "":
                     terminal.detail(r.output.strip())
 
                 if r.done or r.exit_code != 0:
```

### Comparing `beta9-0.1.2/src/beta9/abstractions/function.py` & `beta9-0.1.2rc1/src/beta9/abstractions/function.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,28 +59,18 @@
     """
 
     def __init__(
         self,
         cpu: Union[int, float, str] = 1.0,
         memory: int = 128,
         gpu: str = "",
-        timeout: int = 3600,
-        retries: int = 3,
         image: Image = Image(),
         volumes: Optional[List[Volume]] = None,
     ) -> None:
-        super().__init__(
-            cpu=cpu,
-            memory=memory,
-            gpu=gpu,
-            image=image,
-            volumes=volumes,
-            timeout=timeout,
-            retries=retries,
-        )
+        super().__init__(cpu=cpu, memory=memory, gpu=gpu, image=image, volumes=volumes)
 
         self.function_stub: FunctionServiceStub = FunctionServiceStub(self.channel)
         self.syncer: FileSyncer = FileSyncer(self.gateway_stub)
 
     def __call__(self, func):
         return _CallableWrapper(func, self)
 
@@ -161,28 +151,19 @@
             terminal.header("Deployed 🎉")
             terminal.detail(
                 f"Call your deployment at: {gateway_url}/api/v1/function/{name}/v{deploy_response.version}"
             )
 
         return deploy_response.ok
 
-    def _format_args(self, args):
-        if isinstance(args, tuple):
-            return list(args)
-        elif not isinstance(args, list):
-            return [args]
-        return args
-
     def _gather_and_yield_results(self, inputs: Sequence) -> Iterator[Any]:
         container_count = len(inputs)
 
         async def _gather_async():
-            tasks = [
-                asyncio.create_task(self._call_remote(*self._format_args(args))) for args in inputs
-            ]
+            tasks = [asyncio.create_task(self._call_remote(input)) for input in inputs]
             for task in asyncio.as_completed(tasks):
                 yield await task
 
         async_gen = _gather_async()
         with terminal.progress(f"Running {container_count} containers..."):
             while True:
                 try:
```

### Comparing `beta9-0.1.2/src/beta9/abstractions/image.py` & `beta9-0.1.2rc1/src/beta9/abstractions/image.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/abstractions/map.py` & `beta9-0.1.2rc1/src/beta9/abstractions/map.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/abstractions/queue.py` & `beta9-0.1.2rc1/src/beta9/abstractions/queue.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/abstractions/taskqueue.py` & `beta9-0.1.2rc1/src/beta9/abstractions/taskqueue.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 import json
 import os
 from typing import Any, Callable, Union
 
 from .. import terminal
 from ..abstractions.base.runner import (
     TASKQUEUE_DEPLOYMENT_STUB_TYPE,
-    TASKQUEUE_SERVE_STUB_TYPE,
     TASKQUEUE_STUB_TYPE,
     RunnerAbstraction,
 )
 from ..abstractions.image import Image
 from ..clients.gateway import DeployStubRequest, DeployStubResponse
-from ..clients.taskqueue import (
-    StartTaskQueueServeRequest,
-    StopTaskQueueServeRequest,
-    TaskQueuePutRequest,
-    TaskQueuePutResponse,
-    TaskQueueServiceStub,
-)
+from ..clients.taskqueue import TaskQueuePutRequest, TaskQueuePutResponse, TaskQueueServiceStub
 from ..config import GatewayConfig, get_gateway_config
 
 
 class TaskQueue(RunnerAbstraction):
     """
     Decorator which allows you to create a task queue out of the decorated function. The tasks are executed
     asynchronously, in remote containers. You can interact with the task queue either through an API (when deployed), or directly
@@ -146,61 +139,14 @@
             terminal.header("Deployed 🎉")
             terminal.detail(
                 f"Call your deployment at: {gateway_url}/api/v1/taskqueue/{name}/v{deploy_response.version}"
             )
 
         return deploy_response.ok
 
-    def serve(self):
-        if not self.parent.prepare_runtime(
-            func=self.func, stub_type=TASKQUEUE_SERVE_STUB_TYPE, force_create_stub=True
-        ):
-            return False
-
-        try:
-            with terminal.progress("Serving taskqueue..."):
-                return self.parent.run_sync(
-                    self._serve(dir=os.getcwd(), object_id=self.parent.object_id)
-                )
-        except KeyboardInterrupt:
-            response = terminal.prompt(
-                text="Would you like to stop the container? (y/n)", default="y"
-            )
-            if response == "y":
-                terminal.header("Stopping serve container")
-                self.parent.run_sync(
-                    self.parent.taskqueue_stub.stop_task_queue_serve(
-                        StopTaskQueueServeRequest(stub_id=self.parent.stub_id)
-                    )
-                )
-
-        terminal.print("Goodbye 👋")
-
-    async def _serve(self, *, dir: str, object_id: str):
-        sync_task = self.parent.loop.create_task(
-            self.parent.sync_dir_to_workspace(dir=dir, object_id=object_id)
-        )
-        try:
-            async for r in self.parent.taskqueue_stub.start_task_queue_serve(
-                StartTaskQueueServeRequest(
-                    stub_id=self.parent.stub_id,
-                )
-            ):
-                if r.output != "":
-                    terminal.detail(r.output.strip())
-
-                if r.done or r.exit_code != 0:
-                    last_response = r
-                    break
-
-            if last_response is None or not last_response.done or last_response.exit_code != 0:
-                terminal.error("Serve container failed ☠️")
-        finally:
-            sync_task.cancel()
-
     def put(self, *args, **kwargs) -> bool:
         if not self.parent.prepare_runtime(
             func=self.func,
             stub_type=TASKQUEUE_STUB_TYPE,
         ):
             return False
```

### Comparing `beta9-0.1.2/src/beta9/abstractions/volume.py` & `beta9-0.1.2rc1/src/beta9/abstractions/volume.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/cli/config.py` & `beta9-0.1.2rc1/src/beta9/cli/config.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/cli/contexts.py` & `beta9-0.1.2rc1/src/beta9/cli/contexts.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/cli/deployment.py` & `beta9-0.1.2rc1/src/beta9/cli/deployment.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/cli/extraclick.py` & `beta9-0.1.2rc1/src/beta9/cli/extraclick.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/cli/main.py` & `beta9-0.1.2rc1/src/beta9/cli/main.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/cli/task.py` & `beta9-0.1.2rc1/src/beta9/cli/task.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/cli/volume.py` & `beta9-0.1.2rc1/src/beta9/cli/volume.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/clients/container/__init__.py` & `beta9-0.1.2rc1/src/beta9/clients/container/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/clients/endpoint/__init__.py` & `beta9-0.1.2rc1/src/beta9/clients/image/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: endpoint.proto
+# sources: image.proto
 # plugin: python-betterproto
 # This file has been @generated
 
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
     AsyncIterator,
     Dict,
+    List,
     Optional,
 )
 
 import betterproto
 import grpclib
 from betterproto.grpc.grpclib_server import ServiceBase
 
@@ -19,112 +20,126 @@
 if TYPE_CHECKING:
     import grpclib.server
     from betterproto.grpc.grpclib_client import MetadataLike
     from grpclib.metadata import Deadline
 
 
 @dataclass(eq=False, repr=False)
-class StartEndpointServeRequest(betterproto.Message):
-    stub_id: str = betterproto.string_field(1)
+class VerifyImageBuildRequest(betterproto.Message):
+    python_version: str = betterproto.string_field(1)
+    python_packages: List[str] = betterproto.string_field(2)
+    commands: List[str] = betterproto.string_field(3)
+    force_rebuild: bool = betterproto.bool_field(4)
+    existing_image_uri: str = betterproto.string_field(5)
 
 
 @dataclass(eq=False, repr=False)
-class StartEndpointServeResponse(betterproto.Message):
-    output: str = betterproto.string_field(1)
-    done: bool = betterproto.bool_field(2)
-    exit_code: int = betterproto.int32_field(3)
+class VerifyImageBuildResponse(betterproto.Message):
+    image_id: str = betterproto.string_field(1)
+    valid: bool = betterproto.bool_field(2)
+    exists: bool = betterproto.bool_field(3)
 
 
 @dataclass(eq=False, repr=False)
-class StopEndpointServeRequest(betterproto.Message):
-    stub_id: str = betterproto.string_field(1)
+class BuildImageRequest(betterproto.Message):
+    python_version: str = betterproto.string_field(1)
+    """These parameters are used for a "beta9" managed image"""
+
+    python_packages: List[str] = betterproto.string_field(2)
+    commands: List[str] = betterproto.string_field(3)
+    existing_image_uri: str = betterproto.string_field(4)
+    """These parameters are used for an existing image"""
+
+    existing_image_creds: str = betterproto.string_field(5)
 
 
 @dataclass(eq=False, repr=False)
-class StopEndpointServeResponse(betterproto.Message):
-    ok: bool = betterproto.bool_field(1)
+class BuildImageResponse(betterproto.Message):
+    image_id: str = betterproto.string_field(1)
+    msg: str = betterproto.string_field(2)
+    done: bool = betterproto.bool_field(3)
+    success: bool = betterproto.bool_field(4)
 
 
-class EndpointServiceStub(betterproto.ServiceStub):
-    async def start_endpoint_serve(
+class ImageServiceStub(betterproto.ServiceStub):
+    async def verify_image_build(
         self,
-        start_endpoint_serve_request: "StartEndpointServeRequest",
+        verify_image_build_request: "VerifyImageBuildRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> AsyncIterator["StartEndpointServeResponse"]:
-        async for response in self._unary_stream(
-            "/endpoint.EndpointService/StartEndpointServe",
-            start_endpoint_serve_request,
-            StartEndpointServeResponse,
+    ) -> "VerifyImageBuildResponse":
+        return await self._unary_unary(
+            "/image.ImageService/VerifyImageBuild",
+            verify_image_build_request,
+            VerifyImageBuildResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
-        ):
-            yield response
+        )
 
-    async def stop_endpoint_serve(
+    async def build_image(
         self,
-        stop_endpoint_serve_request: "StopEndpointServeRequest",
+        build_image_request: "BuildImageRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "StopEndpointServeResponse":
-        return await self._unary_unary(
-            "/endpoint.EndpointService/StopEndpointServe",
-            stop_endpoint_serve_request,
-            StopEndpointServeResponse,
+    ) -> AsyncIterator["BuildImageResponse"]:
+        async for response in self._unary_stream(
+            "/image.ImageService/BuildImage",
+            build_image_request,
+            BuildImageResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
-        )
+        ):
+            yield response
 
 
-class EndpointServiceBase(ServiceBase):
+class ImageServiceBase(ServiceBase):
 
-    async def start_endpoint_serve(
-        self, start_endpoint_serve_request: "StartEndpointServeRequest"
-    ) -> AsyncIterator["StartEndpointServeResponse"]:
+    async def verify_image_build(
+        self, verify_image_build_request: "VerifyImageBuildRequest"
+    ) -> "VerifyImageBuildResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
-        yield StartEndpointServeResponse()
 
-    async def stop_endpoint_serve(
-        self, stop_endpoint_serve_request: "StopEndpointServeRequest"
-    ) -> "StopEndpointServeResponse":
+    async def build_image(
+        self, build_image_request: "BuildImageRequest"
+    ) -> AsyncIterator["BuildImageResponse"]:
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
+        yield BuildImageResponse()
 
-    async def __rpc_start_endpoint_serve(
+    async def __rpc_verify_image_build(
         self,
-        stream: "grpclib.server.Stream[StartEndpointServeRequest, StartEndpointServeResponse]",
+        stream: "grpclib.server.Stream[VerifyImageBuildRequest, VerifyImageBuildResponse]",
+    ) -> None:
+        request = await stream.recv_message()
+        response = await self.verify_image_build(request)
+        await stream.send_message(response)
+
+    async def __rpc_build_image(
+        self, stream: "grpclib.server.Stream[BuildImageRequest, BuildImageResponse]"
     ) -> None:
         request = await stream.recv_message()
         await self._call_rpc_handler_server_stream(
-            self.start_endpoint_serve,
+            self.build_image,
             stream,
             request,
         )
 
-    async def __rpc_stop_endpoint_serve(
-        self,
-        stream: "grpclib.server.Stream[StopEndpointServeRequest, StopEndpointServeResponse]",
-    ) -> None:
-        request = await stream.recv_message()
-        response = await self.stop_endpoint_serve(request)
-        await stream.send_message(response)
-
     def __mapping__(self) -> Dict[str, grpclib.const.Handler]:
         return {
-            "/endpoint.EndpointService/StartEndpointServe": grpclib.const.Handler(
-                self.__rpc_start_endpoint_serve,
-                grpclib.const.Cardinality.UNARY_STREAM,
-                StartEndpointServeRequest,
-                StartEndpointServeResponse,
-            ),
-            "/endpoint.EndpointService/StopEndpointServe": grpclib.const.Handler(
-                self.__rpc_stop_endpoint_serve,
+            "/image.ImageService/VerifyImageBuild": grpclib.const.Handler(
+                self.__rpc_verify_image_build,
                 grpclib.const.Cardinality.UNARY_UNARY,
-                StopEndpointServeRequest,
-                StopEndpointServeResponse,
+                VerifyImageBuildRequest,
+                VerifyImageBuildResponse,
+            ),
+            "/image.ImageService/BuildImage": grpclib.const.Handler(
+                self.__rpc_build_image,
+                grpclib.const.Cardinality.UNARY_STREAM,
+                BuildImageRequest,
+                BuildImageResponse,
             ),
         }
```

### Comparing `beta9-0.1.2/src/beta9/clients/function/__init__.py` & `beta9-0.1.2rc1/src/beta9/clients/function/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/clients/gateway/__init__.py` & `beta9-0.1.2rc1/src/beta9/clients/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/clients/map/__init__.py` & `beta9-0.1.2rc1/src/beta9/clients/map/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/clients/simplequeue/__init__.py` & `beta9-0.1.2rc1/src/beta9/clients/simplequeue/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/clients/taskqueue/__init__.py` & `beta9-0.1.2rc1/src/beta9/clients/taskqueue/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -84,36 +84,14 @@
 class TaskQueueMonitorResponse(betterproto.Message):
     ok: bool = betterproto.bool_field(1)
     cancelled: bool = betterproto.bool_field(2)
     complete: bool = betterproto.bool_field(3)
     timed_out: bool = betterproto.bool_field(4)
 
 
-@dataclass(eq=False, repr=False)
-class StartTaskQueueServeRequest(betterproto.Message):
-    stub_id: str = betterproto.string_field(1)
-
-
-@dataclass(eq=False, repr=False)
-class StartTaskQueueServeResponse(betterproto.Message):
-    output: str = betterproto.string_field(1)
-    done: bool = betterproto.bool_field(2)
-    exit_code: int = betterproto.int32_field(3)
-
-
-@dataclass(eq=False, repr=False)
-class StopTaskQueueServeRequest(betterproto.Message):
-    stub_id: str = betterproto.string_field(1)
-
-
-@dataclass(eq=False, repr=False)
-class StopTaskQueueServeResponse(betterproto.Message):
-    ok: bool = betterproto.bool_field(1)
-
-
 class TaskQueueServiceStub(betterproto.ServiceStub):
     async def task_queue_put(
         self,
         task_queue_put_request: "TaskQueuePutRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
@@ -193,49 +171,14 @@
             task_queue_length_request,
             TaskQueueLengthResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    async def start_task_queue_serve(
-        self,
-        start_task_queue_serve_request: "StartTaskQueueServeRequest",
-        *,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> AsyncIterator["StartTaskQueueServeResponse"]:
-        async for response in self._unary_stream(
-            "/taskqueue.TaskQueueService/StartTaskQueueServe",
-            start_task_queue_serve_request,
-            StartTaskQueueServeResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ):
-            yield response
-
-    async def stop_task_queue_serve(
-        self,
-        stop_task_queue_serve_request: "StopTaskQueueServeRequest",
-        *,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "StopTaskQueueServeResponse":
-        return await self._unary_unary(
-            "/taskqueue.TaskQueueService/StopTaskQueueServe",
-            stop_task_queue_serve_request,
-            StopTaskQueueServeResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
 
 class TaskQueueServiceBase(ServiceBase):
 
     async def task_queue_put(
         self, task_queue_put_request: "TaskQueuePutRequest"
     ) -> "TaskQueuePutResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
@@ -257,25 +200,14 @@
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
     async def task_queue_length(
         self, task_queue_length_request: "TaskQueueLengthRequest"
     ) -> "TaskQueueLengthResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
-    async def start_task_queue_serve(
-        self, start_task_queue_serve_request: "StartTaskQueueServeRequest"
-    ) -> AsyncIterator["StartTaskQueueServeResponse"]:
-        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
-        yield StartTaskQueueServeResponse()
-
-    async def stop_task_queue_serve(
-        self, stop_task_queue_serve_request: "StopTaskQueueServeRequest"
-    ) -> "StopTaskQueueServeResponse":
-        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
-
     async def __rpc_task_queue_put(
         self, stream: "grpclib.server.Stream[TaskQueuePutRequest, TaskQueuePutResponse]"
     ) -> None:
         request = await stream.recv_message()
         response = await self.task_queue_put(request)
         await stream.send_message(response)
 
@@ -309,33 +241,14 @@
         self,
         stream: "grpclib.server.Stream[TaskQueueLengthRequest, TaskQueueLengthResponse]",
     ) -> None:
         request = await stream.recv_message()
         response = await self.task_queue_length(request)
         await stream.send_message(response)
 
-    async def __rpc_start_task_queue_serve(
-        self,
-        stream: "grpclib.server.Stream[StartTaskQueueServeRequest, StartTaskQueueServeResponse]",
-    ) -> None:
-        request = await stream.recv_message()
-        await self._call_rpc_handler_server_stream(
-            self.start_task_queue_serve,
-            stream,
-            request,
-        )
-
-    async def __rpc_stop_task_queue_serve(
-        self,
-        stream: "grpclib.server.Stream[StopTaskQueueServeRequest, StopTaskQueueServeResponse]",
-    ) -> None:
-        request = await stream.recv_message()
-        response = await self.stop_task_queue_serve(request)
-        await stream.send_message(response)
-
     def __mapping__(self) -> Dict[str, grpclib.const.Handler]:
         return {
             "/taskqueue.TaskQueueService/TaskQueuePut": grpclib.const.Handler(
                 self.__rpc_task_queue_put,
                 grpclib.const.Cardinality.UNARY_UNARY,
                 TaskQueuePutRequest,
                 TaskQueuePutResponse,
@@ -360,20 +273,8 @@
             ),
             "/taskqueue.TaskQueueService/TaskQueueLength": grpclib.const.Handler(
                 self.__rpc_task_queue_length,
                 grpclib.const.Cardinality.UNARY_UNARY,
                 TaskQueueLengthRequest,
                 TaskQueueLengthResponse,
             ),
-            "/taskqueue.TaskQueueService/StartTaskQueueServe": grpclib.const.Handler(
-                self.__rpc_start_task_queue_serve,
-                grpclib.const.Cardinality.UNARY_STREAM,
-                StartTaskQueueServeRequest,
-                StartTaskQueueServeResponse,
-            ),
-            "/taskqueue.TaskQueueService/StopTaskQueueServe": grpclib.const.Handler(
-                self.__rpc_stop_task_queue_serve,
-                grpclib.const.Cardinality.UNARY_UNARY,
-                StopTaskQueueServeRequest,
-                StopTaskQueueServeResponse,
-            ),
         }
```

### Comparing `beta9-0.1.2/src/beta9/clients/volume/__init__.py` & `beta9-0.1.2rc1/src/beta9/clients/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/config.py` & `beta9-0.1.2rc1/src/beta9/config.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/logging.py` & `beta9-0.1.2rc1/src/beta9/logging.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/runner/common.py` & `beta9-0.1.2rc1/src/beta9/runner/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 class Config:
     container_id: Optional[str]
     container_hostname: Optional[str]
     stub_id: Optional[str]
     stub_type: Optional[str]
     concurrency: Optional[int]
     keep_warm_seconds: Optional[int]
-    timeout: Optional[int]
     python_version: str
     handler: str
     loader: str
     task_id: Optional[str]
     bind_port: int
 
     @classmethod
@@ -33,15 +32,14 @@
         concurrency = int(os.getenv("CONCURRENCY", 1))
         keep_warm_seconds = float(os.getenv("KEEP_WARM_SECONDS", 10))
         python_version = os.getenv("PYTHON_VERSION")
         handler = os.getenv("HANDLER")
         loader = os.getenv("LOADER")
         task_id = os.getenv("TASK_ID")
         bind_port = int(os.getenv("BIND_PORT"))
-        timeout = int(os.getenv("TIMEOUT", 180))
 
         if concurrency <= 0:
             concurrency = 1
 
         if not container_id or not stub_id:
             raise RunnerException("Invalid runner environment")
 
@@ -53,29 +51,27 @@
             concurrency=concurrency,
             keep_warm_seconds=keep_warm_seconds,
             python_version=python_version,
             handler=handler,
             loader=loader,
             task_id=task_id,
             bind_port=bind_port,
-            timeout=timeout,
         )
 
 
 config: Config = Config.load_from_env()
 
 
 def load_handler() -> Callable:
     sys.path.insert(0, USER_CODE_VOLUME)
 
     try:
         module, func = config.handler.split(":")
         target_module = importlib.import_module(module)
         method = getattr(target_module, func)
-        print(f"Handler {config.handler} loaded.")
         return method
     except BaseException:
         raise RunnerException()
 
 
 def load_loader() -> Union[Callable, None]:
     sys.path.insert(0, USER_CODE_VOLUME)
```

### Comparing `beta9-0.1.2/src/beta9/runner/container.py` & `beta9-0.1.2rc1/src/beta9/runner/container.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/runner/function.py` & `beta9-0.1.2rc1/src/beta9/runner/function.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,22 +138,21 @@
         )
 
         task_status = TaskStatus.Complete
         error = None
 
         # Invoke function
         try:
+            handler = load_handler()
             get_args_resp: FunctionGetArgsResponse = run_sync(
                 function_stub.function_get_args(FunctionGetArgsRequest(task_id=task_id)),
             )
             if not get_args_resp.ok:
                 raise InvalidFunctionArgumentsException
 
-            handler = load_handler()
-
             payload: dict = _load_args(get_args_resp.args)
             args = payload.get("args") or []
             kwargs = payload.get("kwargs") or {}
             result = handler(*args, **kwargs)
         except BaseException as exc:
             result = error = exc
             task_status = TaskStatus.Error
```

### Comparing `beta9-0.1.2/src/beta9/runner/serve.py` & `beta9-0.1.2rc1/src/beta9/runner/serve.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/runner/taskqueue.py` & `beta9-0.1.2rc1/src/beta9/runner/taskqueue.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import atexit
 import json
 import os
 import signal
 import sys
 import threading
 import time
 import traceback
@@ -30,64 +31,53 @@
 from ..exceptions import RunnerException
 from ..logging import StdoutJsonInterceptor
 from ..runner.common import config, load_handler
 from ..type import TaskExitCode, TaskStatus
 
 TASK_PROCESS_WATCHDOG_INTERVAL = 0.01
 TASK_POLLING_INTERVAL = 0.01
-TASK_MANAGER_INTERVAL = 0.1
 
 
 class TaskQueueManager:
     def __init__(self) -> None:
+        self._setup_signal_handlers()
+
+        set_start_method("spawn", force=True)
+
         # Manager attributes
         self.pid: int = os.getpid()
         self.exit_code: int = 0
-        self.shutdown_event = Event()
-
-        self._setup_signal_handlers()
-        set_start_method("spawn", force=True)
 
         # Task worker attributes
         self.task_worker_count: int = config.concurrency
         self.task_processes: List[Process] = []
         self.task_workers: List[TaskQueueWorker] = []
         self.task_worker_startup_events: List[Event] = [
             Event() for _ in range(self.task_worker_count)
         ]
         self.task_worker_watchdog_threads: List[threading.Thread] = []
 
     def _setup_signal_handlers(self):
-        if os.getpid() == self.pid:
-            signal.signal(signal.SIGTERM, self._init_shutdown)
-
-    def _init_shutdown(self, signum=None, frame=None):
-        self.shutdown_event.set()
+        signal.signal(signal.SIGTERM, self.shutdown)
 
     def run(self):
         for worker_index in range(self.task_worker_count):
             print(f"Starting task worker[{worker_index}]")
             self._start_worker(worker_index)
 
-        while not self.shutdown_event.is_set():
-            time.sleep(TASK_MANAGER_INTERVAL)
-
-        self.shutdown()
-
-    def shutdown(self):
-        print("Spinning down taskqueue")
+        for task_process in self.task_processes:
+            task_process.join()
 
-        # Terminate all worker processes
+    def shutdown(self, signum=None, frame=None):
         for task_process in self.task_processes:
             task_process.terminate()
-            task_process.join(timeout=5)
+            task_process.join()
 
         for task_process in self.task_processes:
             if task_process.is_alive():
-                print("Task process did not join within the timeout. Terminating...")
                 task_process.terminate()
                 task_process.join(timeout=0)
 
             if task_process.exitcode != 0:
                 self.exit_code = task_process.exitcode
 
     def _start_worker(self, worker_index: int):
@@ -296,11 +286,13 @@
                         monitor_task.cancel()
 
             loop.run_until_complete(_run_task())
 
 
 if __name__ == "__main__":
     tq = TaskQueueManager()
+    atexit.register(tq.shutdown)
+
     tq.run()
 
     if tq.exit_code != 0 and tq.exit_code != TaskExitCode.SigTerm:
         sys.exit(tq.exit_code)
```

### Comparing `beta9-0.1.2/src/beta9/sync.py` & `beta9-0.1.2rc1/src/beta9/sync.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/terminal.py` & `beta9-0.1.2rc1/src/beta9/terminal.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/src/beta9/type.py` & `beta9-0.1.2rc1/src/beta9/type.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.2/PKG-INFO` & `beta9-0.1.2rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: beta9
-Version: 0.1.2
+Version: 0.1.2rc1
 Summary: 
 Author: beam.cloud
 Author-email: support@beam.cloud
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asgiref (>=3.7.2,<4.0.0)
 Requires-Dist: betterproto[compiler] (==2.0.0b6)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: cloudpickle (>=3.0.0,<4.0.0)
 Requires-Dist: croniter (>=2.0.3,<3.0.0)
 Requires-Dist: fastapi (>=0.109.0,<0.110.0)
 Requires-Dist: grpcio (>=1.60.0,<2.0.0)
```

