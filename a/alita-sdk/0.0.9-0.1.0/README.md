# Comparing `tmp/alita_sdk-0.0.9.tar.gz` & `tmp/alita_sdk-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alita_sdk-0.0.9.tar", last modified: Mon Mar 18 10:32:47 2024, max compression
+gzip compressed data, was "alita_sdk-0.1.0.tar", last modified: Wed Apr 24 11:06:08 2024, max compression
```

## Comparing `alita_sdk-0.0.9.tar` & `alita_sdk-0.1.0.tar`

### file list

```diff
@@ -1,36 +1,41 @@
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-18 10:32:47.414049 alita_sdk-0.0.9/
--rw-r--r--   0 arozumenko   (501) staff       (20)    11357 2024-03-08 11:24:37.000000 alita_sdk-0.0.9/LICENSE
--rw-r--r--   0 arozumenko   (501) staff       (20)     3905 2024-03-18 10:32:47.413834 alita_sdk-0.0.9/PKG-INFO
--rw-r--r--   0 arozumenko   (501) staff       (20)     3200 2024-03-10 12:01:09.000000 alita_sdk-0.0.9/README.md
--rw-r--r--   0 arozumenko   (501) staff       (20)      705 2024-03-18 10:32:28.000000 alita_sdk-0.0.9/pyproject.toml
--rw-r--r--   0 arozumenko   (501) staff       (20)       92 2024-03-10 17:05:00.000000 alita_sdk-0.0.9/requirements.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)       38 2024-03-18 10:32:47.414093 alita_sdk-0.0.9/setup.cfg
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-18 10:32:47.409391 alita_sdk-0.0.9/src/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:38.000000 alita_sdk-0.0.9/src/__init__.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-18 10:32:47.409477 alita_sdk-0.0.9/src/alita_sdk/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:50.000000 alita_sdk-0.0.9/src/alita_sdk/__init__.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-18 10:32:47.411252 alita_sdk-0.0.9/src/alita_sdk/agents/
--rw-r--r--   0 arozumenko   (501) staff       (20)     2412 2024-03-18 10:31:52.000000 alita_sdk-0.0.9/src/alita_sdk/agents/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     2993 2024-03-18 10:31:45.000000 alita_sdk-0.0.9/src/alita_sdk/agents/alita_openai.py
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-10 11:28:03.000000 alita_sdk-0.0.9/src/alita_sdk/agents/base_actions.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     2325 2024-03-13 17:32:26.000000 alita_sdk-0.0.9/src/alita_sdk/agents/mixedAgentParser.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     2283 2024-03-18 10:31:02.000000 alita_sdk-0.0.9/src/alita_sdk/agents/mixedAgentRenderes.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     1231 2024-03-13 15:14:36.000000 alita_sdk-0.0.9/src/alita_sdk/agents/utils.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-18 10:32:47.411929 alita_sdk-0.0.9/src/alita_sdk/clients/
--rw-r--r--   0 arozumenko   (501) staff       (20)       31 2024-03-09 15:53:40.000000 alita_sdk-0.0.9/src/alita_sdk/clients/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)    14057 2024-03-18 09:54:26.000000 alita_sdk-0.0.9/src/alita_sdk/clients/client.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-18 10:32:47.412627 alita_sdk-0.0.9/src/alita_sdk/llms/
--rw-r--r--   0 arozumenko   (501) staff       (20)       33 2024-03-09 14:45:23.000000 alita_sdk-0.0.9/src/alita_sdk/llms/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     8311 2024-03-10 11:45:00.000000 alita_sdk-0.0.9/src/alita_sdk/llms/alita.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-18 10:32:47.413373 alita_sdk-0.0.9/src/alita_sdk/tools/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-11 07:45:42.000000 alita_sdk-0.0.9/src/alita_sdk/tools/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)      863 2024-03-13 12:05:45.000000 alita_sdk-0.0.9/src/alita_sdk/tools/datasource.py
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-11 07:46:26.000000 alita_sdk-0.0.9/src/alita_sdk/tools/prompt.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-18 10:32:47.413469 alita_sdk-0.0.9/src/alita_sdk/utils/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-13 15:14:37.000000 alita_sdk-0.0.9/src/alita_sdk/utils/__init__.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-18 10:32:47.413606 alita_sdk-0.0.9/src/alita_sdk.egg-info/
--rw-r--r--   0 arozumenko   (501) staff       (20)     3905 2024-03-18 10:32:47.000000 alita_sdk-0.0.9/src/alita_sdk.egg-info/PKG-INFO
--rw-r--r--   0 arozumenko   (501) staff       (20)      749 2024-03-18 10:32:47.000000 alita_sdk-0.0.9/src/alita_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)        1 2024-03-18 10:32:47.000000 alita_sdk-0.0.9/src/alita_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)       93 2024-03-18 10:32:47.000000 alita_sdk-0.0.9/src/alita_sdk.egg-info/requires.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)       19 2024-03-18 10:32:47.000000 alita_sdk-0.0.9/src/alita_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:06:08.879981 alita_sdk-0.1.0/
+-rw-r--r--   0 arozumenko   (501) staff       (20)    11357 2024-03-08 11:24:37.000000 alita_sdk-0.1.0/LICENSE
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3939 2024-04-24 11:06:08.879762 alita_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3200 2024-03-10 12:01:09.000000 alita_sdk-0.1.0/README.md
+-rw-r--r--   0 arozumenko   (501) staff       (20)      705 2024-04-23 06:09:40.000000 alita_sdk-0.1.0/pyproject.toml
+-rw-r--r--   0 arozumenko   (501) staff       (20)      111 2024-04-24 11:05:21.000000 alita_sdk-0.1.0/requirements.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)       38 2024-04-24 11:06:08.880028 alita_sdk-0.1.0/setup.cfg
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:06:08.872859 alita_sdk-0.1.0/src/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:38.000000 alita_sdk-0.1.0/src/__init__.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:06:08.872964 alita_sdk-0.1.0/src/alita_sdk/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:50.000000 alita_sdk-0.1.0/src/alita_sdk/__init__.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:06:08.875017 alita_sdk-0.1.0/src/alita_sdk/agents/
+-rw-r--r--   0 arozumenko   (501) staff       (20)     2412 2024-03-18 10:31:52.000000 alita_sdk-0.1.0/src/alita_sdk/agents/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3030 2024-03-26 19:45:28.000000 alita_sdk-0.1.0/src/alita_sdk/agents/alita_openai.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-10 11:28:03.000000 alita_sdk-0.1.0/src/alita_sdk/agents/base_actions.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     2566 2024-04-03 10:33:12.000000 alita_sdk-0.1.0/src/alita_sdk/agents/mixedAgentParser.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     2283 2024-03-18 10:31:02.000000 alita_sdk-0.1.0/src/alita_sdk/agents/mixedAgentRenderes.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     1231 2024-03-13 15:14:36.000000 alita_sdk-0.1.0/src/alita_sdk/agents/utils.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:06:08.875266 alita_sdk-0.1.0/src/alita_sdk/clients/
+-rw-r--r--   0 arozumenko   (501) staff       (20)       31 2024-03-09 15:53:40.000000 alita_sdk-0.1.0/src/alita_sdk/clients/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)    17120 2024-04-23 06:28:54.000000 alita_sdk-0.1.0/src/alita_sdk/clients/client.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:06:08.875955 alita_sdk-0.1.0/src/alita_sdk/llms/
+-rw-r--r--   0 arozumenko   (501) staff       (20)       33 2024-03-09 14:45:23.000000 alita_sdk-0.1.0/src/alita_sdk/llms/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     8317 2024-03-26 15:53:02.000000 alita_sdk-0.1.0/src/alita_sdk/llms/alita.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:06:08.876981 alita_sdk-0.1.0/src/alita_sdk/toolkits/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-04-12 11:47:05.000000 alita_sdk-0.1.0/src/alita_sdk/toolkits/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     1985 2024-04-12 12:00:03.000000 alita_sdk-0.1.0/src/alita_sdk/toolkits/datasource.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      734 2024-04-12 11:47:16.000000 alita_sdk-0.1.0/src/alita_sdk/toolkits/prompt.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:06:08.878581 alita_sdk-0.1.0/src/alita_sdk/tools/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-11 07:45:42.000000 alita_sdk-0.1.0/src/alita_sdk/tools/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      743 2024-04-12 14:28:55.000000 alita_sdk-0.1.0/src/alita_sdk/tools/datasource.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      281 2024-04-12 14:28:45.000000 alita_sdk-0.1.0/src/alita_sdk/tools/prompt.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:06:08.879172 alita_sdk-0.1.0/src/alita_sdk/utils/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-13 15:14:37.000000 alita_sdk-0.1.0/src/alita_sdk/utils/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)    10148 2024-04-04 04:14:44.000000 alita_sdk-0.1.0/src/alita_sdk/utils/streamlit.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:06:08.879484 alita_sdk-0.1.0/src/alita_sdk.egg-info/
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3939 2024-04-24 11:06:08.000000 alita_sdk-0.1.0/src/alita_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 arozumenko   (501) staff       (20)      887 2024-04-24 11:06:08.000000 alita_sdk-0.1.0/src/alita_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)        1 2024-04-24 11:06:08.000000 alita_sdk-0.1.0/src/alita_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)      112 2024-04-24 11:06:08.000000 alita_sdk-0.1.0/src/alita_sdk.egg-info/requires.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)       19 2024-04-24 11:06:08.000000 alita_sdk-0.1.0/src/alita_sdk.egg-info/top_level.txt
```

### Comparing `alita_sdk-0.0.9/LICENSE` & `alita_sdk-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.0.9/PKG-INFO` & `alita_sdk-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alita_sdk
-Version: 0.0.9
+Version: 0.1.0
 Summary: SDK for building langchain agents using resouces from Alita
 Author-email: Artem Rozumenko <support@analysta.ai>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/alita-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: langchain_core==0.1.30
 Requires-Dist: langchain==0.1.11
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: openai==1.13.3
 Requires-Dist: python-dotenv==1.0.1
+Requires-Dist: alita_tools==0.0.9
 
 Alita SDK
 =========
 
 Alita SDK, built on top of Langchain, enables the creation of intelligent agents within the Alita Platform using project-specific prompts and data sources. This SDK is designed for developers looking to integrate advanced AI capabilities into their projects with ease.
 
 Prerequisites
```

### Comparing `alita_sdk-0.0.9/README.md` & `alita_sdk-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.0.9/pyproject.toml` & `alita_sdk-0.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alita_sdk"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Artem Rozumenko", email="support@analysta.ai" },
 ]
 description = "SDK for building langchain agents using resouces from Alita"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `alita_sdk-0.0.9/src/alita_sdk/agents/__init__.py` & `alita_sdk-0.1.0/src/alita_sdk/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.0.9/src/alita_sdk/agents/alita_openai.py` & `alita_sdk-0.1.0/src/alita_sdk/agents/alita_openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,20 +45,17 @@
             dumpd(self), input, name=config.get("run_name")
         )
         messages = []
         if input.get("intermediate_steps"):
             messages = format_to_messages(input["intermediate_steps"])
         print(input)
         try:
-            run = self._create_thread_and_run(
-                self.chat_history + 
-                input["chat_history"][:-1] + 
-                messages + 
-                [input["chat_history"][-1]]
-            )
+            mgs = self.chat_history + input["chat_history"][:-1] + messages + [input["chat_history"][-1]]
+            callback_manager.on_llm_start(dumpd(self), [message["content"] for message in mgs])
+            run = self._create_thread_and_run(mgs)
             response = self._get_response(run)
         except BaseException as e:
             run_manager.on_chain_error(e, metadata=format_exc())
             raise e
         else:
             run_manager.on_chain_end(response)
             return response
```

### Comparing `alita_sdk-0.0.9/src/alita_sdk/agents/mixedAgentParser.py` & `alita_sdk-0.1.0/src/alita_sdk/agents/mixedAgentParser.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,15 +54,22 @@
 {criticism}
 
 Running Tool:
 {action} with param {tool_input}
 """
         if action:
             if action == 'complete_task':
-                return AgentFinish({"output": tool_input[list(tool_input.keys())[0]]}, log=log)
+                
+                try:
+                    output = tool_input[list(tool_input.keys())[0]]
+                except AttributeError:
+                    output = tool_input
+                if output.strip() == "final_answer":
+                    output = txt
+                return AgentFinish({"output": output}, log=log)  
             return AgentAction(action, tool_input, log)
         elif txt:
             return AgentFinish({"output": txt}, log=log)
         else:
             raise OutputParserException(f"""ERROR: RESPONSE FORMAT IS INCORRECT
 The response may have a great data, format response to the required JSON strcuture. 
 Expected format: {FORMAT_INSTRUCTIONS}
```

### Comparing `alita_sdk-0.0.9/src/alita_sdk/agents/mixedAgentRenderes.py` & `alita_sdk-0.1.0/src/alita_sdk/agents/mixedAgentRenderes.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.0.9/src/alita_sdk/agents/utils.py` & `alita_sdk-0.1.0/src/alita_sdk/agents/utils.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.0.9/src/alita_sdk/clients/client.py` & `alita_sdk-0.1.0/src/alita_sdk/clients/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 import logging
 import requests
 from typing import Dict, List, Any, Optional
 from jinja2 import Environment, DebugUndefined, meta
+from langchain_core.pydantic_v1 import BaseModel, Field
 
 from langchain_core.messages import (
     AIMessage,
     HumanMessage,
     SystemMessage,
     BaseMessage,
     ToolMessage
 )
 from langchain_core.prompts import ChatPromptTemplate
 from langchain.agents import  AgentExecutor
+from langchain_core.utils.function_calling import convert_to_openai_function
 
 logger = logging.getLogger(__name__)
 from ..agents import create_mixed_agent
 from ..agents.alita_openai import AlitaAssistantRunnable
+from ..toolkits.prompt import PromptToolkit
+from ..toolkits.datasource import DatasourcesToolkit
+from alita_tools.openapi import AlitaOpenAPIToolkit
+from pydantic import create_model
 
 class Jinja2TemplatedChatMessagesTemplate(ChatPromptTemplate):
     
     def _resolve_variables(self, message:BaseMessage, kwargs:Dict) -> BaseMessage:
         environment = Environment(undefined=DebugUndefined)
         template = environment.from_string(message.content)
         content = template.render(kwargs)
@@ -50,18 +56,20 @@
             if isinstance(message_template, BaseMessage):
                 message = self._resolve_variables(message_template, kwargs)
                 logger.debug(message.content)
                 result.append(message)
         return result
     
 
-    
 class AlitaDataSource:
-    def __init__(self, alita:Any, datasource_id:int, datasource_settings, datasource_predict_settings):
+    def __init__(self, alita:Any, datasource_id:int, name:str, description: str,
+                 datasource_settings, datasource_predict_settings):
         self.alita = alita
+        self.name = name
+        self.description = description
         self.datasource_id = datasource_id
         self.datasource_settings = datasource_settings
         self.datasource_predict_settings = datasource_predict_settings
     
     def predict(self, user_input: str, chat_history: Optional[list[BaseMessage]]=[]):
         messages = chat_history + [HumanMessage(content=user_input)]
         return self.alita.rag(self.datasource_id, messages, 
@@ -69,14 +77,45 @@
                               self.datasource_predict_settings)
         
     def search(self, query: str):
         return self.alita.search(self.datasource_id, [HumanMessage(content=query)], 
                                   self.datasource_settings)
         
 
+class AlitaPrompt:
+    def __init__(self, alita:Any, prompt: ChatPromptTemplate, name:str, description: str, llm_settings: dict):
+        self.alita = alita
+        self.prompt = prompt
+        self.name = name
+        self.llm_settings = llm_settings
+        self.description = description
+    
+    def create_pydantic_model(self):
+        fields = {}
+        for variable in self.prompt.input_variables:
+            fields[variable] = (str, None)
+        if "input" not in list(fields.keys()):
+            fields["input"] = (str, None)
+        return create_model("PromptVariables", **fields)
+        
+    
+    def predict(self, variables: dict={}):
+        input = variables.pop("input", None)
+        alita_vars = []
+        for key, value in variables.items():
+            alita_vars.append({
+                "name": key,
+                "value": value
+            })
+        messages = [SystemMessage(content=self.prompt.messages[0].content), HumanMessage(content=input)]
+        result = []
+        for message in self.alita.predict(messages, self.llm_settings, variables=alita_vars):
+            result.append(message.content)
+        return "\n\n".join(result)
+
 
 class Assistant:
     def __init__(self, client:Any, prompt:ChatPromptTemplate, tools: list, 
                  openai_tools: Optional[Dict]=None):
         self.prompt = prompt
         self.client = client
         self.tools = tools
@@ -93,15 +132,15 @@
         return AgentExecutor.from_agent_and_tools(agent=agent, tools=self.tools,
                                                   verbose=True, handle_parsing_errors=True, 
                                                   max_execution_time=None,
                                                   return_intermediate_steps=True)
     
     # This one is used only in Alita OpenAI
     def apredict(self, messages: list[BaseMessage]):
-        yield from response = self.client.ainvoke([self.prompt.messages[0]] + messages, functions=self.openai_tools)
+        yield from self.client.ainvoke([self.prompt.messages[0]] + messages, functions=self.openai_tools)
     
     def predict(self, messages: list[BaseMessage]):
         response = self.client.invoke([self.prompt.messages[0]] + messages, functions=self.openai_tools)
         return response
     
 
 class AlitaClient:
@@ -114,18 +153,21 @@
         }
         self.predict_url = f"{self.base_url}/api/v1/prompt_lib/predict/prompt_lib/{self.project_id}"
         self.prompt_versions = f"{self.base_url}/api/v1/prompt_lib/version/prompt_lib/{self.project_id}"
         self.prompts = f"{self.base_url}/api/v1/prompt_lib/prompt/prompt_lib/{self.project_id}"
         self.datasources = f"{self.base_url}/api/v1/datasources/datasource/prompt_lib/{self.project_id}"
         self.datasources_predict = f"{self.base_url}/api/v1/datasources/predict/prompt_lib/{self.project_id}"
         self.datasources_search = f"{self.base_url}/api/v1/datasources/search/prompt_lib/{self.project_id}"
+        self.application_versions = f"{self.base_url}/api/v1/applications/version/prompt_lib/{self.project_id}"
+        
 
-    def prompt(self, prompt_id, prompt_version_id, chat_history=None):
+    def prompt(self, prompt_id, prompt_version_id, chat_history=None, return_tool=False):
         url = f"{self.prompt_versions}/{prompt_id}/{prompt_version_id}"
         data = requests.get(url, headers=self.headers).json()
+        model_settings = data['model_settings']
         messages = [SystemMessage(content=data['context'])]
         variables = {}
         if data['messages']:
             for message in data['messages']:
                 if message.get('role') == 'assistant':
                     messages.append(AIMessage(content=message['content']))
                 elif message.get('role') == 'user':
@@ -141,49 +183,77 @@
             else:
                 input_variables.append(variable['name'])
         template = Jinja2TemplatedChatMessagesTemplate(messages=messages)
         if input_variables and not variables:
             template.input_variables = input_variables
         if variables:
             template.partial_variables = variables
-        return template
+        if not return_tool:
+            return template
+        else:
+            url = f"{self.prompts}/{prompt_id}"
+            data = requests.get(url, headers=self.headers).json()
+            return AlitaPrompt(self, template, data['name'], data['description'], model_settings)
+
+    
+    def application(self, client: Any, application_id:int, application_version_id:int, tools: Optional[list] = []):
+        url = f"{self.application_versions}/{application_id}/{application_version_id}"
+        data = requests.get(url, headers=self.headers).json()
+        messages = [SystemMessage(content=data['instructions'])]
+        variables = {}
+        input_variables = []
+        for variable in data['variables']:
+            print(variable)
+            if variable['value'] != "":
+                variables[variable['name']] = variable['value']
+            else:
+                input_variables.append(variable['name'])
+        template = Jinja2TemplatedChatMessagesTemplate(messages=messages)
+        if input_variables and not variables:
+            template.input_variables = input_variables
+        if variables:
+            template.partial_variables = variables
+        if input_variables:
+            prompt_type = 'react'
+        else:
+            prompt_type = 'openai'
+        prompts = []
+        for tool in data['tools']:
+            if tool['type'] == 'prompt':
+                prompts.append([tool['settings']['prompt_id'], tool['settings']['prompt_version_id']])
+            elif tool['type'] == 'datasource':
+                tools += DatasourcesToolkit.get_toolkit(self, [tool['settings']['datasource_id']], tool['settings']['actions']).get_tools()
+            elif tool['type'] == 'openapi':
+                headers = {}
+                if tool['settings'].get('authentication'):
+                    if tool['settings']['authentication']['type'] == 'api_key': 
+                        auth_type = tool['settings']['authentication']['settings']['auth_type']
+                        auth_key = tool["settings"]["authentication"]["settings"]["api_key"]
+                        if auth_type.lower() == 'bearer':
+                            headers['Authorization'] = f'Bearer {auth_key}'
+                        if auth_type.lower() == 'basic':
+                            headers['Authorization'] = f'Basic {auth_key}'
+                        if auth_type.lower() == 'custom':
+                            headers[tool["settings"]["authentication"]["settings"]["custom_header_name"]] = f'{auth_key}'  
+                tools += AlitaOpenAPIToolkit.get_toolkit(tool['settings']['schema_settings'], headers={}).get_tools()
+        if len(prompts) > 0:
+            tools += PromptToolkit.get_toolkit(self, prompts).get_tools() 
+        if prompt_type == 'openai':
+            open_ai_funcs = [convert_to_openai_function(t) for t in tools]
+            return Assistant(client, template, tools, open_ai_funcs).getOpenAIAgentExecutor()
+        else:
+            return Assistant(client, template, tools).getAgentExecutor()
 
     def datasource(self, datasource_id:int) -> AlitaDataSource:
         url = f"{self.datasources}/{datasource_id}"
         data = requests.get(url, headers=self.headers).json()
-        ai_model = data['version_details']['datasource_settings']['chat']['chat_model']
-        datasource_model = data['version_details']['datasource_settings']['chat']['embedding_model']
-        temperature = data['version_details']['datasource_settings']['chat']['temperature']
-        top_p = data['version_details']['datasource_settings']['chat']['top_p']
-        top_k = data['version_details']['datasource_settings']['chat']['top_k']
-        max_length = data['version_details']['datasource_settings']['chat']['max_length']
-        stream = data['version_details']['datasource_settings']['chat'].get('stream', True)
-        cut_off_score = data['version_details']['datasource_settings']['chat'].get('cut_off_score', 0.5)
-        page_top_k = data['version_details']['datasource_settings']['chat'].get('page_top_k', 5)
-        fetch_k = data['version_details']['datasource_settings']['chat'].get('fetch_k', 30)
-        embedding_k = data['version_details']['datasource_settings']['chat'].get('embedding_k', 5)
-        datasource_settings = {
-            "embedding_integration_uid": datasource_model['integration_uid'],
-            "embedding_model_name": datasource_model['model_name'],
-            "cut_off_score": cut_off_score,
-            "page_top_k": page_top_k,
-            "fetch_k": fetch_k,
-            "top_k": embedding_k
-        }
-        datasource_predict_settings = {
-            "ai_integration_uid": ai_model["integration_uid"],
-            "ai_model_name": ai_model["model_name"],
-            "temperature": temperature,
-            "top_p": top_p,
-            "top_k": top_k,
-            "max_length": max_length,
-            "stream": stream,
-        }
-        return AlitaDataSource(self, datasource_id,datasource_settings, datasource_predict_settings)
-    
+        datasource_model = data['version_details']['datasource_settings']['chat']['chat_settings_embedding']
+        chat_model = data['version_details']['datasource_settings']['chat']['chat_settings_ai']
+        return AlitaDataSource(self, datasource_id, data["name"], data["description"],
+                               datasource_model, chat_model)
     
     def assistant(self, prompt_id: int, prompt_version_id: int, 
                   tools: list, openai_tools: Optional[Dict]=None, 
                   client: Optional[Any] = None):
         prompt = self.prompt(prompt_id=prompt_id, prompt_version_id=prompt_version_id)
         return Assistant(client, prompt, tools, openai_tools)
     
@@ -244,16 +314,17 @@
         response = requests.post(self.predict_url, headers=self.headers, json=prompt_data)
         if response.status_code != 200:
             logger.error("Error in response of predict: {response.content}")
             raise requests.exceptions.HTTPError(response.content)
         try:
             response_data = response.json()
             response_messages = []
+            print(response_data['messages'])
             for message in response_data['messages']:
-                if message.get('role') == 'user':
+                if message.get('type') == 'user':
                     response_messages.append(HumanMessage(content=message['content']))
                 else:
                     response_messages.append(AIMessage(content=message['content']))
             return response_messages
         except TypeError:
             logger.error(f"TypeError in response of predict: {response_data}")
             raise
@@ -279,19 +350,14 @@
         data = {
             "chat_history": [
                 {
                     "role": "user",
                     "content": user_input
                 }
             ],
-            "embedding_integration_uid": datasource_settings['embedding_integration_uid'],
-            "embedding_model_name": datasource_settings['embedding_model_name'],
-            "cut_off_score": datasource_settings["cut_off_score"],
-            "page_top_k": datasource_settings["page_top_k"],
-            "fetch_k": datasource_settings["fetch_k"],
-            "top_k": datasource_settings["top_k"]
+            "chat_settings_embedding": datasource_settings,
+            "str_content": True
         }
         headers = self.headers | {"Content-Type": "application/json"}
         response = requests.post(f"{self.datasources_search}/{datasource_id}", headers=headers, json=data).json()
         content = "\n\n".join([finding["page_content"] for finding in response["findings"]])
         return AIMessage(content=content, additional_kwargs={"references": response['references']})
-
```

### Comparing `alita_sdk-0.0.9/src/alita_sdk/llms/alita.py` & `alita_sdk-0.1.0/src/alita_sdk/llms/alita.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         return  {
                 "temperature": self.temperature,
                 "top_k": self.top_k,
                 "top_p": self.top_p,
                 "max_tokens": self.max_tokens,
                 "stream": self.stream_response,
                 "model": {
-                    "name": self.model_name,
+                    "model_name": self.model_name,
                     "integration_uid": self.integration_uid,
                 }
             }
     
     @property
     def _identifying_params(self) -> dict:
         """
```

### Comparing `alita_sdk-0.0.9/src/alita_sdk.egg-info/PKG-INFO` & `alita_sdk-0.1.0/src/alita_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alita_sdk
-Version: 0.0.9
+Version: 0.1.0
 Summary: SDK for building langchain agents using resouces from Alita
 Author-email: Artem Rozumenko <support@analysta.ai>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/alita-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: langchain_core==0.1.30
 Requires-Dist: langchain==0.1.11
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: openai==1.13.3
 Requires-Dist: python-dotenv==1.0.1
+Requires-Dist: alita_tools==0.0.9
 
 Alita SDK
 =========
 
 Alita SDK, built on top of Langchain, enables the creation of intelligent agents within the Alita Platform using project-specific prompts and data sources. This SDK is designed for developers looking to integrate advanced AI capabilities into their projects with ease.
 
 Prerequisites
```

### Comparing `alita_sdk-0.0.9/src/alita_sdk.egg-info/SOURCES.txt` & `alita_sdk-0.1.0/src/alita_sdk.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -15,11 +15,15 @@
 src/alita_sdk/agents/mixedAgentParser.py
 src/alita_sdk/agents/mixedAgentRenderes.py
 src/alita_sdk/agents/utils.py
 src/alita_sdk/clients/__init__.py
 src/alita_sdk/clients/client.py
 src/alita_sdk/llms/__init__.py
 src/alita_sdk/llms/alita.py
+src/alita_sdk/toolkits/__init__.py
+src/alita_sdk/toolkits/datasource.py
+src/alita_sdk/toolkits/prompt.py
 src/alita_sdk/tools/__init__.py
 src/alita_sdk/tools/datasource.py
 src/alita_sdk/tools/prompt.py
-src/alita_sdk/utils/__init__.py
+src/alita_sdk/utils/__init__.py
+src/alita_sdk/utils/streamlit.py
```

