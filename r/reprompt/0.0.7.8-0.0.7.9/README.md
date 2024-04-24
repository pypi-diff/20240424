# Comparing `tmp/reprompt-0.0.7.8.tar.gz` & `tmp/reprompt-0.0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reprompt-0.0.7.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "reprompt-0.0.7.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `reprompt-0.0.7.8.tar` & `reprompt-0.0.7.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      334 2024-04-04 23:08:33.473524 reprompt-0.0.7.8/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1157 2024-04-04 23:08:33.473643 reprompt-0.0.7.8/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      417 2024-04-04 23:08:33.473790 reprompt-0.0.7.8/.github/dependabot.yml
--rw-r--r--   0        0        0      418 2024-04-04 23:08:33.473883 reprompt-0.0.7.8/.github/template-sync.yml
--rw-r--r--   0        0        0      472 2024-04-07 21:52:20.071061 reprompt-0.0.7.8/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2024-04-07 21:52:20.071267 reprompt-0.0.7.8/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2024-04-19 03:54:13.429435 reprompt-0.0.7.8/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      368 2024-04-04 23:08:33.474380 reprompt-0.0.7.8/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      307 2024-04-19 03:54:13.429968 reprompt-0.0.7.8/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0     1799 2024-04-04 23:08:33.474551 reprompt-0.0.7.8/.gitignore
--rw-r--r--   0        0        0     1540 2024-04-04 23:08:33.474640 reprompt-0.0.7.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2024-04-04 23:08:33.474722 reprompt-0.0.7.8/.pypirc
--rw-r--r--   0        0        0      459 2024-04-04 23:08:33.474853 reprompt-0.0.7.8/.vscode/launch.json
--rw-r--r--   0        0        0      817 2024-04-04 23:08:33.474937 reprompt-0.0.7.8/.vscode/settings.json
--rw-r--r--   0        0        0     1127 2024-04-07 21:52:20.071438 reprompt-0.0.7.8/LICENSE
--rw-r--r--   0        0        0     7737 2024-04-19 03:54:13.430955 reprompt-0.0.7.8/README.md
--rw-r--r--   0        0        0      634 2024-04-04 23:08:33.475348 reprompt-0.0.7.8/docs/Makefile
--rw-r--r--   0        0        0     2321 2024-04-04 23:08:33.475439 reprompt-0.0.7.8/docs/conf.py
--rw-r--r--   0        0        0      360 2024-04-04 23:08:33.475525 reprompt-0.0.7.8/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-04-04 23:08:33.475604 reprompt-0.0.7.8/docs/developer.md
--rw-r--r--   0        0        0      468 2024-04-04 23:08:33.475685 reprompt-0.0.7.8/docs/index.rst
--rw-r--r--   0        0        0      800 2024-04-04 23:08:33.475772 reprompt-0.0.7.8/docs/make.bat
--rw-r--r--   0        0        0       51 2024-04-04 23:08:33.475852 reprompt-0.0.7.8/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-04-04 23:08:33.475929 reprompt-0.0.7.8/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-04-04 23:08:33.476081 reprompt-0.0.7.8/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-04-04 23:08:33.476163 reprompt-0.0.7.8/docs/pyproject.md
--rw-r--r--   0        0        0      425 2024-04-04 23:08:33.476254 reprompt-0.0.7.8/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      415 2024-04-04 23:08:33.476339 reprompt-0.0.7.8/docs/python_package.rst
--rw-r--r--   0        0        0       42 2024-04-04 23:08:33.476409 reprompt-0.0.7.8/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-04-04 23:08:33.476479 reprompt-0.0.7.8/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-04-04 23:08:33.476563 reprompt-0.0.7.8/docs/workflows.md
--rw-r--r--   0        0        0     6649 2024-04-19 03:54:13.431657 reprompt-0.0.7.8/pyproject.toml
--rw-r--r--   0        0        0     1281 2024-04-22 18:29:53.853436 reprompt-0.0.7.8/src/reprompt/__init__.py
--rw-r--r--   0        0        0      859 2024-04-07 23:40:24.407699 reprompt-0.0.7.8/src/reprompt/background_task_manager.py
--rw-r--r--   0        0        0      167 2024-04-19 03:54:13.432588 reprompt-0.0.7.8/src/reprompt/config.py
--rw-r--r--   0        0        0     3873 2024-04-22 18:19:11.940377 reprompt-0.0.7.8/src/reprompt/tracing.py
--rw-r--r--   0        0        0      989 2024-04-04 23:08:33.477233 reprompt-0.0.7.8/tests/conftest.py
--rw-r--r--   0        0        0      511 2024-04-07 21:52:20.073113 reprompt-0.0.7.8/tests/openai_example_script.py
--rw-r--r--   0        0        0      283 2024-04-07 21:52:20.073222 reprompt-0.0.7.8/tests/test_init.py
--rw-r--r--   0        0        0     1673 2024-04-07 21:52:20.073331 reprompt-0.0.7.8/tests/test_openai_tracing.py
--rw-r--r--   0        0        0     9640 1970-01-01 00:00:00.000000 reprompt-0.0.7.8/PKG-INFO
+-rw-r--r--   0        0        0      334 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1157 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      417 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/.github/dependabot.yml
+-rw-r--r--   0        0        0      418 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/.github/template-sync.yml
+-rw-r--r--   0        0        0      472 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      368 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      307 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0     1799 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/.gitignore
+-rw-r--r--   0        0        0     1540 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/.pypirc
+-rw-r--r--   0        0        0      459 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/.vscode/launch.json
+-rw-r--r--   0        0        0      817 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/.vscode/settings.json
+-rw-r--r--   0        0        0     1127 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/LICENSE
+-rw-r--r--   0        0        0    12833 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/README.md
+-rw-r--r--   0        0        0      634 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/docs/Makefile
+-rw-r--r--   0        0        0     2321 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/docs/developer.md
+-rw-r--r--   0        0        0      468 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/docs/make.bat
+-rw-r--r--   0        0        0       51 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/docs/pyproject.md
+-rw-r--r--   0        0        0      425 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      415 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/docs/python_package.rst
+-rw-r--r--   0        0        0       42 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/docs/workflows.md
+-rw-r--r--   0        0        0     6649 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/pyproject.toml
+-rw-r--r--   0        0        0     1297 2024-04-24 04:25:49.567207 reprompt-0.0.7.9/src/reprompt/__init__.py
+-rw-r--r--   0        0        0      859 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/src/reprompt/background_task_manager.py
+-rw-r--r--   0        0        0      167 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/src/reprompt/config.py
+-rw-r--r--   0        0        0     4732 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/src/reprompt/tracing.py
+-rw-r--r--   0        0        0      989 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/tests/conftest.py
+-rw-r--r--   0        0        0      511 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/tests/openai_example_script.py
+-rw-r--r--   0        0        0      283 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/tests/test_init.py
+-rw-r--r--   0        0        0     1673 2024-04-24 04:25:33.919212 reprompt-0.0.7.9/tests/test_openai_tracing.py
+-rw-r--r--   0        0        0    14736 1970-01-01 00:00:00.000000 reprompt-0.0.7.9/PKG-INFO
```

### Comparing `reprompt-0.0.7.8/.devcontainer/devcontainer.json` & `reprompt-0.0.7.9/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.8/.github/workflows/schedule-update-actions.yml` & `reprompt-0.0.7.9/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.8/.gitignore` & `reprompt-0.0.7.9/.gitignore`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.8/.pre-commit-config.yaml` & `reprompt-0.0.7.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.8/.vscode/settings.json` & `reprompt-0.0.7.9/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.8/LICENSE` & `reprompt-0.0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.8/docs/Makefile` & `reprompt-0.0.7.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.8/docs/conf.py` & `reprompt-0.0.7.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.8/docs/make.bat` & `reprompt-0.0.7.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.8/docs/pylint.md` & `reprompt-0.0.7.9/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.8/pyproject.toml` & `reprompt-0.0.7.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.8/src/reprompt/__init__.py` & `reprompt-0.0.7.9/src/reprompt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Reprompt"""
 
 from __future__ import annotations
 
 import logging
 
 from . import config
-from .tracing import FunctionTrace, get_edits, write_traces, write_traces_sync
+from .tracing import FunctionTrace, get_edits, get_edits_sync, write_traces, write_traces_sync
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 # IMPORTANT: setting version for Reprompt package
-__version__ = "0.0.7.8"
+__version__ = "0.0.7.9"
 # IMPORTANT: All the functions we want to expose publicly from the reprompt module
 __all__ = ["init", "FunctionTrace", "write_traces", "get_edits", "write_traces_sync"]
 
 
 def init(api_base_url: str = None, api_key: str = None, debug: bool = False):
     if debug:
         logger.setLevel(logging.DEBUG)
```

### Comparing `reprompt-0.0.7.8/src/reprompt/background_task_manager.py` & `reprompt-0.0.7.9/src/reprompt/background_task_manager.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.8/src/reprompt/tracing.py` & `reprompt-0.0.7.9/src/reprompt/tracing.py`

 * *Files 12% similar despite different names*

```diff
@@ -103,7 +103,29 @@
                     logger.error(f"Failed to fetch edits: ({response.status}) {error_message}")
                     return {"error": error_message}  # Return the error message in a dict
                 else:
                     logger.debug("Fetched example overrides")
                     return await response.json()
     except aiohttp.ClientError:
         logger.error("Cannot connect to reprompt to fetch edits")
+
+
+def get_edits_sync(input: str) -> dict:
+    if config.api_key is None:
+        logger.error("API key is required to fetch edits")
+        return
+
+    try:
+        response = requests.post(
+            f"{config.api_base_url}/api/overrides/get_example_overrides",
+            json={"input": input},
+            headers={"Content-Type": "application/json", "apiKey": config.api_key},
+        )
+        if response.status_code != 200:
+            logger.error(f"Failed to fetch edits: ({response.status_code}) {response.text}")
+            return {"error": response.text}
+        else:
+            logger.debug("Fetched example overrides")
+            return response.json()
+    except requests.exceptions.RequestException:
+        logger.error("Cannot connect to reprompt to fetch edits")
+        return {"error": "Cannot connect to reprompt to fetch edits"}
```

### Comparing `reprompt-0.0.7.8/tests/conftest.py` & `reprompt-0.0.7.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.8/tests/test_openai_tracing.py` & `reprompt-0.0.7.9/tests/test_openai_tracing.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.8/PKG-INFO` & `reprompt-0.0.7.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reprompt
-Version: 0.0.7.8
+Version: 0.0.7.9
 Summary: Reprompt
 Author-email: Lukas Martinelli <me@lukasmartinelli.ch>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -45,15 +45,15 @@
 
 
 # Installing Reprompt
 
 Specify the specific version of reprompt in your requirements.txt file.
 
 ```
-reprompt==0.0.7.4
+reprompt==0.0.7.8
 ```
 
 And install it.
 
 ```
 pip install -r requirements.txt
 ```
@@ -87,16 +87,119 @@
 
 ## Add edits
 
 Head over to [Reprompt Dashboard](https://app.repromptai.com/tune) and create a couple edits.
 
 ![](https://github.com/reprompt/reprompt/assets/1288339/85ff3dcc-1f97-4c7d-845f-00d3b49814a8)
 
+### Simple Integration Example
 
-### Full Integration Example
+```python
+from __future__ import annotations
+
+import json
+import os
+
+import openai
+import reprompt
+
+from fastapi import FastAPI, Request
+from starlette.responses import FileResponse
+
+openai.api_key = os.getenv("OPENAI_API_KEY")
+reprompt.init(api_key=os.getenv("OPENAI_API_KEY"))
+
+app = FastAPI(title="api")
+
+
+@app.post("/api/chat")
+async def chat_with_openai(request: Request):
+    body = await request.json()
+    print(body)
+    user_input = body["message"]
+
+    edits = await reprompt.get_edits(user_input)
+    prompt = """
+You are an AI assistant tasked with drafting responses to incoming emails.
+Your capabilities include understanding the content of each email, identifying the appropriate tone based on
+the context, and formulating clear, concise, and polite responses.
+
+"""
+
+    # Incorporate edits from reprompt
+    prompt += f"""
+### EXAMPLE ANSWERS ###
+{json.dumps(edits)}
+"""
+    response = openai.chat.completions.create(
+        model="gpt-3.5-turbo",
+        messages=[
+            {"role": "system", "content": prompt},
+            {"role": "user", "content": user_input},
+        ],
+    )
+    return {"response": response.choices[0].message.content}
+```
+
+### Integration tips
+
+**What are edits?**
+AI edits refer to the examples returned by the get_edits function. These edits are based on the feedback and adjustments made in the Reprompt dashboard, aimed at enhancing the model's responses.
+
+**What should I do with IF statements in my prompt?**
+If statements such as `If the email sounds angry or frustrated, start the reply with an apology.` or `If the received email is brief, keep the reply concise.` often don't work as expected in prompts. Instead of relying on conditional logic within the prompt, it's more effective to use examples. Providing GPT with clear examples of desired outputs can significantly improve the performance and relevance of the responses.
+
+**Do I need to change anything in my prompt to work with get_edits?**
+
+No significant changes are required in your prompt structure. The edits received from get_edits should be added to the end of your prompt as examples. These edits are designed to guide the model towards generating responses that align with your specific requirements.
+
+
+_Before integrating edits_
+Initially, the prompt might attempt to cover various scenarios with implicit IF statements or general instructions, lacking specificity or examples:
+
+```
+You are an AI assistant tasked with drafting responses to incoming emails. Your capabilities include understanding the content of each email, identifying the appropriate tone based on the context, and formulating clear, concise, and polite responses. Please ensure to apologize if the email sounds frustrated or angry, prioritize replies marked as urgent, and keep your responses brief if the original email is short.
+```
+
+_After integrating edits_
+After integrating edits, the prompt includes specific examples that guide the AI in handling various types of emails. These examples act as models for the AI to follow, improving its ability to generate appropriate responses:
+
+```
+You are an AI assistant tasked with drafting responses to incoming emails. Your capabilities include understanding the content of each email, identifying the appropriate tone based on the context, and formulating clear, concise, and polite responses.
+
+### EXAMPLE ANSWERS ###
+
+${json.dumps(edits)}
+```
+
+
+**How do I handle hardcoded examples in my prompt?**
+
+You should remove hardcoded examples from your prompt. This not only saves tokens but also allows the prompt to be more focused and targeted. Our platform enables your Product Manager (PM) to write examples that can be dynamically pulled in at query time, optimizing the prompt's effectiveness.
+
+
+**What information do I need to provide with the user message?**
+
+When using get_edits, you only need to tell us the user message. There's no need to include the entire prompt structure, as the edits provided will be appended to the bottom of your prompt as positive and negative examples.
+
+
+**Is chat history or a session ID required?**
+No, you don't need to provide chat history or a session ID. The get_edits functionality focuses on the current interaction.
+
+**What should I do with IF statements in my prompt?**
+IF statements often don't work as expected in prompts. Instead of relying on conditional logic within the prompt, it's more effective to use examples. Providing GPT with clear examples of desired outputs can significantly improve the performance and relevance of the responses.
+
+**Should I always call json.dumps on the edits?**
+It's not always necessary to use json.dumps on the edits unless you're incorporating them into a JSON-structured prompt or need to format them as a string for other reasons.
+
+**When I make edits in the Reprompt dashboard, does it need to be Markdown or JSON?**
+The format for editing examples should match the expected output format of your application. If you expect the output to be in Markdown, then the edits should also be made in Markdown to ensure consistency.
+
+
+### Integration Example with a RAG
 
 Here's how you might integrate Reprompt into a specific part of your FastAPI application, focusing on generating responses with OpenAI and using Reprompt for tracing and edits:
 
 
 ```python
 from fastapi import FastAPI, HTTPException, Request, JSONResponse
 import reprompt
@@ -269,9 +372,7 @@
     # Implement the logic to search with Weaviate
 
 def llm_generate_response(search_results):
     # Implement the logic to generate a response using an LLM
 
 ```
 
-
-
```

