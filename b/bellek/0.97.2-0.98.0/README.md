# Comparing `tmp/bellek-0.97.2.tar.gz` & `tmp/bellek-0.98.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bellek-0.97.2.tar", last modified: Sun Apr 21 20:25:09 2024, max compression
+gzip compressed data, was "bellek-0.98.0.tar", last modified: Wed Apr 24 20:00:54 2024, max compression
```

## Comparing `bellek-0.97.2.tar` & `bellek-0.98.0.tar`

### file list

```diff
@@ -1,87 +1,90 @@
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:25:09.419680 bellek-0.97.2/
--rw-rw-r--   0 bdsaglam   (501) staff       (20)    11337 2022-09-05 16:31:43.000000 bellek-0.97.2/LICENSE
--rw-rw-r--   0 bdsaglam   (501) staff       (20)      111 2022-09-05 16:31:43.000000 bellek-0.97.2/MANIFEST.in
--rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-21 20:25:09.419155 bellek-0.97.2/PKG-INFO
--rw-r--r--   0 bdsaglam   (501) staff       (20)      184 2023-04-09 15:45:53.000000 bellek-0.97.2/README.md
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:25:09.344537 bellek-0.97.2/bellek/
--rw-r--r--   0 bdsaglam   (501) staff       (20)       23 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    55079 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/_modidx.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:25:09.350132 bellek-0.97.2/bellek/hf/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/hf/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:25:09.351981 bellek-0.97.2/bellek/hf/datasets/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/hf/datasets/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1193 2024-04-21 20:24:54.000000 bellek-0.97.2/bellek/hf/datasets/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:25:09.354323 bellek-0.97.2/bellek/hf/transformers/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/hf/transformers/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    12968 2024-04-21 20:24:54.000000 bellek-0.97.2/bellek/hf/transformers/experiment.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2039 2024-04-21 20:24:54.000000 bellek-0.97.2/bellek/hf/transformers/llama2.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      790 2024-04-21 20:24:54.000000 bellek-0.97.2/bellek/hf/transformers/llama3.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2934 2024-04-21 20:24:54.000000 bellek-0.97.2/bellek/hf/transformers/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:25:09.357002 bellek-0.97.2/bellek/jerx/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/jerx/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1356 2024-04-21 20:24:54.000000 bellek-0.97.2/bellek/jerx/dataset.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3386 2024-04-21 20:24:54.000000 bellek-0.97.2/bellek/jerx/eval.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:25:09.369777 bellek-0.97.2/bellek/jerx/fewshot/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/jerx/fewshot/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     9537 2024-04-21 20:24:54.000000 bellek-0.97.2/bellek/jerx/fewshot/llm.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     4108 2024-04-21 20:24:54.000000 bellek-0.97.2/bellek/jerx/prompt.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:25:09.370632 bellek-0.97.2/bellek/jerx/reward/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/jerx/reward/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2550 2024-04-21 20:24:54.000000 bellek-0.97.2/bellek/jerx/reward/gpt.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1186 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/jerx/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:25:09.372206 bellek-0.97.2/bellek/lang/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/lang/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1575 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/lang/dataset.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2160 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/lang/qdecomp.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:25:09.373334 bellek-0.97.2/bellek/langchain/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/langchain/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      915 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/langchain/cache.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1271 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/langchain/obs.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:25:09.374555 bellek-0.97.2/bellek/llama_index/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/llama_index/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:25:09.375320 bellek-0.97.2/bellek/llama_index/data_structs/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/llama_index/data_structs/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2483 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/llama_index/data_structs/data_structs.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:25:09.376059 bellek-0.97.2/bellek/llama_index/graph_stores/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/llama_index/graph_stores/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     9059 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/llama_index/graph_stores/kuzu.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:25:09.376383 bellek-0.97.2/bellek/llama_index/indices/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/llama_index/indices/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:25:09.403635 bellek-0.97.2/bellek/llama_index/indices/knowledge_graph/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    13058 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    14785 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/llama_index/indices/knowledge_graph/retrievers.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      855 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/llama_index/llms.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1420 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/llama_index/obs.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      779 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/logging.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:25:09.416185 bellek-0.97.2/bellek/ml/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/ml/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2225 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/ml/clip.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     8515 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/ml/coop.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    28983 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/ml/data.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3293 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/ml/evaluation.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3231 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/ml/experiment.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      711 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/ml/layer.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1718 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/ml/loss.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     9174 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/ml/mcd.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      939 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/ml/vision.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:25:09.417013 bellek-0.97.2/bellek/musique/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/musique/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3081 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/musique/eval.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      539 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/testing.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:25:09.418416 bellek-0.97.2/bellek/text/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/text/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      399 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/text/utils.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     4864 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/utils.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      823 2024-04-21 20:24:55.000000 bellek-0.97.2/bellek/wandb.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-21 20:25:09.349068 bellek-0.97.2/bellek.egg-info/
--rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-21 20:25:09.000000 bellek-0.97.2/bellek.egg-info/PKG-INFO
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1748 2024-04-21 20:25:09.000000 bellek-0.97.2/bellek.egg-info/SOURCES.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2024-04-21 20:25:09.000000 bellek-0.97.2/bellek.egg-info/dependency_links.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)       34 2024-04-21 20:25:09.000000 bellek-0.97.2/bellek.egg-info/entry_points.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2023-01-13 22:27:25.000000 bellek-0.97.2/bellek.egg-info/not-zip-safe
--rw-r--r--   0 bdsaglam   (501) staff       (20)      399 2024-04-21 20:25:09.000000 bellek-0.97.2/bellek.egg-info/requires.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        7 2024-04-21 20:25:09.000000 bellek-0.97.2/bellek.egg-info/top_level.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1316 2024-04-21 20:24:37.000000 bellek-0.97.2/settings.ini
--rw-r--r--   0 bdsaglam   (501) staff       (20)       38 2024-04-21 20:25:09.419804 bellek-0.97.2/setup.cfg
--rw-rw-r--   0 bdsaglam   (501) staff       (20)     2541 2022-09-05 16:31:43.000000 bellek-0.97.2/setup.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.130186 bellek-0.98.0/
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)    11337 2022-09-05 16:31:43.000000 bellek-0.98.0/LICENSE
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)      111 2022-09-05 16:31:43.000000 bellek-0.98.0/MANIFEST.in
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-24 20:00:54.129402 bellek-0.98.0/PKG-INFO
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      184 2023-04-09 15:45:53.000000 bellek-0.98.0/README.md
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.098225 bellek-0.98.0/bellek/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       23 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    55622 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/_modidx.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.103315 bellek-0.98.0/bellek/hf/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/hf/__init__.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.104086 bellek-0.98.0/bellek/hf/datasets/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/hf/datasets/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1193 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/hf/datasets/utils.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.106665 bellek-0.98.0/bellek/hf/transformers/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/hf/transformers/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    12968 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/hf/transformers/experiment.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2039 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/hf/transformers/llama2.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      790 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/hf/transformers/llama3.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2934 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/hf/transformers/utils.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.109657 bellek-0.98.0/bellek/jerx/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/jerx/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1356 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/jerx/dataset.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3386 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/jerx/eval.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.110688 bellek-0.98.0/bellek/jerx/fewshot/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/jerx/fewshot/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     9537 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/jerx/fewshot/llm.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.112076 bellek-0.98.0/bellek/jerx/offline/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/jerx/offline/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      984 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/jerx/offline/llm.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     4108 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/jerx/prompt.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.113238 bellek-0.98.0/bellek/jerx/reward/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/jerx/reward/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2550 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/jerx/reward/gpt.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1186 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/jerx/utils.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.114724 bellek-0.98.0/bellek/lang/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/lang/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1575 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/lang/dataset.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2160 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/lang/qdecomp.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.116105 bellek-0.98.0/bellek/langchain/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/langchain/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      915 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/langchain/cache.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1271 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/langchain/obs.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.117608 bellek-0.98.0/bellek/llama_index/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/llama_index/__init__.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.118580 bellek-0.98.0/bellek/llama_index/data_structs/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/llama_index/data_structs/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2483 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/llama_index/data_structs/data_structs.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.119337 bellek-0.98.0/bellek/llama_index/graph_stores/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/llama_index/graph_stores/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     9059 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/llama_index/graph_stores/kuzu.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.119775 bellek-0.98.0/bellek/llama_index/indices/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/llama_index/indices/__init__.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.120807 bellek-0.98.0/bellek/llama_index/indices/knowledge_graph/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/llama_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    13058 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/llama_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    14785 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/llama_index/indices/knowledge_graph/retrievers.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      855 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/llama_index/llms.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1420 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/llama_index/obs.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      779 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/logging.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.126556 bellek-0.98.0/bellek/ml/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/ml/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2225 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/ml/clip.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     8515 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/ml/coop.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    28983 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/ml/data.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3293 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/ml/evaluation.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3231 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/ml/experiment.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      711 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/ml/layer.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1718 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/ml/loss.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     9174 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/ml/mcd.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      939 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/ml/vision.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.127330 bellek-0.98.0/bellek/musique/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/musique/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3081 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/musique/eval.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      539 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/testing.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.128575 bellek-0.98.0/bellek/text/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/text/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      399 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/text/utils.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     4864 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/utils.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      823 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/wandb.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.102599 bellek-0.98.0/bellek.egg-info/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-24 20:00:53.000000 bellek-0.98.0/bellek.egg-info/PKG-INFO
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1807 2024-04-24 20:00:54.000000 bellek-0.98.0/bellek.egg-info/SOURCES.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2024-04-24 20:00:53.000000 bellek-0.98.0/bellek.egg-info/dependency_links.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       34 2024-04-24 20:00:53.000000 bellek-0.98.0/bellek.egg-info/entry_points.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2023-01-13 22:27:25.000000 bellek-0.98.0/bellek.egg-info/not-zip-safe
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      399 2024-04-24 20:00:53.000000 bellek-0.98.0/bellek.egg-info/requires.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        7 2024-04-24 20:00:53.000000 bellek-0.98.0/bellek.egg-info/top_level.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1316 2024-04-24 20:00:20.000000 bellek-0.98.0/settings.ini
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       38 2024-04-24 20:00:54.130316 bellek-0.98.0/setup.cfg
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)     2541 2022-09-05 16:31:43.000000 bellek-0.98.0/setup.py
```

### Comparing `bellek-0.97.2/LICENSE` & `bellek-0.98.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/PKG-INFO` & `bellek-0.98.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bellek
-Version: 0.97.2
+Version: 0.98.0
 Summary: My digital memory
 Home-page: https://github.com/bdsaglam/bellek
 Author: Barış Deniz Sağlam
 Author-email: bdsaglam@gmail.com
 License: Apache Software License 2.0
 Keywords: notebook
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bellek-0.97.2/bellek/_modidx.py` & `bellek-0.98.0/bellek/_modidx.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,18 @@
                                   'bellek.jerx.eval.evaluate_jerx_single': ('jerx.eval.html#evaluate_jerx_single', 'bellek/jerx/eval.py'),
                                   'bellek.jerx.eval.evaluate_model_jerx': ('jerx.eval.html#evaluate_model_jerx', 'bellek/jerx/eval.py'),
                                   'bellek.jerx.eval.evaluate_pipe_jerx': ('jerx.eval.html#evaluate_pipe_jerx', 'bellek/jerx/eval.py')},
             'bellek.jerx.fewshot.llm': { 'bellek.jerx.fewshot.llm.make_kg_triplet_extract_fn': ( 'jerx.fewshot.llm.html#make_kg_triplet_extract_fn',
                                                                                                  'bellek/jerx/fewshot/llm.py'),
                                          'bellek.jerx.fewshot.llm.parse_triplet_response': ( 'jerx.fewshot.llm.html#parse_triplet_response',
                                                                                              'bellek/jerx/fewshot/llm.py')},
+            'bellek.jerx.offline.llm': { 'bellek.jerx.offline.llm.make_kg_triplet_extract_fn': ( 'jerx.offline.llm.html#make_kg_triplet_extract_fn',
+                                                                                                 'bellek/jerx/offline/llm.py'),
+                                         'bellek.jerx.offline.llm.parse_triplet_response': ( 'jerx.offline.llm.html#parse_triplet_response',
+                                                                                             'bellek/jerx/offline/llm.py')},
             'bellek.jerx.prompt': { 'bellek.jerx.prompt.JERXChatFormatter': ('jerx.prompt.html#jerxchatformatter', 'bellek/jerx/prompt.py'),
                                     'bellek.jerx.prompt.JERXChatFormatter.__post_init__': ( 'jerx.prompt.html#jerxchatformatter.__post_init__',
                                                                                             'bellek/jerx/prompt.py'),
                                     'bellek.jerx.prompt.JERXChatFormatter._format_triplets': ( 'jerx.prompt.html#jerxchatformatter._format_triplets',
                                                                                                'bellek/jerx/prompt.py'),
                                     'bellek.jerx.prompt.JERXChatFormatter.format': ( 'jerx.prompt.html#jerxchatformatter.format',
                                                                                      'bellek/jerx/prompt.py'),
```

### Comparing `bellek-0.97.2/bellek/hf/datasets/utils.py` & `bellek-0.98.0/bellek/hf/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/hf/transformers/experiment.py` & `bellek-0.98.0/bellek/hf/transformers/experiment.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/hf/transformers/llama2.py` & `bellek-0.98.0/bellek/hf/transformers/llama2.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/hf/transformers/llama3.py` & `bellek-0.98.0/bellek/hf/transformers/llama3.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/hf/transformers/utils.py` & `bellek-0.98.0/bellek/hf/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/jerx/dataset.py` & `bellek-0.98.0/bellek/jerx/dataset.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/jerx/eval.py` & `bellek-0.98.0/bellek/jerx/eval.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/jerx/fewshot/llm.py` & `bellek-0.98.0/bellek/jerx/fewshot/llm.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/jerx/prompt.py` & `bellek-0.98.0/bellek/jerx/prompt.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/jerx/reward/gpt.py` & `bellek-0.98.0/bellek/jerx/reward/gpt.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/jerx/utils.py` & `bellek-0.98.0/bellek/jerx/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/lang/dataset.py` & `bellek-0.98.0/bellek/lang/dataset.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/lang/qdecomp.py` & `bellek-0.98.0/bellek/lang/qdecomp.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/langchain/cache.py` & `bellek-0.98.0/bellek/langchain/cache.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/langchain/obs.py` & `bellek-0.98.0/bellek/langchain/obs.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/llama_index/data_structs/data_structs.py` & `bellek-0.98.0/bellek/llama_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/llama_index/graph_stores/kuzu.py` & `bellek-0.98.0/bellek/llama_index/graph_stores/kuzu.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/llama_index/indices/knowledge_graph/base.py` & `bellek-0.98.0/bellek/llama_index/indices/knowledge_graph/base.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/llama_index/indices/knowledge_graph/retrievers.py` & `bellek-0.98.0/bellek/llama_index/indices/knowledge_graph/retrievers.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/llama_index/llms.py` & `bellek-0.98.0/bellek/llama_index/llms.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/llama_index/obs.py` & `bellek-0.98.0/bellek/llama_index/obs.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/logging.py` & `bellek-0.98.0/bellek/logging.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/ml/clip.py` & `bellek-0.98.0/bellek/ml/clip.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/ml/coop.py` & `bellek-0.98.0/bellek/ml/coop.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/ml/data.py` & `bellek-0.98.0/bellek/ml/data.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/ml/evaluation.py` & `bellek-0.98.0/bellek/ml/evaluation.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/ml/experiment.py` & `bellek-0.98.0/bellek/ml/experiment.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/ml/layer.py` & `bellek-0.98.0/bellek/ml/layer.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/ml/loss.py` & `bellek-0.98.0/bellek/ml/loss.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/ml/mcd.py` & `bellek-0.98.0/bellek/ml/mcd.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/ml/vision.py` & `bellek-0.98.0/bellek/ml/vision.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/musique/eval.py` & `bellek-0.98.0/bellek/musique/eval.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/testing.py` & `bellek-0.98.0/bellek/testing.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/utils.py` & `bellek-0.98.0/bellek/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek/wandb.py` & `bellek-0.98.0/bellek/wandb.py`

 * *Files identical despite different names*

### Comparing `bellek-0.97.2/bellek.egg-info/PKG-INFO` & `bellek-0.98.0/bellek.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bellek
-Version: 0.97.2
+Version: 0.98.0
 Summary: My digital memory
 Home-page: https://github.com/bdsaglam/bellek
 Author: Barış Deniz Sağlam
 Author-email: bdsaglam@gmail.com
 License: Apache Software License 2.0
 Keywords: notebook
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bellek-0.97.2/bellek.egg-info/SOURCES.txt` & `bellek-0.98.0/bellek.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 bellek/jerx/__init__.py
 bellek/jerx/dataset.py
 bellek/jerx/eval.py
 bellek/jerx/prompt.py
 bellek/jerx/utils.py
 bellek/jerx/fewshot/__init__.py
 bellek/jerx/fewshot/llm.py
+bellek/jerx/offline/__init__.py
+bellek/jerx/offline/llm.py
 bellek/jerx/reward/__init__.py
 bellek/jerx/reward/gpt.py
 bellek/lang/__init__.py
 bellek/lang/dataset.py
 bellek/lang/qdecomp.py
 bellek/langchain/__init__.py
 bellek/langchain/cache.py
```

### Comparing `bellek-0.97.2/settings.ini` & `bellek-0.98.0/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = bellek
 lib_name = bellek
-version = 0.97.2
+version = 0.98.0
 min_python = 3.10
 license = apache2
 doc_path = _docs
 lib_path = bellek
 nbs_path = nbs
 recursive = True
 tst_flags = notest
```

### Comparing `bellek-0.97.2/setup.py` & `bellek-0.98.0/setup.py`

 * *Files identical despite different names*

