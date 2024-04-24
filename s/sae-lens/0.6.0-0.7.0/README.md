# Comparing `tmp/sae_lens-0.6.0.tar.gz` & `tmp/sae_lens-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae_lens-0.6.0.tar", max compression
+gzip compressed data, was "sae_lens-0.7.0.tar", max compression
```

## Comparing `sae_lens-0.6.0.tar` & `sae_lens-0.7.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1069 2024-04-21 14:42:33.992668 sae_lens-0.6.0/LICENSE
--rw-r--r--   0        0        0     2553 2024-04-21 14:42:33.992668 sae_lens-0.6.0/README.md
--rw-r--r--   0        0        0     1773 2024-04-21 14:42:35.020676 sae_lens-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      943 2024-04-21 14:42:35.020676 sae_lens-0.6.0/sae_lens/__init__.py
--rw-r--r--   0        0        0        0 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/analysis/__init__.py
--rw-r--r--   0        0        0    15645 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/analysis/dashboard_runner.py
--rw-r--r--   0        0        0     3535 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/analysis/feature_statistics.py
--rw-r--r--   0        0        0      992 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/analysis/neuronpedia_integration.py
--rw-r--r--   0        0        0    17944 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/analysis/neuronpedia_runner.py
--rw-r--r--   0        0        0    18275 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/analysis/tsea.py
--rw-r--r--   0        0        0     6645 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/toolkit/pretrained_saes.py
--rw-r--r--   0        0        0        0 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/__init__.py
--rw-r--r--   0        0        0      471 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/activation_functions.py
--rw-r--r--   0        0        0    16793 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/activations_store.py
--rw-r--r--   0        0        0     2849 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/cache_activations_runner.py
--rw-r--r--   0        0        0     9927 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/config.py
--rw-r--r--   0        0        0     6169 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/evals.py
--rw-r--r--   0        0        0     3747 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/geometric_median.py
--rw-r--r--   0        0        0     1528 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/lm_runner.py
--rw-r--r--   0        0        0     1020 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/load_model.py
--rw-r--r--   0        0        0     3675 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/optim.py
--rw-r--r--   0        0        0     8052 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/sae_group.py
--rw-r--r--   0        0        0     2319 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/session_loader.py
--rw-r--r--   0        0        0    15324 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/sparse_autoencoder.py
--rw-r--r--   0        0        0     3276 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/toy_model_runner.py
--rw-r--r--   0        0        0    17362 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/toy_models.py
--rw-r--r--   0        0        0    19179 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/train_sae_on_language_model.py
--rw-r--r--   0        0        0     5002 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/train_sae_on_toy_model.py
--rw-r--r--   0        0        0     1628 2024-04-21 14:42:34.004668 sae_lens-0.6.0/sae_lens/training/utils.py
--rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 sae_lens-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-24 09:17:34.150974 sae_lens-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2553 2024-04-24 09:17:34.150974 sae_lens-0.7.0/README.md
+-rw-r--r--   0        0        0     1773 2024-04-24 09:17:35.234976 sae_lens-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      943 2024-04-24 09:17:35.234976 sae_lens-0.7.0/sae_lens/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/analysis/__init__.py
+-rw-r--r--   0        0        0    15645 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/analysis/dashboard_runner.py
+-rw-r--r--   0        0        0     3535 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/analysis/feature_statistics.py
+-rw-r--r--   0        0        0     2443 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/analysis/neuronpedia_integration.py
+-rw-r--r--   0        0        0    18451 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/analysis/neuronpedia_runner.py
+-rw-r--r--   0        0        0    18275 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/analysis/tsea.py
+-rw-r--r--   0        0        0     6645 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/toolkit/pretrained_saes.py
+-rw-r--r--   0        0        0        0 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/training/__init__.py
+-rw-r--r--   0        0        0      471 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/training/activation_functions.py
+-rw-r--r--   0        0        0    16793 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/training/activations_store.py
+-rw-r--r--   0        0        0     2849 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/training/cache_activations_runner.py
+-rw-r--r--   0        0        0     9927 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/training/config.py
+-rw-r--r--   0        0        0     6169 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/training/evals.py
+-rw-r--r--   0        0        0     3747 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/training/geometric_median.py
+-rw-r--r--   0        0        0     1528 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/training/lm_runner.py
+-rw-r--r--   0        0        0     1020 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/training/load_model.py
+-rw-r--r--   0        0        0     3675 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/training/optim.py
+-rw-r--r--   0        0        0     8052 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/training/sae_group.py
+-rw-r--r--   0        0        0     2319 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/training/session_loader.py
+-rw-r--r--   0        0        0    15324 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/training/sparse_autoencoder.py
+-rw-r--r--   0        0        0     3276 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/training/toy_model_runner.py
+-rw-r--r--   0        0        0    17362 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/training/toy_models.py
+-rw-r--r--   0        0        0    19179 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/training/train_sae_on_language_model.py
+-rw-r--r--   0        0        0     5002 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/training/train_sae_on_toy_model.py
+-rw-r--r--   0        0        0     1628 2024-04-24 09:17:34.162974 sae_lens-0.7.0/sae_lens/training/utils.py
+-rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 sae_lens-0.7.0/PKG-INFO
```

### Comparing `sae_lens-0.6.0/LICENSE` & `sae_lens-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sae_lens-0.6.0/README.md` & `sae_lens-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `sae_lens-0.6.0/pyproject.toml` & `sae_lens-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sae-lens"
-version = "0.6.0"
+version = "0.7.0"
 description = "Training and Analyzing Sparse Autoencoders (SAEs)"
 authors = ["Joseph Bloom"]
 readme = "README.md"
 packages = [{include = "sae_lens"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `sae_lens-0.6.0/sae_lens/__init__.py` & `sae_lens-0.7.0/sae_lens/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.0"
+__version__ = "0.7.0"
 
 from .training.activations_store import ActivationsStore
 from .training.cache_activations_runner import cache_activations_runner
 from .training.config import CacheActivationsRunnerConfig, LanguageModelSAERunnerConfig
 from .training.evals import run_evals
 from .training.lm_runner import language_model_sae_runner
 from .training.sae_group import SparseAutoencoderDictionary
```

### Comparing `sae_lens-0.6.0/sae_lens/analysis/dashboard_runner.py` & `sae_lens-0.7.0/sae_lens/analysis/dashboard_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.6.0/sae_lens/analysis/feature_statistics.py` & `sae_lens-0.7.0/sae_lens/analysis/feature_statistics.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.6.0/sae_lens/analysis/neuronpedia_runner.py` & `sae_lens-0.7.0/sae_lens/analysis/neuronpedia_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,14 +187,15 @@
         # write dead into file so we can create them as dead in Neuronpedia
         skipped_indexes = set(range(self.n_features)) - set(self.target_feature_indexes)
         skipped_indexes_json = json.dumps(
             {
                 "model_id": self.model_id,
                 "layer": str(self.layer),
                 "sae_id": self.sae_id,
+                "log_sparsity": self.sparsity_threshold,
                 "skipped_indexes": list(skipped_indexes),
             }
         )
         with open(f"{self.outputs_dir}/skipped_indexes.json", "w") as f:
             f.write(skipped_indexes_json)
 
         tokens_file = f"{self.outputs_dir}/tokens_{self.n_batches_to_sample_from}_{self.n_prompts_to_select}.pt"
@@ -233,14 +234,21 @@
                 if feature_batch_count < self.start_batch:
                     # print(f"Skipping batch - it's after start_batch: {feature_batch_count}")
                     continue
                 if self.end_batch is not None and feature_batch_count > self.end_batch:
                     # print(f"Skipping batch - it's after end_batch: {feature_batch_count}")
                     continue
 
+                output_file = f"{self.outputs_dir}/batch-{feature_batch_count}.json"
+                # if output_file exists, skip
+                if os.path.isfile(output_file):
+                    logline = f"\n++++++++++ Skipping Batch #{feature_batch_count} output. File exists: {output_file} ++++++++++\n"
+                    print(logline)
+                    continue
+
                 print(f"========== Running Batch #{feature_batch_count} ==========")
 
                 layout = SaeVisLayoutConfig(
                     columns=[
                         Column(
                             SequencesConfig(
                                 stack_mode="stack-all",
@@ -417,13 +425,15 @@
                     "features": features_outputs,
                     "n_batches_to_sample_from": self.n_batches_to_sample_from,
                     "n_prompts_to_select": self.n_prompts_to_select,
                 }
                 json_object = json.dumps(to_write, cls=NpEncoder)
 
                 with open(
-                    f"{self.outputs_dir}/batch-{feature_batch_count}.json",
+                    output_file,
                     "w",
                 ) as f:
                     f.write(json_object)
 
+                logline = f"\n========== Completed Batch #{feature_batch_count} output: {output_file} ==========\n"
+
         return
```

### Comparing `sae_lens-0.6.0/sae_lens/analysis/tsea.py` & `sae_lens-0.7.0/sae_lens/analysis/tsea.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.6.0/sae_lens/toolkit/pretrained_saes.py` & `sae_lens-0.7.0/sae_lens/toolkit/pretrained_saes.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.6.0/sae_lens/training/activations_store.py` & `sae_lens-0.7.0/sae_lens/training/activations_store.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.6.0/sae_lens/training/cache_activations_runner.py` & `sae_lens-0.7.0/sae_lens/training/cache_activations_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.6.0/sae_lens/training/config.py` & `sae_lens-0.7.0/sae_lens/training/config.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.6.0/sae_lens/training/evals.py` & `sae_lens-0.7.0/sae_lens/training/evals.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.6.0/sae_lens/training/geometric_median.py` & `sae_lens-0.7.0/sae_lens/training/geometric_median.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.6.0/sae_lens/training/lm_runner.py` & `sae_lens-0.7.0/sae_lens/training/lm_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.6.0/sae_lens/training/load_model.py` & `sae_lens-0.7.0/sae_lens/training/load_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.6.0/sae_lens/training/optim.py` & `sae_lens-0.7.0/sae_lens/training/optim.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.6.0/sae_lens/training/sae_group.py` & `sae_lens-0.7.0/sae_lens/training/sae_group.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.6.0/sae_lens/training/session_loader.py` & `sae_lens-0.7.0/sae_lens/training/session_loader.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.6.0/sae_lens/training/sparse_autoencoder.py` & `sae_lens-0.7.0/sae_lens/training/sparse_autoencoder.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.6.0/sae_lens/training/toy_model_runner.py` & `sae_lens-0.7.0/sae_lens/training/toy_model_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.6.0/sae_lens/training/toy_models.py` & `sae_lens-0.7.0/sae_lens/training/toy_models.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.6.0/sae_lens/training/train_sae_on_language_model.py` & `sae_lens-0.7.0/sae_lens/training/train_sae_on_language_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.6.0/sae_lens/training/train_sae_on_toy_model.py` & `sae_lens-0.7.0/sae_lens/training/train_sae_on_toy_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.6.0/sae_lens/training/utils.py` & `sae_lens-0.7.0/sae_lens/training/utils.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.6.0/PKG-INFO` & `sae_lens-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sae-lens
-Version: 0.6.0
+Version: 0.7.0
 Summary: Training and Analyzing Sparse Autoencoders (SAEs)
 Author: Joseph Bloom
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

