# Comparing `tmp/dagster_scaleway-0.1.2.tar.gz` & `tmp/dagster_scaleway-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_scaleway-0.1.2.tar", max compression
+gzip compressed data, was "dagster_scaleway-0.1.3.tar", max compression
```

## Comparing `dagster_scaleway-0.1.2.tar` & `dagster_scaleway-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1606 2024-01-14 19:40:11.828045 dagster_scaleway-0.1.2/README.md
--rw-r--r--   0        0        0      130 2024-01-14 19:40:11.828045 dagster_scaleway-0.1.2/dagster_scaleway/__init__.py
--rw-r--r--   0        0        0      647 2024-01-14 19:40:11.828045 dagster_scaleway-0.1.2/dagster_scaleway/cli.py
--rw-r--r--   0        0        0     7026 2024-01-14 19:40:11.828045 dagster_scaleway-0.1.2/dagster_scaleway/serverless_job_context.py
--rw-r--r--   0        0        0    11070 2024-01-14 19:40:11.828045 dagster_scaleway-0.1.2/dagster_scaleway/serverless_job_launcher.py
--rw-r--r--   0        0        0      705 2024-01-14 19:40:23.548137 dagster_scaleway-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2113 1970-01-01 00:00:00.000000 dagster_scaleway-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1638 2024-04-24 08:35:07.818086 dagster_scaleway-0.1.3/README.md
+-rw-r--r--   0        0        0      130 2024-04-24 08:35:07.818086 dagster_scaleway-0.1.3/dagster_scaleway/__init__.py
+-rw-r--r--   0        0        0      647 2024-04-24 08:35:07.818086 dagster_scaleway-0.1.3/dagster_scaleway/cli.py
+-rw-r--r--   0        0        0     7036 2024-04-24 08:35:07.818086 dagster_scaleway-0.1.3/dagster_scaleway/serverless_job_context.py
+-rw-r--r--   0        0        0    11129 2024-04-24 08:35:07.818086 dagster_scaleway-0.1.3/dagster_scaleway/serverless_job_launcher.py
+-rw-r--r--   0        0        0      705 2024-04-24 08:35:12.794072 dagster_scaleway-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 dagster_scaleway-0.1.3/PKG-INFO
```

### Comparing `dagster_scaleway-0.1.2/README.md` & `dagster_scaleway-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 
 Build a docker image containing your Dagster code and push it to the Scaleway Registry (or any other registry of your choice):
 
 ```bash
 dagster project scaffold --name my-dagster-project
 cd my-dagster-project
 
-echo<<EOF > Dockerfile
+cat <<EOF > Dockerfile
 FROM python:3.12-slim-bookworm
 WORKDIR /app
 COPY . .
+RUN pip install pendulum==2.0.3
 RUN pip install .
 # Install the Dagster Scaleway module. You can also specify it in your "setup.py" file
 RUN pip install dagster_scaleway
 EOF
 ```
 
 Build and push the image:
```

### Comparing `dagster_scaleway-0.1.2/dagster_scaleway/cli.py` & `dagster_scaleway-0.1.3/dagster_scaleway/cli.py`

 * *Files identical despite different names*

### Comparing `dagster_scaleway-0.1.2/dagster_scaleway/serverless_job_context.py` & `dagster_scaleway-0.1.3/dagster_scaleway/serverless_job_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 class ScalewayServerlessJobContext(
     NamedTuple(
         "_ScalewayServerlessJobContext",
         [
             ("docker_image", Optional[str]),
             ("env_vars", Sequence[str]),
-            ("region", str),
+            ("region", Optional[str]),
             ("memory_limit", int),
             ("cpu_limit", int),
         ],
     )
 ):
     """Encapsulates the configuration for a Scaleway Serverless Job.
     Dagster code. Can be set at the instance level (via config in the `DockerRunLauncher`),
```

### Comparing `dagster_scaleway-0.1.2/dagster_scaleway/serverless_job_launcher.py` & `dagster_scaleway-0.1.3/dagster_scaleway/serverless_job_launcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from typing import Any, Mapping, Optional
 
 import dagster._check as check
 from dagster._core.launcher.base import (
     CheckRunHealthResult,
     LaunchRunContext,
-    ResumeRunContext,
     RunLauncher,
     WorkerStatus,
 )
 from dagster._core.origin import JobPythonOrigin
 from dagster._core.storage.dagster_run import DagsterRun
 from dagster._core.storage.tags import DOCKER_IMAGE_TAG
 from dagster._core.utils import parse_env_var
-from dagster._grpc.types import ExecuteRunArgs, ResumeRunArgs
+from dagster._grpc.types import ExecuteRunArgs
 from dagster._serdes import ConfigurableClass
 from dagster._serdes.config_class import ConfigurableClassData
 from typing_extensions import Self
 
 
 import scaleway.jobs.v1alpha1 as scw
 import scaleway
@@ -111,98 +110,122 @@
         """
         if dagster_run.op_selection:
             return list(dagster_run.op_selection)[-1]
         if dagster_run.asset_selection:
             return list(dagster_run.asset_selection)[-1].to_user_string()
         return dagster_run.run_id
 
-    def _create_or_update_job_definition(
+    def _get_or_create_job_definition(
         self,
         client: scaleway.Client,
         run: DagsterRun,
         docker_image: str,
-        command: list[str],
     ) -> scw.JobDefinition:
         serverless_job_context = self.get_serverless_job_context(run)
         api = scw.JobsV1Alpha1API(client)
 
-        job_def_env = dict(
-            [parse_env_var(env_var) for env_var in serverless_job_context.env_vars]
-        )
-        job_def_env["DAGSTER_RUN_JOB_NAME"] = run.job_name
-        job_def_env["DAGSTER_RUN_ID"] = run.run_id
-        job_def_env["INPUT_JSON"] = command[-1]
-
-        api = scw.JobsV1Alpha1API(client)
-
-        wrapped_command = [COMMAND_WRAPPER] + command[:-1]
-        description = (
-            f"JobDefinition for {run.job_name}."
-            + " "
-            + "Created by the ServerlessJobRunLauncher from dagster-scaleway."
-        )
         job_def_name = self._get_semantic_job_name(run)
 
         for job_def in api.list_job_definitions_all():
             if job_def.name != job_def_name:
                 continue
 
-            job_def = api.update_job_definition(
-                job_definition_id=job_def.id,
-                name=job_def_name,
-                image_uri=docker_image,
-                environment_variables=job_def_env,
-                command=" ".join(wrapped_command),
-                memory_limit=serverless_job_context.memory_limit,
-                cpu_limit=serverless_job_context.cpu_limit,
-                description=description,
+            return self._update_job_definition(
+                client, serverless_job_context, job_def, docker_image
             )
 
-            self._instance.report_engine_event(
-                message=f"Updated job {job_def.id} for Dagster run {run.run_id}",
-                dagster_run=run,
-                cls=self.__class__,
-            )
+        job_def_env = dict(
+            [parse_env_var(env_var) for env_var in serverless_job_context.env_vars]
+        )
 
-            return job_def
+        job_def_name = self._get_semantic_job_name(run)
 
         job_def = api.create_job_definition(
             name=job_def_name,
             image_uri=docker_image,
             environment_variables=job_def_env,
-            command=" ".join(wrapped_command),
+            command=COMMAND_WRAPPER,
             memory_limit=serverless_job_context.memory_limit,
             cpu_limit=serverless_job_context.cpu_limit,
-            description=description,
+            description="Created by the ServerlessJobRunLauncher from dagster-scaleway.",
             project_id=client.default_project_id,
         )
 
         self._instance.report_engine_event(
             message=f"Created job {job_def.id} for Dagster run {run.run_id}",
             dagster_run=run,
             cls=self.__class__,
         )
 
         return job_def
 
-    def _launch_serverless_job_with_command(
+    def _update_job_definition(
+        self,
+        client: scaleway.Client,
+        context: ScalewayServerlessJobContext,
+        job_def: scw.JobDefinition,
+        docker_image: str,
+    ) -> scw.JobDefinition:
+        """Reconcile the job definition with the desired state"""
+        api = scw.JobsV1Alpha1API(client)
+        has_changed = False
+
+        if job_def.image_uri != docker_image:
+            job_def.image_uri = docker_image
+            has_changed = True
+
+        if job_def.memory_limit != context.memory_limit:
+            job_def.memory_limit = context.memory_limit
+            has_changed = True
+
+        if job_def.cpu_limit != context.cpu_limit:
+            job_def.cpu_limit = context.cpu_limit
+            has_changed = True
+
+        if not has_changed:
+            return job_def
+
+        return api.update_job_definition(
+            job_definition_id=job_def.id,
+            image_uri=docker_image,
+            memory_limit=context.memory_limit,
+            cpu_limit=context.cpu_limit,
+        )
+
+    def _start_serverless_job_with_command(
         self, run: DagsterRun, docker_image: str, command: list[str]
     ):
         serverless_job_context = self.get_serverless_job_context(run)
         client = self._get_client(serverless_job_context)
         api = scw.JobsV1Alpha1API(client)
 
-        job_def = self._create_or_update_job_definition(
-            client, run, docker_image, command
+        job_def = self._get_or_create_job_definition(client, run, docker_image)
+
+        extra_env = {
+            "DAGSTER_RUN_JOB_NAME": run.job_name,
+            "DAGSTER_RUN_ID": run.run_id,
+            "INPUT_JSON": command[-1],
+        }
+        wrapped_command = [COMMAND_WRAPPER] + command[:-1]
+
+        start_response = api.start_job_definition(
+            job_definition_id=job_def.id,
+            command=" ".join(wrapped_command),
+            environment_variables=extra_env,
         )
 
-        job_run = api.start_job_definition(job_definition_id=job_def.id)
+        if len(start_response.job_runs) != 1:
+            raise RuntimeError(
+                f"Expected 1 job run to be created, got {len(start_response.job_runs)}"
+            )
+
+        job_run = start_response.job_runs[0]
 
         self._instance.report_engine_event(
-            message=f"Started job definition {job_def.name} with run id {job_run.id} for Dagster run {run.run_id}",
+            message=f"Started job definition {job_def.name} with job run id {job_run.id} for Dagster run {run.run_id}",
             dagster_run=run,
             cls=self.__class__,
         )
 
         self._instance.add_run_tags(
             run.run_id,
             {
@@ -219,33 +242,19 @@
 
         command = ExecuteRunArgs(
             job_origin=job_code_origin,
             run_id=run.run_id,
             instance_ref=self._instance.get_ref(),
         ).get_command_args()
 
-        self._launch_serverless_job_with_command(run, docker_image, command)
+        self._start_serverless_job_with_command(run, docker_image, list(command))
 
     @property
     def supports_resume_run(self):
-        # TODO?: check if we can resume a run
-        return True
-
-    def resume_run(self, context: ResumeRunContext) -> None:
-        run = context.dagster_run
-        job_code_origin = check.not_none(context.job_code_origin)
-        docker_image = self._get_docker_image(job_code_origin)
-
-        command = ResumeRunArgs(
-            job_origin=job_code_origin,
-            run_id=run.run_id,
-            instance_ref=self._instance.get_ref(),
-        ).get_command_args()
-
-        self._launch_serverless_job_with_command(run, docker_image, command)
+        return False
 
     def _get_scaleway_job_run_from_dagster_run(self, run) -> Optional[scw.JobRun]:
         if not run or run.is_finished:
             return None
 
         job_run_id = run.tags.get(SERVERLESS_JOBS_RUN_ID)
 
@@ -299,22 +308,22 @@
     def supports_check_run_worker_health(self):
         return True
 
     def check_run_worker_health(self, run: DagsterRun):
         job_run = self._get_scaleway_job_run_from_dagster_run(run)
         if job_run is None:
             return CheckRunHealthResult(
-                WorkerStatus.NOT_FOUND,
+                status=WorkerStatus.NOT_FOUND,
                 run_worker_id=run.run_id,
                 msg=f"Unable to find Scaleway job run with id {run.run_id} for Dagster run {run.run_id}",
             )
 
-        health = CheckRunHealthResult(run_worker_id=run.run_id)
-        health.transient = job_run.state in scw.JOB_RUN_TRANSIENT_STATUSES
-        health.status = SERVERLESS_JOBS_STATES_TO_WORKER_STATUS.get(
-            job_run.state, WorkerStatus.UNKNOWN
+        health = CheckRunHealthResult(
+            status=SERVERLESS_JOBS_STATES_TO_WORKER_STATUS.get(
+                job_run.state, WorkerStatus.UNKNOWN
+            ),
+            run_worker_id=run.run_id,
+            msg=job_run.error_message,
+            transient=job_run.state in scw.JOB_RUN_TRANSIENT_STATUSES,
         )
 
-        if job_run.error_message:
-            health.msg = job_run.error_message
-
         return health
```

### Comparing `dagster_scaleway-0.1.2/pyproject.toml` & `dagster_scaleway-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "dagster-scaleway"
 # Version will be updated by CI
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Andy Méry <amery@scaleway.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 packages = [{ include = "dagster_scaleway" }]
 
 [tool.poetry.scripts]
 dagster-scaleway = "dagster_scaleway.cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-scaleway = "^1.4.1"
+scaleway = "^2.1.0"
 dagster = "^1.6.0"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.15.9"
 pre-commit = "^2.21.0"
 dagit = "^1.6.0"
 ruff = "^0.1.6"
```

### Comparing `dagster_scaleway-0.1.2/PKG-INFO` & `dagster_scaleway-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: dagster-scaleway
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 License: Apache-2.0
 Author: Andy Méry
 Author-email: amery@scaleway.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dagster (>=1.6.0,<2.0.0)
-Requires-Dist: scaleway (>=1.4.1,<2.0.0)
+Requires-Dist: scaleway (>=2.1.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Dagster Scaleway (WIP)
 
 This repository contains a [Dagster](https://dagster.io) integration for [Scaleway](https://www.scaleway.com/en/).
 
 It allows you to run Dagster pipelines on [Scaleway Serverless Jobs](https://www.scaleway.com/en/docs/serverless/jobs/quickstart/).
@@ -24,18 +24,19 @@
 
 Build a docker image containing your Dagster code and push it to the Scaleway Registry (or any other registry of your choice):
 
 ```bash
 dagster project scaffold --name my-dagster-project
 cd my-dagster-project
 
-echo<<EOF > Dockerfile
+cat <<EOF > Dockerfile
 FROM python:3.12-slim-bookworm
 WORKDIR /app
 COPY . .
+RUN pip install pendulum==2.0.3
 RUN pip install .
 # Install the Dagster Scaleway module. You can also specify it in your "setup.py" file
 RUN pip install dagster_scaleway
 EOF
 ```
 
 Build and push the image:
```

