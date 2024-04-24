# Comparing `tmp/mist-medical-0.4.5a0.tar.gz` & `tmp/mist_medical-0.4.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mist-medical-0.4.5a0.tar", last modified: Fri Apr  5 18:21:25 2024, max compression
+gzip compressed data, was "mist_medical-0.4.6a0.tar", last modified: Wed Apr 24 19:44:17 2024, max compression
```

## Comparing `mist-medical-0.4.5a0.tar` & `mist_medical-0.4.6a0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.382039 mist-medical-0.4.5a0/
--rwxr-xr-x   0 runner    (1001) docker     (127)      231 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-05 18:21:25.382039 mist-medical-0.4.5a0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2554 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.374039 mist-medical-0.4.5a0/mist/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.374039 mist-medical-0.4.5a0/mist/analyze_data/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/analyze_data/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16741 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/analyze_data/analyze.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.378039 mist-medical-0.4.5a0/mist/conversion_tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/conversion_tools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3775 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/conversion_tools/csv.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5762 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/conversion_tools/msd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1313 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/convert_to_mist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.378039 mist-medical-0.4.5a0/mist/data_loading/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/data_loading/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12303 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/data_loading/dali_loader.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1552 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/eval_preds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.378039 mist-medical-0.4.5a0/mist/evaluate_preds/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/evaluate_preds/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5350 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/evaluate_preds/evaluate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.378039 mist-medical-0.4.5a0/mist/inference/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/inference/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11316 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/inference/main_inference.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3689 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.378039 mist-medical-0.4.5a0/mist/metrics/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/metrics/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22757 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/metrics/lookup_tables.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18301 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/metrics/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.378039 mist-medical-0.4.5a0/mist/models/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/models/attn_unet.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9112 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/models/get_model.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6272 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/models/layers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15447 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/models/mgnets.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16466 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/models/nnunet.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/models/swin_unetr.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8118 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/models/unet.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2488 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/post_preds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.378039 mist-medical-0.4.5a0/mist/postprocess_preds/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/postprocess_preds/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8387 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/postprocess_preds/postprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2588 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.378039 mist-medical-0.4.5a0/mist/preprocess_data/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/preprocess_data/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10643 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/preprocess_data/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.382039 mist-medical-0.4.5a0/mist/runtime/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/runtime/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8099 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/runtime/args.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7534 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/runtime/loss.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1849 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/runtime/progress_bar.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21551 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/runtime/run.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22443 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/runtime/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.382039 mist-medical-0.4.5a0/mist/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      291 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/scripts/analyze_entrypoint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      372 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/scripts/preprocess_entrypoint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      865 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/scripts/run_all_entrypoint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      863 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/mist/scripts/train_entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:21:25.382039 mist-medical-0.4.5a0/mist_medical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-05 18:21:25.000000 mist-medical-0.4.5a0/mist_medical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-05 18:21:25.000000 mist-medical-0.4.5a0/mist_medical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 18:21:25.000000 mist-medical-0.4.5a0/mist_medical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-05 18:21:25.000000 mist-medical-0.4.5a0/mist_medical.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-05 18:21:25.000000 mist-medical-0.4.5a0/mist_medical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 18:21:25.000000 mist-medical-0.4.5a0/mist_medical.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2132 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 18:21:25.382039 mist-medical-0.4.5a0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       68 2024-04-05 18:21:20.000000 mist-medical-0.4.5a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.438225 mist_medical-0.4.6a0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      231 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-24 19:44:17.438225 mist_medical-0.4.6a0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2554 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.430225 mist_medical-0.4.6a0/mist/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.430225 mist_medical-0.4.6a0/mist/analyze_data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/analyze_data/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16741 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/analyze_data/analyze.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.430225 mist_medical-0.4.6a0/mist/conversion_tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/conversion_tools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3775 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/conversion_tools/csv.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5762 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/conversion_tools/msd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1313 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/convert_to_mist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.430225 mist_medical-0.4.6a0/mist/data_loading/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/data_loading/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12303 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/data_loading/dali_loader.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1552 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/eval_preds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.430225 mist_medical-0.4.6a0/mist/evaluate_preds/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/evaluate_preds/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5350 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/evaluate_preds/evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.434224 mist_medical-0.4.6a0/mist/inference/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/inference/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11828 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/inference/main_inference.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3689 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.434224 mist_medical-0.4.6a0/mist/metrics/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/metrics/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22757 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/metrics/lookup_tables.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18301 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/metrics/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.434224 mist_medical-0.4.6a0/mist/models/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/models/attn_unet.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9112 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/models/get_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6272 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/models/layers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15447 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/models/mgnets.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16466 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/models/nnunet.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/models/swin_unetr.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8118 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/models/unet.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2488 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/post_preds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.434224 mist_medical-0.4.6a0/mist/postprocess_preds/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/postprocess_preds/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8387 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/postprocess_preds/postprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2588 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.434224 mist_medical-0.4.6a0/mist/preprocess_data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/preprocess_data/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10643 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/preprocess_data/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.434224 mist_medical-0.4.6a0/mist/runtime/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/runtime/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8099 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/runtime/args.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7534 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/runtime/loss.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1849 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/runtime/progress_bar.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21551 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/runtime/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22443 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.438225 mist_medical-0.4.6a0/mist/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      291 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/scripts/analyze_entrypoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      372 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/scripts/preprocess_entrypoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      865 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/scripts/run_all_entrypoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      863 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/scripts/train_entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.438225 mist_medical-0.4.6a0/mist_medical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-24 19:44:17.000000 mist_medical-0.4.6a0/mist_medical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-24 19:44:17.000000 mist_medical-0.4.6a0/mist_medical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:44:17.000000 mist_medical-0.4.6a0/mist_medical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-24 19:44:17.000000 mist_medical-0.4.6a0/mist_medical.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-24 19:44:17.000000 mist_medical-0.4.6a0/mist_medical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 19:44:17.000000 mist_medical-0.4.6a0/mist_medical.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2132 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:44:17.438225 mist_medical-0.4.6a0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       68 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/setup.py
```

### Comparing `mist-medical-0.4.5a0/PKG-INFO` & `mist_medical-0.4.6a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mist-medical
-Version: 0.4.5a0
+Version: 0.4.6a0
 Summary: MIST is a simple, fully automated framework for 3D medical imaging segmentation.
 Author: Rice University, The University of Texas MD Anderson Cancer Center
 Author-email: Adrian Celaya <aecelaya@rice.edu>, David Fuentes <dtfuentes@mdanderson.org>, Beatrice Riviere <riviere@rice.edu>, Evan Lim <EMLim@mdanderson.org>, Rachel Glenn <rglenn1@mdanderson.org>, Alex Balsells <atb8@rice.edu>
 License: Medical Imaging Segmentation Toolkit (MIST) (c) 2024 by Adrian Celaya
         is licenced under Attribution-NonCommercial-ShareAlike 4.0 International.
         To view a copy of this license, visit http://creativecommons.org/licenses/by-nc-sa/4.0/
 Project-URL: homepage, https://github.com/aecelaya/MIST
```

### Comparing `mist-medical-0.4.5a0/README.md` & `mist_medical-0.4.6a0/README.md`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/analyze_data/analyze.py` & `mist_medical-0.4.6a0/mist/analyze_data/analyze.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/conversion_tools/csv.py` & `mist_medical-0.4.6a0/mist/conversion_tools/csv.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/conversion_tools/msd.py` & `mist_medical-0.4.6a0/mist/conversion_tools/msd.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/convert_to_mist.py` & `mist_medical-0.4.6a0/mist/convert_to_mist.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/data_loading/dali_loader.py` & `mist_medical-0.4.6a0/mist/data_loading/dali_loader.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/eval_preds.py` & `mist_medical-0.4.6a0/mist/eval_preds.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/evaluate_preds/evaluate.py` & `mist_medical-0.4.6a0/mist/evaluate_preds/evaluate.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/inference/main_inference.py` & `mist_medical-0.4.6a0/mist/inference/main_inference.py`

 * *Files 5% similar despite different names*

```diff
@@ -211,85 +211,95 @@
         config = json.load(file)
 
     create_empty_dir(dest)
 
     # Set up rich progress bar
     testing_progress = get_progress_bar("Testing")
 
+    messages = list()
+
     # Run prediction on all samples and compute metrics
     with testing_progress as pb:
         for ii in pb.track(range(len(df))):
             patient = df.iloc[ii].to_dict()
+            try:
+                # Create individual folders for each prediction if output_std is enabled
+                if output_std:
+                    output_std_dest = os.path.join(dest, str(patient['id']))
+                    create_empty_dir(output_std_dest)
+                else:
+                    output_std_dest = dest
+
+                if "mask" in df.columns and "fold" in df.columns:
+                    image_list = list(patient.values())[3:]
+                elif "mask" in df.columns or "fold" in df.columns:
+                    image_list = list(patient.values())[2:]
+                else:
+                    image_list = list(patient.values())[1:]
+
+                og_ants_img = ants.image_read(image_list[0])
+
+                if no_preprocess:
+                    torch_img, _, fg_bbox, _ = convert_nifti_to_numpy(image_list, None)
+                else:
+                    torch_img, _, fg_bbox, _ = preprocess_example(config, image_list, None, False, None)
+
+                # Make image channels first and add batch dimension
+                torch_img = np.transpose(torch_img, axes=(3, 0, 1, 2))
+                torch_img = np.expand_dims(torch_img, axis=0)
+
+                torch_img = torch.Tensor(torch_img.copy()).to(torch.float32)
+                torch_img = torch_img.to("cuda")
+
+                prediction, std_images = predict_single_example(torch_img,
+                                                                og_ants_img,
+                                                                config,
+                                                                models,
+                                                                overlap,
+                                                                blend_mode,
+                                                                tta,
+                                                                output_std,
+                                                                fg_bbox)
+
+                # Apply postprocessing if required
+                transforms = ["remove_small_objects", "top_k_cc", "fill_holes"]
+                for transform in transforms:
+                    if len(config[transform]) > 0:
+                        for i in range(len(config[transform])):
+                            if transform == "remove_small_objects":
+                                transform_kwargs = {"small_object_threshold": config[transform][i][1]}
+                            if transform == "top_k_cc":
+                                transform_kwargs = {"morph_cleanup": config[transform][i][1],
+                                                    "morph_cleanup_iterations": config[transform][i][2],
+                                                    "top_k": config[transform][i][3]}
+                            if transform == "fill_holes":
+                                transform_kwargs = {"fill_label": config[transform][i][1]}
+
+                            prediction = apply_transform(prediction,
+                                                         transform,
+                                                         config["labels"],
+                                                         config[transform][i][0],
+                                                         transform_kwargs)
+
+                # Write prediction mask to nifti file and save to disk
+                prediction_filename = '{}.nii.gz'.format(str(patient['id']))
+                output = os.path.join(output_std_dest, prediction_filename)
+                ants.image_write(prediction, output)
+
+                # Write standard deviation image(s) to nifti file and save to disk (only for foreground labels)
+                if output_std:
+                    for i in range(len(std_images)):
+                        if config["labels"][i] > 0:
+                            std_image_filename = '{}_std_{}.nii.gz'.format(patient['id'], config['labels'][i])
+                            output = os.path.join(output_std_dest, std_image_filename)
+                            ants.image_write(std_images[i], output)
+
+            except:
+                id = patient["id"]
+                messages += f"Prediction failed for {id}\n"
+
+            if len(messages) > 0:
+                text = Text(messages)
+                console.print(text)
 
-            # Create individual folders for each prediction if output_std is enabled
-            if output_std:
-                output_std_dest = os.path.join(dest, str(patient['id']))
-                create_empty_dir(output_std_dest)
-            else:
-                output_std_dest = dest
-
-            if "mask" in df.columns and "fold" in df.columns:
-                image_list = list(patient.values())[3:]
-            elif "mask" in df.columns or "fold" in df.columns:
-                image_list = list(patient.values())[2:]
-            else:
-                image_list = list(patient.values())[1:]
-
-            og_ants_img = ants.image_read(image_list[0])
-
-            if no_preprocess:
-                torch_img, _, fg_bbox, _ = convert_nifti_to_numpy(image_list, None)
-            else:
-                torch_img, _, fg_bbox, _ = preprocess_example(config, image_list, None, False, None)
-
-            # Make image channels first and add batch dimension
-            torch_img = np.transpose(torch_img, axes=(3, 0, 1, 2))
-            torch_img = np.expand_dims(torch_img, axis=0)
-
-            torch_img = torch.Tensor(torch_img.copy()).to(torch.float32)
-            torch_img = torch_img.to("cuda")
-
-            prediction, std_images = predict_single_example(torch_img,
-                                                            og_ants_img,
-                                                            config,
-                                                            models,
-                                                            overlap,
-                                                            blend_mode,
-                                                            tta,
-                                                            output_std,
-                                                            fg_bbox)
-
-            # Apply postprocessing if required
-            transforms = ["remove_small_objects", "top_k_cc", "fill_holes"]
-            for transform in transforms:
-                if len(config[transform]) > 0:
-                    for i in range(len(config[transform])):
-                        if transform == "remove_small_objects":
-                            transform_kwargs = {"small_object_threshold": config[transform][i][1]}
-                        if transform == "top_k_cc":
-                            transform_kwargs = {"morph_cleanup": config[transform][i][1],
-                                                "morph_cleanup_iterations": config[transform][i][2],
-                                                "top_k": config[transform][i][3]}
-                        if transform == "fill_holes":
-                            transform_kwargs = {"fill_label": config[transform][i][1]}
-
-                        prediction = apply_transform(prediction,
-                                                     transform,
-                                                     config["labels"],
-                                                     config[transform][i][0],
-                                                     transform_kwargs)
-
-            # Write prediction mask to nifti file and save to disk
-            prediction_filename = '{}.nii.gz'.format(str(patient['id']))
-            output = os.path.join(output_std_dest, prediction_filename)
-            ants.image_write(prediction, output)
-
-            # Write standard deviation image(s) to nifti file and save to disk (only for foreground labels)
-            if output_std:
-                for i in range(len(std_images)):
-                    if config["labels"][i] > 0:
-                        std_image_filename = '{}_std_{}.nii.gz'.format(patient['id'], config['labels'][i])
-                        output = os.path.join(output_std_dest, std_image_filename)
-                        ants.image_write(std_images[i], output)
-
-        # Clean up
-        gc.collect()
+            # Clean up
+            gc.collect()
```

### Comparing `mist-medical-0.4.5a0/mist/main.py` & `mist_medical-0.4.6a0/mist/main.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/metrics/lookup_tables.py` & `mist_medical-0.4.6a0/mist/metrics/lookup_tables.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/metrics/metrics.py` & `mist_medical-0.4.6a0/mist/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/models/attn_unet.py` & `mist_medical-0.4.6a0/mist/models/attn_unet.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/models/get_model.py` & `mist_medical-0.4.6a0/mist/models/get_model.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/models/layers.py` & `mist_medical-0.4.6a0/mist/models/layers.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/models/mgnets.py` & `mist_medical-0.4.6a0/mist/models/mgnets.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/models/nnunet.py` & `mist_medical-0.4.6a0/mist/models/nnunet.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/models/swin_unetr.py` & `mist_medical-0.4.6a0/mist/models/swin_unetr.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/models/unet.py` & `mist_medical-0.4.6a0/mist/models/unet.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/post_preds.py` & `mist_medical-0.4.6a0/mist/post_preds.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/postprocess_preds/postprocess.py` & `mist_medical-0.4.6a0/mist/postprocess_preds/postprocess.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/predict.py` & `mist_medical-0.4.6a0/mist/predict.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/preprocess_data/preprocess.py` & `mist_medical-0.4.6a0/mist/preprocess_data/preprocess.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/runtime/args.py` & `mist_medical-0.4.6a0/mist/runtime/args.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/runtime/loss.py` & `mist_medical-0.4.6a0/mist/runtime/loss.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/runtime/progress_bar.py` & `mist_medical-0.4.6a0/mist/runtime/progress_bar.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/runtime/run.py` & `mist_medical-0.4.6a0/mist/runtime/run.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/runtime/utils.py` & `mist_medical-0.4.6a0/mist/runtime/utils.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/scripts/run_all_entrypoint.py` & `mist_medical-0.4.6a0/mist/scripts/run_all_entrypoint.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist/scripts/train_entrypoint.py` & `mist_medical-0.4.6a0/mist/scripts/train_entrypoint.py`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/mist_medical.egg-info/PKG-INFO` & `mist_medical-0.4.6a0/mist_medical.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mist-medical
-Version: 0.4.5a0
+Version: 0.4.6a0
 Summary: MIST is a simple, fully automated framework for 3D medical imaging segmentation.
 Author: Rice University, The University of Texas MD Anderson Cancer Center
 Author-email: Adrian Celaya <aecelaya@rice.edu>, David Fuentes <dtfuentes@mdanderson.org>, Beatrice Riviere <riviere@rice.edu>, Evan Lim <EMLim@mdanderson.org>, Rachel Glenn <rglenn1@mdanderson.org>, Alex Balsells <atb8@rice.edu>
 License: Medical Imaging Segmentation Toolkit (MIST) (c) 2024 by Adrian Celaya
         is licenced under Attribution-NonCommercial-ShareAlike 4.0 International.
         To view a copy of this license, visit http://creativecommons.org/licenses/by-nc-sa/4.0/
 Project-URL: homepage, https://github.com/aecelaya/MIST
```

### Comparing `mist-medical-0.4.5a0/mist_medical.egg-info/SOURCES.txt` & `mist_medical-0.4.6a0/mist_medical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mist-medical-0.4.5a0/pyproject.toml` & `mist_medical-0.4.6a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mist-medical"
-version = "0.4.5-alpha"
+version = "0.4.6-alpha"
 requires-python = ">= 3.8"
 description = "MIST is a simple, fully automated framework for 3D medical imaging segmentation."
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
     {name = "Adrian Celaya", email = "aecelaya@rice.edu"},
     {name = "David Fuentes", email = "dtfuentes@mdanderson.org"},
```

