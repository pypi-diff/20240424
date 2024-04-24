# Comparing `tmp/llm_quantkit-0.25.tar.gz` & `tmp/llm_quantkit-0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_quantkit-0.25.tar", last modified: Fri Apr 12 21:36:27 2024, max compression
+gzip compressed data, was "llm_quantkit-0.26.tar", last modified: Wed Apr 24 12:02:24 2024, max compression
```

## Comparing `llm_quantkit-0.25.tar` & `llm_quantkit-0.26.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:36:27.417880 llm_quantkit-0.25/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-12 21:36:14.000000 llm_quantkit-0.25/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-12 21:36:27.417880 llm_quantkit-0.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-12 21:36:14.000000 llm_quantkit-0.25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:36:27.417880 llm_quantkit-0.25/llm_quantkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-12 21:36:27.000000 llm_quantkit-0.25/llm_quantkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-12 21:36:27.000000 llm_quantkit-0.25/llm_quantkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:36:27.000000 llm_quantkit-0.25/llm_quantkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 21:36:27.000000 llm_quantkit-0.25/llm_quantkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-12 21:36:27.000000 llm_quantkit-0.25/llm_quantkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 21:36:27.000000 llm_quantkit-0.25/llm_quantkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-12 21:36:15.000000 llm_quantkit-0.25/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:36:27.413880 llm_quantkit-0.25/quantkit/
--rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-04-12 21:36:15.000000 llm_quantkit-0.25/quantkit/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    64290 2024-04-12 21:36:15.000000 llm_quantkit-0.25/quantkit/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    15979 2024-04-12 21:36:15.000000 llm_quantkit-0.25/quantkit/quantkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-12 21:36:15.000000 llm_quantkit-0.25/quantkit/safetensor.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 21:36:27.417880 llm_quantkit-0.25/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:02:24.656302 llm_quantkit-0.26/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-24 12:02:13.000000 llm_quantkit-0.26/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-24 12:02:24.656302 llm_quantkit-0.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-24 12:02:13.000000 llm_quantkit-0.26/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:02:24.656302 llm_quantkit-0.26/llm_quantkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-24 12:02:24.000000 llm_quantkit-0.26/llm_quantkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-24 12:02:24.000000 llm_quantkit-0.26/llm_quantkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:02:24.000000 llm_quantkit-0.26/llm_quantkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 12:02:24.000000 llm_quantkit-0.26/llm_quantkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 12:02:24.000000 llm_quantkit-0.26/llm_quantkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 12:02:24.000000 llm_quantkit-0.26/llm_quantkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-24 12:02:13.000000 llm_quantkit-0.26/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:02:24.656302 llm_quantkit-0.26/quantkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-04-24 12:02:13.000000 llm_quantkit-0.26/quantkit/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64290 2024-04-24 12:02:13.000000 llm_quantkit-0.26/quantkit/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15984 2024-04-24 12:02:13.000000 llm_quantkit-0.26/quantkit/quantkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-24 12:02:13.000000 llm_quantkit-0.26/quantkit/safetensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 12:02:24.656302 llm_quantkit-0.26/setup.cfg
```

### Comparing `llm_quantkit-0.25/LICENSE` & `llm_quantkit-0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_quantkit-0.25/PKG-INFO` & `llm_quantkit-0.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-quantkit
-Version: 0.25
+Version: 0.26
 Summary: cli tool for downloading and quantizing LLMs
 Author-email: xhedit <jevd@protonmail.com>
 License: MIT License
 Project-URL: repository, https://github.com/xhedit/quantkit
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
```

### Comparing `llm_quantkit-0.25/README.md` & `llm_quantkit-0.26/README.md`

 * *Files identical despite different names*

### Comparing `llm_quantkit-0.25/llm_quantkit.egg-info/PKG-INFO` & `llm_quantkit-0.26/llm_quantkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-quantkit
-Version: 0.25
+Version: 0.26
 Summary: cli tool for downloading and quantizing LLMs
 Author-email: xhedit <jevd@protonmail.com>
 License: MIT License
 Project-URL: repository, https://github.com/xhedit/quantkit
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
```

### Comparing `llm_quantkit-0.25/pyproject.toml` & `llm_quantkit-0.26/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llm-quantkit"
 description = "cli tool for downloading and quantizing LLMs"
 readme = "README.md"
 license = { text = "MIT License" }
-version = "0.25"
+version = "0.26"
 authors = [{ name = "xhedit", email = "jevd@protonmail.com" }]
 dependencies = [
     "click",
     "torch>=2.0.0",
     "einops",
     "tqdm",
     "transformers",
```

### Comparing `llm_quantkit-0.25/quantkit/cli.py` & `llm_quantkit-0.26/quantkit/cli.py`

 * *Files identical despite different names*

### Comparing `llm_quantkit-0.25/quantkit/convert.py` & `llm_quantkit-0.26/quantkit/convert.py`

 * *Files identical despite different names*

### Comparing `llm_quantkit-0.25/quantkit/quantkit.py` & `llm_quantkit-0.26/quantkit/quantkit.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         step_two = quant_type
         do_step_two = True
         quant_type = "F32" if f32 else "F16"
 
     # fix vocab here
 
     if output is None:
-        output = model_dir + "_" + (step_two.upper() or quant_type.upper()) + ".gguf"
+        output = str(model_dir) + "_" + (step_two.upper() or quant_type.upper()) + ".gguf"
 
     #def do_gguf_conversion(model: str, output: str, out_type: str, vocab_dir: str, vocab_type: str, context: int, pad_vocab: bool, concurrency: bool, big_endian: bool) -> None:
     if do_step_two:
         do_gguf_conversion(Path(model_dir), "tmp.gguf", quant_type.lower(), None, "spm,hfft", -1, False, False, False)
 
         if built_in_imatrix or (imatrix is None and cal_file is not None):
             imatrix = run_imatrix(cal_file, n_gpu_layers)
```

### Comparing `llm_quantkit-0.25/quantkit/safetensor.py` & `llm_quantkit-0.26/quantkit/safetensor.py`

 * *Files identical despite different names*

