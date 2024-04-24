# Comparing `tmp/loamy-0.0.6.tar.gz` & `tmp/loamy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loamy-0.0.6.tar", max compression
+gzip compressed data, was "loamy-0.0.7.tar", max compression
```

## Comparing `loamy-0.0.6.tar` & `loamy-0.0.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2024-04-21 00:14:10.021277 loamy-0.0.6/LICENSE
--rw-r--r--   0        0        0     2776 2024-04-21 00:14:10.021277 loamy-0.0.6/README.md
--rw-r--r--   0        0        0     1316 2024-04-21 00:14:10.021277 loamy-0.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-21 00:14:10.021277 loamy-0.0.6/src/loamy/__init__.py
--rw-r--r--   0        0        0     6055 2024-04-21 00:14:10.021277 loamy-0.0.6/src/loamy/session.py
--rw-r--r--   0        0        0     3525 1970-01-01 00:00:00.000000 loamy-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-24 01:45:20.515570 loamy-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2973 2024-04-24 01:45:20.515570 loamy-0.0.7/README.md
+-rw-r--r--   0        0        0     1340 2024-04-24 01:45:20.515570 loamy-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 01:45:20.515570 loamy-0.0.7/src/loamy/__init__.py
+-rw-r--r--   0        0        0    10583 2024-04-24 01:45:20.515570 loamy-0.0.7/src/loamy/session.py
+-rw-r--r--   0        0        0     3761 1970-01-01 00:00:00.000000 loamy-0.0.7/PKG-INFO
```

### Comparing `loamy-0.0.6/LICENSE` & `loamy-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `loamy-0.0.6/README.md` & `loamy-0.0.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 ![CI Workflow](https://github.com/fullerzz/zConcurrent/actions/workflows/ci.yml/badge.svg)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
+[![PyPI version](https://badge.fury.io/py/loamy.svg)](https://badge.fury.io/py/loamy)
+[![MIT License](https://img.shields.io/badge/license-MIT-blue)](https://img.shields.io/badge/license-MIT-blue)
 
 # Overview
 
 This project allows you to execute a list of http operations asynchronously from within an synchronous context.
 
 It does not care whether you should do this. It simply allows you to do so if you desire.
```

### Comparing `loamy-0.0.6/pyproject.toml` & `loamy-0.0.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "loamy"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = ["Zach Fuller <zach.fuller1222@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/fullerzz/loamy"
 packages = [{include = "loamy", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = ">=3.9.5"
 aiodns = "~3.1.1"
 msgspec = "~0.18.6"
 uvloop = { version = "0.19.0", optional = true }
+loguru = "^0.7.2"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "~0.3.7"
+ruff = "^0.4.0"
 pre-commit = "3.5.0"
 pytest = "^7.4.4"
 pytest-asyncio = "^0.21.1"
 blacksheep = "^2.0.7"
 uvicorn = "^0.24.0.post1"
 mypy = "^1.9.0"
 pip-audit = "^2.7.2"
@@ -34,15 +35,15 @@
 line-length = 88
 indent-width = 4
 
 target-version = "py310"
 
 [tool.ruff.lint]
 select = ["E", "F", "W", "C90", "I", "N", "UP", "ASYNC", "S", "B", "ERA", "PLE", "PLW", "PERF", "RUF"]
-ignore = []
+ignore = ["E501"]
 
 # Allow fix for all enabled rules (when `--fix`) is provided.
 fixable = ["ALL"]
 unfixable = []
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
```

### Comparing `loamy-0.0.6/PKG-INFO` & `loamy-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: loamy
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Home-page: https://github.com/fullerzz/loamy
 License: MIT
 Author: Zach Fuller
 Author-email: zach.fuller1222@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: uvloop
 Requires-Dist: aiodns (>=3.1.1,<3.2.0)
 Requires-Dist: aiohttp (>=3.9.5)
+Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: msgspec (>=0.18.6,<0.19.0)
 Requires-Dist: uvloop (==0.19.0) ; extra == "uvloop"
 Project-URL: Repository, https://github.com/fullerzz/loamy
 Description-Content-Type: text/markdown
 
 ![CI Workflow](https://github.com/fullerzz/zConcurrent/actions/workflows/ci.yml/badge.svg)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
+[![PyPI version](https://badge.fury.io/py/loamy.svg)](https://badge.fury.io/py/loamy)
+[![MIT License](https://img.shields.io/badge/license-MIT-blue)](https://img.shields.io/badge/license-MIT-blue)
 
 # Overview
 
 This project allows you to execute a list of http operations asynchronously from within an synchronous context.
 
 It does not care whether you should do this. It simply allows you to do so if you desire.
```

