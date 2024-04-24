# Comparing `tmp/detoxio_dtx-0.1.3.tar.gz` & `tmp/detoxio_dtx-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detoxio_dtx-0.1.3.tar", max compression
+gzip compressed data, was "detoxio_dtx-0.1.4.tar", max compression
```

## Comparing `detoxio_dtx-0.1.3.tar` & `detoxio_dtx-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      695 2024-04-15 15:20:34.979930 detoxio_dtx-0.1.3/README.md
--rw-r--r--   0        0        0      948 2024-04-15 15:20:34.979930 detoxio_dtx-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        1 2024-04-15 15:20:34.979930 detoxio_dtx-0.1.3/src/dtx/__init__.py
--rw-r--r--   0        0        0     5631 2024-04-15 15:20:34.979930 detoxio_dtx-0.1.3/src/dtx/cli/__init__.py
--rw-r--r--   0        0        0     1580 2024-04-15 15:20:34.979930 detoxio_dtx-0.1.3/src/dtx/cli/console.py
--rw-r--r--   0        0        0     3180 2024-04-15 15:20:34.979930 detoxio_dtx-0.1.3/src/dtx/cli/inferencing.py
--rw-r--r--   0        0        0      714 2024-04-15 15:20:34.979930 detoxio_dtx-0.1.3/src/dtx/cli/utils.py
--rw-r--r--   0        0        0     1718 1970-01-01 00:00:00.000000 detoxio_dtx-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      695 2024-04-24 17:25:38.995736 detoxio_dtx-0.1.4/README.md
+-rw-r--r--   0        0        0      948 2024-04-24 17:25:38.995736 detoxio_dtx-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-04-24 17:25:38.995736 detoxio_dtx-0.1.4/src/dtx/__init__.py
+-rw-r--r--   0        0        0     6508 2024-04-24 17:25:38.995736 detoxio_dtx-0.1.4/src/dtx/cli/__init__.py
+-rw-r--r--   0        0        0     1580 2024-04-24 17:25:38.995736 detoxio_dtx-0.1.4/src/dtx/cli/console.py
+-rw-r--r--   0        0        0     3180 2024-04-24 17:25:38.995736 detoxio_dtx-0.1.4/src/dtx/cli/inferencing.py
+-rw-r--r--   0        0        0      714 2024-04-24 17:25:38.995736 detoxio_dtx-0.1.4/src/dtx/cli/utils.py
+-rw-r--r--   0        0        0     1718 1970-01-01 00:00:00.000000 detoxio_dtx-0.1.4/PKG-INFO
```

### Comparing `detoxio_dtx-0.1.3/README.md` & `detoxio_dtx-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `detoxio_dtx-0.1.3/pyproject.toml` & `detoxio_dtx-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "detoxio-dtx"
-version = "0.1.3"
+version = "0.1.4"
 description = "detoxio.ai - API first LLM security testing and red team automation"
 authors = ["detoxio.ai <hello@detoxio.ai>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://detoxio.ai"
 documentation = "https://docs.detoxio.ai"
 classifiers = [
```

### Comparing `detoxio_dtx-0.1.3/src/dtx/cli/__init__.py` & `detoxio_dtx-0.1.4/src/dtx/cli/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import traceback
 import click
 import tqdm
 import detoxio.config as config
 import detoxio.adapters.exceptions as exceptions
+import proto.dtx.services.prompts.v1.prompts_pb2 as prompts_pb2
+import proto.dtx.messages.common.threat_pb2 as threat_pb2
 
 from detoxio.scanner import LLMScanner, LLMPrompt, LLMResponse
 from detoxio.reporting import JSONLinesLLMScanReport, MarkdownLLMScanReport
 from detoxio.adapters.grpc import get_secure_channel_with_token
 from detoxio.adapters.prompts import get_prompts_service
 
 from dtx.cli.utils import print_info, print_error, print_success, print_verbose, is_verbose
@@ -41,28 +43,40 @@
 
     # Exception handling is at main()
     prompt_service.ping()
     print_success("Server is reachable and authenticated")
 
 @click.command("prompts", help="Retrieve prompts from the Detoxio API")
 @click.option("--count", type=int, help="The number of prompts to retrieve", default=1)
-def prompts(count):
+@click.option("--class", type=str, help="The threat class of prompts to retrieve")
+@click.option("--category", type=str, help="The threat category of prompts to retrieve")
+@click.option("--label", type=str, help="Additional labels to filter prompts (example: k1=v1,k2=v2)")
+def prompts(count, **kwargs):
     """
     Retrieve prompts from the Detoxio API.
     """
 
     key = config.load_key_from_env()
     channel = get_secure_channel_with_token(config.get_api_host(), config.get_api_port(), key)
     prompt_service = get_prompts_service(channel)
+    filter = prompts_pb2.PromptGenerationFilterOption()
+
+    klass, category, label = kwargs.get("class"), kwargs.get("category"), kwargs.get("label")
+    if klass:
+        filter.threat_class = threat_pb2.ThreatClass.Value(klass)
+    if category:
+        filter.threat_category = threat_pb2.ThreatCategory.Value(category)
+    if label:
+        map(lambda x: filter.labels.update({x[0]: x[1]}) , [kv.strip().split("=") for kv in label.strip().split(",")])
 
     print_info(f"Retrieving {count} prompt(s) from the API")
 
     # Our API currently support a single prompt retrieval
     for i in range(count):
-        prompt = prompt_service.generate_prompt(count=1)
+        prompt = prompt_service.generate_prompt(count=1, filter=filter)
         print_info(f"Prompt {i + 1}: {prompt.prompts[0].data.content}")
 
 @click.command("scan", help="Scan a model from Hugging Face for security vulnerablities")
 @click.option("--model", type=str, required=True, help="The model to scan")
 @click.option("--count", type=int, help="The number prompts to generate for scanning", default=10)
 @click.option("--jsonl", type=str, help="Output the results in JSONL format")
 @click.option("--markdown", type=str, help="Output the results in Markdown format")
```

### Comparing `detoxio_dtx-0.1.3/src/dtx/cli/console.py` & `detoxio_dtx-0.1.4/src/dtx/cli/console.py`

 * *Files identical despite different names*

### Comparing `detoxio_dtx-0.1.3/src/dtx/cli/inferencing.py` & `detoxio_dtx-0.1.4/src/dtx/cli/inferencing.py`

 * *Files identical despite different names*

### Comparing `detoxio_dtx-0.1.3/src/dtx/cli/utils.py` & `detoxio_dtx-0.1.4/src/dtx/cli/utils.py`

 * *Files identical despite different names*

### Comparing `detoxio_dtx-0.1.3/PKG-INFO` & `detoxio_dtx-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detoxio-dtx
-Version: 0.1.3
+Version: 0.1.4
 Summary: detoxio.ai - API first LLM security testing and red team automation
 Home-page: https://detoxio.ai
 License: Apache-2.0
 Author: detoxio.ai
 Author-email: hello@detoxio.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

