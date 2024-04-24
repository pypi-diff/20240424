# Comparing `tmp/getai-0.0.5.tar.gz` & `tmp/getai-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getai-0.0.5.tar", max compression
+gzip compressed data, was "getai-0.0.6.tar", max compression
```

## Comparing `getai-0.0.5.tar` & `getai-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1247 2024-04-23 11:42:53.993269 getai-0.0.5/LICENSE
--rw-r--r--   0        0        0     8542 2024-04-23 11:36:27.654734 getai-0.0.5/README.md
--rw-r--r--   0        0        0        0 2024-04-23 11:20:21.512462 getai-0.0.5/getai/__init__.py
--rw-r--r--   0        0        0      133 2024-04-23 11:20:21.512462 getai-0.0.5/getai/__main__.py
--rw-r--r--   0        0        0    13580 2024-04-23 21:26:46.319887 getai-0.0.5/getai/dataset_downloader.py
--rw-r--r--   0        0        0       37 2024-04-23 11:20:21.512462 getai-0.0.5/getai/getai_config.yaml
--rw-r--r--   0        0        0     7471 2024-04-23 21:29:55.208418 getai-0.0.5/getai/main.py
--rw-r--r--   0        0        0    27604 2024-04-23 22:25:13.540753 getai-0.0.5/getai/model_downloader.py
--rw-r--r--   0        0        0     3088 2024-04-23 11:52:12.548596 getai-0.0.5/getai/utils.py
--rw-r--r--   0        0        0      740 2024-04-23 22:28:55.820492 getai-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     9357 1970-01-01 00:00:00.000000 getai-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1247 2024-04-23 11:42:53.993269 getai-0.0.6/LICENSE
+-rw-r--r--   0        0        0     8542 2024-04-23 11:36:27.654734 getai-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 11:20:21.512462 getai-0.0.6/getai/__init__.py
+-rw-r--r--   0        0        0      133 2024-04-23 11:20:21.512462 getai-0.0.6/getai/__main__.py
+-rw-r--r--   0        0        0    13580 2024-04-23 21:26:46.319887 getai-0.0.6/getai/dataset_downloader.py
+-rw-r--r--   0        0        0       37 2024-04-23 11:20:21.512462 getai-0.0.6/getai/getai_config.yaml
+-rw-r--r--   0        0        0     7471 2024-04-24 09:51:09.949507 getai-0.0.6/getai/main.py
+-rw-r--r--   0        0        0    28922 2024-04-24 10:55:00.450309 getai-0.0.6/getai/model_downloader.py
+-rw-r--r--   0        0        0     3088 2024-04-24 09:51:09.949507 getai-0.0.6/getai/utils.py
+-rw-r--r--   0        0        0      740 2024-04-24 10:55:37.034764 getai-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     9357 1970-01-01 00:00:00.000000 getai-0.0.6/PKG-INFO
```

### Comparing `getai-0.0.5/LICENSE` & `getai-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `getai-0.0.5/README.md` & `getai-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `getai-0.0.5/getai/dataset_downloader.py` & `getai-0.0.6/getai/dataset_downloader.py`

 * *Files identical despite different names*

### Comparing `getai-0.0.5/getai/main.py` & `getai-0.0.6/getai/main.py`

 * *Files identical despite different names*

### Comparing `getai-0.0.5/getai/model_downloader.py` & `getai-0.0.6/getai/model_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,29 @@
 import base64
 import datetime
 import hashlib
 import json
 import logging
 import re
 from pathlib import Path
+from typing import Optional, Union, Dict, BinaryIO
+import os
+import requests
 
 import aiofiles
 import aiohttp
+from aiofiles import open as aio_open
+
 from aiohttp import ClientSession, TCPConnector
 from prompt_toolkit import PromptSession
 from prompt_toolkit.completion import WordCompleter
 from rainbow_tqdm import tqdm
 
 from .utils import convert_to_bytes, interactive_branch_selection
+import chunk
 
 BASE_URL = "https://huggingface.co"
 
 logging.basicConfig(format='%(asctime)s - %(message)s', level=logging.DEBUG)
 
 file_size_pattern = re.compile(r'<a class="[^"]*" title="Download file"[^>]*>([\d.]+ [GMK]B)')
 
@@ -242,42 +248,65 @@
             output_folder = self.get_output_folder(identifier, branch_to_use, is_lora, is_llamacpp, self.output_dir)
             sha256_dict = dict(sha256_list)
             await self.download_model_files(identifier, branch_to_use, links, sha256_dict, output_folder)
             if check:
                 await self.check_model_files(identifier, branch_to_use, links, sha256_dict, output_folder)
         else:
             print(f"No active session available to download model {identifier}.")
-            
+
+    async def http_get(self, session, url: str, temp_file: BinaryIO, resume_size=0, headers=None):
+        headers = headers or {}
+        if resume_size > 0:
+            headers["Range"] = f"bytes={resume_size}-"
+        async with session.get(url, headers=headers) as r:
+            content_length = int(r.headers.get("Content-Length", 0))
+            total = resume_size + content_length
+            progress = tqdm(
+                unit="B",
+                unit_scale=True,
+                total=total,
+                initial=resume_size,
+                desc=f"Downloading {Path(url).name}",
+            )
+            async for chunk in r.content.iter_chunked(1024):
+                if chunk: 
+                    progress.update(len(chunk))
+                    temp_file.write(chunk)
+            progress.close()
+
     async def download_model_file(self, session, url, output_folder, file_hash):
         filename = Path(url.rsplit('/', 1)[1])
         output_path = output_folder / filename
 
         # Create a lock for the file if it doesn't exist
         if output_path not in self.file_locks:
             self.file_locks[output_path] = asyncio.Lock()
 
         # Acquire the lock before accessing the file
         async with self.file_locks[output_path]:
             if output_path.exists():
-                current_hash = await self.calculate_file_sha256(output_path)
-                if current_hash == file_hash:
-                    print(f"'{filename}' exists and matches expected SHA256 hash; skipping.")
+                if file_hash is not None:
+                    current_hash = await self.calculate_file_sha256(output_path)
+                    if current_hash == file_hash:
+                        self.logger.debug(f"'{filename}' exists and matches expected SHA256 hash; skipping.")
+                        return
+                    else:
+                        self.logger.debug(f"'{filename}' exists but SHA256 hash doesn't match; resuming download.")
+                        self.logger.debug(f"Expected SHA256: {file_hash}")
+                        self.logger.debug(f"Actual SHA256: {current_hash}")
+                        resume_size = output_path.stat().st_size
+                else:
+                    self.logger.debug(f"'{filename}' exists but no expected SHA256 hash provided; skipping.")
                     return
-                print(f"'{filename}' exists but SHA256 hash matching failed; redownloading.")
-
-            async with session.get(url) as response:
-                response.raise_for_status()
-                total_size = response.content_length or 0
-                async with aiofiles.open(output_path, 'wb') as f:
-                    progress_bar = tqdm(total=total_size, desc=filename.name, unit='iB', unit_scale=True, ncols=100)
-                    async for chunk in response.content.iter_chunked(1024):
-                        await f.write(chunk)
-                        progress_bar.update(len(chunk))
-                    progress_bar.close()
+            else:
+                resume_size = 0
 
+            async with aiofiles.open(output_path, "ab") as temp_file:
+                await self.http_get(session, url, temp_file, resume_size=resume_size)
+                
     async def search_models(self, query, model_id_filter=None, rfilename_filter=None):
         async with self.session as session:
             url = f"{BASE_URL}/api/models"
             params = {
                 "search": query,
                 "sort": "downloads",
                 "direction": "-1",
@@ -460,24 +489,29 @@
         sha256_str = '\n'.join([f' {sha256} {filename}' for filename, sha256 in sha256_dict.items()])
         if sha256_str:
             metadata += f'sha256sum:\n{sha256_str}'
         metadata += '\n'
         metadata_path = output_folder / 'huggingface-metadata.txt'
         async with aiofiles.open(metadata_path, 'w') as metafile:
             await metafile.write(metadata)
-        tasks = []
-        if self.session:
-            for link in links:
+        
+        semaphore = asyncio.Semaphore(self.max_connections)
+
+        async def download_file(link):
+            async with semaphore:
                 filename = Path(link).name
                 if filename in sha256_dict:
                     file_hash = sha256_dict[filename]
                 else:
                     print(f"Warning: No SHA256 hash found for {filename}. Downloading without sha256 verification.")
                     file_hash = None
-                tasks.append(self.download_model_file(self.session, link, output_folder, file_hash))
+                await self.download_model_file(self.session, link, output_folder, file_hash)
+        
+        if self.session:
+            tasks = [asyncio.ensure_future(download_file(link)) for link in links]
             await asyncio.gather(*tasks)
 
     async def check_model_files(self, model, branch, links, sha256_dict, output_folder):
         validated = True
         for link in links:
             filename = Path(link).name
             file_path = output_folder / filename
@@ -499,21 +533,22 @@
                 print(f"Checksum validated: {file_path}")
         if validated:
             print(f'[+] Validated all files and checksums for model: {model}, branch: {branch}!')
         else:
             print(f'[-] Invalid files or checksums for model: {model}, branch: {branch}. You may need to rerun the download process with the --clean flag.')
 
     async def calculate_file_sha256(self, file_path):
+        chunk_size = 1024 * 1024
         sha256 = hashlib.sha256()
-        async with aiofiles.open(file_path, 'rb') as f:
+        async with aio_open(file_path, 'rb') as file:
             while True:
-                data = await f.read(4096)
-                if not data:
+                chunk = await file.read(chunk_size)
+                if not chunk:
                     break
-                sha256.update(data)
+                sha256.update(chunk)
         return sha256.hexdigest()
 
     async def get_branch_file_sizes_for_models(self, models, quiet=False):
         branch_sizes = {}
         for model in models:
             model_id = model['id']
             if model_id not in branch_sizes:
```

### Comparing `getai-0.0.5/getai/utils.py` & `getai-0.0.6/getai/utils.py`

 * *Files identical despite different names*

### Comparing `getai-0.0.5/pyproject.toml` & `getai-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "getai"
-version = "0.0.5"
+version = "0.0.6"
 description = "GetAI - An asynchronous AI search and download tool for AI models, datasets, and tools. Designed to streamline the process of downloading machine learning models, datasets, and more."
 authors = ["Ben Gorlick <ben@unifiedlearning.ai>"]
 license = "MIT - with attribution"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `getai-0.0.5/PKG-INFO` & `getai-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getai
-Version: 0.0.5
+Version: 0.0.6
 Summary: GetAI - An asynchronous AI search and download tool for AI models, datasets, and tools. Designed to streamline the process of downloading machine learning models, datasets, and more.
 License: MIT - with attribution
 Author: Ben Gorlick
 Author-email: ben@unifiedlearning.ai
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

