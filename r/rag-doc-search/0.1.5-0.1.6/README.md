# Comparing `tmp/rag_doc_search-0.1.5.tar.gz` & `tmp/rag_doc_search-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rag_doc_search-0.1.5.tar", max compression
+gzip compressed data, was "rag_doc_search-0.1.6.tar", max compression
```

## Comparing `rag_doc_search-0.1.5.tar` & `rag_doc_search-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     3303 2024-04-15 11:58:43.574400 rag_doc_search-0.1.5/README.md
--rw-r--r--   0        0        0      675 2024-04-15 11:57:41.852052 rag_doc_search-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1692 2024-04-09 09:50:20.319082 rag_doc_search-0.1.5/rag_doc_search/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 06:19:39.064794 rag_doc_search-0.1.5/rag_doc_search/src/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 06:19:39.066001 rag_doc_search-0.1.5/rag_doc_search/src/bot_models/__init__.py
--rw-r--r--   0        0        0     2991 2024-04-15 11:57:02.681552 rag_doc_search-0.1.5/rag_doc_search/src/bot_models/azure_chatbot_model.py
--rw-r--r--   0        0        0     3265 2024-03-07 06:31:57.292277 rag_doc_search-0.1.5/rag_doc_search/src/bot_models/bedrock_chatbot_model.py
--rw-r--r--   0        0        0     4691 2024-04-15 11:49:29.070013 rag_doc_search-0.1.5/rag_doc_search/src/bot_models/chatbot_model.py
--rw-r--r--   0        0        0     2463 2024-04-09 09:50:20.320028 rag_doc_search-0.1.5/rag_doc_search/src/bot_models/openai_chatbot_model.py
--rw-r--r--   0        0        0        0 2024-03-05 06:19:39.069930 rag_doc_search-0.1.5/rag_doc_search/src/enums/__init__.py
--rw-r--r--   0        0        0      657 2024-04-09 09:50:20.320782 rag_doc_search-0.1.5/rag_doc_search/src/enums/provider.py
--rw-r--r--   0        0        0      530 2024-03-05 06:19:39.072113 rag_doc_search-0.1.5/rag_doc_search/src/enums/search_type.py
--rw-r--r--   0        0        0        0 2024-03-05 06:19:39.072542 rag_doc_search-0.1.5/rag_doc_search/src/models/__init__.py
--rw-r--r--   0        0        0      583 2024-03-05 06:19:39.074318 rag_doc_search-0.1.5/rag_doc_search/src/models/chat_response.py
--rw-r--r--   0        0        0      215 2024-03-05 06:19:39.074627 rag_doc_search-0.1.5/rag_doc_search/src/models/user_prompt.py
--rw-r--r--   0        0        0      578 2024-03-05 06:19:39.075688 rag_doc_search-0.1.5/rag_doc_search/src/prompt_templates/default_prompt_templates.py
--rw-r--r--   0        0        0        0 2024-03-05 06:19:39.047879 rag_doc_search-0.1.5/rag_doc_search/utils/__init__.py
--rw-r--r--   0        0        0      945 2024-03-07 06:31:57.296465 rag_doc_search-0.1.5/rag_doc_search/utils/callback.py
--rw-r--r--   0        0        0    14038 2024-04-15 11:37:44.195295 rag_doc_search-0.1.5/rag_doc_search/utils/config.py
--rw-r--r--   0        0        0     2318 2024-03-05 06:19:39.052900 rag_doc_search-0.1.5/rag_doc_search/utils/miscellaneous.py
--rw-r--r--   0        0        0     4292 1970-01-01 00:00:00.000000 rag_doc_search-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     3303 2024-04-24 12:39:35.747312 rag_doc_search-0.1.6/README.md
+-rw-r--r--   0        0        0      675 2024-04-24 12:40:06.521215 rag_doc_search-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1692 2024-04-09 09:50:20.319082 rag_doc_search-0.1.6/rag_doc_search/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-05 06:19:39.064794 rag_doc_search-0.1.6/rag_doc_search/src/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-05 06:19:39.066001 rag_doc_search-0.1.6/rag_doc_search/src/bot_models/__init__.py
+-rw-r--r--   0        0        0     2991 2024-04-15 11:57:02.681552 rag_doc_search-0.1.6/rag_doc_search/src/bot_models/azure_chatbot_model.py
+-rw-r--r--   0        0        0     3265 2024-03-07 06:31:57.292277 rag_doc_search-0.1.6/rag_doc_search/src/bot_models/bedrock_chatbot_model.py
+-rw-r--r--   0        0        0     4691 2024-04-24 12:39:35.748041 rag_doc_search-0.1.6/rag_doc_search/src/bot_models/chatbot_model.py
+-rw-r--r--   0        0        0     2463 2024-04-09 09:50:20.320028 rag_doc_search-0.1.6/rag_doc_search/src/bot_models/openai_chatbot_model.py
+-rw-r--r--   0        0        0        0 2024-03-05 06:19:39.069930 rag_doc_search-0.1.6/rag_doc_search/src/enums/__init__.py
+-rw-r--r--   0        0        0      657 2024-04-09 09:50:20.320782 rag_doc_search-0.1.6/rag_doc_search/src/enums/provider.py
+-rw-r--r--   0        0        0      530 2024-03-05 06:19:39.072113 rag_doc_search-0.1.6/rag_doc_search/src/enums/search_type.py
+-rw-r--r--   0        0        0        0 2024-03-05 06:19:39.072542 rag_doc_search-0.1.6/rag_doc_search/src/models/__init__.py
+-rw-r--r--   0        0        0      583 2024-03-05 06:19:39.074318 rag_doc_search-0.1.6/rag_doc_search/src/models/chat_response.py
+-rw-r--r--   0        0        0      215 2024-03-05 06:19:39.074627 rag_doc_search-0.1.6/rag_doc_search/src/models/user_prompt.py
+-rw-r--r--   0        0        0      578 2024-03-05 06:19:39.075688 rag_doc_search-0.1.6/rag_doc_search/src/prompt_templates/default_prompt_templates.py
+-rw-r--r--   0        0        0        0 2024-03-05 06:19:39.047879 rag_doc_search-0.1.6/rag_doc_search/utils/__init__.py
+-rw-r--r--   0        0        0      945 2024-03-07 06:31:57.296465 rag_doc_search-0.1.6/rag_doc_search/utils/callback.py
+-rw-r--r--   0        0        0    13546 2024-04-24 12:39:53.863413 rag_doc_search-0.1.6/rag_doc_search/utils/config.py
+-rw-r--r--   0        0        0     2318 2024-03-05 06:19:39.052900 rag_doc_search-0.1.6/rag_doc_search/utils/miscellaneous.py
+-rw-r--r--   0        0        0     4292 1970-01-01 00:00:00.000000 rag_doc_search-0.1.6/PKG-INFO
```

### Comparing `rag_doc_search-0.1.5/README.md` & `rag_doc_search-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.5/pyproject.toml` & `rag_doc_search-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rag-doc-search"
-version = "0.1.5"
+version = "0.1.6"
 description = "This package offers a lightweight and straightforward solution for implementing Retrieval-augmented generation (RAG) functionality with large language models (LLMs)."
 authors = ["Harshad Kadam <harshad.kadam@sourcefuse.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 boto3 = "^1.34.55"
```

### Comparing `rag_doc_search-0.1.5/rag_doc_search/__init__.py` & `rag_doc_search-0.1.6/rag_doc_search/__init__.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.5/rag_doc_search/src/bot_models/azure_chatbot_model.py` & `rag_doc_search-0.1.6/rag_doc_search/src/bot_models/azure_chatbot_model.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.5/rag_doc_search/src/bot_models/bedrock_chatbot_model.py` & `rag_doc_search-0.1.6/rag_doc_search/src/bot_models/bedrock_chatbot_model.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.5/rag_doc_search/src/bot_models/chatbot_model.py` & `rag_doc_search-0.1.6/rag_doc_search/src/bot_models/chatbot_model.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.5/rag_doc_search/src/bot_models/openai_chatbot_model.py` & `rag_doc_search-0.1.6/rag_doc_search/src/bot_models/openai_chatbot_model.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.5/rag_doc_search/src/enums/provider.py` & `rag_doc_search-0.1.6/rag_doc_search/src/enums/provider.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.5/rag_doc_search/src/enums/search_type.py` & `rag_doc_search-0.1.6/rag_doc_search/src/enums/search_type.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.5/rag_doc_search/src/models/chat_response.py` & `rag_doc_search-0.1.6/rag_doc_search/src/models/chat_response.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.5/rag_doc_search/src/prompt_templates/default_prompt_templates.py` & `rag_doc_search-0.1.6/rag_doc_search/src/prompt_templates/default_prompt_templates.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.5/rag_doc_search/utils/callback.py` & `rag_doc_search-0.1.6/rag_doc_search/utils/callback.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.5/rag_doc_search/utils/config.py` & `rag_doc_search-0.1.6/rag_doc_search/utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,39 +68,31 @@
                     )
                 if not os.environ.get("AZURE_OPENAI_ENDPOINT"):
                     raise ValueError(
                         "AZURE_OPENAI_ENDPOINT environment variable is required for Azure OpenAI"
                     )
                 if not os.environ.get("AZURE_OPENAI_API_VERSION"):
                     os.environ["AZURE_OPENAI_API_VERSION"] = "2023-05-15"
-                    print( os.environ.get("AZURE_OPENAI_API_VERSION") )
                     self.logger.warning(
                         'AZURE_OPENAI_API_VERSION key not found in enviroment variables, so "2023-05-15" will be used as default value.'
                     )
-                    print(
-                        'AZURE_OPENAI_API_VERSION key not found in enviroment variables, so "2023-05-15" will be used as default value.'
-                    )
 
             case AIProvider.BEDROCK:
                 if not os.environ.get("AWS_ACCESS_KEY") or not os.environ.get(
                     "AWS_SECRET_ACCESS_KEY"
                 ):
                     raise ValueError(
                         "AWS_ACCESS_KEY and AWS_SECRET_ACCESS_KEY environment variables are required for Bedrock"
                     )
 
                 if not os.environ.get("AWS_REGION"):
                     os.environ["AWS_REGION"] = "us-east-1"
-                    print( os.environ.get("AWS_REGION") )
                     self.logger.warning(
                         'AWS_REGION key not found in enviroment variables, so "us-east-1" will be used as default value.'
                     )
-                    print(
-                        'AWS_REGION key not found in enviroment variables, so "us-east-1" will be used as default value.'
-                    )
             case _:
                 self.logger.warning("Default case AIProvider")
 
     def _validate_and_initialize_vector_store_provider(self, config_json: dict):
         """
         Validates and initializes the vector store provider based on the configuration JSON.
         Also validates and initializes vector store config properties and checks required environment variables as per provider.
@@ -265,15 +257,15 @@
                         database=os.environ.get("PGVECTOR_DATABASE", "postgres"),
                         user=os.environ.get("PGVECTOR_USER", "postgres"),
                         password=os.environ.get("PGVECTOR_PASSWORD", "postgres"),
                     )
                     self.vector_store = PGVector(
                         collection_name="city_bot",
                         connection_string=CONNECTION_STRING,
-                        embedding_function=self.embeddings,
+                        embedding_function=embeddings,
                     )
                     self.vector_store.as_retriever
                 case _:
                     self.logger.warning("Default case VectorStoreProvider")
         return self.vector_store
 
     def get_retriever_args(self) -> dict:
```

### Comparing `rag_doc_search-0.1.5/rag_doc_search/utils/miscellaneous.py` & `rag_doc_search-0.1.6/rag_doc_search/utils/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.5/PKG-INFO` & `rag_doc_search-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag-doc-search
-Version: 0.1.5
+Version: 0.1.6
 Summary: This package offers a lightweight and straightforward solution for implementing Retrieval-augmented generation (RAG) functionality with large language models (LLMs).
 Author: Harshad Kadam
 Author-email: harshad.kadam@sourcefuse.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

