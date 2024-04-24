# Comparing `tmp/latch_cloud_clients-0.1.2.tar.gz` & `tmp/latch_cloud_clients-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_cloud_clients-0.1.2.tar", max compression
+gzip compressed data, was "latch_cloud_clients-0.1.3.tar", max compression
```

## Comparing `latch_cloud_clients-0.1.2.tar` & `latch_cloud_clients-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     7052 2024-04-19 18:57:40.206110 latch_cloud_clients-0.1.2/LICENSE
--rw-r--r--   0        0        0      121 2024-04-23 21:26:46.040298 latch_cloud_clients-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-04-19 18:57:40.207571 latch_cloud_clients-0.1.2/latch_cloud_clients/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 19:11:11.691773 latch_cloud_clients-0.1.2/latch_cloud_clients/aws/__init__.py
--rw-r--r--   0        0        0     9677 2024-04-23 19:11:28.023463 latch_cloud_clients-0.1.2/latch_cloud_clients/aws/aws.py
--rw-r--r--   0        0        0     4098 2024-04-23 19:11:50.057387 latch_cloud_clients-0.1.2/latch_cloud_clients/aws/client_pool.py
--rw-r--r--   0        0        0        0 2024-04-23 19:28:36.193575 latch_cloud_clients-0.1.2/latch_cloud_clients/gcp/__init__.py
--rw-r--r--   0        0        0     3100 2024-04-23 19:28:30.737616 latch_cloud_clients-0.1.2/latch_cloud_clients/gcp/client_pool.py
--rw-r--r--   0        0        0     3369 2024-04-23 22:28:19.034702 latch_cloud_clients-0.1.2/latch_cloud_clients/gcp/pubsub.py
--rw-r--r--   0        0        0        0 2024-04-23 19:28:30.747372 latch_cloud_clients-0.1.2/latch_cloud_clients/gcp/py.typed
--rw-r--r--   0        0        0    13697 2024-04-23 22:29:19.411186 latch_cloud_clients-0.1.2/latch_cloud_clients/gcp/storage.py
--rw-r--r--   0        0        0        0 2024-04-19 18:57:40.208421 latch_cloud_clients-0.1.2/latch_cloud_clients/py.typed
--rw-r--r--   0        0        0    24433 2024-04-23 22:23:31.663069 latch_cloud_clients-0.1.2/latch_cloud_clients/storage_clients.py
--rw-r--r--   0        0        0     1455 2024-04-23 22:29:39.245203 latch_cloud_clients-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 latch_cloud_clients-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     7052 2024-04-19 18:57:40.206110 latch_cloud_clients-0.1.3/LICENSE
+-rw-r--r--   0        0        0      121 2024-04-23 21:26:46.040298 latch_cloud_clients-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 18:57:40.207571 latch_cloud_clients-0.1.3/latch_cloud_clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 19:11:11.691773 latch_cloud_clients-0.1.3/latch_cloud_clients/aws/__init__.py
+-rw-r--r--   0        0        0     9677 2024-04-23 19:11:28.023463 latch_cloud_clients-0.1.3/latch_cloud_clients/aws/aws.py
+-rw-r--r--   0        0        0     4098 2024-04-23 19:11:50.057387 latch_cloud_clients-0.1.3/latch_cloud_clients/aws/client_pool.py
+-rw-r--r--   0        0        0        0 2024-04-23 19:28:36.193575 latch_cloud_clients-0.1.3/latch_cloud_clients/gcp/__init__.py
+-rw-r--r--   0        0        0     3100 2024-04-23 19:28:30.737616 latch_cloud_clients-0.1.3/latch_cloud_clients/gcp/client_pool.py
+-rw-r--r--   0        0        0     3369 2024-04-23 22:28:19.034702 latch_cloud_clients-0.1.3/latch_cloud_clients/gcp/pubsub.py
+-rw-r--r--   0        0        0        0 2024-04-23 19:28:30.747372 latch_cloud_clients-0.1.3/latch_cloud_clients/gcp/py.typed
+-rw-r--r--   0        0        0    13697 2024-04-23 22:29:19.411186 latch_cloud_clients-0.1.3/latch_cloud_clients/gcp/storage.py
+-rw-r--r--   0        0        0        0 2024-04-19 18:57:40.208421 latch_cloud_clients-0.1.3/latch_cloud_clients/py.typed
+-rw-r--r--   0        0        0    24434 2024-04-24 00:05:21.984419 latch_cloud_clients-0.1.3/latch_cloud_clients/storage_clients.py
+-rw-r--r--   0        0        0     1455 2024-04-24 00:05:29.032923 latch_cloud_clients-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 latch_cloud_clients-0.1.3/PKG-INFO
```

### Comparing `latch_cloud_clients-0.1.2/LICENSE` & `latch_cloud_clients-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.2/latch_cloud_clients/aws/aws.py` & `latch_cloud_clients-0.1.3/latch_cloud_clients/aws/aws.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.2/latch_cloud_clients/aws/client_pool.py` & `latch_cloud_clients-0.1.3/latch_cloud_clients/aws/client_pool.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.2/latch_cloud_clients/gcp/client_pool.py` & `latch_cloud_clients-0.1.3/latch_cloud_clients/gcp/client_pool.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.2/latch_cloud_clients/gcp/pubsub.py` & `latch_cloud_clients-0.1.3/latch_cloud_clients/gcp/pubsub.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.2/latch_cloud_clients/gcp/storage.py` & `latch_cloud_clients-0.1.3/latch_cloud_clients/gcp/storage.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.2/latch_cloud_clients/storage_clients.py` & `latch_cloud_clients-0.1.3/latch_cloud_clients/storage_clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 import math
 from collections.abc import AsyncGenerator, Coroutine
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any
 
 import botocore.exceptions
-from aws.aws import max_presigned_url_age
 from google.api_core.exceptions import (
     NotFound,
 )
 from latch_o11y.o11y import trace_function_with_span
 from opentelemetry.trace import Span, get_tracer
 from types_aiobotocore_s3.type_defs import (
     CompletedPartTypeDef,
 )
 
+from .aws.aws import max_presigned_url_age
 from .aws.client_pool import s3_pool
 from .gcp.client_pool import gcp_pool
 
 tracer = get_tracer(__name__)
 
 MP_THRESHOLD = 25000000
 MP_CHUNK_SIZE = 25000000
```

### Comparing `latch_cloud_clients-0.1.2/pyproject.toml` & `latch_cloud_clients-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latch-cloud-clients"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Taras Priadka <taras@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_cloud_clients"}]
 
 [tool.poetry.dependencies]
```

### Comparing `latch_cloud_clients-0.1.2/PKG-INFO` & `latch_cloud_clients-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latch-cloud-clients
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 License: CC0 1.0
 Author: Taras Priadka
 Author-email: taras@latch.bio
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

