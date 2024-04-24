# Comparing `tmp/getai-0.0.7.tar.gz` & `tmp/getai-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getai-0.0.7.tar", max compression
+gzip compressed data, was "getai-0.0.8.tar", max compression
```

## Comparing `getai-0.0.7.tar` & `getai-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1247 2024-04-23 11:42:53.993269 getai-0.0.7/LICENSE
--rw-r--r--   0        0        0     8542 2024-04-23 11:36:27.654734 getai-0.0.7/README.md
--rw-r--r--   0        0        0        0 2024-04-23 11:20:21.512462 getai-0.0.7/getai/__init__.py
--rw-r--r--   0        0        0      133 2024-04-23 11:20:21.512462 getai-0.0.7/getai/__main__.py
--rw-r--r--   0        0        0    13580 2024-04-23 21:26:46.319887 getai-0.0.7/getai/dataset_downloader.py
--rw-r--r--   0        0        0       37 2024-04-23 11:20:21.512462 getai-0.0.7/getai/getai_config.yaml
--rw-r--r--   0        0        0     7471 2024-04-24 09:51:09.949507 getai-0.0.7/getai/main.py
--rw-r--r--   0        0        0    28896 2024-04-24 11:00:39.252499 getai-0.0.7/getai/model_downloader.py
--rw-r--r--   0        0        0     3088 2024-04-24 09:51:09.949507 getai-0.0.7/getai/utils.py
--rw-r--r--   0        0        0      739 2024-04-24 11:02:21.335753 getai-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     9457 1970-01-01 00:00:00.000000 getai-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1247 2024-04-23 11:42:53.993269 getai-0.0.8/LICENSE
+-rw-r--r--   0        0        0     8542 2024-04-23 11:36:27.654734 getai-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 11:20:21.512462 getai-0.0.8/getai/__init__.py
+-rw-r--r--   0        0        0      133 2024-04-23 11:20:21.512462 getai-0.0.8/getai/__main__.py
+-rw-r--r--   0        0        0    13580 2024-04-23 21:26:46.319887 getai-0.0.8/getai/dataset_downloader.py
+-rw-r--r--   0        0        0       37 2024-04-23 11:20:21.512462 getai-0.0.8/getai/getai_config.yaml
+-rw-r--r--   0        0        0     7471 2024-04-24 09:51:09.949507 getai-0.0.8/getai/main.py
+-rw-r--r--   0        0        0    29224 2024-04-24 11:15:31.790074 getai-0.0.8/getai/model_downloader.py
+-rw-r--r--   0        0        0     3088 2024-04-24 09:51:09.949507 getai-0.0.8/getai/utils.py
+-rw-r--r--   0        0        0      739 2024-04-24 11:13:12.355567 getai-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     9457 1970-01-01 00:00:00.000000 getai-0.0.8/PKG-INFO
```

### Comparing `getai-0.0.7/LICENSE` & `getai-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `getai-0.0.7/README.md` & `getai-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `getai-0.0.7/getai/dataset_downloader.py` & `getai-0.0.8/getai/dataset_downloader.py`

 * *Files identical despite different names*

### Comparing `getai-0.0.7/getai/main.py` & `getai-0.0.8/getai/main.py`

 * *Files identical despite different names*

### Comparing `getai-0.0.7/getai/model_downloader.py` & `getai-0.0.8/getai/model_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 from rainbow_tqdm import tqdm
 
 from .utils import convert_to_bytes, interactive_branch_selection
 import chunk
 
 BASE_URL = "https://huggingface.co"
 
-logging.basicConfig(format='%(asctime)s - %(message)s', level=logging.DEBUG)
+# this program has two different loggers - root logging and self.logger within the AsyncModelDownloader class
+# the root logger is used for general logging, while the self.logger is used for more specific logging within the class
+
+logging.basicConfig(format='%(asctime)s - %(message)s', level=logging.INFO)
 
 file_size_pattern = re.compile(r'<a class="[^"]*" title="Download file"[^>]*>([\d.]+ [GMK]B)')
 
 
 class AsyncSearch:
 
     def __init__(self, query, filtered_models, total_models, branch_sizes, session, model_downloader):
@@ -194,30 +197,30 @@
         print(f"Search results sorted by '{sort_criteria}' in {'descending' if reverse else 'ascending'} order.")
 
 
 class AsyncModelDownloader:
 
     def __init__(self, max_retries=5, output_dir=None, max_connections=5, hf_token=None):
         self.logger = logging.getLogger(__name__)
-        self.logger.setLevel(logging.DEBUG)
+        self.logger.setLevel(logging.INFO)  # change the self.logger level to DEBUG for more verbose output
         self.output_dir = output_dir
         self.max_retries = max_retries
         self.max_connections = max_connections
         self.token = hf_token
         self.connector = None
         self.session = None
         self.timeout = aiohttp.ClientTimeout(total=None)
         self.branch_sizes = {}
         self.file_locks = {}  
 
     async def __aenter__(self):
         self.connector = TCPConnector(limit=self.max_connections)
         headers = {'Authorization': f'Bearer {self.token}'} if self.token else {}
         self.session = ClientSession(connector=self.connector, headers=headers)
-        self.logger.debug(f"Using token for authorization: {self.token is not None}")
+        self.logger.info(f"Using HF token for authorization: {self.token is not None}")
         self.logger.debug(f"Session created with headers: {headers}")
         return self
 
     async def __aexit__(self, _exc_type, _exc_val, _exc_tb):
         await self.close()
 
     async def close(self):
@@ -285,16 +288,16 @@
                 if file_hash is not None:
                     current_hash = await self.calculate_file_sha256(output_path)
                     if current_hash == file_hash:
                         self.logger.debug(f"'{filename}' exists and matches expected SHA256 hash; skipping.")
                         return
                     else:
                         self.logger.debug(f"'{filename}' exists but SHA256 hash doesn't match; resuming download.")
-                        self.logger.debug(f"Expected SHA256: {file_hash}")
-                        self.logger.debug(f"Actual SHA256: {current_hash}")
+                        self.logger.info(f"Expected SHA256: {file_hash}")
+                        self.logger.info(f"Actual SHA256: {current_hash}")
                         resume_size = output_path.stat().st_size
                 else:
                     self.logger.debug(f"'{filename}' exists but no expected SHA256 hash provided; skipping.")
                     return
             else:
                 resume_size = 0
 
@@ -551,28 +554,28 @@
             model_id = model['id']
             if model_id not in branch_sizes:
                 branch_sizes[model_id] = await self.get_branch_file_sizes(model_id, quiet=quiet)
         return branch_sizes
 
     async def get_branch_file_sizes(self, model, quiet=False):
         if not quiet:
-            print(f"Fetching file sizes for {model}...")
+            self.logger.debug(f"Fetching file sizes for {model}...")
         branches = await self.get_model_branches(model)
         branch_sizes = {}
         if self.session:
             for branch in branches:
                 page_url = f"{BASE_URL}/{model}/tree/{branch}"
                 try:
                     async with self.session.get(page_url) as response:
                         if response.status == 200:
                             text = await response.text()
                             file_sizes = file_size_pattern.findall(text)
                             total_size = sum(convert_to_bytes(size) for size in file_sizes)
                             branch_sizes[branch] = total_size
                         else:
                             if not quiet:
-                                print(f"Failed to fetch page for branch: {branch}")
+                                self.logger.info(f"Failed to fetch page for branch: {branch}")
                 except Exception as e:
                     if not quiet:
-                        print(f"Error fetching branch file sizes for {model}, branch {branch}: {e}")
+                        self.logger.info(f"Error fetching branch file sizes for {model}, branch {branch}: {e}")
                     continue
         return branch_sizes
```

### Comparing `getai-0.0.7/getai/utils.py` & `getai-0.0.8/getai/utils.py`

 * *Files identical despite different names*

### Comparing `getai-0.0.7/pyproject.toml` & `getai-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "getai"
-version = "0.0.7"
+version = "0.0.8"
 description = "GetAI - An asynchronous AI search and download tool for AI models, datasets, and tools. Designed to streamline the process of downloading machine learning models, datasets, and more."
 authors = ["Ben Gorlick <ben@unifiedlearning.ai>"]
 license = "MIT - with attribution"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `getai-0.0.7/PKG-INFO` & `getai-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getai
-Version: 0.0.7
+Version: 0.0.8
 Summary: GetAI - An asynchronous AI search and download tool for AI models, datasets, and tools. Designed to streamline the process of downloading machine learning models, datasets, and more.
 License: MIT - with attribution
 Author: Ben Gorlick
 Author-email: ben@unifiedlearning.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

