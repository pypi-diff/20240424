# Comparing `tmp/getai-0.0.3.tar.gz` & `tmp/getai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getai-0.0.3.tar", max compression
+gzip compressed data, was "getai-0.0.4.tar", max compression
```

## Comparing `getai-0.0.3.tar` & `getai-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1247 2024-04-23 11:42:53.993269 getai-0.0.3/LICENSE
--rw-r--r--   0        0        0     8542 2024-04-23 11:36:27.654734 getai-0.0.3/README.md
--rw-r--r--   0        0        0        0 2024-04-23 11:20:21.512462 getai-0.0.3/getai/__init__.py
--rw-r--r--   0        0        0      133 2024-04-23 11:20:21.512462 getai-0.0.3/getai/__main__.py
--rw-r--r--   0        0        0    13484 2024-04-23 11:37:33.678508 getai-0.0.3/getai/dataset_downloader.py
--rw-r--r--   0        0        0       37 2024-04-23 11:20:21.512462 getai-0.0.3/getai/getai_config.yaml
--rw-r--r--   0        0        0     7327 2024-04-23 11:39:31.809895 getai-0.0.3/getai/main.py
--rw-r--r--   0        0        0    27321 2024-04-23 11:38:50.364408 getai-0.0.3/getai/model_downloader.py
--rw-r--r--   0        0        0     3088 2024-04-23 11:52:12.548596 getai-0.0.3/getai/utils.py
--rw-r--r--   0        0        0      740 2024-04-23 12:13:19.894252 getai-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     9357 1970-01-01 00:00:00.000000 getai-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1247 2024-04-23 11:42:53.993269 getai-0.0.4/LICENSE
+-rw-r--r--   0        0        0     8542 2024-04-23 11:36:27.654734 getai-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 11:20:21.512462 getai-0.0.4/getai/__init__.py
+-rw-r--r--   0        0        0      133 2024-04-23 11:20:21.512462 getai-0.0.4/getai/__main__.py
+-rw-r--r--   0        0        0    13580 2024-04-23 21:26:46.319887 getai-0.0.4/getai/dataset_downloader.py
+-rw-r--r--   0        0        0       37 2024-04-23 11:20:21.512462 getai-0.0.4/getai/getai_config.yaml
+-rw-r--r--   0        0        0     7471 2024-04-23 21:29:55.208418 getai-0.0.4/getai/main.py
+-rw-r--r--   0        0        0    27341 2024-04-23 21:27:24.548406 getai-0.0.4/getai/model_downloader.py
+-rw-r--r--   0        0        0     3088 2024-04-23 11:52:12.548596 getai-0.0.4/getai/utils.py
+-rw-r--r--   0        0        0      740 2024-04-23 21:30:36.343960 getai-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     9357 1970-01-01 00:00:00.000000 getai-0.0.4/PKG-INFO
```

### Comparing `getai-0.0.3/LICENSE` & `getai-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `getai-0.0.3/README.md` & `getai-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `getai-0.0.3/getai/dataset_downloader.py` & `getai-0.0.4/getai/dataset_downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,22 +219,24 @@
             url = f"{BASE_URL}/api/datasets/{dataset_id}/tree/{revision or 'main'}"
             async with self.session.get(url) as response:
                 if response.status == 200:
                     file_tree = await response.json()
                     output_folder = self.get_dataset_output_folder(dataset_id)
                     output_folder.mkdir(parents=True, exist_ok=True)
                     logger.info(f"Downloading dataset files to: {output_folder}")
+                    tasks = []
                     for file in file_tree:
                         file_url = f"{BASE_URL}/datasets/{dataset_id}/resolve/{revision or 'main'}/{file['path']}"
-                        await self.download_dataset_file(file_url, output_folder / file['path'])
+                        tasks.append(self.download_dataset_file(file_url, output_folder / file['path']))
+                    await asyncio.gather(*tasks)
                 else:
                     logging.error(f"Error fetching dataset file tree: HTTP {response.status}")
         except Exception as e:
             logging.exception(f"Error downloading dataset files: {e}")
-
+        
     async def download_dataset_file(self, url, file_path):
         try:
             async with self.session.get(url) as response:
                 if response.status == 200:
                     total_size = response.content_length or 0
                     output_path = Path(file_path)
                     output_path.parent.mkdir(parents=True, exist_ok=True)
```

### Comparing `getai-0.0.3/getai/main.py` & `getai-0.0.4/getai/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,76 +80,73 @@
 
     if args.mode == 'search':
         if not args.search_mode:
             logging.error("Please specify the search mode (model or dataset).")
             return
 
         if args.search_mode == 'model':
-            model_downloader = AsyncModelDownloader(
+            async with AsyncModelDownloader(
                 max_retries=5,
                 output_dir=None,
                 max_connections=5,
                 hf_token=hf_token
-            )
-            async with model_downloader:
+            ) as model_downloader:
                 try:
                     await model_downloader.search_models(args.query)
                 except KeyboardInterrupt:
                     print("\nKeyboardInterrupt received. Closing model downloader...")
-                finally:
-                    await close_model_downloader(model_downloader)
-        else: 
-            dataset_downloader = AsyncDatasetDownloader(
+                except Exception as e:
+                    print(f"Error during model search: {e}")
+        else:
+            async with AsyncDatasetDownloader(
                 max_retries=5,
                 output_dir=None,
                 max_connections=5,
                 hf_token=hf_token
-            )
-            try:
-                await dataset_downloader.search_datasets(
-                    query=args.query,
-                    author=args.author,
-                    filter=args.filter,
-                    sort=args.sort,
-                    direction=args.direction,
-                    limit=args.limit,
-                    full=args.full
-                )
-            except KeyboardInterrupt:
-                print("\nKeyboardInterrupt received. Closing dataset downloader...")
-            finally:
-                await close_dataset_downloader(dataset_downloader)
+            ) as dataset_downloader:
+                try:
+                    await dataset_downloader.search_datasets(
+                        query=args.query,
+                        author=args.author,
+                        filter=args.filter,
+                        sort=args.sort,
+                        direction=args.direction,
+                        limit=args.limit,
+                        full=args.full
+                    )
+                except KeyboardInterrupt:
+                    print("\nKeyboardInterrupt received. Closing dataset downloader...")
+                except Exception as e:
+                    print(f"Error during dataset search: {e}")
     elif args.mode == 'dataset':
-        dataset_downloader = AsyncDatasetDownloader(
+        async with AsyncDatasetDownloader(
             max_retries=args.max_retries,
             output_dir=args.output_dir,
             max_connections=args.max_connections,
             hf_token=hf_token
-        )
-
-        try:
-            await dataset_downloader.download_dataset_info(args.identifier, args.revision, args.full)
-        except KeyboardInterrupt:
-            print("\nKeyboardInterrupt received. Closing dataset downloader...")
-        finally:
-            await close_dataset_downloader(dataset_downloader)
+        ) as dataset_downloader:
+            try:
+                await dataset_downloader.download_dataset_info(args.identifier, args.revision, args.full)
+            except KeyboardInterrupt:
+                print("\nKeyboardInterrupt received. Closing dataset downloader...")
+            except Exception as e:
+                print(f"Error during dataset download: {e}")
     else:  # args.mode == 'model'
-        model_downloader = AsyncModelDownloader(
+        async with AsyncModelDownloader(
             max_retries=args.max_retries,
             output_dir=args.output_dir,
             max_connections=args.max_connections,
             hf_token=hf_token
-        )
-
-        try:
-            await model_downloader.download_model(args.identifier, args.branch, args.clean, args.check)
-        except KeyboardInterrupt:
-            print("\nKeyboardInterrupt received. Closing model downloader...")
-        finally:
-            await close_model_downloader(model_downloader)
+        ) as model_downloader:
+            try:
+                await model_downloader.download_model(args.identifier, args.branch, args.clean, args.check)
+            except KeyboardInterrupt:
+                print("\nKeyboardInterrupt received. Closing model downloader...")
+            except Exception as e:
+                print(f"Error during model download: {e}")
 
 
 if __name__ == "__main__":
     loop = asyncio.get_event_loop()
     try:
         loop.run_until_complete(main())
     except KeyboardInterrupt:
```

### Comparing `getai-0.0.3/getai/model_downloader.py` & `getai-0.0.4/getai/model_downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,27 +229,27 @@
             selected_branch = await self.select_branch_interactive(branches)
             print(f"Downloading {model_id} from branch '\033[96m{selected_branch}\033[0m'...")
             await self.download_model(model_id, selected_branch, False, False)
         else:
             print(f"No active session available to download model {model_id}.")
 
     async def download_model(self, identifier, branch, clean, check):
-        branch_sizes = await self.get_branch_file_sizes(identifier)
-        branches = await self.get_model_branches(identifier)
         if self.session:
+            branch_sizes = await self.get_branch_file_sizes(identifier)
+            branches = await self.get_model_branches(identifier)
             branch_to_use = await self.select_branch(branches, branch, branch_sizes)
             links, sha256_list, is_lora, is_llamacpp = await self.get_download_links_from_huggingface(identifier, branch_to_use, text_only=False)
             output_folder = self.get_output_folder(identifier, branch_to_use, is_lora, is_llamacpp, self.output_dir)
             sha256_dict = dict(sha256_list)
             await self.download_model_files(identifier, branch_to_use, links, sha256_dict, output_folder)
             if check:
                 await self.check_model_files(identifier, branch_to_use, links, sha256_dict, output_folder)
         else:
             print(f"No active session available to download model {identifier}.")
-
+            
     async def download_model_file(self, session, url, output_folder, file_hash):
         filename = Path(url.rsplit('/', 1)[1])
         output_path = output_folder / filename
 
         # Create a lock for the file if it doesn't exist
         if output_path not in self.file_locks:
             self.file_locks[output_path] = asyncio.Lock()
```

### Comparing `getai-0.0.3/getai/utils.py` & `getai-0.0.4/getai/utils.py`

 * *Files identical despite different names*

### Comparing `getai-0.0.3/pyproject.toml` & `getai-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "getai"
-version = "0.0.3"
+version = "0.0.4"
 description = "GetAI - An asynchronous AI search and download tool for AI models, datasets, and tools. Designed to streamline the process of downloading machine learning models, datasets, and more."
 authors = ["Ben Gorlick <ben@unifiedlearning.ai>"]
 license = "MIT - with attribution"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `getai-0.0.3/PKG-INFO` & `getai-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getai
-Version: 0.0.3
+Version: 0.0.4
 Summary: GetAI - An asynchronous AI search and download tool for AI models, datasets, and tools. Designed to streamline the process of downloading machine learning models, datasets, and more.
 License: MIT - with attribution
 Author: Ben Gorlick
 Author-email: ben@unifiedlearning.ai
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

