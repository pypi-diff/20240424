# Comparing `tmp/langchain_groq-0.1.1.tar.gz` & `tmp/langchain_groq-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_groq-0.1.1.tar", max compression
+gzip compressed data, was "langchain_groq-0.1.2.tar", max compression
```

## Comparing `langchain_groq-0.1.1.tar` & `langchain_groq-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2024-04-09 23:31:59.353546 langchain_groq-0.1.1/LICENSE
--rw-r--r--   0        0        0     1986 2024-04-09 23:31:59.353546 langchain_groq-0.1.1/README.md
--rw-r--r--   0        0        0       72 2024-04-09 23:31:59.353546 langchain_groq-0.1.1/langchain_groq/__init__.py
--rw-r--r--   0        0        0    38440 2024-04-09 23:31:59.353546 langchain_groq-0.1.1/langchain_groq/chat_models.py
--rw-r--r--   0        0        0        0 2024-04-09 23:31:59.353546 langchain_groq-0.1.1/langchain_groq/py.typed
--rw-r--r--   0        0        0     2544 2024-04-09 23:31:59.353546 langchain_groq-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2793 1970-01-01 00:00:00.000000 langchain_groq-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-11 16:21:09.617260 langchain_groq-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1986 2024-04-11 16:21:09.617260 langchain_groq-0.1.2/README.md
+-rw-r--r--   0        0        0       72 2024-04-11 16:21:09.617260 langchain_groq-0.1.2/langchain_groq/__init__.py
+-rw-r--r--   0        0        0    39886 2024-04-11 16:21:09.617260 langchain_groq-0.1.2/langchain_groq/chat_models.py
+-rw-r--r--   0        0        0        0 2024-04-11 16:21:09.617260 langchain_groq-0.1.2/langchain_groq/py.typed
+-rw-r--r--   0        0        0     2544 2024-04-11 16:21:09.617260 langchain_groq-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2793 1970-01-01 00:00:00.000000 langchain_groq-0.1.2/PKG-INFO
```

### Comparing `langchain_groq-0.1.1/LICENSE` & `langchain_groq-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_groq-0.1.1/README.md` & `langchain_groq-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `langchain_groq-0.1.1/langchain_groq/chat_models.py` & `langchain_groq-0.1.2/langchain_groq/chat_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,16 @@
     JsonOutputParser,
     PydanticOutputParser,
 )
 from langchain_core.output_parsers.base import OutputParserLike
 from langchain_core.output_parsers.openai_tools import (
     JsonOutputKeyToolsParser,
     PydanticToolsParser,
+    make_invalid_tool_call,
+    parse_tool_call,
 )
 from langchain_core.outputs import ChatGeneration, ChatGenerationChunk, ChatResult
 from langchain_core.pydantic_v1 import BaseModel, Field, SecretStr, root_validator
 from langchain_core.runnables import Runnable, RunnableMap, RunnablePassthrough
 from langchain_core.tools import BaseTool
 from langchain_core.utils import (
     convert_to_secret_str,
@@ -274,17 +276,28 @@
         if "tools" in kwargs:
             response = self.client.create(
                 messages=message_dicts, **{**params, **kwargs}
             )
             chat_result = self._create_chat_result(response)
             generation = chat_result.generations[0]
             message = generation.message
+            tool_call_chunks = [
+                {
+                    "name": rtc["function"].get("name"),
+                    "args": rtc["function"].get("arguments"),
+                    "id": rtc.get("id"),
+                    "index": rtc.get("index"),
+                }
+                for rtc in message.additional_kwargs["tool_calls"]
+            ]
             chunk_ = ChatGenerationChunk(
                 message=AIMessageChunk(
-                    content=message.content, additional_kwargs=message.additional_kwargs
+                    content=message.content,
+                    additional_kwargs=message.additional_kwargs,
+                    tool_call_chunks=tool_call_chunks,
                 ),
                 generation_info=generation.generation_info,
             )
             if run_manager:
                 geninfo = chunk_.generation_info or {}
                 run_manager.on_llm_new_token(
                     chunk_.text,
@@ -334,17 +347,28 @@
         if "tools" in kwargs:
             response = await self.async_client.create(
                 messages=message_dicts, **{**params, **kwargs}
             )
             chat_result = self._create_chat_result(response)
             generation = chat_result.generations[0]
             message = generation.message
+            tool_call_chunks = [
+                {
+                    "name": rtc["function"].get("name"),
+                    "args": rtc["function"].get("arguments"),
+                    "id": rtc.get("id"),
+                    "index": rtc.get("index"),
+                }
+                for rtc in message.additional_kwargs["tool_calls"]
+            ]
             chunk_ = ChatGenerationChunk(
                 message=AIMessageChunk(
-                    content=message.content, additional_kwargs=message.additional_kwargs
+                    content=message.content,
+                    additional_kwargs=message.additional_kwargs,
+                    tool_call_chunks=tool_call_chunks,
                 ),
                 generation_info=generation.generation_info,
             )
             if run_manager:
                 geninfo = chunk_.generation_info or {}
                 await run_manager.on_llm_new_token(
                     chunk_.text,
@@ -879,17 +903,32 @@
     if role == "user":
         return HumanMessage(content=_dict.get("content", ""))
     elif role == "assistant":
         content = _dict.get("content", "") or ""
         additional_kwargs: Dict = {}
         if function_call := _dict.get("function_call"):
             additional_kwargs["function_call"] = dict(function_call)
-        if tool_calls := _dict.get("tool_calls"):
-            additional_kwargs["tool_calls"] = tool_calls
-        return AIMessage(content=content, id=id_, additional_kwargs=additional_kwargs)
+        tool_calls = []
+        invalid_tool_calls = []
+        if raw_tool_calls := _dict.get("tool_calls"):
+            additional_kwargs["tool_calls"] = raw_tool_calls
+            for raw_tool_call in raw_tool_calls:
+                try:
+                    tool_calls.append(parse_tool_call(raw_tool_call, return_id=True))
+                except Exception as e:
+                    invalid_tool_calls.append(
+                        make_invalid_tool_call(raw_tool_call, str(e))
+                    )
+        return AIMessage(
+            content=content,
+            id=id_,
+            additional_kwargs=additional_kwargs,
+            tool_calls=tool_calls,
+            invalid_tool_calls=invalid_tool_calls,
+        )
     elif role == "system":
         return SystemMessage(content=_dict.get("content", ""))
     elif role == "function":
         return FunctionMessage(content=_dict.get("content", ""), name=_dict.get("name"))
     elif role == "tool":
         additional_kwargs = {}
         if "name" in _dict:
```

### Comparing `langchain_groq-0.1.1/pyproject.toml` & `langchain_groq-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-groq"
-version = "0.1.1"
+version = "0.1.2"
 description = "An integration package connecting Groq and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/groq"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.41"
+langchain-core = "^0.1.42"
 groq = ">=0.4.1,<1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
```

### Comparing `langchain_groq-0.1.1/PKG-INFO` & `langchain_groq-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: langchain-groq
-Version: 0.1.1
+Version: 0.1.2
 Summary: An integration package connecting Groq and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: groq (>=0.4.1,<1)
-Requires-Dist: langchain-core (>=0.1.41,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.42,<0.2.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/groq
 Description-Content-Type: text/markdown
 
 # langchain-groq
 
 ## Welcome to Groq! 🚀
```

