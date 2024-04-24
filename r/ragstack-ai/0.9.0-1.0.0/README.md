# Comparing `tmp/ragstack_ai-0.9.0.tar.gz` & `tmp/ragstack_ai-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragstack_ai-0.9.0.tar", max compression
+gzip compressed data, was "ragstack_ai-1.0.0.tar", max compression
```

## Comparing `ragstack_ai-0.9.0.tar` & `ragstack_ai-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3781 2024-03-13 10:20:09.714284 ragstack_ai-0.9.0/LICENSE.md
--rw-r--r--   0        0        0     2395 2024-03-13 10:20:09.714284 ragstack_ai-0.9.0/PACKAGE_README.md
--rw-r--r--   0        0        0     1203 2024-03-13 10:20:09.726284 ragstack_ai-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      271 2024-03-13 10:20:09.730284 ragstack_ai-0.9.0/ragstack/__init__.py
--rw-r--r--   0        0        0     3693 1970-01-01 00:00:00.000000 ragstack_ai-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     3781 2024-04-24 15:31:59.581683 ragstack_ai-1.0.0/LICENSE.md
+-rw-r--r--   0        0        0     2395 2024-04-24 15:31:59.581683 ragstack_ai-1.0.0/PACKAGE_README.md
+-rw-r--r--   0        0        0     1790 2024-04-24 15:31:59.613683 ragstack_ai-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      271 2024-04-24 15:31:59.613683 ragstack_ai-1.0.0/ragstack/__init__.py
+-rw-r--r--   0        0        0     3207 1970-01-01 00:00:00.000000 ragstack_ai-1.0.0/PKG-INFO
```

### Comparing `ragstack_ai-0.9.0/LICENSE.md` & `ragstack_ai-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ragstack_ai-0.9.0/PACKAGE_README.md` & `ragstack_ai-1.0.0/PACKAGE_README.md`

 * *Files identical despite different names*

### Comparing `ragstack_ai-0.9.0/PKG-INFO` & `ragstack_ai-1.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,23 @@
 Metadata-Version: 2.1
 Name: ragstack-ai
-Version: 0.9.0
+Version: 1.0.0
 Summary: DataStax RAGStack
 Home-page: https://github.com/datastax/ragstack-ai
 License: BUSL-1.1
 Author: DataStax
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: langchain-google
-Provides-Extra: langchain-nvidia
-Requires-Dist: astrapy (>=0.7.0,<0.8.0)
-Requires-Dist: cassio (>=0.1.3,<0.2.0)
-Requires-Dist: langchain (==0.1.12)
-Requires-Dist: langchain-community (==0.0.28)
-Requires-Dist: langchain-core (==0.1.31)
-Requires-Dist: langchain-google-genai (==0.0.9) ; extra == "langchain-google"
-Requires-Dist: langchain-google-vertexai (==0.1.0) ; extra == "langchain-google"
-Requires-Dist: langchain-nvidia-ai-endpoints (==0.0.3) ; extra == "langchain-nvidia"
-Requires-Dist: langchain-openai (==0.0.8)
-Requires-Dist: llama-index[langchain] (==0.9.48)
-Requires-Dist: llama-parse (==0.1.4)
-Requires-Dist: unstructured (==0.12.5)
+Requires-Dist: ragstack-ai-colbert (==1.0.0)
+Requires-Dist: ragstack-ai-langchain[colbert,google,nvidia] (==1.0.0)
+Requires-Dist: ragstack-ai-llamaindex[azure,bedrock,colbert,google] (==1.0.0)
 Project-URL: Documentation, https://docs.datastax.com/en/ragstack
 Project-URL: Repository, https://github.com/datastax/ragstack-ai
 Description-Content-Type: text/markdown
 
 # RAGStack
 [![Release Notes](https://img.shields.io/github/v/release/datastax/ragstack-ai.svg)](https://github.com/datastax/ragstack-ai/releases)
 [![Downloads](https://static.pepy.tech/badge/ragstack-ai/month)](https://www.pepy.tech/projects/ragstack-ai)
```

