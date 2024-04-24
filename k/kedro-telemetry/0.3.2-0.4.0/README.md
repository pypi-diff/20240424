# Comparing `tmp/kedro-telemetry-0.3.2.tar.gz` & `tmp/kedro_telemetry-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-telemetry-0.3.2.tar", last modified: Thu Feb 29 11:32:05 2024, max compression
+gzip compressed data, was "kedro_telemetry-0.4.0.tar", last modified: Wed Apr 24 12:33:38 2024, max compression
```

## Comparing `kedro-telemetry-0.3.2.tar` & `kedro_telemetry-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:32:05.375582 kedro-telemetry-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-02-29 11:32:05.375582 kedro-telemetry-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-02-29 11:31:51.000000 kedro-telemetry-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:32:05.371582 kedro-telemetry-0.3.2/kedro_telemetry/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-29 11:31:51.000000 kedro-telemetry-0.3.2/kedro_telemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-02-29 11:31:51.000000 kedro-telemetry-0.3.2/kedro_telemetry/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-02-29 11:31:51.000000 kedro-telemetry-0.3.2/kedro_telemetry/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:32:05.375582 kedro-telemetry-0.3.2/kedro_telemetry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-02-29 11:32:05.000000 kedro-telemetry-0.3.2/kedro_telemetry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-02-29 11:32:05.000000 kedro-telemetry-0.3.2/kedro_telemetry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 11:32:05.000000 kedro-telemetry-0.3.2/kedro_telemetry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-29 11:32:05.000000 kedro-telemetry-0.3.2/kedro_telemetry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 11:32:05.000000 kedro-telemetry-0.3.2/kedro_telemetry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-02-29 11:32:05.000000 kedro-telemetry-0.3.2/kedro_telemetry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-29 11:32:05.000000 kedro-telemetry-0.3.2/kedro_telemetry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-02-29 11:31:51.000000 kedro-telemetry-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 11:32:05.375582 kedro-telemetry-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:32:05.375582 kedro-telemetry-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-02-29 11:31:51.000000 kedro-telemetry-0.3.2/tests/test_masking.py
--rw-r--r--   0 runner    (1001) docker     (127)    24356 2024-02-29 11:31:51.000000 kedro-telemetry-0.3.2/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:33:38.273292 kedro_telemetry-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-24 12:33:38.273292 kedro_telemetry-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-24 12:33:29.000000 kedro_telemetry-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:33:38.269292 kedro_telemetry-0.4.0/kedro_telemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 12:33:29.000000 kedro_telemetry-0.4.0/kedro_telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-04-24 12:33:29.000000 kedro_telemetry-0.4.0/kedro_telemetry/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12542 2024-04-24 12:33:29.000000 kedro_telemetry-0.4.0/kedro_telemetry/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:33:38.273292 kedro_telemetry-0.4.0/kedro_telemetry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-24 12:33:38.000000 kedro_telemetry-0.4.0/kedro_telemetry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-24 12:33:38.000000 kedro_telemetry-0.4.0/kedro_telemetry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:33:38.000000 kedro_telemetry-0.4.0/kedro_telemetry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-24 12:33:38.000000 kedro_telemetry-0.4.0/kedro_telemetry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:33:38.000000 kedro_telemetry-0.4.0/kedro_telemetry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-24 12:33:38.000000 kedro_telemetry-0.4.0/kedro_telemetry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 12:33:38.000000 kedro_telemetry-0.4.0/kedro_telemetry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-24 12:33:29.000000 kedro_telemetry-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 12:33:38.273292 kedro_telemetry-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:33:38.273292 kedro_telemetry-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7938 2024-04-24 12:33:29.000000 kedro_telemetry-0.4.0/tests/test_masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24378 2024-04-24 12:33:29.000000 kedro_telemetry-0.4.0/tests/test_plugin.py
```

### Comparing `kedro-telemetry-0.3.2/PKG-INFO` & `kedro_telemetry-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: kedro-telemetry
-Version: 0.3.2
+Version: 0.4.0
 Summary: Kedro-Telemetry
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Source, https://github.com/kedro-org/kedro-plugins/tree/main/kedro-telemetry
 Project-URL: Documentation, https://github.com/kedro-org/kedro-plugins/blob/main/kedro-telemetry/README.md
 Project-URL: Tracker, https://github.com/kedro-org/kedro-plugins/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: kedro>=0.18.0
 Requires-Dist: requests~=2.20
+Requires-Dist: appdirs>=1.4.4
 Provides-Extra: test
 Requires-Dist: bandit<2.0,>=1.6.2; extra == "test"
-Requires-Dist: behave; extra == "test"
 Requires-Dist: black~=22.0; extra == "test"
+Requires-Dist: mypy~=1.0; extra == "test"
 Requires-Dist: pre-commit>=2.9.2; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: pytest-xdist[psutil]~=2.2.1; extra == "test"
 Requires-Dist: PyYAML==5.3.1; extra == "test"
 Requires-Dist: trufflehog<3.0,>=2.1.0; extra == "test"
 Requires-Dist: ruff~=0.0.290; extra == "test"
 Requires-Dist: wheel; extra == "test"
+Requires-Dist: types-requests; extra == "test"
+Requires-Dist: types-PyYAML; extra == "test"
+Requires-Dist: types-toml; extra == "test"
 
 # Kedro-Telemetry
 
 [![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://pypi.org/project/kedro-telemetry/)
 [![PyPI version](https://badge.fury.io/py/kedro-telemetry.svg)](https://pypi.org/project/kedro-telemetry/)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
```

### Comparing `kedro-telemetry-0.3.2/README.md` & `kedro_telemetry-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `kedro-telemetry-0.3.2/kedro_telemetry/masking.py` & `kedro_telemetry-0.4.0/kedro_telemetry/masking.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Module containing command masking functionality."""
-from typing import Any, Dict, Iterator, List, Union
+from __future__ import annotations
+
+from typing import Any, Iterator
 
 import click
 
 MASK = "*****"
 
 
 def _recurse_cli(
-    cli_element: Union[click.Command, click.Group, click.CommandCollection],
+    cli_element: click.Command | (click.Group | (click.CommandCollection | None)),
     ctx: click.Context,
-    io_dict: Dict[str, Any],
+    io_dict: dict[str | None, Any],
     get_help: bool = False,
 ) -> None:
     """
     Code copied over from kedro.tools.cli to maintain backwards compatibility
     with previous versions of kedro (<0.17.5).
 
     Recursive function that checks the type of the command (key) and decides:
@@ -34,15 +36,15 @@
     Returns:
         None (underlying `io_dict` is mutated by the recursion)
     """
     if isinstance(cli_element, (click.Group, click.CommandCollection)):
         element_name = cli_element.name or "kedro"
         io_dict[element_name] = {}
         for command_name in cli_element.list_commands(ctx):
-            _recurse_cli(  # type: ignore
+            _recurse_cli(
                 cli_element.get_command(ctx, command_name),
                 ctx,
                 io_dict[element_name],
                 get_help,
             )
         if not get_help:
             nested_parameter_list = [
@@ -61,29 +63,31 @@
             ]
             io_dict[cli_element.name] = dict.fromkeys(
                 [item for sublist in nested_parameter_list for item in sublist], None
             )
 
 
 def _get_cli_structure(
-    cli_obj: Union[click.Command, click.Group, click.CommandCollection],
+    cli_obj: click.Command | (click.Group | click.CommandCollection),
     get_help: bool = False,
-) -> Dict[str, Any]:
+) -> dict[str | None, Any]:
     """Code copied over from kedro.tools.cli to maintain backwards compatibility
     with previous versions of kedro (<0.17.5).
     Convenience wrapper function for `_recurse_cli` to work within
     `click.Context` and return a `dict`.
     """
-    output: Dict[str, Any] = {}
+    output: dict[str | None, Any] = {}
     with click.Context(cli_obj) as ctx:  # type: ignore
         _recurse_cli(cli_obj, ctx, output, get_help)
     return output
 
 
-def _mask_kedro_cli(cli_struct: Dict[str, Any], command_args: List[str]) -> List[str]:
+def _mask_kedro_cli(
+    cli_struct: dict[str | None, Any], command_args: list[str]
+) -> list[str]:
     """Takes a dynamic vocabulary (based on `KedroCLI`) and returns
     a masked CLI input"""
     output = []
 
     # Preserve the initial part of the command until parameters sections begin
     arg_index = 0
     current_CLI = cli_struct.get("kedro", {})
@@ -110,15 +114,15 @@
                 output.append(MASK)
         else:
             output.append(MASK)
 
     return output
 
 
-def _recursive_items(dictionary: Dict[Any, Any]) -> Iterator[Any]:
+def _recursive_items(dictionary: dict[Any, Any]) -> Iterator[Any]:
     for key, value in dictionary.items():
         if isinstance(value, dict):
             yield key
             yield from _recursive_items(value)
         else:
             yield key
             yield value
```

### Comparing `kedro-telemetry-0.3.2/kedro_telemetry/plugin.py` & `kedro_telemetry-0.4.0/kedro_telemetry/plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """Kedro Telemetry plugin for collecting Kedro usage data."""
 
-import getpass
+from __future__ import annotations
+
 import hashlib
 import json
 import logging
 import os
 import sys
+import uuid
 from copy import deepcopy
 from datetime import datetime
 from pathlib import Path
-from typing import Any, Dict, List
+from typing import Any
 
 import click
 import requests
 import toml
 import yaml
+from appdirs import user_config_dir
 from kedro import __version__ as KEDRO_VERSION
 from kedro.framework.cli.cli import KedroCLI
 from kedro.framework.cli.hooks import cli_hook_impl
 from kedro.framework.hooks import hook_impl
 from kedro.framework.project import PACKAGE_NAME, pipelines
 from kedro.framework.startup import ProjectMetadata
 from kedro.io.data_catalog import DataCatalog
@@ -37,40 +40,71 @@
     "JENKINS_URL",  # https://www.jenkins.io/doc/book/pipeline/jenkinsfile/#using-environment-variables
     "CODEBUILD_BUILD_ID",  # https://docs.aws.amazon.com/codebuild/latest/userguide/build-env-ref-env-vars.html
     "CIRCLECI",  # https://circleci.com/docs/variables/#built-in-environment-variables
     "TRAVIS",  # https://docs.travis-ci.com/user/environment-variables/#default-environment-variables
     "BUILDKITE",  # https://buildkite.com/docs/pipelines/environment-variables
 }
 TIMESTAMP_FORMAT = "%Y-%m-%dT%H:%M:%S.%fZ"
+CONFIG_FILENAME = "telemetry.toml"
 
 logger = logging.getLogger(__name__)
 
 
 def _hash(string: str) -> str:
     return hashlib.sha512(bytes(string, encoding="utf8")).hexdigest()
 
 
-def _get_hashed_username():
+def _get_or_create_uuid() -> str:
+    """
+    Reads a UUID from a configuration file or generates and saves a new one if not present.
+    """
+    config_path = user_config_dir("kedro")
+    full_path = os.path.join(config_path, CONFIG_FILENAME)
+
     try:
-        username = getpass.getuser()
-        return _hash(username)
-    except Exception as exc:
-        logger.warning(
-            "Something went wrong with getting the username. Exception: %s",
-            exc,
-        )
+        if os.path.exists(full_path):
+            with open(full_path) as f:
+                config = toml.load(f)
+
+                if "telemetry" in config and "uuid" in config["telemetry"]:
+                    return uuid.UUID(config["telemetry"]["uuid"]).hex
+
+        # Generate a new UUID and save it to the config file
+        new_uuid = _generate_new_uuid(full_path)
+
+        return new_uuid
+
+    except Exception as e:
+        logging.error(f"Failed to retrieve UUID: {e}")
+        return ""
+
+
+def _generate_new_uuid(full_path: str) -> str:
+    try:
+        config: dict[str, dict[str, Any]] = {}
+        config["telemetry"] = {}
+        new_uuid = uuid.uuid4().hex
+        config["telemetry"]["uuid"] = new_uuid
+
+        os.makedirs(os.path.dirname(full_path), exist_ok=True)
+        with open(full_path, "w") as f:
+            toml.dump(config, f)
+
+        return new_uuid
+    except Exception as e:
+        logging.error(f"Failed to create UUID: {e}")
         return ""
 
 
 class KedroTelemetryCLIHooks:
     """Hook to send CLI command data to Heap"""
 
     @cli_hook_impl
     def before_command_run(
-        self, project_metadata: ProjectMetadata, command_args: List[str]
+        self, project_metadata: ProjectMetadata, command_args: list[str]
     ):
         """Hook implementation to send command run data to Heap"""
         try:
             if not project_metadata:  # in package mode
                 return
 
             consent = _check_for_telemetry_consent(project_metadata.project_path)
@@ -78,42 +112,42 @@
                 logger.debug(
                     "Kedro-Telemetry is installed, but you have opted out of "
                     "sharing usage analytics so none will be collected.",
                 )
                 return
 
             # get KedroCLI and its structure from actual project root
-            cli = KedroCLI(project_path=Path.cwd())
+            cli = KedroCLI(project_path=project_metadata.project_path)
             cli_struct = _get_cli_structure(cli_obj=cli, get_help=False)
             masked_command_args = _mask_kedro_cli(
                 cli_struct=cli_struct, command_args=command_args
             )
             main_command = masked_command_args[0] if masked_command_args else "kedro"
 
             logger.debug("You have opted into product usage analytics.")
-            hashed_username = _get_hashed_username()
+            user_uuid = _get_or_create_uuid()
             project_properties = _get_project_properties(
-                hashed_username, project_metadata.project_path
+                user_uuid, project_metadata.project_path
             )
             cli_properties = _format_user_cli_data(
                 project_properties, masked_command_args
             )
 
             _send_heap_event(
                 event_name=f"Command run: {main_command}",
-                identity=hashed_username,
+                identity=user_uuid,
                 properties=cli_properties,
             )
 
             # send generic event too, so it's easier in data processing
             generic_properties = deepcopy(cli_properties)
             generic_properties["main_command"] = main_command
             _send_heap_event(
                 event_name="CLI command",
-                identity=hashed_username,
+                identity=user_uuid,
                 properties=generic_properties,
             )
         except Exception as exc:
             logger.warning(
                 "Something went wrong in hook implementation to send command run data to Heap. "
                 "Exception: %s",
                 exc,
@@ -137,40 +171,40 @@
                 "sharing usage analytics so none will be collected.",
             )
             return
 
         logger.debug("You have opted into product usage analytics.")
 
         default_pipeline = pipelines.get("__default__")  # __default__
-        hashed_username = _get_hashed_username()
+        user_uuid = _get_or_create_uuid()
 
-        project_properties = _get_project_properties(hashed_username, self.project_path)
+        project_properties = _get_project_properties(user_uuid, self.project_path)
 
         project_statistics_properties = _format_project_statistics_data(
             project_properties, catalog, default_pipeline, pipelines
         )
         _send_heap_event(
             event_name="Kedro Project Statistics",
-            identity=hashed_username,
+            identity=user_uuid,
             properties=project_statistics_properties,
         )
 
 
 def _is_known_ci_env(known_ci_env_var_keys=KNOWN_CI_ENV_VAR_KEYS):
     # Most CI tools will set the CI environment variable to true
     if os.getenv("CI") == "true":
         return True
     # Not all CI tools follow this convention, we can check through those that don't
     return any(os.getenv(key) for key in known_ci_env_var_keys)
 
 
-def _get_project_properties(hashed_username: str, project_path: str) -> Dict:
-    hashed_package_name = _hash(PACKAGE_NAME) if PACKAGE_NAME else "undefined"
+def _get_project_properties(user_uuid: str, project_path: Path) -> dict:
+    hashed_package_name = _hash(str(PACKAGE_NAME)) if PACKAGE_NAME else "undefined"
     properties = {
-        "username": hashed_username,
+        "username": user_uuid,
         "package_name": hashed_package_name,
         "project_version": KEDRO_VERSION,
         "telemetry_version": TELEMETRY_VERSION,
         "python_version": sys.version,
         "os": sys.platform,
         "is_ci_env": _is_known_ci_env(),
     }
@@ -191,15 +225,15 @@
                 ]
 
     return properties
 
 
 def _format_user_cli_data(
     properties: dict,
-    command_args: List[str],
+    command_args: list[str],
 ):
     """Add format CLI command data to send to Heap."""
     cli_properties = properties.copy()
     cli_properties["command"] = (
         f"kedro {' '.join(command_args)}" if command_args else "kedro"
     )
     return cli_properties
@@ -231,15 +265,15 @@
     This will be the development ID if it's set as an
     environment variable, otherwise it will be the production ID.
     """
     return os.environ.get("HEAP_APPID_DEV", HEAP_APPID_PROD)
 
 
 def _send_heap_event(
-    event_name: str, identity: str, properties: Dict[str, Any] = None
+    event_name: str, identity: str, properties: dict[str, Any] | None = None
 ) -> None:
     data = {
         "app_id": _get_heap_app_id(),
         "event": event_name,
         "timestamp": datetime.now().strftime(TIMESTAMP_FORMAT),
         "properties": properties or {},
     }
```

### Comparing `kedro-telemetry-0.3.2/kedro_telemetry.egg-info/PKG-INFO` & `kedro_telemetry-0.4.0/kedro_telemetry.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: kedro-telemetry
-Version: 0.3.2
+Version: 0.4.0
 Summary: Kedro-Telemetry
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Source, https://github.com/kedro-org/kedro-plugins/tree/main/kedro-telemetry
 Project-URL: Documentation, https://github.com/kedro-org/kedro-plugins/blob/main/kedro-telemetry/README.md
 Project-URL: Tracker, https://github.com/kedro-org/kedro-plugins/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: kedro>=0.18.0
 Requires-Dist: requests~=2.20
+Requires-Dist: appdirs>=1.4.4
 Provides-Extra: test
 Requires-Dist: bandit<2.0,>=1.6.2; extra == "test"
-Requires-Dist: behave; extra == "test"
 Requires-Dist: black~=22.0; extra == "test"
+Requires-Dist: mypy~=1.0; extra == "test"
 Requires-Dist: pre-commit>=2.9.2; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: pytest-xdist[psutil]~=2.2.1; extra == "test"
 Requires-Dist: PyYAML==5.3.1; extra == "test"
 Requires-Dist: trufflehog<3.0,>=2.1.0; extra == "test"
 Requires-Dist: ruff~=0.0.290; extra == "test"
 Requires-Dist: wheel; extra == "test"
+Requires-Dist: types-requests; extra == "test"
+Requires-Dist: types-PyYAML; extra == "test"
+Requires-Dist: types-toml; extra == "test"
 
 # Kedro-Telemetry
 
 [![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://pypi.org/project/kedro-telemetry/)
 [![PyPI version](https://badge.fury.io/py/kedro-telemetry.svg)](https://pypi.org/project/kedro-telemetry/)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
```

### Comparing `kedro-telemetry-0.3.2/pyproject.toml` & `kedro_telemetry-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -9,36 +9,41 @@
 ]
 description = "Kedro-Telemetry"
 requires-python = ">=3.8"
 license = {text = "Apache Software License (Apache 2.0)"}
 dependencies = [
     "kedro>=0.18.0",
     "requests~=2.20",
+    "appdirs>=1.4.4",
 ]
 dynamic = ["readme", "version"]
 
 [project.urls]
 Source = "https://github.com/kedro-org/kedro-plugins/tree/main/kedro-telemetry"
 Documentation = "https://github.com/kedro-org/kedro-plugins/blob/main/kedro-telemetry/README.md"
 Tracker = "https://github.com/kedro-org/kedro-plugins/issues"
 
 [project.optional-dependencies]
 test = [
     "bandit>=1.6.2, <2.0",
-    "behave",
     "black~=22.0",
+    "mypy~=1.0",
     "pre-commit>=2.9.2",
     "pytest",
     "pytest-cov",
     "pytest-mock",
     "pytest-xdist[psutil]~=2.2.1",
     "PyYAML==5.3.1", # Temporary fix, to be removed
     "trufflehog>=2.1.0, <3.0",
     "ruff~=0.0.290",
-    "wheel"
+    "wheel",
+    # mypy requirements
+    "types-requests",
+    "types-PyYAML",
+    "types-toml",
 ]
 
 [project.entry-points."kedro.cli_hooks"]
 kedro-telemetry = "kedro_telemetry.plugin:cli_hooks"
 
 [project.entry-points."kedro.hooks"]
 kedro-telemetry = "kedro_telemetry.plugin:project_hooks"
```

### Comparing `kedro-telemetry-0.3.2/tests/test_masking.py` & `kedro_telemetry-0.4.0/tests/test_masking.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Testing module for CLI tools"""
+
 import shutil
 from collections import namedtuple
 from pathlib import Path
 
 import pytest
 from kedro import __version__ as kedro_version
 from kedro.framework.cli.cli import KedroCLI, cli
@@ -105,17 +106,19 @@
                 "-s",
                 "--checkout",
                 "--directory",
                 "--help",
                 "--example",
                 "--name",
                 "--tools",
+                "--telemetry",
                 "-e",
                 "-n",
                 "-t",
+                "-tc",
             ]
         )
         # now check that once params and args are reached, the values are None
         assert raw_cli_structure["kedro"]["new"]["--starter"] is None
         assert raw_cli_structure["kedro"]["new"]["--checkout"] is None
         assert raw_cli_structure["kedro"]["new"]["--help"] is None
         assert raw_cli_structure["kedro"]["new"]["-c"] is None
```

### Comparing `kedro-telemetry-0.3.2/tests/test_plugin.py` & `kedro_telemetry-0.4.0/tests/test_plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -127,24 +127,24 @@
             "kedro_telemetry.plugin._check_for_telemetry_consent", return_value=True
         )
         mocker.patch("kedro_telemetry.plugin._is_known_ci_env", return_value=True)
         mocked_anon_id = mocker.patch("kedro_telemetry.plugin._hash")
         mocked_anon_id.return_value = "digested"
         mocker.patch("kedro_telemetry.plugin.PACKAGE_NAME", "spaceflights")
         mocker.patch(
-            "kedro_telemetry.plugin._get_hashed_username",
-            return_value="hashed_username",
+            "kedro_telemetry.plugin._get_or_create_uuid",
+            return_value="user_uuid",
         )
 
         mocked_heap_call = mocker.patch("kedro_telemetry.plugin._send_heap_event")
         telemetry_hook = KedroTelemetryCLIHooks()
         command_args = ["--version"]
         telemetry_hook.before_command_run(fake_metadata, command_args)
         expected_properties = {
-            "username": "hashed_username",
+            "username": "user_uuid",
             "package_name": "digested",
             "project_version": kedro_version,
             "telemetry_version": TELEMETRY_VERSION,
             "python_version": sys.version,
             "os": sys.platform,
             "command": "kedro --version",
             "is_ci_env": True,
@@ -153,46 +153,46 @@
             **expected_properties,
             "main_command": "--version",
         }
 
         expected_calls = [
             mocker.call(
                 event_name="Command run: --version",
-                identity="hashed_username",
+                identity="user_uuid",
                 properties=expected_properties,
             ),
             mocker.call(
                 event_name="CLI command",
-                identity="hashed_username",
+                identity="user_uuid",
                 properties=generic_properties,
             ),
         ]
         assert mocked_heap_call.call_args_list == expected_calls
 
     def test_before_command_run_with_tools(self, mocker, fake_metadata):
         mocker.patch(
             "kedro_telemetry.plugin._check_for_telemetry_consent", return_value=True
         )
         mocker.patch("kedro_telemetry.plugin._is_known_ci_env", return_value=True)
         mocked_anon_id = mocker.patch("kedro_telemetry.plugin._hash")
         mocked_anon_id.return_value = "digested"
         mocker.patch("kedro_telemetry.plugin.PACKAGE_NAME", "spaceflights")
         mocker.patch(
-            "kedro_telemetry.plugin._get_hashed_username",
-            return_value="hashed_username",
+            "kedro_telemetry.plugin._get_or_create_uuid",
+            return_value="user_uuid",
         )
 
         mocked_heap_call = mocker.patch("kedro_telemetry.plugin._send_heap_event")
         mocker.patch("builtins.open", mocker.mock_open(read_data=MOCK_PYPROJECT_TOOLS))
         mocker.patch("pathlib.Path.exists", return_value=True)
         telemetry_hook = KedroTelemetryCLIHooks()
         command_args = ["--version"]
         telemetry_hook.before_command_run(fake_metadata, command_args)
         expected_properties = {
-            "username": "hashed_username",
+            "username": "user_uuid",
             "package_name": "digested",
             "project_version": kedro_version,
             "telemetry_version": TELEMETRY_VERSION,
             "python_version": sys.version,
             "os": sys.platform,
             "is_ci_env": True,
             "command": "kedro --version",
@@ -203,40 +203,44 @@
             **expected_properties,
             "main_command": "--version",
         }
 
         expected_calls = [
             mocker.call(
                 event_name="Command run: --version",
-                identity="hashed_username",
+                identity="user_uuid",
                 properties=expected_properties,
             ),
             mocker.call(
                 event_name="CLI command",
-                identity="hashed_username",
+                identity="user_uuid",
                 properties=generic_properties,
             ),
         ]
         assert mocked_heap_call.call_args_list == expected_calls
 
     def test_before_command_run_empty_args(self, mocker, fake_metadata):
         mocker.patch(
             "kedro_telemetry.plugin._check_for_telemetry_consent", return_value=True
         )
         mocker.patch("kedro_telemetry.plugin._is_known_ci_env", return_value=True)
         mocked_anon_id = mocker.patch("kedro_telemetry.plugin._hash")
         mocked_anon_id.return_value = "digested"
         mocker.patch("kedro_telemetry.plugin.PACKAGE_NAME", "spaceflights")
+        mocker.patch(
+            "kedro_telemetry.plugin._get_or_create_uuid",
+            return_value="user_uuid",
+        )
 
         mocked_heap_call = mocker.patch("kedro_telemetry.plugin._send_heap_event")
         telemetry_hook = KedroTelemetryCLIHooks()
         command_args = []
         telemetry_hook.before_command_run(fake_metadata, command_args)
         expected_properties = {
-            "username": "digested",
+            "username": "user_uuid",
             "package_name": "digested",
             "project_version": kedro_version,
             "telemetry_version": TELEMETRY_VERSION,
             "python_version": sys.version,
             "os": sys.platform,
             "is_ci_env": True,
             "command": "kedro",
@@ -245,20 +249,20 @@
             "main_command": "kedro",
             **expected_properties,
         }
 
         expected_calls = [
             mocker.call(
                 event_name="Command run: kedro",
-                identity="digested",
+                identity="user_uuid",
                 properties=expected_properties,
             ),
             mocker.call(
                 event_name="CLI command",
-                identity="digested",
+                identity="user_uuid",
                 properties=generic_properties,
             ),
         ]
 
         assert mocked_heap_call.call_args_list == expected_calls
 
     def test_before_command_run_no_consent_given(self, mocker, fake_metadata):
@@ -292,15 +296,15 @@
         mocker.patch(
             "kedro_telemetry.plugin._check_for_telemetry_consent", return_value=True
         )
         mocker.patch("kedro_telemetry.plugin._is_known_ci_env", return_value=True)
         mocked_anon_id = mocker.patch("kedro_telemetry.plugin._hash")
         mocked_anon_id.return_value = "digested"
         mocker.patch("kedro_telemetry.plugin.PACKAGE_NAME", "spaceflights")
-        mocker.patch("getpass.getuser", side_effect=Exception)
+        mocker.patch("builtins.open", side_effect=Exception)
 
         mocked_heap_call = mocker.patch("kedro_telemetry.plugin._send_heap_event")
         telemetry_hook = KedroTelemetryCLIHooks()
         command_args = ["--version"]
         telemetry_hook.before_command_run(fake_metadata, command_args)
         expected_properties = {
             "username": "",
@@ -470,28 +474,28 @@
         mocker.patch(
             "kedro_telemetry.plugin._check_for_telemetry_consent", return_value=True
         )
         mocker.patch("kedro_telemetry.plugin._is_known_ci_env", return_value=True)
         mocker.patch("kedro_telemetry.plugin._hash", return_value="digested")
         mocker.patch("kedro_telemetry.plugin.PACKAGE_NAME", "spaceflights")
         mocker.patch(
-            "kedro_telemetry.plugin._get_hashed_username",
-            return_value="hashed_username",
+            "kedro_telemetry.plugin._get_or_create_uuid",
+            return_value="user_uuid",
         )
         mocked_heap_call = mocker.patch("kedro_telemetry.plugin._send_heap_event")
         mocker.patch("kedro_telemetry.plugin.open")
         mocker.patch("kedro_telemetry.plugin.toml.load")
 
         # Without CLI invoked - i.e. `session.run` in Jupyter/IPython
         telemetry_hook = KedroTelemetryProjectHooks()
         telemetry_hook.after_context_created(fake_context)
         telemetry_hook.after_catalog_created(fake_catalog)
 
         project_properties = {
-            "username": "hashed_username",
+            "username": "user_uuid",
             "package_name": "digested",
             "project_version": kedro_version,
             "telemetry_version": TELEMETRY_VERSION,
             "python_version": sys.version,
             "os": sys.platform,
             "is_ci_env": True,
         }
@@ -500,15 +504,15 @@
             "number_of_nodes": 2,
             "number_of_pipelines": 2,
         }
         expected_properties = {**project_properties, **project_statistics}
 
         expected_call = mocker.call(
             event_name="Kedro Project Statistics",
-            identity="hashed_username",
+            identity="user_uuid",
             properties=expected_properties,
         )
 
         # The 1st call is the Project Hook without CLI
         assert mocked_heap_call.call_args_list[0] == expected_call
 
     def test_after_context_created_with_kedro_run(  # noqa: PLR0913
@@ -526,31 +530,31 @@
         mocker.patch(
             "kedro_telemetry.plugin._check_for_telemetry_consent", return_value=True
         )
         mocker.patch("kedro_telemetry.plugin._is_known_ci_env", return_value=True)
         mocker.patch("kedro_telemetry.plugin._hash", return_value="digested")
         mocker.patch("kedro_telemetry.plugin.PACKAGE_NAME", "spaceflights")
         mocker.patch(
-            "kedro_telemetry.plugin._get_hashed_username",
-            return_value="hashed_username",
+            "kedro_telemetry.plugin._get_or_create_uuid",
+            return_value="user_uuid",
         )
         mocked_heap_call = mocker.patch("kedro_telemetry.plugin._send_heap_event")
         mocker.patch("kedro_telemetry.plugin.toml.load")
         # CLI run first
         telemetry_cli_hook = KedroTelemetryCLIHooks()
         command_args = ["--version"]
         telemetry_cli_hook.before_command_run(fake_metadata, command_args)
 
         # Follow by project run
         telemetry_hook = KedroTelemetryProjectHooks()
         telemetry_hook.after_context_created(fake_context)
         telemetry_hook.after_catalog_created(fake_catalog)
 
         project_properties = {
-            "username": "hashed_username",
+            "username": "user_uuid",
             "package_name": "digested",
             "project_version": kedro_version,
             "telemetry_version": TELEMETRY_VERSION,
             "python_version": sys.version,
             "os": sys.platform,
             "is_ci_env": True,
         }
@@ -559,15 +563,15 @@
             "number_of_nodes": 2,
             "number_of_pipelines": 2,
         }
         expected_properties = {**project_properties, **project_statistics}
 
         expected_call = mocker.call(
             event_name="Kedro Project Statistics",
-            identity="hashed_username",
+            identity="user_uuid",
             properties=expected_properties,
         )
 
         # CLI hook makes the first 2 calls, the 3rd one is the Project hook
         assert mocked_heap_call.call_args_list[2] == expected_call
 
     def test_after_context_created_with_kedro_run_and_tools(  # noqa: PLR0913
@@ -585,16 +589,16 @@
         mocker.patch(
             "kedro_telemetry.plugin._check_for_telemetry_consent", return_value=True
         )
         mocker.patch("kedro_telemetry.plugin._is_known_ci_env", return_value=True)
         mocker.patch("kedro_telemetry.plugin._hash", return_value="digested")
         mocker.patch("kedro_telemetry.plugin.PACKAGE_NAME", "spaceflights")
         mocker.patch(
-            "kedro_telemetry.plugin._get_hashed_username",
-            return_value="hashed_username",
+            "kedro_telemetry.plugin._get_or_create_uuid",
+            return_value="user_uuid",
         )
         mocked_heap_call = mocker.patch("kedro_telemetry.plugin._send_heap_event")
         mocker.patch("builtins.open", mocker.mock_open(read_data=MOCK_PYPROJECT_TOOLS))
         mocker.patch("pathlib.Path.exists", return_value=True)
 
         # CLI run first
         telemetry_cli_hook = KedroTelemetryCLIHooks()
@@ -603,15 +607,15 @@
 
         # Follow by project run
         telemetry_hook = KedroTelemetryProjectHooks()
         telemetry_hook.after_context_created(fake_context)
         telemetry_hook.after_catalog_created(fake_catalog)
 
         project_properties = {
-            "username": "hashed_username",
+            "username": "user_uuid",
             "package_name": "digested",
             "project_version": kedro_version,
             "telemetry_version": TELEMETRY_VERSION,
             "python_version": sys.version,
             "os": sys.platform,
             "is_ci_env": True,
             "tools": "Linting, Testing, Custom Logging, Documentation, Data Structure, PySpark",
@@ -622,15 +626,15 @@
             "number_of_nodes": 2,
             "number_of_pipelines": 2,
         }
         expected_properties = {**project_properties, **project_statistics}
 
         expected_call = mocker.call(
             event_name="Kedro Project Statistics",
-            identity="hashed_username",
+            identity="user_uuid",
             properties=expected_properties,
         )
 
         # CLI hook makes the first 2 calls, the 3rd one is the Project hook
         assert mocked_heap_call.call_args_list[2] == expected_call
 
     def test_after_context_created_no_consent_given(self, mocker):
```

