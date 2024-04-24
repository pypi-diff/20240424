# Comparing `tmp/mlx_transformers-0.1.2.tar.gz` & `tmp/mlx_transformers-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx_transformers-0.1.2.tar", last modified: Mon Apr 22 16:28:43 2024, max compression
+gzip compressed data, was "mlx_transformers-0.1.3.tar", last modified: Wed Apr 24 16:06:42 2024, max compression
```

## Comparing `mlx_transformers-0.1.2.tar` & `mlx_transformers-0.1.3.tar`

### file list

```diff
@@ -1,38 +1,44 @@
-drwxr-xr-x   0 odunayoogundepo   (501) staff       (20)        0 2024-04-22 16:28:43.145086 mlx_transformers-0.1.2/
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)     1359 2024-04-19 02:15:19.000000 mlx_transformers-0.1.2/CONTRIBUTING.md
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)    11357 2024-04-16 01:01:16.000000 mlx_transformers-0.1.2/LICENSE
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)       38 2024-04-17 00:39:45.000000 mlx_transformers-0.1.2/MANIFEST.in
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)     4234 2024-04-22 16:28:43.144774 mlx_transformers-0.1.2/PKG-INFO
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)     3436 2024-04-22 16:27:30.000000 mlx_transformers-0.1.2/README.md
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)       90 2024-04-17 01:03:34.000000 mlx_transformers-0.1.2/pyproject.toml
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)      155 2024-04-22 11:27:08.000000 mlx_transformers-0.1.2/requirements.txt
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)       38 2024-04-22 16:28:43.145151 mlx_transformers-0.1.2/setup.cfg
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)      963 2024-04-22 16:28:39.000000 mlx_transformers-0.1.2/setup.py
-drwxr-xr-x   0 odunayoogundepo   (501) staff       (20)        0 2024-04-22 16:28:43.139040 mlx_transformers-0.1.2/src/
-drwxr-xr-x   0 odunayoogundepo   (501) staff       (20)        0 2024-04-22 16:28:43.140329 mlx_transformers-0.1.2/src/mlx_transformers/
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)        0 2024-04-16 01:11:50.000000 mlx_transformers-0.1.2/src/mlx_transformers/__init__.py
-drwxr-xr-x   0 odunayoogundepo   (501) staff       (20)        0 2024-04-22 16:28:43.143482 mlx_transformers-0.1.2/src/mlx_transformers/models/
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)      393 2024-04-22 15:47:11.000000 mlx_transformers-0.1.2/src/mlx_transformers/models/__init__.py
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)     1205 2024-04-22 15:47:11.000000 mlx_transformers-0.1.2/src/mlx_transformers/models/base.py
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)    27727 2024-04-22 15:53:15.000000 mlx_transformers-0.1.2/src/mlx_transformers/models/bert.py
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)     6553 2024-04-22 11:27:08.000000 mlx_transformers-0.1.2/src/mlx_transformers/models/cache.py
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)        7 2024-04-22 11:27:08.000000 mlx_transformers-0.1.2/src/mlx_transformers/models/clip.py
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)    25559 2024-04-22 16:09:01.000000 mlx_transformers-0.1.2/src/mlx_transformers/models/llama.py
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)        7 2024-04-22 11:27:08.000000 mlx_transformers-0.1.2/src/mlx_transformers/models/llava.py
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)    17437 2024-04-18 21:56:35.000000 mlx_transformers-0.1.2/src/mlx_transformers/models/m2m_100.py
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)     3147 2024-04-22 15:47:11.000000 mlx_transformers-0.1.2/src/mlx_transformers/models/modelling_outputs.py
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)    24983 2024-04-22 16:12:09.000000 mlx_transformers-0.1.2/src/mlx_transformers/models/roberta.py
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)        7 2024-04-22 11:27:08.000000 mlx_transformers-0.1.2/src/mlx_transformers/models/t5.py
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)     1592 2024-04-22 16:12:09.000000 mlx_transformers-0.1.2/src/mlx_transformers/models/utils.py
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)    16073 2024-04-19 02:15:41.000000 mlx_transformers-0.1.2/src/mlx_transformers/models/xlm_roberta.py
-drwxr-xr-x   0 odunayoogundepo   (501) staff       (20)        0 2024-04-22 16:28:43.144436 mlx_transformers-0.1.2/src/mlx_transformers.egg-info/
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)     4234 2024-04-22 16:28:43.000000 mlx_transformers-0.1.2/src/mlx_transformers.egg-info/PKG-INFO
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)      925 2024-04-22 16:28:43.000000 mlx_transformers-0.1.2/src/mlx_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)        1 2024-04-22 16:28:43.000000 mlx_transformers-0.1.2/src/mlx_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)      155 2024-04-22 16:28:43.000000 mlx_transformers-0.1.2/src/mlx_transformers.egg-info/requires.txt
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)       17 2024-04-22 16:28:43.000000 mlx_transformers-0.1.2/src/mlx_transformers.egg-info/top_level.txt
-drwxr-xr-x   0 odunayoogundepo   (501) staff       (20)        0 2024-04-22 16:28:43.144203 mlx_transformers-0.1.2/tests/
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)     8491 2024-04-22 15:47:11.000000 mlx_transformers-0.1.2/tests/test_bert.py
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)     1773 2024-04-22 16:12:09.000000 mlx_transformers-0.1.2/tests/test_llama.py
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)     9439 2024-04-22 15:56:46.000000 mlx_transformers-0.1.2/tests/test_roberta.py
--rw-r--r--   0 odunayoogundepo   (501) staff       (20)     2364 2024-04-19 14:34:03.000000 mlx_transformers-0.1.2/tests/test_xlm_roberta.py
+drwxr-xr-x   0 odunayoogundepo   (501) staff       (20)        0 2024-04-24 16:06:42.938916 mlx_transformers-0.1.3/
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)     1254 2024-04-23 02:15:21.000000 mlx_transformers-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)    11357 2024-04-16 01:01:16.000000 mlx_transformers-0.1.3/LICENSE
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)       38 2024-04-17 00:39:45.000000 mlx_transformers-0.1.3/MANIFEST.in
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)     5052 2024-04-24 16:06:42.938704 mlx_transformers-0.1.3/PKG-INFO
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)     4276 2024-04-24 16:02:56.000000 mlx_transformers-0.1.3/README.md
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)       90 2024-04-17 01:03:34.000000 mlx_transformers-0.1.3/pyproject.toml
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)      155 2024-04-24 12:36:02.000000 mlx_transformers-0.1.3/requirements.txt
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)       38 2024-04-24 16:06:42.938963 mlx_transformers-0.1.3/setup.cfg
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)      936 2024-04-24 16:06:27.000000 mlx_transformers-0.1.3/setup.py
+drwxr-xr-x   0 odunayoogundepo   (501) staff       (20)        0 2024-04-24 16:06:42.932332 mlx_transformers-0.1.3/src/
+drwxr-xr-x   0 odunayoogundepo   (501) staff       (20)        0 2024-04-24 16:06:42.933566 mlx_transformers-0.1.3/src/mlx_transformers/
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)       13 2024-04-24 16:02:56.000000 mlx_transformers-0.1.3/src/mlx_transformers/__init__.py
+drwxr-xr-x   0 odunayoogundepo   (501) staff       (20)        0 2024-04-24 16:06:42.937346 mlx_transformers-0.1.3/src/mlx_transformers/models/
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)      670 2024-04-24 16:02:56.000000 mlx_transformers-0.1.3/src/mlx_transformers/models/__init__.py
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)     1598 2024-04-24 16:02:56.000000 mlx_transformers-0.1.3/src/mlx_transformers/models/base.py
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)    28002 2024-04-24 16:02:56.000000 mlx_transformers-0.1.3/src/mlx_transformers/models/bert.py
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)     6812 2024-04-24 16:02:56.000000 mlx_transformers-0.1.3/src/mlx_transformers/models/cache.py
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)        7 2024-04-22 11:27:08.000000 mlx_transformers-0.1.3/src/mlx_transformers/models/clip.py
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)        0 2024-04-24 16:02:56.000000 mlx_transformers-0.1.3/src/mlx_transformers/models/fuyu.py
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)    25631 2024-04-24 16:02:56.000000 mlx_transformers-0.1.3/src/mlx_transformers/models/llama.py
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)        7 2024-04-22 11:27:08.000000 mlx_transformers-0.1.3/src/mlx_transformers/models/llava.py
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)    17512 2024-04-24 16:02:56.000000 mlx_transformers-0.1.3/src/mlx_transformers/models/m2m_100.py
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)     3129 2024-04-24 16:02:56.000000 mlx_transformers-0.1.3/src/mlx_transformers/models/modelling_outputs.py
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)      826 2024-04-24 16:02:56.000000 mlx_transformers-0.1.3/src/mlx_transformers/models/persimmon.py
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)    29165 2024-04-24 16:02:56.000000 mlx_transformers-0.1.3/src/mlx_transformers/models/phi.py
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)    29781 2024-04-24 16:02:56.000000 mlx_transformers-0.1.3/src/mlx_transformers/models/phi3.py
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)    25186 2024-04-24 16:02:56.000000 mlx_transformers-0.1.3/src/mlx_transformers/models/roberta.py
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)        7 2024-04-22 11:27:08.000000 mlx_transformers-0.1.3/src/mlx_transformers/models/t5.py
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)     2796 2024-04-24 16:02:56.000000 mlx_transformers-0.1.3/src/mlx_transformers/models/utils.py
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)    25168 2024-04-24 16:02:56.000000 mlx_transformers-0.1.3/src/mlx_transformers/models/xlm_roberta.py
+drwxr-xr-x   0 odunayoogundepo   (501) staff       (20)        0 2024-04-24 16:06:42.938435 mlx_transformers-0.1.3/src/mlx_transformers.egg-info/
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)     5052 2024-04-24 16:06:42.000000 mlx_transformers-0.1.3/src/mlx_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)     1110 2024-04-24 16:06:42.000000 mlx_transformers-0.1.3/src/mlx_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)        1 2024-04-24 16:06:42.000000 mlx_transformers-0.1.3/src/mlx_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)      155 2024-04-24 16:06:42.000000 mlx_transformers-0.1.3/src/mlx_transformers.egg-info/requires.txt
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)       17 2024-04-24 16:06:42.000000 mlx_transformers-0.1.3/src/mlx_transformers.egg-info/top_level.txt
+drwxr-xr-x   0 odunayoogundepo   (501) staff       (20)        0 2024-04-24 16:06:42.938240 mlx_transformers-0.1.3/tests/
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)     8487 2024-04-24 16:02:56.000000 mlx_transformers-0.1.3/tests/test_bert.py
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)     1061 2024-04-24 16:02:56.000000 mlx_transformers-0.1.3/tests/test_llama.py
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)     1034 2024-04-24 16:02:56.000000 mlx_transformers-0.1.3/tests/test_phi.py
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)     1201 2024-04-24 16:02:56.000000 mlx_transformers-0.1.3/tests/test_phi3.py
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)     9361 2024-04-24 16:02:56.000000 mlx_transformers-0.1.3/tests/test_roberta.py
+-rw-r--r--   0 odunayoogundepo   (501) staff       (20)     9380 2024-04-24 16:02:56.000000 mlx_transformers-0.1.3/tests/test_xlm_roberta.py
```

### Comparing `mlx_transformers-0.1.2/CONTRIBUTING.md` & `mlx_transformers-0.1.3/CONTRIBUTING.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,23 +9,14 @@
 3. Every PR should have passing tests and at least one review. 
 4. For code formatting install `pre-commit` using something like `pip install pre-commit` and run `pre-commit install`.
    This should install hooks for running `black` and `clang-format` to ensure
    consistent style for C++ and python code.
  
    You can also run the formatters manually as follows on individual files:
  
-     ```bash
-     clang-format -i file.cpp
-     ```
- 
-     ```bash
-     black file.py
-     ```
-
-     or,
 
      ```bash
      # single file
      pre-commit run --files file1.py 
 
      # specific files
      pre-commit run --files file1.py file2.py
```

### Comparing `mlx_transformers-0.1.2/LICENSE` & `mlx_transformers-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlx_transformers-0.1.2/PKG-INFO` & `mlx_transformers-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mlx-transformers
-Version: 0.1.2
-Summary: MLX transformers is a machine learning framework with similar Interface to Huggingface transformers using MLX core as backend.
+Version: 0.1.3
+Summary: MLX transformers is a machine learning framework with similar Interface     to Huggingface transformers.
 Home-page: https://github.com/ToluClassics/mlx-transformers
 Author: Ogundepo Odunayo
 Author-email: ogundepoodunayo@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -21,45 +21,58 @@
 Requires-Dist: transformers>=4.40.0
 
 # MLX Transformers
 
 [![PyPI](https://img.shields.io/pypi/v/mlx-transformers?color=red)](https://pypi.org/project/mlx-transformers/)
 
 
-MLX Transformers is a library that provides model implementation in [MLX](https://github.com/ml-explore/mlx). It uses a similar model interface as HuggingFace Transformers and provides a way to load and use models in Apple Silicon devices. Implemented models have the same modules 
+MLX Transformers is a library that provides model implementations in [MLX](https://github.com/ml-explore/mlx). It uses a similar model interface as HuggingFace Transformers and provides a way to load and use models in Apple Silicon devices. Implemented models have the same modules and module key as the original implementations in transformers.
 
-MLX transformers is currently only available for infernce on Apple Silicon devices. Training support will be added in the future.
+MLX transformers is currently only available for inference on Apple Silicon devices. Training support will be added in the future.
 
 # Installation
 
 This library is available on PyPI and can be installed using pip:
 
 ```bash
 pip install mlx-transformers
 ```
 
+It is also recommended to install [`asitop`](https://github.com/tlkh/asitop)
+which can be super useful for monitoring the GPU and CPU usage on Apple Silicon devices.
+
+## Models Supported
+
+- Phi Family of Models (Phi3, Phi2, Phi)
+- LLama
+- Machine Translation Models (NLLB, M2M-100)
+- Encoder Models (Bert, RoBERTa, XLMRoberta, Sentence Transformers)
 
 ## Quick Tour
 
 A list of the available models can be found in the `mlx_transformers.models` module and are also listed in the [section below](#available-model-architectures). The following example demonstrates how to load a model and use it for inference:
 
 
 - You can load the model using MLX transformers in few lines of code
 
     ```python
+    import mlx.core as mx
     from transformers import BertConfig, BertTokenizer
     from mlx_transformers.models import BertForMaskedLM as MLXBertForMaskedLM
 
     tokenizer = BertTokenizer.from_pretrained("bert-base-uncased")
     config = BertConfig.from_pretrained("bert-base-uncased")
+    
     model = MLXBertForMaskedLM(config)
     model.from_pretrained("bert-base-uncased")
 
     sample_input = "Hello, world!"
     inputs = tokenizer(sample_input, return_tensors="np")
+    inputs = {key: mx.array(v) for key, v in inputs.items()}
+
     outputs = model(**inputs)
     ```
 
 ### Sentence Transformer Example
 
 ```python
 import mlx.core as mx
@@ -82,42 +95,45 @@
 tokenizer = AutoTokenizer.from_pretrained('sentence-transformers/all-MiniLM-L6-v2')
 config = AutoConfig.from_pretrained('sentence-transformers/all-MiniLM-L6-v2')
 
 model = MLXBertModel(config)
 model.from_pretrained("sentence-transformers/all-MiniLM-L6-v2")
 
 inputs = tokenizer(sentences, return_tensors="np", padding=True, truncation=True)
+inputs = {key: mx.array(v) for key, v in inputs.items()}
+
 outputs = model(**inputs)
 
 sentence_embeddings = _mean_pooling(outputs.last_hidden_state, inputs.attention_mask)
 ```
 
 
-## Available Models
+## Other Examples
 
-The following models have been ported to MLX Transformers from Huggingface for inference:
+The `examples` directory contains a few examples that demonstrate how to use the models in MLX Transformers. 
 
-1. Bert
-2. Roberta
-3. XLMRoberta
-4. M2M100
-5. Sentence Transformers
-6. Llama
-7. CLIP -> Coming soon...
-8. T5 -> Coming soon...
+1. [LLama Example](examples/llama_generation.py)
+    ```bash
+    python3 examples/llama_generation.py --model-name "meta-llama/Llama-2-7b-hf"  
+    ```
 
-## Examples
+2. [NLLB Translation Example](examples/nllb_translation.py)
+    ```bash
+    python3 examples/nllb_translation.py --model_name facebook/nllb-200-distilled-600M --source_language English --target_language Yoruba --text_to_translate "Let us translate text to Yoruba"
 
-The `examples` directory contains a few examples that demonstrate how to use the models in MLX Transformers. 
+    Output:==> ['Ẹ jẹ́ ká tú àwọn ẹsẹ Bíbélì sí èdè Yoruba']
+    ```
 
-1. [LLama Example](examples/llama_generation.py)
+3. [Phi Generation Example](examples/phi3_generation.py)
     ```bash
-    python3 examples/llama_generation.py --model-name "meta-llama/Llama-2-7b-hf" --model-path meta-llama-Llama-2-7b-hf.npz 
+    python3 examples/phi3_generation.py --temp 1.0
     ```
 
+
 ## Benchmarks
 
 Coming soon...
 
 ## Contributions
 
-Contributions to MLX transformers are welcome. See the contributing documentation for instructions on setting up a development environment.
+Contributions to MLX transformers are welcome. We would like to have as many model implementations as possible.
+See the contributing documentation for instructions on setting up a development environment.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mlx_transformers-0.1.2/README.md` & `mlx_transformers-0.1.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,56 @@
 # MLX Transformers
 
 [![PyPI](https://img.shields.io/pypi/v/mlx-transformers?color=red)](https://pypi.org/project/mlx-transformers/)
 
 
-MLX Transformers is a library that provides model implementation in [MLX](https://github.com/ml-explore/mlx). It uses a similar model interface as HuggingFace Transformers and provides a way to load and use models in Apple Silicon devices. Implemented models have the same modules 
+MLX Transformers is a library that provides model implementations in [MLX](https://github.com/ml-explore/mlx). It uses a similar model interface as HuggingFace Transformers and provides a way to load and use models in Apple Silicon devices. Implemented models have the same modules and module key as the original implementations in transformers.
 
-MLX transformers is currently only available for infernce on Apple Silicon devices. Training support will be added in the future.
+MLX transformers is currently only available for inference on Apple Silicon devices. Training support will be added in the future.
 
 # Installation
 
 This library is available on PyPI and can be installed using pip:
 
 ```bash
 pip install mlx-transformers
 ```
 
+It is also recommended to install [`asitop`](https://github.com/tlkh/asitop)
+which can be super useful for monitoring the GPU and CPU usage on Apple Silicon devices.
+
+## Models Supported
+
+- Phi Family of Models (Phi3, Phi2, Phi)
+- LLama
+- Machine Translation Models (NLLB, M2M-100)
+- Encoder Models (Bert, RoBERTa, XLMRoberta, Sentence Transformers)
 
 ## Quick Tour
 
 A list of the available models can be found in the `mlx_transformers.models` module and are also listed in the [section below](#available-model-architectures). The following example demonstrates how to load a model and use it for inference:
 
 
 - You can load the model using MLX transformers in few lines of code
 
     ```python
+    import mlx.core as mx
     from transformers import BertConfig, BertTokenizer
     from mlx_transformers.models import BertForMaskedLM as MLXBertForMaskedLM
 
     tokenizer = BertTokenizer.from_pretrained("bert-base-uncased")
     config = BertConfig.from_pretrained("bert-base-uncased")
+    
     model = MLXBertForMaskedLM(config)
     model.from_pretrained("bert-base-uncased")
 
     sample_input = "Hello, world!"
     inputs = tokenizer(sample_input, return_tensors="np")
+    inputs = {key: mx.array(v) for key, v in inputs.items()}
+
     outputs = model(**inputs)
     ```
 
 ### Sentence Transformer Example
 
 ```python
 import mlx.core as mx
@@ -60,42 +73,45 @@
 tokenizer = AutoTokenizer.from_pretrained('sentence-transformers/all-MiniLM-L6-v2')
 config = AutoConfig.from_pretrained('sentence-transformers/all-MiniLM-L6-v2')
 
 model = MLXBertModel(config)
 model.from_pretrained("sentence-transformers/all-MiniLM-L6-v2")
 
 inputs = tokenizer(sentences, return_tensors="np", padding=True, truncation=True)
+inputs = {key: mx.array(v) for key, v in inputs.items()}
+
 outputs = model(**inputs)
 
 sentence_embeddings = _mean_pooling(outputs.last_hidden_state, inputs.attention_mask)
 ```
 
 
-## Available Models
+## Other Examples
 
-The following models have been ported to MLX Transformers from Huggingface for inference:
+The `examples` directory contains a few examples that demonstrate how to use the models in MLX Transformers. 
 
-1. Bert
-2. Roberta
-3. XLMRoberta
-4. M2M100
-5. Sentence Transformers
-6. Llama
-7. CLIP -> Coming soon...
-8. T5 -> Coming soon...
+1. [LLama Example](examples/llama_generation.py)
+    ```bash
+    python3 examples/llama_generation.py --model-name "meta-llama/Llama-2-7b-hf"  
+    ```
 
-## Examples
+2. [NLLB Translation Example](examples/nllb_translation.py)
+    ```bash
+    python3 examples/nllb_translation.py --model_name facebook/nllb-200-distilled-600M --source_language English --target_language Yoruba --text_to_translate "Let us translate text to Yoruba"
 
-The `examples` directory contains a few examples that demonstrate how to use the models in MLX Transformers. 
+    Output:==> ['Ẹ jẹ́ ká tú àwọn ẹsẹ Bíbélì sí èdè Yoruba']
+    ```
 
-1. [LLama Example](examples/llama_generation.py)
+3. [Phi Generation Example](examples/phi3_generation.py)
     ```bash
-    python3 examples/llama_generation.py --model-name "meta-llama/Llama-2-7b-hf" --model-path meta-llama-Llama-2-7b-hf.npz 
+    python3 examples/phi3_generation.py --temp 1.0
     ```
 
+
 ## Benchmarks
 
 Coming soon...
 
 ## Contributions
 
-Contributions to MLX transformers are welcome. See the contributing documentation for instructions on setting up a development environment.
+Contributions to MLX transformers are welcome. We would like to have as many model implementations as possible.
+See the contributing documentation for instructions on setting up a development environment.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mlx_transformers-0.1.2/setup.py` & `mlx_transformers-0.1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import setuptools
-from setuptools import find_packages, setup
+from setuptools import find_packages
 
-description = "MLX transformers is a machine learning framework with similar Interface to Huggingface transformers using MLX core as backend."
+description = "MLX transformers is a machine learning framework with similar Interface \
+    to Huggingface transformers."
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="mlx-transformers",
-    version="0.1.2",
+    version="0.1.3",
     author="Ogundepo Odunayo",
     author_email="ogundepoodunayo@gmail.com",
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ToluClassics/mlx-transformers",
     install_requires=requirements,
```

### Comparing `mlx_transformers-0.1.2/src/mlx_transformers/models/base.py` & `mlx_transformers-0.1.3/src/mlx_transformers/models/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,53 @@
 import importlib
-import os
-from typing import Optional
+from typing import Callable, Optional
 
 import mlx.core as mx
-from huggingface_hub import HfFileSystem, hf_hub_download
 from mlx.utils import tree_unflatten
-from safetensors.numpy import load_file
-from transformers import AutoConfig
-from transformers.utils.import_utils import is_safetensors_available
 
 CONFIG_FILE = "config.json"
 WEIGHTS_FILE_NAME = "model.safetensors"
 
 
 def _sanitize_keys(key):
     keys = key.split(".")
     return ".".join(keys[1:])
 
 
 class MlxPretrainedMixin:
-
     def from_pretrained(
         self,
         model_name_or_path: str,
         cache_dir: Optional[str] = None,
         revision: Optional[str] = "main",
         float16: bool = False,
+        huggingface_model_architecture: Optional[Callable] = None,
+        trust_remote_code: bool = False,
     ):
+        if huggingface_model_architecture:
+            architecture = huggingface_model_architecture
+        elif hasattr(self.config, "architectures"):
+            architecture = self.config.architectures[0]
+        else:
+            raise ValueError("No architecture found for loading this model")
 
-        architecture = self.config.architectures[0]
         transformers_module = importlib.import_module("transformers")
-
         _class = getattr(transformers_module, architecture, None)
 
-        model = _class.from_pretrained(model_name_or_path)
+        if not _class:
+            raise ValueError(f"Could not find the class for {architecture}")
+
+        dtype = mx.float16 if float16 else mx.float32
+
+        model = _class.from_pretrained(
+            model_name_or_path, trust_remote_code=trust_remote_code
+        )
+
         # # save the tensors
         tensors = {
-            key: mx.array(tensor.numpy()) for key, tensor in model.state_dict().items()
+            key: mx.array(tensor.numpy()).astype(dtype)
+            for key, tensor in model.state_dict().items()
         }
 
         tensors = [(key, tensor) for key, tensor in tensors.items()]
 
         self.update(tree_unflatten(tensors))
```

### Comparing `mlx_transformers-0.1.2/src/mlx_transformers/models/bert.py` & `mlx_transformers-0.1.3/src/mlx_transformers/models/bert.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,22 @@
 from typing import List, Optional, Tuple, Union
 
 import mlx.core as mx
 import mlx.nn as nn
 from transformers import BertConfig
 
 from .base import MlxPretrainedMixin
-from .modelling_outputs import *
+from .modelling_outputs import (
+    BaseModelOutputWithPastAndCrossAttentions,
+    BaseModelOutputWithPoolingAndCrossAttentions,
+    MaskedLMOutput,
+    QuestionAnsweringModelOutput,
+    SequenceClassifierOutput,
+    TokenClassifierOutput,
+)
 from .utils import ACT2FN, get_extended_attention_mask
 
 logger = logging.getLogger(__name__)
 
 
 class BertEmbeddings(nn.Module):
     def __init__(self, config: BertConfig):
@@ -57,16 +64,16 @@
 class BertSelfAttention(nn.Module):
     def __init__(self, config, position_embedding_type=None):
         super().__init__()
         if config.hidden_size % config.num_attention_heads != 0 and not hasattr(
             config, "embedding_size"
         ):
             raise ValueError(
-                f"The hidden size ({config.hidden_size}) is not a multiple of the number of attention "
-                f"heads ({config.num_attention_heads})"
+                f"The hidden size ({config.hidden_size}) is not a multiple of the number"
+                f"of attention heads ({config.num_attention_heads})"
             )
 
         self.num_attention_heads = config.num_attention_heads
         self.attention_head_size = int(config.hidden_size / config.num_attention_heads)
         self.all_head_size = self.num_attention_heads * self.attention_head_size
 
         self.query = nn.Linear(config.hidden_size, self.all_head_size)
@@ -92,21 +99,21 @@
         B, L, D = mixed_query_layer.shape
 
         key_layer = self.transpose_for_scores(self.key(hidden_states))
         value_layer = self.transpose_for_scores(self.value(hidden_states))
 
         query_layer = self.transpose_for_scores(mixed_query_layer)
 
-        # Take the dot product between "query" and "key" to get the raw attention scores.
+        # Take the dot product between "query" and "key" to get the raw attention scores
         attention_scores = query_layer @ key_layer.transpose(0, 1, 3, 2)
 
         attention_scores = attention_scores / math.sqrt(self.attention_head_size)
 
         if attention_mask is not None:
-            # Apply the attention mask is (precomputed for all layers in BertModel forward() function)
+            # Apply the attention mask is (precomputed for all layers in forward)
             attention_scores = attention_scores + attention_mask
 
         # Normalize the attention scores to probabilities.
         attention_probs = mx.softmax(attention_scores, axis=-1)
 
         # This is actually dropping out entire tokens to attend to, which might
         # seem a bit unusual, but is taken from the original Transformer paper.
@@ -149,15 +156,14 @@
 
     def __call__(
         self,
         hidden_states: mx.array,
         attention_mask: Optional[mx.array] = None,
         output_attentions: Optional[bool] = False,
     ) -> Tuple[mx.array]:
-
         self_outputs = self.self(
             hidden_states,
             attention_mask,
             output_attentions,
         )
         attention_output = self.output(self_outputs[0], hidden_states)
         outputs = (attention_output,) + self_outputs[
@@ -184,17 +190,22 @@
 class BertOutput(nn.Module):
     def __init__(self, config):
         super().__init__()
         self.dense = nn.Linear(config.intermediate_size, config.hidden_size)
         self.LayerNorm = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
         self.dropout = nn.Dropout(config.hidden_dropout_prob)
 
+        self.train = config.train if hasattr(config, "train") else False
+
     def __call__(self, hidden_states: mx.array, input_tensor: mx.array) -> mx.array:
         hidden_states = self.dense(hidden_states)
-        # hidden_states = self.dropout(hidden_states)
+
+        if self.train:
+            hidden_states = self.dropout(hidden_states)
+
         hidden_states = self.LayerNorm(hidden_states + input_tensor)
         return hidden_states
 
 
 class BertLayer(nn.Module):
     def __init__(self, config):
         super().__init__()
@@ -211,15 +222,14 @@
         attention_mask: Optional[mx.array] = None,
         head_mask: Optional[mx.array] = None,
         encoder_hidden_states: Optional[mx.array] = None,
         encoder_attention_mask: Optional[mx.array] = None,
         past_key_value: Optional[Tuple[Tuple[mx.array]]] = None,
         output_attentions: Optional[bool] = False,
     ) -> Tuple[mx.array]:
-
         self_attention_outputs = self.attention(
             hidden_states,
             attention_mask,
             output_attentions=output_attentions,
         )
 
         attention_output = self_attention_outputs[0]
@@ -251,15 +261,14 @@
         output_hidden_states: Optional[bool] = False,
         return_dict: Optional[bool] = True,
     ) -> Union[Tuple[mx.array], BaseModelOutputWithPastAndCrossAttentions]:
         all_hidden_states = () if output_hidden_states else None
         all_self_attentions = () if output_attentions else None
 
         for i, layer_module in enumerate(self.layer):
-
             if output_hidden_states:
                 all_hidden_states = all_hidden_states + (hidden_states,)
 
             layer_outputs = layer_module(
                 hidden_states,
                 attention_mask,
                 output_attentions,
@@ -300,14 +309,16 @@
         self.activation = nn.Tanh()  # TODO: fix tanh
 
     def __call__(self, hidden_states: mx.array) -> mx.array:
         # We "pool" the model by simply taking the hidden state corresponding
         # to the first token.
         first_token_tensor = hidden_states[:, 0]
         pooled_output = self.dense(first_token_tensor)
+
+        # TODO: fix tanh
         # pooled_output = self.activation(pooled_output)
 
         pooled_output = mx.tanh(pooled_output)
         return pooled_output
 
 
 class BertPredictionHeadTransform(nn.Module):
@@ -324,15 +335,14 @@
         hidden_states = self.dense(hidden_states)
         hidden_states = self.transform_act_fn(hidden_states)
         hidden_states = self.LayerNorm(hidden_states)
         return hidden_states
 
 
 class BertModel(nn.Module, MlxPretrainedMixin):
-
     def __init__(self, config, add_pooling_layer=True):
         super().__init__()
 
         self.config = config
 
         self.embeddings = BertEmbeddings(config)
         self.encoder = BertEncoder(config)
@@ -352,31 +362,28 @@
         token_type_ids: Optional[mx.array] = None,
         position_ids: Optional[mx.array] = None,
         use_cache: Optional[bool] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
     ) -> Union[Tuple[List], BaseModelOutputWithPoolingAndCrossAttentions]:
-
         output_attentions = (
             output_attentions
             if output_attentions is not None
             else self.config.output_attentions
         )
         output_hidden_states = (
             output_hidden_states
             if output_hidden_states is not None
             else self.config.output_hidden_states
         )
         return_dict = (
             return_dict if return_dict is not None else self.config.use_return_dict
         )
 
-        use_cache = False
-
         input_shape = input_ids.shape
 
         batch_size, seq_length = input_shape
 
         if attention_mask is None:
             attention_mask = mx.ones(((batch_size, seq_length + 0)))
 
@@ -430,16 +437,14 @@
         self.transform = BertPredictionHeadTransform(config)
 
         # The output weights are the same as the input embeddings, but there is
         # an output-only bias for each token.
         self.decoder = nn.Linear(config.hidden_size, config.vocab_size, bias=False)
 
         self.bias = mx.zeros(config.vocab_size)
-
-        # Need a link between the two variables so that the bias is correctly resized with `resize_token_embeddings`
         self.decoder.bias = self.bias
 
     def __call__(self, hidden_states):
         hidden_states = self.transform(hidden_states)
         hidden_states = self.decoder(hidden_states)
         return hidden_states
 
@@ -469,15 +474,14 @@
         position_ids: Optional[mx.array] = None,
         use_cache: Optional[bool] = None,
         labels: Optional[mx.array] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
     ):
-
         return_dict = (
             return_dict if return_dict is not None else self.config.use_return_dict
         )
         outputs = self.bert(
             input_ids,
             attention_mask=attention_mask,
             token_type_ids=token_type_ids,
@@ -536,17 +540,18 @@
         labels: Optional[mx.array] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
     ) -> Union[Tuple[mx.array], SequenceClassifierOutput]:
         r"""
         labels (`array` of shape `(batch_size,)`, *optional*):
-            Labels for computing the sequence classification/regression loss. Indices should be in `[0, ...,
-            config.num_labels - 1]`. If `config.num_labels == 1` a regression loss is computed (Mean-Square loss), If
-            `config.num_labels > 1` a classification loss is computed (Cross-Entropy).
+            Labels for computing the sequence classification/regression loss.
+            Indices should be in `[0, ..., config.num_labels - 1]`.
+            If `config.num_labels == 1` a regression loss is computed (Mean-Square loss)
+            If `config.num_labels > 1` a classification loss is computed (Cross-Entropy)
         """
         return_dict = (
             return_dict if return_dict is not None else self.config.use_return_dict
         )
 
         outputs = self.bert(
             input_ids,
@@ -612,14 +617,16 @@
             config.classifier_dropout
             if config.classifier_dropout is not None
             else config.hidden_dropout_prob
         )
         self.dropout = nn.Dropout(classifier_dropout)
         self.classifier = nn.Linear(config.hidden_size, config.num_labels)
 
+        self.train = config.train if hasattr(config, "train") else False
+
     def __call__(
         self,
         input_ids: Optional[mx.array] = None,
         attention_mask: Optional[mx.array] = None,
         token_type_ids: Optional[mx.array] = None,
         position_ids: Optional[mx.array] = None,
         labels: Optional[mx.array] = None,
@@ -643,15 +650,17 @@
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
 
         sequence_output = outputs.last_hidden_state
 
-        sequence_output = self.dropout(sequence_output)
+        if self.train:
+            sequence_output = self.dropout(sequence_output)
+
         logits = self.classifier(sequence_output)
 
         loss = None
         if labels is not None:
             loss_fct = nn.losses.cross_entropy
             loss = loss_fct(logits.view(-1, self.num_labels), labels.view(-1))
```

### Comparing `mlx_transformers-0.1.2/src/mlx_transformers/models/cache.py` & `mlx_transformers-0.1.3/src/mlx_transformers/models/cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any, Dict, List, Optional, Tuple
 
 import mlx.core as mx
 
 logger = logging.getLogger(__name__)
 
 
+# Adapted from: https://github.com/huggingface/transformers/blob/e74d793a3c3c0bc9bf3fb94bb31dd16934b1b0db/src/transformers/cache_utils.py#L14
 @dataclass
 class Cache:
     """
     Base, abstract class for all caches. The actual data structure is specific to each subclass.
     """
 
     def update(
@@ -46,61 +47,67 @@
         if max_length is not None and previous_seq_length + new_seq_length > max_length:
             return max_length - new_seq_length
         return previous_seq_length
 
     @property
     def seen_tokens(self):
         logger.warning_once(
-            "The `seen_tokens` attribute is deprecated and will be removed in v4.41. Use the `cache_position` "
+            "The `seen_tokens` attribute is deprecated and will be removed in v4.41."
+            "Use the `cache_position` "
             "model input instead."
         )
         if hasattr(self, "_seen_tokens"):
             return self._seen_tokens
         else:
             return None
 
 
 class DynamicCache(Cache):
     """
-    A cache that grows dynamically as more tokens are generated. This is the default for generative models.
+    A cache that grows dynamically as more tokens are generated.
+    This is the default for generative models.
 
-    It stores the Key and Value states as a list of tensors, one for each layer. The expected shape for each tensor is
+    It stores the Key and Value states as a list of tensors, one for each layer.
+    The expected shape for each tensor is
     `[batch_size, num_heads, seq_len, head_dim]`.
     """
 
     def __init__(self) -> None:
         self.key_cache: List[mx.array] = []
         self.value_cache: List[mx.array] = []
         self._seen_tokens = (
             0  # Used in `generate` to keep tally of how many tokens the cache has seen
         )
 
     def __getitem__(self, layer_idx: int) -> List[Tuple[mx.array]]:
         """
-        Support for backwards-compatible `past_key_value` indexing, e.g. `past_key_value[0][0].shape[2]` to get the
+        Support for backwards-compatible `past_key_value` indexing, e.g.
+        `past_key_value[0][0].shape[2]` to get the
         sequence length.
         """
         if layer_idx < len(self):
             return (self.key_cache[layer_idx], self.value_cache[layer_idx])
         else:
             raise KeyError(
                 f"Cache only has {len(self)} layers, attempted to access layer with index {layer_idx}"
             )
 
     def __iter__(self):
         """
-        Support for backwards-compatible `past_key_value` iteration, e.g. `for x in past_key_value:` to iterate over
+        Support for backwards-compatible `past_key_value` iteration, e.g.
+        `for x in past_key_value:` to iterate over
         keys and values
         """
         for layer_idx in range(len(self)):
             yield (self.key_cache[layer_idx], self.value_cache[layer_idx])
 
     def __len__(self):
         """
-        Support for backwards-compatible `past_key_value` length, e.g. `len(past_key_value)`. This value corresponds
+        Support for backwards-compatible `past_key_value` length, e.g.
+         `len(past_key_value)`. This value corresponds
         to the number of layers in the model.
         """
         return len(self.key_cache)
 
     def update(
         self,
         key_states: mx.array,
@@ -135,25 +142,33 @@
         else:
             self.key_cache[layer_idx] = key_states
             self.value_cache[layer_idx] = value_states
 
         return self.key_cache[layer_idx], self.value_cache[layer_idx]
 
     def get_seq_length(self, layer_idx: Optional[int] = 0) -> int:
-        """Returns the sequence length of the cached states. A layer index can be optionally passed."""
+        """
+        Returns the sequence length of the cached states.
+        A layer index can be optionally passed.
+        """
         if len(self.key_cache) <= layer_idx:
             return 0
         return self.key_cache[layer_idx].shape[-2]
 
     def get_max_length(self) -> Optional[int]:
-        """Returns the maximum sequence length of the cached states. DynamicCache does not have a maximum length."""
+        """
+        Returns the maximum sequence length of the cached states.
+        DynamicCache does not have a maximum length.
+        """
         return None
 
     def to_legacy_cache(self) -> Tuple[Tuple[mx.array], Tuple[mx.array]]:
-        """Converts the `DynamicCache` instance into the its equivalent in the legacy cache format."""
+        """
+        Converts the `DynamicCache` instance into the its equivalent in the legacy cache format.
+        """
         legacy_cache = ()
         for layer_idx in range(len(self)):
             legacy_cache += ((self.key_cache[layer_idx], self.value_cache[layer_idx]),)
         return legacy_cache
 
     @classmethod
     def from_legacy_cache(
```

### Comparing `mlx_transformers-0.1.2/src/mlx_transformers/models/llama.py` & `mlx_transformers-0.1.3/src/mlx_transformers/models/llama.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import math
-from typing import Optional
+from typing import Optional, Dict
 
 import mlx.core as mx
 import mlx.nn as nn
 import numpy as np
 from transformers import LlamaConfig
 
 from .base import MlxPretrainedMixin
 from .cache import Cache, DynamicCache
-from .modelling_outputs import *
+from .modelling_outputs import (
+    BaseModelOutputWithPast,
+    CausalLMOutputWithPast,
+)
 from .utils import ACT2FN
 
 
 class LlamaRMSNorm(nn.Module):
     def __init__(self, hidden_size, eps=1e-6):
         """
         LlamaRMSNorm is equivalent to T5LayerNorm
@@ -50,15 +53,15 @@
         )
         self.max_seq_len_cached = max_position_embeddings
 
         t = mx.arange(self.max_seq_len_cached).astype(mx.int64)
         t = t / self.scaling_factor
         freqs = mx.outer(t, self.inv_freq)
 
-        emb = mx.concatenate([freqs, freqs], axis=-1)
+        mx.concatenate([freqs, freqs], axis=-1)
 
     def __call__(self, x, position_ids):
         inv_freq_expanded = self.inv_freq[None, :, None].astype(mx.float32)
         inv_freq_expanded = mx.broadcast_to(
             inv_freq_expanded, (position_ids.shape[0], inv_freq_expanded.shape[1], 1)
         )
 
@@ -71,23 +74,21 @@
         cos = mx.cos(emb)
         sin = mx.sin(emb)
 
         return cos.astype(x_dtype), sin.astype(x_dtype)
 
 
 class LlamaLinearScalingRotaryEmbedding(LlamaRotaryEmbedding):
-
     def __call__(self, x, position_ids):
         position_ids = position_ids / self.scaling_factor
         cos, sin = super().__call__(x, position_ids)
         return cos, sin
 
 
 class LlamaDynamicNTKScalingRotaryEmbedding(LlamaRotaryEmbedding):
-
     def forward(self, x, position_ids):
         seq_len = mx.max(position_ids) + 1
         if seq_len > self.max_position_embeddings:
             base = self.base * (
                 (self.scaling_factor * seq_len / self.max_position_embeddings)
                 - (self.scaling_factor - 1)
             ) ** (self.dim / (self.dim - 2))
@@ -126,15 +127,14 @@
 
     def __call__(self, x):
         down_proj = self.down_proj(self.act_fn(self.gate_proj(x)) * self.up_proj(x))
         return down_proj
 
 
 def repeat_kv(hidden_states, n_rep):
-
     batch, num_key_value_heads, slen, head_dim = hidden_states.shape
     if n_rep == 1:
         return hidden_states
 
     hidden_states = hidden_states[:, :, None, :, :]
     hidden_states = mx.broadcast_to(
         hidden_states, (batch, num_key_value_heads, n_rep, slen, head_dim)
@@ -215,15 +215,14 @@
         attention_mask=None,
         position_ids=None,
         past_key_value=None,
         output_attentions=False,
         use_cache=False,
         cache_position=None,
     ):
-
         bsz, q_len, _ = hidden_states.shape
 
         query_states = self.q_proj(hidden_states)
         key_states = self.k_proj(hidden_states)
         value_states = self.v_proj(hidden_states)
 
         # Prepare the queries, keys and values for the attention computation
@@ -542,15 +541,14 @@
     def _update_causal_mask(
         self,
         attention_mask: mx.array,
         input_tensor: mx.array,
         cache_position: mx.array,
         past_seen_tokens: int,
     ):
-
         dtype = input_tensor.dtype
         min_dtype = np.finfo(np.float32).min
         sequence_length = input_tensor.shape[1]
         if hasattr(
             getattr(self.layers[0], "self_attn", {}), "past_key_value"
         ):  # static cache
             target_length = self.config.max_position_embeddings
@@ -606,15 +604,14 @@
 
         causal_mask = mx.array(causal_mask)
 
         return causal_mask
 
 
 class LlamaForCausalLM(nn.Module, MlxPretrainedMixin):
-
     def __init__(self, config):
         super().__init__()
         self.config = config
         self.model = LlamaModel(config)
         self.vocab_size = config.vocab_size
         self.lm_head = nn.Linear(config.hidden_size, config.vocab_size, bias=False)
 
@@ -663,16 +660,17 @@
         return_dict = (
             return_dict if return_dict is not None else self.config.use_return_dict
         )
 
         if attention_mask is not None and position_ids is None:
             # create position_ids on the fly for batch generation
             position_ids = attention_mask.astype(mx.int32).cumsum(-1) - 1
-            position_ids, attention_mask = np.array(position_ids), np.array(
-                attention_mask
+            position_ids, attention_mask = (
+                np.array(position_ids),
+                np.array(attention_mask),
             )
 
             position_ids = np.ma.array(
                 data=position_ids, mask=attention_mask == 0
             ).filled(1)
             position_ids = mx.array(position_ids)
             if past_key_values:
```

### Comparing `mlx_transformers-0.1.2/src/mlx_transformers/models/m2m_100.py` & `mlx_transformers-0.1.3/src/mlx_transformers/models/m2m_100.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Copyright © 2023 Apple Inc.
 
 import math
-import os
-from typing import List, Optional, Tuple
+from typing import Optional, Tuple
 
 import mlx.core as mx
 import mlx.nn as nn
 import numpy as np
 import torch
 from transformers import M2M100Config
 from transformers.modeling_attn_mask_utils import _prepare_4d_causal_attention_mask
 
+from .base import MlxPretrainedMixin
+
 
 def _prepare_4d_attention_mask(mask: mx.array, tgt_len: Optional[int] = None):
     """Create 4d attention mask from a 2d mask."""
 
     bsz, src_len = mask.shape
 
     if tgt_len is None:
@@ -108,15 +109,14 @@
         num_heads: int,
         dropout: float = 0.0,
         is_decoder: bool = False,
         bias: bool = True,
         is_causal: bool = False,
         args: M2M100Config = None,
     ):
-
         super().__init__()
         self.args = args
 
         self.embed_dim = embed_dim
         self.num_heads = num_heads
         self.dropout = dropout
 
@@ -140,15 +140,14 @@
         self,
         hidden_states: mx.array,
         key_value_states: Optional[mx.array] = None,
         past_key_value: Optional[Tuple[mx.array]] = None,
         attention_mask: Optional[mx.array] = None,
         layer_head_mask: Optional[mx.array] = None,
     ):
-
         is_cross_attention = key_value_states is not None
 
         bsz, tgt_len, _ = hidden_states.shape
 
         query_states = self.q_proj(hidden_states) * self.scaling
 
         if (
@@ -180,22 +179,23 @@
         value_states = value_states.reshape(proj_shape)
 
         src_len = key_states.shape[1]
         attn_weights = query_states @ key_states.transpose(0, 2, 1)
 
         if attn_weights.shape != (bsz * self.num_heads, tgt_len, src_len):
             raise ValueError(
-                f"Attention weights should be of size {(bsz * self.num_heads, tgt_len, src_len)}, but is"
-                f" {attn_weights.shape}"
+                f"Weights should be of size {(bsz * self.num_heads, tgt_len, src_len)}"
+                f", but is {attn_weights.shape}"
             )
 
         if attention_mask is not None:
             if attention_mask.shape != (bsz, 1, tgt_len, src_len):
                 raise ValueError(
-                    f"Attention mask should be of size {(bsz, 1, tgt_len, src_len)}, but is {attention_mask.shape}"
+                    f"Attention mask should be of size {(bsz, 1, tgt_len, src_len)}, "
+                    "but is {attention_mask.shape}"
                 )
 
             attn_weights = (
                 attn_weights.reshape(bsz, self.num_heads, tgt_len, src_len)
                 + attention_mask
             )
             attn_weights = attn_weights.reshape(bsz * self.num_heads, tgt_len, src_len)
@@ -351,15 +351,14 @@
             config.max_position_embeddings, embed_dim, self.padding_idx
         )
 
         self.layers = [M2M100EncoderLayer(config) for _ in range(config.encoder_layers)]
         self.layer_norm = nn.LayerNorm(embed_dim)
 
     def __call__(self, input_ids: mx.array, attention_mask: mx.array):
-
         input_shape = input_ids.shape
         input_ids = input_ids.reshape(-1, input_shape[-1])
 
         inputs_embeds = self.embed_tokens(input_ids) * self.embed_scale
 
         embed_pos = self.embed_positions(input_ids)
 
@@ -401,26 +400,26 @@
         self,
         input_ids: mx.array,
         attention_mask: mx.array,
         encoder_hidden_states: mx.array,
         encoder_attention_mask: mx.array,
         past_key_values: mx.array,
     ):
-
         input_shape = input_ids.shape
         input_ids = input_ids.reshape(-1, input_shape[-1])
 
         past_key_values_length = (
             past_key_values[0][0].shape[2] if past_key_values is not None else 0
         )
 
         inputs_embeds = self.embed_tokens(input_ids) * self.embed_scale
 
         # create causal mask
         # [bsz, seq_len] -> [bsz, 1, tgt_seq_len, src_seq_len]
+        # TODO: Fix this
         combined_attention_mask = _prepare_4d_causal_attention_mask(
             torch.tensor(np.array(attention_mask)),
             input_shape,
             torch.tensor(np.array(inputs_embeds)),
             past_key_values_length,
         )
         combined_attention_mask = mx.array(combined_attention_mask.numpy())
@@ -463,28 +462,27 @@
         input_ids: mx.array,
         attention_mask: mx.array,
         decoder_input_ids: mx.array,
         encoder_attention_mask: mx.array,
         decoder_attention_mask: mx.array,
         past_key_values: mx.array,
     ):
-
         encoder_hidden_states = self.encoder(input_ids, attention_mask)
         decoder_hidden_states = self.decoder(
             decoder_input_ids,
             encoder_hidden_states,
             decoder_attention_mask,
             encoder_attention_mask,
             past_key_values,
         )
 
         return decoder_hidden_states
 
 
-class M2M100ForConditionalGeneration(nn.Module):
+class M2M100ForConditionalGeneration(nn.Module, MlxPretrainedMixin):
     def __init__(self, config: M2M100Config):
         super().__init__()
 
         self.config = config
         self.model = M2M100Model(config)
         self.lm_head = nn.Linear(config.d_model, config.vocab_size, bias=False)
```

### Comparing `mlx_transformers-0.1.2/src/mlx_transformers/models/modelling_outputs.py` & `mlx_transformers-0.1.3/src/mlx_transformers/models/modelling_outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Optional, Tuple
 
 import mlx.core as mx
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
@@ -88,12 +88,11 @@
     past_key_values: Optional[Tuple[Tuple[mx.array]]] = None
     hidden_states: Optional[Tuple[mx.array, ...]] = None
     attentions: Optional[Tuple[mx.array, ...]] = None
 
 
 @dataclass
 class MaskedLMOutput:
-
     loss: Optional[mx.array] = None
     logits: mx.array = None
     hidden_states: Optional[Tuple[mx.array, ...]] = None
     attentions: Optional[Tuple[mx.array, ...]] = None
```

### Comparing `mlx_transformers-0.1.2/src/mlx_transformers/models/roberta.py` & `mlx_transformers-0.1.3/src/mlx_transformers/models/roberta.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,21 @@
 from typing import List, Optional, Tuple, Union
 
 import mlx.core as mx
 import mlx.nn as nn
 from transformers import RobertaConfig
 
 from .base import MlxPretrainedMixin
-from .modelling_outputs import *
+from .modelling_outputs import (
+    BaseModelOutputWithPastAndCrossAttentions,
+    BaseModelOutputWithPoolingAndCrossAttentions,
+    SequenceClassifierOutput,
+    TokenClassifierOutput,
+    QuestionAnsweringModelOutput,
+)
 from .utils import ACT2FN, get_extended_attention_mask
 
 logger = logging.getLogger(__name__)
 
 
 def create_position_ids_from_input_ids(
     input_ids, padding_idx, past_key_values_length=0
@@ -48,15 +54,14 @@
     def __call__(
         self,
         input_ids: mx.array,
         position_ids: mx.array,
         token_type_ids: mx.array = None,
         inputs_embeds: mx.array = None,
     ) -> mx.array:
-
         if position_ids is None:
             if input_ids is not None:
                 position_ids = create_position_ids_from_input_ids(
                     input_ids, self.padding_idx
                 )
             else:
                 position_ids = self.create_position_ids_from_inputs_embeds(
@@ -64,15 +69,15 @@
                 )
 
         if input_ids is not None:
             input_shape = input_ids.shape
         else:
             input_shape = inputs_embeds.shape[:-1]
 
-        seq_length = input_shape[1]
+        input_shape[1]
 
         if token_type_ids is None:
             token_type_ids = mx.zeros(input_shape, dtype="int32")
 
         if inputs_embeds is None:
             inputs_embeds = self.word_embeddings(input_ids)
 
@@ -83,15 +88,14 @@
 
         position_embeddings = self.position_embeddings(position_ids)
         embeddings += position_embeddings
 
         return self.LayerNorm(embeddings)
 
     def create_position_ids_from_inputs_embeds(self, inputs_embeds: mx.array):
-
         input_shape = inputs_embeds.shape[:-1]
         seq_length = input_shape[1]
 
         position_ids = mx.arange(
             self.padding_idx + 1,
             seq_length + self.padding_idx + 1,
             dtype=inputs_embeds.dtype,
@@ -197,15 +201,14 @@
 
     def __call__(
         self,
         hidden_states: mx.array,
         attention_mask: Optional[mx.array] = None,
         output_attentions: Optional[bool] = False,
     ) -> Tuple[mx.array]:
-
         self_outputs = self.self(
             hidden_states,
             attention_mask,
             output_attentions,
         )
         attention_output = self.output(self_outputs[0], hidden_states)
         outputs = (attention_output,) + self_outputs[
@@ -258,15 +261,14 @@
         attention_mask: Optional[mx.array] = None,
         head_mask: Optional[mx.array] = None,
         encoder_hidden_states: Optional[mx.array] = None,
         encoder_attention_mask: Optional[mx.array] = None,
         past_key_value: Optional[Tuple[Tuple[mx.array]]] = None,
         output_attentions: Optional[bool] = False,
     ) -> Tuple[mx.array]:
-
         self_attention_outputs = self.attention(
             hidden_states,
             attention_mask,
             output_attentions=output_attentions,
         )
 
         attention_output = self_attention_outputs[0]
@@ -298,15 +300,14 @@
         output_hidden_states: Optional[bool] = False,
         return_dict: Optional[bool] = True,
     ) -> Union[Tuple[mx.array], BaseModelOutputWithPastAndCrossAttentions]:
         all_hidden_states = () if output_hidden_states else None
         all_self_attentions = () if output_attentions else None
 
         for i, layer_module in enumerate(self.layer):
-
             if output_hidden_states:
                 all_hidden_states = all_hidden_states + (hidden_states,)
 
             layer_outputs = layer_module(
                 hidden_states,
                 attention_mask,
                 output_attentions,
@@ -354,15 +355,14 @@
         # pooled_output = self.activation(pooled_output)
 
         pooled_output = mx.tanh(pooled_output)
         return pooled_output
 
 
 class RobertaModel(nn.Module, MlxPretrainedMixin):
-
     def __init__(self, config, add_pooling_layer=True):
         super().__init__()
 
         self.config = config
 
         self.embeddings = RobertaEmbeddings(config)
         self.encoder = RobertaEncoder(config)
@@ -382,31 +382,28 @@
         token_type_ids: Optional[mx.array] = None,
         position_ids: Optional[mx.array] = None,
         use_cache: Optional[bool] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
     ) -> Union[Tuple[List], BaseModelOutputWithPoolingAndCrossAttentions]:
-
         output_attentions = (
             output_attentions
             if output_attentions is not None
             else self.config.output_attentions
         )
         output_hidden_states = (
             output_hidden_states
             if output_hidden_states is not None
             else self.config.output_hidden_states
         )
         return_dict = (
             return_dict if return_dict is not None else self.config.use_return_dict
         )
 
-        use_cache = False
-
         input_shape = input_ids.shape
 
         batch_size, seq_length = input_shape
 
         if attention_mask is None:
             attention_mask = mx.ones(((batch_size, seq_length + 0)))
 
@@ -494,15 +491,14 @@
         token_type_ids: Optional[mx.array] = None,
         position_ids: Optional[mx.array] = None,
         labels: Optional[mx.array] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
     ) -> Union[Tuple[mx.array], SequenceClassifierOutput]:
-
         return_dict = (
             return_dict if return_dict is not None else self.config.use_return_dict
         )
 
         outputs = self.roberta(
             input_ids,
             attention_mask=attention_mask,
@@ -518,15 +514,17 @@
         loss = None
         if labels is not None:
             # move labels to correct device to enable model parallelism
             labels = labels.to(logits.device)
             if self.config.problem_type is None:
                 if self.num_labels == 1:
                     self.config.problem_type = "regression"
-                elif self.num_labels > 1 and (labels.dtype == mx.array):
+                elif self.num_labels > 1 and (
+                    labels.dtype == mx.long or labels.dtype == mx.int
+                ):
                     self.config.problem_type = "single_label_classification"
                 else:
                     self.config.problem_type = "multi_label_classification"
 
             if self.config.problem_type == "regression":
                 loss_fct = nn.losses.mse_loss
                 if self.num_labels == 1:
@@ -574,15 +572,14 @@
         token_type_ids: Optional[mx.array] = None,
         position_ids: Optional[mx.array] = None,
         labels: Optional[mx.array] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
     ) -> Union[Tuple[mx.array], TokenClassifierOutput]:
-
         return_dict = (
             return_dict if return_dict is not None else self.config.use_return_dict
         )
 
         outputs = self.roberta(
             input_ids,
             attention_mask=attention_mask,
@@ -634,15 +631,14 @@
         position_ids: Optional[mx.array] = None,
         start_positions: Optional[mx.array] = None,
         end_positions: Optional[mx.array] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
     ) -> Union[Tuple[mx.array], QuestionAnsweringModelOutput]:
-
         return_dict = (
             return_dict if return_dict is not None else self.config.use_return_dict
         )
 
         outputs = self.roberta(
             input_ids,
             attention_mask=attention_mask,
```

### Comparing `mlx_transformers-0.1.2/src/mlx_transformers.egg-info/PKG-INFO` & `mlx_transformers-0.1.3/src/mlx_transformers.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mlx-transformers
-Version: 0.1.2
-Summary: MLX transformers is a machine learning framework with similar Interface to Huggingface transformers using MLX core as backend.
+Version: 0.1.3
+Summary: MLX transformers is a machine learning framework with similar Interface     to Huggingface transformers.
 Home-page: https://github.com/ToluClassics/mlx-transformers
 Author: Ogundepo Odunayo
 Author-email: ogundepoodunayo@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -21,45 +21,58 @@
 Requires-Dist: transformers>=4.40.0
 
 # MLX Transformers
 
 [![PyPI](https://img.shields.io/pypi/v/mlx-transformers?color=red)](https://pypi.org/project/mlx-transformers/)
 
 
-MLX Transformers is a library that provides model implementation in [MLX](https://github.com/ml-explore/mlx). It uses a similar model interface as HuggingFace Transformers and provides a way to load and use models in Apple Silicon devices. Implemented models have the same modules 
+MLX Transformers is a library that provides model implementations in [MLX](https://github.com/ml-explore/mlx). It uses a similar model interface as HuggingFace Transformers and provides a way to load and use models in Apple Silicon devices. Implemented models have the same modules and module key as the original implementations in transformers.
 
-MLX transformers is currently only available for infernce on Apple Silicon devices. Training support will be added in the future.
+MLX transformers is currently only available for inference on Apple Silicon devices. Training support will be added in the future.
 
 # Installation
 
 This library is available on PyPI and can be installed using pip:
 
 ```bash
 pip install mlx-transformers
 ```
 
+It is also recommended to install [`asitop`](https://github.com/tlkh/asitop)
+which can be super useful for monitoring the GPU and CPU usage on Apple Silicon devices.
+
+## Models Supported
+
+- Phi Family of Models (Phi3, Phi2, Phi)
+- LLama
+- Machine Translation Models (NLLB, M2M-100)
+- Encoder Models (Bert, RoBERTa, XLMRoberta, Sentence Transformers)
 
 ## Quick Tour
 
 A list of the available models can be found in the `mlx_transformers.models` module and are also listed in the [section below](#available-model-architectures). The following example demonstrates how to load a model and use it for inference:
 
 
 - You can load the model using MLX transformers in few lines of code
 
     ```python
+    import mlx.core as mx
     from transformers import BertConfig, BertTokenizer
     from mlx_transformers.models import BertForMaskedLM as MLXBertForMaskedLM
 
     tokenizer = BertTokenizer.from_pretrained("bert-base-uncased")
     config = BertConfig.from_pretrained("bert-base-uncased")
+    
     model = MLXBertForMaskedLM(config)
     model.from_pretrained("bert-base-uncased")
 
     sample_input = "Hello, world!"
     inputs = tokenizer(sample_input, return_tensors="np")
+    inputs = {key: mx.array(v) for key, v in inputs.items()}
+
     outputs = model(**inputs)
     ```
 
 ### Sentence Transformer Example
 
 ```python
 import mlx.core as mx
@@ -82,42 +95,45 @@
 tokenizer = AutoTokenizer.from_pretrained('sentence-transformers/all-MiniLM-L6-v2')
 config = AutoConfig.from_pretrained('sentence-transformers/all-MiniLM-L6-v2')
 
 model = MLXBertModel(config)
 model.from_pretrained("sentence-transformers/all-MiniLM-L6-v2")
 
 inputs = tokenizer(sentences, return_tensors="np", padding=True, truncation=True)
+inputs = {key: mx.array(v) for key, v in inputs.items()}
+
 outputs = model(**inputs)
 
 sentence_embeddings = _mean_pooling(outputs.last_hidden_state, inputs.attention_mask)
 ```
 
 
-## Available Models
+## Other Examples
 
-The following models have been ported to MLX Transformers from Huggingface for inference:
+The `examples` directory contains a few examples that demonstrate how to use the models in MLX Transformers. 
 
-1. Bert
-2. Roberta
-3. XLMRoberta
-4. M2M100
-5. Sentence Transformers
-6. Llama
-7. CLIP -> Coming soon...
-8. T5 -> Coming soon...
+1. [LLama Example](examples/llama_generation.py)
+    ```bash
+    python3 examples/llama_generation.py --model-name "meta-llama/Llama-2-7b-hf"  
+    ```
 
-## Examples
+2. [NLLB Translation Example](examples/nllb_translation.py)
+    ```bash
+    python3 examples/nllb_translation.py --model_name facebook/nllb-200-distilled-600M --source_language English --target_language Yoruba --text_to_translate "Let us translate text to Yoruba"
 
-The `examples` directory contains a few examples that demonstrate how to use the models in MLX Transformers. 
+    Output:==> ['Ẹ jẹ́ ká tú àwọn ẹsẹ Bíbélì sí èdè Yoruba']
+    ```
 
-1. [LLama Example](examples/llama_generation.py)
+3. [Phi Generation Example](examples/phi3_generation.py)
     ```bash
-    python3 examples/llama_generation.py --model-name "meta-llama/Llama-2-7b-hf" --model-path meta-llama-Llama-2-7b-hf.npz 
+    python3 examples/phi3_generation.py --temp 1.0
     ```
 
+
 ## Benchmarks
 
 Coming soon...
 
 ## Contributions
 
-Contributions to MLX transformers are welcome. See the contributing documentation for instructions on setting up a development environment.
+Contributions to MLX transformers are welcome. We would like to have as many model implementations as possible.
+See the contributing documentation for instructions on setting up a development environment.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mlx_transformers-0.1.2/src/mlx_transformers.egg-info/SOURCES.txt` & `mlx_transformers-0.1.3/src/mlx_transformers.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,25 @@
 src/mlx_transformers.egg-info/requires.txt
 src/mlx_transformers.egg-info/top_level.txt
 src/mlx_transformers/models/__init__.py
 src/mlx_transformers/models/base.py
 src/mlx_transformers/models/bert.py
 src/mlx_transformers/models/cache.py
 src/mlx_transformers/models/clip.py
+src/mlx_transformers/models/fuyu.py
 src/mlx_transformers/models/llama.py
 src/mlx_transformers/models/llava.py
 src/mlx_transformers/models/m2m_100.py
 src/mlx_transformers/models/modelling_outputs.py
+src/mlx_transformers/models/persimmon.py
+src/mlx_transformers/models/phi.py
+src/mlx_transformers/models/phi3.py
 src/mlx_transformers/models/roberta.py
 src/mlx_transformers/models/t5.py
 src/mlx_transformers/models/utils.py
 src/mlx_transformers/models/xlm_roberta.py
 tests/test_bert.py
 tests/test_llama.py
+tests/test_phi.py
+tests/test_phi3.py
 tests/test_roberta.py
 tests/test_xlm_roberta.py
```

### Comparing `mlx_transformers-0.1.2/tests/test_bert.py` & `mlx_transformers-0.1.3/tests/test_bert.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 
 def load_hgf_model(model_name: str, hgf_model_class):
     model = hgf_model_class.from_pretrained(model_name)
     return model
 
 
 class TestMlxBert(unittest.TestCase):
-
     @classmethod
     def setUpClass(cls) -> None:
         cls.model_name = "bert-base-uncased"
         cls.config = BertConfig.from_pretrained(cls.model_name)
         cls.tokenizer = BertTokenizer.from_pretrained(cls.model_name)
         cls.hgf_model_class = BertForMaskedLM
 
@@ -61,15 +60,14 @@
         outputs_hgf = hgf_model(**inputs_hgf)
         outputs_hgf = outputs_hgf.logits.detach().numpy()
 
         self.assertTrue(np.allclose(outputs_mlx, outputs_hgf, atol=1e-4))
 
 
 class TestMlxBertForSequenceClassification(unittest.TestCase):
-
     @classmethod
     def setUpClass(cls) -> None:
         cls.model_name = "textattack/bert-base-uncased-yelp-polarity"
         cls.config = AutoConfig.from_pretrained(cls.model_name)
         cls.tokenizer = AutoTokenizer.from_pretrained(cls.model_name)
 
         cls.hgf_model_class = BertForSequenceClassification
@@ -108,15 +106,14 @@
         predicted_class_id = outputs_hgf.argmax().item()
         hgf_label = hgf_model.config.id2label[predicted_class_id]
 
         self.assertEqual(mlx_label, hgf_label)
 
 
 class TestMlxBertForTokenClassification(unittest.TestCase):
-
     @classmethod
     def setUpClass(cls) -> None:
         cls.model_name = "dslim/bert-base-NER"
         cls.config = AutoConfig.from_pretrained(cls.model_name)
         cls.tokenizer = AutoTokenizer.from_pretrained(cls.model_name)
 
         cls.hgf_model_class = BertForTokenClassification
@@ -173,15 +170,14 @@
             for t in hgf_predicted_token_class_ids[0]
         ]
 
         self.assertEqual(mlx_predicted_tokens_classes, hgf_predicted_tokens_classes)
 
 
 class TestMlxBertForQuestionAnswering(unittest.TestCase):
-
     @classmethod
     def setUpClass(cls) -> None:
         cls.model_name = "deepset/bert-base-cased-squad2"
         cls.tokenizer = AutoTokenizer.from_pretrained(cls.model_name)
         cls.config = AutoConfig.from_pretrained(cls.model_name)
 
         cls.hgf_model_class = BertForQuestionAnswering
```

### Comparing `mlx_transformers-0.1.2/tests/test_roberta.py` & `mlx_transformers-0.1.3/tests/test_roberta.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 import os
-import sys
 import unittest
 
 import mlx.core as mx
 import numpy as np
 from transformers import (
+    AutoTokenizer,
     RobertaConfig,
-    RobertaModel,
-    RobertaTokenizer,
+    RobertaForQuestionAnswering,
     RobertaForSequenceClassification,
     RobertaForTokenClassification,
     RobertaForQuestionAnswering,
-    AutoTokenizer
+    AutoTokenizer,
+    RobertaModel,
+    RobertaTokenizer,
 )
 
+from src.mlx_transformers.models import (
+    RobertaForQuestionAnswering as MlxRobertaForQuestionAnswering,
+)
+from src.mlx_transformers.models import (
+    RobertaForSequenceClassification as MlxRobertaForSequenceClassification,
+)
+from src.mlx_transformers.models import (
+    RobertaForTokenClassification as MlxRobertaForTokenClassification,
+)
 from src.mlx_transformers.models import RobertaModel as MlxRobertaModel
-from src.mlx_transformers.models import RobertaForSequenceClassification as MlxRobertaForSequenceClassification
-from src.mlx_transformers.models import RobertaForTokenClassification as MlxRobertaForTokenClassification
-from src.mlx_transformers.models import RobertaForQuestionAnswering as MlxRobertaForQuestionAnswering
 from src.mlx_transformers.models.utils import convert
 
 
 def load_model(model_name: str, mlx_model_class, hgf_model_class):
     current_directory = os.path.dirname(os.path.realpath(__file__))
     weights_path = os.path.join(
-        current_directory,
-        "model_checkpoints",
-        model_name.replace(
-            "/",
-            "-") + ".npz")
+        current_directory, "model_checkpoints", model_name.replace("/", "-") + ".npz"
+    )
 
     if not os.path.exists(weights_path):
         convert(model_name, weights_path, hgf_model_class)
 
     config = RobertaConfig.from_pretrained(model_name)
     # print(config)
     model = mlx_model_class(config)
@@ -44,24 +48,20 @@
 
 def load_hgf_model(model_name: str, hgf_model_class):
     model = hgf_model_class.from_pretrained(model_name)
     return model
 
 
 class TestMlxRoberta(unittest.TestCase):
-
     @classmethod
     def setUpClass(cls) -> None:
         cls.model_name = "FacebookAI/roberta-base"
         cls.model_class = MlxRobertaModel
         cls.hgf_model_class = RobertaModel
-        cls.model = load_model(
-            cls.model_name,
-            cls.model_class,
-            cls.hgf_model_class)
+        cls.model = load_model(cls.model_name, cls.model_class, cls.hgf_model_class)
         cls.tokenizer = RobertaTokenizer.from_pretrained(cls.model_name)
         cls.input_text = "Hello, my dog is cute"
 
     def test_forward(self) -> None:
         inputs = self.tokenizer(
             self.input_text, return_tensors="np", padding=True, truncation=True
         )
@@ -86,24 +86,20 @@
         outputs_hgf = hgf_model(**inputs_hgf)
         outputs_hgf = outputs_hgf.last_hidden_state.detach().numpy()
 
         self.assertTrue(np.allclose(outputs_mlx, outputs_hgf, atol=1e-4))
 
 
 class TestMlxRobertaForSequenceClassification(unittest.TestCase):
-
     @classmethod
     def setUpClass(cls) -> None:
         cls.model_name = "cardiffnlp/twitter-roberta-base-emotion"
         cls.model_class = MlxRobertaForSequenceClassification
         cls.hgf_model_class = RobertaForSequenceClassification
-        cls.model = load_model(
-            cls.model_name,
-            cls.model_class,
-            cls.hgf_model_class)
+        cls.model = load_model(cls.model_name, cls.model_class, cls.hgf_model_class)
         cls.tokenizer = AutoTokenizer.from_pretrained(cls.model_name)
         cls.input_text = "Hello, my dog is cute"
 
     def test_forward(self) -> None:
         inputs = self.tokenizer(
             self.input_text, return_tensors="np", padding=True, truncation=True
         )
@@ -133,84 +129,81 @@
         predicted_class_id = outputs_hgf.argmax().item()
         hgf_label = hgf_model.config.id2label[predicted_class_id]
 
         self.assertEqual(mlx_label, hgf_label)
 
 
 class TestMlxRobertaForTokenClassification(unittest.TestCase):
-
     @classmethod
     def setUpClass(cls) -> None:
         cls.model_name = "Jean-Baptiste/roberta-large-ner-english"
         cls.model_class = MlxRobertaForTokenClassification
         cls.hgf_model_class = RobertaForTokenClassification
-        cls.model = load_model(
-            cls.model_name,
-            cls.model_class,
-            cls.hgf_model_class)
+        cls.model = load_model(cls.model_name, cls.model_class, cls.hgf_model_class)
         cls.tokenizer = AutoTokenizer.from_pretrained(cls.model_name)
         cls.input_text = "HuggingFace is a company based in Paris and New York"
 
     def test_forward(self) -> None:
         inputs = self.tokenizer(
             self.input_text,
             return_tensors="np",
             padding=True,
             truncation=True,
-            add_special_tokens=False)
+            add_special_tokens=False,
+        )
 
         inputs = {key: mx.array(v) for key, v in inputs.items()}
         outputs = self.model(**inputs)
         self.assertIsInstance(outputs.logits, mx.array)
 
     def test_model_output_hgf(self):
         inputs_mlx = self.tokenizer(
             self.input_text,
             return_tensors="np",
             padding=True,
             truncation=True,
-            add_special_tokens=False)
+            add_special_tokens=False,
+        )
 
         inputs_mlx = {key: mx.array(v) for key, v in inputs_mlx.items()}
         outputs_mlx = self.model(**inputs_mlx)
         outputs_mlx = np.array(outputs_mlx.logits)
         mlx_predicted_token_class_ids = outputs_mlx.argmax(-1)
         mlx_predicted_tokens_classes = [
-            self.model.config.id2label[t.item()] for t in mlx_predicted_token_class_ids[0]]
+            self.model.config.id2label[t.item()]
+            for t in mlx_predicted_token_class_ids[0]
+        ]
 
         inputs_hgf = self.tokenizer(
             self.input_text,
             return_tensors="pt",
             padding=True,
             truncation=True,
-            add_special_tokens=False)
+            add_special_tokens=False,
+        )
         hgf_model = load_hgf_model(self.model_name, self.hgf_model_class)
         outputs_hgf = hgf_model(**inputs_hgf)
         outputs_hgf = outputs_hgf.logits
 
         hgf_predicted_token_class_ids = outputs_hgf.argmax(-1)
         hgf_predicted_tokens_classes = [
-            hgf_model.config.id2label[t.item()] for t in hgf_predicted_token_class_ids[0]]
+            hgf_model.config.id2label[t.item()]
+            for t in hgf_predicted_token_class_ids[0]
+        ]
 
-        self.assertEqual(
-            mlx_predicted_tokens_classes,
-            hgf_predicted_tokens_classes)
+        self.assertEqual(mlx_predicted_tokens_classes, hgf_predicted_tokens_classes)
 
 
 class TestMlxRobertaForQuestionAnswering(unittest.TestCase):
-
     @classmethod
     def setUpClass(cls) -> None:
         cls.model_name = "deepset/roberta-base-squad2"
         cls.model_class = MlxRobertaForQuestionAnswering
         cls.hgf_model_class = RobertaForQuestionAnswering
-        cls.model = load_model(
-            cls.model_name,
-            cls.model_class,
-            cls.hgf_model_class)
+        cls.model = load_model(cls.model_name, cls.model_class, cls.hgf_model_class)
         cls.tokenizer = AutoTokenizer.from_pretrained(cls.model_name)
         cls.input_question = "Who was Jim Henson?"
         cls.input_text = "Jim Henson was a nice puppet"
 
     def test_forward(self) -> None:
         inputs = self.tokenizer(
             self.input_question, self.input_text, return_tensors="np"
@@ -227,32 +220,36 @@
         )
 
         inputs_mlx = {key: mx.array(v) for key, v in inputs_mlx.items()}
         outputs_mlx = self.model(**inputs_mlx)
 
         mlx_answer_start_index = outputs_mlx.start_logits.argmax().item()
         mlx_answer_end_index = outputs_mlx.end_logits.argmax().item()
-        mlx_predict_answer_tokens = inputs_mlx['input_ids'].tolist()
-        mlx_predict_answer_tokens = mlx_predict_answer_tokens[
-            0][mlx_answer_start_index: mlx_answer_end_index + 1]
+        mlx_predict_answer_tokens = inputs_mlx["input_ids"].tolist()
+        mlx_predict_answer_tokens = mlx_predict_answer_tokens[0][
+            mlx_answer_start_index : mlx_answer_end_index + 1
+        ]
         mlx_answer = self.tokenizer.decode(
-            mlx_predict_answer_tokens, skip_special_tokens=True)
+            mlx_predict_answer_tokens, skip_special_tokens=True
+        )
 
         inputs_hgf = self.tokenizer(
             self.input_question, self.input_text, return_tensors="pt"
         )
 
         hgf_model = load_hgf_model(self.model_name, self.hgf_model_class)
         outputs_hgf = hgf_model(**inputs_hgf)
 
         hgf_answer_start_index = outputs_hgf.start_logits.argmax()
         hgf_answer_end_index = outputs_hgf.end_logits.argmax()
-        hgf_predict_answer_tokens = inputs_hgf.input_ids[0,
-                                                         hgf_answer_start_index: hgf_answer_end_index + 1]
+        hgf_predict_answer_tokens = inputs_hgf.input_ids[
+            0, hgf_answer_start_index : hgf_answer_end_index + 1
+        ]
         hgf_answer = self.tokenizer.decode(
-            hgf_predict_answer_tokens, skip_special_tokens=True)
+            hgf_predict_answer_tokens, skip_special_tokens=True
+        )
 
         self.assertEqual(mlx_answer, hgf_answer)
 
 
 if __name__ == "__main__":
     unittest.main()
```

