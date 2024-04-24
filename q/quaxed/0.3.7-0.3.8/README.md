# Comparing `tmp/quaxed-0.3.7.tar.gz` & `tmp/quaxed-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed Mar 27 19:15:35 2024, max compression
+gzip compressed data, last modified: Wed Apr 24 03:58:22 2024, max compression
```

## Comparing `quaxed-0.3.7.tar` & `quaxed-0.3.8.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      380 2024-03-27 19:15:35.000000 quaxed-0.3.7/.copier-answers.yml
--rw-r--r--   0        0        0      125 2024-03-27 19:15:35.000000 quaxed-0.3.7/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-03-27 19:15:35.000000 quaxed-0.3.7/.gitattributes
--rw-r--r--   0        0        0     2899 2024-03-27 19:15:35.000000 quaxed-0.3.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-03-27 19:15:35.000000 quaxed-0.3.7/.readthedocs.yml
--rw-r--r--   0        0        0     2778 2024-03-27 19:15:35.000000 quaxed-0.3.7/noxfile.py
--rw-r--r--   0        0        0     2387 2024-03-27 19:15:35.000000 quaxed-0.3.7/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-03-27 19:15:35.000000 quaxed-0.3.7/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-03-27 19:15:35.000000 quaxed-0.3.7/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1539 2024-03-27 19:15:35.000000 quaxed-0.3.7/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1641 2024-03-27 19:15:35.000000 quaxed-0.3.7/.github/workflows/ci.yml
--rw-r--r--   0        0        0      834 2024-03-27 19:15:35.000000 quaxed-0.3.7/docs/conf.py
--rw-r--r--   0        0        0      193 2024-03-27 19:15:35.000000 quaxed-0.3.7/docs/index.md
--rw-r--r--   0        0        0      946 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/__init__.py
--rw-r--r--   0        0        0     1728 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/_jax.py
--rw-r--r--   0        0        0      411 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/_version.py
--rw-r--r--   0        0        0       82 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/_version.pyi
--rw-r--r--   0        0        0      620 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/lax.py
--rw-r--r--   0        0        0      407 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/operator.py
--rw-r--r--   0        0        0     2044 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/operator.pyi
--rw-r--r--   0        0        0        0 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/py.typed
--rw-r--r--   0        0        0     1687 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/array_api/__init__.py
--rw-r--r--   0        0        0      145 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/array_api/_constants.py
--rw-r--r--   0        0        0     7836 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/array_api/_creation_functions.py
--rw-r--r--   0        0        0      882 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/array_api/_data_type_functions.py
--rw-r--r--   0        0        0       89 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/array_api/_dispatch.py
--rw-r--r--   0        0        0     6639 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/array_api/_elementwise_functions.py
--rw-r--r--   0        0        0      287 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/array_api/_indexing_functions.py
--rw-r--r--   0        0        0      756 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/array_api/_linear_algebra_functions.py
--rw-r--r--   0        0        0     1716 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/array_api/_manipulation_functions.py
--rw-r--r--   0        0        0      772 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/array_api/_searching_functions.py
--rw-r--r--   0        0        0      630 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/array_api/_set_functions.py
--rw-r--r--   0        0        0      623 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/array_api/_sorting_functions.py
--rw-r--r--   0        0        0     1913 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/array_api/_statistical_functions.py
--rw-r--r--   0        0        0      723 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/array_api/_types.py
--rw-r--r--   0        0        0      569 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/array_api/_utility_functions.py
--rw-r--r--   0        0        0      158 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/array_api/_utils.py
--rw-r--r--   0        0        0     3447 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/array_api/fft.py
--rw-r--r--   0        0        0     3714 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/array_api/linalg.py
--rw-r--r--   0        0        0      253 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/numpy/__init__.py
--rw-r--r--   0        0        0     8914 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/numpy/_core.py
--rw-r--r--   0        0        0       84 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/scipy/__init__.py
--rw-r--r--   0        0        0     1025 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/scipy/special.py
--rw-r--r--   0        0        0     1925 2024-03-27 19:15:35.000000 quaxed-0.3.7/src/quaxed/scipy/special.pyi
--rw-r--r--   0        0        0       21 2024-03-27 19:15:35.000000 quaxed-0.3.7/tests/__init__.py
--rw-r--r--   0        0        0    38885 2024-03-27 19:15:35.000000 quaxed-0.3.7/tests/myarray.py
--rw-r--r--   0        0        0      177 2024-03-27 19:15:35.000000 quaxed-0.3.7/tests/test_package.py
--rw-r--r--   0        0        0       31 2024-03-27 19:15:35.000000 quaxed-0.3.7/tests/array_api/__init__.py
--rw-r--r--   0        0        0     1710 2024-03-27 19:15:35.000000 quaxed-0.3.7/tests/array_api/test_jax.py
--rw-r--r--   0        0        0    35919 2024-03-27 19:15:35.000000 quaxed-0.3.7/tests/array_api/test_myarray.py
--rw-r--r--   0        0        0       27 2024-03-27 19:15:35.000000 quaxed-0.3.7/tests/numpy/__init__.py
--rw-r--r--   0        0        0     1784 2024-03-27 19:15:35.000000 quaxed-0.3.7/tests/numpy/test_jax.py
--rw-r--r--   0        0        0     2218 2024-03-27 19:15:35.000000 quaxed-0.3.7/.gitignore
--rw-r--r--   0        0        0     1528 2024-03-27 19:15:35.000000 quaxed-0.3.7/LICENSE
--rw-r--r--   0        0        0     1553 2024-03-27 19:15:35.000000 quaxed-0.3.7/README.md
--rw-r--r--   0        0        0     4254 2024-03-27 19:15:35.000000 quaxed-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     3289 2024-03-27 19:15:35.000000 quaxed-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0      380 2024-04-24 03:58:22.000000 quaxed-0.3.8/.copier-answers.yml
+-rw-r--r--   0        0        0      125 2024-04-24 03:58:22.000000 quaxed-0.3.8/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-04-24 03:58:22.000000 quaxed-0.3.8/.gitattributes
+-rw-r--r--   0        0        0     2899 2024-04-24 03:58:22.000000 quaxed-0.3.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-04-24 03:58:22.000000 quaxed-0.3.8/.readthedocs.yml
+-rw-r--r--   0        0        0     2778 2024-04-24 03:58:22.000000 quaxed-0.3.8/noxfile.py
+-rw-r--r--   0        0        0     2387 2024-04-24 03:58:22.000000 quaxed-0.3.8/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-04-24 03:58:22.000000 quaxed-0.3.8/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-04-24 03:58:22.000000 quaxed-0.3.8/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     1539 2024-04-24 03:58:22.000000 quaxed-0.3.8/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1641 2024-04-24 03:58:22.000000 quaxed-0.3.8/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      834 2024-04-24 03:58:22.000000 quaxed-0.3.8/docs/conf.py
+-rw-r--r--   0        0        0      193 2024-04-24 03:58:22.000000 quaxed-0.3.8/docs/index.md
+-rw-r--r--   0        0        0      945 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/__init__.py
+-rw-r--r--   0        0        0     1728 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/_jax.py
+-rw-r--r--   0        0        0      411 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/_version.py
+-rw-r--r--   0        0        0       82 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/_version.pyi
+-rw-r--r--   0        0        0      620 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/lax.py
+-rw-r--r--   0        0        0      407 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/operator.py
+-rw-r--r--   0        0        0     2044 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/operator.pyi
+-rw-r--r--   0        0        0        0 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/py.typed
+-rw-r--r--   0        0        0     1687 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_constants.py
+-rw-r--r--   0        0        0     7836 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_creation_functions.py
+-rw-r--r--   0        0        0      882 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_data_type_functions.py
+-rw-r--r--   0        0        0       89 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_dispatch.py
+-rw-r--r--   0        0        0     6639 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_elementwise_functions.py
+-rw-r--r--   0        0        0      287 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_indexing_functions.py
+-rw-r--r--   0        0        0      756 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_linear_algebra_functions.py
+-rw-r--r--   0        0        0     1716 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_manipulation_functions.py
+-rw-r--r--   0        0        0      772 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_searching_functions.py
+-rw-r--r--   0        0        0      630 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_set_functions.py
+-rw-r--r--   0        0        0      623 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_sorting_functions.py
+-rw-r--r--   0        0        0     1913 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_statistical_functions.py
+-rw-r--r--   0        0        0      707 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_types.py
+-rw-r--r--   0        0        0      569 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_utility_functions.py
+-rw-r--r--   0        0        0      158 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_utils.py
+-rw-r--r--   0        0        0     3447 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/fft.py
+-rw-r--r--   0        0        0     3714 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/linalg.py
+-rw-r--r--   0        0        0      253 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/numpy/__init__.py
+-rw-r--r--   0        0        0     8948 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/numpy/_core.py
+-rw-r--r--   0        0        0       84 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/scipy/__init__.py
+-rw-r--r--   0        0        0     1030 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/scipy/special.py
+-rw-r--r--   0        0        0     1925 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/scipy/special.pyi
+-rw-r--r--   0        0        0       21 2024-04-24 03:58:22.000000 quaxed-0.3.8/tests/__init__.py
+-rw-r--r--   0        0        0    38885 2024-04-24 03:58:22.000000 quaxed-0.3.8/tests/myarray.py
+-rw-r--r--   0        0        0      177 2024-04-24 03:58:22.000000 quaxed-0.3.8/tests/test_package.py
+-rw-r--r--   0        0        0       31 2024-04-24 03:58:22.000000 quaxed-0.3.8/tests/array_api/__init__.py
+-rw-r--r--   0        0        0     1710 2024-04-24 03:58:22.000000 quaxed-0.3.8/tests/array_api/test_jax.py
+-rw-r--r--   0        0        0    35919 2024-04-24 03:58:22.000000 quaxed-0.3.8/tests/array_api/test_myarray.py
+-rw-r--r--   0        0        0       27 2024-04-24 03:58:22.000000 quaxed-0.3.8/tests/numpy/__init__.py
+-rw-r--r--   0        0        0     1784 2024-04-24 03:58:22.000000 quaxed-0.3.8/tests/numpy/test_jax.py
+-rw-r--r--   0        0        0     2218 2024-04-24 03:58:22.000000 quaxed-0.3.8/.gitignore
+-rw-r--r--   0        0        0     1528 2024-04-24 03:58:22.000000 quaxed-0.3.8/LICENSE
+-rw-r--r--   0        0        0     1553 2024-04-24 03:58:22.000000 quaxed-0.3.8/README.md
+-rw-r--r--   0        0        0     4254 2024-04-24 03:58:22.000000 quaxed-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     3289 2024-04-24 03:58:22.000000 quaxed-0.3.8/PKG-INFO
```

### Comparing `quaxed-0.3.7/.pre-commit-config.yaml` & `quaxed-0.3.8/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,26 @@
   autofix_commit_msg: "style: pre-commit fixes"
   autoupdate_schedule: "monthly"
 
 default_stages: [pre-commit, pre-push]
 
 repos:
   - repo: https://github.com/commitizen-tools/commitizen
-    rev: v3.14.1
+    rev: v3.21.3
     hooks:
       - id: commitizen
       - id: commitizen-branch
         stages: [push]
 
   - repo: meta
     hooks:
       - id: check-useless-excludes
 
   - repo: https://github.com/scientific-python/cookie
-    rev: 2024.01.24
+    rev: 2024.03.10
     hooks:
       - id: sp-repo-review
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: "v4.5.0"
     hooks:
       - id: check-added-large-files
@@ -43,22 +43,22 @@
     rev: "v1.10.0"
     hooks:
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.27.4
+    rev: 0.28.1
     hooks:
       - id: check-dependabot
       - id: check-github-workflows
       - id: check-readthedocs
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.2.0"
+    rev: "v0.3.5"
     hooks:
       # Run the linter
       - id: ruff
         types_or: [python, pyi, jupyter]
         args: ["--fix", "--show-fixes"]
       # Run the formatter
       - id: ruff-format
@@ -74,15 +74,15 @@
     rev: "v4.0.0-alpha.8"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: "v1.8.0"
+    rev: "v1.9.0"
     hooks:
       - id: mypy
         files: src
         additional_dependencies:
           - pytest
         exclude: |
           (?x)^(
```

### Comparing `quaxed-0.3.7/noxfile.py` & `quaxed-0.3.8/noxfile.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/.github/CONTRIBUTING.md` & `quaxed-0.3.8/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/.github/matchers/pylint.json` & `quaxed-0.3.8/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/.github/workflows/cd.yml` & `quaxed-0.3.8/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/.github/workflows/ci.yml` & `quaxed-0.3.8/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -62,8 +62,8 @@
 
       - name: Test package
         run: >-
           python -m pytest tests/ src/ docs/ -ra --cov --cov-report=xml
           --cov-report=term --durations=20
 
       - name: Upload coverage report
-        uses: codecov/codecov-action@v4.1.0
+        uses: codecov/codecov-action@v4.3.0
```

### Comparing `quaxed-0.3.7/docs/conf.py` & `quaxed-0.3.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/src/quaxed/__init__.py` & `quaxed-0.3.8/src/quaxed/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Copyright (c) 2023 Nathaniel Starkman. All rights reserved.
 
 quaxed: Array-API JAX compatibility
 """
 
 # pylint: disable=redefined-builtin
 
-
 __all__ = ["__version__", "array_api"]
 
 from typing import Any
 
 import plum
 from jaxtyping import ArrayLike
```

### Comparing `quaxed-0.3.7/src/quaxed/_jax.py` & `quaxed-0.3.8/src/quaxed/_jax.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/src/quaxed/lax.py` & `quaxed-0.3.8/src/quaxed/lax.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/src/quaxed/operator.pyi` & `quaxed-0.3.8/src/quaxed/operator.pyi`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/src/quaxed/array_api/__init__.py` & `quaxed-0.3.8/src/quaxed/array_api/__init__.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/src/quaxed/array_api/_creation_functions.py` & `quaxed-0.3.8/src/quaxed/array_api/_creation_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/src/quaxed/array_api/_data_type_functions.py` & `quaxed-0.3.8/src/quaxed/array_api/_data_type_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/src/quaxed/array_api/_elementwise_functions.py` & `quaxed-0.3.8/src/quaxed/array_api/_elementwise_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/src/quaxed/array_api/_linear_algebra_functions.py` & `quaxed-0.3.8/src/quaxed/array_api/_linear_algebra_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/src/quaxed/array_api/_manipulation_functions.py` & `quaxed-0.3.8/src/quaxed/array_api/_manipulation_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/src/quaxed/array_api/_searching_functions.py` & `quaxed-0.3.8/src/quaxed/array_api/_searching_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/src/quaxed/array_api/_set_functions.py` & `quaxed-0.3.8/src/quaxed/array_api/_set_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/src/quaxed/array_api/_sorting_functions.py` & `quaxed-0.3.8/src/quaxed/array_api/_sorting_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/src/quaxed/array_api/_statistical_functions.py` & `quaxed-0.3.8/src/quaxed/array_api/_statistical_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/src/quaxed/array_api/_types.py` & `quaxed-0.3.8/src/quaxed/array_api/_types.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,12 +25,10 @@
 _T_co = TypeVar("_T_co", covariant=True)
 
 
 @runtime_checkable
 class NestedSequence(Protocol[_T_co]):
     """A nested sequence."""
 
-    def __getitem__(self, key: int, /) -> "_T_co | NestedSequence[_T_co]":
-        ...
+    def __getitem__(self, key: int, /) -> "_T_co | NestedSequence[_T_co]": ...
 
-    def __len__(self, /) -> int:
-        ...
+    def __len__(self, /) -> int: ...
```

### Comparing `quaxed-0.3.7/src/quaxed/array_api/_utility_functions.py` & `quaxed-0.3.8/src/quaxed/array_api/_utility_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/src/quaxed/array_api/fft.py` & `quaxed-0.3.8/src/quaxed/array_api/fft.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/src/quaxed/array_api/linalg.py` & `quaxed-0.3.8/src/quaxed/array_api/linalg.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/src/quaxed/numpy/_core.py` & `quaxed-0.3.8/src/quaxed/numpy/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     "isclose",
     "log",
     "log10",
     "matmul",
     "moveaxis",
     "power",
     "squeeze",
+    "tan",
     "trace",
     "vectorize",
 ]
 
 import functools
 from collections.abc import Callable, Collection
 from typing import Any, TypeVar
@@ -75,14 +76,15 @@
 isclose = quaxify(jnp.isclose)
 log = quaxify(jnp.log)
 log10 = quaxify(jnp.log10)
 matmul = quaxify(jnp.matmul)
 moveaxis = quaxify(jnp.moveaxis)
 power = quaxify(jnp.power)
 squeeze = quaxify(jnp.squeeze)
+tan = quaxify(jnp.tan)
 trace = quaxify(jnp.trace)
 
 
 # =====================================
 # `jax.numpy.vectorize`
```

### Comparing `quaxed-0.3.7/src/quaxed/scipy/special.py` & `quaxed-0.3.8/src/quaxed/scipy/special.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+# ruff:noqa: F822
+
 """Quaxed :mod:`jax.scipy.special`."""
 
-__all__ = [  # noqa: F822
+__all__ = [
     "bernoulli",
     "betainc",
     "betaln",
     "beta",
     "bessel_jn",
     "digamma",
     "entr",
```

### Comparing `quaxed-0.3.7/src/quaxed/scipy/special.pyi` & `quaxed-0.3.8/src/quaxed/scipy/special.pyi`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/tests/myarray.py` & `quaxed-0.3.8/tests/myarray.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/tests/array_api/test_jax.py` & `quaxed-0.3.8/tests/array_api/test_jax.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/tests/array_api/test_myarray.py` & `quaxed-0.3.8/tests/array_api/test_myarray.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/tests/numpy/test_jax.py` & `quaxed-0.3.8/tests/numpy/test_jax.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/.gitignore` & `quaxed-0.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/LICENSE` & `quaxed-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/README.md` & `quaxed-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/pyproject.toml` & `quaxed-0.3.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.7/PKG-INFO` & `quaxed-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: quaxed
-Version: 0.3.7
+Version: 0.3.8
 Summary: Array-API JAX compatibility
 Project-URL: Homepage, https://github.com/GalacticDynamics/quaxed
 Project-URL: Bug Tracker, https://github.com/GalacticDynamics/quaxed/issues
 Project-URL: Discussions, https://github.com/GalacticDynamics/quaxed/discussions
 Project-URL: Changelog, https://github.com/GalacticDynamics/quaxed/releases
 Author-email: Nathaniel Starkman <nstarman@users.noreply.github.com>
 License-File: LICENSE
```

