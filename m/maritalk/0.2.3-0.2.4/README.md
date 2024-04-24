# Comparing `tmp/maritalk-0.2.3.tar.gz` & `tmp/maritalk-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maritalk-0.2.3.tar", last modified: Fri Apr 12 17:58:36 2024, max compression
+gzip compressed data, was "maritalk-0.2.4.tar", last modified: Wed Apr 24 12:03:58 2024, max compression
```

## Comparing `maritalk-0.2.3.tar` & `maritalk-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:58:36.836048 maritalk-0.2.3/
--rw-rw-r--   0 root         (0) root         (0)     1088 2023-09-04 19:10:06.000000 maritalk-0.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)    10180 2024-04-12 17:58:36.836048 maritalk-0.2.3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8339 2024-04-12 17:58:00.000000 maritalk-0.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:58:36.832048 maritalk-0.2.3/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:58:36.832048 maritalk-0.2.3/examples/local/
--rw-rw-r--   0 root         (0) root         (0)      996 2024-04-12 17:58:00.000000 maritalk-0.2.3/examples/local/question_answering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:58:36.836048 maritalk-0.2.3/maritalk/
--rw-rw-r--   0 root         (0) root         (0)      156 2023-12-03 16:28:52.000000 maritalk-0.2.3/maritalk/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1238 2024-04-12 17:58:00.000000 maritalk-0.2.3/maritalk/download.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:58:36.836048 maritalk-0.2.3/maritalk/resources/
--rw-rw-r--   0 root         (0) root         (0)     8917 2024-04-12 17:58:00.000000 maritalk-0.2.3/maritalk/resources/api.py
--rw-rw-r--   0 root         (0) root         (0)    11855 2024-04-12 17:58:02.000000 maritalk-0.2.3/maritalk/resources/local.py
--rw-rw-r--   0 root         (0) root         (0)     1042 2024-04-12 17:58:00.000000 maritalk-0.2.3/maritalk/start.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:58:36.836048 maritalk-0.2.3/maritalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10180 2024-04-12 17:58:36.000000 maritalk-0.2.3/maritalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      351 2024-04-12 17:58:36.000000 maritalk-0.2.3/maritalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 17:58:36.000000 maritalk-0.2.3/maritalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-04-12 17:58:36.000000 maritalk-0.2.3/maritalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-12 17:58:36.000000 maritalk-0.2.3/maritalk.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      721 2024-04-12 17:58:30.000000 maritalk-0.2.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 17:58:36.836048 maritalk-0.2.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)       37 2023-09-04 19:10:06.000000 maritalk-0.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:03:58.052019 maritalk-0.2.4/
+-rw-rw-r--   0 root         (0) root         (0)     1088 2023-09-04 19:10:06.000000 maritalk-0.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    10180 2024-04-24 12:03:58.052019 maritalk-0.2.4/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8339 2024-04-23 13:50:33.000000 maritalk-0.2.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:03:58.048020 maritalk-0.2.4/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:03:58.052019 maritalk-0.2.4/examples/local/
+-rw-rw-r--   0 root         (0) root         (0)     5374 2024-04-17 16:21:14.000000 maritalk-0.2.4/examples/local/benchmark.py
+-rw-rw-r--   0 root         (0) root         (0)      991 2024-04-17 16:21:14.000000 maritalk-0.2.4/examples/local/question_answering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:03:58.052019 maritalk-0.2.4/maritalk/
+-rw-rw-r--   0 root         (0) root         (0)      156 2023-12-03 16:28:52.000000 maritalk-0.2.4/maritalk/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1258 2024-04-24 12:00:57.000000 maritalk-0.2.4/maritalk/download.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:03:58.052019 maritalk-0.2.4/maritalk/resources/
+-rw-rw-r--   0 root         (0) root         (0)     8917 2024-04-17 16:21:11.000000 maritalk-0.2.4/maritalk/resources/api.py
+-rw-rw-r--   0 root         (0) root         (0)    14686 2024-04-24 12:00:57.000000 maritalk-0.2.4/maritalk/resources/local.py
+-rw-rw-r--   0 root         (0) root         (0)     1050 2024-04-24 12:00:57.000000 maritalk-0.2.4/maritalk/start.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:03:58.052019 maritalk-0.2.4/maritalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10180 2024-04-24 12:03:58.000000 maritalk-0.2.4/maritalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      379 2024-04-24 12:03:58.000000 maritalk-0.2.4/maritalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 12:03:58.000000 maritalk-0.2.4/maritalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-24 12:03:58.000000 maritalk-0.2.4/maritalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-24 12:03:58.000000 maritalk-0.2.4/maritalk.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      721 2024-04-24 12:01:03.000000 maritalk-0.2.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 12:03:58.052019 maritalk-0.2.4/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)       37 2023-09-04 19:10:06.000000 maritalk-0.2.4/setup.py
```

### Comparing `maritalk-0.2.3/LICENSE` & `maritalk-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `maritalk-0.2.3/PKG-INFO` & `maritalk-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maritalk
-Version: 0.2.3
+Version: 0.2.4
 Summary: Client library for the MariTalk API
 Author-email: Maritaca AI <info@maritaca.ai>
 License: The MIT License
         
         Copyright (c) Maritaca AI (https://maritaca.ai)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -45,15 +45,15 @@
 - [Exemplo de uso](#exemplo-de-uso)
 - [Exemplo de uso via requisições HTTP - Python](https://github.com/maritaca-ai/maritalk-api/blob/main/examples/api/maritalk_via_requisições_https.ipynb)
 - [Exemplo de uso via requisições HTTP - JavaScript](https://github.com/maritaca-ai/maritalk-api/blob/main/examples/api/maritalk_via_requisições_https.js)
 - [Exemplo MariTalk + RAG com LangChain](https://python.langchain.com/docs/integrations/chat/maritalk)
 - [Exemplo Maritalk no LlamaIndex](https://docs.llamaindex.ai/en/latest/examples/llm/maritalk)
 - [Documentação Swagger](https://chat.maritaca.ai/docs)
 
-[MariTalk local](https://github.com/maritaca-ai/maritalk-api/blob/main/README-Local.md)
+[MariTalk Local](https://github.com/maritaca-ai/maritalk-api/blob/main/README-Local.md)
 
 [Chat (gratuito)](#web-chat)
 
 # Introdução
 Este repositório contém o código e a documentação explicando como usar a API da MariTalk e a versão local para deploy on-premises.
 A MariTalk é uma assistente baseada em um modelo de linguagem que foi especialmente treinado para entender bem o português.
 Ela é capaz de seguir instruções de maneira zero-shot, assim como o ChatGPT.
```

### Comparing `maritalk-0.2.3/README.md` & `maritalk-0.2.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 - [Exemplo de uso](#exemplo-de-uso)
 - [Exemplo de uso via requisições HTTP - Python](https://github.com/maritaca-ai/maritalk-api/blob/main/examples/api/maritalk_via_requisições_https.ipynb)
 - [Exemplo de uso via requisições HTTP - JavaScript](https://github.com/maritaca-ai/maritalk-api/blob/main/examples/api/maritalk_via_requisições_https.js)
 - [Exemplo MariTalk + RAG com LangChain](https://python.langchain.com/docs/integrations/chat/maritalk)
 - [Exemplo Maritalk no LlamaIndex](https://docs.llamaindex.ai/en/latest/examples/llm/maritalk)
 - [Documentação Swagger](https://chat.maritaca.ai/docs)
 
-[MariTalk local](https://github.com/maritaca-ai/maritalk-api/blob/main/README-Local.md)
+[MariTalk Local](https://github.com/maritaca-ai/maritalk-api/blob/main/README-Local.md)
 
 [Chat (gratuito)](#web-chat)
 
 # Introdução
 Este repositório contém o código e a documentação explicando como usar a API da MariTalk e a versão local para deploy on-premises.
 A MariTalk é uma assistente baseada em um modelo de linguagem que foi especialmente treinado para entender bem o português.
 Ela é capaz de seguir instruções de maneira zero-shot, assim como o ChatGPT.
```

### Comparing `maritalk-0.2.3/examples/local/question_answering.py` & `maritalk-0.2.4/examples/local/question_answering.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import maritalk
 
 client = maritalk.MariTalkLocal()
 client.start_server(license=os.environ["MARITALK_LICENSE"])
 
 # Question selected from the FaQuAD dataset:
 # https://huggingface.co/datasets/eraldoluis/faquad?row=32
-result = client.generate_chat([
+result = client.generate([
     {
         "role": "user",
         "content": """Com base no texto abaixo, resposta a pergunta "Qual o objetivo do POSCOMP?"
 Contexto: O Exame Nacional para Ingresso na Pós-Graduação em Computação (POSCOMP) é um exame aplicado em todas as regiões do País. Em parceria com a Sociedade Peruana de Computação, desde 2006 o Exame passou a ser realizado no Peru. O POSCOMP testa conhecimentos na área de Computação e tem como objetivo específico avaliar os conhecimentos de candidatos a Programas de Pós-Graduação em Computação oferecidos no Brasil. A grande maioria dos Programas de Pós-Graduação no País utiliza, de alguma forma, o resultado do POSCOMP em seu processo seletivo."""
     }
 ])
 print(result["output"])
```

### Comparing `maritalk-0.2.3/maritalk/download.py` & `maritalk-0.2.4/maritalk/download.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,11 +32,11 @@
     dependencies = {"cuda_version": args.cuda or detected_versions["cuda_version"]}
 
     if dependencies["cuda_version"] is None:
         raise Exception(
             "No libcublas.so found. cuBLAS v11 or v12 is required to run MariTalk. You can manually set the version using the `cuda_version` argument."
         )
 
-    bin_folder = os.path.dirname(args.path)
+    bin_folder = os.path.dirname(os.path.expanduser(args.path))
     if bin_folder:
         os.makedirs(bin_folder, exist_ok=True)
     download(args.license, args.path, dependencies)
```

### Comparing `maritalk-0.2.3/maritalk/resources/api.py` & `maritalk-0.2.4/maritalk/resources/api.py`

 * *Files identical despite different names*

### Comparing `maritalk-0.2.3/maritalk/resources/local.py` & `maritalk-0.2.4/maritalk/resources/local.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import os
 import re
 import csv
+import sys
 import time
 import atexit
+import threading
 import subprocess
 from tqdm import tqdm
 from pathlib import Path
 from typing import List, Dict, Optional, Union, Optional
 import requests
 from requests.exceptions import ConnectionError
 
 
 def check_gpu():
     try:
         result = subprocess.run(
             [
-                'nvidia-smi',
-                '--query-gpu=name,compute_cap',
-                '--format=csv',
+                "nvidia-smi",
+                "--query-gpu=name,compute_cap",
+                "--format=csv",
             ],
             capture_output=True,
             text=True,
             check=True,
         )
-        reader = csv.reader(result.stdout.strip().split('\n'))
+        reader = csv.reader(result.stdout.strip().split("\n"))
         headers = next(reader)
         rows = list(reader)
 
         for row in rows:
             gpu_name, compute_cap = row
             if float(compute_cap) >= 8.0:
                 return True
@@ -46,43 +48,43 @@
 def find_libs():
     versions = {
         "cuda_version": None,
     }
 
     try:
         output = subprocess.run(
-            ['nvidia-smi'],
+            ["nvidia-smi"],
             stdout=subprocess.PIPE,
-        ).stdout.decode('utf-8')
+        ).stdout.decode("utf-8")
         cuda_version_match = re.search(r"CUDA Version: (\d+\.\d+)", output)
 
         if not cuda_version_match:
-            raise Exception("""Could not automatically detect the CUDA version. Verify the CUDA Toolkit installation or set the `cuda_version` parameter manually. For example:
+            raise Exception(
+                """Could not automatically detect the CUDA version. Verify the CUDA Toolkit installation or set the `cuda_version` parameter manually. For example:
 
 ```
 model.start_server("<YOUR LICENSE>", cuda_version="12.3")
 ```
 
-To install the CUDA Toolkit, please refer to: https://developer.nvidia.com/cuda-downloads""")
+To install the CUDA Toolkit, please refer to: https://developer.nvidia.com/cuda-downloads"""
+            )
 
         versions["cuda_version"] = cuda_version_match.group(1)
     except subprocess.CalledProcessError as e:
         raise Exception(f"Error executing command: {e}")
     except FileNotFoundError as e:
         raise Exception(
             "Nvidia-SMI is not installed. Please install the Nvidia driver and the CUDA toolkit."
         )
 
     return versions
 
 
 def download(license: str, bin_path: str, dependencies: Dict[str, int]):
-    download_url = (
-        "https://functions.maritaca.ai/local/download"
-    )
+    download_url = "https://functions.maritaca.ai/local/download"
     response = requests.post(
         download_url,
         json={
             "license": license,
             "cuda_version": dependencies["cuda_version"],
         },
     )
@@ -120,14 +122,46 @@
                 raise Exception(
                     f"Invalid response from the server while downloading: {response.text}"
                 )
     except requests.exceptions.RequestException as e:
         raise Exception(f"Error downloading MariTalk binary: {e}")
 
 
+def _get_total_mem():
+    try:
+        output = subprocess.check_output(["free", "-h"], text=True)
+        for line in output.splitlines():
+            if line.startswith("Mem:"):
+                mem_info = line.split()[1]
+                return _convert_to_gb(mem_info)
+        return None
+    except (subprocess.CalledProcessError, FileNotFoundError):
+        return None
+
+
+def _convert_to_gb(mem_str):
+    """
+    Convert memory string from `free -h` (like 251Gi) to gigabytes as a float.
+    """
+    match = re.match(r"([0-9.]+)([KMGTPE]i)", mem_str)
+    if match:
+        value, unit = match.groups()
+        unit_factor = {"Mi": 1 / 1024, "Gi": 1, "Ti": 1024}
+        return float(value) * unit_factor[unit]
+    return None
+
+
+def _get_file_size(file_path):
+    try:
+        file_size_bytes = os.path.getsize(file_path)
+        return file_size_bytes / (1024**3)
+    except Exception:
+        return None
+
+
 def start_server(
     license: str,
     bin_path: str = "~/bin/maritalk",
     cuda_version: Optional[int] = None,
     port: int = 9000,
 ):
     bin_path = os.path.expanduser(bin_path)
@@ -146,65 +180,122 @@
             )
 
         bin_folder = os.path.dirname(bin_path)
         if bin_folder:
             os.makedirs(bin_folder, exist_ok=True)
         download(license, bin_path, dependencies)
 
+    bin_size = _get_file_size(bin_path)
+
+    if bin_size:
+        min_memory = 30 if bin_size < 20 else 130
+        memory_available = _get_total_mem()
+        if memory_available and memory_available < min_memory:
+            print(
+                "WARNING: Verify that there is enough memory to load the model (at least 30 GB for the small version and 130 GB for the medium version)."
+            )
+
     args = [bin_path, "--license", license, "--port", str(port)]
     return subprocess.Popen(
         args,
         stdout=subprocess.PIPE,
-        stderr=subprocess.STDOUT,
+        stderr=subprocess.PIPE,
     )
 
 
 class MariTalkLocal:
     def __init__(self, host: str = "localhost", port: int = 9000):
         self.api_url = f"http://{host}:{port}"
         """@private"""
         self.port = port
         """@private"""
         self.process = None
         """@private"""
+        self.loading = False
+        """@private"""
+        self.loaded = False
+        """@private"""
 
     def start_server(
         self,
         license: str,
         bin_path: str = "~/bin/maritalk",
         cuda_version: Optional[int] = None,
+        verbose: str = True,
     ):
-        print(f"Starting MariTalk Local API at http://localhost:{self.port}")
+        if self.loaded:
+            return
+
+        self.loading = True
+        if verbose:
+            print(f"Starting MariTalk Local API at http://localhost:{self.port}/")
+            print(
+                "This process can take a few minutes (up to 10 minutes for the small version, depending on the hardware)."
+            )
+            loading_thread = threading.Thread(target=self._show_loading)
+            loading_thread.start()
         self.process = start_server(license, bin_path, cuda_version, self.port)
+
         while True:
             try:
                 if self.process.poll() is not None:
                     output, _ = self.process.communicate()
-                    output = output.decode('utf-8')
+                    output = output.decode("utf-8")
                     raise Exception(
                         f"Failed to start process.\nOutput: {output}\nTry to run it manually: `{' '.join(self.process.args)}`"
                     )
 
                 self.status()
                 break
             except ConnectionError as ex:
                 time.sleep(1)
 
+        if verbose:
+            loading_thread.join()
+            print()
+
+        self.loading = False
+        self.loaded = True
+
         def terminate():
             print("Stopping MariTalk...")
             self.stop_server()
 
         atexit.register(terminate)
 
+    def _show_loading(self):
+        spinner = ["⠋", "⠙", "⠚", "⠞", "⠖", "⠦", "⠴", "⠲", "⠳", "⠓"]
+        spinner_index = 0
+        start_time = time.time()
+
+        try:
+            while self.loading:
+                current_time = time.time()
+                elapsed_time = int(current_time - start_time)
+                minutes, seconds = divmod(elapsed_time, 60)
+
+                output = (
+                    f"\rLoading... {spinner[spinner_index]} ({minutes}min:{seconds}s)"
+                )
+                sys.stdout.write(output)
+                sys.stdout.flush()
+                spinner_index = (spinner_index + 1) % len(
+                    spinner
+                )
+                time.sleep(0.1)
+        except KeyboardInterrupt:
+            sys.stdout.flush()
+
     def stop_server(self):
         if not self.process:
             print("No process attached to this client!")
             return
         self.process.terminate()
         self.process = None
+        self.loaded = False
 
     def status(self):
         response = requests.get(self.api_url)
         return response.json()
 
     def generate_raw(
         self,
@@ -322,8 +413,10 @@
         if response.headers.get("content-type") == "application/json":
             return response.json()
 
         # Raise for any other failed responses
         response.raise_for_status()
 
     def generate_chat(self, *args, **kwargs):
-        raise Exception('This method was changed, please use `generate` for chat messages or `generate_raw` for raw few-shot examples instead.')
+        raise Exception(
+            "This method was changed, please use `generate` for chat messages or `generate_raw` for raw few-shot examples instead."
+        )
```

### Comparing `maritalk-0.2.3/maritalk/start.py` & `maritalk-0.2.4/maritalk/start.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,8 +27,8 @@
     atexit.register(lambda: process.terminate())
 
     while True:
         output = process.stdout.readline()
         if process.poll() is not None and output == b"":
             break
         if output:
-            print(output.decode().strip())
+            print(output.decode().strip(), end='')
```

### Comparing `maritalk-0.2.3/maritalk.egg-info/PKG-INFO` & `maritalk-0.2.4/maritalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maritalk
-Version: 0.2.3
+Version: 0.2.4
 Summary: Client library for the MariTalk API
 Author-email: Maritaca AI <info@maritaca.ai>
 License: The MIT License
         
         Copyright (c) Maritaca AI (https://maritaca.ai)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -45,15 +45,15 @@
 - [Exemplo de uso](#exemplo-de-uso)
 - [Exemplo de uso via requisições HTTP - Python](https://github.com/maritaca-ai/maritalk-api/blob/main/examples/api/maritalk_via_requisições_https.ipynb)
 - [Exemplo de uso via requisições HTTP - JavaScript](https://github.com/maritaca-ai/maritalk-api/blob/main/examples/api/maritalk_via_requisições_https.js)
 - [Exemplo MariTalk + RAG com LangChain](https://python.langchain.com/docs/integrations/chat/maritalk)
 - [Exemplo Maritalk no LlamaIndex](https://docs.llamaindex.ai/en/latest/examples/llm/maritalk)
 - [Documentação Swagger](https://chat.maritaca.ai/docs)
 
-[MariTalk local](https://github.com/maritaca-ai/maritalk-api/blob/main/README-Local.md)
+[MariTalk Local](https://github.com/maritaca-ai/maritalk-api/blob/main/README-Local.md)
 
 [Chat (gratuito)](#web-chat)
 
 # Introdução
 Este repositório contém o código e a documentação explicando como usar a API da MariTalk e a versão local para deploy on-premises.
 A MariTalk é uma assistente baseada em um modelo de linguagem que foi especialmente treinado para entender bem o português.
 Ela é capaz de seguir instruções de maneira zero-shot, assim como o ChatGPT.
```

### Comparing `maritalk-0.2.3/pyproject.toml` & `maritalk-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "maritalk"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="Maritaca AI", email="info@maritaca.ai" },
 ]
 description = "Client library for the MariTalk API"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
```

