# Comparing `tmp/decor8ai-0.22.tar.gz` & `tmp/decor8ai-0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decor8ai-0.22.tar", max compression
+gzip compressed data, was "decor8ai-0.23.tar", max compression
```

## Comparing `decor8ai-0.22.tar` & `decor8ai-0.23.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11446 2024-04-17 17:24:20.585730 decor8ai-0.22/README.md
--rw-r--r--   0        0        0        0 2023-10-24 05:55:12.275635 decor8ai-0.22/decor8ai/__init__.py
--rw-r--r--   0        0        0     7176 2024-04-17 17:15:42.773864 decor8ai-0.22/decor8ai/client.py
--rw-r--r--   0        0        0      534 2024-04-17 17:27:02.341074 decor8ai-0.22/pyproject.toml
--rw-r--r--   0        0        0    12126 1970-01-01 00:00:00.000000 decor8ai-0.22/PKG-INFO
+-rw-r--r--   0        0        0    11446 2024-04-17 17:24:20.585730 decor8ai-0.23/README.md
+-rw-r--r--   0        0        0        0 2023-10-24 05:55:12.275635 decor8ai-0.23/decor8ai/__init__.py
+-rw-r--r--   0        0        0     7166 2024-04-24 16:03:53.276629 decor8ai-0.23/decor8ai/client.py
+-rw-r--r--   0        0        0      534 2024-04-24 16:07:20.043986 decor8ai-0.23/pyproject.toml
+-rw-r--r--   0        0        0    12126 1970-01-01 00:00:00.000000 decor8ai-0.23/PKG-INFO
```

### Comparing `decor8ai-0.22/README.md` & `decor8ai-0.23/README.md`

 * *Files identical despite different names*

### Comparing `decor8ai-0.22/decor8ai/client.py` & `decor8ai-0.23/decor8ai/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import requests
 import os
 import json
 from urllib.parse import urlparse
 
 dev_server_url = 'http://localhost:8000'
-prod_server_url = 'https://prod-app.decor8.ai:8000'
+prod_server_url = 'https://api.decor8.ai'
 url = prod_server_url
 token = os.environ.get('DECOR8AI_API_KEY')
 
 
 def prime_the_room_walls(input_image):
     def is_url(path):
         try:
```

### Comparing `decor8ai-0.22/pyproject.toml` & `decor8ai-0.23/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "decor8ai"
-version = "0.22"
+version = "0.23"
 description = "Decor8 AI is an AI Interior Design Tool. With Decor8 AI Python SDK, you can automate interior design generation tasks for room photos."
 authors = ["Akhilesh Joshi <akhilesh@immex.tech>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.decor8.ai"
 repository = "https://github.com/immex-tech/decor8ai-sdk"
```

### Comparing `decor8ai-0.22/PKG-INFO` & `decor8ai-0.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decor8ai
-Version: 0.22
+Version: 0.23
 Summary: Decor8 AI is an AI Interior Design Tool. With Decor8 AI Python SDK, you can automate interior design generation tasks for room photos.
 Home-page: https://www.decor8.ai
 License: MIT
 Author: Akhilesh Joshi
 Author-email: akhilesh@immex.tech
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

