# Comparing `tmp/image-tools-stackabletech-0.0.5.tar.gz` & `tmp/image_tools_stackabletech-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image-tools-stackabletech-0.0.5.tar", last modified: Thu Oct 19 15:48:38 2023, max compression
+gzip compressed data, was "image_tools_stackabletech-0.0.6.tar", last modified: Wed Apr 24 15:45:04 2024, max compression
```

## Comparing `image-tools-stackabletech-0.0.5.tar` & `image_tools_stackabletech-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 razvan    (1000) razvan    (1000)        0 2023-10-19 15:48:38.303884 image-tools-stackabletech-0.0.5/
--rw-rw-r--   0 razvan    (1000) razvan    (1000)     1069 2023-08-22 16:10:26.000000 image-tools-stackabletech-0.0.5/LICENSE
--rw-r--r--   0 razvan    (1000) razvan    (1000)     1998 2023-10-19 15:48:38.303884 image-tools-stackabletech-0.0.5/PKG-INFO
--rw-rw-r--   0 razvan    (1000) razvan    (1000)     1272 2023-10-19 15:36:41.000000 image-tools-stackabletech-0.0.5/README.md
--rw-rw-r--   0 razvan    (1000) razvan    (1000)      898 2023-10-19 15:38:13.000000 image-tools-stackabletech-0.0.5/pyproject.toml
--rw-rw-r--   0 razvan    (1000) razvan    (1000)       38 2023-10-19 15:48:38.303884 image-tools-stackabletech-0.0.5/setup.cfg
-drwxrwxr-x   0 razvan    (1000) razvan    (1000)        0 2023-10-19 15:48:38.303884 image-tools-stackabletech-0.0.5/src/
-drwxrwxr-x   0 razvan    (1000) razvan    (1000)        0 2023-10-19 15:48:38.303884 image-tools-stackabletech-0.0.5/src/image_tools/
--rw-rw-r--   0 razvan    (1000) razvan    (1000)       34 2023-08-22 16:09:39.000000 image-tools-stackabletech-0.0.5/src/image_tools/__init__.py
--rw-rw-r--   0 razvan    (1000) razvan    (1000)     6278 2023-10-19 15:35:20.000000 image-tools-stackabletech-0.0.5/src/image_tools/args.py
--rw-rw-r--   0 razvan    (1000) razvan    (1000)     5996 2023-10-19 15:12:32.000000 image-tools-stackabletech-0.0.5/src/image_tools/bake.py
--rw-rw-r--   0 razvan    (1000) razvan    (1000)      711 2023-08-22 16:09:39.000000 image-tools-stackabletech-0.0.5/src/image_tools/lib.py
--rw-rw-r--   0 razvan    (1000) razvan    (1000)     4132 2023-08-23 14:52:21.000000 image-tools-stackabletech-0.0.5/src/image_tools/preflight.py
-drwxrwxr-x   0 razvan    (1000) razvan    (1000)        0 2023-10-19 15:48:38.303884 image-tools-stackabletech-0.0.5/src/image_tools/test/
--rw-rw-r--   0 razvan    (1000) razvan    (1000)    14577 2023-08-22 16:22:46.000000 image-tools-stackabletech-0.0.5/src/image_tools/test/conf.py
-drwxrwxr-x   0 razvan    (1000) razvan    (1000)        0 2023-10-19 15:48:38.303884 image-tools-stackabletech-0.0.5/src/image_tools_stackabletech.egg-info/
--rw-r--r--   0 razvan    (1000) razvan    (1000)     1998 2023-10-19 15:48:38.000000 image-tools-stackabletech-0.0.5/src/image_tools_stackabletech.egg-info/PKG-INFO
--rw-rw-r--   0 razvan    (1000) razvan    (1000)      509 2023-10-19 15:48:38.000000 image-tools-stackabletech-0.0.5/src/image_tools_stackabletech.egg-info/SOURCES.txt
--rw-rw-r--   0 razvan    (1000) razvan    (1000)        1 2023-10-19 15:48:38.000000 image-tools-stackabletech-0.0.5/src/image_tools_stackabletech.egg-info/dependency_links.txt
--rw-rw-r--   0 razvan    (1000) razvan    (1000)       92 2023-10-19 15:48:38.000000 image-tools-stackabletech-0.0.5/src/image_tools_stackabletech.egg-info/entry_points.txt
--rw-rw-r--   0 razvan    (1000) razvan    (1000)       60 2023-10-19 15:48:38.000000 image-tools-stackabletech-0.0.5/src/image_tools_stackabletech.egg-info/requires.txt
--rw-rw-r--   0 razvan    (1000) razvan    (1000)       12 2023-10-19 15:48:38.000000 image-tools-stackabletech-0.0.5/src/image_tools_stackabletech.egg-info/top_level.txt
+drwxrwxr-x   0 razvan    (1000) razvan    (1000)        0 2024-04-24 15:45:04.290118 image_tools_stackabletech-0.0.6/
+-rw-rw-r--   0 razvan    (1000) razvan    (1000)     1069 2023-12-01 16:23:46.000000 image_tools_stackabletech-0.0.6/LICENSE
+-rw-r--r--   0 razvan    (1000) razvan    (1000)     2171 2024-04-24 15:45:04.290118 image_tools_stackabletech-0.0.6/PKG-INFO
+-rw-rw-r--   0 razvan    (1000) razvan    (1000)     1445 2024-04-24 15:35:44.000000 image_tools_stackabletech-0.0.6/README.md
+-rw-rw-r--   0 razvan    (1000) razvan    (1000)      898 2024-04-24 15:35:44.000000 image_tools_stackabletech-0.0.6/pyproject.toml
+-rw-rw-r--   0 razvan    (1000) razvan    (1000)       38 2024-04-24 15:45:04.290118 image_tools_stackabletech-0.0.6/setup.cfg
+drwxrwxr-x   0 razvan    (1000) razvan    (1000)        0 2024-04-24 15:45:04.282118 image_tools_stackabletech-0.0.6/src/
+drwxrwxr-x   0 razvan    (1000) razvan    (1000)        0 2024-04-24 15:45:04.286118 image_tools_stackabletech-0.0.6/src/image_tools/
+-rw-rw-r--   0 razvan    (1000) razvan    (1000)       34 2023-12-01 16:23:46.000000 image_tools_stackabletech-0.0.6/src/image_tools/__init__.py
+-rw-rw-r--   0 razvan    (1000) razvan    (1000)     6230 2024-04-24 15:35:44.000000 image_tools_stackabletech-0.0.6/src/image_tools/args.py
+-rw-rw-r--   0 razvan    (1000) razvan    (1000)     5996 2023-12-01 16:23:46.000000 image_tools_stackabletech-0.0.6/src/image_tools/bake.py
+-rw-rw-r--   0 razvan    (1000) razvan    (1000)      711 2023-12-01 16:23:46.000000 image_tools_stackabletech-0.0.6/src/image_tools/lib.py
+-rw-rw-r--   0 razvan    (1000) razvan    (1000)     4524 2024-04-24 15:35:44.000000 image_tools_stackabletech-0.0.6/src/image_tools/preflight.py
+drwxrwxr-x   0 razvan    (1000) razvan    (1000)        0 2024-04-24 15:45:04.286118 image_tools_stackabletech-0.0.6/src/image_tools/test/
+-rw-rw-r--   0 razvan    (1000) razvan    (1000)    14577 2023-12-01 16:23:46.000000 image_tools_stackabletech-0.0.6/src/image_tools/test/conf.py
+drwxrwxr-x   0 razvan    (1000) razvan    (1000)        0 2024-04-24 15:45:04.290118 image_tools_stackabletech-0.0.6/src/image_tools_stackabletech.egg-info/
+-rw-r--r--   0 razvan    (1000) razvan    (1000)     2171 2024-04-24 15:45:04.000000 image_tools_stackabletech-0.0.6/src/image_tools_stackabletech.egg-info/PKG-INFO
+-rw-rw-r--   0 razvan    (1000) razvan    (1000)      509 2024-04-24 15:45:04.000000 image_tools_stackabletech-0.0.6/src/image_tools_stackabletech.egg-info/SOURCES.txt
+-rw-rw-r--   0 razvan    (1000) razvan    (1000)        1 2024-04-24 15:45:04.000000 image_tools_stackabletech-0.0.6/src/image_tools_stackabletech.egg-info/dependency_links.txt
+-rw-rw-r--   0 razvan    (1000) razvan    (1000)       92 2024-04-24 15:45:04.000000 image_tools_stackabletech-0.0.6/src/image_tools_stackabletech.egg-info/entry_points.txt
+-rw-rw-r--   0 razvan    (1000) razvan    (1000)       60 2024-04-24 15:45:04.000000 image_tools_stackabletech-0.0.6/src/image_tools_stackabletech.egg-info/requires.txt
+-rw-rw-r--   0 razvan    (1000) razvan    (1000)       12 2024-04-24 15:45:04.000000 image_tools_stackabletech-0.0.6/src/image_tools_stackabletech.egg-info/top_level.txt
```

### Comparing `image-tools-stackabletech-0.0.5/LICENSE` & `image_tools_stackabletech-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `image-tools-stackabletech-0.0.5/PKG-INFO` & `image_tools_stackabletech-0.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-tools-stackabletech
-Version: 0.0.5
+Version: 0.0.6
 Summary: Image tools for the Stackable Data Platform.
 Author-email: Razvan Mihai <razvan.mihai@stackable.tech>
 Project-URL: Homepage, https://github.com/stackabletech/image-tools
 Project-URL: Bug Tracker, https://github.com/stackabletech/image-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,61 +13,68 @@
 License-File: LICENSE
 Requires-Dist: Jinja2>=3.1.2
 Requires-Dist: PyYAML>=6.0
 Provides-Extra: lint
 Requires-Dist: ruff==0.0.275; extra == "lint"
 Requires-Dist: mypy==1.4.0; extra == "lint"
 
-# image-tools
+# image-tools v0.0.6
 
-Version: 0.0.5
+Commandline tools to manage Stackable container images available at https://github.com/stackabletech/docker-images
 
-## Installation
+This repository (and the installable package) contain two tools:
 
-We recommend to use [pipx](https://pypa.github.io/pipx/):
+* `bake` : build and publish product images.
+* `check-container` : run RedHat preflight checks on container images.
 
-    pipx install image-tools-stackabletech
+## Usage examples
 
-But you can also use `pip`:
+Run either `bake` or `check-container` with `--help` to get an overview of the accepted flags and their functionality.
+Below are some common usage examples:
 
-    # from PyPI
-    pip install image-tools-stackabletech
-    # from GitHub
-    pip install git+https://github.com/stackabletech/image-tools.git@main
+```shell
+# Build images of the hello-world containers
+bake -p hello-world -i 0.0.0-dev
 
-## Description
+# Build only one version [0.37.2] of OPA
+bake -p opa=0.37.2 -i 0.0.0-dev
 
-Tools to manage Stackable container images available at https://github.com/stackabletech/docker-images
+# Build half of all versions defined for OPA
+bake -p opa -i 0.0.0-dev  --shard-count 2 --shard-index 0
 
-Following tools are installed:
+# Build the other half of all versions defined for OPA
+bake -p opa -i 0.0.0-dev  --shard-count 2 --shard-index 1
+```
 
-* `bake` : build and publish product images.
-* `check-container` : run RedHat preflight checks on container images.
-
-## Examples
+## Installation
 
-    # Build images of the hello-world containers
-    bake -p hello-world -i 0.0.0-dev
+We recommend to use [pipx](https://pypa.github.io/pipx/):
 
-    # Build only one version [0.37.2] of OPA
-    bake -p opa=0.37.2 -i 0.0.0-dev
+```shell
+pipx install image-tools-stackabletech
+```
 
-    # Build half of all versions defined for OPA
-    bake -p opa -i 0.0.0-dev  --shard-count 2 --shard-index 0
+But you can also use `pip`:
 
-    # Build the other half of all versions defined for OPA
-    bake -p opa -i 0.0.0-dev  --shard-count 2 --shard-index 1
+```shell
+# from PyPI
+pip install image-tools-stackabletech
+# from GitHub
+pip install git+https://github.com/stackabletech/image-tools.git@main
+```
 
 ## Release a new version
 
 Update the version in:
 
 * `pyproject.toml`
 * `README.md` : version and pip install command.
 
 Update the CHANGELOG.
 Commit and tag.
 Build and publish:
 
-    rm -rf dist/
-    python -m build --sdist --wheel .
-    twine upload dist/*
+```shell
+rm -rf dist/
+python -m build --sdist --wheel .
+twine upload dist/*
+```
```

### Comparing `image-tools-stackabletech-0.0.5/README.md` & `image_tools_stackabletech-0.0.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,61 @@
-# image-tools
+# image-tools v0.0.6
 
-Version: 0.0.5
+Commandline tools to manage Stackable container images available at https://github.com/stackabletech/docker-images
 
-## Installation
+This repository (and the installable package) contain two tools:
 
-We recommend to use [pipx](https://pypa.github.io/pipx/):
+* `bake` : build and publish product images.
+* `check-container` : run RedHat preflight checks on container images.
 
-    pipx install image-tools-stackabletech
+## Usage examples
 
-But you can also use `pip`:
+Run either `bake` or `check-container` with `--help` to get an overview of the accepted flags and their functionality.
+Below are some common usage examples:
 
-    # from PyPI
-    pip install image-tools-stackabletech
-    # from GitHub
-    pip install git+https://github.com/stackabletech/image-tools.git@main
+```shell
+# Build images of the hello-world containers
+bake -p hello-world -i 0.0.0-dev
 
-## Description
+# Build only one version [0.37.2] of OPA
+bake -p opa=0.37.2 -i 0.0.0-dev
 
-Tools to manage Stackable container images available at https://github.com/stackabletech/docker-images
+# Build half of all versions defined for OPA
+bake -p opa -i 0.0.0-dev  --shard-count 2 --shard-index 0
 
-Following tools are installed:
+# Build the other half of all versions defined for OPA
+bake -p opa -i 0.0.0-dev  --shard-count 2 --shard-index 1
+```
 
-* `bake` : build and publish product images.
-* `check-container` : run RedHat preflight checks on container images.
-
-## Examples
+## Installation
 
-    # Build images of the hello-world containers
-    bake -p hello-world -i 0.0.0-dev
+We recommend to use [pipx](https://pypa.github.io/pipx/):
 
-    # Build only one version [0.37.2] of OPA
-    bake -p opa=0.37.2 -i 0.0.0-dev
+```shell
+pipx install image-tools-stackabletech
+```
 
-    # Build half of all versions defined for OPA
-    bake -p opa -i 0.0.0-dev  --shard-count 2 --shard-index 0
+But you can also use `pip`:
 
-    # Build the other half of all versions defined for OPA
-    bake -p opa -i 0.0.0-dev  --shard-count 2 --shard-index 1
+```shell
+# from PyPI
+pip install image-tools-stackabletech
+# from GitHub
+pip install git+https://github.com/stackabletech/image-tools.git@main
+```
 
 ## Release a new version
 
 Update the version in:
 
 * `pyproject.toml`
 * `README.md` : version and pip install command.
 
 Update the CHANGELOG.
 Commit and tag.
 Build and publish:
 
-    rm -rf dist/
-    python -m build --sdist --wheel .
-    twine upload dist/*
+```shell
+rm -rf dist/
+python -m build --sdist --wheel .
+twine upload dist/*
+```
```

### Comparing `image-tools-stackabletech-0.0.5/pyproject.toml` & `image_tools_stackabletech-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "image-tools-stackabletech"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name = "Razvan Mihai", email = "razvan.mihai@stackable.tech" }
 ]
 description = "Image tools for the Stackable Data Platform."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `image-tools-stackabletech-0.0.5/src/image_tools/args.py` & `image_tools_stackabletech-0.0.6/src/image_tools/args.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # This is the stackable release version
 from argparse import Namespace, ArgumentParser
-from typing import List
 import re
 import importlib.util
 import sys
 
 DEFAULT_IMAGE_VERSION_FORMATS = [
     re.compile(r"[2-9][0-9]\.[1-9][0-2]?\.\d+(-.+)?"),
     re.compile(r"0\.0\.0-dev(-.+)?"),
@@ -39,15 +38,15 @@
                         action="store_true")
     parser.add_argument("-d", "--dry", help="Dry run.", action="store_true")
     parser.add_argument(
         "-a",
         "--architecture",
         help="Target platform for image. Default: linux/amd64.",
         nargs="+",
-        default=["linux/amd64"],
+        default="linux/amd64",
         type=check_architecture_input,
     )
     parser.add_argument(
         "-o",
         "--organization",
         help="Organization name within the given registry. Default: stackable",
         default="stackable",
@@ -128,16 +127,15 @@
     parser.add_argument(
         "-s", "--submit", help="Submit results", action="store_true")
     parser.add_argument("-d", "--dry", help="Dry run.", action="store_true")
     parser.add_argument(
         "-a",
         "--architecture",
         help="Target platform for image. Default: linux/amd64.",
-        nargs="+",
-        default=["linux/amd64"],
+        default="linux/amd64",
         type=check_architecture_input,
     )
     parser.add_argument(
         "-t",
         "--token",
         help="RedHat portal API token",
     )
@@ -170,15 +168,15 @@
 
     if result.submit and not result.token:
         raise ValueError("Missing API token for submitting results.")
 
     return result
 
 
-def check_architecture_input(architecture) -> List[str]:
+def check_architecture_input(architecture: str) -> str:
     supported_arch = ["linux/amd64", "linux/arm64"]
 
     if architecture not in supported_arch:
         raise ValueError(
             f"Architecture {architecture} not supported. Supported: {supported_arch}"
         )
```

### Comparing `image-tools-stackabletech-0.0.5/src/image_tools/bake.py` & `image_tools_stackabletech-0.0.6/src/image_tools/bake.py`

 * *Files identical despite different names*

### Comparing `image-tools-stackabletech-0.0.5/src/image_tools/lib.py` & `image_tools_stackabletech-0.0.6/src/image_tools/lib.py`

 * *Files identical despite different names*

### Comparing `image-tools-stackabletech-0.0.5/src/image_tools/preflight.py` & `image_tools_stackabletech-0.0.6/src/image_tools/preflight.py`

 * *Files 13% similar despite different names*

```diff
@@ -67,14 +67,22 @@
                     "--submit",
                     "--pyxis-api-token",
                     args.token,
                     "--certification-project-id",
                     f"ospid-{conf.open_shift_projects[args.product]['id']}",
                  ]
             )
+        if args.architecture:
+            cmd_args.extend(
+                ["--platform",
+                    # this argument value has already been checked against valid values with an expected prefix.
+                    # Preflight provides the same "linux/" prefix and so it must be removed here.
+                    args.architecture.split("linux/")[1],
+                 ]
+            )
         result[img] = Command(args=cmd_args)
     return result
 
 
 def main() -> int:
     """Run OpenShift verification checks against the product images."""
     logging.basicConfig(
```

### Comparing `image-tools-stackabletech-0.0.5/src/image_tools/test/conf.py` & `image_tools_stackabletech-0.0.6/src/image_tools/test/conf.py`

 * *Files identical despite different names*

### Comparing `image-tools-stackabletech-0.0.5/src/image_tools_stackabletech.egg-info/PKG-INFO` & `image_tools_stackabletech-0.0.6/src/image_tools_stackabletech.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-tools-stackabletech
-Version: 0.0.5
+Version: 0.0.6
 Summary: Image tools for the Stackable Data Platform.
 Author-email: Razvan Mihai <razvan.mihai@stackable.tech>
 Project-URL: Homepage, https://github.com/stackabletech/image-tools
 Project-URL: Bug Tracker, https://github.com/stackabletech/image-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,61 +13,68 @@
 License-File: LICENSE
 Requires-Dist: Jinja2>=3.1.2
 Requires-Dist: PyYAML>=6.0
 Provides-Extra: lint
 Requires-Dist: ruff==0.0.275; extra == "lint"
 Requires-Dist: mypy==1.4.0; extra == "lint"
 
-# image-tools
+# image-tools v0.0.6
 
-Version: 0.0.5
+Commandline tools to manage Stackable container images available at https://github.com/stackabletech/docker-images
 
-## Installation
+This repository (and the installable package) contain two tools:
 
-We recommend to use [pipx](https://pypa.github.io/pipx/):
+* `bake` : build and publish product images.
+* `check-container` : run RedHat preflight checks on container images.
 
-    pipx install image-tools-stackabletech
+## Usage examples
 
-But you can also use `pip`:
+Run either `bake` or `check-container` with `--help` to get an overview of the accepted flags and their functionality.
+Below are some common usage examples:
 
-    # from PyPI
-    pip install image-tools-stackabletech
-    # from GitHub
-    pip install git+https://github.com/stackabletech/image-tools.git@main
+```shell
+# Build images of the hello-world containers
+bake -p hello-world -i 0.0.0-dev
 
-## Description
+# Build only one version [0.37.2] of OPA
+bake -p opa=0.37.2 -i 0.0.0-dev
 
-Tools to manage Stackable container images available at https://github.com/stackabletech/docker-images
+# Build half of all versions defined for OPA
+bake -p opa -i 0.0.0-dev  --shard-count 2 --shard-index 0
 
-Following tools are installed:
+# Build the other half of all versions defined for OPA
+bake -p opa -i 0.0.0-dev  --shard-count 2 --shard-index 1
+```
 
-* `bake` : build and publish product images.
-* `check-container` : run RedHat preflight checks on container images.
-
-## Examples
+## Installation
 
-    # Build images of the hello-world containers
-    bake -p hello-world -i 0.0.0-dev
+We recommend to use [pipx](https://pypa.github.io/pipx/):
 
-    # Build only one version [0.37.2] of OPA
-    bake -p opa=0.37.2 -i 0.0.0-dev
+```shell
+pipx install image-tools-stackabletech
+```
 
-    # Build half of all versions defined for OPA
-    bake -p opa -i 0.0.0-dev  --shard-count 2 --shard-index 0
+But you can also use `pip`:
 
-    # Build the other half of all versions defined for OPA
-    bake -p opa -i 0.0.0-dev  --shard-count 2 --shard-index 1
+```shell
+# from PyPI
+pip install image-tools-stackabletech
+# from GitHub
+pip install git+https://github.com/stackabletech/image-tools.git@main
+```
 
 ## Release a new version
 
 Update the version in:
 
 * `pyproject.toml`
 * `README.md` : version and pip install command.
 
 Update the CHANGELOG.
 Commit and tag.
 Build and publish:
 
-    rm -rf dist/
-    python -m build --sdist --wheel .
-    twine upload dist/*
+```shell
+rm -rf dist/
+python -m build --sdist --wheel .
+twine upload dist/*
+```
```

