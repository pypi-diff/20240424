# Comparing `tmp/llama_index_readers_microsoft_sharepoint-0.1.6.tar.gz` & `tmp/llama_index_readers_microsoft_sharepoint-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_microsoft_sharepoint-0.1.6.tar", max compression
+gzip compressed data, was "llama_index_readers_microsoft_sharepoint-0.1.7.tar", max compression
```

## Comparing `llama_index_readers_microsoft_sharepoint-0.1.6.tar` & `llama_index_readers_microsoft_sharepoint-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1782 2024-04-01 21:33:17.112191 llama_index_readers_microsoft_sharepoint-0.1.6/README.md
--rw-r--r--   0        0        0      107 2024-04-01 21:33:17.112191 llama_index_readers_microsoft_sharepoint-0.1.6/llama_index/readers/microsoft_sharepoint/__init__.py
--rw-r--r--   0        0        0    15522 2024-04-01 21:33:17.112191 llama_index_readers_microsoft_sharepoint-0.1.6/llama_index/readers/microsoft_sharepoint/base.py
--rw-r--r--   0        0        0    41139 2024-04-01 21:33:17.112191 llama_index_readers_microsoft_sharepoint-0.1.6/llama_index/readers/microsoft_sharepoint/file_path_info.png
--rw-r--r--   0        0        0     1594 2024-04-01 21:33:17.112191 llama_index_readers_microsoft_sharepoint-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 llama_index_readers_microsoft_sharepoint-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1782 2024-04-04 17:50:25.610780 llama_index_readers_microsoft_sharepoint-0.1.7/README.md
+-rw-r--r--   0        0        0      107 2024-04-04 17:50:25.610780 llama_index_readers_microsoft_sharepoint-0.1.7/llama_index/readers/microsoft_sharepoint/__init__.py
+-rw-r--r--   0        0        0    15493 2024-04-04 17:50:25.614780 llama_index_readers_microsoft_sharepoint-0.1.7/llama_index/readers/microsoft_sharepoint/base.py
+-rw-r--r--   0        0        0    41139 2024-04-04 17:50:25.614780 llama_index_readers_microsoft_sharepoint-0.1.7/llama_index/readers/microsoft_sharepoint/file_path_info.png
+-rw-r--r--   0        0        0     1594 2024-04-04 17:50:25.614780 llama_index_readers_microsoft_sharepoint-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 llama_index_readers_microsoft_sharepoint-0.1.7/PKG-INFO
```

### Comparing `llama_index_readers_microsoft_sharepoint-0.1.6/README.md` & `llama_index_readers_microsoft_sharepoint-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_microsoft_sharepoint-0.1.6/llama_index/readers/microsoft_sharepoint/base.py` & `llama_index_readers_microsoft_sharepoint-0.1.7/llama_index/readers/microsoft_sharepoint/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,15 +331,15 @@
 
         self._site_id_with_host_name = self._get_site_id_with_host_name(
             access_token, sharepoint_site_name
         )
 
         self._drive_id = self._get_drive_id()
 
-        if sharepoint_folder_id is None:
+        if not sharepoint_folder_id:
             sharepoint_folder_id = self._get_sharepoint_folder_id(
                 sharepoint_folder_path
             )
 
         return self._download_files_and_extract_metadata(
             sharepoint_folder_id, download_dir, recursive
         )
@@ -374,15 +374,15 @@
         return simple_loader.load_data()
 
     def load_data(
         self,
         sharepoint_site_name: Optional[str] = None,
         sharepoint_folder_path: Optional[str] = None,
         sharepoint_folder_id: Optional[str] = None,
-        recursive: bool = False,
+        recursive: bool = True,
     ) -> List[Document]:
         """
         Loads the files from the specified folder in the SharePoint site.
 
         Args:
             sharepoint_site_name (Optional[str]): The name of the SharePoint site.
             sharepoint_folder_path (Optional[str]): The path of the folder in the SharePoint site.
@@ -391,28 +391,28 @@
         Returns:
             List[Document]: A list containing the documents with metadata.
 
         Raises:
             Exception: If an error occurs while accessing SharePoint site.
         """
         # If no arguments are provided to load_data, default to the object attributes
-        if sharepoint_site_name is None:
+        if not sharepoint_site_name:
             sharepoint_site_name = self.sharepoint_site_name
 
-        if sharepoint_folder_path is None:
+        if not sharepoint_folder_path:
             sharepoint_folder_path = self.sharepoint_folder_path
 
-        if sharepoint_folder_id is None:
+        if not sharepoint_folder_id:
             sharepoint_folder_id = self.sharepoint_folder_id
 
         # TODO: make both of these values optional — and just default to the client ID defaults
-        if sharepoint_site_name is None:
+        if not sharepoint_site_name:
             raise ValueError("sharepoint_site_name must be provided.")
 
-        if sharepoint_folder_path is None and sharepoint_folder_id is None:
+        if not sharepoint_folder_path and not sharepoint_folder_id:
             raise ValueError(
                 "sharepoint_folder_path or sharepoint_folder_id must be provided."
             )
 
         try:
             with tempfile.TemporaryDirectory() as temp_dir:
                 files_metadata = self._download_files_from_sharepoint(
```

### Comparing `llama_index_readers_microsoft_sharepoint-0.1.6/llama_index/readers/microsoft_sharepoint/file_path_info.png` & `llama_index_readers_microsoft_sharepoint-0.1.7/llama_index/readers/microsoft_sharepoint/file_path_info.png`

 * *Files identical despite different names*

### Comparing `llama_index_readers_microsoft_sharepoint-0.1.6/pyproject.toml` & `llama_index_readers_microsoft_sharepoint-0.1.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 description = "llama-index readers microsoft_sharepoint integration"
 exclude = ["**/BUILD"]
 keywords = ["microsoft 365", "microsoft365", "sharepoint"]
 license = "MIT"
 maintainers = ["arun-soliton"]
 name = "llama-index-readers-microsoft-sharepoint"
 readme = "README.md"
-version = "0.1.6"
+version = "0.1.7"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_readers_microsoft_sharepoint-0.1.6/PKG-INFO` & `llama_index_readers_microsoft_sharepoint-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-microsoft-sharepoint
-Version: 0.1.6
+Version: 0.1.7
 Summary: llama-index readers microsoft_sharepoint integration
 License: MIT
 Keywords: microsoft 365,microsoft365,sharepoint
 Author: Your Name
 Author-email: you@example.com
 Maintainer: arun-soliton
 Requires-Python: >=3.8.1,<4.0
```

