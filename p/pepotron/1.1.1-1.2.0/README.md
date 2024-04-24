# Comparing `tmp/pepotron-1.1.1.tar.gz` & `tmp/pepotron-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, last modified: Wed Apr 24 15:03:24 2024, max compression
```

## Comparing `pepotron-1.1.1.tar` & `pepotron-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 pepotron-1.1.1/.coveragerc
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pepotron-1.1.1/.editorconfig
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pepotron-1.1.1/.flake8
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 pepotron-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pepotron-1.1.1/RELEASING.md
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 pepotron-1.1.1/tox.ini
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 pepotron-1.1.1/.github/labels.yml
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 pepotron-1.1.1/.github/release-drafter.yml
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pepotron-1.1.1/.github/renovate.json
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pepotron-1.1.1/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 pepotron-1.1.1/.github/workflows/labels.yml
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pepotron-1.1.1/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pepotron-1.1.1/.github/workflows/release-drafter.yml
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 pepotron-1.1.1/.github/workflows/require-pr-label.yml
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 pepotron-1.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 pepotron-1.1.1/src/pepotron/__init__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pepotron-1.1.1/src/pepotron/__main__.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 pepotron-1.1.1/src/pepotron/_cache.py
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 pepotron-1.1.1/src/pepotron/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pepotron-1.1.1/src/pepotron/scripts/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pepotron-1.1.1/src/pepotron/scripts/run_command.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pepotron-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 pepotron-1.1.1/tests/test_cache.py
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 pepotron-1.1.1/tests/test_pepotron.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 pepotron-1.1.1/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pepotron-1.1.1/LICENSE.txt
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 pepotron-1.1.1/README.md
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 pepotron-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 pepotron-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      409 2024-04-24 15:03:24.000000 pepotron-1.2.0/.coveragerc
+-rw-r--r--   0        0        0      368 2024-04-24 15:03:24.000000 pepotron-1.2.0/.editorconfig
+-rw-r--r--   0        0        0     1807 2024-04-24 15:03:24.000000 pepotron-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      816 2024-04-24 15:03:24.000000 pepotron-1.2.0/RELEASING.md
+-rw-r--r--   0        0        0      667 2024-04-24 15:03:24.000000 pepotron-1.2.0/tox.ini
+-rw-r--r--   0        0        0     1074 2024-04-24 15:03:24.000000 pepotron-1.2.0/.github/labels.yml
+-rw-r--r--   0        0        0      892 2024-04-24 15:03:24.000000 pepotron-1.2.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0      350 2024-04-24 15:03:24.000000 pepotron-1.2.0/.github/renovate.json
+-rw-r--r--   0        0        0     1725 2024-04-24 15:03:24.000000 pepotron-1.2.0/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      389 2024-04-24 15:03:24.000000 pepotron-1.2.0/.github/workflows/labels.yml
+-rw-r--r--   0        0        0      321 2024-04-24 15:03:24.000000 pepotron-1.2.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1084 2024-04-24 15:03:24.000000 pepotron-1.2.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      517 2024-04-24 15:03:24.000000 pepotron-1.2.0/.github/workflows/require-pr-label.yml
+-rw-r--r--   0        0        0     1709 2024-04-24 15:03:24.000000 pepotron-1.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     5204 2024-04-24 15:03:24.000000 pepotron-1.2.0/src/pepotron/__init__.py
+-rw-r--r--   0        0        0      104 2024-04-24 15:03:24.000000 pepotron-1.2.0/src/pepotron/__main__.py
+-rw-r--r--   0        0        0     1651 2024-04-24 15:03:24.000000 pepotron-1.2.0/src/pepotron/_cache.py
+-rw-r--r--   0        0        0     2268 2024-04-24 15:03:24.000000 pepotron-1.2.0/src/pepotron/cli.py
+-rw-r--r--   0        0        0        0 2024-04-24 15:03:24.000000 pepotron-1.2.0/src/pepotron/scripts/__init__.py
+-rw-r--r--   0        0        0      613 2024-04-24 15:03:24.000000 pepotron-1.2.0/src/pepotron/scripts/run_command.py
+-rw-r--r--   0        0        0        0 2024-04-24 15:03:24.000000 pepotron-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     2899 2024-04-24 15:03:24.000000 pepotron-1.2.0/tests/test_cache.py
+-rw-r--r--   0        0        0     3158 2024-04-24 15:03:24.000000 pepotron-1.2.0/tests/test_pepotron.py
+-rw-r--r--   0        0        0     3077 2024-04-24 15:03:24.000000 pepotron-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1079 2024-04-24 15:03:24.000000 pepotron-1.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     5073 2024-04-24 15:03:24.000000 pepotron-1.2.0/README.md
+-rw-r--r--   0        0        0     2285 2024-04-24 15:03:24.000000 pepotron-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6529 2024-04-24 15:03:24.000000 pepotron-1.2.0/PKG-INFO
```

### Comparing `pepotron-1.1.1/.pre-commit-config.yaml` & `pepotron-1.2.0/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,74 @@
 repos:
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v3.14.0
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.4.1
     hooks:
-      - id: pyupgrade
-        args: [--py38-plus]
+      - id: ruff
+        args: [--exit-non-zero-on-fix]
 
   - repo: https://github.com/psf/black-pre-commit-mirror
-    rev: 23.9.1
+    rev: 24.4.0
     hooks:
       - id: black
 
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
-    hooks:
-      - id: isort
-        args: [--add-import=from __future__ import annotations]
-
-  - repo: https://github.com/PyCQA/flake8
-    rev: 6.1.0
-    hooks:
-      - id: flake8
-        additional_dependencies:
-          [flake8-2020, flake8-errmsg, flake8-implicit-str-concat, flake8-logging]
-
-  - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.10.0
-    hooks:
-      - id: python-check-blanket-noqa
-
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.6.0
     hooks:
+      - id: check-added-large-files
       - id: check-case-conflict
-      - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: check-json
       - id: check-toml
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
+      - id: forbid-submodules
       - id: trailing-whitespace
 
+  - repo: https://github.com/python-jsonschema/check-jsonschema
+    rev: 0.28.2
+    hooks:
+      - id: check-github-workflows
+      - id: check-renovate
+
+  - repo: https://github.com/rhysd/actionlint
+    rev: v1.6.27
+    hooks:
+      - id: actionlint
+
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.5.1
+    rev: v1.9.0
     hooks:
       - id: mypy
         args: [--strict, --pretty, --show-error-codes]
         additional_dependencies:
-          [
-            platformdirs,
-            pytest,
-            rapidfuzz,
-            types-freezegun,
-            types-python-slugify,
-            urllib3,
-          ]
+          [platformdirs, pytest, python-slugify, rapidfuzz, types-freezegun, urllib3]
 
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 1.2.0
+    rev: 1.8.0
     hooks:
       - id: pyproject-fmt
         additional_dependencies: [tox]
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.14
+    rev: v0.16
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/tox-dev/tox-ini-fmt
     rev: 1.3.1
     hooks:
       - id: tox-ini-fmt
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.3
+    rev: v4.0.0-alpha.8
     hooks:
       - id: prettier
         args: [--prose-wrap=always, --print-width=88]
 
+  - repo: meta
+    hooks:
+      - id: check-hooks-apply
+      - id: check-useless-excludes
+
 ci:
   autoupdate_schedule: quarterly
```

### Comparing `pepotron-1.1.1/RELEASING.md` & `pepotron-1.2.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `pepotron-1.1.1/tox.ini` & `pepotron-1.2.0/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 [tox]
 requires =
     tox>=4.2
 env_list =
+    cli
     cog
     lint
-    py{py3, 312, 311, 310, 39, 38}
+    py{py3, 313, 312, 311, 310, 39, 38}
 
 [testenv]
 extras =
     tests
 commands =
     {envpython} -m pytest \
       --cov pepotron \
       --cov tests \
       --cov-report html \
       --cov-report term \
       --cov-report xml \
       {posargs}
+
+[testenv:cli]
+commands =
     pep --version
     pep --help
+    pep --dry-run 8
+    pep --dry-run 3.13
+    pep --dry-run dead batteries
 
 [testenv:cog]
 deps =
     cogapp
 commands =
     cog -Pr README.md
```

### Comparing `pepotron-1.1.1/.github/release-drafter.yml` & `pepotron-1.2.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pepotron-1.1.1/.github/workflows/release-drafter.yml` & `pepotron-1.2.0/.github/workflows/release-drafter.yml`

 * *Files 11% similar despite different names*

```diff
@@ -25,10 +25,10 @@
       contents: write
       # write permission is required for autolabeler
       # otherwise, read permission is required at least
       pull-requests: write
     runs-on: ubuntu-latest
     steps:
       # Drafts your next release notes as pull requests are merged into "main"
-      - uses: release-drafter/release-drafter@v5
+      - uses: release-drafter/release-drafter@v6
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `pepotron-1.1.1/.github/workflows/test.yml` & `pepotron-1.2.0/.github/workflows/test.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,62 @@
 name: Test
 
 on: [push, pull_request, workflow_dispatch]
 
+permissions:
+  contents: read
+
 env:
   FORCE_COLOR: 1
+  PIP_DISABLE_PIP_VERSION_CHECK: 1
 
 jobs:
   test:
-    runs-on: ${{ matrix.os }}
+    runs-on: "${{ matrix.os }}-${{ matrix.os-version || 'latest' }}"
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["pypy3.10", "3.8", "3.9", "3.10", "3.11", "3.12"]
-        os: [windows-latest, macos-latest, ubuntu-latest]
+        python-version: ["pypy3.10", "3.8", "3.9", "3.10", "3.11", "3.12", "3.13"]
+        os: [Windows, macOS, Ubuntu]
+        # Python 3.8 and 3.9 are on macos-13 but not macos-latest (macos-14-arm64)
+        # https://github.com/actions/setup-python/issues/696#issuecomment-1637587760
+        include:
+          - { python-version: "3.8", os: "macOS", os-version: "13" }
+          - { python-version: "3.9", os: "macOS", os-version: "13" }
 
     steps:
       - uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
           allow-prereleases: true
           cache: pip
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
-          python -m pip install -U wheel
           python -m pip install -U tox
 
       - name: Tox tests
         run: |
           tox -e py
 
+      - name: Test CLI
+        run: |
+          tox -e cli
+
       - name: Cog
-        if: matrix.python-version == '3.11' && matrix.os == 'ubuntu-latest'
+        if: matrix.python-version == '3.12' && matrix.os == 'ubuntu-latest'
         run: |
           tox -e cog
 
       - name: Upload coverage
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v3.1.5
         with:
           flags: ${{ matrix.os }}
           name: ${{ matrix.os }} Python ${{ matrix.python-version }}
 
   success:
     needs: test
     runs-on: ubuntu-latest
```

### Comparing `pepotron-1.1.1/src/pepotron/__init__.py` & `pepotron-1.2.0/src/pepotron/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 CLI to open PEPs in your browser
 """
+
 from __future__ import annotations
 
 import importlib.metadata
 import logging
 from pathlib import Path
 from typing import Any
 
@@ -37,14 +38,15 @@
     "3.7": 537,
     "3.8": 569,
     "3.9": 596,
     "3.10": 619,
     "3.11": 664,
     "3.12": 693,
     "3.13": 719,
+    "3.14": 745,
 }
 
 
 def _download_peps_json(json_url: str = BASE_URL + JSON_PATH) -> Path:
     cache_file = _cache.filename(json_url)
     logging.info("Cache file: %s", cache_file)
 
@@ -89,15 +91,15 @@
 
 def _next_available_pep() -> int:
     try:
         # Python 3.10+
         from itertools import pairwise
     except ImportError:
         # Python 3.9 and below
-        def pairwise(iterable):  # type: ignore
+        def pairwise(iterable):  # type: ignore[no-redef,no-untyped-def]
             from itertools import tee
 
             a, b = tee(iterable)
             next(b, None)
             return zip(a, b)
 
     published = _get_published_peps()
@@ -114,15 +116,15 @@
             next_pep = x + 1
             break
 
     return next_pep
 
 
 def _get_github_prs() -> list[Any]:
-    from ghapi.all import GhApi  # type: ignore
+    from ghapi.all import GhApi  # type: ignore[import-not-found]
 
     api = GhApi(owner="python", repo="peps", authenticate=False)
     return api.pulls.list(per_page=100)  # type: ignore[no-any-return]
 
 
 def _get_pr_peps() -> set[int]:
     import re
```

### Comparing `pepotron-1.1.1/src/pepotron/_cache.py` & `pepotron-1.2.0/src/pepotron/_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Cache functions
 """
+
 from __future__ import annotations
 
 import datetime as dt
 import json
 import logging
 import sys
 from pathlib import Path
```

### Comparing `pepotron-1.1.1/src/pepotron/cli.py` & `pepotron-1.2.0/src/pepotron/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 pepotron: CLI to open PEPs in your browser
 """
+
 from __future__ import annotations
 
 import argparse
 import atexit
 import logging
 
 from . import BASE_URL, __version__, _cache, open_bpo, open_pep
@@ -34,15 +35,16 @@
 def main() -> None:
     parser = argparse.ArgumentParser(
         description=__doc__, formatter_class=argparse.RawDescriptionHelpFormatter
     )
     parser.add_argument(
         "search",
         nargs="*",
-        help="PEP number, or Python version for its schedule, or words from title",
+        help="PEP number, or Python version for its schedule, or words from title, "
+        "or 'next' to find next available PEP number",
     )
     parser.add_argument(
         "-u", "--url", default=BASE_URL, help=f"Base URL for PEPs (default: {BASE_URL})"
     )
     parser.add_argument("-p", "--pr", type=int, help="Open preview for python/peps PR")
     parser.add_argument(
         "--clear-cache", action="store_true", help="Clear cache before running"
```

### Comparing `pepotron-1.1.1/src/pepotron/scripts/run_command.py` & `pepotron-1.2.0/src/pepotron/scripts/run_command.py`

 * *Files identical despite different names*

### Comparing `pepotron-1.1.1/tests/test_cache.py` & `pepotron-1.2.0/tests/test_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Unit tests for _cache
 """
+
 from __future__ import annotations
 
 import tempfile
 from pathlib import Path
 
 from freezegun import freeze_time
```

### Comparing `pepotron-1.1.1/tests/test_pepotron.py` & `pepotron-1.2.0/tests/test_pepotron.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Unit tests
 """
+
 from __future__ import annotations
 
 from collections import namedtuple
 
 import pytest
 
 import pepotron
@@ -104,15 +105,15 @@
     filename = pepotron._download_peps_json()
     # Assert
     assert filename.suffix == ".json"
 
 
 def test__download_peps_json_error() -> None:
     with pytest.raises(RuntimeError):
-        pepotron._download_peps_json("https://httpstat.us/404")
+        pepotron._download_peps_json("https://httpbin.org/status/404")
 
 
 def test_pep() -> None:
     url = pepotron.open_pep("8", dry_run=True)
     assert url == "https://peps.python.org/pep-0008/"
```

### Comparing `pepotron-1.1.1/.gitignore` & `pepotron-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pepotron-1.1.1/LICENSE.txt` & `pepotron-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pepotron-1.1.1/README.md` & `pepotron-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pepotron-1.1.1/pyproject.toml` & `pepotron-1.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,15 @@
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
+  "Programming Language :: Python :: 3.13",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
@@ -58,12 +59,38 @@
 
 [tool.hatch]
 version.source = "vcs"
 
 [tool.hatch.version.raw-options]
 local_scheme = "no-local-version"
 
-[tool.isort]
-profile = "black"
+[tool.ruff]
+fix = true
+
+[tool.ruff.lint]
+select = [
+  "C4", # flake8-comprehensions
+  "E", # pycodestyle errors
+  "EM", # flake8-errmsg
+  "F", # pyflakes errors
+  "I", # isort
+  "ISC", # flake8-implicit-str-concat
+  "LOG", # flake8-logging
+  "PGH", # pygrep-hooks
+  "RUF100", # unused noqa (yesqa)
+  "UP", # pyupgrade
+  "W", # pycodestyle warnings
+  "YTT", # flake8-2020
+]
+extend-ignore = [
+  "E203", # Whitespace before ':'
+  "E221", # Multiple spaces before operator
+  "E226", # Missing whitespace around arithmetic operator
+  "E241", # Multiple spaces after ','
+]
+
+[tool.ruff.lint.isort]
+known-first-party = ["pepotron"]
+required-imports = ["from __future__ import annotations"]
 
 [tool.pytest.ini_options]
 addopts = "--color=yes"
```

### Comparing `pepotron-1.1.1/PKG-INFO` & `pepotron-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pepotron
-Version: 1.1.1
+Version: 1.2.0
 Summary: CLI to open PEPs in your browser
 Project-URL: Changelog, https://github.com/hugovk/pepotron/releases
 Project-URL: Homepage, https://github.com/hugovk/pepotron
 Project-URL: Source, https://github.com/hugovk/pepotron
 Author: Hugo van Kemenade
 License: MIT
 License-File: LICENSE.txt
@@ -16,14 +16,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: ghapi
 Requires-Dist: platformdirs
 Requires-Dist: python-slugify
 Requires-Dist: rapidfuzz
```

