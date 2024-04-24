# Comparing `tmp/py_infraflow_cdk-0.1.9.8.9.0.tar.gz` & `tmp/py_infraflow_cdk-0.1.9.8.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_infraflow_cdk-0.1.9.8.9.0.tar", max compression
+gzip compressed data, was "py_infraflow_cdk-0.1.9.8.9.1.tar", max compression
```

## Comparing `py_infraflow_cdk-0.1.9.8.9.0.tar` & `py_infraflow_cdk-0.1.9.8.9.1.tar`

### file list

```diff
@@ -1,37 +1,39 @@
--rw-r--r--   0        0        0      337 2024-01-24 18:03:42.816211 py_infraflow_cdk-0.1.9.8.9.0/README.md
--rw-r--r--   0        0        0        0 2024-01-22 17:24:55.856613 py_infraflow_cdk-0.1.9.8.9.0/infraflow/__init__.py
--rw-r--r--   0        0        0      240 2024-01-22 17:24:55.856719 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/__init__.py
--rw-r--r--   0        0        0        0 2024-01-22 17:24:55.856794 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/_step_functions/__init__.py
--rw-r--r--   0        0        0     1329 2024-01-22 17:24:55.856883 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/_step_functions/core.py
--rw-r--r--   0        0        0     1261 2024-01-22 17:24:55.856942 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/_step_functions/patterns.py
--rw-r--r--   0        0        0      280 2024-01-22 17:24:55.857004 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/api_gateway.py
--rw-r--r--   0        0        0     6645 2024-02-28 20:33:11.558797 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/app_patterns/express_default_dlq_processor.py
--rw-r--r--   0        0        0     9928 2024-03-20 16:31:56.830041 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/app_patterns/standard.py
--rw-r--r--   0        0        0      156 2024-01-22 17:24:55.857163 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/arns.py
--rw-r--r--   0        0        0        0 2024-01-22 17:24:55.857224 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/core/__init__.py
--rw-r--r--   0        0        0      364 2024-01-22 17:24:55.857292 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/core/component_service.py
--rw-r--r--   0        0        0      316 2024-01-22 17:24:55.857349 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/core/construct.py
--rw-r--r--   0        0        0     5168 2024-03-20 16:31:56.831033 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/core/environment.py
--rw-r--r--   0        0        0     1020 2024-01-24 18:03:42.816662 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/core/service_stage.py
--rw-r--r--   0        0        0      367 2024-02-19 16:57:57.498391 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/core/utils.py
--rw-r--r--   0        0        0     8940 2024-03-21 16:56:06.915768 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/docker.py
--rw-r--r--   0        0        0     8184 2024-02-19 16:53:56.961586 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/events.py
--rw-r--r--   0        0        0      139 2024-01-22 17:24:55.857712 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/iam/__init__.py
--rw-r--r--   0        0        0   533095 2024-01-24 18:03:42.817968 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/iam/_actions.py
--rw-r--r--   0        0        0   249582 2024-01-22 17:24:55.859417 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/iam/action_groups.py
--rw-r--r--   0        0        0   108710 2024-01-22 17:24:55.859750 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/iam/actions
--rw-r--r--   0        0        0     4943 2024-01-22 17:24:55.859832 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/iam/base.py
--rw-r--r--   0        0        0        0 2024-03-20 16:31:56.831151 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/instrumentation/__init__.py
--rw-r--r--   0        0        0     5116 2024-03-20 16:31:56.831360 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/instrumentation/docker.py
--rw-r--r--   0        0        0     8529 2024-03-20 17:54:18.876768 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/instrumentation/lambdas.py
--rw-r--r--   0        0        0     5600 2024-03-20 16:31:56.831629 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/instrumentation/queues.py
--rw-r--r--   0        0        0     6202 2024-03-20 17:21:29.663934 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/lambdas.py
--rw-r--r--   0        0        0      349 2024-02-28 20:32:26.259456 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/queue.py
--rw-r--r--   0        0        0        0 2024-01-22 17:24:55.859986 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/sg/__init__.py
--rw-r--r--   0        0        0     3481 2024-01-24 18:03:42.818220 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/sg/patterns.py
--rw-r--r--   0        0        0      715 2024-01-24 18:03:42.818283 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/sg/ports.py
--rw-r--r--   0        0        0      629 2024-01-22 17:24:55.860118 py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/sg/tier_maps.py
--rw-r--r--   0        0        0      141 2024-01-24 18:03:42.818392 py_infraflow_cdk-0.1.9.8.9.0/infraflow/priv_utils/__init__.py
--rw-r--r--   0        0        0      154 2024-01-22 17:24:55.860264 py_infraflow_cdk-0.1.9.8.9.0/infraflow/util.py
--rw-r--r--   0        0        0      687 2024-03-21 17:02:41.552748 py_infraflow_cdk-0.1.9.8.9.0/pyproject.toml
--rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 py_infraflow_cdk-0.1.9.8.9.0/PKG-INFO
+-rw-r--r--   0        0        0      337 2024-01-24 18:03:42.816211 py_infraflow_cdk-0.1.9.8.9.1/README.md
+-rw-r--r--   0        0        0        0 2024-01-22 17:24:55.856613 py_infraflow_cdk-0.1.9.8.9.1/infraflow/__init__.py
+-rw-r--r--   0        0        0      240 2024-01-22 17:24:55.856719 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-22 17:24:55.856794 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/_step_functions/__init__.py
+-rw-r--r--   0        0        0     1329 2024-01-22 17:24:55.856883 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/_step_functions/core.py
+-rw-r--r--   0        0        0     1261 2024-01-22 17:24:55.856942 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/_step_functions/patterns.py
+-rw-r--r--   0        0        0      280 2024-01-22 17:24:55.857004 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/api_gateway.py
+-rw-r--r--   0        0        0     7248 2024-04-11 23:31:09.971668 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/app_patterns/express_default_dlq_processor.py
+-rw-r--r--   0        0        0    12703 2024-04-24 21:30:34.435023 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/app_patterns/standard.py
+-rw-r--r--   0        0        0      156 2024-01-22 17:24:55.857163 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/arns.py
+-rw-r--r--   0        0        0        0 2024-01-22 17:24:55.857224 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/core/__init__.py
+-rw-r--r--   0        0        0      364 2024-01-22 17:24:55.857292 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/core/component_service.py
+-rw-r--r--   0        0        0      316 2024-01-22 17:24:55.857349 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/core/construct.py
+-rw-r--r--   0        0        0     5168 2024-03-20 16:31:56.831033 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/core/environment.py
+-rw-r--r--   0        0        0     1020 2024-01-24 18:03:42.816662 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/core/service_stage.py
+-rw-r--r--   0        0        0      367 2024-02-19 16:57:57.498391 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/core/utils.py
+-rw-r--r--   0        0        0    10311 2024-04-11 23:31:09.972747 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/docker.py
+-rw-r--r--   0        0        0     8184 2024-02-19 16:53:56.961586 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/events.py
+-rw-r--r--   0        0        0      139 2024-01-22 17:24:55.857712 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/iam/__init__.py
+-rw-r--r--   0        0        0   533095 2024-01-24 18:03:42.817968 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/iam/_actions.py
+-rw-r--r--   0        0        0   249582 2024-01-22 17:24:55.859417 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/iam/action_groups.py
+-rw-r--r--   0        0        0   108710 2024-01-22 17:24:55.859750 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/iam/actions
+-rw-r--r--   0        0        0     4943 2024-01-22 17:24:55.859832 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/iam/base.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:31:56.831151 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/instrumentation/__init__.py
+-rw-r--r--   0        0        0     1376 2024-04-11 23:31:09.973506 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/instrumentation/alarms.py
+-rw-r--r--   0        0        0     5936 2024-04-11 23:31:09.974012 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/instrumentation/docker.py
+-rw-r--r--   0        0        0     7304 2024-04-11 23:31:09.974549 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/instrumentation/lambdas.py
+-rw-r--r--   0        0        0     1704 2024-04-11 23:31:09.974803 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/instrumentation/metrics.py
+-rw-r--r--   0        0        0     4435 2024-04-11 23:31:09.975272 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/instrumentation/queues.py
+-rw-r--r--   0        0        0     6208 2024-04-11 23:31:09.976357 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/lambdas.py
+-rw-r--r--   0        0        0      349 2024-02-28 20:32:26.259456 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/queue.py
+-rw-r--r--   0        0        0        0 2024-01-22 17:24:55.859986 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/sg/__init__.py
+-rw-r--r--   0        0        0     3481 2024-01-24 18:03:42.818220 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/sg/patterns.py
+-rw-r--r--   0        0        0      715 2024-01-24 18:03:42.818283 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/sg/ports.py
+-rw-r--r--   0        0        0      629 2024-01-22 17:24:55.860118 py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/sg/tier_maps.py
+-rw-r--r--   0        0        0      141 2024-01-24 18:03:42.818392 py_infraflow_cdk-0.1.9.8.9.1/infraflow/priv_utils/__init__.py
+-rw-r--r--   0        0        0      154 2024-01-22 17:24:55.860264 py_infraflow_cdk-0.1.9.8.9.1/infraflow/util.py
+-rw-r--r--   0        0        0      687 2024-04-24 21:31:16.494614 py_infraflow_cdk-0.1.9.8.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 py_infraflow_cdk-0.1.9.8.9.1/PKG-INFO
```

### Comparing `py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/_step_functions/core.py` & `py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/_step_functions/core.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/_step_functions/patterns.py` & `py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/_step_functions/patterns.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/app_patterns/express_default_dlq_processor.py` & `py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/app_patterns/express_default_dlq_processor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import copy
 import datetime
 from enum import Enum
-from typing import Union
+from typing import Union, Optional
 
 from aws_cdk import Duration
+from aws_cdk.aws_ecs_patterns import QueueProcessingFargateService
 from aws_cdk.aws_sqs import Queue
 from constructs import Construct
 
 from infraflow.cdk.docker import EcsCluster, add_queue_environment_variables, ContainerSize, ContainerImage, \
     ContainerInstanceInfo
 from infraflow.cdk.events import Event
-from infraflow.cdk.lambdas import LambdaContext
+from infraflow.cdk.lambdas import LambdaContext, QueueFunctionConstruct
 from infraflow.cdk.queue import QueueSubscription
 
 
 class PROCESSOR_TYPE(Enum):
     LAMBDA_PYTHON = 1
     ECS_DOCKER = 2
 
@@ -71,15 +72,15 @@
         self.max_retries = max_retries
         self.environment = copy.copy(container.environment)
         self.environment['BATCH_SIZE'] = str(subscription.batch_size)
         self.environment['MAX_RETRIES'] = str(max_retries)
         self.command = container.command
 
 
-class DualPriorityResilientProcessor(Construct):
+class DualPriorityResilientJob(Construct):
     def __init__(
             self,
             scope: Construct,
             construct_id: str,
             event: Event,
             lambda_context: LambdaContext,
             ecs_cluster: EcsCluster,
@@ -94,46 +95,56 @@
         self.lambda_context = lambda_context
         self.express_event = copy.copy(event).express_only() if express_processor else None
         self.default_event = copy.copy(event).non_express() if express_processor else copy.copy(event)
         self.default_processor = default_processor
         self.express_processor = express_processor
         # self.retry_processor = retry_processor
         self.dead_letter_processor = dead_letter_processor
+        self.express_ecs: Optional[QueueProcessingFargateService] = None
+        self.default_ecs: Optional[QueueProcessingFargateService] = None
+        self.express_lambda: Optional[QueueFunctionConstruct] = None
+        self.default_lambda: Optional[QueueFunctionConstruct] = None
+        self.dlq = None
 
     def create_resources(self):
         if isinstance(self.dead_letter_processor, LambdaPythonProcessorConfig):
             dead_letter_processor = copy.copy(self.dead_letter_processor)
             dead_letter_processor.max_concurrency = 0
-            dlq = self.create_lambda_processor(dead_letter_processor, 'DeadLetter')
+            dlq = self.create_lambda_processor(dead_letter_processor, 'DeadLetter').queue
         elif isinstance(self.dead_letter_processor, EcsDockerProcessorConfig):
             dlq = Queue(self, 'DeadLetterQueue')
         else:
             dlq = None
+        self.dlq = dlq
 
         # if isinstance(self.retry_processor, LambdaPythonProcessorConfig):
         #     retry_qf = self.create_lambda_processor(self.retry_processor, 'Retry', dlq=dlq)
         #     retry_queue = retry_qf.queue
         # elif isinstance(self.retry_processor, EcsDockerProcessorConfig):
         #     retry_queue = Queue(self, 'RetryQueue')
         # else:
         #     retry_queue = None
 
         if isinstance(self.default_processor, LambdaPythonProcessorConfig):
             default_qf = self.create_lambda_processor(self.default_processor, 'Default', dlq=dlq)
             self.default_event.subscribe(default_qf)
+            self.default_lambda = default_qf
         elif isinstance(self.default_processor, EcsDockerProcessorConfig):
             queue, service = self.create_ecs_processor(self.default_processor, 'Default')
             self.default_event.subscribe(queue)
+            self.default_ecs = service
 
         if isinstance(self.express_processor, LambdaPythonProcessorConfig):
             express_qf = self.create_lambda_processor(self.express_processor, 'Express', dlq=dlq)
             self.express_event.subscribe(express_qf)
+            self.express_lambda = express_qf
         elif isinstance(self.express_processor, EcsDockerProcessorConfig):
             queue, service = self.create_ecs_processor(self.express_processor, 'Express')
             self.express_event.subscribe(queue)
+            self.express_lambda = service
 
     def create_lambda_processor(self, processor_config: LambdaPythonProcessorConfig, suffix, dlq):
         return self.lambda_context.queued_function(
             processor_config.handler,
             timeout=processor_config.timeout,
             max_concurrency=processor_config.max_concurrency,
             batch_size=processor_config.batch_size,
```

### Comparing `py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/app_patterns/standard.py` & `py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/app_patterns/standard.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-from typing import Optional, Any
+from typing import Optional, Any, Union
 
 from aws_cdk import App, aws_sns, IResource
 import aws_cdk.aws_lambda as aws_lambda
 import aws_cdk.aws_apigateway as apigateway
 import aws_cdk.aws_events as aws_events
 from aws_cdk.aws_ec2 import InterfaceVpcEndpointAwsService
+from aws_cdk.aws_ecs import FargateService
+from aws_cdk.aws_ecs_patterns import QueueProcessingFargateService
 from aws_cdk.aws_iam import IRole, Role, ServicePrincipal, ManagedPolicy, PolicyStatement, Effect
+from aws_cdk.aws_lambda import Function
+from aws_cdk.aws_sqs import Queue
 from aws_cdk.aws_stepfunctions import IStateMachine
+from constructs import Construct
 
 from infraflow.cdk import ServiceStageStack, EnvConfig
-from infraflow.cdk.app_patterns.express_default_dlq_processor import ProcessorConfig, DualPriorityResilientProcessor, \
+from infraflow.cdk.app_patterns.express_default_dlq_processor import ProcessorConfig, DualPriorityResilientJob, \
     PROCESSOR_TYPE
 from infraflow.cdk.core.environment import DEFAULT_INTERFACE_SERVICES
 from infraflow.cdk.docker import EcsCluster
 from infraflow.cdk.events import EventBridgeEvents, InfraflowEventBus, SnsEvents, Event
 from infraflow.cdk.iam import PolicyBuilder, IamAction
-from infraflow.cdk.lambdas import LambdaContext
+from infraflow.cdk.lambdas import LambdaContext, QueueFunctionConstruct
 from infraflow.cdk.sg.patterns import Tiered
 from infraflow.cdk.sg.ports import port_for
 
 
 class StandardServiceStage(ServiceStageStack):
     # noinspection PyDefaultArgument
     def __init__(self,
@@ -124,24 +129,51 @@
     def ecs_cluster(self) -> EcsCluster:
         self.use_ecs()
         return self._ecs_cluster
 
     def handle_event(self, event: Event, default: ProcessorConfig, express: ProcessorConfig = None):
         uses_docker = express.type == PROCESSOR_TYPE.ECS_DOCKER or default.type == PROCESSOR_TYPE.ECS_DOCKER
         uses_lambda = express.type == PROCESSOR_TYPE.LAMBDA_PYTHON or default.type == PROCESSOR_TYPE.LAMBDA_PYTHON
-        processor = DualPriorityResilientProcessor(
+        job = DualPriorityResilientJob(
             default_processor=default,
             express_processor=express,
             ecs_cluster=self.ecs_cluster if uses_docker else None,
             lambda_context=self.lambda_context if uses_lambda else None,
             event=event,
             construct_id=event.id+"Processor",
             scope=self
         )
-        processor.create_resources()
+        job.create_resources()
+        return job
+
+    def instrumentation_for_lambda(self, resource: Union[Function, QueueFunctionConstruct]):
+        if isinstance(resource, Function):
+            return self.lambda_context.lambda_instrumentation[resource]
+        elif isinstance(resource, QueueFunctionConstruct):
+            return self.lambda_context.lambda_instrumentation[resource.function]
+        else:
+            raise ValueError("")
+
+    def instrumentation_for_queue(self, resource: Union[Queue, QueueFunctionConstruct, QueueProcessingFargateService]):
+        if isinstance(resource, Queue):
+            return self.lambda_context.queue_instrumentation[resource] or self.ecs_cluster.queue_instrumentation[resource]
+        elif isinstance(resource, QueueFunctionConstruct):
+            return self.lambda_context.queue_instrumentation[resource.queue]
+        elif isinstance(resource, QueueProcessingFargateService):
+            return self.ecs_cluster.queue_instrumentation[resource.sqs_queue]
+        else:
+            raise ValueError("")
+
+    def instrumentation_for_ecs_service(self, resource: Union[FargateService, QueueProcessingFargateService]):
+        if isinstance(resource, FargateService):
+            return self.ecs_cluster.service_instrumentation[resource]
+        elif isinstance(resource, QueueProcessingFargateService):
+            return self.ecs_cluster.service_instrumentation[resource.service]
+        else:
+            raise ValueError("")
 
     def use_ecs(self):
         if not self._ecs_execution_role:
             self._ecs_execution_role = Role(self, "EcsExecRole", assumed_by=ServicePrincipal("ecs.amazonaws.com"))
             self._ecs_execution_role.add_managed_policy(
                 self.managed_policy("EcsTaskExecutionPolicy", name="AmazonECSTaskExecutionRolePolicy")
             )
@@ -158,25 +190,37 @@
             self._ecs_execution_role.assume_role_policy.add_statements(
                 PolicyStatement(
                     effect=Effect.ALLOW,
                     actions=['sts:AssumeRole'],
                     principals=[ServicePrincipal("ecs-tasks.amazonaws.com")]
                 )
             )
+            self._ecs_execution_role.add_to_policy(
+                PolicyStatement(
+                    effect=Effect.ALLOW,
+                    resources=['*'],
+                    actions=['ssm:GetParameters',
+                             'ssm:GetParameter',
+                             'ssm:GetParametersByPath',
+                             'secretsmanager:GetSecretValue',
+                             'kms:Decrypt']
+                )
+            ) ## 04.24 -> allow ecs execution: ssm:GetParameters, secretsmanager:GetSecretValue AND kms:Decrypt
 
         self._ecs_cluster = self._ecs_cluster or EcsCluster(
             self,
             "EcsCluster",
             execution_role=self._ecs_execution_role,
             task_role=self.app_role
         )
         ecr_required_endpoints = [
             InterfaceVpcEndpointAwsService.ECR,
             InterfaceVpcEndpointAwsService.ECR_DOCKER,
-            InterfaceVpcEndpointAwsService.SECRETS_MANAGER
+            InterfaceVpcEndpointAwsService.SECRETS_MANAGER,
+            InterfaceVpcEndpointAwsService.S3
         ]
         for endpoint in ecr_required_endpoints:
             if endpoint not in self.vpc_endpoint_services:
                 self.vpc_endpoint_services.append(endpoint)
 
 
     def use_monolith_lambda_api(self, handler):
@@ -219,14 +263,26 @@
             policy = PolicyBuilder()
             policy.allow_resource(resource).for_actions(actions)
             self.app_role.attach_inline_policy(policy.build_cdk_policy(self, f"{name}Policy"))
 
     @property
     def app_role(self) -> IRole:
         self._app_role = self._app_role or Role(self, 'Role', assumed_by=ServicePrincipal("lambda.amazonaws.com"))
+        self._app_role.add_to_policy(
+            PolicyStatement(
+                effect=Effect.ALLOW,
+                resources=['*'],
+                actions=['ssm:GetParameters',
+                         'ssm:GetParameter',
+                         'ssm:GetParametersByPath',
+                         'secretsmanager:GetSecretValue',
+                         'kms:Decrypt']
+            )
+        )  ## 04.24 -> allow ecs execution: ssm:GetParameters, secretsmanager:GetSecretValue AND kms:Decrypt
+
         self._app_role.assume_role_policy.add_statements(
             PolicyStatement(
                 effect=Effect.ALLOW,
                 actions=['sts:AssumeRole'],
                 principals=[ServicePrincipal("ecs.amazonaws.com")]
             )
         )
```

### Comparing `py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/core/environment.py` & `py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/core/environment.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/core/service_stage.py` & `py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/core/service_stage.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/events.py` & `py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/events.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/iam/_actions.py` & `py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/iam/_actions.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/iam/action_groups.py` & `py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/iam/action_groups.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/iam/actions` & `py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/iam/actions`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/iam/base.py` & `py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/iam/base.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/instrumentation/docker.py` & `py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/instrumentation/docker.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,117 +1,131 @@
 from datetime import timedelta
 from typing import Union
 
 from aws_cdk import Duration
 from aws_cdk.aws_cloudwatch import ComparisonOperator, TreatMissingData, GraphWidget
 from aws_cdk.aws_ecs import FargateService
+from aws_cdk.aws_logs import MetricFilter, FilterPattern, LogGroup
+from constructs import Construct
 
 from infraflow.cdk.core.utils import to_duration
+from infraflow.cdk.instrumentation.alarms import AlarmsBase
+from infraflow.cdk.instrumentation.metrics import InfraflowMetric
 
 
 class EcsServiceMetrics:
-    def __init__(self, ecs_service: FargateService):
+    def __init__(self, ecs_service: FargateService, log_group: LogGroup, scope: Construct=None):
+        self.log_group = log_group
         self.ecs_service = ecs_service
+        self.scope = ecs_service.stack if scope is None else scope
 
-    def cpu_ave(self, period):
-        return self.ecs_service.metric_cpu_utilization(statistic="average", period=to_duration(period))
-
-    def cpu_min(self, period):
-        return self.ecs_service.metric_cpu_utilization(statistic="min", period=to_duration(period))
-
-    def cpu_max(self, period):
-        return self.ecs_service.metric_cpu_utilization(statistic="max", period=to_duration(period))
-
-    def memory_ave(self, period):
-        return self.ecs_service.metric_memory_utilization(statistic="average", period=to_duration(period))
-
-    def memory_min(self, period):
-        return self.ecs_service.metric_memory_utilization(statistic="min", period=to_duration(period))
+    @property
+    def cpu(self) -> InfraflowMetric:
+        return InfraflowMetric(self.ecs_service.metric_cpu_utilization())
+
+    @property
+    def memory(self) -> InfraflowMetric:
+        return InfraflowMetric(self.ecs_service.metric_memory_utilization())
+
+    def log_filter(self, id: str, metric_name: str, metric_value: str, filter_pattern: FilterPattern):
+        return MetricFilter(
+            self.ecs_service,
+            id,
+            log_group=self.log_group,
+            metric_namespace=self.ecs_service.stack.stack_name,
+            metric_name=metric_name,
+            filter_pattern=filter_pattern,
+            metric_value=metric_value
+        )
 
-    def memory_max(self, period):
-        return self.ecs_service.metric_memory_utilization(statistic="max", period=to_duration(period))
 
-class EcsServiceAlarms:
-    def __init__(self, ecs_service: FargateService):
+class EcsServiceAlarms(AlarmsBase):
+    def __init__(self, ecs_service: FargateService, name: str = None, scope: Construct = None):
+        super().__init__(name or ecs_service.service_name, ecs_service, scope or ecs_service.stack)
         self.ecs_service = ecs_service
         self.metrics = EcsServiceMetrics(ecs_service)
+        self.scope = ecs_service.stack if scope is None else scope
 
     def cpu_over_threshold(self, over_timespan: Union[int, timedelta, Duration], evaluation_periods: int, threshold: float):
-        return self.metrics.cpu_ave(period=over_timespan).create_alarm(
-            alarm_name="ContainerCPUOverThreshold",
+        return self.create_alarm(self.metrics.cpu.average.over(period=over_timespan),
+            name=f"ContainerCPUOverThreshold",
             alarm_description="Container CPU Over Threshold",
             evaluation_periods=evaluation_periods,
             threshold=threshold,
             comparison_operator=ComparisonOperator.GREATER_THAN_THRESHOLD,
             treat_missing_data=TreatMissingData.NOT_BREACHING,
         )
 
     def cpu_under_threshold(self, over_timespan: Union[int, timedelta, Duration], evaluation_periods: int, threshold: float):
-        return self.metrics.cpu_ave(period=over_timespan).create_alarm(
-            alarm_name="ContainerCPUUnderThreshold",
+        return self.create_alarm(self.metrics.cpu.average.over(period=over_timespan),
+            name=f"ContainerCPUUnderThreshold",
             alarm_description="Container CPU Under Threshold",
             evaluation_periods=evaluation_periods,
             threshold=threshold,
             comparison_operator=ComparisonOperator.LESS_THAN_THRESHOLD,
             treat_missing_data=TreatMissingData.NOT_BREACHING,
         )
 
     def memory_over_threshold(self, over_timespan: Union[int, timedelta, Duration], evaluation_periods: int, threshold: float):
-        return self.metrics.cpu_ave(period=over_timespan).create_alarm(
-            alarm_name="ContainerMemoryOverThreshold",
+        return self.create_alarm(self.metrics.cpu.average.over(period=over_timespan),
+            name=f"ContainerMemoryOverThreshold",
             alarm_description="Container Memory Over Threshold",
             evaluation_periods=evaluation_periods,
             threshold=threshold,
             comparison_operator=ComparisonOperator.GREATER_THAN_THRESHOLD,
             treat_missing_data=TreatMissingData.NOT_BREACHING,
         )
 
     def memory_under_threshold(self, over_timespan: Union[int, timedelta, Duration], evaluation_periods: int, threshold: float):
-        return self.metrics.cpu_ave(period=over_timespan).create_alarm(
-            alarm_name="ContainerMemoryUnderThreshold",
+        return self.create_alarm(self.metrics.cpu.average.over(period=over_timespan),
+            name=f"ContainerMemoryUnderThreshold",
             alarm_description="Container Memory Under Threshold",
             evaluation_periods=evaluation_periods,
             threshold=threshold,
             comparison_operator=ComparisonOperator.LESS_THAN_THRESHOLD,
             treat_missing_data=TreatMissingData.NOT_BREACHING,
         )
 
 
 class EcsServiceWidgets:
-    def __init__(self, ecs_service: FargateService):
+    def __init__(self, ecs_service: FargateService, scope: Construct=None):
         self.ecs_service = ecs_service
         self.metrics = EcsServiceMetrics(ecs_service)
+        self.scope = ecs_service.stack if scope is None else scope
 
     def combined_widget(self, period: Union[int, timedelta, Duration], width: int, height: int):
         widget = GraphWidget(
             title=f"{self.ecs_service.service_name} - CPU",
             height=height,
             width=width,
         )
-        widget.add_left_metric(self.metrics.cpu_ave(period=period))
-        widget.add_right_metric(self.metrics.memory_ave(period=period))
+        widget.add_left_metric(self.metrics.cpu.average.over(period=period))
+        widget.add_right_metric(self.metrics.memory.average.over(period=period))
         return widget
 
     def cpu_widget(self, period: Union[int, timedelta, Duration], width: int, height: int):
         widget = GraphWidget(
             title=f"{self.ecs_service.service_name} - CPU",
             height=height,
             width=width,
         )
-        widget.add_left_metric(self.metrics.cpu_ave(period=period))
+        widget.add_left_metric(self.metrics.cpu.average.over(period=period))
         return widget
 
     def memory_widget(self, period: Union[int, timedelta, Duration], width: int, height: int):
         widget = GraphWidget(
             title=f"{self.ecs_service.service_name} - Memory",
             height=height,
             width=width,
         )
-        widget.add_left_metric(self.metrics.memory_ave(period=period))
+        widget.add_left_metric(self.metrics.memory.average.over(period=period))
         return widget
 
+
 class EcsServiceInstrumentation:
-    def __init__(self, ecs_service: FargateService):
-        self.metrics = EcsServiceMetrics(ecs_service)
+    def __init__(self, ecs_service: FargateService, log_group: LogGroup, scope: Construct=None):
+        self.scope = ecs_service.stack if scope is None else scope
+        self.log_group = log_group
+        self.metrics = EcsServiceMetrics(ecs_service, log_group, scope=self.scope)
         self.ecs_service = ecs_service
-        self.widgets = EcsServiceWidgets(ecs_service)
-        self.alarms = EcsServiceAlarms(ecs_service)
+        self.widgets = EcsServiceWidgets(ecs_service, scope=self.scope)
+        self.alarms = EcsServiceAlarms(ecs_service, scope=self.scope)
```

### Comparing `py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/instrumentation/lambdas.py` & `py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/instrumentation/lambdas.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,176 +1,171 @@
 from datetime import timedelta
 from typing import Union
 
 from aws_cdk import Duration
 from aws_cdk.aws_cloudwatch import Metric, ComparisonOperator, TreatMissingData, GraphWidget
 from aws_cdk.aws_lambda import Function
+from aws_cdk.aws_logs import MetricFilter, FilterPattern
+from constructs import Construct
 
 from infraflow.cdk.core.utils import to_duration
+from infraflow.cdk.instrumentation.alarms import AlarmsBase
+from infraflow.cdk.instrumentation.metrics import InfraflowMetric
 
 
 class LambdaMetrics:
-    def __init__(self, function: Function):
+    def __init__(self, function: Function, scope: Construct=None):
         self.function = function
+        self.scope = function.stack if scope is None else scope
 
-    def duration_ave(self, period: Union[int, timedelta, Duration]) -> Metric:
-        return self.function.metric_duration(statistic="average", period=to_duration(period))
+    @property
+    def duration(self) -> InfraflowMetric:
+        return InfraflowMetric(self.function.metric_duration())
 
-    def duration_max(self, period: Union[int, timedelta, Duration]) -> Metric:
-        return self.function.metric_duration(statistic="max", period=to_duration(period))
 
-    def duration_min(self, period: Union[int, timedelta, Duration]) -> Metric:
-        return self.function.metric_duration(statistic="min", period=to_duration(period))
+    @property
+    def concurrent_executions(self) -> InfraflowMetric:
+        return InfraflowMetric(self.function.metric_all_concurrent_executions())
 
-    def concurrent_executions_ave(self, period: Union[int, timedelta, Duration]) -> Metric:
-        return self.function.metric_all_concurrent_executions(statistic="average", period=to_duration(period))
 
-    def concurrent_executions_max(self, period: Union[int, timedelta, Duration]) -> Metric:
-        return self.function.metric_all_concurrent_executions(statistic="max", period=to_duration(period))
+    @property
+    def invocations(self) -> InfraflowMetric:
+        return InfraflowMetric(self.function.metric_invocations())
 
-    def concurrent_executions_min(self, period: Union[int, timedelta, Duration]) -> Metric:
-        return self.function.metric_all_concurrent_executions(statistic="min", period=to_duration(period))
 
-    def invocations_ave(self, period: Union[int, timedelta, Duration]) -> Metric:
-        return self.function.metric_invocations(statistic="average", period=to_duration(period))
+    @property
+    def errors(self) -> InfraflowMetric:
+        return InfraflowMetric(self.function.metric_errors())
 
-    def invocations_max(self, period: Union[int, timedelta, Duration]) -> Metric:
-        return self.function.metric_all_invocations(statistic="max", period=to_duration(period))
 
-    def invocations_min(self, period: Union[int, timedelta, Duration]) -> Metric:
-        return self.function.metric_invocations(statistic="min", period=to_duration(period))
+    @property
+    def throttles(self) -> InfraflowMetric:
+        return InfraflowMetric(self.function.metric_throttles())
 
-    def invocations_sum(self, period: Union[int, timedelta, Duration]) -> Metric:
-        return self.function.metric_invocations(statistic="sum", period=to_duration(period))
-
-    def errors_ave(self, period: Union[int, timedelta, Duration]) -> Metric:
-        return self.function.metric_errors(statistic="average", period=to_duration(period))
-
-    def errors_max(self, period: Union[int, timedelta, Duration]) -> Metric:
-        return self.function.metric_errors(statistic="max", period=to_duration(period))
-
-    def errors_min(self, period: Union[int, timedelta, Duration]) -> Metric:
-        return self.function.metric_errors(statistic="min", period=to_duration(period))
-
-    def errors_sum(self, period: Union[int, timedelta, Duration]) -> Metric:
-        return self.function.metric_errors(statistic="sum", period=to_duration(period))
-
-    def throttles_ave(self, period: Union[int, timedelta, Duration]) -> Metric:
-        return self.function.metric_throttles(statistic="average", period=to_duration(period))
-
-    def throttles_max(self, period: Union[int, timedelta, Duration]) -> Metric:
-        return self.function.metric_throttles(statistic="max", period=to_duration(period))
-
-    def throttles_min(self, period: Union[int, timedelta, Duration]) -> Metric:
-        return self.function.metric_throttles(statistic="min", period=to_duration(period))
-
-    def throttles_sum(self, period: Union[int, timedelta, Duration]) -> Metric:
-        return self.function.metric_throttles(statistic="sum", period=to_duration(period))
+    def log_filter(self, id: str, metric_name: str, metric_value: str, filter_pattern: FilterPattern):
+        return MetricFilter(
+            self.function,
+            id,
+            log_group=self.function.log_group,
+            metric_namespace=self.function.stack.stack_name,
+            metric_name=metric_name,
+            filter_pattern=filter_pattern,
+            metric_value=metric_value
+        )
 
 
-class LambdaAlarms:
-    def __init__(self, function: Function, reserved_concurrency: int):
+class LambdaAlarms(AlarmsBase):
+    def __init__(self, function: Function, reserved_concurrency: int, name: str = None, scope: Construct = None):
+        super().__init__(name or function.function_name, function, scope or function.stack)
         self.function = function
         self.metrics = LambdaMetrics(function)
         self.reserved_concurrency = reserved_concurrency
+        self.scope = function.stack if scope is None else scope
 
     def running_longer_than_expected(self, over_timespan: Union[int, timedelta, Duration], evaluation_periods: int, percent_of_timeout_threshold: float):
-        return self.metrics.duration_max(over_timespan).create_alarm(
-            alarm_name="LambdaRunningLongerThanExpected",
+        return self.create_alarm(
+            self.metrics.duration.max.over(over_timespan),
+            name=f"LambdaRunningLongerThanExpected",
             alarm_description="Lambda running longer than expected",
             threshold=to_duration(round(self.function.timeout.to_seconds() * percent_of_timeout_threshold)),
             evaluation_periods=evaluation_periods,
             comparison_operator=ComparisonOperator.GREATER_THAN_THRESHOLD,
             treat_missing_data=TreatMissingData.NOT_BREACHING,
         )
 
     def invocations_exceed_threshold(self, over_timespan: Union[int, timedelta, Duration], evaluation_periods: int, threshold: int):
-        return self.metrics.invocations_ave(over_timespan).create_alarm(
-            alarm_name="LambdaInvocationsExceedThreshold",
+        return self.create_alarm(
+            self.metrics.invocations.average.over(over_timespan),
+            name=f"LambdaInvocationsExceedThreshold",
             alarm_description="Lambda invocations exceed threshold",
             threshold=threshold,
             evaluation_periods=evaluation_periods,
             comparison_operator=ComparisonOperator.GREATER_THAN_THRESHOLD,
             treat_missing_data=TreatMissingData.NOT_BREACHING,
         )
 
     def concurrency_exceed_threshold(self, over_timespan: Union[int, timedelta, Duration], evaluation_periods: int, percent_of_max_threshold: float):
-        return self.metrics.concurrent_executions_ave(over_timespan).create_alarm(
-            alarm_name="LambdaConcurrencyExceedThreshold",
+        return self.create_alarm(
+            self.metrics.concurrent_executions.average.over(over_timespan),
+            name=f"{self.function.function_name}LambdaConcurrencyExceedThreshold",
             alarm_description="Lambda concurrency exceed threshold",
             threshold=round(self.reserved_concurrency * percent_of_max_threshold),
             evaluation_periods=evaluation_periods,
             comparison_operator=ComparisonOperator.GREATER_THAN_THRESHOLD,
             treat_missing_data=TreatMissingData.NOT_BREACHING,
         )
 
     def errors_exceed_threshold(self, over_timespan: Union[int, timedelta, Duration], evaluation_periods: int, threshold: float):
-        return self.metrics.errors_ave(over_timespan).create_alarm(
-            alarm_name="LambdaErrorsExceedThreshold",
+        return self.create_alarm(
+            self.metrics.errors.average.over(over_timespan),
+            name=f"{self.function.function_name}LambdaErrorsExceedThreshold",
             alarm_description="Lambda errors exceed threshold",
             threshold=threshold,
             evaluation_periods=evaluation_periods,
             comparison_operator=ComparisonOperator.GREATER_THAN_THRESHOLD,
             treat_missing_data=TreatMissingData.NOT_BREACHING,
         )
 
 
 
 class LambdaWidgets:
-    def __init__(self, function: Function):
+    def __init__(self, function: Function, scope: Construct=None):
         self.function = function
         self.metrics = LambdaMetrics(function)
+        self.scope = function.stack if scope is None else scope
 
     def errors_sum_widget(self, period: Union[int, timedelta, Duration], width: int, height: int):
         widget = GraphWidget(
             title=f"{self.function.function_name} - Total Errors",
             height=height,
             width=width,
         )
-        widget.add_left_metric(self.metrics.errors_sum(period=period))
+        widget.add_left_metric(self.metrics.errors.sum.over(period=period))
         return widget
 
     def concurrent_executions_widget(self, period: Union[int, timedelta, Duration], width: int, height: int):
         widget = GraphWidget(
             title=f"{self.function.function_name} - Concurrent Executions",
             height=height,
             width=width,
         )
-        widget.add_left_metric(self.metrics.concurrent_executions_max(period=period))
+        widget.add_left_metric(self.metrics.concurrent_executions.max.over(period=period))
         return widget
 
     def invocation_widget(self, period: Union[int, timedelta, Duration], width: int, height: int):
         widget = GraphWidget(
             title=f"{self.function.function_name} - Invocations",
             height=height,
             width=width,
         )
-        widget.add_left_metric(self.metrics.invocations_sum(period=period))
+        widget.add_left_metric(self.metrics.invocations.sum.over(period=period))
         return widget
 
     def duration_widget(self, period: Union[int, timedelta, Duration], width: int, height: int):
         widget = GraphWidget(
             title=f"{self.function.function_name} - Duration",
             height=height,
             width=width,
         )
-        widget.add_left_metric(self.metrics.duration_ave(period=period))
+        widget.add_left_metric(self.metrics.duration.average.over(period=period))
         return widget
 
     def throttle_widget(self, period: Union[int, timedelta, Duration], width: int, height: int):
         widget = GraphWidget(
             title=f"{self.function.function_name} - Throttles",
             height=height,
             width=width,
         )
-        widget.add_left_metric(self.metrics.throttles_sum(period=period))
+        widget.add_left_metric(self.metrics.throttles.sum.over(period=period))
         return widget
 
 
 class LambdaInstrumentation:
-    def __init__(self, function: Function, reserved_concurrency):
-        self.metrics = LambdaMetrics(function)
+    def __init__(self, function: Function, reserved_concurrency, scope: Construct=None):
+        self.scope = function.stack if scope is None else scope
+        self.metrics = LambdaMetrics(function, scope=self.scope)
         self.reserved_concurrency = reserved_concurrency
         self.function = function
-        self.widgets = LambdaWidgets(function)
-        self.alarms = LambdaAlarms(function=function, reserved_concurrency=reserved_concurrency)
+        self.widgets = LambdaWidgets(function, scope=self.scope)
+        self.alarms = LambdaAlarms(function, scope=self.scope)
+        self.log_group = function.log_group
```

### Comparing `py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/instrumentation/queues.py` & `py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/instrumentation/queues.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,123 +1,114 @@
+import builtins
+import typing
 from datetime import timedelta
 from typing import Union
 
+import jsii
 from aws_cdk import Duration
-from aws_cdk.aws_cloudwatch import ComparisonOperator, TreatMissingData, GraphWidget
+from aws_cdk.aws_cloudwatch import ComparisonOperator, TreatMissingData, GraphWidget, Metric
 from aws_cdk.aws_sqs import Queue
+from constructs import Construct
 
 from infraflow.cdk.core.utils import to_duration
+from infraflow.cdk.instrumentation.alarms import AlarmsBase
+from infraflow.cdk.instrumentation.metrics import InfraflowMetric
 
 
 class QueueMetrics:
-    def __init__(self, queue: Queue):
+    def __init__(self, queue: Queue, scope: Construct=None):
         self.queue = queue
+        self.scope = queue.stack if scope is None else scope
 
-    def sent_ave(self, period: Union[int, timedelta, Duration]):
-        return self.queue.metric_number_of_messages_sent(period=to_duration(period) if period else None, statistic="average")
+    @property
+    def sent(self) -> InfraflowMetric:
+        return InfraflowMetric(self.queue.metric_number_of_messages_sent())
 
-    def sent_max(self, period: Union[int, timedelta, Duration]):
-        return self.queue.metric_number_of_messages_sent(period=to_duration(period) if period else None, statistic="max")
+    @property
+    def length(self) -> InfraflowMetric:
+        return InfraflowMetric(self.queue.metric_approximate_number_of_messages_visible())
 
-    def sent_min(self, period: Union[int, timedelta, Duration]):
-        return self.queue.metric_number_of_messages_sent(period=to_duration(period) if period else None, statistic="min")
+    @property
+    def age_of_oldest(self):
+        return InfraflowMetric(self.queue.metric_approximate_age_of_oldest_message())
 
-    def sent_sum(self, period: Union[int, timedelta, Duration]):
-        return self.queue.metric_number_of_messages_sent(period=to_duration(period) if period else None, statistic="sum")
 
-    def length_ave(self, period: Union[int, timedelta, Duration]):
-        return self.queue.metric_approximate_number_of_messages_visible(period=to_duration(period) if period else None, statistic="average")
 
-    def length_max(self, period: Union[int, timedelta, Duration]):
-        return self.queue.metric_approximate_number_of_messages_visible(period=to_duration(period) if period else None, statistic="max")
-
-    def length_min(self, period: Union[int, timedelta, Duration]):
-        return self.queue.metric_approximate_number_of_messages_visible(period=to_duration(period) if period else None, statistic="min")
-
-    def age_of_oldest_ave(self, period: Union[int, timedelta, Duration]):
-        return self.queue.metric_approximate_age_of_oldest_message(period=to_duration(period) if period else None, statistic="average")
-
-    def age_of_oldest_max(self, period: Union[int, timedelta, Duration]):
-        return self.queue.metric_approximate_age_of_oldest_message(period=to_duration(period) if period else None, statistic="max")
-
-    def age_of_oldest_min(self, period: Union[int, timedelta, Duration]):
-        return self.queue.metric_approximate_age_of_oldest_message(period=to_duration(period) if period else None, statistic="min")
-
-
-class QueueAlarms:
-    def __init__(self, queue: Queue):
+class QueueAlarms(AlarmsBase):
+    def __init__(self, queue: Queue, name: str = None, scope: Construct = None):
+        super().__init__(name or queue.queue_name, queue, scope or queue.stack)
         self.queue = queue
         self.metrics = QueueMetrics(queue)
 
     def age_of_oldest_over_threshold(self, threshold: int, period: Union[int, timedelta, Duration], evaluation_periods: int):
-        return self.metrics.age_of_oldest_ave(period).create_alarm(
-            alarm_name=f"{self.queue.queue_name}_AgeOfOldestOverThreshold",
+        return self.create_alarm(
+            self.metrics.age_of_oldest.average.over(period),
+            name=f"AgeOfOldestOverThreshold",
             threshold=threshold,
             evaluation_periods=evaluation_periods,
             comparison_operator=ComparisonOperator.GREATER_THAN_OR_EQUAL_TO_THRESHOLD,
-            period=to_duration(period),
-            statistic="average",
             treat_missing_data=TreatMissingData.NOT_BREACHING,
         )
 
     def length_over_threshold(self, threshold: int, period: Union[int, timedelta, Duration], evaluation_periods: int):
-        return self.metrics.length_ave(period).create_alarm(
-            alarm_name=f"{self.queue.queue_name}_LengthOverThreshold",
+        return self.create_alarm(
+            self.metrics.length.average.over(period),
+            name=f"LengthOverThreshold",
             threshold=threshold,
             evaluation_periods=evaluation_periods,
             comparison_operator=ComparisonOperator.GREATER_THAN_OR_EQUAL_TO_THRESHOLD,
-            period=to_duration(period),
-            statistic="average",
             treat_missing_data=TreatMissingData.NOT_BREACHING,
         )
 
     def sent_over_threshold(self, threshold: int, period: Union[int, timedelta, Duration], evaluation_periods: int):
-        return self.metrics.sent_ave(period).create_alarm(
-            alarm_name=f"{self.queue.queue_name}_SentOverThreshold",
+        return self.create_alarm(
+            metric=self.metrics.sent.average.over(period),
+            name=f"SentOverThreshold",
             threshold=threshold,
             evaluation_periods=evaluation_periods,
             comparison_operator=ComparisonOperator.GREATER_THAN_OR_EQUAL_TO_THRESHOLD,
-            period=to_duration(period),
-            statistic="average",
             treat_missing_data=TreatMissingData.NOT_BREACHING,
         )
 
 
+
 class QueueWidgets:
-    def __init__(self, queue: Queue):
+    def __init__(self, queue: Queue, scope: Construct=None):
         self.queue = queue
         self.metrics = QueueMetrics(queue)
+        self.scope = queue.stack if scope is None else scope
 
     def age_max_widget(self, period: Union[int, timedelta, Duration], width: int, height: int):
         widget = GraphWidget(
             title=f"{self.queue.queue_name} - Age of Oldest Message",
             height=height,
             width=width,
         )
-        widget.add_left_metric(self.metrics.age_of_oldest_max(period=period))
+        widget.add_left_metric(self.metrics.age_of_oldest.max.over(period=period))
         return widget
 
     def length_max_widget(self, period: Union[int, timedelta, Duration], width: int, height: int):
         widget = GraphWidget(
             title=f"{self.queue.queue_name} - Length of Queue",
             height=height,
             width=width,
         )
-        widget.add_left_metric(self.metrics.length_max(period=period))
+        widget.add_left_metric(self.metrics.length.max.over(period=period))
         return widget
 
     def sent_sum_widget(self, period: Union[int, timedelta, Duration], width: int, height: int):
         widget = GraphWidget(
             title=f"{self.queue.queue_name} - Total Messages Sent",
             height=height,
             width=width,
         )
-        widget.add_left_metric(self.metrics.sent_sum(period=period))
+        widget.add_left_metric(self.metrics.sent.sum.over(period=period))
         return widget
 
 
 class QueueInstrumentation:
-    def __init__(self, queue: Queue):
-        self.metrics = QueueMetrics(queue)
+    def __init__(self, queue: Queue, scope: Construct=None):
+        self.scope = queue.stack if scope is None else scope
+        self.metrics = QueueMetrics(queue, self.scope)
         self.queue = queue
-        self.widgets = QueueWidgets(queue)
-        self.alarms = QueueAlarms(queue)
+        self.widgets = QueueWidgets(queue, self.scope)
+        self.alarms = QueueAlarms(queue, self.scope)
```

### Comparing `py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/lambdas.py` & `py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/lambdas.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         self.runtime = runtime
         self.path = path
         self.stage = stage
         self.default_sg = stage.default_sg
         self.queues: list[aws_sqs.Queue] = []
         self.functions: list[aws_lambda.Function] = []
         self.queue_instrumentation: dict[aws_sqs.Queue, QueueInstrumentation] = {}
-        self.lambda_instrumentation: dict[aws_sqs.Queue, LambdaInstrumentation] = {}
+        self.lambda_instrumentation: dict[aws_lambda.Function, LambdaInstrumentation] = {}
 
     # def to_cdk(self):
     #     return dict(
     #         scope=self.scope,
     #         code=aws_lambda.Code.from_asset(self.path),
     #         runtime=self.runtime
     #     )
```

### Comparing `py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/sg/patterns.py` & `py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/sg/patterns.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/sg/ports.py` & `py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/sg/ports.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.0/infraflow/cdk/sg/tier_maps.py` & `py_infraflow_cdk-0.1.9.8.9.1/infraflow/cdk/sg/tier_maps.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.0/pyproject.toml` & `py_infraflow_cdk-0.1.9.8.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-infraflow-cdk"
-version = "0.1.9.8.9.0"
+version = "0.1.9.8.9.1"
 description = "Build Event Based and Microservice infrastructure and connections using these reusable AWS CDK patterns"
 authors = ["Matthew Beatty <infraflow@upcontent.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "infraflow"}]
 
 [tool.poetry.dependencies]
```

### Comparing `py_infraflow_cdk-0.1.9.8.9.0/PKG-INFO` & `py_infraflow_cdk-0.1.9.8.9.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-infraflow-cdk
-Version: 0.1.9.8.9.0
+Version: 0.1.9.8.9.1
 Summary: Build Event Based and Microservice infrastructure and connections using these reusable AWS CDK patterns
 License: MIT
 Author: Matthew Beatty
 Author-email: infraflow@upcontent.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

