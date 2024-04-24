# Comparing `tmp/getai-0.0.4.tar.gz` & `tmp/getai-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getai-0.0.4.tar", max compression
+gzip compressed data, was "getai-0.0.5.tar", max compression
```

## Comparing `getai-0.0.4.tar` & `getai-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1247 2024-04-23 11:42:53.993269 getai-0.0.4/LICENSE
--rw-r--r--   0        0        0     8542 2024-04-23 11:36:27.654734 getai-0.0.4/README.md
--rw-r--r--   0        0        0        0 2024-04-23 11:20:21.512462 getai-0.0.4/getai/__init__.py
--rw-r--r--   0        0        0      133 2024-04-23 11:20:21.512462 getai-0.0.4/getai/__main__.py
--rw-r--r--   0        0        0    13580 2024-04-23 21:26:46.319887 getai-0.0.4/getai/dataset_downloader.py
--rw-r--r--   0        0        0       37 2024-04-23 11:20:21.512462 getai-0.0.4/getai/getai_config.yaml
--rw-r--r--   0        0        0     7471 2024-04-23 21:29:55.208418 getai-0.0.4/getai/main.py
--rw-r--r--   0        0        0    27341 2024-04-23 21:27:24.548406 getai-0.0.4/getai/model_downloader.py
--rw-r--r--   0        0        0     3088 2024-04-23 11:52:12.548596 getai-0.0.4/getai/utils.py
--rw-r--r--   0        0        0      740 2024-04-23 21:30:36.343960 getai-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     9357 1970-01-01 00:00:00.000000 getai-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1247 2024-04-23 11:42:53.993269 getai-0.0.5/LICENSE
+-rw-r--r--   0        0        0     8542 2024-04-23 11:36:27.654734 getai-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 11:20:21.512462 getai-0.0.5/getai/__init__.py
+-rw-r--r--   0        0        0      133 2024-04-23 11:20:21.512462 getai-0.0.5/getai/__main__.py
+-rw-r--r--   0        0        0    13580 2024-04-23 21:26:46.319887 getai-0.0.5/getai/dataset_downloader.py
+-rw-r--r--   0        0        0       37 2024-04-23 11:20:21.512462 getai-0.0.5/getai/getai_config.yaml
+-rw-r--r--   0        0        0     7471 2024-04-23 21:29:55.208418 getai-0.0.5/getai/main.py
+-rw-r--r--   0        0        0    27604 2024-04-23 22:25:13.540753 getai-0.0.5/getai/model_downloader.py
+-rw-r--r--   0        0        0     3088 2024-04-23 11:52:12.548596 getai-0.0.5/getai/utils.py
+-rw-r--r--   0        0        0      740 2024-04-23 22:28:55.820492 getai-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     9357 1970-01-01 00:00:00.000000 getai-0.0.5/PKG-INFO
```

### Comparing `getai-0.0.4/LICENSE` & `getai-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `getai-0.0.4/README.md` & `getai-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `getai-0.0.4/getai/dataset_downloader.py` & `getai-0.0.5/getai/dataset_downloader.py`

 * *Files identical despite different names*

### Comparing `getai-0.0.4/getai/main.py` & `getai-0.0.5/getai/main.py`

 * *Files identical despite different names*

### Comparing `getai-0.0.4/getai/model_downloader.py` & `getai-0.0.5/getai/model_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,25 +51,16 @@
             else:
                 break
 
     async def display_search_results(self):
         while True:
             total_pages = (len(self.filtered_models) + self.page_size - 1) // self.page_size
             current_page = self.search_history[-1][1]
-            current_models = self.get_current_models(current_page)
-
-            # Fetch branch file sizes for the current page models
-            self.branch_sizes = await self.model_downloader.get_branch_file_sizes_for_models(current_models)
-
             while True:
-                self.display_current_page(current_page, total_pages)
-
-                # Prefetch branch sizes for the next pages
-                await self.prefetch_branch_sizes(current_page, total_pages)
-
+                await self.display_current_page(current_page, total_pages)
                 user_input = await self.get_user_input(current_page, total_pages)
 
                 if user_input.lower() == 'n' and current_page < total_pages:
                     current_page += 1
                     self.search_history[-1] = (self.filtered_models, current_page)
                 elif user_input.lower() == 'p' and current_page > 1:
                     current_page -= 1
@@ -86,34 +77,44 @@
                         self.filtered_models, current_page = self.search_history[-1]
                         self.total_models = len(self.filtered_models)
                         break
                     else:
                         print("You are already at the main search results.")
                 elif user_input.isdigit() and 1 <= int(user_input) <= len(self.get_current_models(current_page)):
                     selected_model = self.get_current_models(current_page)[int(user_input) - 1]
-                    await self.model_downloader.download_selected_model(selected_model['id'])
+                    branches = await self.model_downloader.get_model_branches(selected_model['id'])
+                    if len(branches) > 1:
+                        print(f"Multiple branches detected for model: {selected_model['id']}")
+                        selected_branch = await self.model_downloader.select_branch_interactive(branches)
+                        await self.model_downloader.download_model(selected_model['id'], selected_branch, False, False)
+                    else:
+                        await self.model_downloader.download_model(selected_model['id'], 'main', False, False)
                     break
                 else:
                     print("Invalid input. Please try again.")
 
             await self.handle_user_choice()
 
-    def display_current_page(self, current_page, total_pages):
+    async def display_current_page(self, current_page, total_pages):
         start_index = (current_page - 1) * self.page_size
         end_index = min(start_index + self.page_size, len(self.filtered_models))
         current_models = self.filtered_models[start_index:end_index]
         print(f"Search results for '{self.query}' (Page {current_page} of {total_pages}, Total: {self.total_models}):")
         for i, model in enumerate(current_models, start=1):
             model_id, model_name, author = model['id'], model.get('modelName', model['id']), model.get('author', 'N/A')
-            model_size = self.branch_sizes.get(model_id, {}).get('main', 'N/A')
-            if model_size != 'N/A':
-                model_size = f"{model_size / (1024 ** 3):.2f} GB"
-            print(f"{i}. \033[94m{model_name}\033[0m by \033[93m{author}\033[0m (\033[96m{model_id}\033[0m) \033[93m(Size: {model_size})\033[0m")
-        print("Enter 'n' for the next page, 'p' for the previous page, 'f' to filter, 's' to sort, 'r' to return to previous search results, or the model number to download.")
-
+            # Fetch branch file sizes for the current model
+            branch_sizes = await self.model_downloader.get_branch_file_sizes(model_id)
+            if branch_sizes:
+                model_size = sum(branch_sizes.values()) / (1024 ** 3)
+                size_str = f"{model_size:.2f} GB"
+            else:
+                size_str = 'N/A'
+            print(f"{i}. \033[94m{model_name}\033[0m by \033[93m{author}\033[0m (\033[96m{model_id}\033[0m) \033[93m(Size: {size_str})\033[0m")
+        print("Enter 'n' for next page, 'p' for previous page, 'f' to filter, 's' to sort, 'r' for previous results, or the model # to download.")
+        
     async def prefetch_branch_sizes(self, current_page, total_pages):
         prefetch_threshold = 4  # Prefetch threshold in pages
         prefetch_pages = min(prefetch_threshold, total_pages - current_page)
 
         if prefetch_pages > 0:
             start_index = current_page * self.page_size
             end_index = min(start_index + self.page_size * prefetch_pages, len(self.filtered_models))
@@ -144,15 +145,15 @@
     def get_current_models(self, current_page):
         start_index = (current_page - 1) * self.page_size
         end_index = min(start_index + self.page_size, len(self.filtered_models))
         current_models = self.filtered_models[start_index:end_index]
         return current_models
 
     async def handle_user_choice(self):
-        print("Enter 'b' to go back to the filtered search results, 'm' to return to the main search results, or 'q' to quit.")
+        print("Enter 'b' to see the filtered search results, 'm' for the main search results, or 'q' to quit.")
         user_input = await asyncio.get_event_loop().run_in_executor(None, input, "> ")
         if user_input.lower() == 'b':
             return
         elif user_input.lower() == 'm':
             self.filtered_models = self.main_search_models.copy()
             self.total_models = len(self.filtered_models)
             self.search_history = [(self.main_search_models.copy(), 1)]
```

### Comparing `getai-0.0.4/getai/utils.py` & `getai-0.0.5/getai/utils.py`

 * *Files identical despite different names*

### Comparing `getai-0.0.4/pyproject.toml` & `getai-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "getai"
-version = "0.0.4"
+version = "0.0.5"
 description = "GetAI - An asynchronous AI search and download tool for AI models, datasets, and tools. Designed to streamline the process of downloading machine learning models, datasets, and more."
 authors = ["Ben Gorlick <ben@unifiedlearning.ai>"]
 license = "MIT - with attribution"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `getai-0.0.4/PKG-INFO` & `getai-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getai
-Version: 0.0.4
+Version: 0.0.5
 Summary: GetAI - An asynchronous AI search and download tool for AI models, datasets, and tools. Designed to streamline the process of downloading machine learning models, datasets, and more.
 License: MIT - with attribution
 Author: Ben Gorlick
 Author-email: ben@unifiedlearning.ai
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

