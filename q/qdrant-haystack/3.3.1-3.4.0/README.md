# Comparing `tmp/qdrant_haystack-3.3.1.tar.gz` & `tmp/qdrant_haystack-3.4.0.tar.gz`

## Comparing `qdrant_haystack-3.3.1.tar` & `qdrant_haystack-3.4.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.1/pydoc/config.yml
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.1/src/haystack_integrations/components/retrievers/qdrant/__init__.py
--rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.1/src/haystack_integrations/components/retrievers/qdrant/retriever.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.1/src/haystack_integrations/document_stores/qdrant/__init__.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.1/src/haystack_integrations/document_stores/qdrant/converters.py
--rw-r--r--   0        0        0    22943 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.1/src/haystack_integrations/document_stores/qdrant/document_store.py
--rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.1/src/haystack_integrations/document_stores/qdrant/filters.py
--rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.1/src/haystack_integrations/document_stores/qdrant/migrate_to_sparse.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.1/tests/__init__.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.1/tests/test_converters.py
--rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.1/tests/test_dict_converters.py
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.1/tests/test_document_store.py
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.1/tests/test_filters.py
--rw-r--r--   0        0        0    20208 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.1/tests/test_legacy_filters.py
--rw-r--r--   0        0        0    11065 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.1/tests/test_retriever.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.1/LICENSE.txt
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.1/README.md
--rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.1/pyproject.toml
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 qdrant_haystack-3.4.0/examples/embedding_retrieval.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 qdrant_haystack-3.4.0/pydoc/config.yml
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 qdrant_haystack-3.4.0/src/haystack_integrations/components/retrievers/qdrant/__init__.py
+-rw-r--r--   0        0        0     8853 2020-02-02 00:00:00.000000 qdrant_haystack-3.4.0/src/haystack_integrations/components/retrievers/qdrant/retriever.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 qdrant_haystack-3.4.0/src/haystack_integrations/document_stores/qdrant/__init__.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 qdrant_haystack-3.4.0/src/haystack_integrations/document_stores/qdrant/converters.py
+-rw-r--r--   0        0        0    22943 2020-02-02 00:00:00.000000 qdrant_haystack-3.4.0/src/haystack_integrations/document_stores/qdrant/document_store.py
+-rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 qdrant_haystack-3.4.0/src/haystack_integrations/document_stores/qdrant/filters.py
+-rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 qdrant_haystack-3.4.0/src/haystack_integrations/document_stores/qdrant/migrate_to_sparse.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 qdrant_haystack-3.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 qdrant_haystack-3.4.0/tests/test_converters.py
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 qdrant_haystack-3.4.0/tests/test_dict_converters.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 qdrant_haystack-3.4.0/tests/test_document_store.py
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 qdrant_haystack-3.4.0/tests/test_filters.py
+-rw-r--r--   0        0        0    20208 2020-02-02 00:00:00.000000 qdrant_haystack-3.4.0/tests/test_legacy_filters.py
+-rw-r--r--   0        0        0    11137 2020-02-02 00:00:00.000000 qdrant_haystack-3.4.0/tests/test_retriever.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 qdrant_haystack-3.4.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 qdrant_haystack-3.4.0/LICENSE.txt
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 qdrant_haystack-3.4.0/README.md
+-rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 qdrant_haystack-3.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 qdrant_haystack-3.4.0/PKG-INFO
```

### Comparing `qdrant_haystack-3.3.1/pydoc/config.yml` & `qdrant_haystack-3.4.0/pydoc/config.yml`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.3.1/src/haystack_integrations/components/retrievers/qdrant/retriever.py` & `qdrant_haystack-3.4.0/src/haystack_integrations/components/retrievers/qdrant/retriever.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,46 +120,46 @@
             return_embedding=return_embedding or self._return_embedding,
         )
 
         return {"documents": docs}
 
 
 @component
-class QdrantSparseRetriever:
+class QdrantSparseEmbeddingRetriever:
     """
     A component for retrieving documents from an QdrantDocumentStore using sparse vectors.
 
     Usage example:
     ```python
-    from haystack_integrations.components.retrievers.qdrant import QdrantSparseRetriever
+    from haystack_integrations.components.retrievers.qdrant import QdrantSparseEmbeddingRetriever
     from haystack_integrations.document_stores.qdrant import QdrantDocumentStore
     from haystack.dataclasses.sparse_embedding import SparseEmbedding
 
     document_store = QdrantDocumentStore(
         ":memory:",
         recreate_index=True,
         return_embedding=True,
         wait_result_from_api=True,
     )
-    retriever = QdrantSparseRetriever(document_store=document_store)
+    retriever = QdrantSparseEmbeddingRetriever(document_store=document_store)
     sparse_embedding = SparseEmbedding(indices=[0, 1, 2, 3], values=[0.1, 0.8, 0.05, 0.33])
     retriever.run(query_sparse_embedding=sparse_embedding)
     ```
     """
 
     def __init__(
         self,
         document_store: QdrantDocumentStore,
         filters: Optional[Dict[str, Any]] = None,
         top_k: int = 10,
         scale_score: bool = True,
         return_embedding: bool = False,
     ):
         """
-        Create a QdrantSparseRetriever component.
+        Create a QdrantSparseEmbeddingRetriever component.
 
         :param document_store: An instance of QdrantDocumentStore.
         :param filters: A dictionary with filters to narrow down the search space. Default is None.
         :param top_k: The maximum number of documents to retrieve. Default is 10.
         :param scale_score: Whether to scale the scores of the retrieved documents or not. Default is True.
         :param return_embedding: Whether to return the sparse embedding of the retrieved Documents. Default is False.
```

### Comparing `qdrant_haystack-3.3.1/src/haystack_integrations/document_stores/qdrant/converters.py` & `qdrant_haystack-3.4.0/src/haystack_integrations/document_stores/qdrant/converters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.3.1/src/haystack_integrations/document_stores/qdrant/document_store.py` & `qdrant_haystack-3.4.0/src/haystack_integrations/document_stores/qdrant/document_store.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.3.1/src/haystack_integrations/document_stores/qdrant/filters.py` & `qdrant_haystack-3.4.0/src/haystack_integrations/document_stores/qdrant/filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.3.1/src/haystack_integrations/document_stores/qdrant/migrate_to_sparse.py` & `qdrant_haystack-3.4.0/src/haystack_integrations/document_stores/qdrant/migrate_to_sparse.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.3.1/tests/test_converters.py` & `qdrant_haystack-3.4.0/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.3.1/tests/test_dict_converters.py` & `qdrant_haystack-3.4.0/tests/test_dict_converters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.3.1/tests/test_document_store.py` & `qdrant_haystack-3.4.0/tests/test_document_store.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.3.1/tests/test_filters.py` & `qdrant_haystack-3.4.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.3.1/tests/test_legacy_filters.py` & `qdrant_haystack-3.4.0/tests/test_legacy_filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.3.1/tests/test_retriever.py` & `qdrant_haystack-3.4.0/tests/test_retriever.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from haystack.dataclasses import Document, SparseEmbedding
 from haystack.testing.document_store import (
     FilterableDocsFixtureMixin,
     _random_embeddings,
 )
 from haystack_integrations.components.retrievers.qdrant import (
     QdrantEmbeddingRetriever,
-    QdrantSparseRetriever,
+    QdrantSparseEmbeddingRetriever,
 )
 from haystack_integrations.document_stores.qdrant import QdrantDocumentStore
 
 
 class TestQdrantRetriever(FilterableDocsFixtureMixin):
     def test_init_default(self):
         document_store = QdrantDocumentStore(location=":memory:", index="test", use_sparse_embeddings=False)
@@ -131,29 +131,29 @@
 
         assert len(results) == 5
 
         for document in results:
             assert document.embedding is None
 
 
-class TestQdrantSparseRetriever(FilterableDocsFixtureMixin):
+class TestQdrantSparseEmbeddingRetriever(FilterableDocsFixtureMixin):
     def test_init_default(self):
         document_store = QdrantDocumentStore(location=":memory:", index="test")
-        retriever = QdrantSparseRetriever(document_store=document_store)
+        retriever = QdrantSparseEmbeddingRetriever(document_store=document_store)
         assert retriever._document_store == document_store
         assert retriever._filters is None
         assert retriever._top_k == 10
         assert retriever._return_embedding is False
 
     def test_to_dict(self):
         document_store = QdrantDocumentStore(location=":memory:", index="test")
-        retriever = QdrantSparseRetriever(document_store=document_store)
+        retriever = QdrantSparseEmbeddingRetriever(document_store=document_store)
         res = retriever.to_dict()
         assert res == {
-            "type": "haystack_integrations.components.retrievers.qdrant.retriever.QdrantSparseRetriever",
+            "type": "haystack_integrations.components.retrievers.qdrant.retriever.QdrantSparseEmbeddingRetriever",
             "init_parameters": {
                 "document_store": {
                     "type": "haystack_integrations.document_stores.qdrant.document_store.QdrantDocumentStore",
                     "init_parameters": {
                         "location": ":memory:",
                         "url": None,
                         "port": 6333,
@@ -198,27 +198,27 @@
                 "scale_score": True,
                 "return_embedding": False,
             },
         }
 
     def test_from_dict(self):
         data = {
-            "type": "haystack_integrations.components.retrievers.qdrant.retriever.QdrantSparseRetriever",
+            "type": "haystack_integrations.components.retrievers.qdrant.retriever.QdrantSparseEmbeddingRetriever",
             "init_parameters": {
                 "document_store": {
                     "init_parameters": {"location": ":memory:", "index": "test"},
                     "type": "haystack_integrations.document_stores.qdrant.document_store.QdrantDocumentStore",
                 },
                 "filters": None,
                 "top_k": 5,
                 "scale_score": False,
                 "return_embedding": True,
             },
         }
-        retriever = QdrantSparseRetriever.from_dict(data)
+        retriever = QdrantSparseEmbeddingRetriever.from_dict(data)
         assert isinstance(retriever._document_store, QdrantDocumentStore)
         assert retriever._document_store.index == "test"
         assert retriever._filters is None
         assert retriever._top_k == 5
         assert retriever._scale_score is False
         assert retriever._return_embedding is True
 
@@ -237,15 +237,15 @@
         document_store = QdrantDocumentStore(location=":memory:", index="Boi", use_sparse_embeddings=True)
 
         # Add fake sparse embedding to documents
         for doc in filterable_docs:
             doc.sparse_embedding = SparseEmbedding.from_dict(self._generate_mocked_sparse_embedding(1)[0])
 
         document_store.write_documents(filterable_docs)
-        retriever = QdrantSparseRetriever(document_store=document_store)
+        retriever = QdrantSparseEmbeddingRetriever(document_store=document_store)
         sparse_embedding = SparseEmbedding(indices=[0, 1, 2, 3], values=[0.1, 0.8, 0.05, 0.33])
 
         results: List[Document] = retriever.run(query_sparse_embedding=sparse_embedding)["documents"]
         assert len(results) == 10
 
         results = retriever.run(query_sparse_embedding=sparse_embedding, top_k=5, return_embedding=True)["documents"]
         assert len(results) == 5
```

### Comparing `qdrant_haystack-3.3.1/.gitignore` & `qdrant_haystack-3.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.3.1/LICENSE.txt` & `qdrant_haystack-3.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.3.1/README.md` & `qdrant_haystack-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.3.1/pyproject.toml` & `qdrant_haystack-3.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -123,14 +123,16 @@
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "parents"
 
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
+# examples can contain "print" commands
+"examples/**/*" = ["T201"]
 
 
 [tool.coverage.run]
 source = ["haystack_integrations"]
 branch = true
 parallel = false
```

### Comparing `qdrant_haystack-3.3.1/PKG-INFO` & `qdrant_haystack-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: qdrant-haystack
-Version: 3.3.1
+Version: 3.4.0
 Summary: An integration of Qdrant ANN vector database backend with Haystack
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/blob/main/integrations/qdrant/README.md
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Author-email: Kacper Łukawski <kacper.lukawski@qdrant.com>, Anush Shetty <anush.shetty@qdrant.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```

