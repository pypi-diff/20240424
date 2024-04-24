# Comparing `tmp/airbyte_source_microsoft_sharepoint-0.2.2.tar.gz` & `tmp/airbyte_source_microsoft_sharepoint-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_microsoft_sharepoint-0.2.2.tar", max compression
+gzip compressed data, was "airbyte_source_microsoft_sharepoint-0.2.3.tar", max compression
```

## Comparing `airbyte_source_microsoft_sharepoint-0.2.2.tar` & `airbyte_source_microsoft_sharepoint-0.2.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4748 2024-03-28 15:37:58.000000 airbyte_source_microsoft_sharepoint-0.2.2/README.md
--rw-r--r--   0        0        0      973 2024-03-28 16:29:25.587461 airbyte_source_microsoft_sharepoint-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      150 2024-03-28 15:37:58.000000 airbyte_source_microsoft_sharepoint-0.2.2/source_microsoft_sharepoint/__init__.py
--rw-r--r--   0        0        0      766 2024-03-28 15:37:58.000000 airbyte_source_microsoft_sharepoint-0.2.2/source_microsoft_sharepoint/run.py
--rw-r--r--   0        0        0     3211 2024-03-28 15:37:58.000000 airbyte_source_microsoft_sharepoint-0.2.2/source_microsoft_sharepoint/source.py
--rw-r--r--   0        0        0     5146 2024-03-28 15:37:58.000000 airbyte_source_microsoft_sharepoint-0.2.2/source_microsoft_sharepoint/spec.py
--rw-r--r--   0        0        0    12207 2024-03-28 15:37:58.000000 airbyte_source_microsoft_sharepoint-0.2.2/source_microsoft_sharepoint/stream_reader.py
--rw-r--r--   0        0        0     3849 2024-03-28 15:37:58.000000 airbyte_source_microsoft_sharepoint-0.2.2/source_microsoft_sharepoint/utils.py
--rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 airbyte_source_microsoft_sharepoint-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     4748 2024-04-24 10:43:09.000000 airbyte_source_microsoft_sharepoint-0.2.3/README.md
+-rw-r--r--   0        0        0      973 2024-04-24 11:34:35.808321 airbyte_source_microsoft_sharepoint-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      150 2024-04-24 10:43:09.000000 airbyte_source_microsoft_sharepoint-0.2.3/source_microsoft_sharepoint/__init__.py
+-rw-r--r--   0        0        0      766 2024-04-24 10:43:09.000000 airbyte_source_microsoft_sharepoint-0.2.3/source_microsoft_sharepoint/run.py
+-rw-r--r--   0        0        0     3211 2024-04-24 10:43:09.000000 airbyte_source_microsoft_sharepoint-0.2.3/source_microsoft_sharepoint/source.py
+-rw-r--r--   0        0        0     5156 2024-04-24 10:43:09.000000 airbyte_source_microsoft_sharepoint-0.2.3/source_microsoft_sharepoint/spec.py
+-rw-r--r--   0        0        0    12727 2024-04-24 10:43:09.000000 airbyte_source_microsoft_sharepoint-0.2.3/source_microsoft_sharepoint/stream_reader.py
+-rw-r--r--   0        0        0     3849 2024-04-24 10:43:09.000000 airbyte_source_microsoft_sharepoint-0.2.3/source_microsoft_sharepoint/utils.py
+-rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 airbyte_source_microsoft_sharepoint-0.2.3/PKG-INFO
```

### Comparing `airbyte_source_microsoft_sharepoint-0.2.2/README.md` & `airbyte_source_microsoft_sharepoint-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_microsoft_sharepoint-0.2.2/pyproject.toml` & `airbyte_source_microsoft_sharepoint-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.2.2"
+version = "0.2.3"
 name = "airbyte-source-microsoft-sharepoint"
 description = "Source implementation for Microsoft SharePoint."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_microsoft_sharepoint-0.2.2/source_microsoft_sharepoint/run.py` & `airbyte_source_microsoft_sharepoint-0.2.3/source_microsoft_sharepoint/run.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_microsoft_sharepoint-0.2.2/source_microsoft_sharepoint/source.py` & `airbyte_source_microsoft_sharepoint-0.2.3/source_microsoft_sharepoint/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_microsoft_sharepoint-0.2.2/source_microsoft_sharepoint/spec.py` & `airbyte_source_microsoft_sharepoint-0.2.3/source_microsoft_sharepoint/spec.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         airbyte_secret=True,
     )
     client_secret: str = Field(
         title="Client Secret",
         description="Client Secret of your Microsoft developer application",
         airbyte_secret=True,
     )
-    refresh_token: str = Field(
+    refresh_token: Optional[str] = Field(
         title="Refresh Token",
         description="Refresh Token of your Microsoft developer application",
         airbyte_secret=True,
     )
 
 
 class ServiceCredentials(BaseModel):
```

### Comparing `airbyte_source_microsoft_sharepoint-0.2.2/source_microsoft_sharepoint/stream_reader.py` & `airbyte_source_microsoft_sharepoint-0.2.3/source_microsoft_sharepoint/stream_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -195,22 +195,26 @@
     @lru_cache(maxsize=None)
     def drives(self):
         """
         Retrieves and caches SharePoint drives, including the user's drive based on authentication type.
         """
         drives = execute_query_with_retry(self.one_drive_client.drives.get())
 
-        if self.config.credentials.auth_type == "Client":
-            my_drive = execute_query_with_retry(self.one_drive_client.me.drive.get())
-        else:
-            my_drive = execute_query_with_retry(
-                self.one_drive_client.users.get_by_principal_name(self.config.credentials.user_principal_name).drive.get()
-            )
+        # skip this step for application authentication flow
+        if self.config.credentials.auth_type != "Client" or (
+            hasattr(self.config.credentials, "refresh_token") and self.config.credentials.refresh_token
+        ):
+            if self.config.credentials.auth_type == "Client":
+                my_drive = execute_query_with_retry(self.one_drive_client.me.drive.get())
+            else:
+                my_drive = execute_query_with_retry(
+                    self.one_drive_client.users.get_by_principal_name(self.config.credentials.user_principal_name).drive.get()
+                )
 
-        drives.add_child(my_drive)
+            drives.add_child(my_drive)
 
         return drives
 
     def _get_shared_files_from_all_drives(self, parsed_drives):
         drive_ids = [drive.id for drive in parsed_drives]
 
         shared_drive_items = execute_query_with_retry(self.one_drive_client.me.drive.shared_with_me())
@@ -222,19 +226,23 @@
                 yield from self._get_shared_drive_object(parent_reference["driveId"], drive_item.id, drive_item.web_url)
 
     def get_all_files(self):
         if self.config.search_scope in ("ACCESSIBLE_DRIVES", "ALL"):
             # Get files from accessible drives
             yield from self._get_files_by_drive_name(self.drives, self.config.folder_path)
 
-        if self.config.search_scope in ("SHARED_ITEMS", "ALL"):
-            parsed_drives = [] if self.config.search_scope == "SHARED_ITEMS" else self.drives
+        # skip this step for application authentication flow
+        if self.config.credentials.auth_type != "Client" or (
+            hasattr(self.config.credentials, "refresh_token") and self.config.credentials.refresh_token
+        ):
+            if self.config.search_scope in ("SHARED_ITEMS", "ALL"):
+                parsed_drives = [] if self.config.search_scope == "SHARED_ITEMS" else self.drives
 
-            # Get files from shared items
-            yield from self._get_shared_files_from_all_drives(parsed_drives)
+                # Get files from shared items
+                yield from self._get_shared_files_from_all_drives(parsed_drives)
 
     def get_matching_files(self, globs: List[str], prefix: Optional[str], logger: logging.Logger) -> Iterable[RemoteFile]:
         """
         Retrieve all files matching the specified glob patterns in SharePoint.
         """
         files = self.get_all_files()
```

### Comparing `airbyte_source_microsoft_sharepoint-0.2.2/source_microsoft_sharepoint/utils.py` & `airbyte_source_microsoft_sharepoint-0.2.3/source_microsoft_sharepoint/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_microsoft_sharepoint-0.2.2/PKG-INFO` & `airbyte_source_microsoft_sharepoint-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-microsoft-sharepoint
-Version: 0.2.2
+Version: 0.2.3
 Summary: Source implementation for Microsoft SharePoint.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

