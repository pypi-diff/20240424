# Comparing `tmp/unique_sdk-0.7.3.tar.gz` & `tmp/unique_sdk-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unique_sdk-0.7.3.tar", max compression
+gzip compressed data, was "unique_sdk-0.8.0.tar", max compression
```

## Comparing `unique_sdk-0.7.3.tar` & `unique_sdk-0.8.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1065 2024-02-22 20:34:45.135463 unique_sdk-0.7.3/LICENSE
--rw-r--r--   0        0        0    12693 2024-03-27 13:36:17.907620 unique_sdk-0.7.3/README.md
--rw-r--r--   0        0        0     1400 2024-04-18 07:34:45.921205 unique_sdk-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     2594 2024-03-22 15:16:21.679272 unique_sdk-0.7.3/unique_sdk/__init__.py
--rw-r--r--   0        0        0    11523 2024-03-22 15:16:21.683007 unique_sdk-0.7.3/unique_sdk/_api_requestor.py
--rw-r--r--   0        0        0     3603 2024-02-27 19:23:40.262420 unique_sdk-0.7.3/unique_sdk/_api_resource.py
--rw-r--r--   0        0        0       46 2024-02-22 20:34:45.142217 unique_sdk-0.7.3/unique_sdk/_api_version.py
--rw-r--r--   0        0        0     2912 2024-02-22 20:34:45.142578 unique_sdk-0.7.3/unique_sdk/_error.py
--rw-r--r--   0        0        0     2513 2024-04-18 07:34:45.931494 unique_sdk-0.7.3/unique_sdk/_http_client.py
--rw-r--r--   0        0        0     3949 2024-02-22 20:34:45.142939 unique_sdk-0.7.3/unique_sdk/_list_object.py
--rw-r--r--   0        0        0      270 2024-02-22 20:34:45.143185 unique_sdk-0.7.3/unique_sdk/_object_classes.py
--rw-r--r--   0        0        0      255 2024-02-22 20:34:45.143412 unique_sdk-0.7.3/unique_sdk/_request_options.py
--rw-r--r--   0        0        0    10525 2024-02-22 20:34:45.143669 unique_sdk-0.7.3/unique_sdk/_unique_object.py
--rw-r--r--   0        0        0      576 2024-02-22 20:34:45.143826 unique_sdk-0.7.3/unique_sdk/_unique_response.py
--rw-r--r--   0        0        0     5902 2024-02-22 20:34:45.144184 unique_sdk-0.7.3/unique_sdk/_util.py
--rw-r--r--   0        0        0       18 2024-02-22 20:34:45.144336 unique_sdk-0.7.3/unique_sdk/_version.py
--rw-r--r--   0        0        0     2855 2024-02-22 20:34:45.144492 unique_sdk-0.7.3/unique_sdk/_webhook.py
--rw-r--r--   0        0        0        0 2024-02-22 20:34:45.144734 unique_sdk-0.7.3/unique_sdk/api_resources/__init__.py
--rw-r--r--   0        0        0     1738 2024-02-22 20:34:45.144922 unique_sdk-0.7.3/unique_sdk/api_resources/_chat_completion.py
--rw-r--r--   0        0        0     3005 2024-04-11 09:50:40.483379 unique_sdk-0.7.3/unique_sdk/api_resources/_content.py
--rw-r--r--   0        0        0      374 2024-02-22 20:34:45.145139 unique_sdk-0.7.3/unique_sdk/api_resources/_event.py
--rw-r--r--   0        0        0     2310 2024-04-12 09:11:24.416488 unique_sdk-0.7.3/unique_sdk/api_resources/_integrated.py
--rw-r--r--   0        0        0     4937 2024-03-22 15:16:21.690047 unique_sdk-0.7.3/unique_sdk/api_resources/_message.py
--rw-r--r--   0        0        0     1235 2024-04-11 09:50:40.488785 unique_sdk-0.7.3/unique_sdk/api_resources/_search.py
--rw-r--r--   0        0        0     1366 2024-02-22 20:34:45.147647 unique_sdk-0.7.3/unique_sdk/api_resources/_search_string.py
--rw-r--r--   0        0        0    13153 1970-01-01 00:00:00.000000 unique_sdk-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/LICENSE
+-rw-r--r--   0        0        0    15211 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/README.md
+-rw-r--r--   0        0        0     1400 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2594 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/__init__.py
+-rw-r--r--   0        0        0    11523 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_api_requestor.py
+-rw-r--r--   0        0        0     3603 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_api_resource.py
+-rw-r--r--   0        0        0       46 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_api_version.py
+-rw-r--r--   0        0        0     2912 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_error.py
+-rw-r--r--   0        0        0     2513 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_http_client.py
+-rw-r--r--   0        0        0     3949 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_list_object.py
+-rw-r--r--   0        0        0      270 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_object_classes.py
+-rw-r--r--   0        0        0      255 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_request_options.py
+-rw-r--r--   0        0        0    10525 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_unique_object.py
+-rw-r--r--   0        0        0      576 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_unique_response.py
+-rw-r--r--   0        0        0     5902 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_util.py
+-rw-r--r--   0        0        0       18 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_version.py
+-rw-r--r--   0        0        0     2855 2024-04-24 07:50:03.601397 unique_sdk-0.8.0/unique_sdk/_webhook.py
+-rw-r--r--   0        0        0        0 2024-04-24 07:50:03.601397 unique_sdk-0.8.0/unique_sdk/api_resources/__init__.py
+-rw-r--r--   0        0        0     1738 2024-04-24 07:50:03.601397 unique_sdk-0.8.0/unique_sdk/api_resources/_chat_completion.py
+-rw-r--r--   0        0        0     3823 2024-04-24 07:50:03.601397 unique_sdk-0.8.0/unique_sdk/api_resources/_content.py
+-rw-r--r--   0        0        0      374 2024-04-24 07:50:03.601397 unique_sdk-0.8.0/unique_sdk/api_resources/_event.py
+-rw-r--r--   0        0        0     2310 2024-04-24 07:50:03.601397 unique_sdk-0.8.0/unique_sdk/api_resources/_integrated.py
+-rw-r--r--   0        0        0     4937 2024-04-24 07:50:03.601397 unique_sdk-0.8.0/unique_sdk/api_resources/_message.py
+-rw-r--r--   0        0        0     1235 2024-04-24 07:50:03.601397 unique_sdk-0.8.0/unique_sdk/api_resources/_search.py
+-rw-r--r--   0        0        0     1366 2024-04-24 07:50:03.601397 unique_sdk-0.8.0/unique_sdk/api_resources/_search_string.py
+-rw-r--r--   0        0        0    15671 1970-01-01 00:00:00.000000 unique_sdk-0.8.0/PKG-INFO
```

### Comparing `unique_sdk-0.7.3/LICENSE` & `unique_sdk-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.3/README.md` & `unique_sdk-0.8.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 ## Table of Contents
 
 1. [Installation](#installation)
 2. [Requirements](#requirements)
 3. [Usage Instructions](#usage-instructions)
 4. [Webhook Triggers](#webhook-triggers)
 5. [Available API Resources](#available-api-resources)
+   - [Content](#content)
    - [Message](#message)
    - [Chat Completion](#chat-completion)
    - [Search](#search)
    - [Search String](#search-string)
 6. [Error Handling](#error-handling)
 7. [Examples](#examples)
 
@@ -194,19 +195,123 @@
     chatId=chat_id,
     text="Here is your answer.",
 )
 ```
 
 ## Available API Resources
 
+- [Content](#content)
 - [Message](#message)
 - [Chat Completion](#chat-completion)
 - [Search](#search)
 - [Search String](#search-string)
 
+### Content
+
+#### `unique_sdk.Content.search`
+
+Allows you to load full content/files from the knowledge-base of unique with the rights of the userId and companyId. Provided a `where` query for filtering. Filtering can be done on any of the following fields: `
+
+- `id`
+- `key`
+- `ownerId`
+- `title`
+- `url`
+
+Here an example of retrieving all files that contain the number 42 in the `title` or the `key` typically this is used to search by filename.
+
+```python
+unique_sdk.Content.search(
+    user_id=userId,
+    company_id=companyId,
+    where={
+        "OR": [
+            {
+                "title": {
+                    "contains": "42",
+                },
+            },
+            {
+                "key": {
+                    "contains": "42",
+                },
+            },
+        ],
+    },
+    chatId=chatId,
+)
+```
+
+#### `unique_sdk.Content.upsert`
+
+Enables upload of a new Content into the Knowledge base of unique into a specific scope with `scopeId`.
+
+Typical usage is the following. That creates a Content and uploads a file
+
+```python
+
+createdContent = upload_file(
+    userId,
+    companyId,
+    "/path/to/file.pdf",
+    "test.pdf",
+    "application/pdf",
+    "scope_stcj2osgbl722m22jayidx0n",
+)
+
+def upload_file(
+    userId,
+    companyId,
+    path_to_file,
+    displayed_filename,
+    mimeType,
+    scope_or_unique_path,
+):
+    size = os.path.getsize(path_to_file)
+    createdContent = unique_sdk.Content.upsert(
+        user_id=userId,
+        company_id=companyId,
+        input={
+            "key": displayed_filename,
+            "title": displayed_filename,
+            "mimeType": mimeType,
+        },
+        scopeId=scope_or_unique_path,
+    )
+
+    uploadUrl = createdContent.writeUrl
+
+    # upload to azure blob storage SAS url uploadUrl the pdf file translatedFile make sure it is treated as a application/pdf
+    with open(path_to_file, "rb") as file:
+        requests.put(
+            uploadUrl,
+            data=file,
+            headers={
+                "X-Ms-Blob-Content-Type": mimeType,
+                "X-Ms-Blob-Type": "BlockBlob",
+            },
+        )
+
+    unique_sdk.Content.upsert(
+        user_id=userId,
+        company_id=companyId,
+        input={
+            "key": displayed_filename,
+            "title": displayed_filename,
+            "mimeType": mimeType,
+            "byteSize": size,
+        },
+        scopeId=scope_or_unique_path,
+        readUrl=createdContent.readUrl,
+    )
+
+    return createdContent
+
+```
+
 ### Message
 
 #### `unique_sdk.Message.list`
 
 Retrieve a list of messages for a provided `chatId`.
 
 ```python
```

### Comparing `unique_sdk-0.7.3/pyproject.toml` & `unique_sdk-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unique-sdk"
-version = "0.7.3"
+version = "0.8.0"
 description = ""
 authors = [
     "Konstantin Krauss <konstantin@unique.ch>",
     "Andreas Hauri <andreas@unique.ch>",
 ]
 readme = "README.md"
 license = "MIT"
```

### Comparing `unique_sdk-0.7.3/unique_sdk/__init__.py` & `unique_sdk-0.8.0/unique_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.3/unique_sdk/_api_requestor.py` & `unique_sdk-0.8.0/unique_sdk/_api_requestor.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.3/unique_sdk/_api_resource.py` & `unique_sdk-0.8.0/unique_sdk/_api_resource.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.3/unique_sdk/_error.py` & `unique_sdk-0.8.0/unique_sdk/_error.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.3/unique_sdk/_http_client.py` & `unique_sdk-0.8.0/unique_sdk/_http_client.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.3/unique_sdk/_list_object.py` & `unique_sdk-0.8.0/unique_sdk/_list_object.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.3/unique_sdk/_unique_object.py` & `unique_sdk-0.8.0/unique_sdk/_unique_object.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.3/unique_sdk/_unique_response.py` & `unique_sdk-0.8.0/unique_sdk/_unique_response.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.3/unique_sdk/_util.py` & `unique_sdk-0.8.0/unique_sdk/_util.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.3/unique_sdk/_webhook.py` & `unique_sdk-0.8.0/unique_sdk/_webhook.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.3/unique_sdk/api_resources/_chat_completion.py` & `unique_sdk-0.8.0/unique_sdk/api_resources/_chat_completion.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.3/unique_sdk/api_resources/_content.py` & `unique_sdk-0.8.0/unique_sdk/api_resources/_content.py`

 * *Files 24% similar despite different names*

```diff
@@ -61,14 +61,29 @@
         title: Optional["Content.StringNullableFilter"]
         url: Optional["Content.StringNullableFilter"]
 
     class SearchParams(RequestOptions):
         where: "Content.ContentWhereInput"
         chatId: NotRequired[str]
 
+    class Input(TypedDict):
+        key: str
+        title: Optional[str]
+        mimeType: str
+        ownerType: str
+        ownerId: str
+        byteSize: Optional[int]
+
+    class UpsertParams(RequestOptions):
+        input: "Content.Input"
+        scopeId: str
+        sourceOwnerType: str
+        storeInternally: bool
+        fileUrl: Optional[str]
+
     class Chunk(TypedDict):
         text: str
         startPage: Optional[int]
         order: Optional[int]
 
     id: str
     key: str
@@ -77,18 +92,39 @@
     updatedAt: str
     chunks: List[Chunk]
     metadata: Optional[Dict[str, Any]]
 
     @classmethod
     def search(
         cls, user_id: str, company_id: str, **params: Unpack["Content.SearchParams"]
-    ) -> "Content":
+    ) -> List["Content"]:
         return cast(
             "Content",
             cls._static_request(
                 "post",
                 "/content/search",
                 user_id,
                 company_id,
                 params=params,
             ),
         )
+
+    @classmethod
+    def upsert(
+        cls,
+        user_id: str,
+        company_id: str,
+        **params: Unpack["Content.UpsertParams"],
+    ) -> "Content":
+        """
+        UpsertsContent
+        """
+        return cast(
+            "Content",
+            cls._static_request(
+                "post",
+                "/content/upsert",
+                user_id,
+                company_id,
+                params=params,
+            ),
+        )
```

### Comparing `unique_sdk-0.7.3/unique_sdk/api_resources/_integrated.py` & `unique_sdk-0.8.0/unique_sdk/api_resources/_integrated.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.3/unique_sdk/api_resources/_message.py` & `unique_sdk-0.8.0/unique_sdk/api_resources/_message.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.3/unique_sdk/api_resources/_search.py` & `unique_sdk-0.8.0/unique_sdk/api_resources/_search.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.3/unique_sdk/api_resources/_search_string.py` & `unique_sdk-0.8.0/unique_sdk/api_resources/_search_string.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.3/PKG-INFO` & `unique_sdk-0.8.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unique-sdk
-Version: 0.7.3
+Version: 0.8.0
 Summary: 
 License: MIT
 Author: Konstantin Krauss
 Author-email: konstantin@unique.ch
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -22,14 +22,15 @@
 ## Table of Contents
 
 1. [Installation](#installation)
 2. [Requirements](#requirements)
 3. [Usage Instructions](#usage-instructions)
 4. [Webhook Triggers](#webhook-triggers)
 5. [Available API Resources](#available-api-resources)
+   - [Content](#content)
    - [Message](#message)
    - [Chat Completion](#chat-completion)
    - [Search](#search)
    - [Search String](#search-string)
 6. [Error Handling](#error-handling)
 7. [Examples](#examples)
 
@@ -209,19 +210,123 @@
     chatId=chat_id,
     text="Here is your answer.",
 )
 ```
 
 ## Available API Resources
 
+- [Content](#content)
 - [Message](#message)
 - [Chat Completion](#chat-completion)
 - [Search](#search)
 - [Search String](#search-string)
 
+### Content
+
+#### `unique_sdk.Content.search`
+
+Allows you to load full content/files from the knowledge-base of unique with the rights of the userId and companyId. Provided a `where` query for filtering. Filtering can be done on any of the following fields: `
+
+- `id`
+- `key`
+- `ownerId`
+- `title`
+- `url`
+
+Here an example of retrieving all files that contain the number 42 in the `title` or the `key` typically this is used to search by filename.
+
+```python
+unique_sdk.Content.search(
+    user_id=userId,
+    company_id=companyId,
+    where={
+        "OR": [
+            {
+                "title": {
+                    "contains": "42",
+                },
+            },
+            {
+                "key": {
+                    "contains": "42",
+                },
+            },
+        ],
+    },
+    chatId=chatId,
+)
+```
+
+#### `unique_sdk.Content.upsert`
+
+Enables upload of a new Content into the Knowledge base of unique into a specific scope with `scopeId`.
+
+Typical usage is the following. That creates a Content and uploads a file
+
+```python
+
+createdContent = upload_file(
+    userId,
+    companyId,
+    "/path/to/file.pdf",
+    "test.pdf",
+    "application/pdf",
+    "scope_stcj2osgbl722m22jayidx0n",
+)
+
+def upload_file(
+    userId,
+    companyId,
+    path_to_file,
+    displayed_filename,
+    mimeType,
+    scope_or_unique_path,
+):
+    size = os.path.getsize(path_to_file)
+    createdContent = unique_sdk.Content.upsert(
+        user_id=userId,
+        company_id=companyId,
+        input={
+            "key": displayed_filename,
+            "title": displayed_filename,
+            "mimeType": mimeType,
+        },
+        scopeId=scope_or_unique_path,
+    )
+
+    uploadUrl = createdContent.writeUrl
+
+    # upload to azure blob storage SAS url uploadUrl the pdf file translatedFile make sure it is treated as a application/pdf
+    with open(path_to_file, "rb") as file:
+        requests.put(
+            uploadUrl,
+            data=file,
+            headers={
+                "X-Ms-Blob-Content-Type": mimeType,
+                "X-Ms-Blob-Type": "BlockBlob",
+            },
+        )
+
+    unique_sdk.Content.upsert(
+        user_id=userId,
+        company_id=companyId,
+        input={
+            "key": displayed_filename,
+            "title": displayed_filename,
+            "mimeType": mimeType,
+            "byteSize": size,
+        },
+        scopeId=scope_or_unique_path,
+        readUrl=createdContent.readUrl,
+    )
+
+    return createdContent
+
+```
+
 ### Message
 
 #### `unique_sdk.Message.list`
 
 Retrieve a list of messages for a provided `chatId`.
 
 ```python
```

