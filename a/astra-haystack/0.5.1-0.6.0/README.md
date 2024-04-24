# Comparing `tmp/astra_haystack-0.5.1.tar.gz` & `tmp/astra_haystack-0.6.0.tar.gz`

## Comparing `astra_haystack-0.5.1.tar` & `astra_haystack-0.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/__init__.py
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/examples/example.py
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/examples/pipeline_example.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/examples/requirements.txt
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/examples/data/usr_01.txt
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/pydoc/config.yml
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/src/haystack_integrations/components/retrievers/astra/__init__.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/src/haystack_integrations/components/retrievers/astra/retriever.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/src/haystack_integrations/document_stores/astra/__init__.py
--rw-r--r--   0        0        0    12893 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/src/haystack_integrations/document_stores/astra/astra_client.py
--rw-r--r--   0        0        0    17243 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/src/haystack_integrations/document_stores/astra/document_store.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/src/haystack_integrations/document_stores/astra/errors.py
--rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/src/haystack_integrations/document_stores/astra/filters.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0    10434 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/tests/test_document_store.py
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/tests/test_retriever.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/LICENSE
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/README.md
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/__init__.py
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/examples/example.py
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/examples/pipeline_example.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/examples/requirements.txt
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/examples/data/usr_01.txt
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/pydoc/config.yml
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/src/haystack_integrations/components/retrievers/astra/__init__.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/src/haystack_integrations/components/retrievers/astra/retriever.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/src/haystack_integrations/document_stores/astra/__init__.py
+-rw-r--r--   0        0        0    12893 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/src/haystack_integrations/document_stores/astra/astra_client.py
+-rw-r--r--   0        0        0    17620 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/src/haystack_integrations/document_stores/astra/document_store.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/src/haystack_integrations/document_stores/astra/errors.py
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/src/haystack_integrations/document_stores/astra/filters.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0    11745 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/tests/test_document_store.py
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/tests/test_retriever.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/README.md
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/PKG-INFO
```

### Comparing `astra_haystack-0.5.1/examples/example.py` & `astra_haystack-0.6.0/examples/example.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.1/examples/pipeline_example.py` & `astra_haystack-0.6.0/examples/pipeline_example.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.1/examples/data/usr_01.txt` & `astra_haystack-0.6.0/examples/data/usr_01.txt`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.1/pydoc/config.yml` & `astra_haystack-0.6.0/pydoc/config.yml`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.1/src/haystack_integrations/components/retrievers/astra/retriever.py` & `astra_haystack-0.6.0/src/haystack_integrations/components/retrievers/astra/retriever.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.1/src/haystack_integrations/document_stores/astra/astra_client.py` & `astra_haystack-0.6.0/src/haystack_integrations/document_stores/astra/astra_client.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.1/src/haystack_integrations/document_stores/astra/document_store.py` & `astra_haystack-0.6.0/src/haystack_integrations/document_stores/astra/document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         self,
         api_endpoint: Secret = Secret.from_env_var("ASTRA_DB_API_ENDPOINT"),  # noqa: B008
         token: Secret = Secret.from_env_var("ASTRA_DB_APPLICATION_TOKEN"),  # noqa: B008
         collection_name: str = "documents",
         embedding_dimension: int = 768,
         duplicates_policy: DuplicatePolicy = DuplicatePolicy.NONE,
         similarity: str = "cosine",
+        namespace: Optional[str] = None,
     ):
         """
         The connection to Astra DB is established and managed through the JSON API.
         The required credentials (api endpoint and application token) can be generated
         through the UI by clicking and the connect tab, and then selecting JSON API and
         Generate Configuration.
 
@@ -95,21 +96,23 @@
 
         self.api_endpoint = api_endpoint
         self.token = token
         self.collection_name = collection_name
         self.embedding_dimension = embedding_dimension
         self.duplicates_policy = duplicates_policy
         self.similarity = similarity
+        self.namespace = namespace
 
         self.index = AstraClient(
             resolved_api_endpoint,
             resolved_token,
             self.collection_name,
             self.embedding_dimension,
             self.similarity,
+            namespace,
         )
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "AstraDocumentStore":
         """
         Deserializes the component from a dictionary.
 
@@ -124,22 +127,24 @@
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
 
         :returns:
             Dictionary with serialized data.
         """
+
         return default_to_dict(
             self,
             api_endpoint=self.api_endpoint.to_dict(),
             token=self.token.to_dict(),
             collection_name=self.collection_name,
             embedding_dimension=self.embedding_dimension,
             duplicates_policy=self.duplicates_policy.name,
             similarity=self.similarity,
+            namespace=self.namespace,
         )
 
     def write_documents(
         self,
         documents: List[Document],
         policy: DuplicatePolicy = DuplicatePolicy.NONE,
     ):
@@ -206,20 +211,23 @@
                     )
 
             return document_dict
 
         documents_to_write = [_convert_input_document(doc) for doc in documents]
 
         duplicate_documents = []
-        new_documents = []
+        new_documents: List[Document] = []
         i = 0
         while i < len(documents_to_write):
             doc = documents_to_write[i]
+            # check to see if this ID already exists in our new_documents array
+            exists = [d for d in new_documents if d["_id"] == doc["_id"]]
+            # check to see if this ID is already in the DB
             response = self.index.find_documents({"filter": {"_id": doc["_id"]}})
-            if response:
+            if response or exists:
                 if policy == DuplicatePolicy.FAIL:
                     msg = f"ID '{doc['_id']}' already exists."
                     raise DuplicateDocumentError(msg)
                 duplicate_documents.append(doc)
             else:
                 new_documents.append(doc)
             i = i + 1
```

### Comparing `astra_haystack-0.5.1/src/haystack_integrations/document_stores/astra/errors.py` & `astra_haystack-0.6.0/src/haystack_integrations/document_stores/astra/errors.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.1/src/haystack_integrations/document_stores/astra/filters.py` & `astra_haystack-0.6.0/src/haystack_integrations/document_stores/astra/filters.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.1/tests/test_document_store.py` & `astra_haystack-0.6.0/tests/test_document_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,50 @@
 # SPDX-FileCopyrightText: 2023-present Anant Corporation <support@anant.us>
 #
 # SPDX-License-Identifier: Apache-2.0
 import os
 from typing import List
+from unittest import mock
 
 import pytest
 from haystack import Document
 from haystack.document_stores.errors import MissingDocumentError
 from haystack.document_stores.types import DuplicatePolicy
 from haystack.testing.document_store import DocumentStoreBaseTests
 
 from haystack_integrations.document_stores.astra import AstraDocumentStore
 
 
+def test_namespace_init():
+    with mock.patch("haystack_integrations.document_stores.astra.astra_client.AstraDB") as client:
+        AstraDocumentStore()
+        assert "namespace" in client.call_args.kwargs
+        assert client.call_args.kwargs["namespace"] is None
+
+        AstraDocumentStore(namespace="foo")
+        assert "namespace" in client.call_args.kwargs
+        assert client.call_args.kwargs["namespace"] == "foo"
+
+
+def test_to_dict():
+    with mock.patch("haystack_integrations.document_stores.astra.astra_client.AstraDB"):
+        ds = AstraDocumentStore()
+        result = ds.to_dict()
+        assert result["type"] == "haystack_integrations.document_stores.astra.document_store.AstraDocumentStore"
+        assert set(result["init_parameters"]) == {
+            "api_endpoint",
+            "token",
+            "collection_name",
+            "embedding_dimension",
+            "duplicates_policy",
+            "similarity",
+            "namespace",
+        }
+
+
 @pytest.mark.integration
 @pytest.mark.skipif(
     os.environ.get("ASTRA_DB_APPLICATION_TOKEN", "") == "", reason="ASTRA_DB_APPLICATION_TOKEN env var not set"
 )
 @pytest.mark.skipif(os.environ.get("ASTRA_DB_API_ENDPOINT", "") == "", reason="ASTRA_DB_API_ENDPOINT env var not set")
 class TestDocumentStore(DocumentStoreBaseTests):
     """
@@ -70,14 +98,21 @@
         doc2 = Document(id="1", content="test doc 2")
 
         assert document_store.write_documents([doc2], policy=DuplicatePolicy.OVERWRITE) == 1
         self.assert_documents_are_equal(document_store.filter_documents(), [doc2])
         assert document_store.write_documents(documents=[doc1], policy=DuplicatePolicy.OVERWRITE) == 1
         self.assert_documents_are_equal(document_store.filter_documents(), [doc1])
 
+    def test_write_documents_skip_duplicates(self, document_store: AstraDocumentStore):
+        docs = [
+            Document(id="1", content="test doc 1"),
+            Document(id="1", content="test doc 2"),
+        ]
+        assert document_store.write_documents(docs, policy=DuplicatePolicy.SKIP) == 1
+
     def test_delete_documents_non_existing_document(self, document_store: AstraDocumentStore):
         """
         Test delete_documents() doesn't delete any Document when called with non existing id.
         """
         doc = Document(content="test doc")
         document_store.write_documents([doc])
         assert document_store.count_documents() == 1
```

### Comparing `astra_haystack-0.5.1/tests/test_retriever.py` & `astra_haystack-0.6.0/tests/test_retriever.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,27 +26,27 @@
                 "init_parameters": {
                     "api_endpoint": {"type": "env_var", "env_vars": ["ASTRA_DB_API_ENDPOINT"], "strict": True},
                     "token": {"type": "env_var", "env_vars": ["ASTRA_DB_APPLICATION_TOKEN"], "strict": True},
                     "collection_name": "documents",
                     "embedding_dimension": 768,
                     "duplicates_policy": "NONE",
                     "similarity": "cosine",
+                    "namespace": None,
                 },
             },
         },
     }
 
 
 @patch.dict(
     "os.environ",
     {"ASTRA_DB_APPLICATION_TOKEN": "fake-token", "ASTRA_DB_API_ENDPOINT": "http://fake-url.apps.astra.datastax.com"},
 )
 @patch("haystack_integrations.document_stores.astra.document_store.AstraClient")
 def test_retriever_from_json(*_):
-
     data = {
         "type": "haystack_integrations.components.retrievers.astra.retriever.AstraEmbeddingRetriever",
         "init_parameters": {
             "filters": {"bar": "baz"},
             "top_k": 42,
             "document_store": {
                 "type": "haystack_integrations.document_stores.astra.document_store.AstraDocumentStore",
```

### Comparing `astra_haystack-0.5.1/.gitignore` & `astra_haystack-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.1/LICENSE` & `astra_haystack-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.1/README.md` & `astra_haystack-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.1/pyproject.toml` & `astra_haystack-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "Anant Corporation", email = "support@anant.us" },
 ]
 classifiers = [
+  "License :: OSI Approved :: Apache Software License",
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `astra_haystack-0.5.1/PKG-INFO` & `astra_haystack-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.3
 Name: astra-haystack
-Version: 0.5.1
+Version: 0.6.0
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/astra#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/astra
 Author-email: Anant Corporation <support@anant.us>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

