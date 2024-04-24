# Comparing `tmp/fixinventory-plugin-azure-4.0.2.tar.gz` & `tmp/fixinventory_plugin_azure-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory-plugin-azure-4.0.2.tar", last modified: Fri Apr 12 12:16:12 2024, max compression
+gzip compressed data, was "fixinventory_plugin_azure-4.0.3.tar", last modified: Wed Apr 24 10:33:54 2024, max compression
```

## Comparing `fixinventory-plugin-azure-4.0.2.tar` & `fixinventory_plugin_azure-4.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:16:12.813783 fixinventory-plugin-azure-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-12 12:16:12.813783 fixinventory-plugin-azure-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-12 12:11:26.000000 fixinventory-plugin-azure-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:16:12.809783 fixinventory-plugin-azure-4.0.2/fix_plugin_azure/
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-12 12:11:26.000000 fixinventory-plugin-azure-4.0.2/fix_plugin_azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10591 2024-04-12 12:11:26.000000 fixinventory-plugin-azure-4.0.2/fix_plugin_azure/azure_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-04-12 12:11:26.000000 fixinventory-plugin-azure-4.0.2/fix_plugin_azure/collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-12 12:11:26.000000 fixinventory-plugin-azure-4.0.2/fix_plugin_azure/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:16:12.809783 fixinventory-plugin-azure-4.0.2/fix_plugin_azure/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:11:26.000000 fixinventory-plugin-azure-4.0.2/fix_plugin_azure/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32066 2024-04-12 12:11:26.000000 fixinventory-plugin-azure-4.0.2/fix_plugin_azure/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)   308884 2024-04-12 12:11:26.000000 fixinventory-plugin-azure-4.0.2/fix_plugin_azure/resource/compute.py
--rw-r--r--   0 runner    (1001) docker     (127)    81717 2024-04-12 12:11:26.000000 fixinventory-plugin-azure-4.0.2/fix_plugin_azure/resource/containerservice.py
--rw-r--r--   0 runner    (1001) docker     (127)    11954 2024-04-12 12:11:26.000000 fixinventory-plugin-azure-4.0.2/fix_plugin_azure/resource/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)   443338 2024-04-12 12:11:26.000000 fixinventory-plugin-azure-4.0.2/fix_plugin_azure/resource/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-12 12:11:26.000000 fixinventory-plugin-azure-4.0.2/fix_plugin_azure/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:16:12.813783 fixinventory-plugin-azure-4.0.2/fixinventory_plugin_azure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-12 12:16:12.000000 fixinventory-plugin-azure-4.0.2/fixinventory_plugin_azure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-12 12:16:12.000000 fixinventory-plugin-azure-4.0.2/fixinventory_plugin_azure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:16:12.000000 fixinventory-plugin-azure-4.0.2/fixinventory_plugin_azure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-12 12:16:12.000000 fixinventory-plugin-azure-4.0.2/fixinventory_plugin_azure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:12:34.000000 fixinventory-plugin-azure-4.0.2/fixinventory_plugin_azure.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-12 12:16:12.000000 fixinventory-plugin-azure-4.0.2/fixinventory_plugin_azure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 12:16:12.000000 fixinventory-plugin-azure-4.0.2/fixinventory_plugin_azure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-12 12:11:26.000000 fixinventory-plugin-azure-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-12 12:16:12.813783 fixinventory-plugin-azure-4.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:54.668394 fixinventory_plugin_azure-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-24 10:33:54.668394 fixinventory_plugin_azure-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-24 10:29:15.000000 fixinventory_plugin_azure-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:54.664394 fixinventory_plugin_azure-4.0.3/fix_plugin_azure/
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-24 10:29:15.000000 fixinventory_plugin_azure-4.0.3/fix_plugin_azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11410 2024-04-24 10:29:15.000000 fixinventory_plugin_azure-4.0.3/fix_plugin_azure/azure_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8796 2024-04-24 10:29:15.000000 fixinventory_plugin_azure-4.0.3/fix_plugin_azure/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-24 10:29:15.000000 fixinventory_plugin_azure-4.0.3/fix_plugin_azure/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:54.664394 fixinventory_plugin_azure-4.0.3/fix_plugin_azure/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:29:15.000000 fixinventory_plugin_azure-4.0.3/fix_plugin_azure/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32066 2024-04-24 10:29:15.000000 fixinventory_plugin_azure-4.0.3/fix_plugin_azure/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)   308884 2024-04-24 10:29:15.000000 fixinventory_plugin_azure-4.0.3/fix_plugin_azure/resource/compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81717 2024-04-24 10:29:15.000000 fixinventory_plugin_azure-4.0.3/fix_plugin_azure/resource/containerservice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11954 2024-04-24 10:29:15.000000 fixinventory_plugin_azure-4.0.3/fix_plugin_azure/resource/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)   443396 2024-04-24 10:29:15.000000 fixinventory_plugin_azure-4.0.3/fix_plugin_azure/resource/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-24 10:29:15.000000 fixinventory_plugin_azure-4.0.3/fix_plugin_azure/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:54.668394 fixinventory_plugin_azure-4.0.3/fixinventory_plugin_azure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-24 10:33:54.000000 fixinventory_plugin_azure-4.0.3/fixinventory_plugin_azure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-24 10:33:54.000000 fixinventory_plugin_azure-4.0.3/fixinventory_plugin_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:33:54.000000 fixinventory_plugin_azure-4.0.3/fixinventory_plugin_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-24 10:33:54.000000 fixinventory_plugin_azure-4.0.3/fixinventory_plugin_azure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:30:25.000000 fixinventory_plugin_azure-4.0.3/fixinventory_plugin_azure.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-24 10:33:54.000000 fixinventory_plugin_azure-4.0.3/fixinventory_plugin_azure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 10:33:54.000000 fixinventory_plugin_azure-4.0.3/fixinventory_plugin_azure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-24 10:29:15.000000 fixinventory_plugin_azure-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-24 10:33:54.668394 fixinventory_plugin_azure-4.0.3/setup.cfg
```

### Comparing `fixinventory-plugin-azure-4.0.2/PKG-INFO` & `fixinventory_plugin_azure-4.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-azure
-Version: 4.0.2
+Version: 4.0.3
 Summary: Runs collector plugins and sends the result to fixcore.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/azure
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
@@ -15,15 +15,15 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.2
+Requires-Dist: fixinventorylib==4.0.3
 Requires-Dist: retrying
 Requires-Dist: azure-identity
 Requires-Dist: azure-mgmt-resource
 
 # fix-plugin-azure
 An Azure collector plugin for Fix.
```

### Comparing `fixinventory-plugin-azure-4.0.2/fix_plugin_azure/__init__.py` & `fixinventory_plugin_azure-4.0.3/fix_plugin_azure/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import multiprocessing
 from collections import namedtuple
-from concurrent.futures import ThreadPoolExecutor, as_completed
+from concurrent.futures import as_completed, ProcessPoolExecutor
 from typing import Optional, Tuple, Any
 
 from attr import evolve
 
 from fix_plugin_azure.collector import AzureSubscriptionCollector
 from fix_plugin_azure.config import AzureConfig, AzureAccountConfig
 from fix_plugin_azure.resource.base import AzureSubscription
@@ -57,26 +57,27 @@
                 evolve(subscription, account_name=name),
                 ac,
                 self.core_feedback.with_context(cloud.id, subscription.safe_name),
                 self.task_data,
             )
             for name, ac in account_configs.items()
             for subscription in AzureSubscription.list_subscriptions(ac.credentials())
+            if ac.allowed(subscription.subscription_id)
         }
         args = list(args_by_subscription_id.values())
 
         # Send initial progress
         progress = ProgressTree(self.cloud)
         for sub in args:
             progress.add_progress(ProgressDone(sub.subscription.subscription_id, 0, 1))
             log.debug(f"Found {sub.subscription.subscription_id}")
         self.core_feedback.progress(progress)
 
         # Collect all subscriptions
-        with ThreadPoolExecutor(max_workers=config.subscription_pool_size) as executor:
+        with ProcessPoolExecutor(max_workers=config.subscription_pool_size) as executor:
             wait_for = [executor.submit(collect_in_process, sub, self.task_data) for sub in args]
             for future in as_completed(wait_for):
                 subscription, graph = future.result()
                 progress.add_progress(ProgressDone(subscription.subscription_id, 1, 1, path=[cloud.id]))
                 if not isinstance(graph, Graph):
                     log.debug(f"Skipping subscription graph of invalid type {type(graph)}")
                     continue
@@ -86,16 +87,20 @@
 
 def collect_account_proxy(subscription_collector_arg: AzureSubscriptionArg, queue: multiprocessing.Queue) -> None:  # type: ignore
     collector_initializer()
     config, cloud, subscription, account_config, core_feedback, task_data = subscription_collector_arg
     subscription_collector = AzureSubscriptionCollector(
         config, cloud, subscription, account_config.credentials(), core_feedback, task_data
     )
-    subscription_collector.collect()
-    queue.put((subscription_collector_arg.subscription, subscription_collector.graph))
+    try:
+        subscription_collector.collect()
+        queue.put((subscription_collector_arg.subscription, subscription_collector.graph))
+    except Exception as e:
+        log.exception(f"Error collecting subscription {subscription.subscription_id}: {e}. Give up.")
+        queue.put((subscription_collector_arg.subscription, None))  # signal done
 
 
 def collect_in_process(
     subscription_collector_arg: AzureSubscriptionArg, task_data: Optional[Json]
 ) -> Tuple[AzureSubscription, Graph]:
     ctx = multiprocessing.get_context("spawn")
     queue = ctx.Queue()
```

### Comparing `fixinventory-plugin-azure-4.0.2/fix_plugin_azure/azure_client.py` & `fixinventory_plugin_azure-4.0.3/fix_plugin_azure/azure_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod
 from typing import List, MutableMapping, Optional, Any, Union, Dict
 
-from attr import define
+from attr import define, field
 from retrying import retry
 from azure.core.exceptions import (
     ClientAuthenticationError,
     ResourceNotFoundError,
     map_error,
     HttpResponseError,
 )
@@ -17,14 +17,15 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.resource import ResourceManagementClient
 from azure.mgmt.resource.resources._serialization import Serializer
 from azure.mgmt.resource.resources.models import GenericResource
 
 from fix_plugin_azure.config import AzureCredentials
+from fixlib.core.actions import CoreFeedback, ErrorAccumulator
 from fixlib.types import Json
 
 log = logging.getLogger("fix.plugins.azure")
 
 
 class MetricRequestError(HttpResponseError):
     """Error raised when there's an issue retrieving metric data from the Azure API."""
@@ -51,14 +52,15 @@
     service: str
     version: str
     path: str
     path_parameters: List[str] = []
     query_parameters: List[str] = []
     access_path: Optional[str] = None
     expect_array: bool = False
+    expected_error_codes: List[str] = field(factory=list)
 
 
 class AzureClient(ABC):
     @abstractmethod
     def list(self, spec: AzureApiSpec, **kwargs: Any) -> List[Json]:
         pass
 
@@ -78,31 +80,39 @@
     def delete_resource_tag(self, tag_name: str, resource_id: str) -> bool:
         pass
 
     @staticmethod
     def __create_management_client(
         credential: AzureCredentials,
         subscription_id: str,
+        core_feedback: Optional[CoreFeedback] = None,
+        error_accumulator: Optional[ErrorAccumulator] = None,
         resource_group: Optional[str] = None,
     ) -> AzureClient:
-        return AzureResourceManagementClient(credential, subscription_id, resource_group)
+        return AzureResourceManagementClient(
+            credential, subscription_id, resource_group, core_feedback, error_accumulator
+        )
 
     create = __create_management_client
 
 
 class AzureResourceManagementClient(AzureClient):
     def __init__(
         self,
         credential: AzureCredentials,
         subscription_id: str,
         location: Optional[str] = None,
+        core_feedback: Optional[CoreFeedback] = None,
+        accumulator: Optional[ErrorAccumulator] = None,
     ) -> None:
         self.credential = credential
         self.subscription_id = subscription_id
         self.location = location
+        self.core_feedback = core_feedback
+        self.accumulator = accumulator or ErrorAccumulator()
         self.client = ResourceManagementClient(self.credential, self.subscription_id)
 
     def list(self, spec: AzureApiSpec, **kwargs: Any) -> List[Json]:
         result = self._list_with_retry(spec, **kwargs)
         if result is None:
             return []
         return result  # type: ignore
@@ -171,18 +181,22 @@
         except ClientAuthenticationError as e:
             log.error(f"[Azure] Call to Azure API is not authorized!: {e}")
             return None
         except HttpResponseError as e:
             if error := e.error:
                 if error.code == "NoRegisteredProviderFound":
                     return None  # API not available in this region
+                elif error.code in spec.expected_error_codes:
+                    return None
                 elif error.code == "BadRequest" and spec.service == "metric":
                     raise MetricRequestError from e
-            log.warning(f"[Azure] Error encountered while requesting resource: {e}")
-            raise e
+                code = error.code or "Unknown"
+                self.accumulator.add_error(False, code, spec.service, spec.path, str(e), self.location)
+            log.warning(f"[Azure] Client Error: status={e.status_code}, error={e.error}, message={e}")
+            return None
         except Exception as e:
             log.warning(f"[Azure] called service={spec.service}: hit unexpected error: {e}", exc_info=e)
             return None
 
     # noinspection PyProtectedMember
     def _call(self, spec: AzureApiSpec, **kwargs: Any) -> List[Json]:
         ser = Serializer()
@@ -267,8 +281,8 @@
         request = HttpRequest(method="GET", url=url, params=params, headers=headers)
         pipeline_response: PipelineResponse = self.client._client._pipeline.run(request, stream=False)  # type: ignore
         response = pipeline_response.http_response
 
         return response
 
     def for_location(self, location: str) -> AzureClient:
-        return AzureClient.create(self.credential, self.subscription_id, location)
+        return AzureClient.create(self.credential, self.subscription_id, self.core_feedback, self.accumulator, location)
```

### Comparing `fixinventory-plugin-azure-4.0.2/fix_plugin_azure/collector.py` & `fixinventory_plugin_azure-4.0.3/fix_plugin_azure/collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     AzureExpressRoutePortsLocation,
     AzureNetworkVirtualApplianceSku,
     AzureUsage,
     resources as network_resources,
 )
 from fix_plugin_azure.resource.containerservice import resources as aks_resources
 from fixlib.baseresources import Cloud, GraphRoot
-from fixlib.core.actions import CoreFeedback
+from fixlib.core.actions import CoreFeedback, ErrorAccumulator
 from fixlib.graph import Graph
 from fixlib.json import value_in_path
 from fixlib.threading import ExecutorQueue, GatherFutures
 from fixlib.types import Json
 
 log = logging.getLogger("fix.plugin.azure")
 
@@ -68,15 +68,21 @@
     def collect(self) -> None:
         with ThreadPoolExecutor(
             thread_name_prefix=f"azure_{self.subscription.subscription_id}",
             max_workers=self.config.resource_pool_size,
         ) as executor:
             self.core_feedback.progress_done(self.subscription.subscription_id, 0, 1, context=[self.cloud.id])
             queue = ExecutorQueue(executor, "azure_collector")
-            client = AzureClient.create(self.credentials, self.subscription.subscription_id)
+            error_accumulator = ErrorAccumulator()
+            client = AzureClient.create(
+                self.credentials,
+                self.subscription.subscription_id,
+                core_feedback=self.core_feedback,
+                error_accumulator=error_accumulator,
+            )
 
             def get_last_run() -> Optional[datetime]:
                 td = self.task_data
                 if not td:
                     return None
                 if timestamp := value_in_path(self.task_data, ["timing", td.get("step", ""), "started_at"]):
                     return datetime.fromtimestamp(timestamp, timezone.utc)
@@ -119,15 +125,16 @@
             # post process nodes
             for node, data in list(self.graph.nodes(data=True)):
                 if isinstance(node, AzureResource):
                     node.after_collect(builder, data.get("source", {}))
 
             # delete unnecessary nodes after all work is completed
             self.after_collect_filter()
-
+            # report all accumulated errors
+            error_accumulator.report_all(self.core_feedback)
             self.core_feedback.progress_done(self.subscription.subscription_id, 1, 1, context=[self.cloud.id])
             log.info(f"[Azure:{self.subscription.safe_name}] Collecting resources done.")
 
     def collect_resource_list(
         self, name: str, builder: GraphBuilder, resources: List[Type[AzureResource]]
     ) -> Future[None]:
         def collect_resource(clazz: Type[AzureResource]) -> None:
```

### Comparing `fixinventory-plugin-azure-4.0.2/fix_plugin_azure/config.py` & `fixinventory_plugin_azure-4.0.3/fix_plugin_azure/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,21 @@
                 tenant_id=cs.tenant_id,
                 client_id=cs.client_id,
                 client_secret=cs.client_secret,
             )
 
         return DefaultAzureCredential()
 
+    def allowed(self, subscription_id: str) -> bool:
+        if self.subscriptions is not None:
+            return subscription_id in self.subscriptions
+        if self.exclude_subscriptions is not None:
+            return subscription_id not in self.exclude_subscriptions
+        return True
+
 
 @define
 class AzureConfig:
     kind: ClassVar[str] = "azure"
 
     subscription_pool_size: int = field(
         default=4, metadata={"description": "Number of concurrent subscriptions to collect."}
```

### Comparing `fixinventory-plugin-azure-4.0.2/fix_plugin_azure/resource/base.py` & `fixinventory_plugin_azure-4.0.3/fix_plugin_azure/resource/base.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-azure-4.0.2/fix_plugin_azure/resource/compute.py` & `fixinventory_plugin_azure-4.0.3/fix_plugin_azure/resource/compute.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-azure-4.0.2/fix_plugin_azure/resource/containerservice.py` & `fixinventory_plugin_azure-4.0.3/fix_plugin_azure/resource/containerservice.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-azure-4.0.2/fix_plugin_azure/resource/metrics.py` & `fixinventory_plugin_azure-4.0.3/fix_plugin_azure/resource/metrics.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-azure-4.0.2/fix_plugin_azure/resource/network.py` & `fixinventory_plugin_azure-4.0.3/fix_plugin_azure/resource/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -4697,14 +4697,15 @@
         service="network",
         version="2023-05-01",
         path="/subscriptions/{subscriptionId}/providers/Microsoft.Network/locations/{location}/usages",
         path_parameters=["location", "subscriptionId"],
         query_parameters=["api-version"],
         access_path="value",
         expect_array=True,
+        expected_error_codes=["SubscriptionHasNoUsages"],
     )
     mapping: ClassVar[Dict[str, Bender]] = {
         "id": S("id"),
         "tags": S("tags", default={}),
         "name": S("name", "value"),
         "usage_name": S("name") >> Bend(AzureUsageName.mapping),
         "current_value": S("currentValue"),
```

### Comparing `fixinventory-plugin-azure-4.0.2/fix_plugin_azure/utils.py` & `fixinventory_plugin_azure-4.0.3/fix_plugin_azure/utils.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-azure-4.0.2/fixinventory_plugin_azure.egg-info/PKG-INFO` & `fixinventory_plugin_azure-4.0.3/fixinventory_plugin_azure.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-azure
-Version: 4.0.2
+Version: 4.0.3
 Summary: Runs collector plugins and sends the result to fixcore.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/azure
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
@@ -15,15 +15,15 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.2
+Requires-Dist: fixinventorylib==4.0.3
 Requires-Dist: retrying
 Requires-Dist: azure-identity
 Requires-Dist: azure-mgmt-resource
 
 # fix-plugin-azure
 An Azure collector plugin for Fix.
```

### Comparing `fixinventory-plugin-azure-4.0.2/fixinventory_plugin_azure.egg-info/SOURCES.txt` & `fixinventory_plugin_azure-4.0.3/fixinventory_plugin_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-azure-4.0.2/pyproject.toml` & `fixinventory_plugin_azure-4.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fixinventory-plugin-azure"
-version = "4.0.2"
+version = "4.0.3"
 authors = [{name="Some Engineering Inc."}]
 description = "Runs collector plugins and sends the result to fixcore."
 license = { text="AGPLv3" }
 requires-python = ">=3.11"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "fixinventorylib==4.0.2",
+    "fixinventorylib==4.0.3",
     "retrying",
     "azure-identity",
     "azure-mgmt-resource"
 ]
 
 [project.entry-points."fix.plugins"]
 azure = "fix_plugin_azure:AzureCollectorPlugin"
```

