# Comparing `tmp/stac-asset-0.2.4.tar.gz` & `tmp/stac_asset-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-asset-0.2.4.tar", last modified: Tue Apr  2 18:37:36 2024, max compression
+gzip compressed data, was "stac_asset-0.3.0.tar", last modified: Wed Apr 24 13:06:45 2024, max compression
```

## Comparing `stac-asset-0.2.4.tar` & `stac_asset-0.3.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:37:36.578661 stac-asset-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 18:37:27.000000 stac-asset-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 18:37:27.000000 stac-asset-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-02 18:37:27.000000 stac-asset-0.2.4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     8345 2024-04-02 18:37:36.578661 stac-asset-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-02 18:37:27.000000 stac-asset-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-02 18:37:27.000000 stac-asset-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 18:37:36.578661 stac-asset-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:37:36.570661 stac-asset-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:37:36.574661 stac-asset-0.2.4/src/stac_asset/
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15367 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    18913 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/blocking.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/earthdata_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/filesystem_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/planetary_computer_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/s3_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-02 18:37:27.000000 stac-asset-0.2.4/src/stac_asset/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:37:36.574661 stac-asset-0.2.4/src/stac_asset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8345 2024-04-02 18:37:36.000000 stac-asset-0.2.4/src/stac_asset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-02 18:37:36.000000 stac-asset-0.2.4/src/stac_asset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:37:36.000000 stac-asset-0.2.4/src/stac_asset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-02 18:37:36.000000 stac-asset-0.2.4/src/stac_asset.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-02 18:37:36.000000 stac-asset-0.2.4/src/stac_asset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 18:37:36.000000 stac-asset-0.2.4/src/stac_asset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:37:36.574661 stac-asset-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-02 18:37:27.000000 stac-asset-0.2.4/tests/test_blocking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-02 18:37:27.000000 stac-asset-0.2.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-02 18:37:27.000000 stac-asset-0.2.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-02 18:37:27.000000 stac-asset-0.2.4/tests/test_earthdata_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-02 18:37:27.000000 stac-asset-0.2.4/tests/test_filesystem_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-04-02 18:37:27.000000 stac-asset-0.2.4/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-02 18:37:27.000000 stac-asset-0.2.4/tests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-02 18:37:27.000000 stac-asset-0.2.4/tests/test_planetary_computer_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-02 18:37:27.000000 stac-asset-0.2.4/tests/test_s3_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 18:37:27.000000 stac-asset-0.2.4/tests/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:06:45.243191 stac_asset-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 13:06:37.000000 stac_asset-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-24 13:06:37.000000 stac_asset-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-24 13:06:37.000000 stac_asset-0.3.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-04-24 13:06:45.243191 stac_asset-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-24 13:06:37.000000 stac_asset-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-24 13:06:37.000000 stac_asset-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:06:45.243191 stac_asset-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:06:45.235191 stac_asset-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:06:45.239191 stac_asset-0.3.0/src/stac_asset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15367 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18954 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/earthdata_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/filesystem_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/planetary_computer_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-24 13:06:37.000000 stac_asset-0.3.0/src/stac_asset/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:06:45.239191 stac_asset-0.3.0/src/stac_asset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-04-24 13:06:45.000000 stac_asset-0.3.0/src/stac_asset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-24 13:06:45.000000 stac_asset-0.3.0/src/stac_asset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:06:45.000000 stac_asset-0.3.0/src/stac_asset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 13:06:45.000000 stac_asset-0.3.0/src/stac_asset.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-24 13:06:45.000000 stac_asset-0.3.0/src/stac_asset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 13:06:45.000000 stac_asset-0.3.0/src/stac_asset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:06:45.239191 stac_asset-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-24 13:06:37.000000 stac_asset-0.3.0/tests/test_blocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-24 13:06:37.000000 stac_asset-0.3.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-24 13:06:37.000000 stac_asset-0.3.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-24 13:06:37.000000 stac_asset-0.3.0/tests/test_earthdata_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-24 13:06:37.000000 stac_asset-0.3.0/tests/test_filesystem_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-04-24 13:06:37.000000 stac_asset-0.3.0/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-24 13:06:37.000000 stac_asset-0.3.0/tests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-24 13:06:37.000000 stac_asset-0.3.0/tests/test_planetary_computer_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-24 13:06:37.000000 stac_asset-0.3.0/tests/test_s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-24 13:06:37.000000 stac_asset-0.3.0/tests/test_validate.py
```

### Comparing `stac-asset-0.2.4/LICENSE` & `stac_asset-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.4/NOTICE` & `stac_asset-0.3.0/NOTICE`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.4/PKG-INFO` & `stac_asset-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: stac-asset
-Version: 0.2.4
+Version: 0.3.0
 Summary: Read and download STAC assets across platforms and providers
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: Github, https://github.com/stac-utils/stac-asset
 Project-URL: CHANGELOG, https://github.com/stac-utils/stac-asset/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/stac-utils/stac-asset/issues
 Keywords: stac,async
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: aiofiles>=23.1.0
 Requires-Dist: aiobotocore>=2.5.0
 Requires-Dist: aiohttp>=3.8.4
 Requires-Dist: pystac>=1.8.4
@@ -34,22 +33,22 @@
 Provides-Extra: dev
 Requires-Dist: mypy~=1.3; extra == "dev"
 Requires-Dist: pre-commit~=3.3; extra == "dev"
 Requires-Dist: pystac[validation]>=1.8.4; extra == "dev"
 Requires-Dist: pytest~=7.3; extra == "dev"
 Requires-Dist: pytest-asyncio~=0.21; extra == "dev"
 Requires-Dist: pytest-cov>=5.0; extra == "dev"
-Requires-Dist: ruff==0.3.4; extra == "dev"
+Requires-Dist: ruff==0.4.1; extra == "dev"
 Requires-Dist: types-aiofiles~=23.1; extra == "dev"
 Requires-Dist: types-python-dateutil~=2.9; extra == "dev"
 Requires-Dist: types-tqdm~=4.66.0; extra == "dev"
 Requires-Dist: types-tabulate~=0.9.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: pydata-sphinx-theme~=0.13; extra == "docs"
-Requires-Dist: sphinx~=7.2.2; extra == "docs"
+Requires-Dist: sphinx~=7.3; extra == "docs"
 Requires-Dist: sphinx-click~=5.0; extra == "docs"
 
 # stac-asset
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/stac-utils/stac-asset/ci.yaml?style=for-the-badge)](https://github.com/stac-utils/stac-asset/actions/workflows/ci.yaml)
 [![Read the Docs](https://img.shields.io/readthedocs/stac-asset?style=for-the-badge)](https://stac-asset.readthedocs.io/en/stable/)
 [![PyPI](https://img.shields.io/pypi/v/stac-asset?style=for-the-badge)](https://pypi.org/project/stac-asset)
```

### Comparing `stac-asset-0.2.4/README.md` & `stac_asset-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.4/pyproject.toml` & `stac_asset-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 [project]
 name = "stac-asset"
-version = "0.2.4"
+version = "0.3.0"
 description = "Read and download STAC assets across platforms and providers"
 authors = [{ name = "Pete Gadomski", email = "pete.gadomski@gmail.com" }]
 readme = "README.md"
 keywords = ["stac", "async"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Development Status :: 4 - Beta",
 ]
 license = { text = "Apache-2.0" }
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 dependencies = [
     "aiofiles>=23.1.0",
     "aiobotocore>=2.5.0",
     "aiohttp>=3.8.4",
     "pystac>=1.8.4",
     "python-dateutil>=2.7.0",
     "yarl>=1.9.2",
@@ -36,21 +35,21 @@
 dev = [
     "mypy~=1.3",
     "pre-commit~=3.3",
     "pystac[validation]>=1.8.4",
     "pytest~=7.3",
     "pytest-asyncio~=0.21",
     "pytest-cov>=5.0",
-    "ruff==0.3.4",
+    "ruff==0.4.1",
     "types-aiofiles~=23.1",
     "types-python-dateutil~=2.9",
     "types-tqdm~=4.66.0",
     "types-tabulate~=0.9.0",
 ]
-docs = ["pydata-sphinx-theme~=0.13", "sphinx~=7.2.2", "sphinx-click~=5.0"]
+docs = ["pydata-sphinx-theme~=0.13", "sphinx~=7.3", "sphinx-click~=5.0"]
 
 [project.scripts]
 stac-asset = "stac_asset._cli:cli"
 
 [project.urls]
 Github = "https://github.com/stac-utils/stac-asset"
 CHANGELOG = "https://github.com/stac-utils/stac-asset/blob/main/CHANGELOG.md"
```

### Comparing `stac-asset-0.2.4/src/stac_asset/__init__.py` & `stac_asset-0.3.0/src/stac_asset/__init__.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.4/src/stac_asset/_cli.py` & `stac_asset-0.3.0/src/stac_asset/_cli.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.4/src/stac_asset/_functions.py` & `stac_asset-0.3.0/src/stac_asset/_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import asyncio
 import json
 import os.path
 import warnings
-from asyncio import Queue, Task
+from asyncio import Task
 from dataclasses import dataclass
 from pathlib import Path
 from types import TracebackType
 from typing import (
     AsyncIterator,
     List,
     Optional,
@@ -23,15 +23,14 @@
 
 from .client import Client, Clients
 from .config import Config
 from .errors import AssetOverwriteError, DownloadError, DownloadWarning
 from .messages import (
     ErrorAssetDownload,
     FinishAssetDownload,
-    Message,
     SkipAssetDownload,
     StartAssetDownload,
 )
 from .strategy import ErrorStrategy, FileNameStrategy
 from .types import MessageQueue, PathLikeObject
 
 
@@ -234,14 +233,15 @@
         await downloads.add(item, Path(directory), file_name, keep_non_downloaded)
         await downloads.download(messages)
 
     self_href = item.get_self_href()
     if self_href:
         make_asset_hrefs_relative(item)
         d = item.to_dict(include_self_link=True, transform_hrefs=False)
+        os.makedirs(os.path.dirname(self_href), exist_ok=True)
         with open(self_href, "w") as f:
             json.dump(d, f)
 
     return item
 
 
 async def download_collection(
@@ -336,15 +336,15 @@
 
 
 async def download_asset(
     key: str,
     asset: Asset,
     path: Path,
     config: Config,
-    messages: Optional[Queue[Message]] = None,
+    messages: Optional[MessageQueue] = None,
     clients: Optional[Clients] = None,
 ) -> Asset:
     """Downloads an asset.
 
     Args:
         key: The asset key
         asset: The asset
```

### Comparing `stac-asset-0.2.4/src/stac_asset/blocking.py` & `stac_asset-0.3.0/src/stac_asset/blocking.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.4/src/stac_asset/client.py` & `stac_asset-0.3.0/src/stac_asset/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from asyncio import Lock, Queue, QueueFull
+from asyncio import Lock, QueueFull
 from pathlib import Path
 from types import TracebackType
 from typing import AsyncIterator, Dict, List, Optional, Type, TypeVar
 
 import aiofiles
 from yarl import URL
 
 from .config import Config
 from .messages import (
-    Message,
     WriteChunk,
 )
-from .types import PathLikeObject
+from .types import MessageQueue, PathLikeObject
 
 T = TypeVar("T", bound="Client")
 
 
 class Client(ABC):
     """An abstract base class for all clients."""
 
@@ -37,15 +36,15 @@
         pass
 
     @abstractmethod
     async def open_url(
         self,
         url: URL,
         content_type: Optional[str] = None,
-        messages: Optional[Queue[Message]] = None,
+        messages: Optional[MessageQueue] = None,
     ) -> AsyncIterator[bytes]:
         """Opens a url and yields an iterator over its bytes.
 
         This is the core method that all clients must implement.
 
         Args:
             url: The input url
@@ -60,15 +59,15 @@
         if False:  # pragma: no cover
             yield
 
     async def open_href(
         self,
         href: str,
         content_type: Optional[str] = None,
-        messages: Optional[Queue[Message]] = None,
+        messages: Optional[MessageQueue] = None,
     ) -> AsyncIterator[bytes]:
         """Opens a href and yields an iterator over its bytes.
 
         Args:
             href: The input href
             content_type: The expected content type
             messages: An optional queue to use for progress reporting
@@ -83,15 +82,15 @@
 
     async def download_href(
         self,
         href: str,
         path: PathLikeObject,
         clean: bool = True,
         content_type: Optional[str] = None,
-        messages: Optional[Queue[Message]] = None,
+        messages: Optional[MessageQueue] = None,
     ) -> None:
         """Downloads a file to the local filesystem.
 
         Args:
             href: The input href
             path: The output file path
             clean: If an error occurs, delete the output file if it exists
```

### Comparing `stac-asset-0.2.4/src/stac_asset/config.py` & `stac_asset-0.3.0/src/stac_asset/config.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.4/src/stac_asset/earthdata_client.py` & `stac_asset-0.3.0/src/stac_asset/earthdata_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.4/src/stac_asset/errors.py` & `stac_asset-0.3.0/src/stac_asset/errors.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.4/src/stac_asset/filesystem_client.py` & `stac_asset-0.3.0/src/stac_asset/filesystem_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from __future__ import annotations
 
 import os.path
-from asyncio import Queue
 from types import TracebackType
 from typing import AsyncIterator, Optional, Type
 
 import aiofiles
 from yarl import URL
 
 from .client import Client
-from .messages import Message, OpenUrl
+from .messages import OpenUrl
+from .types import MessageQueue
 
 
 class FilesystemClient(Client):
     """A simple client for moving files around on the filesystem.
 
     Mostly used for testing, but could be useful in some real-world cases.
     """
 
     async def open_url(
         self,
         url: URL,
         content_type: Optional[str] = None,
-        messages: Optional[Queue[Message]] = None,
+        messages: Optional[MessageQueue] = None,
     ) -> AsyncIterator[bytes]:
         """Iterates over data from a local url.
 
         Args:
             url: The url to read bytes from
             content_type: The expected content type. Ignored by this client,
                 because filesystems don't have content types.
```

### Comparing `stac-asset-0.2.4/src/stac_asset/http_client.py` & `stac_asset-0.3.0/src/stac_asset/http_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
-from asyncio import Queue
 from types import TracebackType
 from typing import AsyncIterator, Optional, Type, TypeVar
 
 from aiohttp import ClientSession
 from yarl import URL
 
 from . import validate
 from .client import Client
 from .config import Config
-from .messages import Message, OpenUrl
+from .messages import OpenUrl
+from .types import MessageQueue
 
 T = TypeVar("T", bound="HttpClient")
 
 
 class HttpClient(Client):
     """A simple client for making HTTP requests.
 
@@ -44,15 +44,15 @@
         self.session = session
         self.check_content_type = check_content_type
 
     async def open_url(
         self,
         url: URL,
         content_type: Optional[str] = None,
-        messages: Optional[Queue[Message]] = None,
+        messages: Optional[MessageQueue] = None,
     ) -> AsyncIterator[bytes]:
         """Opens a url with this client's session and iterates over its bytes.
 
         Args:
             url: The url to open
             content_type: The expected content type
             messages: An optional queue to use for progress reporting
```

### Comparing `stac-asset-0.2.4/src/stac_asset/messages.py` & `stac_asset-0.3.0/src/stac_asset/messages.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.4/src/stac_asset/planetary_computer_client.py` & `stac_asset-0.3.0/src/stac_asset/planetary_computer_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.4/src/stac_asset/s3_client.py` & `stac_asset-0.3.0/src/stac_asset/s3_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-from asyncio import Queue
 from types import TracebackType
 from typing import Any, AsyncIterator, Dict, Optional, Type
 
 import aiobotocore.session
 import botocore.config
 from aiobotocore.session import AioSession, ClientCreatorContext
 from botocore import UNSIGNED
@@ -14,15 +13,16 @@
 from .client import Client
 from .config import (
     DEFAULT_S3_MAX_ATTEMPTS,
     DEFAULT_S3_REGION_NAME,
     DEFAULT_S3_RETRY_MODE,
     Config,
 )
-from .messages import Message, OpenUrl
+from .messages import OpenUrl
+from .types import MessageQueue
 
 
 class S3Client(Client):
     """A client for interacting with s3 urls.
 
     To use the ``requester_pays`` option, you need to configure your AWS
     credentials. See `the AWS documentation
@@ -82,15 +82,15 @@
         self.retry_mode = retry_mode
         self.max_attempts = max_attempts
 
     async def open_url(
         self,
         url: URL,
         content_type: Optional[str] = None,
-        messages: Optional[Queue[Message]] = None,
+        messages: Optional[MessageQueue] = None,
     ) -> AsyncIterator[bytes]:
         """Opens an s3 url and iterates over its bytes.
 
         Args:
             url: The url to open
             content_type: The expected content type
             messages: An optional queue to use for progress reporting
```

### Comparing `stac-asset-0.2.4/src/stac_asset/strategy.py` & `stac_asset-0.3.0/src/stac_asset/strategy.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.4/src/stac_asset/validate.py` & `stac_asset-0.3.0/src/stac_asset/validate.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.4/src/stac_asset.egg-info/PKG-INFO` & `stac_asset-0.3.0/src/stac_asset.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: stac-asset
-Version: 0.2.4
+Version: 0.3.0
 Summary: Read and download STAC assets across platforms and providers
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: Github, https://github.com/stac-utils/stac-asset
 Project-URL: CHANGELOG, https://github.com/stac-utils/stac-asset/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/stac-utils/stac-asset/issues
 Keywords: stac,async
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: aiofiles>=23.1.0
 Requires-Dist: aiobotocore>=2.5.0
 Requires-Dist: aiohttp>=3.8.4
 Requires-Dist: pystac>=1.8.4
@@ -34,22 +33,22 @@
 Provides-Extra: dev
 Requires-Dist: mypy~=1.3; extra == "dev"
 Requires-Dist: pre-commit~=3.3; extra == "dev"
 Requires-Dist: pystac[validation]>=1.8.4; extra == "dev"
 Requires-Dist: pytest~=7.3; extra == "dev"
 Requires-Dist: pytest-asyncio~=0.21; extra == "dev"
 Requires-Dist: pytest-cov>=5.0; extra == "dev"
-Requires-Dist: ruff==0.3.4; extra == "dev"
+Requires-Dist: ruff==0.4.1; extra == "dev"
 Requires-Dist: types-aiofiles~=23.1; extra == "dev"
 Requires-Dist: types-python-dateutil~=2.9; extra == "dev"
 Requires-Dist: types-tqdm~=4.66.0; extra == "dev"
 Requires-Dist: types-tabulate~=0.9.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: pydata-sphinx-theme~=0.13; extra == "docs"
-Requires-Dist: sphinx~=7.2.2; extra == "docs"
+Requires-Dist: sphinx~=7.3; extra == "docs"
 Requires-Dist: sphinx-click~=5.0; extra == "docs"
 
 # stac-asset
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/stac-utils/stac-asset/ci.yaml?style=for-the-badge)](https://github.com/stac-utils/stac-asset/actions/workflows/ci.yaml)
 [![Read the Docs](https://img.shields.io/readthedocs/stac-asset?style=for-the-badge)](https://stac-asset.readthedocs.io/en/stable/)
 [![PyPI](https://img.shields.io/pypi/v/stac-asset?style=for-the-badge)](https://pypi.org/project/stac-asset)
```

### Comparing `stac-asset-0.2.4/src/stac_asset.egg-info/SOURCES.txt` & `stac_asset-0.3.0/src/stac_asset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.4/tests/test_blocking.py` & `stac_asset-0.3.0/tests/test_blocking.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.4/tests/test_cli.py` & `stac_asset-0.3.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.4/tests/test_earthdata_client.py` & `stac_asset-0.3.0/tests/test_earthdata_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.4/tests/test_filesystem_client.py` & `stac_asset-0.3.0/tests/test_filesystem_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.4/tests/test_functions.py` & `stac_asset-0.3.0/tests/test_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     AssetOverwriteError,
     Config,
     ConfigError,
     DownloadError,
     DownloadWarning,
     ErrorStrategy,
     FileNameStrategy,
-    Message,
     S3Client,
 )
+from stac_asset.types import MessageQueue
 
 pytestmark = [
     pytest.mark.asyncio,
 ]
 
 
 async def test_download_item(tmp_path: Path, item: Item) -> None:
@@ -70,14 +70,26 @@
             item,
             tmp_path,
             config=Config(error_strategy=ErrorStrategy.DELETE, warn=True),
         )
     assert "does-not-exist" not in item.assets
 
 
+async def test_download_nonexistent_asset(tmp_path: Path, item: Item) -> None:
+    # this previously had a bug where the code assumed the directory had
+    # been created by downloading the assets when trying to write the item json,
+    # but it hadn't, so a failure occurred
+    await stac_asset.download_item(
+        item,
+        tmp_path / "dir-that-doesnt-exist",
+        file_name="item.json",
+        config=Config(include=["non-existent-asset"]),
+    )
+
+
 async def test_download_missing_asset_fail_fast(tmp_path: Path, item: Item) -> None:
     item.assets["does-not-exist"] = Asset("not-a-file.md5")
     with pytest.raises(FileNotFoundError):
         await stac_asset.download_item(
             item,
             tmp_path,
             config=Config(fail_fast=True),
@@ -191,15 +203,15 @@
         href="s3://usgs-landsat/collection02/level-2/standard/oli-tirs/2023/092/068/LC09_L2SP_092068_20230522_20230524_02_T2/LC09_L2SP_092068_20230522_20230524_02_T2_thumb_small.jpeg",
     )
     s3_client = S3Client(requester_pays=True)
     item = await stac_asset.download_item(item, tmp_path, clients=[s3_client])
 
 
 async def test_queue(tmp_path: Path, item: Item) -> None:
-    messages: Queue[Message] = Queue()
+    messages: MessageQueue = Queue()
     item = await stac_asset.download_item(item, tmp_path, messages=messages)
     assert not messages.empty()
 
 
 async def test_asset_exists(item: Item) -> None:
     assert await stac_asset.asset_exists(item.assets["data"])
     assert not await stac_asset.asset_exists(Asset(href="not-a-file"))
```

### Comparing `stac-asset-0.2.4/tests/test_planetary_computer_client.py` & `stac_asset-0.3.0/tests/test_planetary_computer_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.4/tests/test_s3_client.py` & `stac_asset-0.3.0/tests/test_s3_client.py`

 * *Files identical despite different names*

### Comparing `stac-asset-0.2.4/tests/test_validate.py` & `stac_asset-0.3.0/tests/test_validate.py`

 * *Files identical despite different names*

