# Comparing `tmp/amazon_bedrock_haystack-0.7.0.tar.gz` & `tmp/amazon_bedrock_haystack-0.7.1.tar.gz`

## Comparing `amazon_bedrock_haystack-0.7.0.tar` & `amazon_bedrock_haystack-0.7.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rwxr-xr-x   0        0        0     1444 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/examples/chatgenerator_example.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/examples/embedders_generator_with_rag_example.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/pydoc/config.yml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/common/amazon_bedrock/__init__.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/common/amazon_bedrock/errors.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/common/amazon_bedrock/utils.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/embedders/amazon_bedrock/__init__.py
--rw-r--r--   0        0        0    12587 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/embedders/amazon_bedrock/document_embedder.py
--rw-r--r--   0        0        0     8479 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/embedders/amazon_bedrock/text_embedder.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/__init__.py
--rw-r--r--   0        0        0    13329 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/adapters.py
--rw-r--r--   0        0        0    12287 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/generator.py
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/handlers.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/chat/__init__.py
--rw-r--r--   0        0        0    23013 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/chat/adapters.py
--rw-r--r--   0        0        0    12343 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/chat/chat_generator.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/tests/conftest.py
--rw-r--r--   0        0        0    15641 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/tests/test_chat_generator.py
--rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/tests/test_document_embedder.py
--rw-r--r--   0        0        0    41832 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/tests/test_generator.py
--rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/tests/test_text_embedder.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/README.md
--rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1444 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/examples/chatgenerator_example.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/examples/embedders_generator_with_rag_example.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/pydoc/config.yml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/common/amazon_bedrock/__init__.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/common/amazon_bedrock/errors.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/common/amazon_bedrock/utils.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/embedders/amazon_bedrock/__init__.py
+-rw-r--r--   0        0        0    12587 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/embedders/amazon_bedrock/document_embedder.py
+-rw-r--r--   0        0        0     8479 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/embedders/amazon_bedrock/text_embedder.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/__init__.py
+-rw-r--r--   0        0        0    13329 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/adapters.py
+-rw-r--r--   0        0        0    12287 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/generator.py
+-rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/handlers.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/chat/__init__.py
+-rw-r--r--   0        0        0    23013 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/chat/adapters.py
+-rw-r--r--   0        0        0    12418 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/chat/chat_generator.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/tests/__init__.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/tests/conftest.py
+-rw-r--r--   0        0        0    15641 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/tests/test_chat_generator.py
+-rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/tests/test_document_embedder.py
+-rw-r--r--   0        0        0    41832 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/tests/test_generator.py
+-rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/tests/test_text_embedder.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/LICENSE.txt
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/README.md
+-rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 amazon_bedrock_haystack-0.7.1/PKG-INFO
```

### Comparing `amazon_bedrock_haystack-0.7.0/examples/chatgenerator_example.py` & `amazon_bedrock_haystack-0.7.1/examples/chatgenerator_example.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.0/examples/embedders_generator_with_rag_example.py` & `amazon_bedrock_haystack-0.7.1/examples/embedders_generator_with_rag_example.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.0/pydoc/config.yml` & `amazon_bedrock_haystack-0.7.1/pydoc/config.yml`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.0/src/haystack_integrations/common/amazon_bedrock/errors.py` & `amazon_bedrock_haystack-0.7.1/src/haystack_integrations/common/amazon_bedrock/errors.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.0/src/haystack_integrations/common/amazon_bedrock/utils.py` & `amazon_bedrock_haystack-0.7.1/src/haystack_integrations/common/amazon_bedrock/utils.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/embedders/amazon_bedrock/document_embedder.py` & `amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/embedders/amazon_bedrock/document_embedder.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/embedders/amazon_bedrock/text_embedder.py` & `amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/embedders/amazon_bedrock/text_embedder.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/adapters.py` & `amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/adapters.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/generator.py` & `amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/generator.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/handlers.py` & `amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/handlers.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/chat/adapters.py` & `amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/chat/adapters.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.0/src/haystack_integrations/components/generators/amazon_bedrock/chat/chat_generator.py` & `amazon_bedrock_haystack-0.7.1/src/haystack_integrations/components/generators/amazon_bedrock/chat/chat_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,25 +206,26 @@
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
 
         :returns:
             Dictionary with serialized data.
         """
+        callback_name = serialize_callable(self.streaming_callback) if self.streaming_callback else None
         return default_to_dict(
             self,
             aws_access_key_id=self.aws_access_key_id.to_dict() if self.aws_access_key_id else None,
             aws_secret_access_key=self.aws_secret_access_key.to_dict() if self.aws_secret_access_key else None,
             aws_session_token=self.aws_session_token.to_dict() if self.aws_session_token else None,
             aws_region_name=self.aws_region_name.to_dict() if self.aws_region_name else None,
             aws_profile_name=self.aws_profile_name.to_dict() if self.aws_profile_name else None,
             model=self.model,
             stop_words=self.stop_words,
             generation_kwargs=self.model_adapter.generation_kwargs,
-            streaming_callback=serialize_callable(self.streaming_callback),
+            streaming_callback=callback_name,
         )
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "AmazonBedrockChatGenerator":
         """
         Deserializes the component from a dictionary.
```

### Comparing `amazon_bedrock_haystack-0.7.0/tests/conftest.py` & `amazon_bedrock_haystack-0.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.0/tests/test_chat_generator.py` & `amazon_bedrock_haystack-0.7.1/tests/test_chat_generator.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.0/tests/test_document_embedder.py` & `amazon_bedrock_haystack-0.7.1/tests/test_document_embedder.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.0/tests/test_generator.py` & `amazon_bedrock_haystack-0.7.1/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.0/tests/test_text_embedder.py` & `amazon_bedrock_haystack-0.7.1/tests/test_text_embedder.py`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.0/.gitignore` & `amazon_bedrock_haystack-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.0/LICENSE.txt` & `amazon_bedrock_haystack-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.0/README.md` & `amazon_bedrock_haystack-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `amazon_bedrock_haystack-0.7.0/pyproject.toml` & `amazon_bedrock_haystack-0.7.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "deepset GmbH", email = "info@deepset.ai" },
 ]
 classifiers = [
+  "License :: OSI Approved :: Apache Software License",
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
```

### Comparing `amazon_bedrock_haystack-0.7.0/PKG-INFO` & `amazon_bedrock_haystack-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.3
 Name: amazon-bedrock-haystack
-Version: 0.7.0
+Version: 0.7.1
 Summary: An integration of Amazon Bedrock as an AmazonBedrockGenerator component.
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/amazon_bedrock#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/amazon_bedrock
 Author-email: deepset GmbH <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

