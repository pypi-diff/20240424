# Comparing `tmp/basicbedrock-0.1.5.tar.gz` & `tmp/basicbedrock-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basicbedrock-0.1.5.tar", last modified: Tue Apr 23 14:52:00 2024, max compression
+gzip compressed data, was "basicbedrock-0.1.6.tar", last modified: Wed Apr 24 15:25:36 2024, max compression
```

## Comparing `basicbedrock-0.1.5.tar` & `basicbedrock-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-23 14:52:00.165076 basicbedrock-0.1.5/
--rw-r--r--   0 dmattsn    (504) staff       (20)     1048 2024-04-07 21:53:42.000000 basicbedrock-0.1.5/LICENSE
--rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-23 14:52:00.164795 basicbedrock-0.1.5/PKG-INFO
--rw-r--r--   0 dmattsn    (504) staff       (20)     1978 2024-04-11 00:27:04.000000 basicbedrock-0.1.5/README.md
--rw-r--r--   0 dmattsn    (504) staff       (20)      811 2024-04-23 14:51:35.000000 basicbedrock-0.1.5/pyproject.toml
--rw-r--r--   0 dmattsn    (504) staff       (20)       38 2024-04-23 14:52:00.165142 basicbedrock-0.1.5/setup.cfg
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-23 14:52:00.158762 basicbedrock-0.1.5/src/
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-23 14:52:00.159798 basicbedrock-0.1.5/src/basicbedrock/
--rw-r--r--   0 dmattsn    (504) staff       (20)      273 2024-04-23 14:50:30.000000 basicbedrock-0.1.5/src/basicbedrock/__init__.py
--rw-r--r--   0 dmattsn    (504) staff       (20)    16145 2024-04-23 14:50:11.000000 basicbedrock-0.1.5/src/basicbedrock/basicbedrock.py
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-23 14:52:00.163019 basicbedrock-0.1.5/src/basicbedrock/models/
--rw-r--r--   0 dmattsn    (504) staff       (20)     2984 2024-04-22 22:00:00.000000 basicbedrock-0.1.5/src/basicbedrock/models/__init__.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     2729 2024-04-22 21:49:02.000000 basicbedrock-0.1.5/src/basicbedrock/models/ai21.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     5028 2024-04-22 21:52:22.000000 basicbedrock-0.1.5/src/basicbedrock/models/amazon.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     4480 2024-04-22 21:58:39.000000 basicbedrock-0.1.5/src/basicbedrock/models/anthropic.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     5241 2024-04-11 00:27:04.000000 basicbedrock-0.1.5/src/basicbedrock/models/baseclasses.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     3037 2024-04-22 21:52:22.000000 basicbedrock-0.1.5/src/basicbedrock/models/cohere.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     2315 2024-04-22 21:52:22.000000 basicbedrock-0.1.5/src/basicbedrock/models/meta.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     1559 2024-04-22 21:49:02.000000 basicbedrock-0.1.5/src/basicbedrock/models/mistral.py
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-23 14:52:00.164423 basicbedrock-0.1.5/src/basicbedrock.egg-info/
--rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-23 14:52:00.000000 basicbedrock-0.1.5/src/basicbedrock.egg-info/PKG-INFO
--rw-r--r--   0 dmattsn    (504) staff       (20)      586 2024-04-23 14:52:00.000000 basicbedrock-0.1.5/src/basicbedrock.egg-info/SOURCES.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)        1 2024-04-23 14:52:00.000000 basicbedrock-0.1.5/src/basicbedrock.egg-info/dependency_links.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)       31 2024-04-23 14:52:00.000000 basicbedrock-0.1.5/src/basicbedrock.egg-info/requires.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)       13 2024-04-23 14:52:00.000000 basicbedrock-0.1.5/src/basicbedrock.egg-info/top_level.txt
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-23 14:52:00.163235 basicbedrock-0.1.5/test/
--rw-r--r--   0 dmattsn    (504) staff       (20)     4526 2024-04-11 01:09:03.000000 basicbedrock-0.1.5/test/tests.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-24 15:25:36.592798 basicbedrock-0.1.6/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     1048 2024-04-07 21:53:42.000000 basicbedrock-0.1.6/LICENSE
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-24 15:25:36.592510 basicbedrock-0.1.6/PKG-INFO
+-rw-r--r--   0 dmattsn    (504) staff       (20)     1978 2024-04-11 00:27:04.000000 basicbedrock-0.1.6/README.md
+-rw-r--r--   0 dmattsn    (504) staff       (20)      811 2024-04-24 15:25:23.000000 basicbedrock-0.1.6/pyproject.toml
+-rw-r--r--   0 dmattsn    (504) staff       (20)       38 2024-04-24 15:25:36.592870 basicbedrock-0.1.6/setup.cfg
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-24 15:25:36.587518 basicbedrock-0.1.6/src/
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-24 15:25:36.588784 basicbedrock-0.1.6/src/basicbedrock/
+-rw-r--r--   0 dmattsn    (504) staff       (20)      273 2024-04-24 15:25:23.000000 basicbedrock-0.1.6/src/basicbedrock/__init__.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)    16145 2024-04-23 14:50:11.000000 basicbedrock-0.1.6/src/basicbedrock/basicbedrock.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-24 15:25:36.591422 basicbedrock-0.1.6/src/basicbedrock/models/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3223 2024-04-24 15:17:04.000000 basicbedrock-0.1.6/src/basicbedrock/models/__init__.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     2729 2024-04-22 21:49:02.000000 basicbedrock-0.1.6/src/basicbedrock/models/ai21.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     5028 2024-04-22 21:52:22.000000 basicbedrock-0.1.6/src/basicbedrock/models/amazon.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     4480 2024-04-22 21:58:39.000000 basicbedrock-0.1.6/src/basicbedrock/models/anthropic.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     5241 2024-04-11 00:27:04.000000 basicbedrock-0.1.6/src/basicbedrock/models/baseclasses.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3037 2024-04-22 21:52:22.000000 basicbedrock-0.1.6/src/basicbedrock/models/cohere.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     2309 2024-04-24 15:17:04.000000 basicbedrock-0.1.6/src/basicbedrock/models/meta.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     1559 2024-04-22 21:49:02.000000 basicbedrock-0.1.6/src/basicbedrock/models/mistral.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-24 15:25:36.591916 basicbedrock-0.1.6/src/basicbedrock.egg-info/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-24 15:25:36.000000 basicbedrock-0.1.6/src/basicbedrock.egg-info/PKG-INFO
+-rw-r--r--   0 dmattsn    (504) staff       (20)      586 2024-04-24 15:25:36.000000 basicbedrock-0.1.6/src/basicbedrock.egg-info/SOURCES.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)        1 2024-04-24 15:25:36.000000 basicbedrock-0.1.6/src/basicbedrock.egg-info/dependency_links.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)       31 2024-04-24 15:25:36.000000 basicbedrock-0.1.6/src/basicbedrock.egg-info/requires.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)       13 2024-04-24 15:25:36.000000 basicbedrock-0.1.6/src/basicbedrock.egg-info/top_level.txt
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-24 15:25:36.591586 basicbedrock-0.1.6/test/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     4526 2024-04-11 01:09:03.000000 basicbedrock-0.1.6/test/tests.py
```

### Comparing `basicbedrock-0.1.5/LICENSE` & `basicbedrock-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.5/PKG-INFO` & `basicbedrock-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basicbedrock
-Version: 0.1.5
+Version: 0.1.6
 Summary: An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas.
 Author-email: cyberitech <mattsod@kaizencyber.io>
 Maintainer-email: cyberitech <mattsod@kaizencyber.io>
 License: Copyright 2024 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `basicbedrock-0.1.5/README.md` & `basicbedrock-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.5/pyproject.toml` & `basicbedrock-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "basicbedrock"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="cyberitech", email="mattsod@kaizencyber.io" },
 ]
 maintainers = [
     { name="cyberitech", email="mattsod@kaizencyber.io" },
 ]
 description = "An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas."
```

### Comparing `basicbedrock-0.1.5/src/basicbedrock/basicbedrock.py` & `basicbedrock-0.1.6/src/basicbedrock/basicbedrock.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.5/src/basicbedrock/models/__init__.py` & `basicbedrock-0.1.6/src/basicbedrock/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,18 @@
     "anthropic.claude-3-sonnet-20240229-v1:0": AnthropicClaude3BaseRequest,
     "anthropic.claude-3-haiku-20240307-v1:0": AnthropicClaude3BaseRequest,
     #  unavailable "anthropic.claude-3-opus-20240229-v1:0":AnthropicClaude3BaseRequest,
     "cohere.command-text-v14": CohereCommandTextBaseRequest,
     "cohere.command-light-text-v14": CohereCommandTextBaseRequest,
     "cohere.embed-english-v3": CohereEmbedBaseRequest,
     "cohere.embed-multilingual-v3": CohereEmbedBaseRequest,
-    "meta.llama2-13b-chat-v1": MetaLlama2ChatV1BaseRequest,
-    "meta.llama2-70b-chat-v1": MetaLlama2ChatV1BaseRequest,
+    "meta.llama2-13b-chat-v1": MetaLlamaV2V3BaseRequest,
+    "meta.llama2-70b-chat-v1": MetaLlamaV2V3BaseRequest,
+    "meta.llama3-8b-instruct-v1:0": MetaLlamaV2V3BaseRequest,
+    "meta.llama3-70b-instruct-v1:0": MetaLlamaV2V3BaseRequest,
     "mistral.mistral-7b-instruct-v0:2": MistralBaseRequest,
     "mistral.mixtral-8x7b-instruct-v0:1": MistralBaseRequest,
     "mistral.mistral-large-2402-v1:0": MistralBaseRequest
 }
 
 model_response_mapping = {
     "ai21.j2-ultra-v1": AI21Jurassic2BaseResponse,
@@ -48,13 +50,15 @@
     "anthropic.claude-3-sonnet-20240229-v1:0": AnthropicClaude3BaseResponse,
     "anthropic.claude-3-haiku-20240307-v1:0": AnthropicClaude3BaseResponse,
     #  unavailable "anthropic.claude-3-opus-20240229-v1:0": AnthropicClaude3BaseResponse,
     "cohere.command-text-v14": CohereCommandTextBaseResponse,
     "cohere.command-light-text-v14": CohereCommandTextBaseResponse,
     "cohere.embed-english-v3": CohereEmbedBaseResponse,
     "cohere.embed-multilingual-v3": CohereEmbedBaseResponse,
-    "meta.llama2-13b-chat-v1": MetaLlama2ChatV1BaseResponse,
-    "meta.llama2-70b-chat-v1": MetaLlama2ChatV1BaseResponse,
+    "meta.llama2-13b-chat-v1": MetaLlamaV2V3BaseResponse,
+    "meta.llama2-70b-chat-v1": MetaLlamaV2V3BaseResponse,
+    "meta.llama3-8b-instruct-v1:0": MetaLlamaV2V3BaseResponse,
+    "meta.llama3-70b-instruct-v1:0":MetaLlamaV2V3BaseResponse,
     "mistral.mistral-7b-instruct-v0:2": MistralBaseResponse,
     "mistral.mixtral-8x7b-instruct-v0:1": MistralBaseResponse,
     "mistral.mistral-large-2402-v1:0": MistralBaseResponse
 }
```

### Comparing `basicbedrock-0.1.5/src/basicbedrock/models/ai21.py` & `basicbedrock-0.1.6/src/basicbedrock/models/ai21.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.5/src/basicbedrock/models/amazon.py` & `basicbedrock-0.1.6/src/basicbedrock/models/amazon.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.5/src/basicbedrock/models/anthropic.py` & `basicbedrock-0.1.6/src/basicbedrock/models/anthropic.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.5/src/basicbedrock/models/baseclasses.py` & `basicbedrock-0.1.6/src/basicbedrock/models/baseclasses.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.5/src/basicbedrock/models/cohere.py` & `basicbedrock-0.1.6/src/basicbedrock/models/cohere.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.5/src/basicbedrock/models/meta.py` & `basicbedrock-0.1.6/src/basicbedrock/models/meta.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Amazon docs currently do not have request schemas for Llama 2 13b and Llama 2 70b, only the chat versions
 """
 import typing
 
 from baseclasses import BaseAbstractRequest, BaseAbstractResponse
 
 
-class MetaLlama2ChatV1BaseRequest(BaseAbstractRequest):
+class MetaLlamaV2V3BaseRequest(BaseAbstractRequest):
     """
     Meta LLama 2 13b chat request format.
     This model supports max_token, temperature and top_p.
     It does not support top_k
     """
     prompt: str = "{PROMPT}"
     max_gen_len: int = 250
@@ -76,15 +76,15 @@
         set the maximum tokens parameter.
         :param max_tokens:
         :return:
         """
         self.max_gen_len = max_tokens
 
 
-class MetaLlama2ChatV1BaseResponse(BaseAbstractResponse):
+class MetaLlamaV2V3BaseResponse(BaseAbstractResponse):
     """
     Response format of Meta Llama 2 V1 family chat response.
     """
 
     def get_answer(self) -> str:
         return self.result_raw['generation']
```

### Comparing `basicbedrock-0.1.5/src/basicbedrock/models/mistral.py` & `basicbedrock-0.1.6/src/basicbedrock/models/mistral.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.5/src/basicbedrock.egg-info/PKG-INFO` & `basicbedrock-0.1.6/src/basicbedrock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basicbedrock
-Version: 0.1.5
+Version: 0.1.6
 Summary: An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas.
 Author-email: cyberitech <mattsod@kaizencyber.io>
 Maintainer-email: cyberitech <mattsod@kaizencyber.io>
 License: Copyright 2024 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `basicbedrock-0.1.5/src/basicbedrock.egg-info/SOURCES.txt` & `basicbedrock-0.1.6/src/basicbedrock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.5/test/tests.py` & `basicbedrock-0.1.6/test/tests.py`

 * *Files identical despite different names*

