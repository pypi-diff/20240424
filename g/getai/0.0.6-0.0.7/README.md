# Comparing `tmp/getai-0.0.6.tar.gz` & `tmp/getai-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getai-0.0.6.tar", max compression
+gzip compressed data, was "getai-0.0.7.tar", max compression
```

## Comparing `getai-0.0.6.tar` & `getai-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1247 2024-04-23 11:42:53.993269 getai-0.0.6/LICENSE
--rw-r--r--   0        0        0     8542 2024-04-23 11:36:27.654734 getai-0.0.6/README.md
--rw-r--r--   0        0        0        0 2024-04-23 11:20:21.512462 getai-0.0.6/getai/__init__.py
--rw-r--r--   0        0        0      133 2024-04-23 11:20:21.512462 getai-0.0.6/getai/__main__.py
--rw-r--r--   0        0        0    13580 2024-04-23 21:26:46.319887 getai-0.0.6/getai/dataset_downloader.py
--rw-r--r--   0        0        0       37 2024-04-23 11:20:21.512462 getai-0.0.6/getai/getai_config.yaml
--rw-r--r--   0        0        0     7471 2024-04-24 09:51:09.949507 getai-0.0.6/getai/main.py
--rw-r--r--   0        0        0    28922 2024-04-24 10:55:00.450309 getai-0.0.6/getai/model_downloader.py
--rw-r--r--   0        0        0     3088 2024-04-24 09:51:09.949507 getai-0.0.6/getai/utils.py
--rw-r--r--   0        0        0      740 2024-04-24 10:55:37.034764 getai-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     9357 1970-01-01 00:00:00.000000 getai-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1247 2024-04-23 11:42:53.993269 getai-0.0.7/LICENSE
+-rw-r--r--   0        0        0     8542 2024-04-23 11:36:27.654734 getai-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 11:20:21.512462 getai-0.0.7/getai/__init__.py
+-rw-r--r--   0        0        0      133 2024-04-23 11:20:21.512462 getai-0.0.7/getai/__main__.py
+-rw-r--r--   0        0        0    13580 2024-04-23 21:26:46.319887 getai-0.0.7/getai/dataset_downloader.py
+-rw-r--r--   0        0        0       37 2024-04-23 11:20:21.512462 getai-0.0.7/getai/getai_config.yaml
+-rw-r--r--   0        0        0     7471 2024-04-24 09:51:09.949507 getai-0.0.7/getai/main.py
+-rw-r--r--   0        0        0    28896 2024-04-24 11:00:39.252499 getai-0.0.7/getai/model_downloader.py
+-rw-r--r--   0        0        0     3088 2024-04-24 09:51:09.949507 getai-0.0.7/getai/utils.py
+-rw-r--r--   0        0        0      739 2024-04-24 11:02:21.335753 getai-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     9457 1970-01-01 00:00:00.000000 getai-0.0.7/PKG-INFO
```

### Comparing `getai-0.0.6/LICENSE` & `getai-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `getai-0.0.6/README.md` & `getai-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `getai-0.0.6/getai/dataset_downloader.py` & `getai-0.0.7/getai/dataset_downloader.py`

 * *Files identical despite different names*

### Comparing `getai-0.0.6/getai/main.py` & `getai-0.0.7/getai/main.py`

 * *Files identical despite different names*

### Comparing `getai-0.0.6/getai/model_downloader.py` & `getai-0.0.7/getai/model_downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 import datetime
 import hashlib
 import json
 import logging
 import re
 from pathlib import Path
 from typing import Optional, Union, Dict, BinaryIO
-import os
-import requests
 
 import aiofiles
 import aiohttp
 from aiofiles import open as aio_open
 
 from aiohttp import ClientSession, TCPConnector
 from prompt_toolkit import PromptSession
```

### Comparing `getai-0.0.6/getai/utils.py` & `getai-0.0.7/getai/utils.py`

 * *Files identical despite different names*

### Comparing `getai-0.0.6/pyproject.toml` & `getai-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "getai"
-version = "0.0.6"
+version = "0.0.7"
 description = "GetAI - An asynchronous AI search and download tool for AI models, datasets, and tools. Designed to streamline the process of downloading machine learning models, datasets, and more."
 authors = ["Ben Gorlick <ben@unifiedlearning.ai>"]
 license = "MIT - with attribution"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.9"
 aiohttp = "^3.9.3"
 aiofiles = "^23.2.1"
 prompt-toolkit = "^3.0.43"
 rainbow-tqdm = "^0.1.3"
 PyYAML = "^6.0.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `getai-0.0.6/PKG-INFO` & `getai-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: getai
-Version: 0.0.6
+Version: 0.0.7
 Summary: GetAI - An asynchronous AI search and download tool for AI models, datasets, and tools. Designed to streamline the process of downloading machine learning models, datasets, and more.
 License: MIT - with attribution
 Author: Ben Gorlick
 Author-email: ben@unifiedlearning.ai
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: prompt-toolkit (>=3.0.43,<4.0.0)
 Requires-Dist: rainbow-tqdm (>=0.1.3,<0.2.0)
```

