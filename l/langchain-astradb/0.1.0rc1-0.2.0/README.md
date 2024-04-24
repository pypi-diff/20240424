# Comparing `tmp/langchain_astradb-0.1.0rc1.tar.gz` & `tmp/langchain_astradb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_astradb-0.1.0rc1.tar", max compression
+gzip compressed data, was "langchain_astradb-0.2.0.tar", max compression
```

## Comparing `langchain_astradb-0.1.0rc1.tar` & `langchain_astradb-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2024-03-14 08:59:36.818380 langchain_astradb-0.1.0rc1/LICENSE
--rw-r--r--   0        0        0     1715 2024-03-14 08:59:36.818380 langchain_astradb-0.1.0rc1/README.md
--rw-r--r--   0        0        0      529 2024-03-14 08:59:36.818380 langchain_astradb-0.1.0rc1/langchain_astradb/__init__.py
--rw-r--r--   0        0        0    20613 2024-03-14 08:59:36.818380 langchain_astradb-0.1.0rc1/langchain_astradb/cache.py
--rw-r--r--   0        0        0     5344 2024-03-14 08:59:36.818380 langchain_astradb-0.1.0rc1/langchain_astradb/chat_message_histories.py
--rw-r--r--   0        0        0     4311 2024-03-14 08:59:36.818380 langchain_astradb-0.1.0rc1/langchain_astradb/document_loaders.py
--rw-r--r--   0        0        0        0 2024-03-14 08:59:36.818380 langchain_astradb-0.1.0rc1/langchain_astradb/py.typed
--rw-r--r--   0        0        0     8737 2024-03-14 08:59:36.818380 langchain_astradb-0.1.0rc1/langchain_astradb/storage.py
--rw-r--r--   0        0        0    13501 2024-03-14 08:59:36.818380 langchain_astradb-0.1.0rc1/langchain_astradb/utils/astradb.py
--rw-r--r--   0        0        0     3165 2024-03-14 08:59:36.818380 langchain_astradb-0.1.0rc1/langchain_astradb/utils/mmr.py
--rw-r--r--   0        0        0    50848 2024-03-14 08:59:36.818380 langchain_astradb-0.1.0rc1/langchain_astradb/vectorstores.py
--rw-r--r--   0        0        0     2392 2024-03-14 08:59:36.822380 langchain_astradb-0.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0     2588 1970-01-01 00:00:00.000000 langchain_astradb-0.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-24 09:08:50.481561 langchain_astradb-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2058 2024-04-24 09:08:50.481561 langchain_astradb-0.2.0/README.md
+-rw-r--r--   0        0        0      529 2024-04-24 09:08:50.481561 langchain_astradb-0.2.0/langchain_astradb/__init__.py
+-rw-r--r--   0        0        0    20613 2024-04-24 09:08:50.485561 langchain_astradb-0.2.0/langchain_astradb/cache.py
+-rw-r--r--   0        0        0     5344 2024-04-24 09:08:50.485561 langchain_astradb-0.2.0/langchain_astradb/chat_message_histories.py
+-rw-r--r--   0        0        0     4311 2024-04-24 09:08:50.485561 langchain_astradb-0.2.0/langchain_astradb/document_loaders.py
+-rw-r--r--   0        0        0        0 2024-04-24 09:08:50.485561 langchain_astradb-0.2.0/langchain_astradb/py.typed
+-rw-r--r--   0        0        0     8737 2024-04-24 09:08:50.485561 langchain_astradb-0.2.0/langchain_astradb/storage.py
+-rw-r--r--   0        0        0    13501 2024-04-24 09:08:50.485561 langchain_astradb-0.2.0/langchain_astradb/utils/astradb.py
+-rw-r--r--   0        0        0     3165 2024-04-24 09:08:50.485561 langchain_astradb-0.2.0/langchain_astradb/utils/mmr.py
+-rw-r--r--   0        0        0    50645 2024-04-24 09:08:50.485561 langchain_astradb-0.2.0/langchain_astradb/vectorstores.py
+-rw-r--r--   0        0        0     2692 2024-04-24 09:08:50.485561 langchain_astradb-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2920 1970-01-01 00:00:00.000000 langchain_astradb-0.2.0/PKG-INFO
```

### Comparing `langchain_astradb-0.1.0rc1/LICENSE` & `langchain_astradb-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.1.0rc1/README.md` & `langchain_astradb-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,102 @@
 # langchain-astradb
 
 This package contains the LangChain integrations for using DataStax Astra DB.
 
 > DataStax [Astra DB](https://docs.datastax.com/en/astra/home/astra.html) is a serverless vector-capable database built on Apache Cassandra® and made conveniently available
 > through an easy-to-use JSON API.
 
-_**Note.** For a short transitional period, only some of the Astra DB integration classes are contained in this package (the remaining ones being still in `langchain-community`). In a short while, and surely by version 0.2 of LangChain, all of the Astra DB support will be removed from `langchain-community` and included in this package._
-
 ## Installation and Setup
 
 Installation of this partner package:
 
 ```bash
 pip install langchain-astradb
 ```
 
 ## Integrations overview
 
+See the [LangChain docs page](https://python.langchain.com/docs/integrations/providers/astradb) and the [API reference](https://api.python.langchain.com/en/latest/astradb_api_reference.html) for more details.
+
 ### Vector Store
 
 ```python
 from langchain_astradb import AstraDBVectorStore
 
 my_store = AstraDBVectorStore(
-  embedding=my_embeddings,
+  embedding=my_embedding,
   collection_name="my_store",
   api_endpoint="https://...",
   token="AstraCS:...",
 )
 ```
 
 ### Chat message history
 
 ```python
 from langchain_astradb import AstraDBChatMessageHistory
+
 message_history = AstraDBChatMessageHistory(
     session_id="test-session",
-    api_endpoint="...",
-    token="...",
+    api_endpoint="https://...",
+    token="AstraCS:...",
+)
+```
+
+## LLM Cache
+
+```python
+from langchain_astradb import AstraDBCache
+
+cache = AstraDBCache(
+    api_endpoint="https://...",
+    token="AstraCS:...",
+)
+```
+
+## Semantic LLM Cache
+
+```python
+from langchain_astradb import AstraDBSemanticCache
+
+cache = AstraDBSemanticCache(
+    embedding=my_embedding,
+    api_endpoint="https://...",
+    token="AstraCS:...",
+)
+```
+
+## Document loader
+
+```python
+from langchain_astradb import AstraDBLoader
+
+loader = AstraDBLoader(
+    collection_name="my_collection",
+    api_endpoint="https://...",
+    token="AstraCS:...",
 )
 ```
 
 ### Store
 
 ```python
 from langchain_astradb import AstraDBStore
+
 store = AstraDBStore(
     collection_name="my_kv_store",
-    api_endpoint="...",
-    token="..."
+    api_endpoint="https://...",
+    token="AstraCS:...",
 )
 ```
 
 ### Byte Store
 
 ```python
 from langchain_astradb import AstraDBByteStore
+
 store = AstraDBByteStore(
     collection_name="my_kv_store",
-    api_endpoint="...",
-    token="..."
+    api_endpoint="https://...",
+    token="AstraCS:...",
 )
 ```
-
-## Reference
-
-See the [LangChain docs page](https://python.langchain.com/docs/integrations/providers/astradb) for a more detailed listing.
```

### Comparing `langchain_astradb-0.1.0rc1/langchain_astradb/__init__.py` & `langchain_astradb-0.2.0/langchain_astradb/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.1.0rc1/langchain_astradb/cache.py` & `langchain_astradb-0.2.0/langchain_astradb/cache.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.1.0rc1/langchain_astradb/chat_message_histories.py` & `langchain_astradb-0.2.0/langchain_astradb/chat_message_histories.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.1.0rc1/langchain_astradb/document_loaders.py` & `langchain_astradb-0.2.0/langchain_astradb/document_loaders.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.1.0rc1/langchain_astradb/storage.py` & `langchain_astradb-0.2.0/langchain_astradb/storage.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.1.0rc1/langchain_astradb/utils/astradb.py` & `langchain_astradb-0.2.0/langchain_astradb/utils/astradb.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.1.0rc1/langchain_astradb/utils/mmr.py` & `langchain_astradb-0.2.0/langchain_astradb/utils/mmr.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.1.0rc1/langchain_astradb/vectorstores.py` & `langchain_astradb-0.2.0/langchain_astradb/vectorstores.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,26 +293,21 @@
             )
         return self.embedding_dimension
 
     @property
     def embeddings(self) -> Embeddings:
         return self.embedding
 
-    @staticmethod
-    def _dont_flip_the_cos_score(similarity0to1: float) -> float:
-        """Keep similarity from client unchanged ad it's in [0:1] already."""
-        return similarity0to1
-
     def _select_relevance_score_fn(self) -> Callable[[float], float]:
         """
         The underlying API calls already returns a "score proper",
         i.e. one in [0, 1] where higher means more *similar*,
         so here the final score transformation is not reversing the interval:
         """
-        return self._dont_flip_the_cos_score
+        return lambda score: score
 
     def clear(self) -> None:
         """Empty the collection of all its stored entries."""
         self.astra_env.ensure_db_setup()
         self.collection.delete_many({})
 
     async def aclear(self) -> None:
```

### Comparing `langchain_astradb-0.1.0rc1/pyproject.toml` & `langchain_astradb-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 [tool.poetry]
 name = "langchain-astradb"
-version = "0.1.0rc1"
+version = "0.2.0"
 description = "An integration package connecting Astra DB and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-datastax"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain-datastax/tree/main/libs/astradb"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 langchain-core = "^0.1.31"
-astrapy = "^0.7.7"
+astrapy = "^1"
 numpy = "^1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 pytest-dotenv = "^0.5.2"
 freezegun = "^1.2.2"
 pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
 langchain = "^0.1.9"
+langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
 
@@ -45,19 +46,21 @@
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
 
 [tool.poetry.group.typing.dependencies]
 mypy = "^0.991"
+langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
+langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
 
 [tool.ruff]
 select = [
   "E", # pycodestyle
   "F", # pyflakes
   "I", # isort
 ]
@@ -78,15 +81,15 @@
 #
 # https://docs.pytest.org/en/7.1.x/reference/reference.html
 # --strict-config       any warnings encountered while parsing the `pytest`
 #                       section of the configuration file raise errors.
 #
 # https://github.com/tophat/syrupy
 # --snapshot-warn-unused    Prints a warning on unused snapshots rather than fail the test suite.
-addopts = "--snapshot-warn-unused --strict-markers --strict-config --durations=5"
+addopts = "--snapshot-warn-unused --strict-markers --strict-config --durations=5 -vv"
 # Registering custom markers.
 # https://docs.pytest.org/en/7.1.x/example/markers.html#registering-markers
 markers = [
   "requires: mark tests as requiring a specific library",
   "asyncio: mark tests as requiring asyncio",
   "compile: mark placeholder test used to compile integration tests without running them",
 ]
```

### Comparing `langchain_astradb-0.1.0rc1/PKG-INFO` & `langchain_astradb-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,89 +1,123 @@
 Metadata-Version: 2.1
 Name: langchain-astradb
-Version: 0.1.0rc1
+Version: 0.2.0
 Summary: An integration package connecting Astra DB and LangChain
 Home-page: https://github.com/langchain-ai/langchain-datastax
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: astrapy (>=0.7.7,<0.8.0)
+Requires-Dist: astrapy (>=1,<2)
 Requires-Dist: langchain-core (>=0.1.31,<0.2.0)
 Requires-Dist: numpy (>=1,<2)
 Project-URL: Repository, https://github.com/langchain-ai/langchain-datastax
 Project-URL: Source Code, https://github.com/langchain-ai/langchain-datastax/tree/main/libs/astradb
 Description-Content-Type: text/markdown
 
 # langchain-astradb
 
 This package contains the LangChain integrations for using DataStax Astra DB.
 
 > DataStax [Astra DB](https://docs.datastax.com/en/astra/home/astra.html) is a serverless vector-capable database built on Apache Cassandra® and made conveniently available
 > through an easy-to-use JSON API.
 
-_**Note.** For a short transitional period, only some of the Astra DB integration classes are contained in this package (the remaining ones being still in `langchain-community`). In a short while, and surely by version 0.2 of LangChain, all of the Astra DB support will be removed from `langchain-community` and included in this package._
-
 ## Installation and Setup
 
 Installation of this partner package:
 
 ```bash
 pip install langchain-astradb
 ```
 
 ## Integrations overview
 
+See the [LangChain docs page](https://python.langchain.com/docs/integrations/providers/astradb) and the [API reference](https://api.python.langchain.com/en/latest/astradb_api_reference.html) for more details.
+
 ### Vector Store
 
 ```python
 from langchain_astradb import AstraDBVectorStore
 
 my_store = AstraDBVectorStore(
-  embedding=my_embeddings,
+  embedding=my_embedding,
   collection_name="my_store",
   api_endpoint="https://...",
   token="AstraCS:...",
 )
 ```
 
 ### Chat message history
 
 ```python
 from langchain_astradb import AstraDBChatMessageHistory
+
 message_history = AstraDBChatMessageHistory(
     session_id="test-session",
-    api_endpoint="...",
-    token="...",
+    api_endpoint="https://...",
+    token="AstraCS:...",
+)
+```
+
+## LLM Cache
+
+```python
+from langchain_astradb import AstraDBCache
+
+cache = AstraDBCache(
+    api_endpoint="https://...",
+    token="AstraCS:...",
+)
+```
+
+## Semantic LLM Cache
+
+```python
+from langchain_astradb import AstraDBSemanticCache
+
+cache = AstraDBSemanticCache(
+    embedding=my_embedding,
+    api_endpoint="https://...",
+    token="AstraCS:...",
+)
+```
+
+## Document loader
+
+```python
+from langchain_astradb import AstraDBLoader
+
+loader = AstraDBLoader(
+    collection_name="my_collection",
+    api_endpoint="https://...",
+    token="AstraCS:...",
 )
 ```
 
 ### Store
 
 ```python
 from langchain_astradb import AstraDBStore
+
 store = AstraDBStore(
     collection_name="my_kv_store",
-    api_endpoint="...",
-    token="..."
+    api_endpoint="https://...",
+    token="AstraCS:...",
 )
 ```
 
 ### Byte Store
 
 ```python
 from langchain_astradb import AstraDBByteStore
+
 store = AstraDBByteStore(
     collection_name="my_kv_store",
-    api_endpoint="...",
-    token="..."
+    api_endpoint="https://...",
+    token="AstraCS:...",
 )
 ```
 
-## Reference
-
-See the [LangChain docs page](https://python.langchain.com/docs/integrations/providers/astradb) for a more detailed listing.
-
```

