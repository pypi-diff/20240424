# Comparing `tmp/poetry_plugin_lambda_build-0.2.4.tar.gz` & `tmp/poetry_plugin_lambda_build-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_lambda_build-0.2.4.tar", max compression
+gzip compressed data, was "poetry_plugin_lambda_build-0.3.0.tar", max compression
```

## Comparing `poetry_plugin_lambda_build-0.2.4.tar` & `poetry_plugin_lambda_build-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2024-04-10 17:25:24.448785 poetry_plugin_lambda_build-0.2.4/LICENSE
--rw-r--r--   0        0        0     5785 2024-04-10 17:25:24.448785 poetry_plugin_lambda_build-0.2.4/README.md
--rw-r--r--   0        0        0        0 2024-04-10 17:25:24.448785 poetry_plugin_lambda_build-0.2.4/poetry_plugin_lambda_build/__init__.py
--rw-r--r--   0        0        0     2176 2024-04-10 17:25:24.448785 poetry_plugin_lambda_build-0.2.4/poetry_plugin_lambda_build/docker.py
--rw-r--r--   0        0        0     7287 2024-04-10 17:25:24.448785 poetry_plugin_lambda_build-0.2.4/poetry_plugin_lambda_build/plugin.py
--rw-r--r--   0        0        0     6374 2024-04-10 17:25:24.448785 poetry_plugin_lambda_build-0.2.4/poetry_plugin_lambda_build/recipes.py
--rw-r--r--   0        0        0      543 2024-04-10 17:25:24.448785 poetry_plugin_lambda_build-0.2.4/poetry_plugin_lambda_build/utils.py
--rw-r--r--   0        0        0      652 2024-04-10 17:25:24.448785 poetry_plugin_lambda_build-0.2.4/poetry_plugin_lambda_build/zip.py
--rw-r--r--   0        0        0      706 2024-04-10 17:25:24.448785 poetry_plugin_lambda_build-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     6446 1970-01-01 00:00:00.000000 poetry_plugin_lambda_build-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-24 17:32:04.499768 poetry_plugin_lambda_build-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5785 2024-04-24 17:32:04.499768 poetry_plugin_lambda_build-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-24 17:32:04.499768 poetry_plugin_lambda_build-0.3.0/poetry_plugin_lambda_build/__init__.py
+-rw-r--r--   0        0        0     2134 2024-04-24 17:32:04.499768 poetry_plugin_lambda_build-0.3.0/poetry_plugin_lambda_build/docker.py
+-rw-r--r--   0        0        0     7165 2024-04-24 17:32:04.499768 poetry_plugin_lambda_build-0.3.0/poetry_plugin_lambda_build/plugin.py
+-rw-r--r--   0        0        0     6724 2024-04-24 17:32:04.499768 poetry_plugin_lambda_build-0.3.0/poetry_plugin_lambda_build/recipes.py
+-rw-r--r--   0        0        0      257 2024-04-24 17:32:04.499768 poetry_plugin_lambda_build-0.3.0/poetry_plugin_lambda_build/utils.py
+-rw-r--r--   0        0        0      652 2024-04-24 17:32:04.499768 poetry_plugin_lambda_build-0.3.0/poetry_plugin_lambda_build/zip.py
+-rw-r--r--   0        0        0      707 2024-04-24 17:32:04.499768 poetry_plugin_lambda_build-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6496 1970-01-01 00:00:00.000000 poetry_plugin_lambda_build-0.3.0/PKG-INFO
```

### Comparing `poetry_plugin_lambda_build-0.2.4/LICENSE` & `poetry_plugin_lambda_build-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.2.4/README.md` & `poetry_plugin_lambda_build-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.2.4/poetry_plugin_lambda_build/docker.py` & `poetry_plugin_lambda_build-0.3.0/poetry_plugin_lambda_build/docker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import tarfile
 from contextlib import contextmanager
-from functools import cache
 
 import docker
 from poetry.console.commands.env_command import EnvCommand
 
 LIST_ARGS = (
     "environment",
     "dns",
@@ -19,15 +18,14 @@
 
 def _parse_string_to_boolean(value: str):
     if value.lower() in ("0", "false"):
         return False
     return True
 
 
-@cache
 def get_docker_client() -> docker.DockerClient:
     return docker.from_env()
 
 
 def copy_to(src: str, dst: str):
     name, dst = dst.split(":")
     container = get_docker_client().containers.get(name)
@@ -55,15 +53,15 @@
     f.close()
     tar = tarfile.open(tar_path)
     tar.extractall(dst)
     os.remove(tar_path)
 
 
 @contextmanager
-def run_container(env_cmd: EnvCommand, *args, **kwargs):
+def run_container(env_cmd: EnvCommand, **kwargs):
     image: str = kwargs.pop("image")
     options: dict = {k: True for k in kwargs.pop("options", [])}
     kwargs: dict = {k: v for k, v in kwargs.items() if v}
 
     for arg in LIST_ARGS:
         if arg in kwargs:
             kwargs[arg] = kwargs[arg].split(",")
```

### Comparing `poetry_plugin_lambda_build-0.2.4/poetry_plugin_lambda_build/plugin.py` & `poetry_plugin_lambda_build-0.3.0/poetry_plugin_lambda_build/plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import enum
-from collections import defaultdict
 from typing import Any
 
 from cleo.application import Application
 from cleo.helpers import argument
 from poetry.console.commands.env_command import EnvCommand
 from poetry.plugins.application_plugin import ApplicationPlugin
 
 from .recipes import (create_package, create_separate_layer_package,
                       create_separated_function_package)
-from .utils import get_path, merge_options
-
+from .utils import remove_prefix
 
 INSTALL_DEPS_CMD = (
     "mkdir -p {container_cache_dir} && "
     "pip install -q --upgrade pip && "
     "pip install -q -t {container_cache_dir} --no-cache-dir -r {requirements}"
 )
 
@@ -26,166 +24,144 @@
 INSTALL_PACKAGE_CMD = (
     "mkdir -p {package_dir} && "
     "pip install poetry --quiet --upgrade pip && "
     "poetry build --quiet && "
     "poetry run pip install --quiet -t {package_dir} --no-cache-dir dist/*.whl --upgrade"
 )
 
-DEFAULT_OPTIONS = {
-    "docker": {
-        "env": None,
-        "entrypoint": "/bin/sh",
-        "dns": None,
-        "network": "host",
-        "options": [],
-    },
-    "layer": {
-        "artifact_path": None,
-        "install_dir": None,
-    },
-    "function": {
-        "artifact_path": None,
-        "install_dir": None,
-    },
-    "artifacts": {"path": "artifacts"},
-    "without": None,
-    "only": None,
-    "with": None,
-    "install_dir": None,
+DEFAULT_PARAMETERS = {
+    "docker_entrypoint": "/bin/sh",
+    "docker_network": "host",
+    "docker_options": [],
     "artifact_path": "package.zip",
     "install_package_cmd": INSTALL_PACKAGE_CMD,
     "install_no_deps_cmd": INSTALL_NO_DEPS_CMD,
-    "install_deps_cmd": INSTALL_DEPS_CMD
+    "install_deps_cmd": INSTALL_DEPS_CMD,
+    "without": None,
+    "only": None,
+    "with": None,
+    "config": [],
 }
 
 
 class BuildType(enum.Enum):
     IN_CONTAINER_MERGED = enum.auto()
     IN_CONTAINER_SEPARATED = enum.auto()
     MERGED = enum.auto()
     SEPARATED = enum.auto()
 
     @classmethod
-    def get_type(cls, options: dict):
-        layer = get_path(options, "layer.artifact_path")
-        function = get_path(options, "function.artifact_path")
-        container_img = get_path(options, "docker.image")
+    def get_type(cls, parameters: dict):
+        layer = parameters.get("layer_artifact_path")
+        function = parameters.get("function_artifact_path")
+        container_img = parameters.get("docker_image")
         if container_img:
             if layer and function:
                 return cls.IN_CONTAINER_SEPARATED
             else:
                 return cls.IN_CONTAINER_MERGED
         else:
             if layer and function:
                 return cls.SEPARATED
             else:
                 return cls.MERGED
 
 
-ARGS = [
-    ("docker_image", "The image to run"),
-    ("docker_entrypoint", "The entrypoint for the container (comma separated string)"),
-    ("docker_environment", "Environment variables to set inside the container (comma separated string) ex. VAR_1=VALUE_1,VAR_2=VALUE_2"),
-    ("docker_dns", "Set custom DNS servers (comma separated string)"),
-    ("docker_network", "The name of the network this container will be connected to at creation time"),
-    ("docker_network_disabled", "Disable networking ex. docker_network_disabled=0"),
-    ("docker_network_mode", "Network_mode"),
-    ("docker_platform",
-     "Platform in the format os[/arch[/variant]]. Only used if the method needs to pull the requested image."),
-    ("package_install_dir",
-     "Installation directory inside zip artifact for single zip package"),
-    ("layer_install_dir",
-     "Installation directory inside zip artifact for layer zip package"),
-    ("function_install_dir",
-     "Installation directory inside zip artifact for function zip package"),
-    ("package_artifact_path", "Output package path"),
-    ("layer_artifact_path", "Output layer package path"),
-    ("function_artifact_path", "Output function package path"),
-    ("only", "The only dependency groups to include"),
-    ("without", "The dependency groups to ignore"),
-    ("with", "The optional dependency groups to include"),
-    ("install_deps_cmd",
-     f"Install dependencies command. Executed during installation of dependencies layer, by default: {INSTALL_DEPS_CMD}"),
-    ("install_no_deps_cmd",
-     f"Install without dependencies command. Executed during installation of function, by default: {INSTALL_NO_DEPS_CMD}"),
-    ("install_package_cmd",
-     f"Install package command. Executed during installation of package without function-layer separation, by default: {INSTALL_PACKAGE_CMD}")
-]
+ARGS = {
+    "docker_image": ("The image to run", True, False, None),
+    "docker_entrypoint": ("The entrypoint for the container (comma separated string)", True, False, None),
+    "docker_environment": ("Environment variables to set inside the container (comma separated string) ex. VAR_1=VALUE_1,VAR_2=VALUE_2", True, False, None),
+    "docker_dns": ("Set custom DNS servers (comma separated string)", True, False, None),
+    "docker_network": ("The name of the network this container will be connected to at creation time", True, False, None),
+    "docker_network_disabled": ("Disable networking ex. docker_network_disabled=0", True, False, None),
+    "docker_network_mode": ("Network_mode", True, False, None),
+    "docker_platform": ("Platform in the format os[/arch[/variant]]. Only used if the method needs to pull the requested image.", True, False, None),
+    "package_install_dir": ("Installation directory inside zip artifact for single zip package", True, False, None),
+    "layer_install_dir": ("Installation directory inside zip artifact for layer zip package", True, False, None),
+    "function_install_dir": ("Installation directory inside zip artifact for function zip package", True, False, None),
+    "install_dir": ("Installation directory inside zip artifact for zip package (not function layer separation)", True, False, None),
+    "package_artifact_path": ("Output package path", True, False, None),
+    "layer_artifact_path": ("Output layer package path", True, False, None),
+    "function_artifact_path": ("Output function package path", True, False, None),
+    "only": ("The only dependency groups to include", True, False, None),
+    "without": ("The dependency groups to ignore", True, False, None),
+    "with": ("The optional dependency groups to include", True, False, None),
+    "install_deps_cmd": (f"Install dependencies command. Executed during installation of dependencies layer, by default: {INSTALL_DEPS_CMD}", True, False, None),
+    "install_no_deps_cmd": (f"Install without dependencies command. Executed during installation of function, by default: {INSTALL_NO_DEPS_CMD}", True, False, None),
+    "install_package_cmd": (f"Install package command. Executed during installation of package without function-layer separation, by default: {INSTALL_PACKAGE_CMD}", True, False, None),
+    "config": ("Manages configuration settings.", True, True, None)
+}
+
+ARGS_SECTIONS = ("layer", "function", "docker", "artifacts")
+
+
+class ParametersContainer(dict):
+    args = ARGS
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.update(DEFAULT_PARAMETERS)
+
+    def put(self, key: Any, value: Any) -> None:
+        prev_value = self.get(key)
+        if isinstance(prev_value, list):
+            self[key].append(value)
+        else:
+            self[key] = value
+        return
+
+    def get_section(self, section: str) -> dict:
+        result = {}
+        for k in self:
+            if k.startswith(section):
+                key = remove_prefix(k, section+"_")
+                result[key] = self[k]
+        return result
 
 
 class BuildLambdaCommand(EnvCommand):
     name = "build-lambda"
     description = "Execute to build lambda lambda artifacts"
 
     arguments = [
-        argument(*arg, optional=True, multiple=False) for arg in ARGS
+        argument(name, *params) for name, params in ARGS.items()
     ]
 
-    def _get_options(self) -> Any:
-        options = defaultdict(dict)
-        options.update(DEFAULT_OPTIONS)
-        override_options = defaultdict(dict)
-        _missed_args = {}
-
+    def _get_parameters(self) -> ParametersContainer:
         pyproject_data = self.poetry.pyproject.data
-        # Gather override args
-        for arg in ARGS:
-            arg_name = arg[0]
-            _argument = self.argument(arg_name) or _missed_args.get(arg_name)
-            if _argument:
-                
-                if arg_name not in _argument:
-                    key = _argument.split("=", 1)[0]
-                    _missed_args[key] = _argument
-                    continue
-
-                try:
-                    key, value = _argument.split("=", 1)
-                    
-                    if "_" in key:
-                        prefix, name = key.split("_", 1)
-                        override_options[prefix][name] = value
-                    else:
-                        override_options[key] = value
-                    
-                except ValueError as e:
-                    raise Exception(
-                        f"Argument {arg_name} has wrong value: {_argument}", e
-                    ) from e
+        container = ParametersContainer()
+        for token in filter(lambda token: any([token.startswith(f"{arg}=") for arg in ARGS]), self.io.input._tokens[1:]):
+            key, value = token.strip().split("=")
+            container.put(key, value)
+
+        try:
+            plugin_conf = pyproject_data["tool"]["poetry-plugin-lambda-build"]
+        except KeyError:
+            plugin_conf = None
 
-        pyproject_data = self.poetry.pyproject.data
-        prefixes = ["layer", "function", "docker", "artifacts"]
-        plugin_conf = get_path(
-            pyproject_data, "tool.poetry-plugin-lambda-build"
-        )
         if plugin_conf:
             for k in plugin_conf:
-                for prefix in prefixes:
-                    if k.startswith(prefix):
-                        arg = k.removeprefix(prefix + "_")
-                        options[prefix][arg] = plugin_conf[k]
-
-        options = merge_options(options, override_options)
-        return options
+                container.put(k, plugin_conf[k])
+        return container
 
     def handle(self) -> Any:
-        options: dict = self._get_options()
-        _type: BuildType = BuildType.get_type(options)
+        parameters: ParametersContainer = self._get_parameters()
+        _type: BuildType = BuildType.get_type(parameters)
         if _type == BuildType.IN_CONTAINER_SEPARATED:
             self.line("Building separated packages in container...", style="info")
-            create_separated_function_package(self, options)
-            create_separate_layer_package(self, options)
+            create_separated_function_package(self, parameters)
+            create_separate_layer_package(self, parameters)
         elif _type == BuildType.SEPARATED:
             self.line("Building separated packages on local...", style="info")
-            create_separate_layer_package(self, options, in_container=False)
-            create_separated_function_package(self, options)
+            create_separate_layer_package(self, parameters, in_container=False)
+            create_separated_function_package(self, parameters)
         elif _type == BuildType.IN_CONTAINER_MERGED:
-            create_package(self, options, in_container=True)
+            create_package(self, parameters, in_container=True)
         else:
-            create_package(self, options, in_container=False)
+            create_package(self, parameters, in_container=False)
         self.line("\n✨ Done!")
 
 
 def factory() -> BuildLambdaCommand:
     return BuildLambdaCommand()
```

### Comparing `poetry_plugin_lambda_build-0.2.4/poetry_plugin_lambda_build/recipes.py` & `poetry_plugin_lambda_build-0.3.0/poetry_plugin_lambda_build/recipes.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import subprocess
 from tempfile import TemporaryDirectory
 from typing import ByteString
 
 from poetry.console.commands.env_command import EnvCommand
 
 from .docker import copy_from, copy_to, run_container
-from .utils import get_path
+from .utils import remove_suffix
 from .zip import create_zip_package
 
 
 class BuildLambdaPluginError(Exception):
     pass
 
 
@@ -30,141 +30,150 @@
     if process.returncode == 0:
         self.line_error(err.decode("utf-8"), style="warning")
         return output
     elif process.returncode == 1:
         self.line_error(err.decode("utf-8"), style="error")
 
     raise BuildLambdaPluginError(output.decode("utf-8"))
-    
+
 
 def create_separate_layer_package(
-    self: EnvCommand, options: dict, in_container: bool = True
+    self: EnvCommand, parameters: dict, in_container: bool = True
 ):
     with TemporaryDirectory() as tmp_dir:
-        install_dir = get_path(options, "layer.install_dir")
+        install_dir = parameters.get("layer_install_dir", "")
         layer_output_dir = os.path.join(tmp_dir, "layer_output")
 
         target = os.path.join(
-            CURRENT_WORK_DIR, get_path(options, "layer.artifact_path")
+            CURRENT_WORK_DIR, parameters.get("layer_artifact_path", "")
         )
         requirements_path = os.path.join(tmp_dir, "requirements.txt")
 
         poetry_export_cmd = "poetry export --format=requirements.txt"
 
-        if options["without"]:
-            poetry_export_cmd+=f" --without={options['without']}"
+        if parameters["without"]:
+            poetry_export_cmd += f" --without={parameters['without']}"
+
+        if parameters["with"]:
+            poetry_export_cmd += f" --with={parameters['with']}"
 
-        if options["with"]:
-            poetry_export_cmd+=f" --with={options['with']}"
-        
-        if options["only"]:
-            poetry_export_cmd+=f" --only={options['only']}"
+        if parameters["only"]:
+            poetry_export_cmd += f" --only={parameters['only']}"
 
         if install_dir:
             layer_output_dir = os.path.join(layer_output_dir, install_dir)
 
         self.line("Generating requirements file...", style="info")
         self.line(f"Executing: {poetry_export_cmd}", style="debug")
+
         output = _run_process(self, poetry_export_cmd)
 
         with open(requirements_path, "w") as f:
             f.write(output.decode("utf-8"))
 
         if in_container:
-            with run_container(self, **options["docker"]) as container:
+            with run_container(self, **parameters.get_section("docker")) as container:
                 copy_to(requirements_path, f"{container.id}:/requirements.txt")
                 self.line("Installing requirements", style="info")
-                install_deps_cmd = options["install_deps_cmd"].format(
+                install_deps_cmd = parameters["install_deps_cmd"].format(
                     container_cache_dir=CONTAINER_CACHE_DIR,
                     requirements="/requirements.txt",
                 )
                 result = container.exec_run(
                     f'sh -c "{install_deps_cmd}"', stream=True)
                 for line in result.output:
                     self.line(line.strip().decode("utf-8"), style="info")
                 self.line(f"Coping output to {layer_output_dir}", style="info")
                 os.makedirs(layer_output_dir, exist_ok=True)
                 copy_from(f"{container.id}:{CONTAINER_CACHE_DIR}/.",
                           layer_output_dir)
         else:
-            install_deps_cmd = options["install_deps_cmd"].format(
+            install_deps_cmd = parameters["install_deps_cmd"].format(
                 container_cache_dir=layer_output_dir, requirements=requirements_path
             )
 
             self.line("Installing requirements", style="info")
             self.line(f"Executing: {install_deps_cmd}", style="debug")
             _run_process(self, install_deps_cmd)
 
         self.line(f"Building {target}...", style="info")
         os.makedirs(os.path.dirname(target), exist_ok=True)
         create_zip_package(
-            layer_output_dir.removesuffix(install_dir)
+            remove_suffix(layer_output_dir, install_dir)
             if install_dir
             else layer_output_dir,
             target,
         )
         self.line(f"target successfully built: {target}...", style="info")
 
 
-def create_separated_function_package(self: EnvCommand, options: dict):
+def create_separated_function_package(self: EnvCommand, parameters: dict):
     with TemporaryDirectory() as tmp_dir:
-        install_dir = get_path(options, "function.install_dir")
+        install_dir = parameters.get("function_install_dir", "")
         package_dir = tmp_dir
         target = os.path.join(
-            CURRENT_WORK_DIR, get_path(options, "function.artifact_path")
+            CURRENT_WORK_DIR, parameters.get("function_artifact_path", "")
         )
 
-        if install_dir:
-            package_dir = os.path.join(package_dir, install_dir)
+        package_dir = os.path.join(package_dir, install_dir)
         self.line("Building function package...", style="info")
 
-        install_cmd = options["install_no_deps_cmd"].format(package_dir=package_dir)
+        install_cmd = parameters["install_no_deps_cmd"].format(
+            package_dir=package_dir)
 
         self.line(f"Executing: {install_cmd}", style="debug")
 
         _run_process(self, install_cmd)
 
         self.line(f"Building target: {target}", style="info")
         os.makedirs(os.path.dirname(target), exist_ok=True)
         create_zip_package(
-            package_dir.removesuffix(
-                install_dir) if install_dir else package_dir,
+            remove_suffix(package_dir, install_dir),
             target,
         )
         self.line(f"target successfully built: {target}...", style="info")
 
 
-def create_package(self: EnvCommand, options: dict, in_container: bool = True):
+def create_package(self: EnvCommand, parameters: dict, in_container: bool = True):
     current_working_directory = os.getcwd()
     with TemporaryDirectory() as package_dir:
-        install_dir = get_path(options, "install_dir")
+        install_dir = parameters.get("install_dir", "")
 
         if install_dir:
             package_dir = os.path.join(package_dir, install_dir)
 
         target = os.path.join(
-            current_working_directory, get_path(options, "artifact_path")
+            current_working_directory, parameters.get("artifact_path", "")
         )
         if in_container:
             self.line("Building package in container", style="info")
-            with run_container(self, **options["docker"]) as container:
-                cmd = options["install_package_cmd"].format(package_dir=package_dir)
+            with run_container(self, **parameters.get_section("docker")) as container:
+
+                for config in parameters["config"]:
+                    result = container.exec_run(
+                        f'poetry config {config}', stream=True)
+                    for line in result.output:
+                        self.line(line.strip().decode("utf-8"), style="info")
+
+                cmd = parameters["install_package_cmd"].format(
+                    package_dir=package_dir)
                 self.line(f"Executing: {cmd}", style="debug")
                 result = container.exec_run(f'sh -c "{cmd}"', stream=True)
 
                 for line in result.output:
                     self.line(line.strip().decode("utf-8"), style="info")
 
                 copy_from(f"{container.id}:{package_dir}/.", package_dir)
         else:
             self.line("Building package on local", style="info")
-            cmd = options["install_package_cmd"].format(package_dir=package_dir)
+            cmd = parameters["install_package_cmd"].format(
+                package_dir=package_dir)
             self.line(f"Executing: {cmd}", style="debug")
             _run_process(self, cmd)
 
         os.makedirs(os.path.dirname(target), exist_ok=True)
         create_zip_package(
-            package_dir.removesuffix(
-                install_dir) if install_dir else package_dir,
+            remove_suffix(
+                package_dir, install_dir) if install_dir else package_dir,
             target,
         )
         self.line(f"target successfully built: {target}...", style="info")
```

### Comparing `poetry_plugin_lambda_build-0.2.4/poetry_plugin_lambda_build/zip.py` & `poetry_plugin_lambda_build-0.3.0/poetry_plugin_lambda_build/zip.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.2.4/pyproject.toml` & `poetry_plugin_lambda_build-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "poetry-plugin-lambda-build"
-version = "0.2.4"
+version = "0.3.0"
 description = "The plugin for poetry that allows you to build zip packages suited for serverless deployment like AWS Lambda, Google App Engine, Azure App Service, and more..."
 authors = ["Michał Murawski <mmurawski777@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 docker = "^7.0.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.1"
 poetry = "^1.7.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."poetry.application.plugin"]
 build-lambda = "poetry_plugin_lambda_build.plugin:LambdaPlugin"
 
 [tool.pytest.ini_options]
-testpaths = ["tests"]
+testpaths = ["tests"]
```

### Comparing `poetry_plugin_lambda_build-0.2.4/PKG-INFO` & `poetry_plugin_lambda_build-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-lambda-build
-Version: 0.2.4
+Version: 0.3.0
 Summary: The plugin for poetry that allows you to build zip packages suited for serverless deployment like AWS Lambda, Google App Engine, Azure App Service, and more...
 Author: Michał Murawski
 Author-email: mmurawski777@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: docker (>=7.0.0,<8.0.0)
 Description-Content-Type: text/markdown
```

