# Comparing `tmp/doctran_openai-0.0.8.tar.gz` & `tmp/doctran_openai-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doctran_openai-0.0.8.tar", max compression
+gzip compressed data, was "doctran_openai-0.0.9.tar", max compression
```

## Comparing `doctran_openai-0.0.8.tar` & `doctran_openai-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2024-04-23 01:40:16.420261 doctran_openai-0.0.8/LICENSE
--rw-r--r--   0        0        0     7846 2024-04-23 01:40:16.420425 doctran_openai-0.0.8/README.md
--rw-r--r--   0        0        0      124 2024-04-23 04:57:37.314031 doctran_openai-0.0.8/doctran_openai/__init__.py
--rw-r--r--   0        0        0     8396 2024-04-23 10:37:28.266936 doctran_openai-0.0.8/doctran_openai/doctran_openai.py
--rw-r--r--   0        0        0      202 2024-04-23 01:40:16.421090 doctran_openai-0.0.8/doctran_openai/transformers/__init__.py
--rw-r--r--   0        0        0    15249 2024-04-23 10:44:06.378621 doctran_openai-0.0.8/doctran_openai/transformers/transformers.py
--rw-r--r--   0        0        0      550 2024-04-23 10:46:04.216865 doctran_openai-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     8607 1970-01-01 00:00:00.000000 doctran_openai-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-23 01:40:16.420261 doctran_openai-0.0.9/LICENSE
+-rw-r--r--   0        0        0     7846 2024-04-23 01:40:16.420425 doctran_openai-0.0.9/README.md
+-rw-r--r--   0        0        0      124 2024-04-23 04:57:37.314031 doctran_openai-0.0.9/doctran_openai/__init__.py
+-rw-r--r--   0        0        0     8262 2024-04-23 12:15:05.971745 doctran_openai-0.0.9/doctran_openai/doctran_openai.py
+-rw-r--r--   0        0        0      202 2024-04-23 01:40:16.421090 doctran_openai-0.0.9/doctran_openai/transformers/__init__.py
+-rw-r--r--   0        0        0    15212 2024-04-23 12:20:24.815714 doctran_openai-0.0.9/doctran_openai/transformers/transformers.py
+-rw-r--r--   0        0        0      550 2024-04-23 12:21:15.438670 doctran_openai-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     8607 1970-01-01 00:00:00.000000 doctran_openai-0.0.9/PKG-INFO
```

### Comparing `doctran_openai-0.0.8/LICENSE` & `doctran_openai-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `doctran_openai-0.0.8/README.md` & `doctran_openai-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `doctran_openai-0.0.8/doctran_openai/doctran_openai.py` & `doctran_openai-0.0.9/doctran_openai/doctran_openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import importlib
 import yaml
-from openai import OpenAI
+import openai
 import uuid
 from enum import Enum
 from typing import List, Optional, Dict, Any, Literal, Union
 from pydantic import BaseModel
 
 
 class ExtractProperty(BaseModel):
@@ -13,22 +13,17 @@
     description: str
     type: Literal["string", "number", "boolean", "array", "object"]
     items: Optional[Union[List, Dict[str, Any]]]
     enum: Optional[List[str]]
     required: bool = True
 
 
-class OpenAIConfig(BaseModel):
-    api_key: str
-    base_url: Optional[str]
-
-
 class DoctranConfig(BaseModel):
     openai_model: str
-    openai: OpenAI
+    openai: Any
     openai_token_limit: int
 
 
 class ContentType(Enum):
     text = "text"
     html = "html"
     pdf = "pdf"
@@ -182,31 +177,31 @@
     def process_template(self, *, template_regex: str) -> 'DocumentTransformationBuilder':
         self.transformations.append((Transformation.process_template, {"template_regex": template_regex}))
         return self
 
 
 class Doctran:
     def __init__(self, openai_api_key: str = None, openai_model: str = "gpt-4", openai_token_limit: int = 8000, openai_api_base: str = None):
+        self.config = DoctranConfig(
+            openai=openai,
+            openai_model=openai_model,
+            openai_token_limit=openai_token_limit
+        )
+
         if openai_api_key:
-            openai_config = OpenAIConfig(api_key=openai_api_key)
+            self.config.api_key = openai_api_key
         elif os.environ.get("OPENAI_API_KEY"):
-            openai_config = OpenAIConfig(api_key=os.environ["OPENAI_API_KEY"])
+            self.config.api_key = os.environ.get("OPENAI_API_KEY")
         else:
             raise Exception("No OpenAI API Key provided")
 
         if openai_api_base:
-            openai_config.base_url = openai_api_base
+            self.config.api_base = openai_api_base
         elif os.environ.get('OPENAI_API_BASE'):
-            openai_config.base_url = os.environ['OPENAI_API_BASE']
-
-        self.config = DoctranConfig(
-            openai_model=openai_model,
-            openai_token_limit=openai_token_limit,
-            **openai_config.dict()
-        )
+            self.config.api_base = os.environ['OPENAI_API_BASE']
 
     def parse(self, *, content: str, content_type: ContentType = "text", uri: str = None,
               metadata: dict = None) -> Document:
         '''
         Parse raw text and apply different chunking schemes based on the content type.
 
         Returns:
```

### Comparing `doctran_openai-0.0.8/doctran_openai/transformers/transformers.py` & `doctran_openai-0.0.9/doctran_openai/transformers/transformers.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,22 +62,22 @@
         return self.executeOpenAICall(document)
 
     def executeOpenAICall(self, document: Document) -> Document:
         try:
             function_call = OpenAIFunctionCall(
                 model=self.config.openai_model,
                 messages=[{"role": "user", "content": document.transformed_content}],
-                tools=[{
+                functions=[{
                     "name": self.function_name,
                     "description": self.function_description,
                     "parameters": self.function_parameters,
                 }],
-                tool_choice={"name": self.function_name}
+                function_call={"name": self.function_name}
             )
-            completion = self.config.openai.completions.create(**function_call.dict())
+            completion = self.config.openai.chat.completions.create(**function_call.dict())
             arguments = completion.choices[0].message.function_call.arguments
             try:
                 arguments = json.loads(arguments)
             except Exception as e:
                 raise Exception(
                     "OpenAI returned malformatted JSON This is likely due to the completion running out of tokens. " +
                     f"Setting a higher token limit may fix this error. JSON returned: {arguments}")
@@ -201,31 +201,33 @@
         nlp_engine = nlp_engine_provider.create_engine()
         analyzer = AnalyzerEngine(nlp_engine=nlp_engine)
         anonymizer = AnonymizerEngine()
         results = analyzer.analyze(text=text,
                                    entities=self.entities if self.entities else None,
                                    language='en')
         # TODO: Define customer operator to replace data types with numbered placeholders to differentiate between different PERSONs, EMAILs, etc
-        anonymized_data = anonymizer.anonymize(text=text,
-                                               analyzer_results=results,
-                                               operators={"DEFAULT": OperatorConfig("replace")})
+        anonymized_data = anonymizer.anonymize(
+            text=text,
+            analyzer_results=results,
+            operators={"DEFAULT": OperatorConfig("replace")}
+        )
 
         # Extract just the anonymized text, discarding items metadata
         anonymized_text = anonymized_data.text
         document.transformed_content = anonymized_text
         return document
 
 
 class DocumentRefiner(OpenAIDocumentTransformer):
-    '''
+    """
     Use OpenAI function calling to remove irrelevant information from the document.
 
     Returns:
         Document: the refined content represented as a Doctran Document
-    '''
+    """
     topics: List[str]
 
     def __init__(self, *, config: DoctranConfig, topics: List[str] = None) -> None:
         super().__init__(config)
         self.topics = topics
         self.function_name = "refine"
         if topics:
@@ -236,40 +238,40 @@
             "type": "string",
             "description": "The document with irrelevant information removed.",
         }
         self.function_parameters["required"].append("refined_document")
 
 
 class DocumentTranslator(OpenAIDocumentTransformer):
-    '''
+    """
     Use OpenAI function calling to translate the document to another language.
 
     Returns:
         Document: the translated document represented as a Doctran Document
-    '''
+    """
     language: str
 
     def __init__(self, *, config: DoctranConfig, language: str) -> None:
         super().__init__(config)
         self.function_name = "translate"
         self.function_description = f"Translate a document into {language}"
         self.function_parameters["properties"]["translated_document"] = {
             "type": "string",
             "description": f"The document translated into {language}."
         }
         self.function_parameters["required"].append("translated_document")
 
 
 class DocumentInterrogator(OpenAIDocumentTransformer):
-    '''
+    """
     Use OpenAI function calling to convert the document to a series of questions and answers.
 
     Returns:
         Document: the interrogated document represented as a Doctran Document
-    '''
+    """
 
     def __init__(self, *, config: DoctranConfig) -> None:
         super().__init__(config)
         self.function_name = "interrogate"
         self.function_description = "Convert a text document into a series of questions and answers."
         self.function_parameters["properties"]["questions_and_answers"] = {
             "type": "array",
@@ -289,22 +291,22 @@
                 "required": ["question", "answer"],
             },
         }
         self.function_parameters["required"].append("questions_and_answers")
 
 
 class DocumentTemplateProcessor(OpenAIDocumentTransformer):
-    '''
+    """
     Use OpenAI function calling to replace a given template pattern in the document with the instructions provided within each placeholder.
 
     For example: "Let's meet on {random day of the week}" -> "Let's meet on Monday"
 
     Returns:
         Document: the interrogated document represented as a Doctran Document
-    '''
+    """
 
     def __init__(self, *, config: DoctranConfig, template_regex: str) -> None:
         super().__init__(config)
         try:
             re.compile(template_regex)
         except re.error as e:
             raise Exception(f"Provided template pattern is not valid regex: {e}")
```

### Comparing `doctran_openai-0.0.8/pyproject.toml` & `doctran_openai-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "doctran_openai"
-version = "0.0.8"
+version = "0.0.9"
 description = "Document transformation framework for vector based retrieval"
 authors = ["William Yang <yangfei86@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10.0"
 pydantic = "^1.10.9"
```

### Comparing `doctran_openai-0.0.8/PKG-INFO` & `doctran_openai-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doctran_openai
-Version: 0.0.8
+Version: 0.0.9
 Summary: Document transformation framework for vector based retrieval
 Author: William Yang
 Author-email: yangfei86@gmail.com
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: doctran_openai Version: 0.0.8 Summary: Document
+Metadata-Version: 2.1 Name: doctran_openai Version: 0.0.9 Summary: Document
 transformation framework for vector based retrieval Author: William Yang
 Author-email: yangfei86@gmail.com Requires-Python: >=3.10.0,<4.0.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: openai (>=1.23.2,<2.0.0) Requires-Dist: presidio-analyzer
 (>=2.2.33,<3.0.0) Requires-Dist: presidio-anonymizer (>=2.2.33,<3.0.0)
```

