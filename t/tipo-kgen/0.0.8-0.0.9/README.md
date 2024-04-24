# Comparing `tmp/tipo-kgen-0.0.8.tar.gz` & `tmp/tipo-kgen-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tipo-kgen-0.0.8.tar", last modified: Tue Apr 23 07:28:21 2024, max compression
+gzip compressed data, was "tipo-kgen-0.0.9.tar", last modified: Tue Apr 23 08:06:30 2024, max compression
```

## Comparing `tipo-kgen-0.0.8.tar` & `tipo-kgen-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 07:28:21.737453 tipo-kgen-0.0.8/
--rw-rw-rw-   0        0        0    11540 2024-03-23 06:06:25.000000 tipo-kgen-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      409 2024-04-23 07:28:21.736448 tipo-kgen-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2352 2024-04-18 03:16:31.000000 tipo-kgen-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 07:28:21.708150 tipo-kgen-0.0.8/kgen/
--rw-rw-rw-   0        0        0        0 2024-04-17 15:02:12.000000 tipo-kgen-0.0.8/kgen/__init__.py
--rw-rw-rw-   0        0        0     4111 2024-04-17 18:14:56.000000 tipo-kgen-0.0.8/kgen/formatter.py
--rw-rw-rw-   0        0        0     4254 2024-04-19 03:08:22.000000 tipo-kgen-0.0.8/kgen/generate.py
--rw-rw-rw-   0        0        0     1145 2024-04-19 07:28:22.000000 tipo-kgen-0.0.8/kgen/logging.py
--rw-rw-rw-   0        0        0     1072 2024-04-19 06:48:03.000000 tipo-kgen-0.0.8/kgen/metainfo.py
--rw-rw-rw-   0        0        0     2971 2024-04-23 07:27:15.000000 tipo-kgen-0.0.8/kgen/models.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:28:21.718666 tipo-kgen-0.0.8/kgen/tag-list/
--rw-rw-rw-   0        0        0        0 2024-04-17 16:47:26.000000 tipo-kgen-0.0.8/kgen/tag-list/__init__.py
--rw-rw-rw-   0        0        0  4459440 2024-04-17 15:02:11.000000 tipo-kgen-0.0.8/kgen/tag-list/artist.txt
--rw-rw-rw-   0        0        0  4079093 2024-04-17 15:02:11.000000 tipo-kgen-0.0.8/kgen/tag-list/characters.txt
--rw-rw-rw-   0        0        0   823337 2024-04-17 15:02:11.000000 tipo-kgen-0.0.8/kgen/tag-list/copyrights.txt
--rw-rw-rw-   0        0        0     8830 2024-04-17 15:02:11.000000 tipo-kgen-0.0.8/kgen/tag-list/meta.txt
--rw-rw-rw-   0        0        0      204 2024-04-19 03:04:45.000000 tipo-kgen-0.0.8/kgen/utils.py
--rw-rw-rw-   0        0        0       42 2024-04-23 07:28:21.738452 tipo-kgen-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      603 2024-04-23 07:28:17.000000 tipo-kgen-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 07:28:21.736448 tipo-kgen-0.0.8/tipo_kgen.egg-info/
--rw-rw-rw-   0        0        0      409 2024-04-23 07:28:21.000000 tipo-kgen-0.0.8/tipo_kgen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2024-04-23 07:28:21.000000 tipo-kgen-0.0.8/tipo_kgen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 07:28:21.000000 tipo-kgen-0.0.8/tipo_kgen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-17 17:29:04.000000 tipo-kgen-0.0.8/tipo_kgen.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2024-04-23 07:28:21.000000 tipo-kgen-0.0.8/tipo_kgen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-23 07:28:21.000000 tipo-kgen-0.0.8/tipo_kgen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 08:06:30.047920 tipo-kgen-0.0.9/
+-rw-rw-rw-   0        0        0    11540 2024-03-23 06:06:25.000000 tipo-kgen-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      409 2024-04-23 08:06:30.047398 tipo-kgen-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2352 2024-04-18 03:16:31.000000 tipo-kgen-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 08:06:30.021749 tipo-kgen-0.0.9/kgen/
+-rw-rw-rw-   0        0        0        0 2024-04-17 15:02:12.000000 tipo-kgen-0.0.9/kgen/__init__.py
+-rw-rw-rw-   0        0        0     4322 2024-04-23 08:04:22.000000 tipo-kgen-0.0.9/kgen/formatter.py
+-rw-rw-rw-   0        0        0     4256 2024-04-23 08:06:15.000000 tipo-kgen-0.0.9/kgen/generate.py
+-rw-rw-rw-   0        0        0     1145 2024-04-19 07:28:22.000000 tipo-kgen-0.0.9/kgen/logging.py
+-rw-rw-rw-   0        0        0     1072 2024-04-19 06:48:03.000000 tipo-kgen-0.0.9/kgen/metainfo.py
+-rw-rw-rw-   0        0        0     3363 2024-04-23 08:06:15.000000 tipo-kgen-0.0.9/kgen/models.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:06:30.032243 tipo-kgen-0.0.9/kgen/tag-list/
+-rw-rw-rw-   0        0        0        0 2024-04-17 16:47:26.000000 tipo-kgen-0.0.9/kgen/tag-list/__init__.py
+-rw-rw-rw-   0        0        0  4459440 2024-04-17 15:02:11.000000 tipo-kgen-0.0.9/kgen/tag-list/artist.txt
+-rw-rw-rw-   0        0        0  4079093 2024-04-17 15:02:11.000000 tipo-kgen-0.0.9/kgen/tag-list/characters.txt
+-rw-rw-rw-   0        0        0   823337 2024-04-17 15:02:11.000000 tipo-kgen-0.0.9/kgen/tag-list/copyrights.txt
+-rw-rw-rw-   0        0        0     8830 2024-04-17 15:02:11.000000 tipo-kgen-0.0.9/kgen/tag-list/meta.txt
+-rw-rw-rw-   0        0        0      206 2024-04-23 08:06:15.000000 tipo-kgen-0.0.9/kgen/utils.py
+-rw-rw-rw-   0        0        0       42 2024-04-23 08:06:30.048442 tipo-kgen-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      603 2024-04-23 07:36:59.000000 tipo-kgen-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:06:30.047398 tipo-kgen-0.0.9/tipo_kgen.egg-info/
+-rw-rw-rw-   0        0        0      409 2024-04-23 08:06:29.000000 tipo-kgen-0.0.9/tipo_kgen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2024-04-23 08:06:29.000000 tipo-kgen-0.0.9/tipo_kgen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 08:06:29.000000 tipo-kgen-0.0.9/tipo_kgen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-17 17:29:04.000000 tipo-kgen-0.0.9/tipo_kgen.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2024-04-23 08:06:29.000000 tipo-kgen-0.0.9/tipo_kgen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-23 08:06:29.000000 tipo-kgen-0.0.9/tipo_kgen.egg-info/top_level.txt
```

### Comparing `tipo-kgen-0.0.8/LICENSE` & `tipo-kgen-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.8/README.md` & `tipo-kgen-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.8/kgen/formatter.py` & `tipo-kgen-0.0.9/kgen/formatter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import pathlib
 
+from . import models
 from .metainfo import SPECIAL, POSSIBLE_QUALITY_TAGS, RATING_TAGS
 
 
 tag_list_folder = pathlib.Path(os.path.dirname(__file__)) / "tag-list"
 tag_lists = {
     os.path.splitext(f)[0]: set(open(tag_list_folder / f).read().strip().split("\n"))
     for f in os.listdir(tag_list_folder)
@@ -58,14 +59,18 @@
 characters: {characters.strip() or '<|empty|>'}
 copyrights: {copyrights.strip() or '<|empty|>'}
 aspect ratio: {f"{aspect_ratio:.1f}" or '<|empty|>'}
 target: {'<|' + target + '|>' if target else '<|long|>'}
 general: {special_tags}, {general.strip().strip(",")}<|input_end|>
 """.strip()
 
+    if models.model_have_quality_info[models.current_model_name]:
+        quality = ", ".join(tag_map.get("quality", ["masterpiece"]))
+        prompt = f"quality: {quality}\n{prompt}"
+
     return prompt
 
 
 if __name__ == "__main__":
     from json import dumps
 
     print(tag_lists.keys())
```

### Comparing `tipo-kgen-0.0.8/kgen/generate.py` & `tipo-kgen-0.0.9/kgen/generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 try:
     from llama_cpp import Llama
 except ImportError:
 
     class Llama:
         pass
 
+
 from transformers import (
     GenerationConfig,
     PreTrainedModel,
     PreTrainedTokenizerBase,
     set_seed,
 )
```

### Comparing `tipo-kgen-0.0.8/kgen/logging.py` & `tipo-kgen-0.0.9/kgen/logging.py`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.8/kgen/metainfo.py` & `tipo-kgen-0.0.9/kgen/metainfo.py`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.8/kgen/models.py` & `tipo-kgen-0.0.9/kgen/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,26 +3,37 @@
 
 from huggingface_hub import hf_hub_download
 from transformers import LlamaForCausalLM, LlamaTokenizer
 
 from .logging import logger
 
 
+text_model = None
+tokenizer = None
+current_model_name = None
+
+
 model_dir = pathlib.Path(__file__).parent / "models"
 model_list = [
     "KBlueLeaf/DanTagGen-delta",
     "KBlueLeaf/DanTagGen-beta",
     "KBlueLeaf/DanTagGen-alpha",
     "KBlueLeaf/DanTagGen-gamma",
 ]
 gguf_name = [
     "ggml-model-Q6_K.gguf",
     "ggml-model-Q8_0.gguf",
     "ggml-model-f16.gguf",
 ]
+model_have_quality_info = {
+    "DanTagGen-delta": True,
+    "DanTagGen-beta": False,
+    "DanTagGen-alpha": False,
+    "DanTagGen-gamma": False,
+}
 
 
 try:
     from llama_cpp import Llama
 except Exception:
     logger.warning("Llama-cpp-python cannot be imported")
     Llama = None
@@ -56,41 +67,44 @@
         for file in os.listdir(model_dir)
         if file.endswith(".gguf")
     ]
     return files
 
 
 def load_model(model_name=model_list[0], gguf=False, device="cpu"):
-    global text_model, tokenizer
+    global text_model, tokenizer, current_model_name
     if gguf:
+        model_name = os.path.basename(model_name)
+        model_repo_name = model_name.split("_")[0]
+        current_model_name = model_repo_name
         try:
             assert Llama is not None
-            model_name = os.path.basename(model_name)
             text_model = Llama(
                 str(model_dir / model_name),
                 n_ctx=384,
                 n_gpu_layers=0 if device == "cpu" else 1000,
                 verbose=False,
             )
             tokenizer = None
             logger.info(f"Llama-cpp-python/gguf model {model_name} loaded")
-            if device=="cuda":
+            if device == "cuda":
                 logger.warning(
                     "llama.cpp have reproducibility issue on cuda "
                     "(https://github.com/ggerganov/llama.cpp/pull/1346) "
                     "It is suggested to use cpu or "
                     "compile llama-cpp-python by yourself "
                     "and set GGML_CUDA_MAX_STREAMS in the file ggml-cuda.cu to 1."
                 )
             return
         except Exception as e:
             logger.warning(f"Llama-cpp-python/gguf model {model_name} load failed")
-            model_name = model_list[0]
+            model_name = model_repo_name
     logger.info(f"Using transformers model {model_name}")
     text_model = LlamaForCausalLM.from_pretrained(model_name).eval().half()
     tokenizer = LlamaTokenizer.from_pretrained(model_name)
+    current_model_name = model_name.split("/")[-1]
     logger.info(f"Model {model_name} loaded")
 
 
 if __name__ == "__main__":
     model_file = download_gguf()
     load_model(model_file, gguf=True)
```

### Comparing `tipo-kgen-0.0.8/kgen/tag-list/artist.txt` & `tipo-kgen-0.0.9/kgen/tag-list/artist.txt`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.8/kgen/tag-list/characters.txt` & `tipo-kgen-0.0.9/kgen/tag-list/characters.txt`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.8/kgen/tag-list/copyrights.txt` & `tipo-kgen-0.0.9/kgen/tag-list/copyrights.txt`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.8/kgen/tag-list/meta.txt` & `tipo-kgen-0.0.9/kgen/tag-list/meta.txt`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.8/setup.py` & `tipo-kgen-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="tipo-kgen",
     packages=find_packages(),
-    version="0.0.8",
+    version="0.0.9",
     license="Apache 2.0",
     url="https://github.com/KohakuBlueleaf/KGen",
     description=(
         "TIPO: Text to Image genration through "
         "text Presampling with LLMs for Optimal prompting"
     ),
     author="Shih-Ying Yeh(KohakuBlueLeaf)",
```

