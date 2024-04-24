# Comparing `tmp/process-twarc-0.20.0.tar.gz` & `tmp/process-twarc-0.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "process-twarc-0.20.0.tar", last modified: Sat Apr 20 13:31:27 2024, max compression
+gzip compressed data, was "process-twarc-0.20.1.tar", last modified: Wed Apr 24 18:19:32 2024, max compression
```

## Comparing `process-twarc-0.20.0.tar` & `process-twarc-0.20.1.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 13:31:27.522455 process-twarc-0.20.0/
--rw-rw-rw-   0        0        0     1077 2023-07-07 10:42:07.000000 process-twarc-0.20.0/LICENSE.txt
--rw-rw-rw-   0        0        0      694 2024-04-20 13:31:27.522455 process-twarc-0.20.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-07 10:42:22.000000 process-twarc-0.20.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 13:31:27.450188 process-twarc-0.20.0/process_twarc/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:17:48.000000 process-twarc-0.20.0/process_twarc/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 13:31:27.484193 process-twarc-0.20.0/process_twarc/build_base_model/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:17:48.000000 process-twarc-0.20.0/process_twarc/build_base_model/__init__.py
--rw-rw-rw-   0        0        0    11979 2024-03-22 11:09:06.000000 process-twarc-0.20.0/process_twarc/build_base_model/build_training_corpus.py
--rw-rw-rw-   0        0        0    11585 2024-03-19 12:52:54.000000 process-twarc-0.20.0/process_twarc/build_base_model/configure_base_model.py
--rw-rw-rw-   0        0        0     1339 2024-03-18 20:17:48.000000 process-twarc-0.20.0/process_twarc/cluster.py
-drwxrwxrwx   0        0        0        0 2024-04-20 13:31:27.494457 process-twarc-0.20.0/process_twarc/corpus_analysis/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:17:48.000000 process-twarc-0.20.0/process_twarc/corpus_analysis/__init__.py
--rw-rw-rw-   0        0        0      476 2024-03-22 11:08:59.000000 process-twarc-0.20.0/process_twarc/corpus_analysis/calculate.py
--rw-rw-rw-   0        0        0    11203 2024-04-01 17:17:24.000000 process-twarc-0.20.0/process_twarc/corpus_analysis/count.py
--rw-rw-rw-   0        0        0     9540 2024-01-28 21:02:58.000000 process-twarc-0.20.0/process_twarc/corpus_analysis/ner.py
--rw-rw-rw-   0        0        0    38302 2024-04-09 11:21:39.000000 process-twarc-0.20.0/process_twarc/corpus_analysis/plot.py
--rw-rw-rw-   0        0        0    12801 2024-03-19 15:44:50.000000 process-twarc-0.20.0/process_twarc/corpus_analysis/pos.py
--rw-rw-rw-   0        0        0    20996 2024-03-20 15:07:31.000000 process-twarc-0.20.0/process_twarc/corpus_analysis/tabulate.py
-drwxrwxrwx   0        0        0        0 2024-04-20 13:31:27.510456 process-twarc-0.20.0/process_twarc/simulate_tweet/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:17:48.000000 process-twarc-0.20.0/process_twarc/simulate_tweet/__init__.py
--rw-rw-rw-   0        0        0     2872 2024-03-18 20:17:48.000000 process-twarc-0.20.0/process_twarc/simulate_tweet/default-pfp.png
--rw-rw-rw-   0        0        0    10020 2024-03-18 20:17:48.000000 process-twarc-0.20.0/process_twarc/simulate_tweet/generate.py
-drwxrwxrwx   0        0        0        0 2024-04-20 13:31:27.521472 process-twarc-0.20.0/process_twarc/train/
--rw-rw-rw-   0        0        0     2200 2024-04-19 17:46:16.000000 process-twarc-0.20.0/process_twarc/train/MLM.py
--rw-rw-rw-   0        0        0        0 2024-03-18 20:17:48.000000 process-twarc-0.20.0/process_twarc/train/__init__.py
--rw-rw-rw-   0        0        0     1227 2024-04-19 17:44:49.000000 process-twarc-0.20.0/process_twarc/train/classifier.py
--rw-rw-rw-   0        0        0    22179 2024-04-20 13:29:57.000000 process-twarc-0.20.0/process_twarc/train/evaluate.py
--rw-rw-rw-   0        0        0    11136 2024-04-01 13:28:06.000000 process-twarc-0.20.0/process_twarc/train/preprocess.py
--rw-rw-rw-   0        0        0    29978 2024-04-20 13:26:45.000000 process-twarc-0.20.0/process_twarc/train/util.py
--rw-rw-rw-   0        0        0    12055 2024-04-01 13:27:54.000000 process-twarc-0.20.0/process_twarc/util.py
-drwxrwxrwx   0        0        0        0 2024-04-20 13:31:27.479289 process-twarc-0.20.0/process_twarc.egg-info/
--rw-rw-rw-   0        0        0      694 2024-04-20 13:31:27.000000 process-twarc-0.20.0/process_twarc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1043 2024-04-20 13:31:27.000000 process-twarc-0.20.0/process_twarc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 13:31:27.000000 process-twarc-0.20.0/process_twarc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-20 13:31:27.000000 process-twarc-0.20.0/process_twarc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-20 13:31:27.000000 process-twarc-0.20.0/process_twarc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       56 2024-04-20 13:31:27.525486 process-twarc-0.20.0/setup.cfg
--rw-rw-rw-   0        0        0     1184 2024-04-20 13:30:58.000000 process-twarc-0.20.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:19:32.055947 process-twarc-0.20.1/
+-rw-rw-rw-   0        0        0     1077 2023-07-07 10:42:07.000000 process-twarc-0.20.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      694 2024-04-24 18:19:32.055947 process-twarc-0.20.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-07 10:42:22.000000 process-twarc-0.20.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 18:19:31.948346 process-twarc-0.20.1/process_twarc/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:17:48.000000 process-twarc-0.20.1/process_twarc/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:19:32.010107 process-twarc-0.20.1/process_twarc/benchmark/
+-rw-rw-rw-   0        0        0        0 2024-04-24 18:16:21.000000 process-twarc-0.20.1/process_twarc/benchmark/__init__.py
+-rw-rw-rw-   0        0        0    11982 2024-04-24 18:16:41.000000 process-twarc-0.20.1/process_twarc/benchmark/generative_ai.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:19:32.015043 process-twarc-0.20.1/process_twarc/build_base_model/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:17:48.000000 process-twarc-0.20.1/process_twarc/build_base_model/__init__.py
+-rw-rw-rw-   0        0        0    11979 2024-03-22 11:09:06.000000 process-twarc-0.20.1/process_twarc/build_base_model/build_training_corpus.py
+-rw-rw-rw-   0        0        0    11585 2024-03-19 12:52:54.000000 process-twarc-0.20.1/process_twarc/build_base_model/configure_base_model.py
+-rw-rw-rw-   0        0        0     1339 2024-03-18 20:17:48.000000 process-twarc-0.20.1/process_twarc/cluster.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:19:32.035066 process-twarc-0.20.1/process_twarc/corpus_analysis/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:17:48.000000 process-twarc-0.20.1/process_twarc/corpus_analysis/__init__.py
+-rw-rw-rw-   0        0        0      476 2024-03-22 11:08:59.000000 process-twarc-0.20.1/process_twarc/corpus_analysis/calculate.py
+-rw-rw-rw-   0        0        0    11203 2024-04-01 17:17:24.000000 process-twarc-0.20.1/process_twarc/corpus_analysis/count.py
+-rw-rw-rw-   0        0        0     9540 2024-01-28 21:02:58.000000 process-twarc-0.20.1/process_twarc/corpus_analysis/ner.py
+-rw-rw-rw-   0        0        0    38302 2024-04-09 11:21:39.000000 process-twarc-0.20.1/process_twarc/corpus_analysis/plot.py
+-rw-rw-rw-   0        0        0    12801 2024-03-19 15:44:50.000000 process-twarc-0.20.1/process_twarc/corpus_analysis/pos.py
+-rw-rw-rw-   0        0        0    20996 2024-03-20 15:07:31.000000 process-twarc-0.20.1/process_twarc/corpus_analysis/tabulate.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:19:32.039949 process-twarc-0.20.1/process_twarc/simulate_tweet/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:17:48.000000 process-twarc-0.20.1/process_twarc/simulate_tweet/__init__.py
+-rw-rw-rw-   0        0        0     2872 2024-03-18 20:17:48.000000 process-twarc-0.20.1/process_twarc/simulate_tweet/default-pfp.png
+-rw-rw-rw-   0        0        0    10020 2024-03-18 20:17:48.000000 process-twarc-0.20.1/process_twarc/simulate_tweet/generate.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:19:32.055055 process-twarc-0.20.1/process_twarc/train/
+-rw-rw-rw-   0        0        0     2200 2024-04-20 13:32:26.000000 process-twarc-0.20.1/process_twarc/train/MLM.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 13:32:26.000000 process-twarc-0.20.1/process_twarc/train/__init__.py
+-rw-rw-rw-   0        0        0     1227 2024-04-20 13:32:26.000000 process-twarc-0.20.1/process_twarc/train/classifier.py
+-rw-rw-rw-   0        0        0    22545 2024-04-23 15:03:36.000000 process-twarc-0.20.1/process_twarc/train/evaluate.py
+-rw-rw-rw-   0        0        0    11136 2024-04-20 13:32:26.000000 process-twarc-0.20.1/process_twarc/train/preprocess.py
+-rw-rw-rw-   0        0        0    29978 2024-04-20 13:32:26.000000 process-twarc-0.20.1/process_twarc/train/util.py
+-rw-rw-rw-   0        0        0    12055 2024-04-01 13:27:54.000000 process-twarc-0.20.1/process_twarc/util.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:19:31.990029 process-twarc-0.20.1/process_twarc.egg-info/
+-rw-rw-rw-   0        0        0      694 2024-04-24 18:19:31.000000 process-twarc-0.20.1/process_twarc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1120 2024-04-24 18:19:31.000000 process-twarc-0.20.1/process_twarc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 18:19:31.000000 process-twarc-0.20.1/process_twarc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-24 18:19:31.000000 process-twarc-0.20.1/process_twarc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-24 18:19:31.000000 process-twarc-0.20.1/process_twarc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       56 2024-04-24 18:19:32.060267 process-twarc-0.20.1/setup.cfg
+-rw-rw-rw-   0        0        0     1184 2024-04-24 18:18:37.000000 process-twarc-0.20.1/setup.py
```

### Comparing `process-twarc-0.20.0/LICENSE.txt` & `process-twarc-0.20.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `process-twarc-0.20.0/PKG-INFO` & `process-twarc-0.20.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: process-twarc
-Version: 0.20.0
+Version: 0.20.1
 Summary: Tools for transforming raw data from Twarc2 to structured data for Masked Language Modeling.
 Home-page: https://github.com/user/Lone-Wolfgang
 Author: Jordan Wolfgang Klein
 Author-email: jordan.klein.21@um.edu.mt
 License: MIT
 Keywords: Twitter,Deduplication,Tokenization,Language Modeling
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `process-twarc-0.20.0/process_twarc/build_base_model/build_training_corpus.py` & `process-twarc-0.20.1/process_twarc/build_base_model/build_training_corpus.py`

 * *Files identical despite different names*

### Comparing `process-twarc-0.20.0/process_twarc/build_base_model/configure_base_model.py` & `process-twarc-0.20.1/process_twarc/build_base_model/configure_base_model.py`

 * *Files identical despite different names*

### Comparing `process-twarc-0.20.0/process_twarc/cluster.py` & `process-twarc-0.20.1/process_twarc/cluster.py`

 * *Files identical despite different names*

### Comparing `process-twarc-0.20.0/process_twarc/corpus_analysis/count.py` & `process-twarc-0.20.1/process_twarc/corpus_analysis/count.py`

 * *Files identical despite different names*

### Comparing `process-twarc-0.20.0/process_twarc/corpus_analysis/ner.py` & `process-twarc-0.20.1/process_twarc/corpus_analysis/ner.py`

 * *Files identical despite different names*

### Comparing `process-twarc-0.20.0/process_twarc/corpus_analysis/plot.py` & `process-twarc-0.20.1/process_twarc/corpus_analysis/plot.py`

 * *Files identical despite different names*

### Comparing `process-twarc-0.20.0/process_twarc/corpus_analysis/pos.py` & `process-twarc-0.20.1/process_twarc/corpus_analysis/pos.py`

 * *Files identical despite different names*

### Comparing `process-twarc-0.20.0/process_twarc/corpus_analysis/tabulate.py` & `process-twarc-0.20.1/process_twarc/corpus_analysis/tabulate.py`

 * *Files identical despite different names*

### Comparing `process-twarc-0.20.0/process_twarc/simulate_tweet/default-pfp.png` & `process-twarc-0.20.1/process_twarc/simulate_tweet/default-pfp.png`

 * *Files identical despite different names*

### Comparing `process-twarc-0.20.0/process_twarc/simulate_tweet/generate.py` & `process-twarc-0.20.1/process_twarc/simulate_tweet/generate.py`

 * *Files identical despite different names*

### Comparing `process-twarc-0.20.0/process_twarc/train/MLM.py` & `process-twarc-0.20.1/process_twarc/train/MLM.py`

 * *Files identical despite different names*

### Comparing `process-twarc-0.20.0/process_twarc/train/classifier.py` & `process-twarc-0.20.1/process_twarc/train/classifier.py`

 * *Files identical despite different names*

### Comparing `process-twarc-0.20.0/process_twarc/train/evaluate.py` & `process-twarc-0.20.1/process_twarc/train/evaluate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sqlite3
 import pandas as pd
 from pandas import ExcelWriter
 from process_twarc.util import load_dict, make_dir
 from process_twarc.train.util import load_splits, get_compute_metrics
-from transformers import AutoTokenizer, AutoModel, Trainer, pipeline
+from transformers import AutoTokenizer, AutoModelForSequenceClassification, Trainer, pipeline
 import os
 from tqdm import tqdm
 import torch
 import shutil
 import matplotlib.pyplot as plt
 import seaborn as sns
 import numpy as np
@@ -157,50 +157,52 @@
 
 def check_results(
     path_to_trial_results: dict,
     path_to_config: str,
     splits_dir: str,
     groups_to_finish: list=[],
     only_check_groups_to_finish: bool=True,
-    finished_groups: list=[]
+    finished_groups: list=[],
+    project: str=None
 ):
     
     def check_trials(
             trials = pd.read_excel(path_to_trial_results, sheet_name=None),
             config = load_dict(path_to_config)
             ):
 
-
         for group, df in trials.items():
             if group in finished_groups:
                 print(f"Skipping {group} because it is finished.")
                 continue
             if only_check_groups_to_finish and group not in groups_to_finish:
                 print(f"Skipping {group} because it is not finished..")
                 continue
             else:
                 print(f"Checking {group}.")
 
             def retrieve_parameters(group=group, config=config):
                 fixed = config["fixed_parameters"]
                 group = config["group_parameters"].get(group, {})
-                return {**fixed, **group}
+                parameters = {**fixed, **group}
+                return parameters
             
             def retrieve_splits(parameters, splits_dir=splits_dir):
                 tokenizer = AutoTokenizer.from_pretrained(parameters["path_to_model"])
                 datasets = load_splits(
                     data_dir=splits_dir,
                     splits = ["development", "test"],
                     tokenizer=tokenizer,
                     label_column=parameters["label_column"]
                 )
                 return datasets, tokenizer
             
-            def init_trainer(run_name, parameters, tokenizer):
-                trained = os.path.join(parameters["completed_dir"], parameters["project"], run_name)
+            def init_trainer(run_name, parameters, tokenizer, project=project):
+                project = project if project else parameters["project"]
+                trained = os.path.join(parameters["completed_dir"], project, run_name)
                 if not os.path.exists(trained):
                     print(f"Model {run_name} does not exist. Skipping...")
                     return None
                 # if "adapter_name" in parameters:
                 #     model = AutoModelForSequenceClassification.from_pretrained(parameters["path_to_model"])
                 #     init(model)
                 #     adapter = model.load_adapter(trained)
@@ -209,15 +211,15 @@
                 #     trainer = AdapterTrainer(
                 #         model=model,
                 #         tokenizer=tokenizer,
                 #         compute_metrics=get_compute_metrics(parameters)
                 #     ) 
                 # else:
                 trainer = Trainer(
-                    model=AutoModel.from_pretrained(trained),
+                    model=AutoModelForSequenceClassification.from_pretrained(trained),
                     tokenizer=tokenizer,
                     compute_metrics=get_compute_metrics(parameters)
                 )
                 return trainer
             
             def evaluate(run_name, parameters, datasets, tokenizer):
                 trainer = init_trainer(run_name, parameters, tokenizer)
@@ -298,20 +300,22 @@
 
 def copy_best_trials(
         path_to_trial_results: str,
         groups_to_finish: list,
         path_to_config: str,
         best_trials_dir: str,
         n_best_trials: int=10,
-        finished_groups: list=[]
+        finished_groups: list=[],
+        project = None
 ):
     parameters = load_dict(path_to_config)["fixed_parameters"]
+    project = project if project else parameters["project"]
     metric_for_best_results = parameters["metric_for_best_results"].replace("eval_", "")
 
-    completed_trials_dir = os.path.join(parameters["completed_dir"], parameters["project"])
+    completed_trials_dir = os.path.join(parameters["completed_dir"], project)
     best_results_column = f"test_{metric_for_best_results}"
 
     trials = pd.read_excel(path_to_trial_results, sheet_name=None)
     #iterate through sheets
     for name, df in trials.items():
         if name not in groups_to_finish:
             continue
@@ -394,15 +398,15 @@
                 # if "adapter_name" in parameters["fixed_parameters"]:
                 #     model = AutoModelForSequenceClassification.from_pretrained(parameters["path_to_model"])
                 #     init(model)
                 #     adapter = model.load_adapter(trained)
                 #     model.set_active_adapters(adapter)
                 #     print("Adapter model loaded.")
                 # else:
-                model = AutoModel.from_pretrained(trained)
+                model = AutoModelForSequenceClassification.from_pretrained(trained)
                 tokenizer = AutoTokenizer.from_pretrained(trained)
 
                 
                 parameters = {**parameters["fixed_parameters"], **parameters["group_parameters"].get(group, {})}
                 label_column = parameters["label_column"]
 
                 if "soft" in label_column:
@@ -451,14 +455,15 @@
 
 
 def evaluate_pipeline(
     path_to_db: str,
     results_dir: str,
     path_to_config: dict,
     splits_dir: str,
+    project: str=None,
     restart: bool=True,
     boxplot_settings: dict=None,
     evaluate_n_best_trials: int=int(),
     groups_to_finish: list=None,
     only_check_groups_to_finish: bool=True,
     copy_n_best_trials: int=10
 ):
@@ -504,15 +509,16 @@
     
     check_results(
         path_to_trial_results=path_to_results,
         path_to_config=path_to_config,
         splits_dir=splits_dir,
         groups_to_finish=groups_to_finish,
         only_check_groups_to_finish=only_check_groups_to_finish,
-        finished_groups=finished_groups
+        finished_groups=finished_groups,
+        project=project
     )
 
     if boxplot_settings:
         generate_test_results_boxplot(
             results=pd.read_excel(path_to_results, sheet_name=None),
             **boxplot_settings
         )
@@ -522,15 +528,16 @@
     if groups_to_finish and copy_n_best_trials:
         copy_best_trials(
             path_to_trial_results=path_to_results,
             groups_to_finish=groups_to_finish,
             path_to_config=path_to_config,
             best_trials_dir=best_trials_dir,
             n_best_trials=copy_n_best_trials,
-            finished_groups=finished_groups
+            finished_groups=finished_groups,
+            project=project
         )
 
     generate_test_results_CM(
         results_dir=results_dir,
         best_trials_dir=best_trials_dir,
         splits_dir=splits_dir,
         path_to_config=path_to_config
```

### Comparing `process-twarc-0.20.0/process_twarc/train/preprocess.py` & `process-twarc-0.20.1/process_twarc/train/preprocess.py`

 * *Files identical despite different names*

### Comparing `process-twarc-0.20.0/process_twarc/train/util.py` & `process-twarc-0.20.1/process_twarc/train/util.py`

 * *Files identical despite different names*

### Comparing `process-twarc-0.20.0/process_twarc/util.py` & `process-twarc-0.20.1/process_twarc/util.py`

 * *Files identical despite different names*

### Comparing `process-twarc-0.20.0/process_twarc.egg-info/PKG-INFO` & `process-twarc-0.20.1/process_twarc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: process-twarc
-Version: 0.20.0
+Version: 0.20.1
 Summary: Tools for transforming raw data from Twarc2 to structured data for Masked Language Modeling.
 Home-page: https://github.com/user/Lone-Wolfgang
 Author: Jordan Wolfgang Klein
 Author-email: jordan.klein.21@um.edu.mt
 License: MIT
 Keywords: Twitter,Deduplication,Tokenization,Language Modeling
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `process-twarc-0.20.0/process_twarc.egg-info/SOURCES.txt` & `process-twarc-0.20.1/process_twarc.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 process_twarc/cluster.py
 process_twarc/util.py
 process_twarc.egg-info/PKG-INFO
 process_twarc.egg-info/SOURCES.txt
 process_twarc.egg-info/dependency_links.txt
 process_twarc.egg-info/requires.txt
 process_twarc.egg-info/top_level.txt
+process_twarc/benchmark/__init__.py
+process_twarc/benchmark/generative_ai.py
 process_twarc/build_base_model/__init__.py
 process_twarc/build_base_model/build_training_corpus.py
 process_twarc/build_base_model/configure_base_model.py
 process_twarc/corpus_analysis/__init__.py
 process_twarc/corpus_analysis/calculate.py
 process_twarc/corpus_analysis/count.py
 process_twarc/corpus_analysis/ner.py
```

### Comparing `process-twarc-0.20.0/setup.py` & `process-twarc-0.20.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='process-twarc',
-    version='0.20.0',
+    version='0.20.1',
     license='MIT',
     description='Tools for transforming raw data from Twarc2 to structured data for Masked Language Modeling.',
     author='Jordan Wolfgang Klein',
     author_email='jordan.klein.21@um.edu.mt',
     url='https://github.com/user/Lone-Wolfgang',
     keywords=['Twitter', 'Deduplication', 'Tokenization', 'Language Modeling'],
     install_requires=[
```

