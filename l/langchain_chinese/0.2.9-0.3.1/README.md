# Comparing `tmp/langchain_chinese-0.2.9.tar.gz` & `tmp/langchain_chinese-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_chinese-0.2.9.tar", max compression
+gzip compressed data, was "langchain_chinese-0.3.1.tar", max compression
```

## Comparing `langchain_chinese-0.2.9.tar` & `langchain_chinese-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,28 @@
--rw-r--r--   0        0        0     1066 2024-02-17 14:31:41.028210 langchain_chinese-0.2.9/LICENSE
--rw-r--r--   0        0        0     4179 2024-02-20 01:18:34.709188 langchain_chinese-0.2.9/README.md
--rw-r--r--   0        0        0        0 2024-02-18 04:12:40.965581 langchain_chinese-0.2.9/langchain_chinese/.pypirc
--rw-r--r--   0        0        0      182 2024-02-20 03:38:21.810352 langchain_chinese-0.2.9/langchain_chinese/__init__.py
--rw-r--r--   0        0        0       22 2024-02-20 03:38:23.932102 langchain_chinese-0.2.9/langchain_chinese/__version__.py
--rw-r--r--   0        0        0        0 2024-02-17 14:33:28.652032 langchain_chinese-0.2.9/langchain_chinese/zhipuai/__init__.py
--rw-r--r--   0        0        0    11561 2024-02-20 02:28:01.765100 langchain_chinese-0.2.9/langchain_chinese/zhipuai/base.py
--rw-r--r--   0        0        0      752 2024-02-20 03:38:41.017892 langchain_chinese-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     4917 1970-01-01 00:00:00.000000 langchain_chinese-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-02-17 14:31:41.028210 langchain_chinese-0.3.1/LICENSE
+-rw-r--r--   0        0        0     7068 2024-03-22 15:20:04.993433 langchain_chinese-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-02-18 04:12:40.965581 langchain_chinese-0.3.1/langchain_chinese/.pypirc
+-rw-r--r--   0        0        0      743 2024-04-17 11:05:39.194120 langchain_chinese-0.3.1/langchain_chinese/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-16 10:55:29.186984 langchain_chinese-0.3.1/langchain_chinese/__version__.py
+-rw-r--r--   0        0        0        0 2024-03-07 05:02:32.649684 langchain_chinese-0.3.1/langchain_chinese/agents/__init__.py
+-rw-r--r--   0        0        0     2722 2024-03-11 11:16:28.698924 langchain_chinese-0.3.1/langchain_chinese/agents/base.py
+-rw-r--r--   0        0        0     7036 2024-04-16 06:56:48.688214 langchain_chinese-0.3.1/langchain_chinese/agents/prompt.py
+-rw-r--r--   0        0        0        0 2024-04-16 09:32:02.865599 langchain_chinese-0.3.1/langchain_chinese/agents/writing/__init__.py
+-rw-r--r--   0        0        0     6780 2024-04-22 14:17:36.209883 langchain_chinese-0.3.1/langchain_chinese/agents/writing/base.py
+-rw-r--r--   0        0        0      936 2024-04-22 08:23:19.731915 langchain_chinese-0.3.1/langchain_chinese/agents/writing/prompts/main.py
+-rw-r--r--   0        0        0      385 2024-04-16 13:01:35.131996 langchain_chinese-0.3.1/langchain_chinese/agents/writing/prompts/translate.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:59:35.052113 langchain_chinese-0.3.1/langchain_chinese/agents/writing/reading/__init__.py
+-rw-r--r--   0        0        0      112 2024-04-16 02:11:52.139352 langchain_chinese-0.3.1/langchain_chinese/agents/writing/reading/base.py
+-rw-r--r--   0        0        0        0 2024-03-03 11:14:01.447370 langchain_chinese-0.3.1/langchain_chinese/document_loaders/__init__.py
+-rw-r--r--   0        0        0     4252 2024-03-03 11:12:06.414308 langchain_chinese-0.3.1/langchain_chinese/document_loaders/base.py
+-rw-r--r--   0        0        0       57 2024-03-17 15:26:04.636361 langchain_chinese-0.3.1/langchain_chinese/langgraph/__init__.py
+-rw-r--r--   0        0        0     5269 2024-03-22 10:25:10.156397 langchain_chinese-0.3.1/langchain_chinese/langgraph/tools_calling.py
+-rw-r--r--   0        0        0       77 2024-03-04 03:23:29.330261 langchain_chinese-0.3.1/langchain_chinese/memory/__init__.py
+-rw-r--r--   0        0        0    10710 2024-03-04 03:27:24.792898 langchain_chinese-0.3.1/langchain_chinese/memory/base.py
+-rw-r--r--   0        0        0     3612 2024-03-06 08:58:53.719955 langchain_chinese-0.3.1/langchain_chinese/memory/memory_manager.py
+-rw-r--r--   0        0        0        0 2024-03-03 02:13:31.722951 langchain_chinese-0.3.1/langchain_chinese/retrievers/__init__.py
+-rw-r--r--   0        0        0     3004 2024-04-16 07:36:51.110370 langchain_chinese-0.3.1/langchain_chinese/retrievers/base.py
+-rw-r--r--   0        0        0      413 2024-04-18 00:26:11.920514 langchain_chinese-0.3.1/langchain_chinese/templates/agents/writing/expand/scripts.ipynb
+-rw-r--r--   0        0        0      471 2024-04-18 00:25:43.311107 langchain_chinese-0.3.1/langchain_chinese/templates/agents/writing/project/README.md
+-rw-r--r--   0        0        0      413 2024-04-17 09:58:36.350187 langchain_chinese-0.3.1/langchain_chinese/templates/agents/writing/project/scripts.ipynb
+-rw-r--r--   0        0        0      842 2024-04-17 09:55:08.431338 langchain_chinese-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7970 1970-01-01 00:00:00.000000 langchain_chinese-0.3.1/PKG-INFO
```

### Comparing `langchain_chinese-0.2.9/LICENSE` & `langchain_chinese-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_chinese-0.2.9/pyproject.toml` & `langchain_chinese-0.3.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 [tool.poetry]
 name = "langchain_chinese"
-version = "0.2.9"
+version = "0.3.1"
 description = "Prepare some firendly tool for Chinese LLMs and langchain"
 authors = ["arcstep <43801@qq.com>"]
 homepage = "https://github.com/arcstep/langchain_chinese"
 repository = "https://github.com/arcstep/langchain_chinese.git"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-zhipuai_pydantic_v1 = "^2.0.1"
+asyncio = "^3.4.3"
+pydantic = ">=1,<3"
+langchain = "^0.1.10"
+langchain-community = "^0.0.25"
+python-dotenv = "^1.0.1"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 setuptools = "^69.1.0"
 poetry2setup = "^1.1.0"
 python-dotenv = "^1.0.1"
-langchain = "^0.1.7"
 ipykernel = "^6.29.2"
-
-[tool.poetry.group.dev.dependencies]
 pytest = "^8.0.1"
+pydantic = "1.10.13"
+docx2txt = "^0.8"
+pypdf = "^4.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.packages]]
 include = "langchain_chinese/**/*"
```

