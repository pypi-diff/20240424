# Comparing `tmp/eidolon_ai_client-0.1.6.tar.gz` & `tmp/eidolon_ai_client-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eidolon_ai_client-0.1.6.tar", max compression
+gzip compressed data, was "eidolon_ai_client-0.1.7.tar", max compression
```

## Comparing `eidolon_ai_client-0.1.6.tar` & `eidolon_ai_client-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/__init__.py
--rw-r--r--   0        0        0     7297 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/client.py
--rw-r--r--   0        0        0     4987 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/events.py
--rw-r--r--   0        0        0     2387 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/group_conversation.py
--rw-r--r--   0        0        0        0 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/util/__init__.py
--rw-r--r--   0        0        0     3728 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/util/aiohttp.py
--rw-r--r--   0        0        0      448 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/util/logger.py
--rw-r--r--   0        0        0     2361 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/util/request_context.py
--rw-r--r--   0        0        0      424 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/util/stream_collector.py
--rw-r--r--   0        0        0      541 2024-04-16 01:18:28.711470 eidolon_ai_client-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 eidolon_ai_client-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-24 05:50:43.436580 eidolon_ai_client-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-24 05:50:43.436580 eidolon_ai_client-0.1.7/eidolon_ai_client/__init__.py
+-rw-r--r--   0        0        0     7297 2024-04-24 05:50:43.436580 eidolon_ai_client-0.1.7/eidolon_ai_client/client.py
+-rw-r--r--   0        0        0     5157 2024-04-24 05:50:43.436580 eidolon_ai_client-0.1.7/eidolon_ai_client/events.py
+-rw-r--r--   0        0        0     2387 2024-04-24 05:50:43.436580 eidolon_ai_client-0.1.7/eidolon_ai_client/group_conversation.py
+-rw-r--r--   0        0        0        0 2024-04-24 05:50:43.436580 eidolon_ai_client-0.1.7/eidolon_ai_client/util/__init__.py
+-rw-r--r--   0        0        0     3728 2024-04-24 05:50:43.436580 eidolon_ai_client-0.1.7/eidolon_ai_client/util/aiohttp.py
+-rw-r--r--   0        0        0      448 2024-04-24 05:50:43.436580 eidolon_ai_client-0.1.7/eidolon_ai_client/util/logger.py
+-rw-r--r--   0        0        0     2361 2024-04-24 05:50:43.436580 eidolon_ai_client-0.1.7/eidolon_ai_client/util/request_context.py
+-rw-r--r--   0        0        0      424 2024-04-24 05:50:43.436580 eidolon_ai_client-0.1.7/eidolon_ai_client/util/stream_collector.py
+-rw-r--r--   0        0        0      645 2024-04-24 05:51:17.572367 eidolon_ai_client-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 eidolon_ai_client-0.1.7/PKG-INFO
```

### Comparing `eidolon_ai_client-0.1.6/eidolon_ai_client/client.py` & `eidolon_ai_client-0.1.7/eidolon_ai_client/client.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_client-0.1.6/eidolon_ai_client/events.py` & `eidolon_ai_client-0.1.7/eidolon_ai_client/events.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import annotations
 
 from abc import ABC
 from enum import Enum
-from pydantic import BaseModel, TypeAdapter
+from pydantic import BaseModel, TypeAdapter, Field
 from typing import List, TypeVar, Generic, Any, AsyncIterator, Type, Literal, Dict, Optional
 
 
 class FileHandle(BaseModel):
     machineURL: str
     process_id: str
     file_id: str
-    metadata: dict = {}
+    metadata: dict = Field(default={}, description="Metadata about the file")
+
+    def get_url(self):
+        return f"{self.machineURL}/processes/{self.process_id}/files/{self.file_id}"
 
 
 class Category(Enum):
     START = "start"
     INPUT = "input"
     END = "end"
     OUTPUT = "output"
```

### Comparing `eidolon_ai_client-0.1.6/eidolon_ai_client/group_conversation.py` & `eidolon_ai_client-0.1.7/eidolon_ai_client/group_conversation.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_client-0.1.6/eidolon_ai_client/util/aiohttp.py` & `eidolon_ai_client-0.1.7/eidolon_ai_client/util/aiohttp.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_client-0.1.6/eidolon_ai_client/util/request_context.py` & `eidolon_ai_client-0.1.7/eidolon_ai_client/util/request_context.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_client-0.1.6/pyproject.toml` & `eidolon_ai_client-0.1.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,31 @@
+[build-system]
+requires = [ "poetry-core",]
+build-backend = "poetry.core.masonry.api"
+
 [tool.poetry]
 name = "eidolon_ai_client"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
-authors = ["Luke Lalor <lukehlalor@gmail.com>"]
+authors = [ "Luke Lalor <lukehlalor@gmail.com>",]
 readme = "README.md"
 
+[tool.ruff]
+line-length = 121
+
+[tool.eidolon]
+update-tag = "client"
+last-update-hash = "4843133d1400a712699fa384421a44b2f95c098f"
+
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 setuptools = "^69.0.2"
 jsonref = "^1.1.0"
 pydantic = "^2.6.1"
 httpx = "^0.27.0"
 httpx-sse = "^0.4.0"
 sse-starlette = "^2.0.0"
 aiostream = "^0.5.2"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.1.7"
 pytest-asyncio = "^0.23.4"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.ruff]
-line-length = 121
```

### Comparing `eidolon_ai_client-0.1.6/PKG-INFO` & `eidolon_ai_client-0.1.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eidolon_ai_client
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Luke Lalor
 Author-email: lukehlalor@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiostream (>=0.5.2,<0.6.0)
```

