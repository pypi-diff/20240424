# Comparing `tmp/kedro-docker-0.5.0.tar.gz` & `tmp/kedro_docker-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-docker-0.5.0.tar", last modified: Thu Dec 21 18:21:46 2023, max compression
+gzip compressed data, was "kedro_docker-0.6.0.tar", last modified: Wed Apr 24 13:47:23 2024, max compression
```

## Comparing `kedro-docker-0.5.0.tar` & `kedro_docker-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:21:46.517580 kedro-docker-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-21 18:21:36.000000 kedro-docker-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12557 2023-12-21 18:21:46.517580 kedro-docker-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11295 2023-12-21 18:21:36.000000 kedro-docker-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:21:46.513580 kedro-docker-0.5.0/kedro_docker/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-21 18:21:36.000000 kedro-docker-0.5.0/kedro_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7528 2023-12-21 18:21:36.000000 kedro-docker-0.5.0/kedro_docker/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11066 2023-12-21 18:21:36.000000 kedro-docker-0.5.0/kedro_docker/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:21:46.517580 kedro-docker-0.5.0/kedro_docker/template/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2023-12-21 18:21:36.000000 kedro-docker-0.5.0/kedro_docker/template/.dive-ci
--rw-r--r--   0 runner    (1001) docker     (127)      428 2023-12-21 18:21:36.000000 kedro-docker-0.5.0/kedro_docker/template/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      664 2023-12-21 18:21:36.000000 kedro-docker-0.5.0/kedro_docker/template/Dockerfile.simple
--rw-r--r--   0 runner    (1001) docker     (127)      812 2023-12-21 18:21:36.000000 kedro-docker-0.5.0/kedro_docker/template/Dockerfile.spark
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:21:46.517580 kedro-docker-0.5.0/kedro_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12557 2023-12-21 18:21:46.000000 kedro-docker-0.5.0/kedro_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      529 2023-12-21 18:21:46.000000 kedro-docker-0.5.0/kedro_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 18:21:46.000000 kedro-docker-0.5.0/kedro_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-21 18:21:46.000000 kedro-docker-0.5.0/kedro_docker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 18:21:46.000000 kedro-docker-0.5.0/kedro_docker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-12-21 18:21:46.000000 kedro-docker-0.5.0/kedro_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-21 18:21:46.000000 kedro-docker-0.5.0/kedro_docker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2023-12-21 18:21:36.000000 kedro-docker-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-21 18:21:46.517580 kedro-docker-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:21:46.517580 kedro-docker-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7151 2023-12-21 18:21:36.000000 kedro-docker-0.5.0/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:47:23.861069 kedro_docker-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-24 13:47:18.000000 kedro_docker-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12599 2024-04-24 13:47:23.861069 kedro_docker-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11295 2024-04-24 13:47:18.000000 kedro_docker-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:47:23.857069 kedro_docker-0.6.0/kedro_docker/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 13:47:18.000000 kedro_docker-0.6.0/kedro_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-04-24 13:47:18.000000 kedro_docker-0.6.0/kedro_docker/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11059 2024-04-24 13:47:18.000000 kedro_docker-0.6.0/kedro_docker/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:47:23.861069 kedro_docker-0.6.0/kedro_docker/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-24 13:47:18.000000 kedro_docker-0.6.0/kedro_docker/template/.dive-ci
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-24 13:47:18.000000 kedro_docker-0.6.0/kedro_docker/template/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-24 13:47:18.000000 kedro_docker-0.6.0/kedro_docker/template/Dockerfile.simple
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-24 13:47:18.000000 kedro_docker-0.6.0/kedro_docker/template/Dockerfile.spark
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:47:23.861069 kedro_docker-0.6.0/kedro_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12599 2024-04-24 13:47:23.000000 kedro_docker-0.6.0/kedro_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-24 13:47:23.000000 kedro_docker-0.6.0/kedro_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:47:23.000000 kedro_docker-0.6.0/kedro_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-24 13:47:23.000000 kedro_docker-0.6.0/kedro_docker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:47:23.000000 kedro_docker-0.6.0/kedro_docker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-24 13:47:23.000000 kedro_docker-0.6.0/kedro_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 13:47:23.000000 kedro_docker-0.6.0/kedro_docker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-24 13:47:18.000000 kedro_docker-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:47:23.861069 kedro_docker-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:47:23.861069 kedro_docker-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-24 13:47:18.000000 kedro_docker-0.6.0/tests/test_helpers.py
```

### Comparing `kedro-docker-0.5.0/PKG-INFO` & `kedro_docker-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-docker
-Version: 0.5.0
+Version: 0.6.0
 Summary: Kedro-Docker makes it easy to package Kedro projects with Docker.
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Source, https://github.com/kedro-org/kedro-plugins/tree/main/kedro-docker
 Project-URL: Documentation, https://github.com/kedro-org/kedro-plugins/blob/main/kedro-docker/README.md
 Project-URL: Tracker, https://github.com/kedro-org/kedro-plugins/issues
 Requires-Python: >=3.8
@@ -13,14 +13,15 @@
 Requires-Dist: kedro>=0.16.0
 Requires-Dist: semver~=2.10
 Provides-Extra: test
 Requires-Dist: bandit; extra == "test"
 Requires-Dist: behave; extra == "test"
 Requires-Dist: black~=22.0; extra == "test"
 Requires-Dist: docker; extra == "test"
+Requires-Dist: mypy~=1.0; extra == "test"
 Requires-Dist: pre-commit>=2.9.2; extra == "test"
 Requires-Dist: psutil; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: pytest-xdist[psutil]~=2.2.1; extra == "test"
 Requires-Dist: PyYAML<7.0,>=5.1; extra == "test"
```

### Comparing `kedro-docker-0.5.0/README.md` & `kedro_docker-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `kedro-docker-0.5.0/kedro_docker/helpers.py` & `kedro_docker-0.6.0/kedro_docker/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """ Utilities for use with click docker commands """
 
+from __future__ import annotations
+
 import os
 import re
 import shutil
 import socket
 import subprocess
 from importlib import import_module
 from itertools import chain
 from pathlib import Path, PurePosixPath
 from subprocess import DEVNULL, PIPE
-from typing import List, Sequence, Tuple, Union
+from typing import Sequence
 
 from click import secho
 from kedro.framework.cli.utils import KedroCliError
 
 
 def check_docker_image_exists(image: str):
     """
@@ -45,30 +47,30 @@
         container_root: Path to project root in the container (e.g., `/home/kedro`).
         volumes: List of volumes to mount.
 
     Yields:
         Tuple[str]: Tuple of the form: ('-v', 'host_path:container_path')
 
     """
-    host_root = Path(host_root).resolve()
-    container_root = PurePosixPath(container_root)
+    host_root_path = Path(host_root).resolve()
+    container_root_path = PurePosixPath(container_root)
     for volume in volumes:
-        hpath = host_root / volume  # host path
-        cpath = PurePosixPath(container_root) / volume  # container path
+        hpath = host_root_path / volume  # host path
+        cpath = PurePosixPath(container_root_path) / volume  # container path
         yield "-v", str(hpath) + ":" + str(cpath)
 
 
 def compose_docker_run_args(  # noqa: PLR0913
-    host_root: str = None,
-    container_root: str = None,
-    mount_volumes: Sequence[str] = None,
-    required_args: Sequence[Tuple[str, Union[str, None]]] = None,
-    optional_args: Sequence[Tuple[str, Union[str, None]]] = None,
-    user_args: Sequence[str] = None,
-) -> List[str]:
+    host_root: str | None = None,
+    container_root: str | None = None,
+    mount_volumes: Sequence[str] | None = None,
+    required_args: Sequence[tuple[str, str | None]] | None = None,
+    optional_args: Sequence[tuple[str, str | None]] | None = None,
+    user_args: Sequence[str] | None = None,
+) -> list[str]:
     """
     Make a list of arguments for the docker command.
 
     Args:
         host_root: Path project root on the host. It must be provided
             if `mount_volumes` are specified, optional otherwise.
         container_root: Path to project root in the container
@@ -89,15 +91,17 @@
 
     mount_volumes = mount_volumes or []
     required_args = required_args or []
     optional_args = optional_args or []
     user_args = user_args or []
     split_user_args = {ua.split("=", 1)[0] for ua in user_args}
 
-    def _add_args(name_: str, value_: str = None, force_: bool = False) -> List[str]:
+    def _add_args(
+        name_: str, value_: str | None = None, force_: bool = False
+    ) -> list[str]:
         """
         Add extra args to existing list of CLI args.
         Args:
             name_: Arg name to add.
             value_: Arg value to add, skipped if None.
             force_: Add the argument even if it's present in the current list of args.
 
@@ -120,15 +124,15 @@
         combined_args = list(chain.from_iterable(vol_gen))
     else:
         combined_args = []
     for arg_name, arg_value in required_args:
         combined_args += _add_args(arg_name, arg_value, True)
     for arg_name, arg_value in optional_args:
         combined_args += _add_args(arg_name, arg_value)
-    return combined_args + user_args
+    return combined_args + list(user_args)
 
 
 def make_container_name(image: str, suffix: str = "") -> str:
     """
     Make default container name for the given Docker image.
 
     Args:
@@ -169,15 +173,15 @@
             if verbose:
                 secho(f"Creating `{dest}`")
         else:
             msg = f"{dest_file} already exists and won't be overwritten."
             secho(msg, fg="yellow")
 
 
-def get_uid_gid(uid: int = None, gid: int = None) -> Tuple[int, int]:
+def get_uid_gid(uid: int | None = None, gid: int | None = None) -> tuple[int, int]:
     """
     Get UID and GID to be passed into the Docker container.
     Defaults to the current user's UID and GID on Unix and (999, 0) on Windows.
 
     Args:
         uid: Input UID.
         gid: Input GID.
@@ -202,15 +206,15 @@
             if os.name == "posix"
             else _default_gid
         )
 
     return uid, gid
 
 
-def add_jupyter_args(run_args: List[str]) -> List[str]:
+def add_jupyter_args(run_args: list[str]) -> list[str]:
     """
     Adds `--ip 0.0.0.0` and `--no-browser` options to run args if those are not
     there yet.
 
     Args:
         run_args: Existing list of run arguments.
```

### Comparing `kedro-docker-0.5.0/kedro_docker/plugin.py` & `kedro_docker-0.6.0/kedro_docker/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ Kedro plugin for packaging a project with Docker """
+
 import shlex
 import subprocess
 from pathlib import Path
 from sys import version_info
-from typing import Dict, Tuple, Union
+from typing import Dict, Sequence
 
 import click
 from kedro import __version__ as kedro_version
 from kedro.framework.cli.utils import KedroCliError, call, forward_command
 from semver import VersionInfo
 
 from .helpers import (
@@ -186,15 +187,15 @@
         optional_args=[("-t", image)],
         user_args=docker_args,
     )
     command = ["docker", "build"] + combined_args + [str(project_path)]
     call(command)
 
 
-def _mount_info() -> Dict[str, Union[str, Tuple]]:
+def _mount_info() -> Dict[str, Sequence[str]]:
     res = {
         "host_root": str(Path.cwd()),
         "container_root": "/home/kedro_docker",
         "mount_volumes": DOCKER_DEFAULT_VOLUMES,
     }
     return res
```

### Comparing `kedro-docker-0.5.0/kedro_docker/template/.dive-ci` & `kedro_docker-0.6.0/kedro_docker/template/.dive-ci`

 * *Files identical despite different names*

### Comparing `kedro-docker-0.5.0/kedro_docker/template/Dockerfile.spark` & `kedro_docker-0.6.0/kedro_docker/template/Dockerfile.spark`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 # install JVM
 RUN apt-get update && mkdir -p /usr/share/man/man1 && \
 apt-get install -y procps default-jre-headless && rm -rf /var/lib/apt/lists/*
 
 # install project requirements
 COPY requirements.txt /tmp/requirements.txt
-RUN pip install --no-cache -r /tmp/requirements.txt && rm -f /tmp/requirements.txt
+RUN python -m pip install -U "pip>=21.2,<23.2"
+RUN pip install --no-cache-dir -r /tmp/requirements.txt && rm -f /tmp/requirements.txt
 
 # add kedro user
 ARG KEDRO_UID=999
 ARG KEDRO_GID=0
 RUN groupadd -f -g ${KEDRO_GID} kedro_group && \
 useradd -m -d /home/kedro_docker -s /bin/bash -g ${KEDRO_GID} -u ${KEDRO_UID} kedro_docker
```

### Comparing `kedro-docker-0.5.0/kedro_docker.egg-info/PKG-INFO` & `kedro_docker-0.6.0/kedro_docker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-docker
-Version: 0.5.0
+Version: 0.6.0
 Summary: Kedro-Docker makes it easy to package Kedro projects with Docker.
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Source, https://github.com/kedro-org/kedro-plugins/tree/main/kedro-docker
 Project-URL: Documentation, https://github.com/kedro-org/kedro-plugins/blob/main/kedro-docker/README.md
 Project-URL: Tracker, https://github.com/kedro-org/kedro-plugins/issues
 Requires-Python: >=3.8
@@ -13,14 +13,15 @@
 Requires-Dist: kedro>=0.16.0
 Requires-Dist: semver~=2.10
 Provides-Extra: test
 Requires-Dist: bandit; extra == "test"
 Requires-Dist: behave; extra == "test"
 Requires-Dist: black~=22.0; extra == "test"
 Requires-Dist: docker; extra == "test"
+Requires-Dist: mypy~=1.0; extra == "test"
 Requires-Dist: pre-commit>=2.9.2; extra == "test"
 Requires-Dist: psutil; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: pytest-xdist[psutil]~=2.2.1; extra == "test"
 Requires-Dist: PyYAML<7.0,>=5.1; extra == "test"
```

### Comparing `kedro-docker-0.5.0/kedro_docker.egg-info/SOURCES.txt` & `kedro_docker-0.6.0/kedro_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kedro-docker-0.5.0/pyproject.toml` & `kedro_docker-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 [project.optional-dependencies]
 test = [
     "bandit",
     "behave",
     "black~=22.0",
     "docker",
+    "mypy~=1.0",
     "pre-commit>=2.9.2",
     "psutil",
     "pytest",
     "pytest-cov",
     "pytest-mock",
     "pytest-xdist[psutil]~=2.2.1",
     "PyYAML>=5.1, <7.0",
```

### Comparing `kedro-docker-0.5.0/tests/test_helpers.py` & `kedro_docker-0.6.0/tests/test_helpers.py`

 * *Files identical despite different names*

