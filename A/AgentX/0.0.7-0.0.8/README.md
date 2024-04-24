# Comparing `tmp/AgentX-0.0.7.tar.gz` & `tmp/agentx-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AgentX-0.0.7.tar", last modified: Mon Apr  8 08:36:13 2024, max compression
+gzip compressed data, was "agentx-0.0.8.tar", last modified: Thu Apr 18 15:57:18 2024, max compression
```

## Comparing `AgentX-0.0.7.tar` & `agentx-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,50 @@
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-08 08:36:13.554272 AgentX-0.0.7/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1076 2024-04-08 08:24:45.000000 AgentX-0.0.7/LICENSE
--rw-r--r--   0 erfan     (1000) erfan     (1000)     4699 2024-04-08 08:36:13.554272 AgentX-0.0.7/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2907 2024-04-08 08:24:45.000000 AgentX-0.0.7/README.md
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1617 2024-04-08 08:31:18.000000 AgentX-0.0.7/pyproject.toml
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2024-04-08 08:36:13.554272 AgentX-0.0.7/setup.cfg
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-08 08:36:13.554272 AgentX-0.0.7/src/
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-08 08:36:13.554272 AgentX-0.0.7/src/AgentX.egg-info/
--rw-r--r--   0 erfan     (1000) erfan     (1000)     4699 2024-04-08 08:36:13.000000 AgentX-0.0.7/src/AgentX.egg-info/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      201 2024-04-08 08:36:13.000000 AgentX-0.0.7/src/AgentX.egg-info/SOURCES.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2024-04-08 08:36:13.000000 AgentX-0.0.7/src/AgentX.egg-info/dependency_links.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      404 2024-04-08 08:36:13.000000 AgentX-0.0.7/src/AgentX.egg-info/requires.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2024-04-08 08:36:13.000000 AgentX-0.0.7/src/AgentX.egg-info/top_level.txt
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-18 15:57:18.976785 agentx-0.0.8/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1076 2024-04-08 08:24:45.000000 agentx-0.0.8/LICENSE
+-rw-r--r--   0 erfan     (1000) erfan     (1000)     4699 2024-04-18 15:57:18.976785 agentx-0.0.8/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2907 2024-04-08 08:24:45.000000 agentx-0.0.8/README.md
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1677 2024-04-18 15:52:38.000000 agentx-0.0.8/pyproject.toml
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2024-04-18 15:57:18.976785 agentx-0.0.8/setup.cfg
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-18 15:57:18.976785 agentx-0.0.8/src/
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-18 15:57:18.976785 agentx-0.0.8/src/AgentX.egg-info/
+-rw-r--r--   0 erfan     (1000) erfan     (1000)     4699 2024-04-18 15:57:18.000000 agentx-0.0.8/src/AgentX.egg-info/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1287 2024-04-18 15:57:18.000000 agentx-0.0.8/src/AgentX.egg-info/SOURCES.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2024-04-18 15:57:18.000000 agentx-0.0.8/src/AgentX.egg-info/dependency_links.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      404 2024-04-18 15:57:18.000000 agentx-0.0.8/src/AgentX.egg-info/requires.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        7 2024-04-18 15:57:18.000000 agentx-0.0.8/src/AgentX.egg-info/top_level.txt
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-18 15:57:18.976785 agentx-0.0.8/src/agentx/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      377 2024-04-18 15:23:07.000000 agentx-0.0.8/src/agentx/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-18 15:57:18.976785 agentx-0.0.8/src/agentx/agents/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       90 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/agents/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-18 15:57:18.976785 agentx-0.0.8/src/agentx/agents/action/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       32 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/agents/action/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2417 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/agents/action/action.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1297 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/agents/action/prompt.jinja2
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-18 15:57:18.976785 agentx-0.0.8/src/agentx/agents/chat/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       27 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/agents/chat/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1723 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/agents/chat/chat.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      679 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/agents/chat/prompt.jinja2
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-18 15:57:18.976785 agentx-0.0.8/src/agentx/agents/coder/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       30 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/agents/coder/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3675 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/agents/coder/coder.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2282 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/agents/coder/prompt.jinja2
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-18 15:57:18.976785 agentx-0.0.8/src/agentx/data_reader/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      102 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/data_reader/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2165 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/data_reader/loaders.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-18 15:57:18.976785 agentx-0.0.8/src/agentx/engine/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      103 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/engine/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      446 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/engine/configuration.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    28923 2024-04-18 15:56:24.000000 agentx-0.0.8/src/agentx/engine/engine.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-18 15:57:18.976785 agentx-0.0.8/src/agentx/llama_cpp/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      389 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/llama_cpp/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    15796 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/llama_cpp/_configuration.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      409 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/llama_cpp/_quantize.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1208 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/llama_cpp/_utils.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    13244 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/llama_cpp/inference.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-04-18 15:57:18.976785 agentx-0.0.8/src/agentx/prompt_templates/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       46 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/prompt_templates/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      446 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/prompt_templates/prompt_template_chatml.jinja2
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      594 2024-04-08 08:30:57.000000 agentx-0.0.8/src/agentx/prompt_templates/prompt_template_gemma.jinja2
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      471 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/prompt_templates/prompt_template_llama.jinja2
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      222 2024-04-08 08:32:08.000000 agentx-0.0.8/src/agentx/prompt_templates/prompt_template_open_chat.jinja2
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      429 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/prompt_templates/prompt_template_zephyr.jinja2
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1796 2024-04-08 08:24:45.000000 agentx-0.0.8/src/agentx/prompt_templates/prompt_templates.py
```

### Comparing `AgentX-0.0.7/LICENSE` & `agentx-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `AgentX-0.0.7/PKG-INFO` & `agentx-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AgentX
-Version: 0.0.7
+Version: 0.0.8
 Summary: AgentX: Seamlessly integrate intelligent agents into your projects. Empower your applications with advanced AI capabilities.
 Author-email: Erfan Zare Chavoshi <erfanzare810@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/erfanzar/AgentX
 Project-URL: Issues, https://github.com/erfanzar/AgentX/issues
 Project-URL: Documentation, https://erfanzar.github.io/AgentX
 Classifier: Programming Language :: Python :: 3
```

### Comparing `AgentX-0.0.7/README.md` & `agentx-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `AgentX-0.0.7/pyproject.toml` & `agentx-0.0.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "AgentX"
-version = "0.0.7"
+version = "0.0.8"
 
 dependencies = [
     "typing~=3.7.4.3",
     "ipython~=8.17.2",
     "tqdm~=4.64.1",
     "pydantic==2.5.3",
     "setuptools~=68.1.2",
@@ -69,9 +69,13 @@
 Documentation = "https://erfanzar.github.io/AgentX"
 
 [build-system]
 
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
-[tool.setuptools.packages]
-find = { where = ["src/"], include = ["**/*.jinja2"] }
+[tool.setuptools.packages.find]
+where = ["src/", ]
+include = ["**/*.jinja2", "agentx", "*"]
+
+[tool.setuptools.package-data]
+"*" = ["*.jinja2"]
```

### Comparing `AgentX-0.0.7/src/AgentX.egg-info/PKG-INFO` & `agentx-0.0.8/src/AgentX.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AgentX
-Version: 0.0.7
+Version: 0.0.8
 Summary: AgentX: Seamlessly integrate intelligent agents into your projects. Empower your applications with advanced AI capabilities.
 Author-email: Erfan Zare Chavoshi <erfanzare810@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/erfanzar/AgentX
 Project-URL: Issues, https://github.com/erfanzar/AgentX/issues
 Project-URL: Documentation, https://erfanzar.github.io/AgentX
 Classifier: Programming Language :: Python :: 3
```

