# Comparing `tmp/agentkit-llm-0.1.5.tar.gz` & `tmp/agentkit-llm-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentkit-llm-0.1.5.tar", last modified: Mon Apr 22 15:36:53 2024, max compression
+gzip compressed data, was "agentkit-llm-0.1.6.tar", last modified: Wed Apr 24 17:53:06 2024, max compression
```

## Comparing `agentkit-llm-0.1.5.tar` & `agentkit-llm-0.1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-22 15:36:53.285534 agentkit-llm-0.1.5/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)    18656 2024-04-10 02:29:46.000000 agentkit-llm-0.1.5/LICENSE
--rw-r--r--   0 holmes    (1000) holmes    (1000)     7914 2024-04-22 15:36:53.285534 agentkit-llm-0.1.5/PKG-INFO
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     7187 2024-04-22 15:34:52.000000 agentkit-llm-0.1.5/README.md
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       38 2024-04-22 15:36:53.285534 agentkit-llm-0.1.5/setup.cfg
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      995 2024-04-22 15:35:35.000000 agentkit-llm-0.1.5/setup.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-22 15:36:53.281534 agentkit-llm-0.1.5/src/
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-22 15:36:53.285534 agentkit-llm-0.1.5/src/agentkit/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      191 2024-04-14 12:48:14.000000 agentkit-llm-0.1.5/src/agentkit/__init__.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2799 2024-04-14 16:35:34.000000 agentkit-llm-0.1.5/src/agentkit/after_query.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     9580 2024-04-14 12:48:55.000000 agentkit-llm-0.1.5/src/agentkit/base_node.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     6649 2024-04-08 08:17:28.000000 agentkit-llm-0.1.5/src/agentkit/compose_prompt.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      621 2024-04-08 07:53:38.000000 agentkit-llm-0.1.5/src/agentkit/exceptions.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)    14727 2024-04-08 11:31:02.000000 agentkit-llm-0.1.5/src/agentkit/graph.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-22 15:36:53.285534 agentkit-llm-0.1.5/src/agentkit/llm_api/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     3139 2024-04-22 15:31:39.000000 agentkit-llm-0.1.5/src/agentkit/llm_api/GPT.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     1479 2024-04-08 11:11:53.000000 agentkit-llm-0.1.5/src/agentkit/llm_api/__init__.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     3965 2024-04-08 11:05:44.000000 agentkit-llm-0.1.5/src/agentkit/llm_api/base.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     4473 2024-04-21 02:26:49.000000 agentkit-llm-0.1.5/src/agentkit/llm_api/claude.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     1473 2024-04-22 15:26:27.000000 agentkit-llm-0.1.5/src/agentkit/llm_api/utils.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2319 2024-04-14 12:49:05.000000 agentkit-llm-0.1.5/src/agentkit/node.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      488 2024-04-08 07:54:08.000000 agentkit-llm-0.1.5/src/agentkit/node_functions.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2213 2024-04-14 12:47:12.000000 agentkit-llm-0.1.5/src/agentkit/utils.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-22 15:36:53.285534 agentkit-llm-0.1.5/src/agentkit_llm.egg-info/
--rw-r--r--   0 holmes    (1000) holmes    (1000)     7914 2024-04-22 15:36:53.000000 agentkit-llm-0.1.5/src/agentkit_llm.egg-info/PKG-INFO
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      652 2024-04-22 15:36:53.000000 agentkit-llm-0.1.5/src/agentkit_llm.egg-info/SOURCES.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)        1 2024-04-22 15:36:53.000000 agentkit-llm-0.1.5/src/agentkit_llm.egg-info/dependency_links.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       51 2024-04-22 15:36:53.000000 agentkit-llm-0.1.5/src/agentkit_llm.egg-info/entry_points.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       71 2024-04-22 15:36:53.000000 agentkit-llm-0.1.5/src/agentkit_llm.egg-info/requires.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)        9 2024-04-22 15:36:53.000000 agentkit-llm-0.1.5/src/agentkit_llm.egg-info/top_level.txt
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-24 17:53:06.160235 agentkit-llm-0.1.6/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)    18656 2024-04-10 02:29:46.000000 agentkit-llm-0.1.6/LICENSE
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     8390 2024-04-24 17:53:06.160235 agentkit-llm-0.1.6/PKG-INFO
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     7906 2024-04-24 17:52:07.000000 agentkit-llm-0.1.6/README.md
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       38 2024-04-24 17:53:06.160235 agentkit-llm-0.1.6/setup.cfg
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      995 2024-04-24 17:35:02.000000 agentkit-llm-0.1.6/setup.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-24 17:53:06.156235 agentkit-llm-0.1.6/src/
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-24 17:53:06.156235 agentkit-llm-0.1.6/src/agentkit/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      191 2024-04-14 12:48:14.000000 agentkit-llm-0.1.6/src/agentkit/__init__.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2799 2024-04-14 16:35:34.000000 agentkit-llm-0.1.6/src/agentkit/after_query.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     9580 2024-04-14 12:48:55.000000 agentkit-llm-0.1.6/src/agentkit/base_node.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     6649 2024-04-08 08:17:28.000000 agentkit-llm-0.1.6/src/agentkit/compose_prompt.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      621 2024-04-08 07:53:38.000000 agentkit-llm-0.1.6/src/agentkit/exceptions.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)    14727 2024-04-08 11:31:02.000000 agentkit-llm-0.1.6/src/agentkit/graph.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-24 17:53:06.156235 agentkit-llm-0.1.6/src/agentkit/llm_api/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     5142 2024-04-24 17:42:15.000000 agentkit-llm-0.1.6/src/agentkit/llm_api/GPT.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     1479 2024-04-08 11:11:53.000000 agentkit-llm-0.1.6/src/agentkit/llm_api/__init__.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     3992 2024-04-24 17:36:07.000000 agentkit-llm-0.1.6/src/agentkit/llm_api/base.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     4615 2024-04-24 17:43:52.000000 agentkit-llm-0.1.6/src/agentkit/llm_api/claude.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     1473 2024-04-22 15:26:27.000000 agentkit-llm-0.1.6/src/agentkit/llm_api/utils.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2319 2024-04-14 12:49:05.000000 agentkit-llm-0.1.6/src/agentkit/node.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      488 2024-04-08 07:54:08.000000 agentkit-llm-0.1.6/src/agentkit/node_functions.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2213 2024-04-14 12:47:12.000000 agentkit-llm-0.1.6/src/agentkit/utils.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-24 17:53:06.160235 agentkit-llm-0.1.6/src/agentkit_llm.egg-info/
+-rw-r--r--   0 holmes    (1000) holmes    (1000)     8390 2024-04-24 17:53:06.000000 agentkit-llm-0.1.6/src/agentkit_llm.egg-info/PKG-INFO
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      652 2024-04-24 17:53:06.000000 agentkit-llm-0.1.6/src/agentkit_llm.egg-info/SOURCES.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)        1 2024-04-24 17:53:06.000000 agentkit-llm-0.1.6/src/agentkit_llm.egg-info/dependency_links.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       51 2024-04-24 17:53:06.000000 agentkit-llm-0.1.6/src/agentkit_llm.egg-info/entry_points.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       71 2024-04-24 17:53:06.000000 agentkit-llm-0.1.6/src/agentkit_llm.egg-info/requires.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)        9 2024-04-24 17:53:06.000000 agentkit-llm-0.1.6/src/agentkit_llm.egg-info/top_level.txt
```

### Comparing `agentkit-llm-0.1.5/LICENSE` & `agentkit-llm-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.5/PKG-INFO` & `agentkit-llm-0.1.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: agentkit-llm
-Version: 0.1.5
-Summary: A LLM prompting framework for LLM agents
-Home-page: https://github.com/Holmeswww/AgentKit
-Author: AgentKit Team
-License: CC-BY-4.0-Attribution
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: colorama
-Requires-Dist: numpy
-Provides-Extra: logging
-Requires-Dist: wandb; extra == "logging"
-Provides-Extra: all
-Requires-Dist: wandb; extra == "all"
-Requires-Dist: openai; extra == "all"
-Requires-Dist: anthropic; extra == "all"
-Requires-Dist: tiktoken; extra == "all"
-
 <div align="center">
 <img src="https://github.com/Holmeswww/AgentKit/raw/main/imgs/AgentKit.png" width="350px">
 
 **AgentKit: Flow Engineering with Graphs, not Coding**
 
 [[Arxiv Paper]](https://arxiv.org/abs/2404.11483)
 [[PDF]](https://arxiv.org/pdf/2404.11483.pdf)
@@ -49,14 +27,15 @@
 # Contents
 
 - [Installation](#Installation)
 - [Getting Started](#Getting-Started)
 - [Using Built-in LLM_API](#Built-in-LLM-API)
 - [Using AgentKit without Programming Experience](#Using-AgentKit-without-Programming-Experience)
 - [Node Components](#Node-Components)
+- [Commonly Asked Questions](#Commonly-Asked-Questions)
 - [Citing AgnetKit](#Citing-AgentKit)
 
 # Installation
 
 Installing the AgentKit stable version is as simple as:
 
 ```bash
@@ -132,14 +111,16 @@
 
 The built-in `agentkit.llm_api` functions require installing with `[all]` setting. See [the installation guide](#Installation) for details.
 
 Currently, the built-in API supports OpenAI and Anthropic, see https://pypi.org/project/openai/ and https://pypi.org/project/anthropic/ for details.
 
 To use the OpenAI models, set environment variables `OPENAI_KEY` and `OPENAI_ORG`. Alternatively, you can put the openai 'key' and 'organization' in the first 2 lines of `~/.openai/openai.key`.
 
+To use the Azure OpenAI models, set environment variables `AZURE_OPENAI_API_KEY`, `AZURE_OPENAI_API_VERSION`, `AZURE_OPENAI_ENDPOINT`, and `AZURE_DEPLOYMENT_NAME`. Alternatively, you can store the Azure OpenAI API key, API version, Azure endpoint, and deployment name in the first 4 lines of `~/.openai/azure_openai.key`.
+
 To use the Anthropic models, set environment variable `ANTHROPIC_KEY`. Alternatively, you can put the anthropic 'key' in 3rd line of `~/.openai/openai.key`.
 
 # Using AgentKit without Programming Experience
 
 First, follow [the installation guide](#Installation) to install AgentKit with `[all]` setting.
 
 Then, set environment variables `OPENAI_KEY` and `OPENAI_ORG` to be your OpenAI key and org_key.
@@ -156,14 +137,20 @@
 # Node Components
 
 ![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/node_archi.png)
 Inside each node (as shown to the left of the figure), AgentKit runs a built-in flow that **preprocesses** the input (Compose), queries the LLM with a preprocessed input and prompt $q_v$, and optionally **postprocesses** the output of the LLM (After-query).
 
 To support advanced capabilities such as branching, AgentKit offers API to dynamically modify the DAG at inference time (as shown to the right of the figure). Nodes/edges could be dynamically added or removed based on the LLM response at some ancestor nodes.
 
+# Commonly Asked Questions
+
+**Q:** I'm using the default `agentkit.llm_api`, and `graph.evaluate()` seems to be stuck.
+
+**A:** The LLM_API function catches and retries all API errors by default. Set `verbose=True` for each node to see which node you are stuck on, and `LLM_API_FUNCTION.debug=True` to see what error is causing the error.
+
 # Citing AgentKit
 ```bibtex
 @article{wu2024agentkit,
     title={AgentKit: Flow Engineering with Graphs, not Coding}, 
     author={Yue Wu and Yewen Fan and So Yeon Min and Shrimai Prabhumoye and Stephen McAleer and Yonatan Bisk and Ruslan Salakhutdinov and Yuanzhi Li and Tom Mitchell},
     year={2024},
     journal={arXiv preprint arXiv:2404.11483}
```

### Comparing `agentkit-llm-0.1.5/README.md` & `agentkit-llm-0.1.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: agentkit-llm
+Version: 0.1.6
+Summary: A LLM prompting framework for LLM agents
+Home-page: https://github.com/Holmeswww/AgentKit
+Author: AgentKit Team
+License: CC-BY-4.0-Attribution
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Description-Content-Type: text/markdown
+Provides-Extra: logging
+Provides-Extra: all
+License-File: LICENSE
+
 <div align="center">
 <img src="https://github.com/Holmeswww/AgentKit/raw/main/imgs/AgentKit.png" width="350px">
 
 **AgentKit: Flow Engineering with Graphs, not Coding**
 
 [[Arxiv Paper]](https://arxiv.org/abs/2404.11483)
 [[PDF]](https://arxiv.org/pdf/2404.11483.pdf)
@@ -27,14 +42,15 @@
 # Contents
 
 - [Installation](#Installation)
 - [Getting Started](#Getting-Started)
 - [Using Built-in LLM_API](#Built-in-LLM-API)
 - [Using AgentKit without Programming Experience](#Using-AgentKit-without-Programming-Experience)
 - [Node Components](#Node-Components)
+- [Commonly Asked Questions](#Commonly-Asked-Questions)
 - [Citing AgnetKit](#Citing-AgentKit)
 
 # Installation
 
 Installing the AgentKit stable version is as simple as:
 
 ```bash
@@ -110,14 +126,16 @@
 
 The built-in `agentkit.llm_api` functions require installing with `[all]` setting. See [the installation guide](#Installation) for details.
 
 Currently, the built-in API supports OpenAI and Anthropic, see https://pypi.org/project/openai/ and https://pypi.org/project/anthropic/ for details.
 
 To use the OpenAI models, set environment variables `OPENAI_KEY` and `OPENAI_ORG`. Alternatively, you can put the openai 'key' and 'organization' in the first 2 lines of `~/.openai/openai.key`.
 
+To use the Azure OpenAI models, set environment variables `AZURE_OPENAI_API_KEY`, `AZURE_OPENAI_API_VERSION`, `AZURE_OPENAI_ENDPOINT`, and `AZURE_DEPLOYMENT_NAME`. Alternatively, you can store the Azure OpenAI API key, API version, Azure endpoint, and deployment name in the first 4 lines of `~/.openai/azure_openai.key`.
+
 To use the Anthropic models, set environment variable `ANTHROPIC_KEY`. Alternatively, you can put the anthropic 'key' in 3rd line of `~/.openai/openai.key`.
 
 # Using AgentKit without Programming Experience
 
 First, follow [the installation guide](#Installation) to install AgentKit with `[all]` setting.
 
 Then, set environment variables `OPENAI_KEY` and `OPENAI_ORG` to be your OpenAI key and org_key.
@@ -134,14 +152,20 @@
 # Node Components
 
 ![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/node_archi.png)
 Inside each node (as shown to the left of the figure), AgentKit runs a built-in flow that **preprocesses** the input (Compose), queries the LLM with a preprocessed input and prompt $q_v$, and optionally **postprocesses** the output of the LLM (After-query).
 
 To support advanced capabilities such as branching, AgentKit offers API to dynamically modify the DAG at inference time (as shown to the right of the figure). Nodes/edges could be dynamically added or removed based on the LLM response at some ancestor nodes.
 
+# Commonly Asked Questions
+
+**Q:** I'm using the default `agentkit.llm_api`, and `graph.evaluate()` seems to be stuck.
+
+**A:** The LLM_API function catches and retries all API errors by default. Set `verbose=True` for each node to see which node you are stuck on, and `LLM_API_FUNCTION.debug=True` to see what error is causing the error.
+
 # Citing AgentKit
 ```bibtex
 @article{wu2024agentkit,
     title={AgentKit: Flow Engineering with Graphs, not Coding}, 
     author={Yue Wu and Yewen Fan and So Yeon Min and Shrimai Prabhumoye and Stephen McAleer and Yonatan Bisk and Ruslan Salakhutdinov and Yuanzhi Li and Tom Mitchell},
     year={2024},
     journal={arXiv preprint arXiv:2404.11483}
@@ -152,8 +176,8 @@
 
 <a href="https://star-history.com/#holmeswww/agentkit&Date">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=holmeswww/agentkit&type=Date&theme=dark" />
    <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=holmeswww/agentkit&type=Date" />
    <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=holmeswww/agentkit&type=Date" />
  </picture>
-</a>
+</a>
```

### Comparing `agentkit-llm-0.1.5/setup.py` & `agentkit-llm-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import pkg_resources
 import pathlib
 
 PKG_NAME = "agentkit-llm"
-VERSION = "0.1.5"
+VERSION = "0.1.6"
 EXTRAS = {
     "logging": ["wandb"],
     "all": ["wandb", "openai", "anthropic", "tiktoken"],
 }
 
 setuptools.setup(
     name=PKG_NAME,
```

### Comparing `agentkit-llm-0.1.5/src/agentkit/after_query.py` & `agentkit-llm-0.1.6/src/agentkit/after_query.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.5/src/agentkit/base_node.py` & `agentkit-llm-0.1.6/src/agentkit/base_node.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.5/src/agentkit/compose_prompt.py` & `agentkit-llm-0.1.6/src/agentkit/compose_prompt.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.5/src/agentkit/exceptions.py` & `agentkit-llm-0.1.6/src/agentkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.5/src/agentkit/graph.py` & `agentkit-llm-0.1.6/src/agentkit/graph.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.5/src/agentkit/llm_api/__init__.py` & `agentkit-llm-0.1.6/src/agentkit/llm_api/__init__.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.5/src/agentkit/llm_api/base.py` & `agentkit-llm-0.1.6/src/agentkit/llm_api/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     model_max = 2048
 
     def __init__(self, model_name, global_conter=None, model_type = "chat"):
         self.name = model_name
         assert model_type in ["chat", "completion"], "type should be either 'chat' or 'completion'"
         self.type = model_type
         self.global_counter = global_conter
+        self.debug = False
     
     def query_chat(self, messages, shrink_idx, model, max_gen=1024, temp=0.):
         raise NotImplementedError
     
     def query_completion(self, messages, shrink_idx, model, max_gen=1024, temp=0.):
         raise NotImplementedError
```

### Comparing `agentkit-llm-0.1.5/src/agentkit/llm_api/claude.py` & `agentkit-llm-0.1.6/src/agentkit/llm_api/claude.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,22 +85,24 @@
                     model=self.name,
                     system=system,
                     messages=messages,
                     temperature=temp,
                     max_tokens=max_gen,
                 )
                 return message.content[0].text, {"prompt":message.usage.input_tokens, "completion":message.usage.output_tokens, "total":message.usage.input_tokens+message.usage.output_tokens}
-            except (anthropic.APIConnectionError, anthropic.APIStatusError, anthropic.InternalServerError) as e:
-                time.sleep(30)
-            except anthropic.RateLimitError as e:
-                time.sleep(5*60)
             except Exception as e:
-                e = str(e)
-                if "However, your messages resulted in" in e:
-                    print("error:", e)
+                if self.debug:
+                    raise e
+                elif isinstance(e, anthropic.APIConnectionError) or isinstance(e, anthropic.APIStatusError) or isinstance(e, anthropic.InternalServerError):
+                    time.sleep(30)
+                elif isinstance(e, anthropic.RateLimitError):
+                    time.sleep(5*60)
+                elif "However, your messages resulted in" in str(e):
+                    print("error:", e, str(e))
+                    e = str(e)
                     index = e.find("your messages resulted in ")
                     import re
                     val = int(re.findall(r'\d+', e[index + len("your messages resulted in ") : ])[0])
                     index2 = e.find("maximum context length is ")
                     model_max = int(re.findall(r'\d+', e[index2 + len("maximum context length is "):])[0])
                     messages = self.shrink_msg_by(messages, shrink_idx, val-model_max)
                 else:
```

### Comparing `agentkit-llm-0.1.5/src/agentkit/llm_api/utils.py` & `agentkit-llm-0.1.6/src/agentkit/llm_api/utils.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.5/src/agentkit/node.py` & `agentkit-llm-0.1.6/src/agentkit/node.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.5/src/agentkit/utils.py` & `agentkit-llm-0.1.6/src/agentkit/utils.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.5/src/agentkit_llm.egg-info/PKG-INFO` & `agentkit-llm-0.1.6/src/agentkit_llm.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 Metadata-Version: 2.1
 Name: agentkit-llm
-Version: 0.1.5
+Version: 0.1.6
 Summary: A LLM prompting framework for LLM agents
 Home-page: https://github.com/Holmeswww/AgentKit
 Author: AgentKit Team
 License: CC-BY-4.0-Attribution
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: colorama
-Requires-Dist: numpy
 Provides-Extra: logging
-Requires-Dist: wandb; extra == "logging"
 Provides-Extra: all
-Requires-Dist: wandb; extra == "all"
-Requires-Dist: openai; extra == "all"
-Requires-Dist: anthropic; extra == "all"
-Requires-Dist: tiktoken; extra == "all"
+License-File: LICENSE
 
 <div align="center">
 <img src="https://github.com/Holmeswww/AgentKit/raw/main/imgs/AgentKit.png" width="350px">
 
 **AgentKit: Flow Engineering with Graphs, not Coding**
 
 [[Arxiv Paper]](https://arxiv.org/abs/2404.11483)
@@ -49,14 +42,15 @@
 # Contents
 
 - [Installation](#Installation)
 - [Getting Started](#Getting-Started)
 - [Using Built-in LLM_API](#Built-in-LLM-API)
 - [Using AgentKit without Programming Experience](#Using-AgentKit-without-Programming-Experience)
 - [Node Components](#Node-Components)
+- [Commonly Asked Questions](#Commonly-Asked-Questions)
 - [Citing AgnetKit](#Citing-AgentKit)
 
 # Installation
 
 Installing the AgentKit stable version is as simple as:
 
 ```bash
@@ -132,14 +126,16 @@
 
 The built-in `agentkit.llm_api` functions require installing with `[all]` setting. See [the installation guide](#Installation) for details.
 
 Currently, the built-in API supports OpenAI and Anthropic, see https://pypi.org/project/openai/ and https://pypi.org/project/anthropic/ for details.
 
 To use the OpenAI models, set environment variables `OPENAI_KEY` and `OPENAI_ORG`. Alternatively, you can put the openai 'key' and 'organization' in the first 2 lines of `~/.openai/openai.key`.
 
+To use the Azure OpenAI models, set environment variables `AZURE_OPENAI_API_KEY`, `AZURE_OPENAI_API_VERSION`, `AZURE_OPENAI_ENDPOINT`, and `AZURE_DEPLOYMENT_NAME`. Alternatively, you can store the Azure OpenAI API key, API version, Azure endpoint, and deployment name in the first 4 lines of `~/.openai/azure_openai.key`.
+
 To use the Anthropic models, set environment variable `ANTHROPIC_KEY`. Alternatively, you can put the anthropic 'key' in 3rd line of `~/.openai/openai.key`.
 
 # Using AgentKit without Programming Experience
 
 First, follow [the installation guide](#Installation) to install AgentKit with `[all]` setting.
 
 Then, set environment variables `OPENAI_KEY` and `OPENAI_ORG` to be your OpenAI key and org_key.
@@ -156,14 +152,20 @@
 # Node Components
 
 ![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/node_archi.png)
 Inside each node (as shown to the left of the figure), AgentKit runs a built-in flow that **preprocesses** the input (Compose), queries the LLM with a preprocessed input and prompt $q_v$, and optionally **postprocesses** the output of the LLM (After-query).
 
 To support advanced capabilities such as branching, AgentKit offers API to dynamically modify the DAG at inference time (as shown to the right of the figure). Nodes/edges could be dynamically added or removed based on the LLM response at some ancestor nodes.
 
+# Commonly Asked Questions
+
+**Q:** I'm using the default `agentkit.llm_api`, and `graph.evaluate()` seems to be stuck.
+
+**A:** The LLM_API function catches and retries all API errors by default. Set `verbose=True` for each node to see which node you are stuck on, and `LLM_API_FUNCTION.debug=True` to see what error is causing the error.
+
 # Citing AgentKit
 ```bibtex
 @article{wu2024agentkit,
     title={AgentKit: Flow Engineering with Graphs, not Coding}, 
     author={Yue Wu and Yewen Fan and So Yeon Min and Shrimai Prabhumoye and Stephen McAleer and Yonatan Bisk and Ruslan Salakhutdinov and Yuanzhi Li and Tom Mitchell},
     year={2024},
     journal={arXiv preprint arXiv:2404.11483}
```

### Comparing `agentkit-llm-0.1.5/src/agentkit_llm.egg-info/SOURCES.txt` & `agentkit-llm-0.1.6/src/agentkit_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

