# Comparing `tmp/git_alert-0.1.0.tar.gz` & `tmp/git_alert-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_alert-0.1.0.tar", max compression
+gzip compressed data, was "git_alert-0.2.0.tar", max compression
```

## Comparing `git_alert-0.1.0.tar` & `git_alert-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1077 2024-04-02 12:23:59.017457 git_alert-0.1.0/LICENSE
--rw-r--r--   0        0        0     2273 2024-04-19 16:31:29.316378 git_alert-0.1.0/README.md
--rw-r--r--   0        0        0      142 2024-04-07 21:11:53.329784 git_alert-0.1.0/git_alert/__init__.py
--rw-r--r--   0        0        0      327 2024-04-19 13:38:45.886073 git_alert-0.1.0/git_alert/__main__.py
--rw-r--r--   0        0        0      628 2024-04-19 13:38:45.886073 git_alert-0.1.0/git_alert/argument_parser.py
--rw-r--r--   0        0        0      703 2024-04-07 21:12:57.897411 git_alert-0.1.0/git_alert/repositories.py
--rw-r--r--   0        0        0      359 2024-04-19 13:38:45.886073 git_alert-0.1.0/git_alert/scripts/git_alert.py
--rw-r--r--   0        0        0     1383 2024-04-19 13:38:45.886073 git_alert-0.1.0/git_alert/traverse.py
--rw-r--r--   0        0        0      764 2024-04-19 15:29:43.672142 git_alert-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2757 1970-01-01 00:00:00.000000 git_alert-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-24 20:33:52.776556 git_alert-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3416 2024-04-24 20:33:52.776556 git_alert-0.2.0/README.md
+-rw-r--r--   0        0        0      142 2024-04-24 20:33:52.780556 git_alert-0.2.0/git_alert/__init__.py
+-rw-r--r--   0        0        0      393 2024-04-24 20:33:52.780556 git_alert-0.2.0/git_alert/__main__.py
+-rw-r--r--   0        0        0     1128 2024-04-24 20:33:52.780556 git_alert-0.2.0/git_alert/argument_parser.py
+-rw-r--r--   0        0        0     1285 2024-04-24 20:33:52.780556 git_alert-0.2.0/git_alert/repositories.py
+-rw-r--r--   0        0        0      433 2024-04-24 20:33:52.780556 git_alert-0.2.0/git_alert/scripts/git_alert.py
+-rw-r--r--   0        0        0     1552 2024-04-24 20:33:52.780556 git_alert-0.2.0/git_alert/traverse.py
+-rw-r--r--   0        0        0      657 2024-04-24 20:33:52.780556 git_alert-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3900 1970-01-01 00:00:00.000000 git_alert-0.2.0/PKG-INFO
```

### Comparing `git_alert-0.1.0/LICENSE` & `git_alert-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `git_alert-0.1.0/README.md` & `git_alert-0.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 ![Codecov](https://img.shields.io/codecov/c/github/nomisreual/git_alert)
 
 This is a Python application that checks in the given directory and all its subdirectories
 for any dirty repositories.
 
+The source code is available on [GitHub](https://github.com/nomisreual/git_alert).
+
 This application aims to ease the frequent use of git as it makes it easy to check for any untracked changes in any of your repositories.
 
 ## Installation:
 
-The application is now available on PyPI, so you can install it using pip:
+The application is now available on **PyPI**, so you can install it using _pip_:
 
 ```
 pip install git_alert
 ```
 
-Alternatively, you can use pipx to make it globally available:
+Alternatively, you can use _pipx_ to make it globally available:
 
 ```
 pipx install git_alert
 ```
 
 Of course you can also clone the repository and install it manually. The package is built using poetry, so the easiest way to build it locally would be
 to use poetry:
@@ -41,25 +43,78 @@
 
 or
 
 ```
 pipx install .
 ```
 
+If you are using flakes to manage your NixOS installation, you can add the provided flake to your
+inputs:
+
+```nix
+{
+  description = "Configuration";
+
+  inputs = {
+    ...
+    git_alert = {
+      url = "github:nomisreual/git_alert";
+      inputs.nixpkgs.follows = "nixpkgs";
+    };
+    ...
+  };
+  outputs = {
+    self,
+    nixpkgs,
+    ...
+  } @ inputs: {
+    # your configuration
+  };
+}
+```
+
+You can then add `git_alert` to your packages (don't forget to add `inputs` to the respective module):
+
+```nix
+# configuration.nix
+{
+  environment.systemPackages = with pkgs; [
+    ...
+
+    inputs.git_alert.packages."x86_64-linux".default
+    ...
+  ];
+}
+# home.nix
+{
+  home.packages = with pkgs; [
+    ...
+
+    inputs.git_alert.packages."x86_64-linux".default
+    ...
+  ];
+}
+```
+
+After rebuilding, you have git_alert at your fingertips and it gets updated whenever you update your flake.
+
 ## Usage:
 
 You can use _git_alert_ by either calling it as a module (`python -m git_alert`) or by directly using the installed package:
 
 ```
-usage: git_alert [-h] [--path PATH] [--only_dirty]
+usage: git_alert [-h] [--path PATH] [--only_dirty] [--ignore IGNORE]
 
 options:
-  -h, --help    show this help message and exit
-  --path PATH   top level directory to start the search in
-  --only_dirty  only show dirty repositories in the final report
+  -h, --help       show this help message and exit
+  --path PATH      top level directory to start the search in
+  --only_dirty     only show dirty repositories in the final report
+  --ignore IGNORE  colon separated list of paths to ignore
+
+Warning: adding a path to ignore will also ignore all subdirectories of that path.
 ```
 
 ## Development:
 
 The tool is aimed to be improved and extended going forward. If you have any ideas or want to contribute, feel free to open an issue or a pull request.
 
 ## Goals:
```

### Comparing `git_alert-0.1.0/git_alert/traverse.py` & `git_alert-0.2.0/git_alert/traverse.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,48 +3,50 @@
 import sys
 from pathlib import Path
 
 from git_alert.repositories import Repositories
 
 
 class GitAlert:
-    def __init__(self, pth: Path, repos: Repositories):
+    def __init__(self, pth: Path, repos: Repositories, ignore: list[str] = []) -> None:
         self._pth = pth
         self._repos = repos
+        self._ignore = {pth: True for pth in ignore}
 
     def traverse(self, pth: Path) -> None:
         """
         Traverse the directory and its subdirectories and check if it is a git repository.
         args:
             pth: Path
         """
+        if pth in self._ignore:
+            return
+
         try:
-            files = pth.glob("*")
-            for file in files:
-                if file.is_dir() and file.name == ".git":
-                    self.check(file)
+            files = list(pth.glob("*"))
 
-                elif file.is_dir():
-                    self.traverse(file)
+            if pth.joinpath(".git") in files:
+                repo = {}
+                repo["path"] = pth
+                repo["status"] = None
+                self._repos.add_repo(repo)
+            else:
+                for file in files:
+                    if file.is_dir():
+                        self.traverse(file)
         except PermissionError:
             print(f"Warning: no access to: {pth}", file=sys.stderr)
 
-    def check(self, pth: Path) -> None:
+    def check(self) -> None:
         """
-        Check if the git repository is clean or dirty.
-        args:
-            pth: Path
+        Check if the git repositories found are clean or dirty.
         """
-        repo = {}
-        output = subprocess.run(
-            ["git", "status"], cwd=pth.parent, stdout=subprocess.PIPE
-        )
-        if "working tree clean" in output.stdout.decode():
-            repo[pth.parent] = "clean"
-            self._repos.add_repo(repo)
-        else:
-            repo[pth.parent] = "dirty"
-            self._repos.add_repo(repo)
+        for pth, repo in self._repos.repos.items():
+            output = subprocess.run(["git", "status"], cwd=pth, stdout=subprocess.PIPE)
+            if "working tree clean" in output.stdout.decode():
+                repo["status"] = "clean"
+            else:
+                repo["status"] = "dirty"
 
     @property
     def repos(self) -> Repositories:
         return self._repos
```

### Comparing `git_alert-0.1.0/pyproject.toml` & `git_alert-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "git_alert"
-version = "0.1.0"
+version = "0.2.0"
 description = "Checks a given path and its sub-directories for dirty git repositories."
 authors = ["Simon Antonius Lauer <simon.lauer@posteo.de>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "git_alert"}]
 
 [tool.poetry.dependencies]
@@ -18,18 +18,13 @@
 
 [tool.poetry.group.development.dependencies]
 flake8 = "^7.0.0"
 black = "^24.3.0"
 pre-commit = "^3.7.0"
 
 
-[tool.poetry.group.publish.dependencies]
-badgie = "^0.12.0"
-coverage = "^7.4.4"
-coverage-badge = "^1.1.0"
-
 [tool.poetry.scripts]
 git_alert = "git_alert.scripts.git_alert:run"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `git_alert-0.1.0/PKG-INFO` & `git_alert-0.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git_alert
-Version: 0.1.0
+Version: 0.2.0
 Summary: Checks a given path and its sub-directories for dirty git repositories.
 License: MIT
 Author: Simon Antonius Lauer
 Author-email: simon.lauer@posteo.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,25 +18,27 @@
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 ![Codecov](https://img.shields.io/codecov/c/github/nomisreual/git_alert)
 
 This is a Python application that checks in the given directory and all its subdirectories
 for any dirty repositories.
 
+The source code is available on [GitHub](https://github.com/nomisreual/git_alert).
+
 This application aims to ease the frequent use of git as it makes it easy to check for any untracked changes in any of your repositories.
 
 ## Installation:
 
-The application is now available on PyPI, so you can install it using pip:
+The application is now available on **PyPI**, so you can install it using _pip_:
 
 ```
 pip install git_alert
 ```
 
-Alternatively, you can use pipx to make it globally available:
+Alternatively, you can use _pipx_ to make it globally available:
 
 ```
 pipx install git_alert
 ```
 
 Of course you can also clone the repository and install it manually. The package is built using poetry, so the easiest way to build it locally would be
 to use poetry:
@@ -55,25 +57,78 @@
 
 or
 
 ```
 pipx install .
 ```
 
+If you are using flakes to manage your NixOS installation, you can add the provided flake to your
+inputs:
+
+```nix
+{
+  description = "Configuration";
+
+  inputs = {
+    ...
+    git_alert = {
+      url = "github:nomisreual/git_alert";
+      inputs.nixpkgs.follows = "nixpkgs";
+    };
+    ...
+  };
+  outputs = {
+    self,
+    nixpkgs,
+    ...
+  } @ inputs: {
+    # your configuration
+  };
+}
+```
+
+You can then add `git_alert` to your packages (don't forget to add `inputs` to the respective module):
+
+```nix
+# configuration.nix
+{
+  environment.systemPackages = with pkgs; [
+    ...
+
+    inputs.git_alert.packages."x86_64-linux".default
+    ...
+  ];
+}
+# home.nix
+{
+  home.packages = with pkgs; [
+    ...
+
+    inputs.git_alert.packages."x86_64-linux".default
+    ...
+  ];
+}
+```
+
+After rebuilding, you have git_alert at your fingertips and it gets updated whenever you update your flake.
+
 ## Usage:
 
 You can use _git_alert_ by either calling it as a module (`python -m git_alert`) or by directly using the installed package:
 
 ```
-usage: git_alert [-h] [--path PATH] [--only_dirty]
+usage: git_alert [-h] [--path PATH] [--only_dirty] [--ignore IGNORE]
 
 options:
-  -h, --help    show this help message and exit
-  --path PATH   top level directory to start the search in
-  --only_dirty  only show dirty repositories in the final report
+  -h, --help       show this help message and exit
+  --path PATH      top level directory to start the search in
+  --only_dirty     only show dirty repositories in the final report
+  --ignore IGNORE  colon separated list of paths to ignore
+
+Warning: adding a path to ignore will also ignore all subdirectories of that path.
 ```
 
 ## Development:
 
 The tool is aimed to be improved and extended going forward. If you have any ideas or want to contribute, feel free to open an issue or a pull request.
 
 ## Goals:
```

