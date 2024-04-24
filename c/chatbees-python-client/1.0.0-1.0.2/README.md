# Comparing `tmp/chatbees_python_client-1.0.0.tar.gz` & `tmp/chatbees_python_client-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatbees_python_client-1.0.0.tar", max compression
+gzip compressed data, was "chatbees_python_client-1.0.2.tar", max compression
```

## Comparing `chatbees_python_client-1.0.0.tar` & `chatbees_python_client-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    11342 2024-02-03 05:19:30.172255 chatbees_python_client-1.0.0/LICENSE
--rw-r--r--   0        0        0     6073 2024-02-11 21:33:26.595699 chatbees_python_client-1.0.0/README.md
--rw-r--r--   0        0        0     6148 2024-03-20 20:25:04.619495 chatbees_python_client-1.0.0/chatbees/.DS_Store
--rw-r--r--   0        0        0      271 2024-04-04 16:21:08.597061 chatbees_python_client-1.0.0/chatbees/__init__.py
--rw-r--r--   0        0        0        0 2024-02-03 05:19:30.172668 chatbees_python_client-1.0.0/chatbees/client/__init__.py
--rw-r--r--   0        0        0     1460 2024-02-11 21:33:26.596005 chatbees_python_client-1.0.0/chatbees/client/admin_management.py
--rw-r--r--   0        0        0     3536 2024-04-04 16:21:08.597882 chatbees_python_client-1.0.0/chatbees/client/collection_management.py
--rw-r--r--   0        0        0        0 2024-02-03 05:19:30.173002 chatbees_python_client-1.0.0/chatbees/client_models/__init__.py
--rw-r--r--   0        0        0      974 2024-04-04 16:21:08.598133 chatbees_python_client-1.0.0/chatbees/client_models/chat.py
--rw-r--r--   0        0        0    12283 2024-04-04 16:21:08.598329 chatbees_python_client-1.0.0/chatbees/client_models/collection.py
--rw-r--r--   0        0        0        0 2024-02-03 05:19:30.173430 chatbees_python_client-1.0.0/chatbees/server_models/__init__.py
--rw-r--r--   0        0        0      138 2024-02-11 21:33:17.343641 chatbees_python_client-1.0.0/chatbees/server_models/admin_api.py
--rw-r--r--   0        0        0      684 2024-02-06 18:41:34.330037 chatbees_python_client-1.0.0/chatbees/server_models/chat.py
--rw-r--r--   0        0        0      998 2024-04-04 16:21:08.598469 chatbees_python_client-1.0.0/chatbees/server_models/collection_api.py
--rw-r--r--   0        0        0     2329 2024-04-04 16:21:08.598600 chatbees_python_client-1.0.0/chatbees/server_models/doc_api.py
--rw-r--r--   0        0        0      640 2024-04-04 16:21:08.598825 chatbees_python_client-1.0.0/chatbees/server_models/ingestion_api.py
--rw-r--r--   0        0        0      841 2024-04-04 16:21:08.598928 chatbees_python_client-1.0.0/chatbees/server_models/ingestion_type.py
--rw-r--r--   0        0        0      358 2024-04-04 16:21:08.599119 chatbees_python_client-1.0.0/chatbees/server_models/search_api.py
--rw-r--r--   0        0        0    11482 2024-04-04 16:21:08.599399 chatbees_python_client-1.0.0/chatbees/tests/api_surface_test.py
--rw-r--r--   0        0        0       39 2024-02-03 05:19:30.174160 chatbees_python_client-1.0.0/chatbees/tests/data/española.txt
--rw-r--r--   0        0        0       32 2024-02-03 05:19:30.174268 chatbees_python_client-1.0.0/chatbees/tests/data/française.txt
--rw-r--r--   0        0        0      463 2024-02-03 05:19:30.174378 chatbees_python_client-1.0.0/chatbees/tests/data/text_file.txt
--rw-r--r--   0        0        0       30 2024-02-03 05:19:30.174477 chatbees_python_client-1.0.0/chatbees/tests/data/中文.txt
--rw-r--r--   0        0        0     8527 2024-04-04 16:21:08.599719 chatbees_python_client-1.0.0/chatbees/tests/smoke_test.py
--rw-r--r--   0        0        0        0 2024-02-03 05:19:30.174691 chatbees_python_client-1.0.0/chatbees/utils/__init__.py
--rw-r--r--   0        0        0     1022 2024-02-06 18:39:33.176649 chatbees_python_client-1.0.0/chatbees/utils/ask.py
--rw-r--r--   0        0        0     1638 2024-03-11 18:24:32.039859 chatbees_python_client-1.0.0/chatbees/utils/config.py
--rw-r--r--   0        0        0     1709 2024-02-03 05:19:30.174998 chatbees_python_client-1.0.0/chatbees/utils/exceptions.py
--rw-r--r--   0        0        0      729 2024-04-04 16:20:59.474400 chatbees_python_client-1.0.0/chatbees/utils/file_upload.py
--rw-r--r--   0        0        0      477 2024-04-04 16:21:45.575686 chatbees_python_client-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6579 1970-01-01 00:00:00.000000 chatbees_python_client-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11342 2024-02-03 05:19:30.172255 chatbees_python_client-1.0.2/LICENSE
+-rw-r--r--   0        0        0     6117 2024-04-24 16:30:23.190228 chatbees_python_client-1.0.2/README.md
+-rw-r--r--   0        0        0     6148 2024-03-20 20:25:04.619495 chatbees_python_client-1.0.2/chatbees/.DS_Store
+-rw-r--r--   0        0        0      271 2024-04-04 16:21:08.597061 chatbees_python_client-1.0.2/chatbees/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-03 05:19:30.172668 chatbees_python_client-1.0.2/chatbees/client/__init__.py
+-rw-r--r--   0        0        0     1460 2024-02-11 21:33:26.596005 chatbees_python_client-1.0.2/chatbees/client/admin_management.py
+-rw-r--r--   0        0        0     3536 2024-04-04 16:21:08.597882 chatbees_python_client-1.0.2/chatbees/client/collection_management.py
+-rw-r--r--   0        0        0        0 2024-02-03 05:19:30.173002 chatbees_python_client-1.0.2/chatbees/client_models/__init__.py
+-rw-r--r--   0        0        0      974 2024-04-04 16:21:08.598133 chatbees_python_client-1.0.2/chatbees/client_models/chat.py
+-rw-r--r--   0        0        0    12283 2024-04-04 16:21:08.598329 chatbees_python_client-1.0.2/chatbees/client_models/collection.py
+-rw-r--r--   0        0        0        0 2024-02-03 05:19:30.173430 chatbees_python_client-1.0.2/chatbees/server_models/__init__.py
+-rw-r--r--   0        0        0      138 2024-02-11 21:33:17.343641 chatbees_python_client-1.0.2/chatbees/server_models/admin_api.py
+-rw-r--r--   0        0        0      684 2024-02-06 18:41:34.330037 chatbees_python_client-1.0.2/chatbees/server_models/chat.py
+-rw-r--r--   0        0        0      998 2024-04-04 16:21:08.598469 chatbees_python_client-1.0.2/chatbees/server_models/collection_api.py
+-rw-r--r--   0        0        0     2329 2024-04-04 16:21:08.598600 chatbees_python_client-1.0.2/chatbees/server_models/doc_api.py
+-rw-r--r--   0        0        0      640 2024-04-04 16:21:08.598825 chatbees_python_client-1.0.2/chatbees/server_models/ingestion_api.py
+-rw-r--r--   0        0        0     1401 2024-04-24 16:30:23.190480 chatbees_python_client-1.0.2/chatbees/server_models/ingestion_type.py
+-rw-r--r--   0        0        0      358 2024-04-04 16:21:08.599119 chatbees_python_client-1.0.2/chatbees/server_models/search_api.py
+-rw-r--r--   0        0        0    11482 2024-04-04 16:21:08.599399 chatbees_python_client-1.0.2/chatbees/tests/api_surface_test.py
+-rw-r--r--   0        0        0       39 2024-02-03 05:19:30.174160 chatbees_python_client-1.0.2/chatbees/tests/data/española.txt
+-rw-r--r--   0        0        0       32 2024-02-03 05:19:30.174268 chatbees_python_client-1.0.2/chatbees/tests/data/française.txt
+-rw-r--r--   0        0        0      463 2024-02-03 05:19:30.174378 chatbees_python_client-1.0.2/chatbees/tests/data/text_file.txt
+-rw-r--r--   0        0        0       30 2024-02-03 05:19:30.174477 chatbees_python_client-1.0.2/chatbees/tests/data/中文.txt
+-rw-r--r--   0        0        0     8508 2024-04-24 16:30:23.191208 chatbees_python_client-1.0.2/chatbees/tests/smoke_test.py
+-rw-r--r--   0        0        0        0 2024-02-03 05:19:30.174691 chatbees_python_client-1.0.2/chatbees/utils/__init__.py
+-rw-r--r--   0        0        0     1022 2024-02-06 18:39:33.176649 chatbees_python_client-1.0.2/chatbees/utils/ask.py
+-rw-r--r--   0        0        0     1638 2024-03-11 18:24:32.039859 chatbees_python_client-1.0.2/chatbees/utils/config.py
+-rw-r--r--   0        0        0     1709 2024-02-03 05:19:30.174998 chatbees_python_client-1.0.2/chatbees/utils/exceptions.py
+-rw-r--r--   0        0        0      729 2024-04-04 16:20:59.474400 chatbees_python_client-1.0.2/chatbees/utils/file_upload.py
+-rw-r--r--   0        0        0      477 2024-04-24 16:30:36.293201 chatbees_python_client-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6623 1970-01-01 00:00:00.000000 chatbees_python_client-1.0.2/PKG-INFO
```

### Comparing `chatbees_python_client-1.0.0/LICENSE` & `chatbees_python_client-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-1.0.0/README.md` & `chatbees_python_client-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # chatbees-python-client
 Python client for [ChatBees](http://www.chatbees.ai), a Serverless Platform for your LLM Apps. ChatBees provides simple and scalable APIs, enabling you to craft a LLM app for your knowledge base in mere minutes.
 
-ChatBees is currently in <ins>**public alpha**</ins>. We're actively improving 
-the product and releasing new features, and we'd love to hear your feedback! 
+We're actively improving the product and releasing new features, and we'd love to hear your feedback!
 Please take a moment to fill out this [feedback form](https://forms.gle/pif6Vx2LqPjW5v4w5) to help us understand your use-case better.
 
 Signup with your google account on https://www.chatbees.ai. You could also try it out in ChatBees public account without signup.
 
 > For the public account, by default, all collections are subject to permanent deletion after 2 weeks. Please let us know if you need to keep it for longer via the feedback form.
 
-ChatBees python client provides very simple APIs for you to directly upload files and ask questions.
+ChatBees python client provides very simple APIs for you to directly upload files, crawl websites, ingest data sources including Confluence, Notion and Google Drive. Then you can simply ask questions.
 
 
 ## Quickstart
 
 You can try out ChatBees in just a few lines of code. You can create your own collections, upload files, then get answers  specific to your data assets. The following example walks you through the process of creating a collection and indexing [the original transformer paper](https://arxiv.org/abs/1706.03762) into that collection.
 
 ```python
```

### Comparing `chatbees_python_client-1.0.0/chatbees/.DS_Store` & `chatbees_python_client-1.0.2/chatbees/.DS_Store`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-1.0.0/chatbees/client/admin_management.py` & `chatbees_python_client-1.0.2/chatbees/client/admin_management.py`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-1.0.0/chatbees/client/collection_management.py` & `chatbees_python_client-1.0.2/chatbees/client/collection_management.py`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-1.0.0/chatbees/client_models/chat.py` & `chatbees_python_client-1.0.2/chatbees/client_models/chat.py`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-1.0.0/chatbees/client_models/collection.py` & `chatbees_python_client-1.0.2/chatbees/client_models/collection.py`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-1.0.0/chatbees/server_models/chat.py` & `chatbees_python_client-1.0.2/chatbees/server_models/chat.py`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-1.0.0/chatbees/server_models/collection_api.py` & `chatbees_python_client-1.0.2/chatbees/server_models/collection_api.py`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-1.0.0/chatbees/server_models/doc_api.py` & `chatbees_python_client-1.0.2/chatbees/server_models/doc_api.py`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-1.0.0/chatbees/server_models/ingestion_api.py` & `chatbees_python_client-1.0.2/chatbees/server_models/ingestion_api.py`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-1.0.0/chatbees/tests/api_surface_test.py` & `chatbees_python_client-1.0.2/chatbees/tests/api_surface_test.py`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-1.0.0/chatbees/tests/smoke_test.py` & `chatbees_python_client-1.0.2/chatbees/tests/smoke_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,28 +118,28 @@
                 col.summarize_document(fname)
 
             # list
             print("list_documents")
             list_doc_names = col.list_documents()
             assert doc_names == set(list_doc_names)
 
-            # ask with top_k
+            # ask
             print("ask")
-            a, refs = col.ask('question?', 4)
-            assert 4 == len(refs)
+            a, refs = col.ask('question?')
+            assert len(refs) > 0
 
             # delete, then list and ask again
             col.delete_document('española.txt')
             doc_names = {'text_file.txt', 'française.txt', '中文.txt'}
 
             list_doc_names = col.list_documents()
             assert doc_names == set(list_doc_names)
 
-            a, refs = col.ask('question?', 4)
-            assert 4 == len(refs)
+            a, refs = col.ask('question?')
+            assert len(refs) > 0
 
             # chat
             chat1 = col.chat()
             chat2 = col.chat(doc_name="text_file.txt")
 
             chat1.ask("q1")
             chat1.ask("q2")
```

### Comparing `chatbees_python_client-1.0.0/chatbees/utils/ask.py` & `chatbees_python_client-1.0.2/chatbees/utils/ask.py`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-1.0.0/chatbees/utils/config.py` & `chatbees_python_client-1.0.2/chatbees/utils/config.py`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-1.0.0/chatbees/utils/exceptions.py` & `chatbees_python_client-1.0.2/chatbees/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-1.0.0/chatbees/utils/file_upload.py` & `chatbees_python_client-1.0.2/chatbees/utils/file_upload.py`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-1.0.0/PKG-INFO` & `chatbees_python_client-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatbees-python-client
-Version: 1.0.0
+Version: 1.0.2
 Summary: Python client for ChatBees
 Author: ChatBees
 Author-email: build@chatbees.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,23 +12,22 @@
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # chatbees-python-client
 Python client for [ChatBees](http://www.chatbees.ai), a Serverless Platform for your LLM Apps. ChatBees provides simple and scalable APIs, enabling you to craft a LLM app for your knowledge base in mere minutes.
 
-ChatBees is currently in <ins>**public alpha**</ins>. We're actively improving 
-the product and releasing new features, and we'd love to hear your feedback! 
+We're actively improving the product and releasing new features, and we'd love to hear your feedback!
 Please take a moment to fill out this [feedback form](https://forms.gle/pif6Vx2LqPjW5v4w5) to help us understand your use-case better.
 
 Signup with your google account on https://www.chatbees.ai. You could also try it out in ChatBees public account without signup.
 
 > For the public account, by default, all collections are subject to permanent deletion after 2 weeks. Please let us know if you need to keep it for longer via the feedback form.
 
-ChatBees python client provides very simple APIs for you to directly upload files and ask questions.
+ChatBees python client provides very simple APIs for you to directly upload files, crawl websites, ingest data sources including Confluence, Notion and Google Drive. Then you can simply ask questions.
 
 
 ## Quickstart
 
 You can try out ChatBees in just a few lines of code. You can create your own collections, upload files, then get answers  specific to your data assets. The following example walks you through the process of creating a collection and indexing [the original transformer paper](https://arxiv.org/abs/1706.03762) into that collection.
 
 ```python
```

