# Comparing `tmp/nova_sdk-0.0.0.1.tar.gz` & `tmp/nova_sdk-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nova_sdk-0.0.0.1.tar", max compression
+gzip compressed data, was "nova_sdk-0.0.1.tar", max compression
```

## Comparing `nova_sdk-0.0.0.1.tar` & `nova_sdk-0.0.1.tar`

### file list

```diff
@@ -1,10 +1,6 @@
--rw-r--r--   0        0        0     1069 2024-04-24 13:43:19.062108 nova_sdk-0.0.0.1/LICENSE
--rw-r--r--   0        0        0     2748 2024-04-24 13:43:19.062108 nova_sdk-0.0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-04-24 13:43:19.062108 nova_sdk-0.0.0.1/nova_sdk/__init__.py
--rw-r--r--   0        0        0     1067 2024-04-24 13:43:19.062108 nova_sdk-0.0.0.1/nova_sdk/config.py
--rw-r--r--   0        0        0     1343 2024-04-24 13:43:19.062108 nova_sdk-0.0.0.1/nova_sdk/deposit.py
--rw-r--r--   0        0        0      302 2024-04-24 13:43:19.062108 nova_sdk-0.0.0.1/nova_sdk/exceptions.py
--rw-r--r--   0        0        0      206 2024-04-24 13:43:19.062108 nova_sdk-0.0.0.1/nova_sdk/utils.py
--rw-r--r--   0        0        0     1427 2024-04-24 13:43:19.062108 nova_sdk-0.0.0.1/nova_sdk/withdraw.py
--rw-r--r--   0        0        0     1919 2024-04-24 13:43:42.974171 nova_sdk-0.0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3582 1970-01-01 00:00:00.000000 nova_sdk-0.0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-23 05:12:54.554887 nova_sdk-0.0.1/LICENSE
+-rw-r--r--   0        0        0     2748 2024-04-23 05:12:54.554887 nova_sdk-0.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 05:12:54.554887 nova_sdk-0.0.1/nova_python_sdk/__init__.py
+-rw-r--r--   0        0        0      273 2024-04-23 05:12:54.554887 nova_sdk-0.0.1/nova_python_sdk/foo.py
+-rw-r--r--   0        0        0     1921 2024-04-23 05:13:12.426958 nova_sdk-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3542 1970-01-01 00:00:00.000000 nova_sdk-0.0.1/PKG-INFO
```

### Comparing `nova_sdk-0.0.0.1/LICENSE` & `nova_sdk-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nova_sdk-0.0.0.1/README.md` & `nova_sdk-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nova_sdk-0.0.0.1/pyproject.toml` & `nova_sdk-0.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tool.poetry]
 name = "nova-sdk"
-version = "0.0.0.1"
+version = "0.0.1"
 description = "This is a template repository for Python projects that use Poetry for their dependency management."
 authors = ["Solidi Labs <lakonema2000@gmail.com>"]
 repository = "https://github.com/Solidi-Labs/nova-python-sdk"
 documentation = "https://lakonema2000.github.io/nova-python-sdk/"
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

### Comparing `nova_sdk-0.0.0.1/PKG-INFO` & `nova_sdk-0.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: nova-sdk
-Version: 0.0.0.1
+Version: 0.0.1
 Summary: This is a template repository for Python projects that use Poetry for their dependency management.
 Home-page: https://github.com/Solidi-Labs/nova-python-sdk
 Author: Solidi Labs
 Author-email: lakonema2000@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: web3 (>=6.17.2,<7.0.0)
 Project-URL: Documentation, https://lakonema2000.github.io/nova-python-sdk/
 Project-URL: Repository, https://github.com/Solidi-Labs/nova-python-sdk
 Description-Content-Type: text/markdown
 
 # nova-python-sdk
 
 [![Release](https://img.shields.io/github/v/release/lakonema2000/nova-python-sdk)](https://img.shields.io/github/v/release/lakonema2000/nova-python-sdk)
```

