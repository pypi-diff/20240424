# Comparing `tmp/ai_microcore-3.6.0.tar.gz` & `tmp/ai_microcore-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_microcore-3.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ai_microcore-3.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ai_microcore-3.6.0.tar` & `ai_microcore-3.6.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rwxr-xr-x   0        0        0     1091 2023-11-04 16:00:47.197704 ai_microcore-3.6.0/LICENSE
--rwxr-xr-x   0        0        0    11116 2024-04-04 12:54:33.488412 ai_microcore-3.6.0/README.md
--rwxr-xr-x   0        0        0     3988 2024-04-20 16:37:09.703182 ai_microcore-3.6.0/microcore/__init__.py
--rwxr-xr-x   0        0        0     6544 2024-04-20 12:26:13.641652 ai_microcore-3.6.0/microcore/_env.py
--rwxr-xr-x   0        0        0     3790 2024-04-20 15:07:06.612137 ai_microcore-3.6.0/microcore/_llm_functions.py
--rwxr-xr-x   0        0        0      786 2024-04-20 12:35:24.174582 ai_microcore-3.6.0/microcore/_prepare_llm_args.py
--rwxr-xr-x   0        0        0     2319 2024-03-08 00:49:48.900573 ai_microcore-3.6.0/microcore/ai_func/__init__.py
--rwxr-xr-x   0        0        0      314 2023-11-04 16:00:47.368478 ai_microcore-3.6.0/microcore/ai_func/python_ai_func.j2
--rwxr-xr-x   0        0        0      576 2023-11-04 19:26:33.244252 ai_microcore-3.6.0/microcore/ai_modules.py
--rwxr-xr-x   0        0        0    11591 2024-04-20 14:59:40.736447 ai_microcore-3.6.0/microcore/configuration.py
--rwxr-xr-x   0        0        0     3133 2024-02-15 20:01:36.859722 ai_microcore-3.6.0/microcore/embedding_db/__init__.py
--rwxr-xr-x   0        0        0     4565 2024-02-15 19:46:15.503154 ai_microcore-3.6.0/microcore/embedding_db/chromadb.py
--rwxr-xr-x   0        0        0     8369 2024-03-08 00:49:49.038994 ai_microcore-3.6.0/microcore/file_storage.py
--rwxr-xr-x   0        0        0     4725 2024-04-20 12:35:24.223611 ai_microcore-3.6.0/microcore/json_parsing.py
--rwxr-xr-x   0        0        0       16 2023-11-06 23:41:28.213361 ai_microcore-3.6.0/microcore/llm/__init__.py
--rwxr-xr-x   0        0        0     4708 2024-04-16 08:56:56.272317 ai_microcore-3.6.0/microcore/llm/_openai_llm_v0.py
--rwxr-xr-x   0        0        0     5120 2024-04-18 17:18:22.746984 ai_microcore-3.6.0/microcore/llm/_openai_llm_v1.py
--rwxr-xr-x   0        0        0     3655 2024-04-16 13:59:52.503374 ai_microcore-3.6.0/microcore/llm/anthropic.py
--rwxr-xr-x   0        0        0     4479 2024-04-16 09:04:29.151454 ai_microcore-3.6.0/microcore/llm/google_genai.py
--rwxr-xr-x   0        0        0     5801 2024-04-18 13:00:32.311278 ai_microcore-3.6.0/microcore/llm/google_vertex_ai.py
--rwxr-xr-x   0        0        0     3229 2024-04-16 14:08:39.822867 ai_microcore-3.6.0/microcore/llm/local_llm.py
--rwxr-xr-x   0        0        0     4812 2024-04-20 14:21:18.005758 ai_microcore-3.6.0/microcore/llm/local_transformers.py
--rwxr-xr-x   0        0        0      272 2023-11-06 23:49:42.323932 ai_microcore-3.6.0/microcore/llm/openai_llm.py
--rwxr-xr-x   0        0        0     2466 2024-04-16 08:13:17.036046 ai_microcore-3.6.0/microcore/logging.py
--rwxr-xr-x   0        0        0      642 2024-03-08 00:49:48.881046 ai_microcore-3.6.0/microcore/message_types.py
--rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.559200 ai_microcore-3.6.0/microcore/templating/__init__.py
--rwxr-xr-x   0        0        0      525 2023-11-12 15:43:10.028753 ai_microcore-3.6.0/microcore/templating/jinja2.py
--rwxr-xr-x   0        0        0     1455 2024-03-31 01:09:15.566074 ai_microcore-3.6.0/microcore/text2speech/elevenlabs.py
--rwxr-xr-x   0        0        0     1046 2024-03-11 12:20:49.086082 ai_microcore-3.6.0/microcore/types.py
--rwxr-xr-x   0        0        0     1601 2024-04-19 09:12:25.103139 ai_microcore-3.6.0/microcore/ui.py
--rwxr-xr-x   0        0        0     9072 2024-04-20 14:50:05.806382 ai_microcore-3.6.0/microcore/utils.py
--rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.618937 ai_microcore-3.6.0/microcore/wrappers/__init__.py
--rwxr-xr-x   0        0        0     1559 2024-04-18 13:05:21.831255 ai_microcore-3.6.0/microcore/wrappers/llm_response_wrapper.py
--rwxr-xr-x   0        0        0      480 2024-04-02 14:01:24.033112 ai_microcore-3.6.0/microcore/wrappers/prompt_wrapper.py
--rwxr-xr-x   0        0        0     1450 2024-04-18 14:27:33.934530 ai_microcore-3.6.0/pyproject.toml
--rw-r--r--   0        0        0    11811 1970-01-01 00:00:00.000000 ai_microcore-3.6.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1091 2023-11-04 16:00:47.197704 ai_microcore-3.6.1/LICENSE
+-rwxr-xr-x   0        0        0    11116 2024-04-04 12:54:33.488412 ai_microcore-3.6.1/README.md
+-rwxr-xr-x   0        0        0     3988 2024-04-23 23:26:29.842689 ai_microcore-3.6.1/microcore/__init__.py
+-rwxr-xr-x   0        0        0     6667 2024-04-23 20:32:58.168012 ai_microcore-3.6.1/microcore/_env.py
+-rwxr-xr-x   0        0        0     3790 2024-04-20 15:07:06.612137 ai_microcore-3.6.1/microcore/_llm_functions.py
+-rwxr-xr-x   0        0        0      786 2024-04-20 12:35:24.174582 ai_microcore-3.6.1/microcore/_prepare_llm_args.py
+-rwxr-xr-x   0        0        0     2319 2024-03-08 00:49:48.900573 ai_microcore-3.6.1/microcore/ai_func/__init__.py
+-rwxr-xr-x   0        0        0      314 2023-11-04 16:00:47.368478 ai_microcore-3.6.1/microcore/ai_func/python_ai_func.j2
+-rwxr-xr-x   0        0        0      576 2023-11-04 19:26:33.244252 ai_microcore-3.6.1/microcore/ai_modules.py
+-rwxr-xr-x   0        0        0    11591 2024-04-20 14:59:40.736447 ai_microcore-3.6.1/microcore/configuration.py
+-rwxr-xr-x   0        0        0     3133 2024-02-15 20:01:36.859722 ai_microcore-3.6.1/microcore/embedding_db/__init__.py
+-rwxr-xr-x   0        0        0     4565 2024-02-15 19:46:15.503154 ai_microcore-3.6.1/microcore/embedding_db/chromadb.py
+-rwxr-xr-x   0        0        0     8400 2024-04-23 02:00:56.476715 ai_microcore-3.6.1/microcore/file_storage.py
+-rwxr-xr-x   0        0        0     4725 2024-04-20 12:35:24.223611 ai_microcore-3.6.1/microcore/json_parsing.py
+-rwxr-xr-x   0        0        0       16 2023-11-06 23:41:28.213361 ai_microcore-3.6.1/microcore/llm/__init__.py
+-rwxr-xr-x   0        0        0     4708 2024-04-16 08:56:56.272317 ai_microcore-3.6.1/microcore/llm/_openai_llm_v0.py
+-rwxr-xr-x   0        0        0     5120 2024-04-18 17:18:22.746984 ai_microcore-3.6.1/microcore/llm/_openai_llm_v1.py
+-rwxr-xr-x   0        0        0     3655 2024-04-16 13:59:52.503374 ai_microcore-3.6.1/microcore/llm/anthropic.py
+-rwxr-xr-x   0        0        0     4479 2024-04-16 09:04:29.151454 ai_microcore-3.6.1/microcore/llm/google_genai.py
+-rwxr-xr-x   0        0        0     5801 2024-04-18 13:00:32.311278 ai_microcore-3.6.1/microcore/llm/google_vertex_ai.py
+-rwxr-xr-x   0        0        0     3413 2024-04-23 17:22:46.408066 ai_microcore-3.6.1/microcore/llm/local_llm.py
+-rwxr-xr-x   0        0        0     5815 2024-04-23 19:57:00.633732 ai_microcore-3.6.1/microcore/llm/local_transformers.py
+-rwxr-xr-x   0        0        0      272 2023-11-06 23:49:42.323932 ai_microcore-3.6.1/microcore/llm/openai_llm.py
+-rwxr-xr-x   0        0        0     2490 2024-04-22 18:59:09.500665 ai_microcore-3.6.1/microcore/logging.py
+-rwxr-xr-x   0        0        0      642 2024-03-08 00:49:48.881046 ai_microcore-3.6.1/microcore/message_types.py
+-rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.559200 ai_microcore-3.6.1/microcore/templating/__init__.py
+-rwxr-xr-x   0        0        0      525 2023-11-12 15:43:10.028753 ai_microcore-3.6.1/microcore/templating/jinja2.py
+-rwxr-xr-x   0        0        0     1455 2024-03-31 01:09:15.566074 ai_microcore-3.6.1/microcore/text2speech/elevenlabs.py
+-rwxr-xr-x   0        0        0     1046 2024-03-11 12:20:49.086082 ai_microcore-3.6.1/microcore/types.py
+-rwxr-xr-x   0        0        0     1601 2024-04-19 09:12:25.103139 ai_microcore-3.6.1/microcore/ui.py
+-rwxr-xr-x   0        0        0     9089 2024-04-21 17:42:07.690371 ai_microcore-3.6.1/microcore/utils.py
+-rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.618937 ai_microcore-3.6.1/microcore/wrappers/__init__.py
+-rwxr-xr-x   0        0        0     1559 2024-04-18 13:05:21.831255 ai_microcore-3.6.1/microcore/wrappers/llm_response_wrapper.py
+-rwxr-xr-x   0        0        0      480 2024-04-02 14:01:24.033112 ai_microcore-3.6.1/microcore/wrappers/prompt_wrapper.py
+-rwxr-xr-x   0        0        0     1450 2024-04-18 14:27:33.934530 ai_microcore-3.6.1/pyproject.toml
+-rw-r--r--   0        0        0    11811 1970-01-01 00:00:00.000000 ai_microcore-3.6.1/PKG-INFO
```

### Comparing `ai_microcore-3.6.0/LICENSE` & `ai_microcore-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.0/README.md` & `ai_microcore-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.0/microcore/__init__.py` & `ai_microcore-3.6.1/microcore/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,8 +139,8 @@
     "configuration",
     "Config",
     "types",
     "ui",
     # "wrappers",
 ]
 
-__version__ = "3.6.0"
+__version__ = "3.6.1"
```

### Comparing `ai_microcore-3.6.0/microcore/_env.py` & `ai_microcore-3.6.1/microcore/_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dataclasses import dataclass, field, asdict
+from dataclasses import dataclass, field, asdict, fields
 from importlib.util import find_spec
 import jinja2
 
 from .configuration import Config, ApiType, LLMConfigError
 from . import AbstractEmbeddingDB
 from .types import TplFunctionType, LLMAsyncFunctionType, LLMFunctionType
 from .templating.jinja2 import make_jinja2_env, make_tpl_function
@@ -135,28 +135,33 @@
 
 
 configure: callable = _Configure
 """Applies configuration to MicroCore environment"""
 
 if True:  # pylint: disable=W0125
     # This block is inside a condition to avoid breaking IDE autocompletion
+
+    _fields = list(map(lambda f: f.name, fields(Config)))
+
     def _config_builder_wrapper(cfg: Config | dict = None, **kwargs):
         """
         - Convert configuration keys to uppercase
         - Add LLM_ prefix to keys if necessary
         - Allow to configure from Config instance or dictionary
         """
         if cfg:
             assert not kwargs, "Cannot pass both cfg and kwargs"
         if isinstance(cfg, dict):
             return _config_builder_wrapper(**cfg)
         kwargs = {str(k).upper(): v for k, v in kwargs.items()}
         for k in list(kwargs.keys()):
-            if not hasattr(Config, k) and hasattr(Config, f"LLM_{k}"):
-                kwargs[f"LLM_{k}"] = kwargs.pop(k)
+            if not hasattr(Config, k) and (
+                hasattr(Config, key := f"LLM_{k}") or key in _fields
+            ):
+                kwargs[key] = kwargs.pop(k)
         return _Configure(**(cfg and asdict(cfg) or kwargs))
 
     configure = _config_builder_wrapper
 
 _env: Env | None = None
```

### Comparing `ai_microcore-3.6.0/microcore/_llm_functions.py` & `ai_microcore-3.6.1/microcore/_llm_functions.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.0/microcore/_prepare_llm_args.py` & `ai_microcore-3.6.1/microcore/_prepare_llm_args.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.0/microcore/ai_func/__init__.py` & `ai_microcore-3.6.1/microcore/ai_func/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.0/microcore/ai_modules.py` & `ai_microcore-3.6.1/microcore/ai_modules.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.0/microcore/configuration.py` & `ai_microcore-3.6.1/microcore/configuration.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.0/microcore/embedding_db/__init__.py` & `ai_microcore-3.6.1/microcore/embedding_db/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.0/microcore/embedding_db/chromadb.py` & `ai_microcore-3.6.1/microcore/embedding_db/chromadb.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.0/microcore/file_storage.py` & `ai_microcore-3.6.1/microcore/file_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 import shutil
 from pathlib import Path
 import chardet
 
 from ._env import config
 from .utils import file_link, list_files
 
+_missing = object()
+
 
 class Storage:
     @property
     def path(self) -> Path:
         return Path(config().STORAGE_PATH)
 
     @property
@@ -98,29 +100,29 @@
             shutil.rmtree(path)
         else:
             os.remove(path)
 
     def write(
         self,
         name: str | Path,
-        content: str = None,
+        content: str = _missing,
         rewrite_existing: bool = None,
         backup_existing: bool = None,
         encoding: str = None,
         append: bool = False,
     ) -> str | os.PathLike:
         """
         :return: str File name for further usage
         """
         if rewrite_existing is None:
             rewrite_existing = True
         if backup_existing is None:
             backup_existing = not append
         encoding = encoding or self.default_encoding
-        if content is None:
+        if content == _missing:
             content = name
             name = f"out{self.default_ext}"
 
         base_name = Path(name).with_suffix("")
         ext = Path(name).suffix or self.default_ext
 
         file_name = f"{base_name}{ext}"
```

### Comparing `ai_microcore-3.6.0/microcore/json_parsing.py` & `ai_microcore-3.6.1/microcore/json_parsing.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.0/microcore/llm/_openai_llm_v0.py` & `ai_microcore-3.6.1/microcore/llm/_openai_llm_v0.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.0/microcore/llm/_openai_llm_v1.py` & `ai_microcore-3.6.1/microcore/llm/_openai_llm_v1.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.0/microcore/llm/anthropic.py` & `ai_microcore-3.6.1/microcore/llm/anthropic.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.0/microcore/llm/google_genai.py` & `ai_microcore-3.6.1/microcore/llm/google_genai.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.0/microcore/llm/google_vertex_ai.py` & `ai_microcore-3.6.1/microcore/llm/google_vertex_ai.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.0/microcore/llm/local_llm.py` & `ai_microcore-3.6.1/microcore/llm/local_llm.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,17 @@
                 prepare_chat_messages(prompt)
                 if config.CHAT_MODE
                 else prepare_prompt(prompt)
             )
             response = await inference_fn(prompt, **args)
             for cb in options["callbacks"]:
                 cb(response)
-            return LLMResponse(response)
+            if not isinstance(response, LLMResponse):
+                response = LLMResponse(response)
+            return response
 
         def llm(prompt, **kwargs):
             try:
                 loop = asyncio.get_running_loop()
                 if loop.is_running():
                     with _sync_await() as sa:
                         return sa(allm(prompt, **kwargs))
@@ -82,13 +84,15 @@
                 prepare_chat_messages(prompt)
                 if config.CHAT_MODE
                 else prepare_prompt(prompt)
             )
             response = inference_fn(prompt, **args)
             for cb in options["callbacks"]:
                 cb(response)
-            return LLMResponse(response)
+            if not isinstance(response, LLMResponse):
+                response = LLMResponse(response)
+            return response
 
         async def allm(prompt, **kwargs):
             return llm(prompt, **kwargs)
 
     return llm, allm
```

### Comparing `ai_microcore-3.6.0/microcore/llm/local_transformers.py` & `ai_microcore-3.6.1/microcore/llm/local_transformers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,86 +1,117 @@
 import logging
 import gc
 
 import transformers
 import torch
 
 from .local_llm import make_llm_functions as make_local_llm_functions
-from ..configuration import Config
+from ..wrappers.llm_response_wrapper import LLMResponse
+from ..configuration import Config, LLMConfigError
 from ..types import LLMFunctionType, LLMAsyncFunctionType
 
 
 def inference(prompt: str, model, tokenizer, **kwargs):
     inputs = tokenizer(prompt, return_tensors="pt").to(model.device)
     outputs = model.generate(**inputs, **kwargs)
-    out = tokenizer.decode(outputs[0][len(inputs[0]) :], skip_special_tokens=True)
-    return out
+    outputs = [
+        tokenizer.decode(i[len(inputs[0]) :], skip_special_tokens=True) for i in outputs
+    ]
+    return LLMResponse(outputs[0], dict(all=outputs))
 
 
 def pipeline_inference(prompt: str, pipeline, **kwargs):
     raw_output = pipeline(prompt, **{"return_full_text": False, **kwargs})
-    return raw_output[0]["generated_text"]
+    return LLMResponse(
+        raw_output[0]["generated_text"],
+        dict(all=list(map(lambda x: x["generated_text"], raw_output))),
+    )
+
+
+def clear_mem():
+    gc.collect()
+    torch.cuda.empty_cache()
 
 
+def try_make_model_config(config: Config):
+    try:
+        model_config = transformers.AutoConfig.from_pretrained(
+            config.MODEL,
+            trust_remote_code=True,
+        )
+    except OSError:
+        model_config = None
+    if config.INIT_PARAMS.get("gradient_checkpointing"):
+        if model_config:
+            model_config.gradient_checkpointing = True
+        else:
+            raise LLMConfigError(
+                "Can't apply gradient checkpointing without model config."
+            )
+    return model_config
+
 def make_llm_functions(
     config: Config, env
 ) -> tuple[LLMFunctionType, LLMAsyncFunctionType]:
     logging.info(f"Loading local Transformers model {config.MODEL}...")
     params = config.INIT_PARAMS
 
     tokenizer = params.get("tokenizer") or transformers.AutoTokenizer.from_pretrained(
         config.MODEL, trust_remote_code=True
     )
 
     if not (model := params.get("model")):
-        gc.collect()
-        torch.cuda.empty_cache()
-        model_config = transformers.AutoConfig.from_pretrained(
-            config.MODEL,
-            trust_remote_code=True,
-        )
-        if params.get("gradient_checkpointing"):
-            model_config.gradient_checkpointing = True
+        clear_mem()
         mc_param_names = [
             "model",  # custom transformers model instance
             "tokenizer",  # custom tokenizer instance
             "device",  # device if model.to(device) is needed
             "quantize_4bit",  # bool, default quantization config will be used
             "inference",  # callable, custom inference function.
             # this is different from Config.INFERENCE_FUNC,
             # because accepts model and tokenizer as arguments
             "always_clear_mem",  # gc.collect() & torch.cuda.empty_cache() before inference
             "gradient_checkpointing",  # bool, enable gradient checkpointing
             "use_pipeline",  # bool
             "pipeline_task",  # str, pipeline task name
         ]
+
         model_init_params = {
             **dict(
                 trust_remote_code=True,
                 torch_dtype="auto",
-                config=model_config,
                 device_map="auto",
                 offload_folder=config.STORAGE_PATH,
             ),
             **{k: v for k, v in params.items() if k not in mc_param_names},
         }
+        if 'config' not in model_init_params:
+            model_init_params['config'] = try_make_model_config(config)
+
         if (
             params.get("quantize_4bit")
             and "quantization_config" not in model_init_params
         ):
             model_init_params["quantization_config"] = transformers.BitsAndBytesConfig(
                 load_in_4bit=True,
                 bnb_4bit_quant_type="nf4",
                 bnb_4bit_compute_dtype=torch.bfloat16,
                 bnb_4bit_use_double_quant=True,
             )
 
         model = transformers.AutoModelForCausalLM.from_pretrained(
             config.MODEL, **model_init_params
         )
+        try:
+            model.generation_config = transformers.GenerationConfig.from_pretrained(
+                config.MODEL
+            )
+        except:  # pylint: disable=bare-except
+            logging.warning("Can't create generation config")
+
         if "device" in params:
             model.to(params["device"])
 
     transformers_model_args = {
         "max_new_tokens": 2048,
     }
     if hasattr(tokenizer, "eos_token_id") and tokenizer.eos_token_id:
@@ -107,19 +138,20 @@
 
     def wrapped_inference(prompt: dict | str, **kwargs):
         if config.CHAT_MODE:
             prompt = tokenizer.apply_chat_template(
                 prompt, add_generation_prompt=True, tokenize=False
             )
         args = {**transformers_model_args, **kwargs}
-        if always_clear_mem:
-            gc.collect()
-            torch.cuda.empty_cache()
+        always_clear_mem and clear_mem()
         if use_pipeline:
-            return pipeline_inference(prompt, pipeline, **args)
-
-        return env.inference(
-            prompt, model=env.model, tokenizer=env.tokenizer, **args
-        )
+            out = pipeline_inference(prompt, pipeline, **args)
+        else:
+            out = env.inference(
+                prompt, model=env.model, tokenizer=env.tokenizer, **args
+            )
+        if not isinstance(out, LLMResponse):
+            out = LLMResponse(out)
+        return out
 
     logging.debug(f"Local Transformers model loaded: {config.MODEL}")
     return make_local_llm_functions(config, wrapped_inference)
```

### Comparing `ai_microcore-3.6.0/microcore/logging.py` & `ai_microcore-3.6.1/microcore/logging.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     DENSE: bool = False
 
 
 def _log_request(prompt, **kwargs):
     nl = "\n" if LoggingConfig.DENSE else "\n" + LoggingConfig.INDENT
     model = _resolve_model(**kwargs)
     print(
-        f"Requesting LLM {Fore.MAGENTA}{model}{Style.RESET_ALL}:",
+        f"{Fore.RESET}Requesting LLM {Fore.MAGENTA}{model}{Style.RESET_ALL}:",
         end=" " if LoggingConfig.DENSE else "\n",
     )
     if is_chat_model(model, env().config):
         for msg in prepare_chat_messages(prompt):
             role, content = (
                 (msg["role"], msg["content"])
                 if isinstance(msg, dict)
@@ -54,15 +54,15 @@
 
 
 def _log_response(out):
     nl = "\n" if LoggingConfig.DENSE else "\n" + LoggingConfig.INDENT
     out_indented = (" " if LoggingConfig.DENSE else nl) + nl.join(
         (out or "").split("\n")
     )
-    print(f"LLM Response:{LoggingConfig.RESPONSE_COLOR}{out_indented}")
+    print(f"{Fore.RESET}LLM Response:{LoggingConfig.RESPONSE_COLOR}{out_indented}")
 
 
 def use_logging():
     """Turns on logging of LLM requests and responses to console."""
     if not is_notebook():
         init(autoreset=True)
     if _log_request not in env().llm_before_handlers:
```

### Comparing `ai_microcore-3.6.0/microcore/message_types.py` & `ai_microcore-3.6.1/microcore/message_types.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.0/microcore/templating/jinja2.py` & `ai_microcore-3.6.1/microcore/templating/jinja2.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.0/microcore/text2speech/elevenlabs.py` & `ai_microcore-3.6.1/microcore/text2speech/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.0/microcore/types.py` & `ai_microcore-3.6.1/microcore/types.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.0/microcore/ui.py` & `ai_microcore-3.6.1/microcore/ui.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.0/microcore/utils.py` & `ai_microcore-3.6.1/microcore/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,15 +252,15 @@
     regex = {int: r"[-+]?\d+", float: r"[-+]?\d*\.?\d+"}[dtype]
 
     numbers = re.findall(regex, str(text))
     if numbers:
         try:
             value = dtype(numbers[idx].strip())
             return round(value) if rounding else value
-        except ValueError:
+        except (ValueError, OverflowError):
             ...
     return return_default(default, text)
 
 
 def dedent(text: str):
     lines = text.splitlines()
     while lines and lines[0].strip() == "":
```

### Comparing `ai_microcore-3.6.0/microcore/wrappers/llm_response_wrapper.py` & `ai_microcore-3.6.1/microcore/wrappers/llm_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.0/pyproject.toml` & `ai_microcore-3.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.6.0/PKG-INFO` & `ai_microcore-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-microcore
-Version: 3.6.0
+Version: 3.6.1
 Summary: # Minimalistic Foundation for AI Applications
 Keywords: llm,large language models,ai,similarity search,ai search,gpt,openai
 Author-email: Vitalii Stepanenko <mail@vitalii.in>
 Maintainer-email: Vitalii Stepanenko <mail@vitalii.in>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ai-microcore Version: 3.6.0 Summary: # Minimalistic
+Metadata-Version: 2.1 Name: ai-microcore Version: 3.6.1 Summary: # Minimalistic
 Foundation for AI Applications Keywords: llm,large language
 models,ai,similarity search,ai search,gpt,openai Author-email: Vitalii
 Stepanenko
 vitalii.in> Maintainer-email: Vitalii Stepanenko
 vitalii.in> Requires-Python: >=3.10 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
```

