# Comparing `tmp/awsiot_credentialhelper-0.6.0.tar.gz` & `tmp/awsiot_credentialhelper-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsiot_credentialhelper-0.6.0.tar", max compression
+gzip compressed data, was "awsiot_credentialhelper-0.7.0.tar", max compression
```

## Comparing `awsiot_credentialhelper-0.6.0.tar` & `awsiot_credentialhelper-0.7.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     9764 2023-11-22 19:50:59.506018 awsiot_credentialhelper-0.6.0/LICENSE
--rw-r--r--   0        0        0     5207 2023-11-22 19:50:59.506018 awsiot_credentialhelper-0.6.0/README.md
--rw-r--r--   0        0        0     2821 2023-11-22 19:51:08.954009 awsiot_credentialhelper-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      433 2023-11-22 19:50:59.510018 awsiot_credentialhelper-0.6.0/src/awsiot_credentialhelper/__init__.py
--rw-r--r--   0        0        0    22197 2023-11-22 19:50:59.510018 awsiot_credentialhelper-0.6.0/src/awsiot_credentialhelper/boto3_session.py
--rw-r--r--   0        0        0        0 2023-11-22 19:50:59.510018 awsiot_credentialhelper-0.6.0/src/awsiot_credentialhelper/py.typed
--rw-r--r--   0        0        0     6489 1970-01-01 00:00:00.000000 awsiot_credentialhelper-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     9764 2024-04-24 18:30:34.463760 awsiot_credentialhelper-0.7.0/LICENSE
+-rw-r--r--   0        0        0     5207 2024-04-24 18:30:34.463760 awsiot_credentialhelper-0.7.0/README.md
+-rw-r--r--   0        0        0     2824 2024-04-24 18:30:49.119794 awsiot_credentialhelper-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      433 2024-04-24 18:30:34.463760 awsiot_credentialhelper-0.7.0/src/awsiot_credentialhelper/__init__.py
+-rw-r--r--   0        0        0    22198 2024-04-24 18:30:34.467760 awsiot_credentialhelper-0.7.0/src/awsiot_credentialhelper/boto3_session.py
+-rw-r--r--   0        0        0        0 2024-04-24 18:30:34.467760 awsiot_credentialhelper-0.7.0/src/awsiot_credentialhelper/py.typed
+-rw-r--r--   0        0        0     6435 1970-01-01 00:00:00.000000 awsiot_credentialhelper-0.7.0/PKG-INFO
```

### Comparing `awsiot_credentialhelper-0.6.0/LICENSE` & `awsiot_credentialhelper-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `awsiot_credentialhelper-0.6.0/README.md` & `awsiot_credentialhelper-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `awsiot_credentialhelper-0.6.0/pyproject.toml` & `awsiot_credentialhelper-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 [tool.poetry]
 name = "awsiot-credentialhelper"
-version = "0.6.0"
+version = "0.7.0"
 description = "AWS IoT Core Credential Provider Session Helper"
 authors = ["Gavin Adams <gavinaws@amazon.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/awslabs/aws-iot-core-credential-provider-session-helper"
 repository = "https://github.com/awslabs/aws-iot-core-credential-provider-session-helper"
 documentation = "https://aws-iot-core-credential-provider-session-helper.readthedocs.io"
@@ -14,28 +14,28 @@
     "Development Status :: 4 - Beta",
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/awslabs/aws-iot-core-credential-provider-session-helper/releases"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.8.1"
 boto3 = "^1.20.27"
 botocore = "^1.23.27"
-awscrt = "^0.16.9"
+awscrt = ">=0.16.9"
 typing-extensions = "^4.5.0"
 # workaround for: https://github.com/python-poetry/poetry-plugin-export/issues/183
 urllib3 = ">=1.25.4,<1.27"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
-flake8 = ">=4.0.1"
+flake8 = ">=6.0.0"
 flake8-bandit = ">=2.1.2"
 flake8-bugbear = ">=21.9.2"
 flake8-docstrings = ">=1.6.0"
 flake8-rst-docstrings = ">=0.2.5"
 furo = ">=2021.11.12"
 isort = ">=5.10.1"
 mypy = ">=0.930"
```

### Comparing `awsiot_credentialhelper-0.6.0/src/awsiot_credentialhelper/boto3_session.py` & `awsiot_credentialhelper-0.7.0/src/awsiot_credentialhelper/boto3_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Session object classes and methods.
 
 Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 SPDX-License-Identifier: Apache-2.0
 """
+
 from __future__ import annotations
 
 import json
 import logging
 from pathlib import Path
 from typing import TypedDict
 from typing import cast
```

### Comparing `awsiot_credentialhelper-0.6.0/PKG-INFO` & `awsiot_credentialhelper-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: awsiot-credentialhelper
-Version: 0.6.0
+Version: 0.7.0
 Summary: AWS IoT Core Credential Provider Session Helper
 Home-page: https://github.com/awslabs/aws-iot-core-credential-provider-session-helper
 License: Apache-2.0
 Author: Gavin Adams
 Author-email: gavinaws@amazon.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: awscrt (>=0.16.9,<0.17.0)
+Requires-Dist: awscrt (>=0.16.9)
 Requires-Dist: boto3 (>=1.20.27,<2.0.0)
 Requires-Dist: botocore (>=1.23.27,<2.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Requires-Dist: urllib3 (>=1.25.4,<1.27)
 Project-URL: Changelog, https://github.com/awslabs/aws-iot-core-credential-provider-session-helper/releases
 Project-URL: Documentation, https://aws-iot-core-credential-provider-session-helper.readthedocs.io
 Project-URL: Repository, https://github.com/awslabs/aws-iot-core-credential-provider-session-helper
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1 Name: awsiot-credentialhelper Version: 0.6.0 Summary: AWS
+Metadata-Version: 2.1 Name: awsiot-credentialhelper Version: 0.7.0 Summary: AWS
 IoT Core Credential Provider Session Helper Home-page: https://github.com/
 awslabs/aws-iot-core-credential-provider-session-helper License: Apache-2.0
 Author: Gavin Adams Author-email: gavinaws@amazon.com Requires-Python:
->=3.8,<4.0 Classifier: Development Status :: 4 - Beta Classifier: License ::
-OSI Approved :: Apache Software License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Requires-Dist: awscrt (>=0.16.9,<0.17.0)
-Requires-Dist: boto3 (>=1.20.27,<2.0.0) Requires-Dist: botocore
-(>=1.23.27,<2.0.0) Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) Requires-
-Dist: urllib3 (>=1.25.4,<1.27) Project-URL: Changelog, https://github.com/
-awslabs/aws-iot-core-credential-provider-session-helper/releases Project-URL:
-Documentation, https://aws-iot-core-credential-provider-session-
+>=3.8.1,<4.0.0 Classifier: Development Status :: 4 - Beta Classifier: License
+:: OSI Approved :: Apache Software License Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
+Dist: awscrt (>=0.16.9) Requires-Dist: boto3 (>=1.20.27,<2.0.0) Requires-Dist:
+botocore (>=1.23.27,<2.0.0) Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
+Requires-Dist: urllib3 (>=1.25.4,<1.27) Project-URL: Changelog, https://
+github.com/awslabs/aws-iot-core-credential-provider-session-helper/releases
+Project-URL: Documentation, https://aws-iot-core-credential-provider-session-
 helper.readthedocs.io Project-URL: Repository, https://github.com/awslabs/aws-
 iot-core-credential-provider-session-helper Description-Content-Type: text/
 markdown # AWS IoT Core Credential Provider Session Helper [![PyPI](https://
 img.shields.io/pypi/v/awsiot-credentialhelper.svg)][pypi status] [![Status]
 (https://img.shields.io/pypi/status/awsiot-credentialhelper.svg)][pypi status]
 [![Python Version](https://img.shields.io/pypi/pyversions/awsiot-
 credentialhelper)][pypi status] [![License](https://img.shields.io/pypi/l/
```

