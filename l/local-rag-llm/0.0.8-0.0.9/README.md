# Comparing `tmp/local_rag_llm-0.0.8.tar.gz` & `tmp/local_rag_llm-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local_rag_llm-0.0.8.tar", last modified: Fri Mar 15 12:00:31 2024, max compression
+gzip compressed data, was "local_rag_llm-0.0.9.tar", last modified: Mon Mar 18 14:43:46 2024, max compression
```

## Comparing `local_rag_llm-0.0.8.tar` & `local_rag_llm-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 danielhopp   (501) staff       (20)        0 2024-03-15 12:00:31.523863 local_rag_llm-0.0.8/
--rw-r--r--   0 danielhopp   (501) staff       (20)     1068 2024-03-05 14:55:47.000000 local_rag_llm-0.0.8/LICENSE
--rw-r--r--   0 danielhopp   (501) staff       (20)     4968 2024-03-15 12:00:31.523685 local_rag_llm-0.0.8/PKG-INFO
--rw-r--r--   0 danielhopp   (501) staff       (20)     4530 2024-03-15 11:45:46.000000 local_rag_llm-0.0.8/README.md
-drwxr-xr-x   0 danielhopp   (501) staff       (20)        0 2024-03-15 12:00:31.522786 local_rag_llm-0.0.8/local_rag_llm/
--rw-r--r--   0 danielhopp   (501) staff       (20)        0 2024-03-06 16:30:17.000000 local_rag_llm-0.0.8/local_rag_llm/__init__.py
--rw-r--r--   0 danielhopp   (501) staff       (20)     8398 2024-03-15 11:59:29.000000 local_rag_llm-0.0.8/local_rag_llm/db_setup.py
--rw-r--r--   0 danielhopp   (501) staff       (20)     8292 2024-03-15 11:59:29.000000 local_rag_llm-0.0.8/local_rag_llm/local_llm.py
--rw-r--r--   0 danielhopp   (501) staff       (20)     5869 2024-03-15 11:45:46.000000 local_rag_llm-0.0.8/local_rag_llm/model_setup.py
-drwxr-xr-x   0 danielhopp   (501) staff       (20)        0 2024-03-15 12:00:31.523510 local_rag_llm-0.0.8/local_rag_llm.egg-info/
--rw-r--r--   0 danielhopp   (501) staff       (20)     4968 2024-03-15 12:00:31.000000 local_rag_llm-0.0.8/local_rag_llm.egg-info/PKG-INFO
--rw-r--r--   0 danielhopp   (501) staff       (20)      282 2024-03-15 12:00:31.000000 local_rag_llm-0.0.8/local_rag_llm.egg-info/SOURCES.txt
--rw-r--r--   0 danielhopp   (501) staff       (20)        1 2024-03-15 12:00:31.000000 local_rag_llm-0.0.8/local_rag_llm.egg-info/dependency_links.txt
--rw-r--r--   0 danielhopp   (501) staff       (20)       14 2024-03-15 12:00:31.000000 local_rag_llm-0.0.8/local_rag_llm.egg-info/top_level.txt
--rw-r--r--   0 danielhopp   (501) staff       (20)       38 2024-03-15 12:00:31.523897 local_rag_llm-0.0.8/setup.cfg
--rw-r--r--   0 danielhopp   (501) staff       (20)      654 2024-03-15 11:59:29.000000 local_rag_llm-0.0.8/setup.py
+drwxr-xr-x   0 danielhopp   (501) staff       (20)        0 2024-03-18 14:43:46.570636 local_rag_llm-0.0.9/
+-rw-r--r--   0 danielhopp   (501) staff       (20)     1068 2024-03-05 14:55:47.000000 local_rag_llm-0.0.9/LICENSE
+-rw-r--r--   0 danielhopp   (501) staff       (20)     4968 2024-03-18 14:43:46.570458 local_rag_llm-0.0.9/PKG-INFO
+-rw-r--r--   0 danielhopp   (501) staff       (20)     4530 2024-03-15 11:45:46.000000 local_rag_llm-0.0.9/README.md
+drwxr-xr-x   0 danielhopp   (501) staff       (20)        0 2024-03-18 14:43:46.569695 local_rag_llm-0.0.9/local_rag_llm/
+-rw-r--r--   0 danielhopp   (501) staff       (20)        0 2024-03-06 16:30:17.000000 local_rag_llm-0.0.9/local_rag_llm/__init__.py
+-rw-r--r--   0 danielhopp   (501) staff       (20)     8398 2024-03-15 11:59:29.000000 local_rag_llm-0.0.9/local_rag_llm/db_setup.py
+-rw-r--r--   0 danielhopp   (501) staff       (20)     8465 2024-03-18 14:42:57.000000 local_rag_llm-0.0.9/local_rag_llm/local_llm.py
+-rw-r--r--   0 danielhopp   (501) staff       (20)     5869 2024-03-15 11:45:46.000000 local_rag_llm-0.0.9/local_rag_llm/model_setup.py
+drwxr-xr-x   0 danielhopp   (501) staff       (20)        0 2024-03-18 14:43:46.570256 local_rag_llm-0.0.9/local_rag_llm.egg-info/
+-rw-r--r--   0 danielhopp   (501) staff       (20)     4968 2024-03-18 14:43:46.000000 local_rag_llm-0.0.9/local_rag_llm.egg-info/PKG-INFO
+-rw-r--r--   0 danielhopp   (501) staff       (20)      282 2024-03-18 14:43:46.000000 local_rag_llm-0.0.9/local_rag_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 danielhopp   (501) staff       (20)        1 2024-03-18 14:43:46.000000 local_rag_llm-0.0.9/local_rag_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 danielhopp   (501) staff       (20)       14 2024-03-18 14:43:46.000000 local_rag_llm-0.0.9/local_rag_llm.egg-info/top_level.txt
+-rw-r--r--   0 danielhopp   (501) staff       (20)       38 2024-03-18 14:43:46.570672 local_rag_llm-0.0.9/setup.cfg
+-rw-r--r--   0 danielhopp   (501) staff       (20)      654 2024-03-18 14:42:57.000000 local_rag_llm-0.0.9/setup.py
```

### Comparing `local_rag_llm-0.0.8/LICENSE` & `local_rag_llm-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `local_rag_llm-0.0.8/PKG-INFO` & `local_rag_llm-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: local_rag_llm
-Version: 0.0.8
+Version: 0.0.9
 Summary: Create and run a local LLM with RAG
 Home-page: https://github.com/dhopp1/local_rag_llm
 Author: Daniel Hopp
 Author-email: daniel.hopp@un.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `local_rag_llm-0.0.8/README.md` & `local_rag_llm-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `local_rag_llm-0.0.8/local_rag_llm/db_setup.py` & `local_rag_llm-0.0.9/local_rag_llm/db_setup.py`

 * *Files identical despite different names*

### Comparing `local_rag_llm-0.0.8/local_rag_llm/local_llm.py` & `local_rag_llm-0.0.9/local_rag_llm/local_llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from importlib import import_module
-from torch import cuda
+import torch
 import os
 import pandas as pd
 
 
 class local_llm:
     """Primary class of the library, use and manage the LLM, your RAG documents, and their metadata
     parameters:
@@ -64,15 +64,21 @@
             os.environ["HF_TOKEN"] = hf_token
         self.temperature = temperature
         self.max_new_tokens = max_new_tokens
         self.context_window = context_window
         self.memory_limit = memory_limit
         self.system_prompt = system_prompt
 
-        self.device = f"cuda:{cuda.current_device()}" if cuda.is_available() else "cpu"
+        if torch.cuda.is_available():
+            self.device = f"cuda:{torch.cuda.current_device()}"
+        elif torch.backends.mps.is_available() and torch.backends.mps.is_built():
+            self.device = "mps"
+        else:
+            self.device = "cpu"
+        
         self.n_gpu_layers = n_gpu_layers
         self.chat_engine = None
 
         self.llm = self.model_setup.instantiate_model(
             text_path=self.text_path,
             llm_url=self.llm_url,
             llm_path=self.llm_path,
```

### Comparing `local_rag_llm-0.0.8/local_rag_llm/model_setup.py` & `local_rag_llm-0.0.9/local_rag_llm/model_setup.py`

 * *Files identical despite different names*

### Comparing `local_rag_llm-0.0.8/local_rag_llm.egg-info/PKG-INFO` & `local_rag_llm-0.0.9/local_rag_llm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: local_rag_llm
-Version: 0.0.8
+Name: local-rag-llm
+Version: 0.0.9
 Summary: Create and run a local LLM with RAG
 Home-page: https://github.com/dhopp1/local_rag_llm
 Author: Daniel Hopp
 Author-email: daniel.hopp@un.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `local_rag_llm-0.0.8/setup.py` & `local_rag_llm-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="local_rag_llm",
-    version="0.0.8",
+    version="0.0.9",
     author="Daniel Hopp",
     author_email="daniel.hopp@un.org",
     description="Create and run a local LLM with RAG",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dhopp1/local_rag_llm",
     packages=setuptools.find_packages(),
```

