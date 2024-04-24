# Comparing `tmp/nova_sdk-0.0.0.3.tar.gz` & `tmp/nova_sdk-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nova_sdk-0.0.0.3.tar", max compression
+gzip compressed data, was "nova_sdk-0.0.1.tar", max compression
```

## Comparing `nova_sdk-0.0.0.3.tar` & `nova_sdk-0.0.1.tar`

### file list

```diff
@@ -1,10 +1,6 @@
--rw-r--r--   0        0        0     1069 2024-04-24 15:02:06.504712 nova_sdk-0.0.0.3/LICENSE
--rw-r--r--   0        0        0     2279 2024-04-24 15:02:06.504712 nova_sdk-0.0.0.3/README.md
--rw-r--r--   0        0        0        0 2024-04-24 15:02:06.504712 nova_sdk-0.0.0.3/nova_sdk/__init__.py
--rw-r--r--   0        0        0     1067 2024-04-24 15:02:06.504712 nova_sdk-0.0.0.3/nova_sdk/config.py
--rw-r--r--   0        0        0     1343 2024-04-24 15:02:06.504712 nova_sdk-0.0.0.3/nova_sdk/deposit.py
--rw-r--r--   0        0        0      302 2024-04-24 15:02:06.504712 nova_sdk-0.0.0.3/nova_sdk/exceptions.py
--rw-r--r--   0        0        0      206 2024-04-24 15:02:06.504712 nova_sdk-0.0.0.3/nova_sdk/utils.py
--rw-r--r--   0        0        0     1427 2024-04-24 15:02:06.504712 nova_sdk-0.0.0.3/nova_sdk/withdraw.py
--rw-r--r--   0        0        0     1918 2024-04-24 15:02:25.092669 nova_sdk-0.0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3112 1970-01-01 00:00:00.000000 nova_sdk-0.0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-23 05:12:54.554887 nova_sdk-0.0.1/LICENSE
+-rw-r--r--   0        0        0     2748 2024-04-23 05:12:54.554887 nova_sdk-0.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 05:12:54.554887 nova_sdk-0.0.1/nova_python_sdk/__init__.py
+-rw-r--r--   0        0        0      273 2024-04-23 05:12:54.554887 nova_sdk-0.0.1/nova_python_sdk/foo.py
+-rw-r--r--   0        0        0     1921 2024-04-23 05:13:12.426958 nova_sdk-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3542 1970-01-01 00:00:00.000000 nova_sdk-0.0.1/PKG-INFO
```

### Comparing `nova_sdk-0.0.0.3/LICENSE` & `nova_sdk-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nova_sdk-0.0.0.3/README.md` & `nova_sdk-0.0.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 # nova-python-sdk
 
-[![Release](https://img.shields.io/github/v/release/solidi-labs/nova-python-sdk)](https://img.shields.io/github/v/release/solidi-labs/nova-python-sdk)
-[![Build status](https://img.shields.io/github/actions/workflow/status/solidi-labs/nova-python-sdk/main.yml?branch=main)](https://github.com/solidi-labs/nova-python-sdk/actions/workflows/main.yml?query=branch%3Amain)
-[![codecov](https://codecov.io/gh/solidi-labs/nova-python-sdk/branch/main/graph/badge.svg)](https://codecov.io/gh/solidi-labs/nova-python-sdk)
-[![Commit activity](https://img.shields.io/github/commit-activity/m/solidi-labs/nova-python-sdk)](https://img.shields.io/github/commit-activity/m/solidi-labs/nova-python-sdk)
-[![License](https://img.shields.io/github/license/solidi-labs/nova-python-sdk)](https://img.shields.io/github/license/solidi-labs/nova-python-sdk)
+[![Release](https://img.shields.io/github/v/release/lakonema2000/nova-python-sdk)](https://img.shields.io/github/v/release/lakonema2000/nova-python-sdk)
+[![Build status](https://img.shields.io/github/actions/workflow/status/lakonema2000/nova-python-sdk/main.yml?branch=main)](https://github.com/lakonema2000/nova-python-sdk/actions/workflows/main.yml?query=branch%3Amain)
+[![codecov](https://codecov.io/gh/lakonema2000/nova-python-sdk/branch/main/graph/badge.svg)](https://codecov.io/gh/lakonema2000/nova-python-sdk)
+[![Commit activity](https://img.shields.io/github/commit-activity/m/lakonema2000/nova-python-sdk)](https://img.shields.io/github/commit-activity/m/lakonema2000/nova-python-sdk)
+[![License](https://img.shields.io/github/license/lakonema2000/nova-python-sdk)](https://img.shields.io/github/license/lakonema2000/nova-python-sdk)
 
 This is a template repository for Python projects that use Poetry for their dependency management.
 
-- **Github repository**: <https://github.com/Solidi-Labs/nova-python-sdk/>
-- **Documentation** <https://solidi-labs.github.io/nova-python-sdk/>
+- **Github repository**: <https://github.com/lakonema2000/nova-python-sdk/>
+- **Documentation** <https://lakonema2000.github.io/nova-python-sdk/>
 
 ## Getting started with your project
 
-Install the environment and the pre-commit hooks with
+First, create a repository on GitHub with the same name as this project, and then run the following commands:
+
+```bash
+git init -b main
+git add .
+git commit -m "init commit"
+git remote add origin git@github.com:lakonema2000/nova-python-sdk.git
+git push -u origin main
+```
+
+Finally, install the environment and the pre-commit hooks with
 
 ```bash
 make install
 ```
 
+You are now ready to start development on your project!
+The CI/CD pipeline will be triggered when you open a pull request, merge to main, or when you create a new release.
+
 To finalize the set-up for publishing to PyPi or Artifactory, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/publishing/#set-up-for-pypi).
 For activating the automatic documentation with MkDocs, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/mkdocs/#enabling-the-documentation-on-github).
 To enable the code coverage reports, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/codecov/).
 
 ## Releasing a new version
 
 - Create an API Token on [Pypi](https://pypi.org/).
-- Add the API Token to your projects secrets with the name `PYPI_TOKEN` by visiting [this page](https://github.com/solidi-labs/nova-python-sdk/settings/secrets/actions/new).
-- Create a [new release](https://github.com/solidi-labs/nova-python-sdk/releases/new) on Github.
+- Add the API Token to your projects secrets with the name `PYPI_TOKEN` by visiting [this page](https://github.com/lakonema2000/nova-python-sdk/settings/secrets/actions/new).
+- Create a [new release](https://github.com/lakonema2000/nova-python-sdk/releases/new) on Github.
 - Create a new tag in the form `*.*.*`.
 
 For more details, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/cicd/#how-to-trigger-a-release).
 
 ---
 
 Repository initiated with [fpgmaas/cookiecutter-poetry](https://github.com/fpgmaas/cookiecutter-poetry).
```

### Comparing `nova_sdk-0.0.0.3/pyproject.toml` & `nova_sdk-0.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tool.poetry]
 name = "nova-sdk"
-version = "0.0.0.3"
+version = "0.0.1"
 description = "This is a template repository for Python projects that use Poetry for their dependency management."
 authors = ["Solidi Labs <lakonema2000@gmail.com>"]
 repository = "https://github.com/Solidi-Labs/nova-python-sdk"
-documentation = "https://solidi-labs.github.io/nova-python-sdk/"
+documentation = "https://lakonema2000.github.io/nova-python-sdk/"
 readme = "README.md"
 packages = [
-  {include = "nova_sdk"}
+  {include = "nova_python_sdk"}
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
-web3 = "^6.17.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 deptry = "^0.12.0"
 mypy = "^1.5.1"
 pre-commit = "^3.4.0"
@@ -28,15 +27,15 @@
 mkdocstrings = {extras = ["python"], version = "^0.23.0"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
-files = ["nova_sdk"]
+files = ["nova_python_sdk"]
 disallow_untyped_defs = "True"
 disallow_any_unimported = "True"
 no_implicit_optional = "True"
 check_untyped_defs = "True"
 warn_return_any = "True"
 warn_unused_ignores = "True"
 show_error_codes = "True"
@@ -91,12 +90,12 @@
 preview = true
 
 [tool.coverage.report]
 skip_empty = true
 
 [tool.coverage.run]
 branch = true
-source = ["nova_sdk"]
+source = ["nova_python_sdk"]
 
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["S101"]
```

