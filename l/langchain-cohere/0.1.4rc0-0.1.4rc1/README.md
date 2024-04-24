# Comparing `tmp/langchain_cohere-0.1.4rc0.tar.gz` & `tmp/langchain_cohere-0.1.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_cohere-0.1.4rc0.tar", max compression
+gzip compressed data, was "langchain_cohere-0.1.4rc1.tar", max compression
```

## Comparing `langchain_cohere-0.1.4rc0.tar` & `langchain_cohere-0.1.4rc1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1072 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/LICENSE
--rw-r--r--   0        0        0     5585 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/README.md
--rw-r--r--   0        0        0      608 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/langchain_cohere/__init__.py
--rw-r--r--   0        0        0    17262 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/langchain_cohere/chat_models.py
--rw-r--r--   0        0        0     8173 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/langchain_cohere/cohere_agent.py
--rw-r--r--   0        0        0     1585 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/langchain_cohere/common.py
--rw-r--r--   0        0        0     5813 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/langchain_cohere/embeddings.py
--rw-r--r--   0        0        0     8058 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/langchain_cohere/llms.py
--rw-r--r--   0        0        0        0 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/langchain_cohere/py.typed
--rw-r--r--   0        0        0     3349 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/langchain_cohere/rag_retrievers.py
--rw-r--r--   0        0        0        0 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/langchain_cohere/react_multi_hop/__init__.py
--rw-r--r--   0        0        0     4913 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/langchain_cohere/react_multi_hop/agent.py
--rw-r--r--   0        0        0     4060 2024-04-18 18:09:53.765208 langchain_cohere-0.1.4rc0/langchain_cohere/react_multi_hop/default_prompt_constants.py
--rw-r--r--   0        0        0    11351 2024-04-18 18:09:53.765208 langchain_cohere-0.1.4rc0/langchain_cohere/react_multi_hop/parsing.py
--rw-r--r--   0        0        0     9728 2024-04-18 18:09:53.765208 langchain_cohere-0.1.4rc0/langchain_cohere/react_multi_hop/prompt.py
--rw-r--r--   0        0        0     4134 2024-04-18 18:09:53.765208 langchain_cohere-0.1.4rc0/langchain_cohere/rerank.py
--rw-r--r--   0        0        0     1655 2024-04-18 18:09:53.765208 langchain_cohere-0.1.4rc0/langchain_cohere/utils.py
--rw-r--r--   0        0        0     2682 2024-04-18 18:09:53.765208 langchain_cohere-0.1.4rc0/pyproject.toml
--rw-r--r--   0        0        0     6413 1970-01-01 00:00:00.000000 langchain_cohere-0.1.4rc0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/LICENSE
+-rw-r--r--   0        0        0     5585 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/README.md
+-rw-r--r--   0        0        0      608 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/langchain_cohere/__init__.py
+-rw-r--r--   0        0        0    19128 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/langchain_cohere/chat_models.py
+-rw-r--r--   0        0        0     8173 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/langchain_cohere/cohere_agent.py
+-rw-r--r--   0        0        0     1585 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/langchain_cohere/common.py
+-rw-r--r--   0        0        0     5813 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/langchain_cohere/embeddings.py
+-rw-r--r--   0        0        0     8058 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/langchain_cohere/llms.py
+-rw-r--r--   0        0        0        0 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/langchain_cohere/py.typed
+-rw-r--r--   0        0        0     3340 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/langchain_cohere/rag_retrievers.py
+-rw-r--r--   0        0        0        0 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/langchain_cohere/react_multi_hop/__init__.py
+-rw-r--r--   0        0        0     4913 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/langchain_cohere/react_multi_hop/agent.py
+-rw-r--r--   0        0        0     4060 2024-04-22 12:55:38.099136 langchain_cohere-0.1.4rc1/langchain_cohere/react_multi_hop/default_prompt_constants.py
+-rw-r--r--   0        0        0    11351 2024-04-22 12:55:38.103137 langchain_cohere-0.1.4rc1/langchain_cohere/react_multi_hop/parsing.py
+-rw-r--r--   0        0        0     9728 2024-04-22 12:55:38.103137 langchain_cohere-0.1.4rc1/langchain_cohere/react_multi_hop/prompt.py
+-rw-r--r--   0        0        0     4134 2024-04-22 12:55:38.103137 langchain_cohere-0.1.4rc1/langchain_cohere/rerank.py
+-rw-r--r--   0        0        0     1655 2024-04-22 12:55:38.103137 langchain_cohere-0.1.4rc1/langchain_cohere/utils.py
+-rw-r--r--   0        0        0     2682 2024-04-22 12:55:38.103137 langchain_cohere-0.1.4rc1/pyproject.toml
+-rw-r--r--   0        0        0     6413 1970-01-01 00:00:00.000000 langchain_cohere-0.1.4rc1/PKG-INFO
```

### Comparing `langchain_cohere-0.1.4rc0/LICENSE` & `langchain_cohere-0.1.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc0/README.md` & `langchain_cohere-0.1.4rc1/README.md`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc0/langchain_cohere/__init__.py` & `langchain_cohere-0.1.4rc1/langchain_cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc0/langchain_cohere/chat_models.py` & `langchain_cohere-0.1.4rc1/langchain_cohere/chat_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import uuid
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncIterator,
     Callable,
     Dict,
     Iterator,
@@ -29,14 +30,15 @@
 from langchain_core.messages import (
     AIMessage,
     AIMessageChunk,
     BaseMessage,
     ChatMessage,
     HumanMessage,
     SystemMessage,
+    ToolMessage,
 )
 from langchain_core.messages import (
     ToolCall as LC_ToolCall,
 )
 from langchain_core.output_parsers.base import OutputParserLike
 from langchain_core.output_parsers.openai_tools import (
     JsonOutputKeyToolsParser,
@@ -48,14 +50,47 @@
 from langchain_core.tools import BaseTool
 
 from langchain_cohere.cohere_agent import (
     _convert_to_cohere_tool,
     _format_to_cohere_tools,
 )
 from langchain_cohere.llms import BaseCohere
+from langchain_cohere.react_multi_hop.prompt import convert_to_documents
+
+
+def _messages_to_cohere_tool_results(
+    messages: List[BaseMessage],
+) -> List[Dict[str, Any]]:
+    """Get tool_results from messages."""
+    tool_results = []
+    for message in messages:
+        if isinstance(message, ToolMessage):
+            tool_message = message
+            previous_ai_msgs = [
+                message
+                for message in messages[:-1]
+                if isinstance(message, AIMessage) and message.tool_calls
+            ]
+            if previous_ai_msgs:
+                previous_ai_msg = previous_ai_msgs[-1]
+                tool_results.extend(
+                    [
+                        {
+                            "call": ToolCall(
+                                name=lc_tool_call["name"],
+                                parameters=lc_tool_call["args"],
+                            ),
+                            "outputs": convert_to_documents(tool_message.content),
+                        }
+                        for lc_tool_call in previous_ai_msg.tool_calls
+                        if lc_tool_call["id"] == tool_message.tool_call_id
+                    ]
+                )
+    return tool_results
+
 
 if TYPE_CHECKING:
     from cohere.types import ListModelsResponse  # noqa: F401
 
 
 def get_role(message: BaseMessage) -> str:
     """Get the role of the message.
@@ -131,19 +166,30 @@
 
     # by enabling automatic prompt truncation, the probability of request failure is
     # reduced with minimal impact on response quality
     prompt_truncation = (
         "AUTO" if formatted_docs is not None or connectors is not None else None
     )
 
+    tool_results: Optional[List[Dict[str, Any]]] = _messages_to_cohere_tool_results(
+        messages
+    )
+    if not tool_results:
+        tool_results = None
+
+    chat_history = [
+        {"role": get_role(x), "message": x.content}
+        for x in messages[:-1]
+        if not isinstance(x, ToolMessage)
+        and not (isinstance(x, AIMessage) and x.tool_calls)
+    ]
     req = {
         "message": messages[-1].content,
-        "chat_history": [
-            {"role": get_role(x), "message": x.content} for x in messages[:-1]
-        ],
+        "chat_history": chat_history,
+        "tool_results": tool_results,
         "documents": formatted_docs,
         "connectors": connectors,
         "prompt_truncation": prompt_truncation,
         "stop_sequences": stop_sequences,
         **kwargs,
     }
 
@@ -236,14 +282,15 @@
 
     @property
     def _default_params(self) -> Dict[str, Any]:
         """Get the default parameters for calling Cohere API."""
         base_params = {
             "model": self.model,
             "temperature": self.temperature,
+            "preamble": self.preamble,
         }
         return {k: v for k, v in base_params.items() if v is not None}
 
     @property
     def _identifying_params(self) -> Dict[str, Any]:
         """Get the identifying parameters."""
         return self._default_params
@@ -344,30 +391,33 @@
                 yield ChatGenerationChunk(
                     message=message,
                     generation_info=generation_info,
                 )
 
     def _get_generation_info(self, response: NonStreamedChatResponse) -> Dict[str, Any]:
         """Get the generation info from cohere API response."""
-        generation_info = {
+        generation_info: Dict[str, Any] = {
             "documents": response.documents,
             "citations": response.citations,
             "search_results": response.search_results,
             "search_queries": response.search_queries,
             "is_search_required": response.is_search_required,
             "generation_id": response.generation_id,
         }
         if response.tool_calls:
             # Only populate tool_calls when 1) present on the response and
             #  2) has one or more calls.
             generation_info["tool_calls"] = _format_cohere_tool_calls(
-                response.generation_id or "", response.tool_calls
+                response.tool_calls
             )
         if hasattr(response, "token_count"):
             generation_info["token_count"] = response.token_count
+        elif hasattr(response, "meta") and response.meta is not None:
+            if hasattr(response.meta, "tokens") and response.meta.tokens is not None:
+                generation_info["token_count"] = response.meta.tokens.dict()
         return generation_info
 
     def _generate(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
@@ -460,33 +510,34 @@
             model = self._get_default_model()
             self._default_model_name = model
 
         return len(self.client.tokenize(text=text, model=model).tokens)
 
 
 def _format_cohere_tool_calls(
-    generation_id: str, tool_calls: Optional[List[ToolCall]] = None
+    tool_calls: Optional[List[ToolCall]] = None,
 ) -> List[Dict]:
     """
     Formats a Cohere API response into the tool call format used elsewhere in Langchain.
     """
     if not tool_calls:
         return []
 
     formatted_tool_calls = []
     for tool_call in tool_calls:
         formatted_tool_calls.append(
             {
-                "id": generation_id,
+                "id": uuid.uuid4().hex[:],
                 "function": {
                     "name": tool_call.name,
                     "arguments": json.dumps(tool_call.parameters),
                 },
                 "type": "function",
             }
         )
     return formatted_tool_calls
 
 
 def _convert_cohere_tool_call_to_langchain(tool_call: ToolCall) -> LC_ToolCall:
     """Convert a Cohere tool call into langchain_core.messages.ToolCall"""
-    return LC_ToolCall(name=tool_call.name, args=tool_call.parameters, id=None)
+    _id = uuid.uuid4().hex[:]
+    return LC_ToolCall(name=tool_call.name, args=tool_call.parameters, id=_id)
```

### Comparing `langchain_cohere-0.1.4rc0/langchain_cohere/cohere_agent.py` & `langchain_cohere-0.1.4rc1/langchain_cohere/cohere_agent.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc0/langchain_cohere/common.py` & `langchain_cohere-0.1.4rc1/langchain_cohere/common.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc0/langchain_cohere/embeddings.py` & `langchain_cohere-0.1.4rc1/langchain_cohere/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc0/langchain_cohere/llms.py` & `langchain_cohere-0.1.4rc1/langchain_cohere/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc0/langchain_cohere/rag_retrievers.py` & `langchain_cohere-0.1.4rc1/langchain_cohere/rag_retrievers.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     from langchain_core.messages import BaseMessage
 
 
 def _get_docs(response: Any) -> List[Document]:
     docs = []
     if (
         "documents" in response.generation_info
-        and len(response.generation_info["documents"]) > 0
+        and response.generation_info["documents"]
     ):
         for doc in response.generation_info["documents"]:
             content = doc.get("snippet", None) or doc.get("text", None)
             if content is not None:
                 docs.append(Document(page_content=content, metadata=doc))
 
     docs.append(
```

### Comparing `langchain_cohere-0.1.4rc0/langchain_cohere/react_multi_hop/agent.py` & `langchain_cohere-0.1.4rc1/langchain_cohere/react_multi_hop/agent.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc0/langchain_cohere/react_multi_hop/default_prompt_constants.py` & `langchain_cohere-0.1.4rc1/langchain_cohere/react_multi_hop/default_prompt_constants.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc0/langchain_cohere/react_multi_hop/parsing.py` & `langchain_cohere-0.1.4rc1/langchain_cohere/react_multi_hop/parsing.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc0/langchain_cohere/react_multi_hop/prompt.py` & `langchain_cohere-0.1.4rc1/langchain_cohere/react_multi_hop/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc0/langchain_cohere/rerank.py` & `langchain_cohere-0.1.4rc1/langchain_cohere/rerank.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc0/langchain_cohere/utils.py` & `langchain_cohere-0.1.4rc1/langchain_cohere/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.4rc0/pyproject.toml` & `langchain_cohere-0.1.4rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-cohere"
-version = "0.1.4rc0"
+version = "0.1.4rc1"
 description = "An integration package connecting Cohere and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-cohere"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_cohere-0.1.4rc0/PKG-INFO` & `langchain_cohere-0.1.4rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-cohere
-Version: 0.1.4rc0
+Version: 0.1.4rc1
 Summary: An integration package connecting Cohere and LangChain
 Home-page: https://github.com/langchain-ai/langchain-cohere
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

