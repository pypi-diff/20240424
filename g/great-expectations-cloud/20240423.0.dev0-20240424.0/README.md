# Comparing `tmp/great_expectations_cloud-20240423.0.dev0.tar.gz` & `tmp/great_expectations_cloud-20240424.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "great_expectations_cloud-20240423.0.dev0.tar", max compression
+gzip compressed data, was "great_expectations_cloud-20240424.0.tar", max compression
```

## Comparing `great_expectations_cloud-20240423.0.dev0.tar` & `great_expectations_cloud-20240424.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2084 2024-04-23 16:11:50.759573 great_expectations_cloud-20240423.0.dev0/LICENSE
--rw-r--r--   0        0        0     9486 2024-04-23 16:11:50.759573 great_expectations_cloud-20240423.0.dev0/README.md
--rw-r--r--   0        0        0      150 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/__init__.py
--rw-r--r--   0        0        0      244 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/__init__.py
--rw-r--r--   0        0        0      733 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/__init__.py
--rw-r--r--   0        0        0      763 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/agent_action.py
--rw-r--r--   0        0        0      316 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
--rw-r--r--   0        0        0     1511 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
--rw-r--r--   0        0        0     1503 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
--rw-r--r--   0        0        0     4279 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py
--rw-r--r--   0        0        0     4171 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
--rw-r--r--   0        0        0     2881 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/list_table_names.py
--rw-r--r--   0        0        0     2041 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py
--rw-r--r--   0        0        0     2993 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/run_metric_list_action.py
--rw-r--r--   0        0        0      733 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/unknown.py
--rw-r--r--   0        0        0    16465 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/agent.py
--rw-r--r--   0        0        0     2851 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/cli.py
--rw-r--r--   0        0        0      858 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/config.py
--rw-r--r--   0        0        0      246 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/constants.py
--rw-r--r--   0        0        0     4598 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/event_handler.py
--rw-r--r--   0        0        0     1360 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/message_service/__init__.py
--rw-r--r--   0        0        0     9260 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
--rw-r--r--   0        0        0     5836 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/message_service/subscriber.py
--rw-r--r--   0        0        0     3562 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/models.py
--rw-r--r--   0        0        0      639 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/run.py
--rw-r--r--   0        0        0      362 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/warnings.py
--rw-r--r--   0        0        0     1762 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/logging/README.md
--rw-r--r--   0        0        0     5395 2024-04-23 16:11:50.795573 great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/logging/logging_cfg.py
--rw-r--r--   0        0        0     9462 2024-04-23 16:11:50.799573 great_expectations_cloud-20240423.0.dev0/pyproject.toml
--rw-r--r--   0        0        0    10820 1970-01-01 00:00:00.000000 great_expectations_cloud-20240423.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0     2084 2024-04-24 18:01:13.866627 great_expectations_cloud-20240424.0/LICENSE
+-rw-r--r--   0        0        0     9269 2024-04-24 18:01:13.866627 great_expectations_cloud-20240424.0/README.md
+-rw-r--r--   0        0        0      150 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/__init__.py
+-rw-r--r--   0        0        0      244 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/__init__.py
+-rw-r--r--   0        0        0      733 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/__init__.py
+-rw-r--r--   0        0        0      763 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/agent_action.py
+-rw-r--r--   0        0        0      316 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
+-rw-r--r--   0        0        0     1511 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
+-rw-r--r--   0        0        0     1503 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
+-rw-r--r--   0        0        0     4279 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/data_assistants/utils.py
+-rw-r--r--   0        0        0     4171 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
+-rw-r--r--   0        0        0     2881 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/list_table_names.py
+-rw-r--r--   0        0        0     2041 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/run_checkpoint.py
+-rw-r--r--   0        0        0     2993 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/run_metric_list_action.py
+-rw-r--r--   0        0        0      739 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/unknown.py
+-rw-r--r--   0        0        0    16465 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/agent.py
+-rw-r--r--   0        0        0      362 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/agent_warnings.py
+-rw-r--r--   0        0        0     2851 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/cli.py
+-rw-r--r--   0        0        0      858 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/config.py
+-rw-r--r--   0        0        0      246 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/constants.py
+-rw-r--r--   0        0        0     4598 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/event_handler.py
+-rw-r--r--   0        0        0     1360 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/message_service/__init__.py
+-rw-r--r--   0        0        0     9260 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
+-rw-r--r--   0        0        0     5836 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/message_service/subscriber.py
+-rw-r--r--   0        0        0     3562 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/models.py
+-rw-r--r--   0        0        0      639 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/run.py
+-rw-r--r--   0        0        0     1762 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/logging/README.md
+-rw-r--r--   0        0        0     5395 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/logging/logging_cfg.py
+-rw-r--r--   0        0        0     9457 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/pyproject.toml
+-rw-r--r--   0        0        0    10598 1970-01-01 00:00:00.000000 great_expectations_cloud-20240424.0/PKG-INFO
```

### Comparing `great_expectations_cloud-20240423.0.dev0/LICENSE` & `great_expectations_cloud-20240424.0/LICENSE`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240423.0.dev0/README.md` & `great_expectations_cloud-20240424.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -214,15 +214,15 @@
 2. [Containerize Agent](./.github/workflows/containerize-agent.yml) - This workflows runs on merge with `main` and will create a new Docker image and push it to Docker Hub and PyPi. It uses the version in `pyproject.toml`.
 
 A visual representation of the workflow is shown [here](./.github/workflows/agent_release_workflows.png)
 
 ### Dependabot and Releases/Pre-releases
 GitHub's Dependabot regularly checks our dependencies for vulnerabilty-based updates and proposes PRs to update dependency version numbers accordingly.
 
-Dependabot may only update the `poetry.lock` file. Before merging Dependabot suggestions, we should also ensure that `pyproject.toml` is aligned with version locked in the `poetry.lock` file by following the instructions above at [Updating `poetry.lock` dependencies](#updating-poetry.lock-dependencies).
+Dependabot may only update the `poetry.lock` file. If only changes to `poetry.lock` are made, this may be done in a pre-release.
 
-Note: if Dependabot suggests an update to a tool in the `[tool.poetry.group.dev.dependencies]` group in `pyproject.toml`, these changes can be merged in a pre-release version (i.e., a standard release is not required). While doing this, make sure any version references in the pre-commit config `.pre-commit-config.yaml` are kept in sync (e.g., ruff).
-
-For other dependency updates, a new release should be orchestrated. This includes updates in the following sections:
-
-- `[tool.poetry.dependencies]`
-- `[tool.poetry.group.*.dependencies]` where `*` is the name of the group (not including the `dev` group)
+For changes to the `pyproject.toml` file:
+- If the version of a tool in the `[tool.poetry.group.dev.dependencies]` group is updated, this may be done in a pre-release.
+   -  While doing this, make sure any version references in the pre-commit config `.pre-commit-config.yaml` are kept in sync (e.g., ruff).
+- For other dependency updates, a new release should be orchestrated. This includes updates in the following sections:
+  - `[tool.poetry.dependencies]`
+  - `[tool.poetry.group.*.dependencies]` where `*` is the name of the group (not including the `dev` group)
```

### Comparing `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/__init__.py` & `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/agent_action.py` & `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/agent_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py` & `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py` & `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py` & `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/data_assistants/utils.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py` & `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/list_table_names.py` & `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/list_table_names.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py` & `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/run_checkpoint.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/run_metric_list_action.py` & `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/run_metric_list_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/actions/unknown.py` & `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/unknown.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 from typing_extensions import override
 
 from great_expectations_cloud.agent.actions.agent_action import (
     ActionResult,
     AgentAction,
 )
+from great_expectations_cloud.agent.agent_warnings import warn_unknown_event
 from great_expectations_cloud.agent.models import (
     UnknownEvent,
 )
-from great_expectations_cloud.agent.warnings import warn_unknown_event
 
 LOGGER: Final[logging.Logger] = logging.getLogger(__name__)
 
 
 class UnknownEventAction(AgentAction[UnknownEvent]):
     @override
     def run(self, event: UnknownEvent, id: str) -> ActionResult:
```

### Comparing `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/agent.py` & `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/agent.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/cli.py` & `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/cli.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/config.py` & `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/config.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/event_handler.py` & `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/event_handler.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/exceptions.py` & `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py` & `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/message_service/subscriber.py` & `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/message_service/subscriber.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/models.py` & `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/models.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/agent/run.py` & `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/run.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/logging/README.md` & `great_expectations_cloud-20240424.0/great_expectations_cloud/logging/README.md`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240423.0.dev0/great_expectations_cloud/logging/logging_cfg.py` & `great_expectations_cloud-20240424.0/great_expectations_cloud/logging/logging_cfg.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240423.0.dev0/pyproject.toml` & `great_expectations_cloud-20240424.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "great_expectations_cloud"
-version = "20240423.0.dev0"
+version = "20240424.0"
 description = "Great Expectations Cloud"
 authors = ["The Great Expectations Team <team@greatexpectations.io>"]
 repository = "https://github.com/great-expectations/cloud"
 homepage = "https://greatexpectations.io"
 readme = "README.md"
 license = "Proprietary"
 classifiers = [
```

### Comparing `great_expectations_cloud-20240423.0.dev0/PKG-INFO` & `great_expectations_cloud-20240424.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: great_expectations_cloud
-Version: 20240423.0.dev0
+Version: 20240424.0
 Summary: Great Expectations Cloud
 Home-page: https://greatexpectations.io
 License: Proprietary
 Author: The Great Expectations Team
 Author-email: team@greatexpectations.io
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 3 - Alpha
@@ -247,16 +247,16 @@
 2. [Containerize Agent](./.github/workflows/containerize-agent.yml) - This workflows runs on merge with `main` and will create a new Docker image and push it to Docker Hub and PyPi. It uses the version in `pyproject.toml`.
 
 A visual representation of the workflow is shown [here](./.github/workflows/agent_release_workflows.png)
 
 ### Dependabot and Releases/Pre-releases
 GitHub's Dependabot regularly checks our dependencies for vulnerabilty-based updates and proposes PRs to update dependency version numbers accordingly.
 
-Dependabot may only update the `poetry.lock` file. Before merging Dependabot suggestions, we should also ensure that `pyproject.toml` is aligned with version locked in the `poetry.lock` file by following the instructions above at [Updating `poetry.lock` dependencies](#updating-poetry.lock-dependencies).
+Dependabot may only update the `poetry.lock` file. If only changes to `poetry.lock` are made, this may be done in a pre-release.
 
-Note: if Dependabot suggests an update to a tool in the `[tool.poetry.group.dev.dependencies]` group in `pyproject.toml`, these changes can be merged in a pre-release version (i.e., a standard release is not required). While doing this, make sure any version references in the pre-commit config `.pre-commit-config.yaml` are kept in sync (e.g., ruff).
-
-For other dependency updates, a new release should be orchestrated. This includes updates in the following sections:
-
-- `[tool.poetry.dependencies]`
-- `[tool.poetry.group.*.dependencies]` where `*` is the name of the group (not including the `dev` group)
+For changes to the `pyproject.toml` file:
+- If the version of a tool in the `[tool.poetry.group.dev.dependencies]` group is updated, this may be done in a pre-release.
+   -  While doing this, make sure any version references in the pre-commit config `.pre-commit-config.yaml` are kept in sync (e.g., ruff).
+- For other dependency updates, a new release should be orchestrated. This includes updates in the following sections:
+  - `[tool.poetry.dependencies]`
+  - `[tool.poetry.group.*.dependencies]` where `*` is the name of the group (not including the `dev` group)
```

