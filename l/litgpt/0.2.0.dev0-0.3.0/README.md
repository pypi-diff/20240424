# Comparing `tmp/litgpt-0.2.0.dev0.tar.gz` & `tmp/litgpt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litgpt-0.2.0.dev0.tar", last modified: Mon Mar 18 13:06:18 2024, max compression
+gzip compressed data, was "litgpt-0.3.0.tar", last modified: Wed Apr 24 15:10:15 2024, max compression
```

## Comparing `litgpt-0.2.0.dev0.tar` & `litgpt-0.3.0.tar`

### file list

```diff
@@ -1,93 +1,104 @@
-drwxrwxr-x   0 carmocca  (1000) carmocca  (1000)        0 2024-03-18 13:06:18.830122 litgpt-0.2.0.dev0/
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    11344 2023-05-04 17:51:35.000000 litgpt-0.2.0.dev0/LICENSE
--rw-r--r--   0 carmocca  (1000) carmocca  (1000)    31438 2024-03-18 13:06:18.830122 litgpt-0.2.0.dev0/PKG-INFO
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    17135 2024-03-18 12:30:01.000000 litgpt-0.2.0.dev0/README.md
-drwxrwxr-x   0 carmocca  (1000) carmocca  (1000)        0 2024-03-18 13:06:18.822122 litgpt-0.2.0.dev0/litgpt/
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     1150 2024-03-15 15:13:46.000000 litgpt-0.2.0.dev0/litgpt/__init__.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     5866 2024-03-15 17:41:11.000000 litgpt-0.2.0.dev0/litgpt/__main__.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     7197 2024-03-15 15:13:46.000000 litgpt-0.2.0.dev0/litgpt/adapter.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     9519 2024-03-15 15:13:46.000000 litgpt-0.2.0.dev0/litgpt/adapter_v2.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     2281 2024-03-15 17:35:36.000000 litgpt-0.2.0.dev0/litgpt/args.py
-drwxrwxr-x   0 carmocca  (1000) carmocca  (1000)        0 2024-03-18 13:06:18.822122 litgpt-0.2.0.dev0/litgpt/chat/
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)        0 2024-03-15 15:13:46.000000 litgpt-0.2.0.dev0/litgpt/chat/__init__.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     8381 2024-03-15 17:41:11.000000 litgpt-0.2.0.dev0/litgpt/chat/base.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    46045 2024-03-15 17:41:11.000000 litgpt-0.2.0.dev0/litgpt/config.py
-drwxrwxr-x   0 carmocca  (1000) carmocca  (1000)        0 2024-03-18 13:06:18.826122 litgpt-0.2.0.dev0/litgpt/data/
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)      960 2024-03-15 15:13:46.000000 litgpt-0.2.0.dev0/litgpt/data/__init__.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     5836 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/litgpt/data/alpaca.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     2007 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/litgpt/data/alpaca_2k.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)      950 2024-03-15 15:13:46.000000 litgpt-0.2.0.dev0/litgpt/data/alpaca_gpt4.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     5200 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/litgpt/data/base.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     4629 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/litgpt/data/deita.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     3079 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/litgpt/data/dolly.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     6921 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/litgpt/data/flan.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     6028 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/litgpt/data/json_data.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     5418 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/litgpt/data/lima.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     2784 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/litgpt/data/lit_data.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     3456 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/litgpt/data/longform.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     4475 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/litgpt/data/openwebtext.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     1963 2024-03-15 15:13:46.000000 litgpt-0.2.0.dev0/litgpt/data/prepare_slimpajama.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     2348 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/litgpt/data/prepare_starcoder.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     4003 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/litgpt/data/tinyllama.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     7305 2024-03-15 15:13:46.000000 litgpt-0.2.0.dev0/litgpt/data/tinystories.py
-drwxrwxr-x   0 carmocca  (1000) carmocca  (1000)        0 2024-03-18 13:06:18.826122 litgpt-0.2.0.dev0/litgpt/finetune/
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)        0 2024-03-15 15:13:46.000000 litgpt-0.2.0.dev0/litgpt/finetune/__init__.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    15877 2024-03-15 17:41:51.000000 litgpt-0.2.0.dev0/litgpt/finetune/adapter.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    15910 2024-03-15 17:41:44.000000 litgpt-0.2.0.dev0/litgpt/finetune/adapter_v2.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    14920 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/litgpt/finetune/full.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    17036 2024-03-15 17:41:11.000000 litgpt-0.2.0.dev0/litgpt/finetune/lora.py
-drwxrwxr-x   0 carmocca  (1000) carmocca  (1000)        0 2024-03-18 13:06:18.826122 litgpt-0.2.0.dev0/litgpt/generate/
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)        0 2024-03-15 15:13:46.000000 litgpt-0.2.0.dev0/litgpt/generate/__init__.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     5067 2024-03-15 17:41:11.000000 litgpt-0.2.0.dev0/litgpt/generate/adapter.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     5085 2024-03-15 17:41:11.000000 litgpt-0.2.0.dev0/litgpt/generate/adapter_v2.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     8393 2024-03-15 17:41:11.000000 litgpt-0.2.0.dev0/litgpt/generate/base.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     4852 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/litgpt/generate/full.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    10749 2024-03-15 15:13:46.000000 litgpt-0.2.0.dev0/litgpt/generate/sequentially.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     9885 2024-03-15 15:13:46.000000 litgpt-0.2.0.dev0/litgpt/generate/tp.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    34503 2024-03-15 15:13:46.000000 litgpt-0.2.0.dev0/litgpt/lora.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    17696 2024-03-15 17:41:11.000000 litgpt-0.2.0.dev0/litgpt/model.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    17010 2024-03-18 12:30:01.000000 litgpt-0.2.0.dev0/litgpt/pretrain.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    13863 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/litgpt/prompts.py
-drwxrwxr-x   0 carmocca  (1000) carmocca  (1000)        0 2024-03-18 13:06:18.826122 litgpt-0.2.0.dev0/litgpt/scripts/
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)        0 2024-03-15 15:13:46.000000 litgpt-0.2.0.dev0/litgpt/scripts/__init__.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    15515 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/litgpt/scripts/convert_hf_checkpoint.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    12230 2024-03-15 15:13:46.000000 litgpt-0.2.0.dev0/litgpt/scripts/convert_lit_checkpoint.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     2146 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/litgpt/scripts/convert_pretrained_checkpoint.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     5204 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/litgpt/scripts/download.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     3818 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/litgpt/scripts/merge_lora.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     4639 2024-03-15 15:13:46.000000 litgpt-0.2.0.dev0/litgpt/tokenizer.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    18535 2024-03-15 18:09:13.000000 litgpt-0.2.0.dev0/litgpt/utils.py
-drwxrwxr-x   0 carmocca  (1000) carmocca  (1000)        0 2024-03-18 13:06:18.830122 litgpt-0.2.0.dev0/litgpt.egg-info/
--rw-r--r--   0 carmocca  (1000) carmocca  (1000)    31438 2024-03-18 13:06:18.000000 litgpt-0.2.0.dev0/litgpt.egg-info/PKG-INFO
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     2023 2024-03-18 13:06:18.000000 litgpt-0.2.0.dev0/litgpt.egg-info/SOURCES.txt
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)        1 2024-03-18 13:06:18.000000 litgpt-0.2.0.dev0/litgpt.egg-info/dependency_links.txt
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)       48 2024-03-18 13:06:18.000000 litgpt-0.2.0.dev0/litgpt.egg-info/entry_points.txt
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)      329 2024-03-18 13:06:18.000000 litgpt-0.2.0.dev0/litgpt.egg-info/requires.txt
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)        7 2024-03-18 13:06:18.000000 litgpt-0.2.0.dev0/litgpt.egg-info/top_level.txt
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     1660 2024-03-18 13:06:10.000000 litgpt-0.2.0.dev0/pyproject.toml
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)       38 2024-03-18 13:06:18.830122 litgpt-0.2.0.dev0/setup.cfg
-drwxrwxr-x   0 carmocca  (1000) carmocca  (1000)        0 2024-03-18 13:06:18.830122 litgpt-0.2.0.dev0/tests/
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     9269 2024-03-15 17:41:11.000000 litgpt-0.2.0.dev0/tests/test_adapter.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    15089 2024-03-15 17:41:11.000000 litgpt-0.2.0.dev0/tests/test_adapter_v2.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     4792 2024-03-15 17:41:11.000000 litgpt-0.2.0.dev0/tests/test_chat.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)      327 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/tests/test_ci.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     1941 2024-03-15 17:41:11.000000 litgpt-0.2.0.dev0/tests/test_cli.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     3220 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/tests/test_config.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     2029 2024-03-18 12:30:01.000000 litgpt-0.2.0.dev0/tests/test_config_hub.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     5866 2024-03-15 15:13:46.000000 litgpt-0.2.0.dev0/tests/test_convert_hf_checkpoint.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    19958 2024-03-15 17:41:11.000000 litgpt-0.2.0.dev0/tests/test_convert_lit_checkpoint.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     1080 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/tests/test_convert_pretrained_checkpoint.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     2800 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/tests/test_full.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     4141 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/tests/test_generate.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     2523 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/tests/test_generate_adapter.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    12781 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/tests/test_generate_sequentially.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     5765 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/tests/test_generate_tp.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     3258 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/tests/test_lm_eval_harness.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    24969 2024-03-15 17:40:49.000000 litgpt-0.2.0.dev0/tests/test_lora.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     3702 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/tests/test_merge_lora.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    30271 2024-03-15 18:09:13.000000 litgpt-0.2.0.dev0/tests/test_model.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     4198 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/tests/test_pretrain.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     3919 2024-03-15 17:40:48.000000 litgpt-0.2.0.dev0/tests/test_prompts.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     1129 2024-03-15 15:13:46.000000 litgpt-0.2.0.dev0/tests/test_rope.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     3524 2024-03-15 15:13:46.000000 litgpt-0.2.0.dev0/tests/test_tokenizer.py
--rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    10006 2024-03-15 18:09:13.000000 litgpt-0.2.0.dev0/tests/test_utils.py
+drwxrwxr-x   0 carmocca  (1000) carmocca  (1000)        0 2024-04-24 15:10:15.323338 litgpt-0.3.0/
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    11344 2023-05-04 17:51:35.000000 litgpt-0.3.0/LICENSE
+-rw-r--r--   0 carmocca  (1000) carmocca  (1000)    38620 2024-04-24 15:10:15.323338 litgpt-0.3.0/PKG-INFO
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    23934 2024-04-24 15:06:13.000000 litgpt-0.3.0/README.md
+drwxrwxr-x   0 carmocca  (1000) carmocca  (1000)        0 2024-04-24 15:10:15.315338 litgpt-0.3.0/litgpt/
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)      848 2024-03-24 20:56:58.000000 litgpt-0.3.0/litgpt/__init__.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     6611 2024-04-23 15:29:14.000000 litgpt-0.3.0/litgpt/__main__.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     7331 2024-04-03 13:01:03.000000 litgpt-0.3.0/litgpt/adapter.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    10946 2024-04-03 13:01:03.000000 litgpt-0.3.0/litgpt/adapter_v2.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     3263 2024-04-03 17:09:32.000000 litgpt-0.3.0/litgpt/args.py
+drwxrwxr-x   0 carmocca  (1000) carmocca  (1000)        0 2024-04-24 15:10:15.319338 litgpt-0.3.0/litgpt/chat/
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)        0 2024-03-15 15:13:46.000000 litgpt-0.3.0/litgpt/chat/__init__.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     8378 2024-04-23 15:29:11.000000 litgpt-0.3.0/litgpt/chat/base.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    48791 2024-04-24 15:06:13.000000 litgpt-0.3.0/litgpt/config.py
+drwxrwxr-x   0 carmocca  (1000) carmocca  (1000)        0 2024-04-24 15:10:15.319338 litgpt-0.3.0/litgpt/data/
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     1022 2024-04-23 15:29:14.000000 litgpt-0.3.0/litgpt/data/__init__.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     5837 2024-03-24 20:56:58.000000 litgpt-0.3.0/litgpt/data/alpaca.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     2008 2024-03-24 20:56:58.000000 litgpt-0.3.0/litgpt/data/alpaca_2k.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)      950 2024-03-24 20:56:58.000000 litgpt-0.3.0/litgpt/data/alpaca_gpt4.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     5200 2024-03-24 20:56:58.000000 litgpt-0.3.0/litgpt/data/base.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     4628 2024-03-24 20:56:58.000000 litgpt-0.3.0/litgpt/data/deita.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     3079 2024-03-24 20:56:58.000000 litgpt-0.3.0/litgpt/data/dolly.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     6921 2024-03-24 20:56:58.000000 litgpt-0.3.0/litgpt/data/flan.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     6317 2024-04-04 14:20:40.000000 litgpt-0.3.0/litgpt/data/json_data.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     5417 2024-03-24 20:56:58.000000 litgpt-0.3.0/litgpt/data/lima.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     2784 2024-03-24 20:56:58.000000 litgpt-0.3.0/litgpt/data/lit_data.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     3455 2024-03-24 20:56:58.000000 litgpt-0.3.0/litgpt/data/longform.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     4475 2024-03-24 20:56:58.000000 litgpt-0.3.0/litgpt/data/openwebtext.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     1963 2024-03-24 20:56:58.000000 litgpt-0.3.0/litgpt/data/prepare_slimpajama.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     2348 2024-03-15 17:40:48.000000 litgpt-0.3.0/litgpt/data/prepare_starcoder.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     5345 2024-04-23 15:29:14.000000 litgpt-0.3.0/litgpt/data/text_files.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     4003 2024-03-24 20:56:58.000000 litgpt-0.3.0/litgpt/data/tinyllama.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     5684 2024-04-23 15:29:14.000000 litgpt-0.3.0/litgpt/data/tinystories.py
+drwxrwxr-x   0 carmocca  (1000) carmocca  (1000)        0 2024-04-24 15:10:15.319338 litgpt-0.3.0/litgpt/deploy/
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     5142 2024-04-24 15:06:14.000000 litgpt-0.3.0/litgpt/deploy/serve.py
+drwxrwxr-x   0 carmocca  (1000) carmocca  (1000)        0 2024-04-24 15:10:15.319338 litgpt-0.3.0/litgpt/eval/
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     4156 2024-04-24 15:06:14.000000 litgpt-0.3.0/litgpt/eval/evaluate.py
+drwxrwxr-x   0 carmocca  (1000) carmocca  (1000)        0 2024-04-24 15:10:15.319338 litgpt-0.3.0/litgpt/finetune/
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)        0 2024-03-15 15:13:46.000000 litgpt-0.3.0/litgpt/finetune/__init__.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    16528 2024-04-24 15:06:14.000000 litgpt-0.3.0/litgpt/finetune/adapter.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    16561 2024-04-24 15:06:14.000000 litgpt-0.3.0/litgpt/finetune/adapter_v2.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    15596 2024-04-24 15:06:14.000000 litgpt-0.3.0/litgpt/finetune/full.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    17688 2024-04-24 15:06:14.000000 litgpt-0.3.0/litgpt/finetune/lora.py
+drwxrwxr-x   0 carmocca  (1000) carmocca  (1000)        0 2024-04-24 15:10:15.319338 litgpt-0.3.0/litgpt/generate/
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)        0 2024-03-15 15:13:46.000000 litgpt-0.3.0/litgpt/generate/__init__.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     5065 2024-04-23 15:29:14.000000 litgpt-0.3.0/litgpt/generate/adapter.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     5083 2024-04-23 15:29:14.000000 litgpt-0.3.0/litgpt/generate/adapter_v2.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     8391 2024-04-23 15:29:14.000000 litgpt-0.3.0/litgpt/generate/base.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     4850 2024-04-23 15:29:14.000000 litgpt-0.3.0/litgpt/generate/full.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    10747 2024-04-23 15:29:14.000000 litgpt-0.3.0/litgpt/generate/sequentially.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     9883 2024-04-23 15:29:14.000000 litgpt-0.3.0/litgpt/generate/tp.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    34718 2024-04-23 15:29:14.000000 litgpt-0.3.0/litgpt/lora.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    18581 2024-04-03 12:56:39.000000 litgpt-0.3.0/litgpt/model.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    17301 2024-04-24 15:06:14.000000 litgpt-0.3.0/litgpt/pretrain.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    14729 2024-04-23 15:29:14.000000 litgpt-0.3.0/litgpt/prompts.py
+drwxrwxr-x   0 carmocca  (1000) carmocca  (1000)        0 2024-04-24 15:10:15.319338 litgpt-0.3.0/litgpt/scripts/
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)        0 2024-03-15 15:13:46.000000 litgpt-0.3.0/litgpt/scripts/__init__.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    15936 2024-04-23 15:29:14.000000 litgpt-0.3.0/litgpt/scripts/convert_hf_checkpoint.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    12234 2024-04-23 15:29:14.000000 litgpt-0.3.0/litgpt/scripts/convert_lit_checkpoint.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     2146 2024-03-15 17:40:48.000000 litgpt-0.3.0/litgpt/scripts/convert_pretrained_checkpoint.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     5477 2024-03-20 15:56:58.000000 litgpt-0.3.0/litgpt/scripts/download.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     3861 2024-04-23 15:29:14.000000 litgpt-0.3.0/litgpt/scripts/merge_lora.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     4611 2024-04-24 15:06:14.000000 litgpt-0.3.0/litgpt/tokenizer.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    19561 2024-04-24 15:06:14.000000 litgpt-0.3.0/litgpt/utils.py
+drwxrwxr-x   0 carmocca  (1000) carmocca  (1000)        0 2024-04-24 15:10:15.323338 litgpt-0.3.0/litgpt.egg-info/
+-rw-r--r--   0 carmocca  (1000) carmocca  (1000)    38620 2024-04-24 15:10:15.000000 litgpt-0.3.0/litgpt.egg-info/PKG-INFO
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     2243 2024-04-24 15:10:15.000000 litgpt-0.3.0/litgpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)        1 2024-04-24 15:10:15.000000 litgpt-0.3.0/litgpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)       48 2024-04-24 15:10:15.000000 litgpt-0.3.0/litgpt.egg-info/entry_points.txt
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)      581 2024-04-24 15:10:15.000000 litgpt-0.3.0/litgpt.egg-info/requires.txt
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)        7 2024-04-24 15:10:15.000000 litgpt-0.3.0/litgpt.egg-info/top_level.txt
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     2009 2024-04-24 15:09:15.000000 litgpt-0.3.0/pyproject.toml
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)       38 2024-04-24 15:10:15.323338 litgpt-0.3.0/setup.cfg
+drwxrwxr-x   0 carmocca  (1000) carmocca  (1000)        0 2024-04-24 15:10:15.323338 litgpt-0.3.0/tests/
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    10954 2024-04-24 15:06:14.000000 litgpt-0.3.0/tests/test_adapter.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    16416 2024-04-24 15:06:14.000000 litgpt-0.3.0/tests/test_adapter_v2.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     1849 2024-04-03 17:09:32.000000 litgpt-0.3.0/tests/test_args.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     5797 2024-04-23 15:29:11.000000 litgpt-0.3.0/tests/test_chat.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)      327 2024-03-15 17:40:48.000000 litgpt-0.3.0/tests/test_ci.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     2180 2024-04-23 15:29:14.000000 litgpt-0.3.0/tests/test_cli.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     2939 2024-04-23 15:29:14.000000 litgpt-0.3.0/tests/test_config.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     2348 2024-03-27 01:57:25.000000 litgpt-0.3.0/tests/test_config_hub.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     5774 2024-03-24 20:56:58.000000 litgpt-0.3.0/tests/test_convert_hf_checkpoint.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    16075 2024-04-24 15:06:14.000000 litgpt-0.3.0/tests/test_convert_lit_checkpoint.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     1076 2024-03-24 20:56:58.000000 litgpt-0.3.0/tests/test_convert_pretrained_checkpoint.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     2174 2024-04-24 15:06:14.000000 litgpt-0.3.0/tests/test_evaluate.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     2863 2024-04-24 15:06:14.000000 litgpt-0.3.0/tests/test_full.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     4083 2024-03-24 20:56:58.000000 litgpt-0.3.0/tests/test_generate.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     2523 2024-03-15 17:40:48.000000 litgpt-0.3.0/tests/test_generate_adapter.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    12558 2024-03-24 20:56:58.000000 litgpt-0.3.0/tests/test_generate_sequentially.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     5690 2024-03-24 20:56:58.000000 litgpt-0.3.0/tests/test_generate_tp.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    26364 2024-04-24 15:06:14.000000 litgpt-0.3.0/tests/test_lora.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     3924 2024-04-23 15:29:14.000000 litgpt-0.3.0/tests/test_merge_lora.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    25839 2024-04-24 15:06:14.000000 litgpt-0.3.0/tests/test_model.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     4572 2024-04-24 15:06:14.000000 litgpt-0.3.0/tests/test_pretrain.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     3830 2024-04-23 15:29:14.000000 litgpt-0.3.0/tests/test_prompts.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     1120 2024-03-24 20:56:58.000000 litgpt-0.3.0/tests/test_rope.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     1635 2024-04-23 15:29:14.000000 litgpt-0.3.0/tests/test_serve.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     2925 2024-04-04 18:11:14.000000 litgpt-0.3.0/tests/test_thunder_ddp.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    12967 2024-04-23 15:29:14.000000 litgpt-0.3.0/tests/test_thunder_fsdp.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     1987 2024-04-04 14:20:40.000000 litgpt-0.3.0/tests/test_thunder_pretrain.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     3373 2024-04-23 15:29:14.000000 litgpt-0.3.0/tests/test_tokenizer.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)     5749 2024-03-25 01:45:43.000000 litgpt-0.3.0/tests/test_unsloth_executor.py
+-rw-rw-r--   0 carmocca  (1000) carmocca  (1000)    10675 2024-04-24 15:06:14.000000 litgpt-0.3.0/tests/test_utils.py
```

### Comparing `litgpt-0.2.0.dev0/LICENSE` & `litgpt-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `litgpt-0.2.0.dev0/PKG-INFO` & `litgpt-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litgpt
-Version: 0.2.0.dev0
+Version: 0.3.0
 Summary: Hackable implementation of state-of-the-art open-source LLMs
 Author-email: Lightning AI <contact@lightning.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -206,201 +206,397 @@
            limitations under the License.
         
 Project-URL: homepage, https://github.com/lightning-AI/litgpt
 Project-URL: documentation, https://github.com/lightning-AI/litgpt/tutorials
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=2.2.0
-Requires-Dist: lightning==2.3.0.dev20240318
+Requires-Dist: lightning==2.3.0.dev20240328
 Requires-Dist: jsonargparse[signatures]>=4.27.6
+Requires-Dist: litserve>=0.1.0
 Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-rerunfailures; extra == "test"
-Requires-Dist: pytest-timeout; extra == "test"
+Requires-Dist: pytest>=8.1.1; extra == "test"
+Requires-Dist: pytest-rerunfailures>=14.0; extra == "test"
+Requires-Dist: pytest-timeout>=2.3.1; extra == "test"
 Requires-Dist: transformers>=4.38.0; extra == "test"
-Requires-Dist: einops; extra == "test"
-Requires-Dist: protobuf; extra == "test"
+Requires-Dist: einops>=0.7.0; extra == "test"
+Requires-Dist: protobuf>=4.23.4; extra == "test"
+Requires-Dist: lightning-thunder==0.2.0.dev20240404; python_version >= "3.10" and extra == "test"
 Provides-Extra: all
 Requires-Dist: bitsandbytes==0.42.0; extra == "all"
-Requires-Dist: sentencepiece; extra == "all"
-Requires-Dist: tokenizers; extra == "all"
-Requires-Dist: datasets; extra == "all"
-Requires-Dist: requests; extra == "all"
-Requires-Dist: litdata; extra == "all"
-Requires-Dist: zstandard; extra == "all"
-Requires-Dist: pandas; extra == "all"
-Requires-Dist: pyarrow; extra == "all"
-Requires-Dist: tensorboard; extra == "all"
-Requires-Dist: torchmetrics; extra == "all"
+Requires-Dist: sentencepiece>=0.2.0; extra == "all"
+Requires-Dist: tokenizers>=0.15.2; extra == "all"
+Requires-Dist: requests>=2.31.0; extra == "all"
+Requires-Dist: litdata>=0.2.2; extra == "all"
+Requires-Dist: zstandard>=0.22.0; extra == "all"
+Requires-Dist: pandas>=1.9.0; extra == "all"
+Requires-Dist: pyarrow>=15.0.2; extra == "all"
+Requires-Dist: tensorboard>=2.14.0; extra == "all"
+Requires-Dist: torchmetrics>=1.3.1; extra == "all"
+Requires-Dist: datasets>=2.18.0; extra == "all"
+Requires-Dist: transformers>=4.38.0; extra == "all"
+Requires-Dist: lm-eval>=0.4.2; extra == "all"
+Requires-Dist: safetensors>=0.4.3; extra == "all"
 Requires-Dist: huggingface_hub[hf_transfer]>=0.21.0; extra == "all"
 
 <div align="center">
-<img src="https://pl-public-data.s3.amazonaws.com/assets_lightning/LitStableLM_Badge.png" alt="LitGPT" width="128"/>
 
-# ⚡ LitGPT
-
-<!--
-<p align="center">
-  <a href="https://www.lightning.ai/">Lightning.ai</a> •
-  <a href="https://lightning.ai/docs/pytorch/stable/">PyTorch Lightning</a> •
-  <a href="https://lightning.ai/docs/fabric/stable/">Fabric</a>
-</p>
--->
-
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytorch-lightning)
-![cpu-tests](https://github.com/lightning-AI/lit-stablelm/actions/workflows/cpu-tests.yml/badge.svg) [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/lit-stablelm/blob/master/LICENSE) [![Discord](https://img.shields.io/discord/1077906959069626439?style=plastic)](https://discord.gg/VptPCZkGNa)
-
-</div>
 
-&nbsp;
-
-⚡ LitGPT is a hackable [implementation](litgpt/model.py) of state-of-the-art open-source large language models released under the **Apache 2.0 license**.
-
-&nbsp;
-## LitGPT supports
-
-✅ &nbsp;[The latest model weights](tutorials/download_model_weights.md): Gemma, Mistral, Mixtral, Phi 2, Llama 2, Falcon, CodeLlama, and [many more](tutorials/download_model_weights.md).
-
-✅ &nbsp;Optimized and efficient code: Flash Attention v2, multi-GPU support via fully-sharded data parallelism, [optional CPU offloading](tutorials/oom.md#do-sharding-across-multiple-gpus), and [TPU and XLA support](./xla).
+# ⚡ LitGPT
 
-✅ &nbsp;[Pretraining](tutorials/pretraining.md), [finetuning](tutorials/finetune.md), and [inference](tutorials/inference.md) in various precision settings: FP32, FP16, BF16, and FP16/FP32 mixed.
+**Pretrain, finetune, evaluate, and deploy 20+ LLMs on your own data**
 
-✅ &nbsp;[Configuration files](config_hub) for great out-of-the-box performance.
+Uses the latest state-of-the-art techniques:
 
-✅ &nbsp;Efficient finetuning: [LoRA](tutorials/finetune_lora.md), [QLoRA](tutorials/finetune_lora.md), [Adapter](tutorials/finetune_adapter.md), and [Adapter v2](tutorials/finetune_adapter.md).
+✅ flash attention &nbsp; &nbsp;  ✅ fp4/8/16/32 &nbsp; &nbsp;  ✅ LoRA, QLoRA, Adapter (v1, v2) &nbsp; &nbsp;  ✅ FSDP &nbsp; &nbsp;  ✅ 1-1000+ GPUs/TPUs
 
-✅ &nbsp;[Quantization](tutorials/quantize.md): 4-bit floats, 8-bit integers, and double quantization.
+---
 
-✅ &nbsp;[Exporting](https://github.com/Lightning-AI/litgpt/blob/wip/tutorials/convert_lit_models.md) to other popular model weight formats.
 
-✅ &nbsp;Many popular datasets for [pretraining](tutorials/pretrain_tinyllama.md) and [finetuning](tutorials/prepare_dataset.md), and [support for custom datasets](tutorials/prepare_dataset.md#preparing-custom-datasets-for-instruction-finetuning).
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytorch-lightning)
+![cpu-tests](https://github.com/lightning-AI/lit-stablelm/actions/workflows/cpu-tests.yml/badge.svg) [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/lit-stablelm/blob/master/LICENSE) [![Discord](https://img.shields.io/discord/1077906959069626439)](https://discord.gg/VptPCZkGNa)
 
-✅ &nbsp;Readable and easy-to-modify code to experiment with the latest research ideas.
+<p align="center">
+  <a href="https://lightning.ai/">Lightning AI</a> •
+  <a href="#choose-from-20-llms">Models</a> •
+  <a href="#quick-start">Quick start</a> •
+  <a href="#use-an-llm-for-inference">Inference</a> •
+  <a href="#finetune-an-llm">Finetune</a> •
+  <a href="#finetune-an-llm">Pretrain</a> •
+    <a href="#deploy-an-llm">Deploy</a> •
+  <a href="#state-of-the-art-features">Features</a> •
+  <a href="#training-recipes">Training recipes (YAML)</a>
+</p>
 
+</div>
 
 &nbsp;
-<br>
+<img src="https://pl-bolts-doc-images.s3.us-east-2.amazonaws.com/GithubLitGPTDAG2.png" alt="LitGPT steps" width="auto"/>
 &nbsp;
 
-## Project templates
-
-The following [Lightning Studio](https://lightning.ai/lightning-ai/studios) templates provide LitGPT tutorials and projects in reproducible environments with multi-GPU and multi-node support:
-
-
-|                                                                                                                                                                                                                                                                                                                                             |                                                                                                                                                                                                                                                                                                                                                |
-|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| <p align="left">[Prepare the TinyLlama 1T token dataset](https://lightning.ai/lightning-ai/studios/prepare-the-tinyllama-1t-token-dataset) <br> [<img src="https://pl-public-data.s3.amazonaws.com/assets_litgpt/readme/3.webp" width="300"></p>](https://lightning.ai/lightning-ai/studios/prepare-the-tinyllama-1t-token-dataset)         | [Pretrain LLMs - TinyLlama 1.1B](https://lightning.ai/lightning-ai/studios/pretrain-llms-tinyllama-1-1b) <br> <p align="left">[<img src="https://pl-public-data.s3.amazonaws.com/assets_litgpt/readme/4.webp" width="300"></p>](https://lightning.ai/lightning-ai/studios/pretrain-llms-tinyllama-1-1b)                                        |
-| [Continued Pretraining with TinyLlama 1.1B](https://lightning.ai/lightning-ai/studios/continued-pretraining-with-tinyllama-1-1b) <br> <p align="left">[<img src="https://pl-public-data.s3.amazonaws.com/assets_litgpt/readme/1.webp" width="300"></p>](https://lightning.ai/lightning-ai/studios/continued-pretraining-with-tinyllama-1-1b) | [Instruction finetuning - TinyLlama 1.1B LLM](https://lightning.ai/lightning-ai/studios/instruction-finetuning-tinyllama-1-1b-llm) <br> <p align="left">[<img src="https://pl-public-data.s3.amazonaws.com/assets_litgpt/readme/2.webp" width="300"></p>](https://lightning.ai/lightning-ai/studios/instruction-finetuning-tinyllama-1-1b-llm) |
-|                                                                                                                                                                                                                                                                                                                                             |                                                                                                                                                                                                                                                                                                                                                |
+# Finetune, pretrain and deploy LLMs Lightning fast ⚡⚡   
+LitGPT is a command-line tool designed to easily [finetune](#finetune-an-llm), [pretrain](#pretrain-an-llm), [evaluate](#use-an-llm), and [deploy](#deploy-an-llm) [20+ LLMs](#choose-from-20-llms) **on your own data**. It features highly-optimized [training recipes](#training-recipes) for the world's most powerful open-source large language models (LLMs).
 
+We reimplemented all model architectures and training recipes from scratch for 4 reasons:   
 
+1. Remove all abstraction layers and have single file implementations.   
+2. Guarantee Apache 2.0 compliance to enable enterprise use without limits.    
+3. Optimized each model's architectural detail to maximize performance, reduce costs, and speed up training.    
+4. Highly-optimized [recipe configs](#training-recipes) we have tested at enterprise scale.               
+
+---
+
+&nbsp;
+
+# Choose from 20+ LLMs
+LitGPT has 🤯 **custom, from-scratch implementations** of [20+ LLMs](tutorials/download_model_weights.md) without layers of abstraction:   
+
+| Model | Model size | Author | Reference |
+|----|----|----|----|
+| Llama 3 | 8B, 70B | Meta AI | [Meta AI 2024](https://github.com/meta-llama/llama3)                                                                     |
+| Llama 2 | 7B, 13B, 70B | Meta AI | [Touvron et al. 2023](https://arxiv.org/abs/2307.09288)                                                                      |
+| Code Llama | 7B, 13B, 34B, 70B | Meta AI | [Rozière et al. 2023](https://arxiv.org/abs/2308.12950) |
+| Mistral | 7B | Mistral AI | [Mistral website](https://mistral.ai/)                                                                                       |
+| CodeGemma | 7B | Google | [Google Team, Google Deepmind](https://ai.google.dev/gemma/docs/codegemma) |
+| ... | ... | ... | ...   |
+
+<details>
+  <summary>See full list of 20+ LLMs</summary>
+
+&nbsp; 
+
+#### All models
+  
+| Model | Model size | Author | Reference |
+|----|----|----|----|
+| CodeGemma | 7B | Google | [Google Team, Google Deepmind](https://ai.google.dev/gemma/docs/codegemma) |
+| Code Llama | 7B, 13B, 34B, 70B | Meta AI | [Rozière et al. 2023](https://arxiv.org/abs/2308.12950) |
+| Dolly | 3B, 7B, 12B | Databricks | [Conover et al. 2023](https://www.databricks.com/blog/2023/04/12/dolly-first-open-commercially-viable-instruction-tuned-llm) |
+| Falcon | 7B, 40B, 180B | TII UAE | [TII 2023](https://falconllm.tii.ae)                                                                                         |
+| FreeWilly2 (Stable Beluga 2) | 70B | Stability AI | [Stability AI 2023](https://stability.ai/blog/stable-beluga-large-instruction-fine-tuned-models)                             |
+| Function Calling Llama 2 | 7B | Trelis | [Trelis et al. 2023](https://huggingface.co/Trelis/Llama-2-7b-chat-hf-function-calling-v2)                                   |
+| Gemma | 2B, 7B | Google | [Google Team, Google Deepmind](https://storage.googleapis.com/deepmind-media/gemma/gemma-report.pdf)                         |
+| Llama 2 | 7B, 13B, 70B | Meta AI | [Touvron et al. 2023](https://arxiv.org/abs/2307.09288)                                                                      |
+| Llama 3 | 8B, 70B | Meta AI | [Meta AI 2024](https://github.com/meta-llama/llama3)                                                                     |
+| LongChat | 7B, 13B | LMSYS | [LongChat Team 2023](https://lmsys.org/blog/2023-06-29-longchat/)                                                            |
+| Mistral | 7B | Mistral AI | [Mistral website](https://mistral.ai/)                                                                                       |
+| Nous-Hermes | 7B, 13B, 70B | NousResearch | [Org page](https://huggingface.co/NousResearch)                                                                              |
+| OpenLLaMA | 3B, 7B, 13B | OpenLM Research | [Geng & Liu 2023](https://github.com/openlm-research/open_llama)                                                             |
+| Phi | 1.3B, 2.7B | Microsoft Research  | [Li et al. 2023](https://arxiv.org/abs/2309.05463)                                                                           |
+| Platypus | 7B, 13B, 70B |  Lee et al. | [Lee, Hunter, and Ruiz 2023](https://arxiv.org/abs/2308.07317)                                                               |
+| Pythia | {14,31,70,160,410}M, {1,1.4,2.8,6.9,12}B | EleutherAI | [Biderman et al. 2023](https://arxiv.org/abs/2304.01373)                                                                     |
+| RedPajama-INCITE | 3B, 7B | Together | [Together 2023](https://together.ai/blog/redpajama-models-v1)                                                                |
+| StableCode | 3B | Stability AI | [Stability AI 2023](https://stability.ai/blog/stablecode-llm-generative-ai-coding)                                           |
+| StableLM  | 3B, 7B | Stability AI | [Stability AI 2023](https://github.com/Stability-AI/StableLM)                                                                |
+| StableLM Zephyr | 3B | Stability AI | [Stability AI 2023](https://stability.ai/blog/stablecode-llm-generative-ai-coding)                                           |
+| TinyLlama | 1.1B | Zhang et al. | [Zhang et al. 2023](https://github.com/jzhang38/TinyLlama)                                                                   |
+| Vicuna | 7B, 13B, 33B | LMSYS | [Li et al. 2023](https://lmsys.org/blog/2023-03-30-vicuna/)
 
+</details>
 
-
-&nbsp;
-<br>
 &nbsp;
 
+## Install LitGPT
 
-
-## Installing LitGPT
-
-You can install LitGPT with all dependencies (including CLI, quantization, tokenizers for all models, etc.) using the following pip command:
+Install LitGPT with all dependencies (including CLI, quantization, tokenizers for all models, etc.):
 
 ```bash
-pip install 'litgpt[all] @ git+https://github.com/Lightning-AI/litgpt'
+pip install 'litgpt[all]'
 ```
 
-Alternatively, can install litgpt from a cloned GitHub repository:
+<details>
+  <summary>Advanced install options</summary>
+
+&nbsp;
+
+Install from source:
 
 ```bash
 git clone https://github.com/Lightning-AI/litgpt
 cd litgpt
 pip install -e '.[all]'
 ```
+</details>
 
+---
 
 &nbsp;
+# Quick start
+After installing LitGPT, select the model and action you want to take on that model (finetune, pretrain, evaluate, deploy, etc...):    
 
-## Using LitGPT
+```bash
+# ligpt [action] [model]
+litgpt  download  meta-llama/Meta-Llama-3-8B-Instruct
+litgpt  chat      meta-llama/Meta-Llama-3-8B-Instruct
+litgpt  finetune  meta-llama/Meta-Llama-3-8B-Instruct    
+litgpt  pretrain  meta-llama/Meta-Llama-3-8B-Instruct    
+litgpt  serve     meta-llama/Meta-Llama-3-8B-Instruct    
+```
 
+&nbsp;
 
-Below is a minimal example to get started with the LitGPT command line interface (CLI), illustrating how to download and use a model:
+###  Use an LLM for inference
+Use LLMs for inference to test its chatting capabilities, run evaluations, or extract embeddings, etc...     
+Here's an example showing how to use the Mistral 7B LLM.
+
+<a target="_blank" href="https://lightning.ai/lightning-ai/studios/litgpt-chat">
+  <img src="https://pl-bolts-doc-images.s3.us-east-2.amazonaws.com/app-2/studio-badge.svg" alt="Open In Studio"/>
+</a>
 
+&nbsp;    
 
 ```bash
 # 1) Download a pretrained model
 litgpt download --repo_id mistralai/Mistral-7B-Instruct-v0.2
 
 # 2) Chat with the model
 litgpt chat \
   --checkpoint_dir checkpoints/mistralai/Mistral-7B-Instruct-v0.2
 
 >> Prompt: What do Llamas eat?
 ```
 
 For more information, refer to the [download](tutorials/download_model_weights.md) and [inference](tutorials/inference.md) tutorials.
 
-
 &nbsp;
-## Finetuning and pretraining
 
-LitGPT supports [pretraining](tutorials/pretrain_tinyllama.md) and [finetuning](tutorials/finetune.md) to optimize models on excisting or custom datasets. Below is an example showing how to finetune a model with LoRA:
+### Finetune an LLM
+[Finetune](tutorials/finetune.md) a model to specialize it on your own custom dataset:
+
+<a target="_blank" href="https://lightning.ai/lightning-ai/studios/litgpt-finetune">
+  <img src="https://pl-bolts-doc-images.s3.us-east-2.amazonaws.com/app-2/studio-badge.svg" alt="Open In Studio"/>
+</a>
+
+&nbsp; 
 
 ```bash
 # 1) Download a pretrained model
 litgpt download --repo_id microsoft/phi-2
 
 # 2) Finetune the model
-litgpt finetune lora \
+curl -L https://huggingface.co/datasets/ksaw008/finance_alpaca/resolve/main/finance_alpaca.json -o my_custom_dataset.json
+
+litgpt finetune \
   --checkpoint_dir checkpoints/microsoft/phi-2 \
-  --data Alpaca2k \
-  --out_dir out/phi-2-lora
+  --data JSON \
+  --data.json_path my_custom_dataset.json \
+  --data.val_split_fraction 0.1 \
+  --out_dir out/custom-model
 
 # 3) Chat with the model
 litgpt chat \
-  --checkpoint_dir out/phi-2-lora/final
+  --checkpoint_dir out/custom-model/final
 ```
 
 &nbsp;
-## Configuration files for enhanced performance
 
-LitGPT also allows users to use configuration files in YAML format instead of specifying settings via the command line interface and comes with a set of model-specific defaults for good out-of-the-box performance:
+### Pretrain an LLM   
+Train an LLM from scratch on your own data via pretraining:
 
+<a target="_blank" href="https://lightning.ai/lightning-ai/studios/litgpt-pretrain">
+<img src="https://pl-bolts-doc-images.s3.us-east-2.amazonaws.com/app-2/studio-badge.svg"; alt="Open In Studio"/>
+</a>
+
+&nbsp; 
 
 ```bash
-litgpt finetune lora \
-  --config https://github.com/Lightning-AI/litgpt/blob/wip/config_hub/finetune/llama-2-7b/lora.yaml
+mkdir -p custom_texts
+curl https://www.gutenberg.org/cache/epub/24440/pg24440.txt --output custom_texts/book1.txt
+curl https://www.gutenberg.org/cache/epub/26393/pg26393.txt --output custom_texts/book2.txt
+
+# 1) Download a tokenizer
+litgpt download \
+  --repo_id EleutherAI/pythia-160m \
+  --tokenizer_only True
+
+# 2) Pretrain the model
+litgpt pretrain \
+  --model_name pythia-160m \
+  --tokenizer_dir checkpoints/EleutherAI/pythia-160m \
+  --data TextFiles \
+  --data.train_data_path "custom_texts/" \
+  --train.max_tokens 10_000_000 \
+  --out_dir out/custom-model
+
+# 3) Chat with the model
+litgpt chat \
+  --checkpoint_dir out/custom-model/final
 ```
 
-For added convenience, you can also manually override config file setting via the CLI:
+&nbsp;
+
+### Continue pretraining an LLM       
+This is another way of finetuning that specializes an already pretrained model by training on custom data:    
 
 
+<a target="_blank" href="https://lightning.ai/lightning-ai/studios/litgpt-continue-pretraining">
+<img src="https://pl-bolts-doc-images.s3.us-east-2.amazonaws.com/app-2/studio-badge.svg"; alt="Open In Studio"/>
+</a>
+
+&nbsp; 
+
 ```bash
-litgpt finetune lora \
-  --config https://raw.githubusercontent.com/Lightning-AI/litgpt/main/config_hub/finetune/llama-2-7b/lora.yaml \
-  --lora_r 4
+mkdir -p custom_texts
+curl https://www.gutenberg.org/cache/epub/24440/pg24440.txt --output custom_texts/book1.txt
+curl https://www.gutenberg.org/cache/epub/26393/pg26393.txt --output custom_texts/book2.txt
+
+# 1) Download a pretrained model
+litgpt download --repo_id EleutherAI/pythia-160m
+
+# 2) Continue pretraining the model
+litgpt pretrain \
+  --model_name pythia-160m \
+  --tokenizer_dir checkpoints/EleutherAI/pythia-160m \
+  --initial_checkpoint_dir checkpoints/EleutherAI/pythia-160m \
+  --data TextFiles \
+  --data.train_data_path "custom_texts/" \
+  --train.max_tokens 10_000_000 \
+  --out_dir out/custom-model
+
+# 3) Chat with the model
+litgpt chat \
+  --checkpoint_dir out/custom-model/final
 ```
 
-You can browse the available configuration files [here](https://github.com/Lightning-AI/litgpt/tree/main/config_hub).
+&nbsp;
+
+### Deploy an LLM
+Once you're ready to deploy a finetuned LLM, run this command:   
+
+<a target="_blank" href="https://lightning.ai/lightning-ai/studios/litgpt-serve">
+  <img src="https://pl-bolts-doc-images.s3.us-east-2.amazonaws.com/app-2/studio-badge.svg" alt="Open In Studio"/>
+</a>
 
 &nbsp;
 
-> [!TIP]
-> **Run large models on smaller consumer devices:**
-> We support 4-bit quantization (as in QLoRA), (bnb.nf4, bnb.nf4-dq, bnb.fp4, bnb.fp4-dq) and 8-bit quantization (bnb.int8) for inference by following [this guide](tutorials/quantize.md).
+```bash
+# locate the checkpoint to your finetuned or pretrained model and call the `serve` command:  
+litgpt serve --checkpoint_dir path/to/your/checkpoint/microsoft/phi-2
+
+# Alternative: if you haven't finetuned, download any checkpoint to deploy it:     
+litgpt download --repo_id microsoft/phi-2
+litgpt serve --checkpoint_dir checkpoints/microsoft/phi-2
+```
 
+Test the server in a separate terminal and integrate the model API into your AI product:    
+```python
+# 3) Use the server (in a separate session)
+import requests, json
+ response = requests.post(
+     "http://127.0.0.1:8000/predict", 
+     json={"prompt": "Fix typos in the following sentence: Exampel input"}
+)
+print(response.json()["output"])
+```
 
 &nbsp;
-<br>
+
+> [!NOTE]
+> **[Read the full docs](tutorials/0_to_litgpt.md)**.
+
+&nbsp;
+
+----
+
+# State-of-the-art features
+✅ &nbsp;State-of-the-art optimizations: Flash Attention v2, multi-GPU support via fully-sharded data parallelism, [optional CPU offloading](tutorials/oom.md#do-sharding-across-multiple-gpus), and [TPU and XLA support](extensions/xla).
+
+✅ &nbsp;[Pretrain](tutorials/pretrain.md), [finetune](tutorials/finetune.md), and [deploy](tutorials/inference.md)
+
+✅ &nbsp;Reduce compute requirements with low-precision settings: FP16, BF16, and FP16/FP32 mixed.
+
+✅ &nbsp;Lower memory requirements with [quantization](tutorials/quantize.md): 4-bit floats, 8-bit integers, and double quantization.
+
+✅ &nbsp;[Configuration files](config_hub) for great out-of-the-box performance.
+
+✅ &nbsp;Parameter-efficient finetuning: [LoRA](tutorials/finetune_lora.md), [QLoRA](tutorials/finetune_lora.md), [Adapter](tutorials/finetune_adapter.md), and [Adapter v2](tutorials/finetune_adapter.md).
+
+✅ &nbsp;[Exporting](tutorials/convert_lit_models.md) to other popular model weight formats.
+
+✅ &nbsp;Many popular datasets for [pretraining](tutorials/pretrain.md) and [finetuning](tutorials/prepare_dataset.md), and [support for custom datasets](tutorials/prepare_dataset.md#preparing-custom-datasets-for-instruction-finetuning).
+
+✅ &nbsp;Readable and easy-to-modify code to experiment with the latest research ideas.
+
 &nbsp;
 
-## Customization
+---
+
+# Training recipes
 
-LitGPT supports rich and customizable [config files](config_hub) to tailor the LLM training to your dataset and hardware needs. Shown below is a configuration file for LoRA finetuning:
+LitGPT comes with validated recipes (YAML configs) to train models under different conditions.  We've generated these recipes based on the parameters we found to perform the best for different training conditions.
+
+Browse all training recipes [here](config_hub).
+
+### Example
+
+```bash
+litgpt finetune \
+  --config https://raw.githubusercontent.com/Lightning-AI/litgpt/main/config_hub/finetune/llama-2-7b/lora.yaml
+```
+
+### What is a config
+Configs let you customize training for all granular parameters like:
+
+```yaml
+# The path to the base model's checkpoint directory to load for finetuning. (type: <class 'Path'>, default: checkpoints/stabilityai/stablelm-base-alpha-3b)
+checkpoint_dir: checkpoints/meta-llama/Llama-2-7b-hf
+
+# Directory in which to save checkpoints and logs. (type: <class 'Path'>, default: out/lora)
+out_dir: out/finetune/qlora-llama2-7b
+
+# The precision to use for finetuning. Possible choices: "bf16-true", "bf16-mixed", "32-true". (type: Optional[str], default: null)
+precision: bf16-true
+
+...
+```
+
+<details>
+  <summary>Example: LoRA finetuning config</summary>
+
+&nbsp;
 
 ```yaml
 # The path to the base model's checkpoint directory to load for finetuning. (type: <class 'Path'>, default: checkpoints/stabilityai/stablelm-base-alpha-3b)
 checkpoint_dir: checkpoints/meta-llama/Llama-2-7b-hf
 
 # Directory in which to save checkpoints and logs. (type: <class 'Path'>, default: out/lora)
 out_dir: out/finetune/qlora-llama2-7b
@@ -518,33 +714,29 @@
 
 # The name of the logger to send metrics to. (type: Literal['wandb', 'tensorboard', 'csv'], default: csv)
 logger_name: csv
 
 # The random seed to use for reproducibility. (type: int, default: 1337)
 seed: 1337
 ```
+</details>
 
+### Override config params via CLI
+Override any parameter in the CLI:
 
-&nbsp;
-
-## LitGPT design principles
-
-This repository follows the main principle of **openness through clarity**.
-
-**LitGPT** is:
-
-- **Simple:** Single-file implementation without boilerplate.
-- **Correct:** Numerically equivalent to the original model.
-- **Optimized:** Runs fast on consumer hardware or at scale.
-- **Open-source:** No strings attached.
-
-Avoiding code duplication is **not** a goal. **Readability** and **hackability** are.
+```bash
+litgpt finetune \
+  --config https://raw.githubusercontent.com/Lightning-AI/litgpt/main/config_hub/finetune/llama-2-7b/lora.yaml \
+  --lora_r 4
+```
 
 &nbsp;
 
+# Community        
+
 ## Get involved!
 
 We appreciate your feedback and contributions. If you have feature requests, questions, or want to contribute code or config files, please don't hesitate to use the [GitHub Issue](https://github.com/Lightning-AI/litgpt/issues) tracker.
 
 We welcome all individual contributors, regardless of their level of experience or hardware. Your contributions are valuable, and we are excited to see what you can accomplish in this collaborative and supportive environment.
 
 &nbsp;
@@ -555,35 +747,37 @@
 If you have general questions about building with LitGPT, please [join our Discord](https://discord.gg/VptPCZkGNa).
 
 
 &nbsp;
 
 ## Tutorials, how-to guides, and docs
 
+
+> [!NOTE]
+> We recommend starting with the **[Zero to LitGPT: Getting Started with Pretraining, Finetuning, and Using LLMs](tutorials/0_to_litgpt.md)** if you are looking to get started with using LitGPT.
+
+Tutorials and in-depth feature documentation can be found below:
+
 -  Finetuning, incl. LoRA, QLoRA, and Adapters ([tutorials/finetune.md](tutorials/finetune.md))
--  Pretraining ([tutorials/pretrain_tinyllama.md](tutorials/pretrain_tinyllama.md))
+-  Pretraining ([tutorials/pretrain.md](tutorials/pretrain.md))
 -  Model evaluation ([tutorials/evaluation.md](tutorials/evaluation.md))
 -  Supported and custom datasets ([tutorials/prepare_dataset.md](tutorials/prepare_dataset.md))
 -  Quantization ([tutorials/quantize.md](tutorials/quantize.md))
 -  Tips for dealing with out-of-memory (OOM) errors ([tutorials/oom.md](tutorials/oom.md))
 
-
-
-
-
 &nbsp;
 
 ## XLA
 
-Lightning AI has partnered with Google to add first-class support for [Cloud TPUs](https://cloud.google.com/tpu) in [Lightning’s frameworks](https://github.com/Lightning-AI/lightning) and LitGPT,
+Lightning AI has partnered with Google to add first-class support for [Cloud TPUs](https://cloud.google.com/tpu) in [Lightning's frameworks](https://github.com/Lightning-AI/lightning) and LitGPT,
 helping democratize AI for millions of developers and researchers worldwide.
 
 Using TPUs with Lightning is as straightforward as changing one line of code.
 
-We provide scripts fully optimized for TPUs in the [XLA directory](xla).
+We provide scripts fully optimized for TPUs in the [XLA directory](extensions/xla).
 
 
 
 &nbsp;
 
 ## Acknowledgements
 
@@ -597,28 +791,39 @@
 
 
 &nbsp;
 
 
 ## Community showcase
 
-Check out the projects below using and building on LitGPT. If you have a project you'd like to add to this section, please don't hestiate to open a pull request.
+Check out the projects below that use and build on LitGPT. If you have a project you'd like to add to this section, please don't hesitate to open a pull request.
 
 &nbsp;
 
 **🏆 NeurIPS 2023 Large Language Model Efficiency Challenge: 1 LLM + 1 GPU + 1 Day**
 
 The LitGPT repository was the official starter kit for the [NeurIPS 2023 LLM Efficiency Challenge](https://llm-efficiency-challenge.github.io), which is a competition focused on finetuning an existing non-instruction tuned LLM for 24 hours on a single GPU.
 
 &nbsp;
 
 **🦙 TinyLlama: An Open-Source Small Language Model**
 
 LitGPT powered the [TinyLlama project](https://github.com/jzhang38/TinyLlama) and [TinyLlama: An Open-Source Small Language Model](https://arxiv.org/abs/2401.02385) research paper.
 
+&nbsp;
+
+**🍪 MicroLlama: MicroLlama-300M**
+
+[MicroLlama](https://github.com/keeeeenw/MicroLlama) is a 300M Llama model pretrained on 50B tokens powered by TinyLlama and LitGPT.
+
+&nbsp;
+
+**🔬 Pre-training Small Base LMs with Fewer Tokens**
+
+The research paper ["Pre-training Small Base LMs with Fewer Tokens"](https://arxiv.org/abs/2404.08634), which utilizes LitGPT, develops smaller base language models by inheriting a few transformer blocks from larger models and training on a tiny fraction of the data used by the larger models. It demonstrates that these smaller models can perform comparably to larger models despite using significantly less training data and resources.
 
 &nbsp;
 
 ## Citation
 
 If you use LitGPT in your research, please cite the following work:
 
@@ -632,8 +837,7 @@
 ```
 
 &nbsp;
 
 ## License
 
 LitGPT is released under the [Apache 2.0](https://github.com/Lightning-AI/litgpt/blob/main/LICENSE) license.
-
```

### Comparing `litgpt-0.2.0.dev0/litgpt/__main__.py` & `litgpt-0.3.0/litgpt/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
+import sys
 
 from typing import TYPE_CHECKING, Any
 
 import torch
 
 from litgpt.chat.base import main as chat_fn
 from litgpt.finetune.adapter import setup as finetune_adapter_fn
@@ -19,14 +20,17 @@
 from litgpt.scripts.convert_hf_checkpoint import convert_hf_checkpoint as convert_hf_checkpoint_fn
 from litgpt.scripts.convert_lit_checkpoint import convert_lit_checkpoint as convert_lit_checkpoint_fn
 from litgpt.scripts.convert_pretrained_checkpoint import (
     convert_pretrained_checkpoint as convert_pretrained_checkpoint_fn,
 )
 from litgpt.scripts.download import download_from_hub as download_fn
 from litgpt.scripts.merge_lora import merge_lora as merge_lora_fn
+from litgpt.eval.evaluate import convert_and_evaluate as evaluate_fn
+from litgpt.deploy.serve import run_server as serve_fn
+
 
 if TYPE_CHECKING:
     from jsonargparse import ArgumentParser
 
 
 def _new_parser(**kwargs: Any) -> "ArgumentParser":
     from jsonargparse import ActionConfigFile, ArgumentParser
@@ -34,14 +38,20 @@
     parser = ArgumentParser(**kwargs)
     parser.add_argument(
         "-c", "--config", action=ActionConfigFile, help="Path to a configuration file in json or yaml format."
     )
     return parser
 
 
+def _rewrite_argv_for_default_subcommand(parser_data: dict, command: str, subcommand: str) -> None:
+    """Rewrites the `sys.argv` such that `litgpt command` defaults to `litgpt command subcommand`."""
+    if len(sys.argv) > 2 and sys.argv[1] == command and sys.argv[2] not in parser_data[command].keys():
+        sys.argv.insert(2, subcommand)
+
+
 def main() -> None:
     parser_data = {
         "download": {"help": "Download weights or tokenizer data from the Hugging Face Hub.", "fn": download_fn},
         "chat": {"help": "Chat with a model.", "fn": chat_fn},
         "finetune": {
             "help": "Finetune a model with one of our existing methods.",
             "lora": {"help": "Finetune a model with LoRA.", "fn": finetune_lora_fn},
@@ -74,21 +84,25 @@
             "from_litgpt": {"fn": convert_lit_checkpoint_fn, "help": "Convert LitGPT weights to Hugging Face weights."},
             "pretrained_checkpoint": {
                 "fn": convert_pretrained_checkpoint_fn,
                 "help": "Convert a checkpoint after pretraining.",
             },
         },
         "merge_lora": {"help": "Merges the LoRA weights with the base model.", "fn": merge_lora_fn},
+        "evaluate": {"help": "Evaluate a model with the LM Evaluation Harness.", "fn": evaluate_fn},
+        "serve": {"help": "Serve and deploy a model with LitServe.", "fn": serve_fn},
     }
 
     from jsonargparse import set_config_read_mode, set_docstring_parse_options
 
     set_docstring_parse_options(attribute_docstrings=True)
     set_config_read_mode(urls_enabled=True)
 
+    _rewrite_argv_for_default_subcommand(parser_data, "finetune", "lora")
+
     root_parser = _new_parser(prog="litgpt")
 
     # register level 1 subcommands and level 2 subsubcommands. If there are more levels in the future we would want to
     # refactor this to do BFS traversal for registration
     subcommands = root_parser.add_subcommands()
     subcommand_to_parser = {}
     for k, v in parser_data.items():
```

### Comparing `litgpt-0.2.0.dev0/litgpt/adapter.py` & `litgpt-0.3.0/litgpt/adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,14 +62,16 @@
             mask = self.mask_cache.index_select(2, input_pos)
         else:
             cos = self.cos[:T]
             sin = self.sin[:T]
             mask = None
 
         x = self.transformer.wte(idx)  # token embeddings of shape (b, t, n_embd)
+        if self.config.scale_embeddings:
+            x = x * (self.config.n_embd**0.5)
         for block in self.transformer.h:
             x = block(x, cos, sin, mask, input_pos)
         x = self.transformer.ln_f(x)
         if lm_head_chunk_size > 0:
             # chunk the lm head logits to reduce the peak memory used by autograd
             return [self.lm_head(x_i) for x_i in x.split(lm_head_chunk_size, dim=1)]
         return self.lm_head(x)  # (b, t, vocab_size)
@@ -145,15 +147,16 @@
 
         T = q.size(2)
         amask = torch.ones(T, aT, dtype=torch.bool, device=q.device)
         ay = super().scaled_dot_product_attention(q, ak, av, amask)
         return y + self.gating_factor * ay
 
     def reset_parameters(self) -> None:
-        torch.nn.init.zeros_(self.gating_factor)
+        if hasattr(self, "gating_factor"):
+            torch.nn.init.zeros_(self.gating_factor)
 
     def _load_from_state_dict(self, state_dict: Dict, prefix: str, *args: Any, **kwargs: Any) -> None:
         """For compatibility with older checkpoints."""
         if (key := prefix + "gating_factor") in state_dict and state_dict[key].size(1) == self.config.n_head:
             state_dict[key] = state_dict[key].permute(0, 2, 1, 3)
         super()._load_from_state_dict(state_dict, prefix, *args, **kwargs)
```

### Comparing `litgpt-0.2.0.dev0/litgpt/adapter_v2.py` & `litgpt-0.3.0/litgpt/adapter_v2.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 LLaMA-Adapter V2: Parameter-Efficient Visual Instruction Model
 https://arxiv.org/abs/2304.15010
 
 Port for LitGPT
 """
 
 from dataclasses import dataclass
-from typing import Any, Dict, Optional, Tuple, Type
+from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 import torch
 import torch.nn as nn
 from typing_extensions import Self
 
 import litgpt
 from litgpt.adapter import GPT as BaseModel
@@ -76,14 +76,43 @@
                 h=nn.ModuleList(Block(config, i) for i in range(config.n_layer)),
                 ln_f=config.norm_class(config.n_embd, eps=config.norm_eps),
             )
         )
         self.max_seq_length = self.config.block_size
         self.mask_cache: Optional[torch.Tensor] = None
 
+    def forward(
+        self, idx: torch.Tensor, input_pos: Optional[torch.Tensor] = None, lm_head_chunk_size: int = 0
+    ) -> Union[torch.Tensor, List[torch.Tensor]]:
+        T = idx.size(1)
+        if self.max_seq_length < T:
+            raise ValueError(f"Cannot forward sequence of length {T}, max seq length is only {self.max_seq_length}.")
+
+        if input_pos is not None:  # use the kv cache
+            cos = self.cos.index_select(0, input_pos)
+            sin = self.sin.index_select(0, input_pos)
+            if self.mask_cache is None:
+                raise TypeError("You need to call `gpt.set_kv_cache()`")
+            mask = self.mask_cache.index_select(2, input_pos)
+        else:
+            cos = self.cos[:T]
+            sin = self.sin[:T]
+            mask = None
+
+        x = self.transformer.wte(idx)  # token embeddings of shape (b, t, n_embd)
+        if self.config.scale_embeddings:
+            x = x * (self.config.n_embd**0.5)
+        for block in self.transformer.h:
+            x = block(x, cos, sin, mask, input_pos)
+        x = self.transformer.ln_f(x)
+        if lm_head_chunk_size > 0:
+            # chunk the lm head logits to reduce the peak memory used by autograd
+            return [self.lm_head(x_i) for x_i in x.split(lm_head_chunk_size, dim=1)]
+        return self.lm_head(x)  # (b, t, vocab_size)
+
     @classmethod
     def from_name(cls, name: str, **kwargs: Any) -> Self:
         return cls(Config.from_name(name, **kwargs))
 
     def _init_weights(self, module: nn.Module) -> None:
         """Meant to be used with `gpt.apply(gpt._init_weights)`. Unused method left for completeness."""
         super()._init_weights(module)
@@ -177,14 +206,16 @@
 class LLaMAMLP(litgpt.model.LLaMAMLP):
     def __init__(self, config: Config) -> None:
         nn.Module.__init__(self)
         self.fc_1 = AdapterV2Linear(config.n_embd, config.intermediate_size, bias=config.bias)
         self.fc_2 = AdapterV2Linear(config.n_embd, config.intermediate_size, bias=config.bias)
         self.proj = AdapterV2Linear(config.intermediate_size, config.n_embd, bias=config.bias)
 
+        self.config = config
+
     def _load_from_state_dict(self, state_dict: Dict, prefix: str, *args: Any, **kwargs: Any) -> None:
         """For compatibility with base checkpoints."""
         mapping = {
             "fc_1.weight": "fc_1.linear.weight",
             "fc_1.bias": "fc_1.linear.bias",
             "fc_2.weight": "fc_2.linear.weight",
             "fc_2.bias": "fc_2.linear.bias",
@@ -195,15 +226,15 @@
         super()._load_from_state_dict(state_dict, prefix, *args, **kwargs)
 
 
 class GemmaMLP(LLaMAMLP):
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         x_fc_1 = self.fc_1(x)
         x_fc_2 = self.fc_2(x)
-        x = torch.nn.functional.gelu(x_fc_1) * x_fc_2
+        x = torch.nn.functional.gelu(x_fc_1, approximate=self.config.gelu_approximate) * x_fc_2
         return self.proj(x)
 
 
 class LLaMAMoE(litgpt.model.LLaMAMoE):
     def __init__(self, config: Config) -> None:
         nn.Module.__init__(self)
         self.gate = AdapterV2Linear(config.n_embd, config.n_expert, bias=False)
```

### Comparing `litgpt-0.2.0.dev0/litgpt/args.py` & `litgpt-0.3.0/litgpt/args.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
-
+import math
 from dataclasses import dataclass
 from typing import Optional
 
 
 @dataclass
 class TrainArgs:
     """Training-related arguments"""
@@ -12,16 +12,18 @@
     """Number of optimizer steps between saving checkpoints"""
     log_interval: int = 1
     """Number of iterations between logging calls"""
     global_batch_size: int = 64
     """Number of samples between optimizer steps across data-parallel ranks"""
     micro_batch_size: int = 4
     """Number of samples per data-parallel rank"""
-    lr_warmup_steps: int = 100
+    lr_warmup_steps: Optional[int] = 100
     """Number of iterations with learning rate warmup active"""
+    lr_warmup_fraction: Optional[float] = None
+    """The fraction of an epoch to use for learning rate warmup"""
     epochs: Optional[int] = None
     """Number of epochs to train on"""
     # TODO: `pretrain` is the only script using `max_tokens` explicitly. replace it with epoch_size*epochs?
     max_tokens: Optional[int] = None
     """Total number of tokens to train on"""
     max_steps: Optional[int] = None
     """Limits the number of optimizer steps to run"""
@@ -34,26 +36,42 @@
     learning_rate: float = 1e-3
     weight_decay: float = 0.02
     beta1: float = 0.9
     beta2: float = 0.95
     max_norm: Optional[float] = None
     min_lr: float = 6e-5
 
+    def __post_init__(self) -> None:
+        if self.lr_warmup_fraction and self.lr_warmup_steps:
+            raise ValueError(
+                "Can't provide both `--train.lr_warmup_fraction` and `--train.lr_warmup_steps`. Choose one."
+            )
+        if self.lr_warmup_fraction and not (0 <= self.lr_warmup_fraction <= 1):
+            raise ValueError("`--train.lr_warmup_fraction` must be between 0 and 1.")
+
     def gradient_accumulation_iters(self, devices: int) -> int:
         """Number of iterations between gradient synchronizations"""
         gradient_accumulation_iters = self.batch_size(devices) // self.micro_batch_size
         assert gradient_accumulation_iters > 0
         return gradient_accumulation_iters
 
     def batch_size(self, devices: int) -> int:
         """Number of samples between optimizer steps per data-parallel rank"""
         batch_size = self.global_batch_size // devices
         assert batch_size > 0
         return batch_size
 
+    def warmup_iters(self, devices: int, max_iters: int, train_dataloader) -> int:
+        """Number of iterations to warm up the learning rate."""
+        if self.lr_warmup_fraction:
+            return min(max_iters, math.ceil(self.lr_warmup_fraction * len(train_dataloader)))
+        if self.lr_warmup_steps:
+            return min(max_iters, self.lr_warmup_steps * self.gradient_accumulation_iters(devices))
+        return 0
+
 
 @dataclass
 class EvalArgs:
     """Evaluation-related arguments"""
 
     interval: int = 600
     """Number of optimizer steps between evaluation calls"""
```

### Comparing `litgpt-0.2.0.dev0/litgpt/chat/base.py` & `litgpt-0.3.0/litgpt/chat/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,24 +127,23 @@
             raise ValueError("Quantization and mixed precision is not supported.")
         dtype = {"16-true": torch.float16, "bf16-true": torch.bfloat16, "32-true": torch.float32}[precision]
         plugins = BitsandbytesPrecision(quantize[4:], dtype)
         precision = None
 
     fabric = L.Fabric(devices=1, precision=precision, plugins=plugins)
 
-    check_valid_checkpoint_dir(checkpoint_dir)
-
-    config = Config.from_file(checkpoint_dir / "model_config.yaml")
-
     checkpoint_path = checkpoint_dir / "lit_model.pth"
 
     # Merge if this is a raw LoRA checkpoint
-    if (checkpoint_path / "lit_model.pth.lora").is_file() and not checkpoint_path.is_file():
+    if (checkpoint_dir / "lit_model.pth.lora").is_file() and not checkpoint_path.is_file():
         print("Merging LoRA weights with the base model. This won't take long and is a one-time-only thing.")
-        merge_lora(checkpoint_path)
+        merge_lora(checkpoint_dir)
+
+    check_valid_checkpoint_dir(checkpoint_dir)
+    config = Config.from_file(checkpoint_dir / "model_config.yaml")
 
     with fabric.init_module(empty_init=True):
         model = GPT(config)
         # enable the kv cache
         model.set_kv_cache(batch_size=1)
     load_checkpoint(fabric, model, checkpoint_path)
     model.eval()
```

### Comparing `litgpt-0.2.0.dev0/litgpt/config.py` & `litgpt-0.3.0/litgpt/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,14 +106,16 @@
         conf_dict.update(kwargs)
         return cls(**conf_dict)
 
     @classmethod
     def from_file(cls, path: Union[str, Path], **kwargs: Any) -> Self:
         with open(path, encoding="utf-8") as fp:
             file_kwargs = yaml.safe_load(fp)
+            if file_kwargs is None:
+                raise ValueError(f"{path} is empty which is likely unexpected.")
         file_kwargs.update(kwargs)
         return cls(**file_kwargs)
 
     @classmethod
     def from_checkpoint(cls, path: Path, **kwargs: Any) -> Self:
         """Automatically load `model_config.yaml` and if it doesn't exist - a matching config from `litgpt/config.py`."""
         if (config_path := path / "model_config.yaml").is_file():
@@ -830,14 +832,64 @@
 ]
 for c in llama_2:
     for kind in ("", "-chat"):
         copy = deepcopy(c)
         copy["name"] = c["name"].format(kind)
         copy["hf_config"]["name"] = c["hf_config"]["name"].format(kind)
         configs.append(copy)
+        
+
+###############
+# Meta LLaMA 3
+###############
+llama_3 = [
+    # https://huggingface.co/meta-llama/Meta-Llama-3-8B/blob/main/config.json
+    dict(
+        name="Llama-3-8B{}",
+        hf_config=dict(org="meta-llama", name="Meta-Llama-3-8B{}"),
+        block_size=8192,
+        vocab_size=128000,
+        padded_vocab_size=128256,
+        n_layer=32,
+        n_head=32,
+        n_query_groups=8,
+        rotary_percentage=1.0,
+        parallel_residual=False,
+        bias=False,
+        norm_class_name="RMSNorm",
+        mlp_class_name="LLaMAMLP",
+        intermediate_size=14336,
+        rope_base=500000,
+    ),
+    # https://huggingface.co/meta-llama/Meta-Llama-3-70B/blob/main/config.json
+    dict(
+        name="Llama-3-70B{}",
+        hf_config=dict(org="meta-llama", name="Meta-Llama-3-70B{}"),
+        block_size=8192,
+        vocab_size=128000,
+        padded_vocab_size=128256,
+        n_layer=80,
+        n_head=64,
+        n_embd=8192,
+        n_query_groups=8,
+        rotary_percentage=1.0,
+        parallel_residual=False,
+        bias=False,
+        norm_class_name="RMSNorm",
+        mlp_class_name="LLaMAMLP",
+        intermediate_size=28672,
+        rope_base=500000,
+    ),
+]
+for c in llama_3:
+    for kind in ("", "-Instruct"):
+        copy = deepcopy(c)
+        copy["name"] = c["name"].format(kind)
+        copy["hf_config"]["name"] = c["hf_config"]["name"].format(kind)
+        configs.append(copy)
 
 
 ###############
 # Google Gemma
 ###############
 gemma = [
     # https://huggingface.co/google/gemma-2b/blob/main/config.json
@@ -882,14 +934,40 @@
 configs.extend(gemma)
 for c in gemma:
     copy = deepcopy(c)
     copy["name"] = f"{c['name']}-it"
     copy["hf_config"]["name"] = f"{c['hf_config']['name']}-it"
     configs.append(copy)
 
+##################
+# Google CodeGemma
+##################
+codegemma = [
+    # https://huggingface.co/google/codegemma-7b-it/blob/main/config.json
+    dict(
+        name="CodeGemma-7b-it",
+        hf_config=dict(org="google", name="codegemma-7b-it"),
+        scale_embeddings=True,
+        vocab_size=256000,
+        padding_multiple=64,
+        n_embd=3072,
+        n_layer=28,
+        n_head=16,
+        head_size=256,
+        rotary_percentage=1.0,
+        parallel_residual=False,
+        bias=False,
+        norm_class_name="RMSNorm",
+        mlp_class_name="GemmaMLP",
+        gelu_approximate="tanh",
+        intermediate_size=24576,
+    ),
+]
+configs.extend(codegemma)
+
 
 ##########################
 # Stability AI FreeWilly2
 ##########################
 freewilly_2 = [
     # https://huggingface.co/stabilityai/FreeWilly2/blob/main/config.json
     dict(
@@ -1382,14 +1460,32 @@
 for c in mistral:
     for kind in ("", "Instruct-"):
         copy = deepcopy(c)
         copy["name"] = c["name"].format(kind)
         copy["hf_config"]["name"] = c["hf_config"]["name"].format(kind)
         configs.append(copy)
 configs.append(
+    # https://huggingface.co/unsloth/mistral-7b-v0.2/blob/main/config.json
+    dict(
+        name="Mistral-7B-v0.2",
+        hf_config=dict(org="unsloth", name="Mistral-7B-v0.2"),
+        padded_vocab_size=32000,
+        block_size=32768,
+        n_layer=32,
+        n_query_groups=8,
+        rotary_percentage=1.0,
+        parallel_residual=False,
+        bias=False,
+        norm_class_name="RMSNorm",
+        norm_eps=1e-05,
+        mlp_class_name="LLaMAMLP",
+        intermediate_size=14336,
+    )
+)
+configs.append(
     # https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2/blob/main/config.json
     dict(
         name="Mistral-7B-Instruct-v0.2",
         hf_config=dict(org="mistralai", name="Mistral-7B-Instruct-v0.2"),
         padded_vocab_size=32000,
         block_size=32768,
         n_layer=32,
```

### Comparing `litgpt-0.2.0.dev0/litgpt/data/__init__.py` & `litgpt-0.3.0/litgpt/data/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from litgpt.data.json_data import JSON
 from litgpt.data.deita import Deita
 from litgpt.data.dolly import Dolly
 from litgpt.data.flan import FLAN
 from litgpt.data.lima import LIMA
 from litgpt.data.lit_data import LitData
 from litgpt.data.longform import LongForm
+from litgpt.data.text_files import TextFiles
 from litgpt.data.tinyllama import TinyLlama
 from litgpt.data.tinystories import TinyStories
 from litgpt.data.openwebtext import OpenWebText
 
 
 __all__ = [
     "Alpaca",
@@ -26,11 +27,12 @@
     "JSON",
     "LIMA",
     "LitData",
     "DataModule",
     "LongForm",
     "OpenWebText",
     "SFTDataset",
+    "TextFiles",
     "TinyLlama",
     "TinyStories",
     "get_sft_collate_fn",
 ]
```

### Comparing `litgpt-0.2.0.dev0/litgpt/data/alpaca.py` & `litgpt-0.3.0/litgpt/data/alpaca.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 
 import json
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Optional, Union
 
 import torch
-from torch.utils.data import random_split, DataLoader
 from lightning_utilities.core.imports import RequirementCache
-from litgpt.data import SFTDataset, get_sft_collate_fn, DataModule
+from torch.utils.data import DataLoader, random_split
+
+from litgpt.data import DataModule, SFTDataset, get_sft_collate_fn
 from litgpt.prompts import PromptStyle
 from litgpt.tokenizer import Tokenizer
 
 _URL = "https://raw.githubusercontent.com/tloen/alpaca-lora/main/alpaca_data_cleaned_archive.json"
 
 
 @dataclass
```

### Comparing `litgpt-0.2.0.dev0/litgpt/data/alpaca_2k.py` & `litgpt-0.3.0/litgpt/data/alpaca_2k.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
 
 
 from dataclasses import dataclass, field
 from pathlib import Path
-from litgpt.data.alpaca import Alpaca
+
 from litgpt.data import SFTDataset
+from litgpt.data.alpaca import Alpaca
 
 
 @dataclass
 class Alpaca2k(Alpaca):
     """Alpaca2k data module for supervised finetuning."""
 
     val_split_fraction: float = 0.05  # to get exactly 100 validation samples,
```

### Comparing `litgpt-0.2.0.dev0/litgpt/data/alpaca_gpt4.py` & `litgpt-0.3.0/litgpt/data/alpaca_gpt4.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
 
 
 from dataclasses import dataclass, field
 from pathlib import Path
-from litgpt.data.alpaca import Alpaca
 
+from litgpt.data.alpaca import Alpaca
 
 _URL = "https://raw.githubusercontent.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM/main/data/alpaca_gpt4_data.json"
 
 
 @dataclass
 class AlpacaGPT4(Alpaca):
     """AlpacaGPT4 data module for supervised finetuning."""
```

### Comparing `litgpt-0.2.0.dev0/litgpt/data/base.py` & `litgpt-0.3.0/litgpt/data/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
 from abc import abstractmethod
 from functools import partial
-from typing import List, Dict, Union, Optional, Callable, Any
+from typing import Any, Callable, Dict, List, Optional, Union
 
 import torch
+from lightning import LightningDataModule
 from torch import Tensor
 from torch.utils.data import Dataset
 
-from lightning import LightningDataModule
 from litgpt import Tokenizer
 from litgpt.prompts import PromptStyle
 
 
 class DataModule(LightningDataModule):
     """Base class for all data modules in LitGPT."""
```

### Comparing `litgpt-0.2.0.dev0/litgpt/data/deita.py` & `litgpt-0.3.0/litgpt/data/deita.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
 """Implementation derived from https://github.com/tloen/alpaca-lora"""
-from pathlib import Path
 from dataclasses import dataclass, field
-
-from typing import Optional, List, Union
+from pathlib import Path
+from typing import List, Optional, Union
 
 import torch
 from torch.utils.data import DataLoader
 
 from litgpt import PromptStyle
 from litgpt.data import DataModule, SFTDataset, get_sft_collate_fn
 from litgpt.tokenizer import Tokenizer
```

### Comparing `litgpt-0.2.0.dev0/litgpt/data/dolly.py` & `litgpt-0.3.0/litgpt/data/dolly.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 from typing import Union
 
 import torch
 from torch.utils.data import random_split
 
 from litgpt import PromptStyle
-from litgpt.data import SFTDataset, Alpaca
+from litgpt.data import Alpaca, SFTDataset
 
 _URL: str = "https://huggingface.co/datasets/databricks/databricks-dolly-15k/resolve/main/databricks-dolly-15k.jsonl"
 
 
 @dataclass
 class Dolly(Alpaca):
     """Dolly data module for supervised finetuning."""
```

### Comparing `litgpt-0.2.0.dev0/litgpt/data/flan.py` & `litgpt-0.3.0/litgpt/data/flan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
 
 import json
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import Optional, Dict, List, Set, Union
+from typing import Dict, List, Optional, Set, Union
 
 import torch
 from torch.utils.data import DataLoader
 
 from litgpt import PromptStyle
-from litgpt.data import SFTDataset, get_sft_collate_fn, DataModule
+from litgpt.data import DataModule, SFTDataset, get_sft_collate_fn
 from litgpt.data.alpaca import download_if_missing
 from litgpt.tokenizer import Tokenizer
 
 _URL = "https://huggingface.co/datasets/Muennighoff/flan/resolve/main"
 
 
 # TODO: Including all subsets, FLAN is too large to be loaded in memory. Switch the implementation to cache
```

### Comparing `litgpt-0.2.0.dev0/litgpt/data/json_data.py` & `litgpt-0.3.0/litgpt/data/json_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
 
 import json
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import Optional, Union, Tuple, Any
+from typing import Any, Optional, Tuple, Union
 
 import torch
-from torch.utils.data import random_split, DataLoader
+from torch.utils.data import DataLoader, random_split
 
 from litgpt import PromptStyle
-from litgpt.data import SFTDataset, get_sft_collate_fn, DataModule
+from litgpt.data import DataModule, SFTDataset, get_sft_collate_fn
 from litgpt.tokenizer import Tokenizer
 
 
 @dataclass
 class JSON(DataModule):
     """Loads JSON or JSONL data for supervised finetuning."""
 
     json_path: Path
-    """A path to a JSON file or a directory with `train.json` and `val.json` containing the data. 
-    The file(s) should contain a list of samples (dicts). Each dict must have the keys 'instruction' and 'output', 
+    """A path to a JSON file or a directory with `train.json` and `val.json` containing the data.
+    The file(s) should contain a list of samples (dicts). Each dict must have the keys 'instruction' and 'output',
     and can optionally have a key 'input' (see Alpaca)."""
     mask_prompt: bool = False
     """Whether to mask the prompt section from the label (with ``ignore_index``)."""
     val_split_fraction: Optional[float] = None
     """The fraction of the dataset to use for the validation dataset. The rest is used for training.
     Only applies if you passed in a single file to `json_path`."""
     prompt_style: Union[str, PromptStyle] = "alpaca"
@@ -38,14 +38,19 @@
     tokenizer: Optional[Tokenizer] = field(default=None, init=False, repr=False)
     batch_size: int = field(default=1, init=False, repr=False)
     max_seq_length: int = field(default=-1, init=False, repr=False)
     train_dataset: Optional[SFTDataset] = field(default=None, init=False, repr=False)
     val_dataset: Optional[SFTDataset] = field(default=None, init=False, repr=False)
 
     def __post_init__(self):
+        if self.json_path.is_file() and self.val_split_fraction is None:
+            raise ValueError(
+                "If `json_path` is a file, you must set `val_split_fraction` to a value between 0 and 1 to split the"
+                " data into train and validation sets."
+            )
         if self.json_path.is_dir() and self.val_split_fraction is not None:
             raise ValueError(
                 "If `json_path` is a directory, it must contain 'train.json' and 'val.json' files and"
                 f" hence `val_split_fraction` should not be set. Got `{self.val_split_fraction=}`."
             )
         if not self.json_path.exists():
             raise FileNotFoundError(
```

### Comparing `litgpt-0.2.0.dev0/litgpt/data/lima.py` & `litgpt-0.3.0/litgpt/data/lima.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
 """Implementation derived from https://github.com/tloen/alpaca-lora"""
 import os
 from dataclasses import dataclass, field
-
-from typing import Optional, List, Union
+from typing import List, Optional, Union
 
 import torch
-from torch.utils.data import random_split, DataLoader
+from torch.utils.data import DataLoader, random_split
 
 from litgpt import PromptStyle
 from litgpt.data import DataModule, SFTDataset, get_sft_collate_fn
 from litgpt.tokenizer import Tokenizer
 
 
 @dataclass
```

### Comparing `litgpt-0.2.0.dev0/litgpt/data/lit_data.py` & `litgpt-0.3.0/litgpt/data/lit_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
 import os
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import Union, Optional, Tuple
+from typing import Optional, Tuple, Union
 
 from torch.utils.data import DataLoader
 
 from litgpt import Tokenizer
 from litgpt.data import DataModule
```

### Comparing `litgpt-0.2.0.dev0/litgpt/data/longform.py` & `litgpt-0.3.0/litgpt/data/longform.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 from pathlib import Path
 from typing import Optional, Union
 
 import torch
 from torch.utils.data import DataLoader
 
 from litgpt import PromptStyle
-from litgpt.data import SFTDataset, get_sft_collate_fn, DataModule
+from litgpt.data import DataModule, SFTDataset, get_sft_collate_fn
 from litgpt.data.alpaca import download_if_missing
 from litgpt.tokenizer import Tokenizer
 
-
 _URL = "https://raw.githubusercontent.com/akoksal/LongForm/main/dataset"
 
 
 @dataclass
 class LongForm(DataModule):
     """LongForm data module for supervised finetuning."""
```

### Comparing `litgpt-0.2.0.dev0/litgpt/data/openwebtext.py` & `litgpt-0.3.0/litgpt/data/openwebtext.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
 import os
 from dataclasses import dataclass, field
 from functools import partial
 from pathlib import Path
-from typing import Union, Optional
+from typing import Optional, Union
 
 from torch.utils.data import DataLoader
 
 from litgpt import Tokenizer
 from litgpt.data import DataModule
```

### Comparing `litgpt-0.2.0.dev0/litgpt/data/prepare_slimpajama.py` & `litgpt-0.3.0/litgpt/data/prepare_slimpajama.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import json
 import os
 import time
 from pathlib import Path
 
 from litgpt import Tokenizer
-from litgpt.utils import CLI
 from litgpt.data.prepare_starcoder import DataChunkRecipe
+from litgpt.utils import CLI
 
 
 class SlimPajamaDataRecipe(DataChunkRecipe):
     def __init__(self, tokenizer: Tokenizer, chunk_size: int):
         super().__init__(chunk_size)
         self.tokenizer = tokenizer
```

### Comparing `litgpt-0.2.0.dev0/litgpt/data/prepare_starcoder.py` & `litgpt-0.3.0/litgpt/data/prepare_starcoder.py`

 * *Files identical despite different names*

### Comparing `litgpt-0.2.0.dev0/litgpt/data/tinyllama.py` & `litgpt-0.3.0/litgpt/data/tinyllama.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import Union, Optional
+from typing import Optional, Union
 
 from torch.utils.data import DataLoader
 
 from litgpt import Tokenizer
 from litgpt.data import DataModule
```

### Comparing `litgpt-0.2.0.dev0/litgpt/finetune/adapter.py` & `litgpt-0.3.0/litgpt/finetune/adapter_v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,75 +11,80 @@
 import torch
 from lightning.fabric.plugins import BitsandbytesPrecision
 from lightning.fabric.strategies import FSDPStrategy
 from lightning.fabric.utilities import ThroughputMonitor
 from torch.utils.data import DataLoader
 from torchmetrics import RunningMean
 
-from litgpt.adapter import GPT, Block, Config, adapter_filter, mark_only_adapter_as_trainable
+from litgpt.adapter_v2 import GPT, Block, Config, adapter_filter, mark_only_adapter_v2_as_trainable
 from litgpt.args import EvalArgs, TrainArgs
 from litgpt.data import Alpaca, DataModule
 from litgpt.generate.base import generate
 from litgpt.prompts import save_prompt_style
 from litgpt.tokenizer import Tokenizer
 from litgpt.utils import (
     CLI,
     CycleIterator,
     check_valid_checkpoint_dir,
     choose_logger,
     chunked_cross_entropy,
     copy_config_files,
     get_default_supported_precision,
+    init_out_dir,
     load_checkpoint,
     num_parameters,
     parse_devices,
     save_hyperparameters,
 )
 
 
 def setup(
     checkpoint_dir: Path = Path("checkpoints/stabilityai/stablelm-base-alpha-3b"),
-    out_dir: Path = Path("out/finetune/adapter"),
+    out_dir: Path = Path("out/finetune/adapter-v2"),
     precision: Optional[str] = None,
     quantize: Optional[Literal["bnb.nf4", "bnb.nf4-dq", "bnb.fp4", "bnb.fp4-dq", "bnb.int8-training"]] = None,
     devices: Union[int, str] = 1,
     data: Optional[DataModule] = None,
     train: TrainArgs = TrainArgs(
         save_interval=1000,
         log_interval=1,
-        global_batch_size=128,
-        micro_batch_size=4,
+        global_batch_size=16,
+        micro_batch_size=1,
         lr_warmup_steps=100,
         epochs=5,
         learning_rate=1e-3,
         max_seq_length=None,
     ),
     eval: EvalArgs = EvalArgs(interval=100, max_new_tokens=100, max_iters=100),
     logger_name: Literal["wandb", "tensorboard", "csv"] = "csv",
     seed: int = 1337,
 ) -> None:
-    """Finetune a model using the Adapter method.
+    """Finetune a model using the Adapter V2 method.
 
     Arguments:
         checkpoint_dir: The path to the base model's checkpoint directory to load for finetuning.
-        out_dir: Directory in which to save checkpoints and logs.
+        out_dir: Directory in which to save checkpoints and logs. If running in a Lightning Studio Job, look for it in
+            /teamspace/jobs/<job-name>/share.
         precision: The precision to use for finetuning. Possible choices: "bf16-true", "bf16-mixed", "32-true".
         quantize: If set, quantize the model with this algorithm. See ``tutorials/quantize.md`` for more information.
         devices: How many devices/GPUs to use.
         data: Data-related arguments. If not provided, the default is ``litgpt.data.Alpaca``.
         train: Training-related arguments. See ``litgpt.args.TrainArgs`` for details.
         eval: Evaluation-related arguments. See ``litgpt.args.EvalArgs`` for details.
         logger_name: The name of the logger to send metrics to.
         seed: The random seed to use for reproducibility.
     """
 
     pprint(locals())
     data = Alpaca() if data is None else data
     devices = parse_devices(devices)
-    config = Config.from_name(name=checkpoint_dir.name)
+    out_dir = init_out_dir(out_dir)
+
+    check_valid_checkpoint_dir(checkpoint_dir)
+    config = Config.from_file(checkpoint_dir / "model_config.yaml")
 
     precision = precision or get_default_supported_precision(training=True)
     logger = choose_logger(logger_name, out_dir, name=f"finetune-{config.name}", log_interval=train.log_interval)
 
     plugins = None
     if quantize is not None and quantize.startswith("bnb."):
         if "mixed" in precision:
@@ -116,33 +121,32 @@
     data: DataModule,
     checkpoint_dir: Path,
     out_dir: Path,
     train: TrainArgs,
     eval: EvalArgs,
 ) -> None:
     validate_args(train, eval)
-    check_valid_checkpoint_dir(checkpoint_dir)
 
     tokenizer = Tokenizer(checkpoint_dir)
     train_dataloader, val_dataloader = get_dataloaders(fabric, data, tokenizer, train)
     steps_per_epoch = len(train_dataloader) // train.gradient_accumulation_iters(devices)
     lr_max_steps = min(train.epochs * steps_per_epoch, (train.max_steps or float("inf")))
 
     fabric.seed_everything(seed)  # same seed for every process to init model (FSDP)
 
     if fabric.global_rank == 0:
         os.makedirs(out_dir, exist_ok=True)
 
     checkpoint_path = checkpoint_dir / "lit_model.pth"
     with fabric.init_module(empty_init=(devices > 1)):
         model = GPT(config)
-    mark_only_adapter_as_trainable(model)
+    mark_only_adapter_v2_as_trainable(model)
 
     fabric.print(f"Number of trainable parameters: {num_parameters(model, requires_grad=True):,}")
-    fabric.print(f"Number of non trainable parameters: {num_parameters(model, requires_grad=False):,}")
+    fabric.print(f"Number of non-trainable parameters: {num_parameters(model, requires_grad=False):,}")
 
     model = fabric.setup_module(model)
 
     trainable_params = [p for p in model.parameters() if p.requires_grad]
     if isinstance(fabric.strategy.precision, BitsandbytesPrecision):
         import bitsandbytes as bnb
 
@@ -173,18 +177,24 @@
         eval,
         data,
     )
     fabric.print(f"Training time: {(time.perf_counter() - train_time):.2f}s")
     if fabric.device.type == "cuda":
         fabric.print(f"Memory used: {torch.cuda.max_memory_allocated() / 1e9:.02f} GB")
 
+    # Final evaluation
+    val_loss = validate(fabric, model, val_dataloader, dataclasses.replace(eval, max_iters=len(val_dataloader)))
+    metrics = {"val_loss": val_loss, "val_ppl": math.exp(val_loss)}
+    fabric.log_dict(metrics)
+    fabric.print(f"Final evaluation | val loss: {val_loss.item():.3f} | val ppl: {math.exp(val_loss):.3f}")
+
     # Save the final Adapter checkpoint at the end of training
-    save_path = out_dir / "final" / "lit_model.pth.adapter"
+    save_path = out_dir / "final" / "lit_model.pth.adapter_v2"
     save_path.parent.mkdir(parents=True, exist_ok=True)
-    save_adapter_checkpoint(fabric, model, save_path)
+    save_adapter_v2_checkpoint(fabric, model, save_path)
     if fabric.global_rank == 0:
         # Copy checkpoint files from original checkpoint dir
         copy_config_files(checkpoint_dir, save_path.parent)
         save_hyperparameters(setup, save_path.parent)
         save_prompt_style(data.prompt_style, save_path.parent)
 
 
@@ -206,15 +216,15 @@
     longest_seq_length, longest_seq_ix = get_longest_seq_length(train_dataloader.dataset)
     model.max_seq_length = min(longest_seq_length, train.max_seq_length or float("inf"))
     fabric.print(
         f"The longest sequence length in the train data is {longest_seq_length}, the model's maximum sequence length is"
         f" {model.max_seq_length} and context length is {model.config.block_size}"
     )
 
-    validate(fabric, model, val_dataloader, tokenizer, dataclasses.replace(eval, max_iters=2), data)  # sanity check
+    validate(fabric, model, val_dataloader, dataclasses.replace(eval, max_iters=2))  # sanity check
 
     train_iterator = CycleIterator(train_dataloader)
     throughput = ThroughputMonitor(fabric, window_size=50)
     running_loss = RunningMean(window=train.gradient_accumulation_iters(devices), sync_on_compute=False).to(
         fabric.device
     )
     max_steps = train.max_steps or float("inf")
@@ -273,66 +283,69 @@
                 f" iter time: {metrics['iter_time'] * 1000:.2f} ms"
                 f"{' (step)' if not is_accumulating else ''}"
             )
             fabric.log_dict(metrics, step=iter_num)
 
         if not is_accumulating and step_count % eval.interval == 0:
             t0 = time.perf_counter()
-            val_loss = validate(fabric, model, val_dataloader, tokenizer, eval, data)
+            val_loss = validate(fabric, model, val_dataloader, eval)
+            generate_example(fabric, model, tokenizer, eval, data)
             t1 = time.perf_counter() - t0
             fabric.print(f"iter {iter_num}: val loss {val_loss.item():.4f}, val time: {t1 * 1000:.2f} ms")
             metrics = {"val_loss": val_loss, "val_ppl": math.exp(val_loss)}
             fabric.log_dict(metrics, step=iter_num)
             fabric.barrier()
 
         if train.save_interval is not None and not is_accumulating and step_count % train.save_interval == 0:
-            checkpoint_file = out_dir / f"step-{step_count:06d}" / "lit_model.pth.adapter"
+            checkpoint_file = out_dir / f"step-{step_count:06d}" / "lit_model.pth.adapter_v2"
             checkpoint_file.parent.mkdir(parents=True, exist_ok=True)
-            save_adapter_checkpoint(fabric, model, checkpoint_file)
+            save_adapter_v2_checkpoint(fabric, model, checkpoint_file)
             if fabric.global_rank == 0:
                 copy_config_files(checkpoint_dir, checkpoint_file.parent)
                 save_hyperparameters(setup, checkpoint_file.parent)
                 save_prompt_style(data.prompt_style, checkpoint_file.parent)
 
 
-# the adapter "kv cache" cannot be initialized under `inference_mode`
 @torch.no_grad()
-def validate(
-    fabric: L.Fabric, model: GPT, val_dataloader: DataLoader, tokenizer: Tokenizer, eval: EvalArgs, data: DataModule
-) -> torch.Tensor:
+def validate(fabric: L.Fabric, model: GPT, val_dataloader: DataLoader, eval: EvalArgs) -> torch.Tensor:
     fabric.print("Validating ...")
     model.eval()
     losses = torch.zeros(min(len(val_dataloader), eval.max_iters))
     for k, batch in enumerate(val_dataloader):
         if k >= eval.max_iters:
             break
         input_ids, targets = batch["input_ids"], batch["labels"]
         logits = model(input_ids)
         losses[k] = chunked_cross_entropy(logits[..., :-1, :], targets[..., 1:], chunk_size=0)
 
     val_loss = losses.mean()
+    model.train()
+    return val_loss
+
 
-    # produce an example:
+# the adapter "kv cache" cannot be initialized under `inference_mode`
+@torch.no_grad()
+def generate_example(fabric: L.Fabric, model: GPT, tokenizer: Tokenizer, eval: EvalArgs, data: DataModule):
     instruction = "Recommend a movie for me to watch during the weekend and explain the reason."
     fabric.print(instruction)
     prompt = data.prompt_style.apply(instruction)
     encoded = tokenizer.encode(prompt, device=fabric.device)
+    model.eval()
+
     with fabric.init_tensor():
         # do not set `max_seq_length=max_returned_token` because memory is not a concern here
         model.set_kv_cache(batch_size=1)
     output = generate(
         model, encoded, max_returned_tokens=len(encoded) + eval.max_new_tokens, temperature=0.8, eos_id=tokenizer.eos_id
     )
     model.clear_kv_cache()
+    model.train()
     output = tokenizer.decode(output)
     fabric.print(output)
 
-    model.train()
-    return val_loss
-
 
 def get_lr_scheduler(optimizer, warmup_steps: int, max_steps: int):
     # linear warmup followed by cosine annealing
     scheduler1 = torch.optim.lr_scheduler.LambdaLR(optimizer, lambda step: step / warmup_steps)
     scheduler2 = torch.optim.lr_scheduler.CosineAnnealingLR(optimizer, T_max=(max_steps - warmup_steps))
     return torch.optim.lr_scheduler.SequentialLR(optimizer, [scheduler1, scheduler2], milestones=[warmup_steps])
 
@@ -354,22 +367,22 @@
     # find out the minimum max_seq_length required during fine-tuning (saves memory!)
     lengths = [len(d["input_ids"]) for d in data]
     longest_seq_length = max(lengths)
     longest_seq_ix = lengths.index(longest_seq_length)
     return longest_seq_length, longest_seq_ix
 
 
-def save_adapter_checkpoint(fabric: L.Fabric, model: torch.nn.Module, file_path: Path) -> None:
-    fabric.print(f"Saving adapter weights to {str(file_path)!r}")
+def save_adapter_v2_checkpoint(fabric: L.Fabric, model: torch.nn.Module, file_path: Path) -> None:
+    fabric.print(f"Saving adapter v2 weights to {str(file_path)!r}")
     fabric.save(file_path, {"model": model}, filter={"model": adapter_filter})
 
 
 def validate_args(train: TrainArgs, eval: EvalArgs) -> None:
     issues = []
-    unsupported = [(train, ["max_tokens", "max_norm", "tie_embeddings"])]
+    unsupported = [(train, ["max_tokens", "max_norm", "tie_embeddings", "lr_warmup_fraction"])]
     for args, names in unsupported:
         for name in names:
             if getattr(args, name) is not None:
                 issues.append(f"{__file__} doesn't support the {name!r} argument. This is set in {args}")
     required = [(train, ["epochs"]), (eval, ["max_new_tokens"])]
     for args, names in required:
         for name in names:
```

### Comparing `litgpt-0.2.0.dev0/litgpt/finetune/adapter_v2.py` & `litgpt-0.3.0/litgpt/finetune/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,75 +11,80 @@
 import torch
 from lightning.fabric.plugins import BitsandbytesPrecision
 from lightning.fabric.strategies import FSDPStrategy
 from lightning.fabric.utilities import ThroughputMonitor
 from torch.utils.data import DataLoader
 from torchmetrics import RunningMean
 
-from litgpt.adapter_v2 import GPT, Block, Config, adapter_filter, mark_only_adapter_v2_as_trainable
+from litgpt.adapter import GPT, Block, Config, adapter_filter, mark_only_adapter_as_trainable
 from litgpt.args import EvalArgs, TrainArgs
 from litgpt.data import Alpaca, DataModule
 from litgpt.generate.base import generate
 from litgpt.prompts import save_prompt_style
 from litgpt.tokenizer import Tokenizer
 from litgpt.utils import (
     CLI,
     CycleIterator,
     check_valid_checkpoint_dir,
     choose_logger,
     chunked_cross_entropy,
     copy_config_files,
     get_default_supported_precision,
+    init_out_dir,
     load_checkpoint,
     num_parameters,
     parse_devices,
     save_hyperparameters,
 )
 
 
 def setup(
     checkpoint_dir: Path = Path("checkpoints/stabilityai/stablelm-base-alpha-3b"),
-    out_dir: Path = Path("out/finetune/adapter-v2"),
+    out_dir: Path = Path("out/finetune/adapter"),
     precision: Optional[str] = None,
     quantize: Optional[Literal["bnb.nf4", "bnb.nf4-dq", "bnb.fp4", "bnb.fp4-dq", "bnb.int8-training"]] = None,
     devices: Union[int, str] = 1,
     data: Optional[DataModule] = None,
     train: TrainArgs = TrainArgs(
         save_interval=1000,
         log_interval=1,
-        global_batch_size=128,
-        micro_batch_size=4,
+        global_batch_size=16,
+        micro_batch_size=1,
         lr_warmup_steps=100,
         epochs=5,
         learning_rate=1e-3,
         max_seq_length=None,
     ),
     eval: EvalArgs = EvalArgs(interval=100, max_new_tokens=100, max_iters=100),
     logger_name: Literal["wandb", "tensorboard", "csv"] = "csv",
     seed: int = 1337,
 ) -> None:
-    """Finetune a model using the Adapter V2 method.
+    """Finetune a model using the Adapter method.
 
     Arguments:
         checkpoint_dir: The path to the base model's checkpoint directory to load for finetuning.
-        out_dir: Directory in which to save checkpoints and logs.
+        out_dir: Directory in which to save checkpoints and logs. If running in a Lightning Studio Job, look for it in
+            /teamspace/jobs/<job-name>/share.
         precision: The precision to use for finetuning. Possible choices: "bf16-true", "bf16-mixed", "32-true".
         quantize: If set, quantize the model with this algorithm. See ``tutorials/quantize.md`` for more information.
         devices: How many devices/GPUs to use.
         data: Data-related arguments. If not provided, the default is ``litgpt.data.Alpaca``.
         train: Training-related arguments. See ``litgpt.args.TrainArgs`` for details.
         eval: Evaluation-related arguments. See ``litgpt.args.EvalArgs`` for details.
         logger_name: The name of the logger to send metrics to.
         seed: The random seed to use for reproducibility.
     """
 
     pprint(locals())
     data = Alpaca() if data is None else data
     devices = parse_devices(devices)
-    config = Config.from_name(name=checkpoint_dir.name)
+    out_dir = init_out_dir(out_dir)
+
+    check_valid_checkpoint_dir(checkpoint_dir)
+    config = Config.from_file(checkpoint_dir / "model_config.yaml")
 
     precision = precision or get_default_supported_precision(training=True)
     logger = choose_logger(logger_name, out_dir, name=f"finetune-{config.name}", log_interval=train.log_interval)
 
     plugins = None
     if quantize is not None and quantize.startswith("bnb."):
         if "mixed" in precision:
@@ -116,33 +121,32 @@
     data: DataModule,
     checkpoint_dir: Path,
     out_dir: Path,
     train: TrainArgs,
     eval: EvalArgs,
 ) -> None:
     validate_args(train, eval)
-    check_valid_checkpoint_dir(checkpoint_dir)
 
     tokenizer = Tokenizer(checkpoint_dir)
     train_dataloader, val_dataloader = get_dataloaders(fabric, data, tokenizer, train)
     steps_per_epoch = len(train_dataloader) // train.gradient_accumulation_iters(devices)
     lr_max_steps = min(train.epochs * steps_per_epoch, (train.max_steps or float("inf")))
 
     fabric.seed_everything(seed)  # same seed for every process to init model (FSDP)
 
     if fabric.global_rank == 0:
         os.makedirs(out_dir, exist_ok=True)
 
     checkpoint_path = checkpoint_dir / "lit_model.pth"
     with fabric.init_module(empty_init=(devices > 1)):
         model = GPT(config)
-    mark_only_adapter_v2_as_trainable(model)
+    mark_only_adapter_as_trainable(model)
 
     fabric.print(f"Number of trainable parameters: {num_parameters(model, requires_grad=True):,}")
-    fabric.print(f"Number of non trainable parameters: {num_parameters(model, requires_grad=False):,}")
+    fabric.print(f"Number of non-trainable parameters: {num_parameters(model, requires_grad=False):,}")
 
     model = fabric.setup_module(model)
 
     trainable_params = [p for p in model.parameters() if p.requires_grad]
     if isinstance(fabric.strategy.precision, BitsandbytesPrecision):
         import bitsandbytes as bnb
 
@@ -173,18 +177,24 @@
         eval,
         data,
     )
     fabric.print(f"Training time: {(time.perf_counter() - train_time):.2f}s")
     if fabric.device.type == "cuda":
         fabric.print(f"Memory used: {torch.cuda.max_memory_allocated() / 1e9:.02f} GB")
 
+    # Final evaluation
+    val_loss = validate(fabric, model, val_dataloader, dataclasses.replace(eval, max_iters=len(val_dataloader)))
+    metrics = {"val_loss": val_loss, "val_ppl": math.exp(val_loss)}
+    fabric.log_dict(metrics)
+    fabric.print(f"Final evaluation | val loss: {val_loss.item():.3f} | val ppl: {math.exp(val_loss):.3f}")
+
     # Save the final Adapter checkpoint at the end of training
-    save_path = out_dir / "final" / "lit_model.pth.adapter_v2"
+    save_path = out_dir / "final" / "lit_model.pth.adapter"
     save_path.parent.mkdir(parents=True, exist_ok=True)
-    save_adapter_v2_checkpoint(fabric, model, save_path)
+    save_adapter_checkpoint(fabric, model, save_path)
     if fabric.global_rank == 0:
         # Copy checkpoint files from original checkpoint dir
         copy_config_files(checkpoint_dir, save_path.parent)
         save_hyperparameters(setup, save_path.parent)
         save_prompt_style(data.prompt_style, save_path.parent)
 
 
@@ -206,15 +216,15 @@
     longest_seq_length, longest_seq_ix = get_longest_seq_length(train_dataloader.dataset)
     model.max_seq_length = min(longest_seq_length, train.max_seq_length or float("inf"))
     fabric.print(
         f"The longest sequence length in the train data is {longest_seq_length}, the model's maximum sequence length is"
         f" {model.max_seq_length} and context length is {model.config.block_size}"
     )
 
-    validate(fabric, model, val_dataloader, tokenizer, dataclasses.replace(eval, max_iters=2), data)  # sanity check
+    validate(fabric, model, val_dataloader, dataclasses.replace(eval, max_iters=2))  # sanity check
 
     train_iterator = CycleIterator(train_dataloader)
     throughput = ThroughputMonitor(fabric, window_size=50)
     running_loss = RunningMean(window=train.gradient_accumulation_iters(devices), sync_on_compute=False).to(
         fabric.device
     )
     max_steps = train.max_steps or float("inf")
@@ -273,66 +283,69 @@
                 f" iter time: {metrics['iter_time'] * 1000:.2f} ms"
                 f"{' (step)' if not is_accumulating else ''}"
             )
             fabric.log_dict(metrics, step=iter_num)
 
         if not is_accumulating and step_count % eval.interval == 0:
             t0 = time.perf_counter()
-            val_loss = validate(fabric, model, val_dataloader, tokenizer, eval, data)
+            val_loss = validate(fabric, model, val_dataloader, eval)
+            generate_example(fabric, model, tokenizer, eval, data)
             t1 = time.perf_counter() - t0
             fabric.print(f"iter {iter_num}: val loss {val_loss.item():.4f}, val time: {t1 * 1000:.2f} ms")
             metrics = {"val_loss": val_loss, "val_ppl": math.exp(val_loss)}
             fabric.log_dict(metrics, step=iter_num)
             fabric.barrier()
 
         if train.save_interval is not None and not is_accumulating and step_count % train.save_interval == 0:
-            checkpoint_file = out_dir / f"step-{step_count:06d}" / "lit_model.pth.adapter_v2"
+            checkpoint_file = out_dir / f"step-{step_count:06d}" / "lit_model.pth.adapter"
             checkpoint_file.parent.mkdir(parents=True, exist_ok=True)
-            save_adapter_v2_checkpoint(fabric, model, checkpoint_file)
+            save_adapter_checkpoint(fabric, model, checkpoint_file)
             if fabric.global_rank == 0:
                 copy_config_files(checkpoint_dir, checkpoint_file.parent)
                 save_hyperparameters(setup, checkpoint_file.parent)
                 save_prompt_style(data.prompt_style, checkpoint_file.parent)
 
 
-# the adapter "kv cache" cannot be initialized under `inference_mode`
 @torch.no_grad()
-def validate(
-    fabric: L.Fabric, model: GPT, val_dataloader: DataLoader, tokenizer: Tokenizer, eval: EvalArgs, data: DataModule
-) -> torch.Tensor:
+def validate(fabric: L.Fabric, model: GPT, val_dataloader: DataLoader, eval: EvalArgs) -> torch.Tensor:
     fabric.print("Validating ...")
     model.eval()
     losses = torch.zeros(min(len(val_dataloader), eval.max_iters))
     for k, batch in enumerate(val_dataloader):
         if k >= eval.max_iters:
             break
         input_ids, targets = batch["input_ids"], batch["labels"]
         logits = model(input_ids)
         losses[k] = chunked_cross_entropy(logits[..., :-1, :], targets[..., 1:], chunk_size=0)
 
     val_loss = losses.mean()
+    model.train()
+    return val_loss
+
 
-    # produce an example:
+# the adapter "kv cache" cannot be initialized under `inference_mode`
+@torch.no_grad()
+def generate_example(fabric: L.Fabric, model: GPT, tokenizer: Tokenizer, eval: EvalArgs, data: DataModule):
     instruction = "Recommend a movie for me to watch during the weekend and explain the reason."
     fabric.print(instruction)
     prompt = data.prompt_style.apply(instruction)
     encoded = tokenizer.encode(prompt, device=fabric.device)
+    model.eval()
+
     with fabric.init_tensor():
         # do not set `max_seq_length=max_returned_token` because memory is not a concern here
         model.set_kv_cache(batch_size=1)
     output = generate(
         model, encoded, max_returned_tokens=len(encoded) + eval.max_new_tokens, temperature=0.8, eos_id=tokenizer.eos_id
     )
     model.clear_kv_cache()
+    model.train()
     output = tokenizer.decode(output)
     fabric.print(output)
 
-    model.train()
-    return val_loss
-
 
 def get_lr_scheduler(optimizer, warmup_steps: int, max_steps: int):
     # linear warmup followed by cosine annealing
     scheduler1 = torch.optim.lr_scheduler.LambdaLR(optimizer, lambda step: step / warmup_steps)
     scheduler2 = torch.optim.lr_scheduler.CosineAnnealingLR(optimizer, T_max=(max_steps - warmup_steps))
     return torch.optim.lr_scheduler.SequentialLR(optimizer, [scheduler1, scheduler2], milestones=[warmup_steps])
 
@@ -354,22 +367,22 @@
     # find out the minimum max_seq_length required during fine-tuning (saves memory!)
     lengths = [len(d["input_ids"]) for d in data]
     longest_seq_length = max(lengths)
     longest_seq_ix = lengths.index(longest_seq_length)
     return longest_seq_length, longest_seq_ix
 
 
-def save_adapter_v2_checkpoint(fabric: L.Fabric, model: torch.nn.Module, file_path: Path) -> None:
-    fabric.print(f"Saving adapter v2 weights to {str(file_path)!r}")
+def save_adapter_checkpoint(fabric: L.Fabric, model: torch.nn.Module, file_path: Path) -> None:
+    fabric.print(f"Saving adapter weights to {str(file_path)!r}")
     fabric.save(file_path, {"model": model}, filter={"model": adapter_filter})
 
 
 def validate_args(train: TrainArgs, eval: EvalArgs) -> None:
     issues = []
-    unsupported = [(train, ["max_tokens", "max_norm", "tie_embeddings"])]
+    unsupported = [(train, ["max_tokens", "max_norm", "tie_embeddings", "lr_warmup_fraction"])]
     for args, names in unsupported:
         for name in names:
             if getattr(args, name) is not None:
                 issues.append(f"{__file__} doesn't support the {name!r} argument. This is set in {args}")
     required = [(train, ["epochs"]), (eval, ["max_new_tokens"])]
     for args, names in required:
         for name in names:
```

### Comparing `litgpt-0.2.0.dev0/litgpt/finetune/full.py` & `litgpt-0.3.0/litgpt/finetune/full.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     CycleIterator,
     check_valid_checkpoint_dir,
     choose_logger,
     chunked_cross_entropy,
     copy_config_files,
     get_default_supported_precision,
     load_checkpoint,
+    init_out_dir,
     num_parameters,
     parse_devices,
     save_hyperparameters,
 )
 
 
 def setup(
@@ -40,45 +41,49 @@
     precision: Optional[str] = None,
     devices: Union[int, str] = 1,
     resume: Union[bool, Path] = False,
     data: Optional[DataModule] = None,
     train: TrainArgs = TrainArgs(
         save_interval=1000,
         log_interval=1,
-        global_batch_size=64,
+        global_batch_size=16,
         micro_batch_size=1,
         lr_warmup_steps=100,
         epochs=5,
         learning_rate=3e-3,
         max_seq_length=None,
     ),
     eval: EvalArgs = EvalArgs(interval=600, max_new_tokens=100, max_iters=100),
     logger_name: Literal["wandb", "tensorboard", "csv"] = "csv",
     seed: int = 1337,
 ) -> None:
     """Finetune a model.
 
     Arguments:
         checkpoint_dir: The path to the base model's checkpoint directory to load for finetuning.
-        out_dir: Directory in which to save checkpoints and logs.
+        out_dir: Directory in which to save checkpoints and logs. If running in a Lightning Studio Job, look for it in
+            /teamspace/jobs/<job-name>/share.
         precision: The precision to use for finetuning. Possible choices: "bf16-true", "bf16-mixed", "32-true".
         devices: How many devices/GPUs to use
         resume: Path to a checkpoint directory to resume from in case training was interrupted, or ``True`` to resume
             from the latest checkpoint in ``out_dir``.
         data: Data-related arguments. If not provided, the default is ``litgpt.data.Alpaca``.
         train: Training-related arguments. See ``litgpt.args.TrainArgs`` for details.
         eval: Evaluation-related arguments. See ``litgpt.args.EvalArgs`` for details.
         logger_name: The name of the logger to send metrics to.
         seed: The random seed to use for reproducibility.
     """
 
     pprint(locals())
     data = Alpaca() if data is None else data
     devices = parse_devices(devices)
-    config = Config.from_name(name=checkpoint_dir.name)
+    out_dir = init_out_dir(out_dir)
+
+    check_valid_checkpoint_dir(checkpoint_dir)
+    config = Config.from_file(checkpoint_dir / "model_config.yaml")
 
     precision = precision or get_default_supported_precision(training=True)
     logger = choose_logger(
         logger_name, out_dir, name=f"finetune-{config.name}", resume=resume, log_interval=train.log_interval
     )
 
     if devices > 1:
@@ -105,15 +110,14 @@
     data: DataModule,
     checkpoint_dir: Path,
     out_dir: Path,
     train: TrainArgs,
     eval: EvalArgs,
 ) -> None:
     validate_args(train, eval)
-    check_valid_checkpoint_dir(checkpoint_dir)
 
     tokenizer = Tokenizer(checkpoint_dir)
     train_dataloader, val_dataloader = get_dataloaders(fabric, data, tokenizer, train)
     steps_per_epoch = len(train_dataloader) // train.gradient_accumulation_iters(devices)
     lr_max_steps = min(train.epochs * steps_per_epoch, (train.max_steps or float("inf")))
 
     fabric.seed_everything(seed)  # same seed for every process to init model (FSDP)
@@ -145,14 +149,20 @@
 
     train_time = time.perf_counter()
     fit(fabric, state, train_dataloader, val_dataloader, devices, resume, checkpoint_dir, out_dir, train, eval, data)
     fabric.print(f"Training time: {(time.perf_counter()-train_time):.2f}s")
     if fabric.device.type == "cuda":
         fabric.print(f"Memory used: {torch.cuda.max_memory_allocated() / 1e9:.02f} GB")
 
+    # Final evaluation
+    val_loss = validate(fabric, model, val_dataloader, dataclasses.replace(eval, max_iters=len(val_dataloader)))
+    metrics = {"val_loss": val_loss, "val_ppl": math.exp(val_loss)}
+    fabric.log_dict(metrics, step=state["iter_num"])
+    fabric.print(f"Final evaluation | val loss: {val_loss.item():.3f} | val ppl: {math.exp(val_loss):.3f}")
+
     # Save the final checkpoint at the end of training
     save_path = out_dir / "final" / "lit_model.pth"
     save_path.parent.mkdir(parents=True, exist_ok=True)
     fabric.save(save_path, {"model": state["model"]})
     if fabric.global_rank == 0:
         # Copy checkpoint files from original checkpoint dir
         copy_config_files(checkpoint_dir, save_path.parent)
@@ -180,15 +190,15 @@
     longest_seq_length, longest_seq_ix = get_longest_seq_length(train_dataloader.dataset)
     model.max_seq_length = min(longest_seq_length, train.max_seq_length or float("inf"))
     fabric.print(
         f"The longest sequence length in the train data is {longest_seq_length}, the model's maximum sequence length is"
         f" {model.max_seq_length} and context length is {model.config.block_size}"
     )
 
-    validate(fabric, model, val_dataloader, tokenizer, dataclasses.replace(eval, max_iters=2), data)  # sanity check
+    validate(fabric, model, val_dataloader, dataclasses.replace(eval, max_iters=2))  # sanity check
     initial_iter = state["iter_num"]
     max_steps = train.max_steps or float("inf")
     train_iterator = CycleIterator(train_dataloader)
 
     # resume data loader state by fast-forwarding through all seen batches
     if resume:
         resume_t0 = time.perf_counter()
@@ -253,15 +263,16 @@
                 f" iter time: {metrics['iter_time'] * 1000:.2f} ms"
                 f"{' (step)' if not is_accumulating else ''}"
             )
             fabric.log_dict(metrics, step=state["iter_num"])
 
         if not is_accumulating and state["step_count"] % eval.interval == 0:
             t0 = time.perf_counter()
-            val_loss = validate(fabric, model, val_dataloader, tokenizer, eval, data)
+            val_loss = validate(fabric, model, val_dataloader, eval)
+            generate_example(fabric, model, tokenizer, eval, data)
             t1 = time.perf_counter() - t0
             fabric.print(f"iter {state['iter_num']}: val loss {val_loss.item():.4f}, val time: {t1 * 1000:.2f} ms")
             metrics = {"val_loss": val_loss, "val_ppl": math.exp(val_loss)}
             fabric.log_dict(metrics, step=state["iter_num"])
             fabric.barrier()
         if train.save_interval is not None and not is_accumulating and state["step_count"] % train.save_interval == 0:
             checkpoint_file = out_dir / f"step-{state['step_count']:06d}" / "lit_model.pth"
@@ -272,47 +283,49 @@
                 copy_config_files(checkpoint_dir, checkpoint_file.parent)
                 save_hyperparameters(setup, checkpoint_file.parent)
                 save_prompt_style(data.prompt_style, checkpoint_file.parent)
 
 
 # FSDP has issues with `inference_mode`
 @torch.no_grad()
-def validate(
-    fabric: L.Fabric, model: GPT, val_dataloader: DataLoader, tokenizer: Tokenizer, eval: EvalArgs, data: DataModule
-) -> torch.Tensor:
+def validate(fabric: L.Fabric, model: GPT, val_dataloader: DataLoader, eval: EvalArgs) -> torch.Tensor:
     fabric.print("Validating ...")
     model.eval()
     losses = torch.zeros(min(len(val_dataloader), eval.max_iters))
     for k, batch in enumerate(val_dataloader):
         if k >= eval.max_iters:
             break
         input_ids, targets = batch["input_ids"], batch["labels"]
         logits = model(input_ids)
         losses[k] = chunked_cross_entropy(logits[..., :-1, :], targets[..., 1:], chunk_size=0)
 
     val_loss = losses.mean()
+    model.train()
+    return val_loss
+
 
-    # produce an example:
+@torch.no_grad()
+def generate_example(fabric: L.Fabric, model: GPT, tokenizer: Tokenizer, eval: EvalArgs, data: DataModule):
     instruction = "Recommend a movie for me to watch during the weekend and explain the reason."
     fabric.print(instruction)
     prompt = data.prompt_style.apply(instruction)
     encoded = tokenizer.encode(prompt, device=fabric.device)
+    model.eval()
+
     with fabric.init_tensor():
         # do not set `max_seq_length=max_returned_token` because memory is not a concern here
         model.set_kv_cache(batch_size=1)
     output = generate(
         model, encoded, max_returned_tokens=len(encoded) + eval.max_new_tokens, temperature=0.8, eos_id=tokenizer.eos_id
     )
     model.clear_kv_cache()
+    model.train()
     output = tokenizer.decode(output)
     fabric.print(output)
 
-    model.train()
-    return val_loss
-
 
 def get_lr_scheduler(optimizer, warmup_steps: int, max_steps: int):
     # linear warmup followed by cosine annealing
     scheduler1 = torch.optim.lr_scheduler.LambdaLR(optimizer, lambda step: step / warmup_steps)
     scheduler2 = torch.optim.lr_scheduler.CosineAnnealingLR(optimizer, T_max=(max_steps - warmup_steps))
     return torch.optim.lr_scheduler.SequentialLR(optimizer, [scheduler1, scheduler2], milestones=[warmup_steps])
 
@@ -336,15 +349,15 @@
     longest_seq_length = max(lengths)
     longest_seq_ix = lengths.index(longest_seq_length)
     return longest_seq_length, longest_seq_ix
 
 
 def validate_args(train: TrainArgs, eval: EvalArgs) -> None:
     issues = []
-    unsupported = [(train, ["max_tokens", "max_norm", "tie_embeddings"])]
+    unsupported = [(train, ["max_tokens", "max_norm", "tie_embeddings", "lr_warmup_fraction"])]
     for args, names in unsupported:
         for name in names:
             if getattr(args, name) is not None:
                 issues.append(f"{__file__} doesn't support the {name!r} argument. This is set in {args}")
     required = [(train, ["epochs"]), (eval, ["max_new_tokens"])]
     for args, names in required:
         for name in names:
```

### Comparing `litgpt-0.2.0.dev0/litgpt/finetune/lora.py` & `litgpt-0.3.0/litgpt/finetune/lora.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     CycleIterator,
     check_valid_checkpoint_dir,
     choose_logger,
     chunked_cross_entropy,
     copy_config_files,
     get_default_supported_precision,
     load_checkpoint,
+    init_out_dir,
     num_parameters,
     parse_devices,
     save_hyperparameters,
 )
 
 
 def setup(
@@ -52,30 +53,31 @@
     lora_projection: bool = False,
     lora_mlp: bool = False,
     lora_head: bool = False,
     data: Optional[DataModule] = None,
     train: TrainArgs = TrainArgs(
         save_interval=1000,
         log_interval=1,
-        global_batch_size=128,
-        micro_batch_size=4,
+        global_batch_size=16,
+        micro_batch_size=1,
         lr_warmup_steps=100,
         epochs=5,
         learning_rate=3e-4,
         max_seq_length=None,
     ),
     eval: EvalArgs = EvalArgs(interval=100, max_new_tokens=100, max_iters=100),
     logger_name: Literal["wandb", "tensorboard", "csv"] = "csv",
     seed: int = 1337,
 ) -> None:
     """Finetune a model using the LoRA method.
 
     Arguments:
         checkpoint_dir: The path to the base model's checkpoint directory to load for finetuning.
-        out_dir: Directory in which to save checkpoints and logs.
+        out_dir: Directory in which to save checkpoints and logs. If running in a Lightning Studio Job, look for it in
+            /teamspace/jobs/<job-name>/share.
         precision: The precision to use for finetuning. Possible choices: "bf16-true", "bf16-mixed", "32-true".
         quantize: If set, quantize the model with this algorithm. See ``tutorials/quantize.md`` for more information.
         devices: How many devices/GPUs to use.
         lora_r: The LoRA rank.
         lora_alpha: The LoRA alpha.
         lora_dropout: The LoRA dropout value.
         lora_query: Whether to apply LoRA to the query weights in attention.
@@ -90,16 +92,19 @@
         logger_name: The name of the logger to send metrics to.
         seed: The random seed to use for reproducibility.
     """
 
     pprint(locals())
     data = Alpaca() if data is None else data
     devices = parse_devices(devices)
-    config = Config.from_name(
-        name=checkpoint_dir.name,
+    out_dir = init_out_dir(out_dir)
+
+    check_valid_checkpoint_dir(checkpoint_dir)
+    config = Config.from_file(
+        checkpoint_dir / "model_config.yaml",
         lora_r=lora_r,
         lora_alpha=lora_alpha,
         lora_dropout=lora_dropout,
         lora_query=lora_query,
         lora_key=lora_key,
         lora_value=lora_value,
         lora_projection=lora_projection,
@@ -146,15 +151,14 @@
     data: DataModule,
     checkpoint_dir: Path,
     out_dir: Path,
     train: TrainArgs,
     eval: EvalArgs,
 ) -> None:
     validate_args(train, eval)
-    check_valid_checkpoint_dir(checkpoint_dir)
 
     tokenizer = Tokenizer(checkpoint_dir)
     train_dataloader, val_dataloader = get_dataloaders(fabric, data, tokenizer, train)
     steps_per_epoch = len(train_dataloader) // train.gradient_accumulation_iters(devices)
     lr_max_steps = min(train.epochs * steps_per_epoch, (train.max_steps or float("inf")))
 
     fabric.seed_everything(seed)  # same seed for every process to init model (FSDP)
@@ -164,15 +168,15 @@
 
     checkpoint_path = checkpoint_dir / "lit_model.pth"
     with fabric.init_module(empty_init=(devices > 1)):
         model = GPT(config)
     mark_only_lora_as_trainable(model)
 
     fabric.print(f"Number of trainable parameters: {num_parameters(model, requires_grad=True):,}")
-    fabric.print(f"Number of non trainable parameters: {num_parameters(model, requires_grad=False):,}")
+    fabric.print(f"Number of non-trainable parameters: {num_parameters(model, requires_grad=False):,}")
 
     model = fabric.setup_module(model)
 
     trainable_params = [p for p in model.parameters() if p.requires_grad]
     if isinstance(fabric.strategy.precision, BitsandbytesPrecision):
         import bitsandbytes as bnb
 
@@ -203,14 +207,20 @@
         eval,
         data,
     )
     fabric.print(f"Training time: {(time.perf_counter()-train_time):.2f}s")
     if fabric.device.type == "cuda":
         fabric.print(f"Memory used: {torch.cuda.max_memory_allocated() / 1e9:.02f} GB")
 
+    # Final evaluation
+    val_loss = validate(fabric, model, val_dataloader, dataclasses.replace(eval, max_iters=len(val_dataloader)))
+    metrics = {"val_loss": val_loss, "val_ppl": math.exp(val_loss)}
+    fabric.log_dict(metrics)
+    fabric.print(f"Final evaluation | val loss: {val_loss.item():.3f} | val ppl: {math.exp(val_loss):.3f}")
+
     # Save the final LoRA checkpoint at the end of training
     save_path = out_dir / "final" / "lit_model.pth.lora"
     save_path.parent.mkdir(parents=True, exist_ok=True)
     save_lora_checkpoint(fabric, model, save_path)
     if fabric.global_rank == 0:
         # Copy checkpoint files from original checkpoint dir
         copy_config_files(checkpoint_dir, save_path.parent)
@@ -237,15 +247,15 @@
     longest_seq_length, longest_seq_ix = get_longest_seq_length(train_dataloader.dataset)
     model.max_seq_length = min(longest_seq_length, train.max_seq_length or float("inf"))
     fabric.print(
         f"The longest sequence length in the train data is {longest_seq_length}, the model's maximum sequence length is"
         f" {model.max_seq_length} and context length is {model.config.block_size}"
     )
 
-    validate(fabric, model, val_dataloader, tokenizer, dataclasses.replace(eval, max_iters=2), data)  # sanity check
+    validate(fabric, model, val_dataloader, dataclasses.replace(eval, max_iters=2))  # sanity check
 
     train_iterator = CycleIterator(train_dataloader)
     throughput = ThroughputMonitor(fabric, window_size=50)
     running_loss = RunningMean(window=train.gradient_accumulation_iters(devices), sync_on_compute=False).to(
         fabric.device
     )
     max_steps = train.max_steps or float("inf")
@@ -304,15 +314,16 @@
                 f" iter time: {metrics['iter_time'] * 1000:.2f} ms"
                 f"{' (step)' if not is_accumulating else ''}"
             )
             fabric.log_dict(metrics, step=iter_num)
 
         if not is_accumulating and step_count % eval.interval == 0:
             t0 = time.perf_counter()
-            val_loss = validate(fabric, model, val_dataloader, tokenizer, eval, data)
+            val_loss = validate(fabric, model, val_dataloader, eval)
+            generate_example(fabric, model, tokenizer, eval, data)
             t1 = time.perf_counter() - t0
             fabric.print(f"iter {iter_num}: val loss {val_loss.item():.4f}, val time: {t1 * 1000:.2f} ms")
             metrics = {"val_loss": val_loss, "val_ppl": math.exp(val_loss)}
             fabric.log_dict(metrics, step=iter_num)
             fabric.barrier()
 
         if train.save_interval is not None and not is_accumulating and step_count % train.save_interval == 0:
@@ -323,47 +334,50 @@
                 copy_config_files(checkpoint_dir, checkpoint_file.parent)
                 save_hyperparameters(setup, checkpoint_file.parent)
                 save_prompt_style(data.prompt_style, checkpoint_file.parent)
 
 
 # FSDP has issues with `inference_mode`
 @torch.no_grad()
-def validate(
-    fabric: L.Fabric, model: GPT, val_dataloader: DataLoader, tokenizer: Tokenizer, eval: EvalArgs, data: DataModule
-) -> torch.Tensor:
+def validate(fabric: L.Fabric, model: GPT, val_dataloader: DataLoader, eval: EvalArgs) -> torch.Tensor:
     fabric.print("Validating ...")
     model.eval()
     losses = torch.zeros(min(len(val_dataloader), eval.max_iters))
     for k, batch in enumerate(val_dataloader):
         if k >= eval.max_iters:
             break
         input_ids, targets = batch["input_ids"], batch["labels"]
         logits = model(input_ids)
         losses[k] = chunked_cross_entropy(logits[..., :-1, :], targets[..., 1:], chunk_size=0)
 
     val_loss = losses.mean()
 
-    # produce an example:
+    model.train()
+    return val_loss
+
+
+@torch.no_grad()
+def generate_example(fabric: L.Fabric, model: GPT, tokenizer: Tokenizer, eval: EvalArgs, data: DataModule):
     instruction = "Recommend a movie for me to watch during the weekend and explain the reason."
     fabric.print(instruction)
     prompt = data.prompt_style.apply(instruction)
     encoded = tokenizer.encode(prompt, device=fabric.device)
+    model.eval()
+
     with fabric.init_tensor():
         # do not set `max_seq_length=max_returned_token` because memory is not a concern here
         model.set_kv_cache(batch_size=1)
     output = generate(
         model, encoded, max_returned_tokens=len(encoded) + eval.max_new_tokens, temperature=0.8, eos_id=tokenizer.eos_id
     )
     model.clear_kv_cache()
+    model.train()
     output = tokenizer.decode(output)
     fabric.print(output)
 
-    model.train()
-    return val_loss
-
 
 def get_lr_scheduler(optimizer, warmup_steps: int, max_steps: int):
     # linear warmup followed by cosine annealing
     scheduler1 = torch.optim.lr_scheduler.LambdaLR(optimizer, lambda step: step / warmup_steps)
     scheduler2 = torch.optim.lr_scheduler.CosineAnnealingLR(optimizer, T_max=(max_steps - warmup_steps))
     return torch.optim.lr_scheduler.SequentialLR(optimizer, [scheduler1, scheduler2], milestones=[warmup_steps])
 
@@ -392,15 +406,15 @@
 def save_lora_checkpoint(fabric: L.Fabric, model: torch.nn.Module, file_path: Path) -> None:
     fabric.print(f"Saving LoRA weights to {str(file_path)!r}")
     fabric.save(file_path, {"model": model}, filter={"model": lora_filter})
 
 
 def validate_args(train: TrainArgs, eval: EvalArgs) -> None:
     issues = []
-    unsupported = [(train, ["max_tokens", "max_norm", "tie_embeddings"])]
+    unsupported = [(train, ["max_tokens", "max_norm", "tie_embeddings", "lr_warmup_fraction"])]
     for args, names in unsupported:
         for name in names:
             if getattr(args, name) is not None:
                 issues.append(f"{__file__} doesn't support the {name!r} argument. This is set in {args}")
     required = [(train, ["epochs"]), (eval, ["max_new_tokens"])]
     for args, names in required:
         for name in names:
```

### Comparing `litgpt-0.2.0.dev0/litgpt/generate/adapter.py` & `litgpt-0.3.0/litgpt/generate/adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 def main(
     prompt: str = "What food do llamas eat?",
     input: str = "",
     adapter_path: Path = Path("out/finetune/adapter/final/lit_model.pth.adapter"),
     checkpoint_dir: Path = Path("checkpoints/stabilityai/stablelm-base-alpha-3b"),
     quantize: Optional[Literal["bnb.nf4", "bnb.nf4-dq", "bnb.fp4", "bnb.fp4-dq", "bnb.int8"]] = None,
     max_new_tokens: int = 100,
-    top_k: Optional[int] = 200,
+    top_k: Optional[int] = 50,
     temperature: float = 0.8,
     precision: Optional[str] = None,
 ) -> None:
     """Generates a response based on a given instruction and an optional input. This script will only work with
     checkpoints from the instruction-tuned adapter model. See ``litgpt.finetune.adapter``.
 
     Args:
@@ -56,15 +56,14 @@
         plugins = BitsandbytesPrecision(quantize[4:], dtype)
         precision = None
 
     fabric = L.Fabric(devices=1, precision=precision, plugins=plugins)
     fabric.launch()
 
     check_valid_checkpoint_dir(checkpoint_dir)
-
     config = Config.from_file(checkpoint_dir / "model_config.yaml")
 
     checkpoint_path = checkpoint_dir / "lit_model.pth"
 
     tokenizer = Tokenizer(checkpoint_dir)
     prompt_style = (
         load_prompt_style(checkpoint_dir) if has_prompt_style(checkpoint_dir) else PromptStyle.from_config(config)
```

### Comparing `litgpt-0.2.0.dev0/litgpt/generate/adapter_v2.py` & `litgpt-0.3.0/litgpt/generate/adapter_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 def main(
     prompt: str = "What food do llamas eat?",
     input: str = "",
     adapter_path: Path = Path("out/finetune/adapter-v2/final/lit_model.pth.adapter_v2"),
     checkpoint_dir: Path = Path("checkpoints/stabilityai/stablelm-base-alpha-3b"),
     quantize: Optional[Literal["bnb.nf4", "bnb.nf4-dq", "bnb.fp4", "bnb.fp4-dq", "bnb.int8"]] = None,
     max_new_tokens: int = 100,
-    top_k: Optional[int] = 200,
+    top_k: Optional[int] = 50,
     temperature: float = 0.8,
     precision: Optional[str] = None,
 ) -> None:
     """Generates a response based on a given instruction and an optional input. This script will only work with
     checkpoints from the instruction-tuned adapter v2 model. See ``litgpt.finetune.adapter_v2``.
 
     Args:
@@ -56,15 +56,14 @@
         plugins = BitsandbytesPrecision(quantize[4:], dtype)
         precision = None
 
     fabric = L.Fabric(devices=1, precision=precision, plugins=plugins)
     fabric.launch()
 
     check_valid_checkpoint_dir(checkpoint_dir)
-
     config = Config.from_file(checkpoint_dir / "model_config.yaml")
 
     checkpoint_path = checkpoint_dir / "lit_model.pth"
 
     tokenizer = Tokenizer(checkpoint_dir)
     prompt_style = (
         load_prompt_style(checkpoint_dir) if has_prompt_style(checkpoint_dir) else PromptStyle.from_config(config)
```

### Comparing `litgpt-0.2.0.dev0/litgpt/generate/base.py` & `litgpt-0.3.0/litgpt/generate/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
 @torch.inference_mode()
 def main(
     prompt: str = "What food do llamas eat?",
     *,
     num_samples: int = 1,
     max_new_tokens: int = 50,
-    top_k: Optional[int] = 200,
+    top_k: Optional[int] = 50,
     temperature: float = 0.8,
     checkpoint_dir: Path = Path("checkpoints/stabilityai/stablelm-base-alpha-3b"),
     quantize: Optional[Literal["bnb.nf4", "bnb.nf4-dq", "bnb.fp4", "bnb.fp4-dq", "bnb.int8"]] = None,
     precision: Optional[str] = None,
     compile: bool = False,
 ) -> None:
     """Generates text samples based on a pre-trained model and tokenizer.
@@ -129,15 +129,14 @@
         dtype = {"16-true": torch.float16, "bf16-true": torch.bfloat16, "32-true": torch.float32}[precision]
         plugins = BitsandbytesPrecision(quantize[4:], dtype)
         precision = None
 
     fabric = L.Fabric(devices=1, precision=precision, plugins=plugins)
 
     check_valid_checkpoint_dir(checkpoint_dir)
-
     config = Config.from_file(checkpoint_dir / "model_config.yaml")
 
     checkpoint_path = checkpoint_dir / "lit_model.pth"
 
     tokenizer = Tokenizer(checkpoint_dir)
     prompt_style = (
         load_prompt_style(checkpoint_dir) if has_prompt_style(checkpoint_dir) else PromptStyle.from_config(config)
```

### Comparing `litgpt-0.2.0.dev0/litgpt/generate/full.py` & `litgpt-0.3.0/litgpt/generate/full.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 def main(
     prompt: str = "What food do llamas eat?",
     input: str = "",
     finetuned_path: Path = Path("out/full/alpaca/lit_model_finetuned.pth"),
     checkpoint_dir: Path = Path("checkpoints/stabilityai/stablelm-base-alpha-3b"),
     quantize: Optional[Literal["bnb.nf4", "bnb.nf4-dq", "bnb.fp4", "bnb.fp4-dq", "bnb.int8"]] = None,
     max_new_tokens: int = 100,
-    top_k: Optional[int] = 200,
+    top_k: Optional[int] = 50,
     temperature: float = 0.8,
     precision: Optional[str] = None,
 ) -> None:
     """Generates a response based on a given instruction and an optional input. This script will only work with
     checkpoints from the instruction-tuned GPT model. See ``litgpt.finetune.full``.
 
     Args:
@@ -55,15 +55,14 @@
         plugins = BitsandbytesPrecision(quantize[4:], dtype)
         precision = None
 
     fabric = L.Fabric(devices=1, precision=precision, plugins=plugins)
     fabric.launch()
 
     check_valid_checkpoint_dir(checkpoint_dir)
-
     config = Config.from_file(checkpoint_dir / "model_config.yaml")
 
     checkpoint_path = finetuned_path
 
     tokenizer = Tokenizer(checkpoint_dir)
     prompt_style = (
         load_prompt_style(checkpoint_dir) if has_prompt_style(checkpoint_dir) else PromptStyle.from_config(config)
```

### Comparing `litgpt-0.2.0.dev0/litgpt/generate/sequentially.py` & `litgpt-0.3.0/litgpt/generate/sequentially.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
 @torch.inference_mode()
 def main(
     prompt: str = "What food do llamas eat?",
     *,
     num_samples: int = 1,
     max_new_tokens: int = 50,
-    top_k: Optional[int] = 200,
+    top_k: Optional[int] = 50,
     temperature: float = 0.8,
     checkpoint_dir: Path = Path("checkpoints/mistralai/Mistral-7B-Instruct-v0.1"),
     quantize: Optional[Literal["bnb.nf4", "bnb.nf4-dq", "bnb.fp4", "bnb.fp4-dq"]] = None,
     precision: Optional[str] = None,
     compile: bool = False,
 ) -> None:
     """Generates text samples based on a pre-trained model and tokenizer.
@@ -154,15 +154,14 @@
 
     fabric = L.Fabric(devices=1, precision=precision, accelerator="cuda", plugins=plugins)
 
     total_devices = CUDAAccelerator.auto_device_count()
     print(f"Using {total_devices} devices", file=sys.stderr)
 
     check_valid_checkpoint_dir(checkpoint_dir)
-
     config = Config.from_file(checkpoint_dir / "model_config.yaml")
 
     checkpoint_path = checkpoint_dir / "lit_model.pth"
 
     tokenizer = Tokenizer(checkpoint_dir)
     encoded = tokenizer.encode(prompt, device=fabric.device)
     prompt_length = encoded.size(0)
```

### Comparing `litgpt-0.2.0.dev0/litgpt/generate/tp.py` & `litgpt-0.3.0/litgpt/generate/tp.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
 @torch.inference_mode()
 def main(
     prompt: str = "What food do llamas eat?",
     *,
     num_samples: int = 1,
     max_new_tokens: int = 50,
-    top_k: Optional[int] = 200,
+    top_k: Optional[int] = 50,
     temperature: float = 0.8,
     checkpoint_dir: Path = Path("checkpoints/stabilityai/stablelm-base-alpha-3b"),
     quantize: Optional[Literal["bnb.nf4", "bnb.nf4-dq", "bnb.fp4", "bnb.fp4-dq"]] = None,
     precision: Optional[str] = None,
     compile: bool = False,
 ) -> None:
     """Generates text samples based on a pre-trained model and tokenizer.
@@ -133,15 +133,14 @@
         precision = None
 
     # set "ddp" as the strategy for the launching functionality, but there's no data-parallelism
     fabric = L.Fabric(devices="auto", strategy="ddp", precision=precision, plugins=plugins)
     fabric.launch()
 
     check_valid_checkpoint_dir(checkpoint_dir)
-
     config = Config.from_file(checkpoint_dir / "model_config.yaml")
 
     model_file = "lit_model.pth"
     checkpoint_path = checkpoint_dir / model_file
 
     tokenizer = Tokenizer(checkpoint_dir)
     encoded = tokenizer.encode(prompt, device=fabric.device)
```

### Comparing `litgpt-0.2.0.dev0/litgpt/lora.py` & `litgpt-0.3.0/litgpt/lora.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,16 +118,16 @@
             lora_dropout: dropout that is applied on the input in the LoRA branch (before multiplying by matrix A)
         """
         super().__init__(r=r, lora_alpha=lora_alpha, lora_dropout=lora_dropout)
         self.linear = torch.nn.Linear(in_features, out_features, **kwargs)
 
         # Actual trainable parameters
         if r > 0:
-            self.lora_A = nn.Parameter(torch.zeros((r, in_features)))
-            self.lora_B = nn.Parameter(torch.zeros((out_features, r)))
+            self.lora_A = nn.Parameter(torch.empty((r, in_features)))
+            self.lora_B = nn.Parameter(torch.empty((out_features, r)))
             self.scaling = self.lora_alpha / self.r
             self.reset_parameters()
 
     def reset_parameters(self) -> None:
         """Reset all the weights, even including pretrained ones."""
         if hasattr(self, "lora_A"):
             # initialize A the same way as the default for nn.Linear and B to zero
@@ -140,35 +140,30 @@
         return (self.lora_B @ self.lora_A) * self.scaling
 
     def merge(self) -> None:
         """Merges the LoRA weights into the full-rank weights (W = W + delta_W)."""
         if self.r > 0 and not self.merged:
             pretrained_dtype = self.linear.weight.data.dtype
             lora_data = self.get_lora_AB()
-            # if the pretrained weights and LoRA weights are of the same dtype - simply sum them
-            if pretrained_dtype == lora_data.dtype:
-                self.linear.weight.data += lora_data
             # if only the pretrained are in quantized form - dequantize, sum with LoRA and quantize the result
-            elif pretrained_dtype == torch.uint8:
+            if pretrained_dtype == torch.uint8:
                 import bitsandbytes as bnb
 
                 weight = self.linear.weight
                 # dequantize the pretrained weights
                 weight_data = bnb.functional.dequantize_4bit(weight.data, weight.quant_state).to(lora_data.dtype)
                 # add pretrained and LoRA weights
                 weight_data += lora_data
                 # assign updated weights and quantize by moving to CUDA device
                 self.linear.weight = bnb.nn.Params4bit(weight_data, requires_grad=False, **weight.__dict__)
                 self.linear.weight.cuda(weight.device)
             else:
-                raise NotImplementedError(
-                    f"Cannot merge the pretrained weights of type {pretrained_dtype}"
-                    f" and LoRA weights of type {lora_data.dtype}"
-                )
-
+                # self.linear might be on CPU and lora_data on CUDA
+                # the inplace add will preserve the dtype of linear.weight
+                self.linear.weight.data += lora_data.to(device=self.linear.weight.data.device)
             self.merged = True
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         # if weights are merged or rank is less or equal to zero (LoRA is disabled) - it's only a regular nn.Linear forward pass;
         # otherwise in addition do the forward pass with LoRA weights and add it's output to the output from pretrained weights
         pretrained = self.linear(x)
         if self.r == 0 or self.merged:
@@ -181,14 +176,15 @@
     # LoRA implemented in a dense layer
     def __init__(
         self,
         # ↓ this part is for pretrained weights
         in_features: int,
         out_features: int,
         # ↓ the remaining part is for LoRA
+        head_size: int,
         n_head: int,
         n_query_groups: int,
         r: int = 0,
         lora_alpha: int = 1,
         lora_dropout: float = 0.0,
         enable_lora: Union[bool, Tuple[bool, bool, bool]] = False,
         **kwargs: Any,
@@ -200,14 +196,15 @@
             2. LoRA A matrix as `self.lora_A`
             3. LoRA B matrix as `self.lora_B`
         Only LoRA's A and B matrices are updated, pretrained weights stay frozen.
 
         Args:
             in_features: number of input features of the pretrained weights
             out_features: number of output features of the pretrained weights
+            head_size: size of a single attention head
             n_head: number of attention heads
             n_query_groups: number of query groups (see diagram in `litgpt/config.py`)
             r: rank of the weight update matrices. To make sense of using LoRA the rank should be smaller than the rank of
                 the weights of the model. The rank can be as low as 1: https://arxiv.org/pdf/2106.09685.pdf (section 7.2)
             lora_alpha: alpha is needed for scaling updates as alpha/r
                 "This scaling helps to reduce the need to retune hyperparameters when we vary r"
                 https://arxiv.org/pdf/2106.09685.pdf (section 4.1)
@@ -228,25 +225,26 @@
         # Actual trainable parameters
         # To better understand initialization let's imagine that we have such parameters:
         # ⚬ in_features: 128 (embeddings_size)
         # ⚬ out_features: 384 (3 * embedding_size)
         # ⚬ r: 2
         # ⚬ enable_lora: [True, False, True]
         if r > 0 and any(enable_lora):
-            self.lora_A = nn.Parameter(torch.zeros((r * sum(enable_lora), in_features)))  # (4, 128)
+            self.lora_A = nn.Parameter(torch.empty((r * sum(enable_lora), in_features)))  # (4, 128)
             enable_q, enable_k, enable_v = enable_lora
-            self.kv_embd_size = self.linear.in_features // (n_head // n_query_groups)
             # qkv_shapes will be used to split a tensor with weights correctly
             qkv_shapes = (
-                self.linear.in_features * enable_q,
-                self.kv_embd_size * enable_k,
-                self.kv_embd_size * enable_v,
+                # if `head_size` is explicitly specified in the config, `n_embd` (or `in_features`)
+                # might not be equal to `head_size * n_head`, thus we use it directly here
+                head_size * n_head * enable_q,
+                head_size * n_query_groups * enable_k,
+                head_size * n_query_groups * enable_v,
             )
             self.qkv_shapes = [s for s in qkv_shapes if s]
-            self.lora_B = nn.Parameter(torch.zeros(sum(self.qkv_shapes), r))  # (256, 2))
+            self.lora_B = nn.Parameter(torch.empty(sum(self.qkv_shapes), r))  # (256, 2))
             # Notes about shapes above
             # - self.lora_A has shape (4, 128): 4 because rank is 2 and LoRA is applied only to two matrices;
             # 128 is the input size of the x (embedding size). (4, 128) and not (128, 4) because later on in
             # F.linear function weights are automatically transposed. In addition conv1d requires channels to
             # be before seq length
             # - self.lora_B has shape (256, 2): 256 because LoRA is applied only to two matrices, so the output is
             # 128*2; 2 tells to have two channels per group for group convolution
@@ -537,14 +535,16 @@
             mask = self.mask_cache.index_select(2, input_pos)
         else:
             cos = self.cos[:T]
             sin = self.sin[:T]
             mask = None
 
         x = self.transformer.wte(idx)  # token embeddings of shape (b, t, n_embd)
+        if self.config.scale_embeddings:
+            x = x * (self.config.n_embd**0.5)
         for block in self.transformer.h:
             x = block(x, cos, sin, mask, input_pos)
         x = self.transformer.ln_f(x)
         if lm_head_chunk_size > 0:
             # chunk the lm head logits to reduce the peak memory used by autograd
             return [self.lm_head(x_i) for x_i in x.split(lm_head_chunk_size, dim=1)]
         return self.lm_head(x)  # (B, T, vocab_size)
@@ -590,14 +590,15 @@
             out_features=shape,
             r=config.lora_r,
             lora_alpha=config.lora_alpha,
             lora_dropout=config.lora_dropout,
             enable_lora=(config.lora_query, config.lora_key, config.lora_value),
             bias=config.bias,
             # for MQA/GQA support
+            head_size=config.head_size,
             n_head=config.n_head,
             n_query_groups=config.n_query_groups,
         )
         # output projection
         # if `head_size` is explicitly specified in the config, `n_emd` might not be equal to `head_size * n_head`
         self.proj = LoRALinear(
             config.head_size * config.n_head,
@@ -682,14 +683,16 @@
             config.n_embd,
             bias=config.bias,
             r=(config.lora_r if config.lora_mlp else 0),
             lora_alpha=config.lora_alpha,
             lora_dropout=config.lora_dropout,
         )
 
+        self.config = config
+
     def _load_from_state_dict(self, state_dict: Dict, prefix: str, *args: Any, **kwargs: Any) -> None:
         """For compatibility with base checkpoints."""
         mapping = {
             "fc_1.weight": "fc_1.linear.weight",
             "fc_1.bias": "fc_1.linear.bias",
             "fc_2.weight": "fc_2.linear.weight",
             "fc_2.bias": "fc_2.linear.bias",
@@ -700,15 +703,15 @@
         super()._load_from_state_dict(state_dict, prefix, *args, **kwargs)
 
 
 class GemmaMLP(LLaMAMLP):
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         x_fc_1 = self.fc_1(x)
         x_fc_2 = self.fc_2(x)
-        x = torch.nn.functional.gelu(x_fc_1) * x_fc_2
+        x = torch.nn.functional.gelu(x_fc_1, approximate=self.config.gelu_approximate) * x_fc_2
         return self.proj(x)
 
 
 class LLaMAMoE(litgpt.model.LLaMAMoE):
     def __init__(self, config: Config) -> None:
         nn.Module.__init__(self)
         self.gate = LoRALinear(
```

### Comparing `litgpt-0.2.0.dev0/litgpt/model.py` & `litgpt-0.3.0/litgpt/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -135,14 +135,20 @@
         for block in self.transformer.h:
             block.attn.kv_cache = None
 
 
 class Block(nn.Module):
     def __init__(self, config: Config) -> None:
         super().__init__()
+        if not config.parallel_residual and config.shared_attention_norm:
+            raise NotImplementedError(
+                "No checkpoint amongst the ones we support uses this configuration"
+                " (non-parallel residual and shared attention norm)."
+            )
+
         self.norm_1 = config.norm_class(config.n_embd, eps=config.norm_eps)
         self.attn = CausalSelfAttention(config)
         self.norm_2 = None if config.shared_attention_norm else config.norm_class(config.n_embd, eps=config.norm_eps)
         self.mlp = config.mlp_class(config)
 
         self.config = config
 
@@ -150,26 +156,38 @@
         self,
         x: torch.Tensor,
         cos: torch.Tensor,
         sin: torch.Tensor,
         mask: Optional[torch.Tensor] = None,
         input_pos: Optional[torch.Tensor] = None,
     ) -> torch.Tensor:
-        n_1 = self.norm_1(x)
-        h = self.attn(n_1, cos, sin, mask, input_pos)
+        """
+        Non-parallel residual       Parallel residual
+           ┌─ x                     ┌─ x ────────────┐             Note: if `shared_attention_norm` is True,
+           │  ↓                     │  ↓             ↓                   the output from `norm_1` is reused
+           │  norm_1                │  norm_1  ───►  norm_2
+           │  ↓                     │  ↓             ↓
+           │  attn                  │  attn          mlp
+           │  ↓                     │  ↓             │
+        ┌─ └► +                     └► + ◄───────────┘
+        │     norm_2
+        │     ↓
+        │     mlp
+        │     ↓
+        └───► +
+        """
+
+        x_normed = self.norm_1(x)
+        attention_output = self.attn(x_normed, cos, sin, mask, input_pos)
+
         if self.config.parallel_residual:
-            n_2 = n_1 if self.config.shared_attention_norm else self.norm_2(x)
-            x = self.mlp(n_2) + h + x
+            x_normed = x_normed if self.config.shared_attention_norm else self.norm_2(x)
+            x = self.mlp(x_normed) + attention_output + x
         else:
-            if self.config.shared_attention_norm:
-                raise NotImplementedError(
-                    "No checkpoint amongst the ones we support uses this configuration"
-                    " (non-parallel residual and shared attention norm)."
-                )
-            x = h + x
+            x = attention_output + x
             x = self.mlp(self.norm_2(x)) + x
         return x
 
 
 class CausalSelfAttention(nn.Module):
     def __init__(self, config: Config) -> None:
         super().__init__()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `litgpt-0.2.0.dev0/litgpt/pretrain.py` & `litgpt-0.3.0/litgpt/pretrain.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
 
 import math
-import os
 import pprint
 import time
 from datetime import timedelta
 from functools import partial
 from pathlib import Path
 from typing import Optional, Tuple, Union
 
@@ -16,24 +15,28 @@
 from lightning.fabric.utilities.throughput import ThroughputMonitor, measure_flops
 from torch.utils.data import DataLoader
 from torchmetrics.aggregation import RunningMean
 from typing_extensions import Literal
 
 from litgpt import Tokenizer
 from litgpt.args import EvalArgs, TrainArgs
+from litgpt.config import name_to_config
 from litgpt.data import DataModule, TinyLlama
 from litgpt.model import GPT, Block, CausalSelfAttention, Config, LLaMAMLP
 from litgpt.utils import (
     CLI,
     CycleIterator,
+    capture_hparams,
     choose_logger,
     chunked_cross_entropy,
     copy_config_files,
+    init_out_dir,
     num_parameters,
     parse_devices,
+    reset_parameters,
     save_config,
     save_hyperparameters,
 )
 
 
 def setup(
     model_name: Optional[str] = None,
@@ -81,20 +84,21 @@
         eval: Evaluation-related arguments. See ``litgpt.args.EvalArgs`` for details.
         devices: How many devices/GPUs to use. Uses all GPUs by default.
         tokenizer_dir: Optional path to the tokenizer dir that was used for preprocessing the dataset. Only some data
             module require this.
         logger_name: The name of the logger to send metrics to.
         seed: The random seed to use for reproducibility.
     """
-    hparams = locals()
+    hparams = capture_hparams()
     data = TinyLlama() if data is None else data
     if model_config is not None and model_name is not None:
         raise ValueError("Only one of `model_name` or `model_config` can be set.")
     elif model_config is None and model_name is None:
-        model_name = "tiny-llama-1.1b"
+        available_models = "\n".join(sorted(name_to_config))
+        raise ValueError(f"Please specify --model_name <model_name>. Available values:\n{available_models}")
     config = Config.from_name(model_name) if model_config is None else model_config
     devices = parse_devices(devices)
     out_dir = init_out_dir(out_dir)
     # in case the dataset requires the Tokenizer
     tokenizer = Tokenizer(tokenizer_dir) if tokenizer_dir is not None else None
 
     logger = choose_logger(
@@ -148,16 +152,16 @@
         out_dir.mkdir(parents=True, exist_ok=True)
 
     fabric.seed_everything(seed)  # same seed for every process to init model (FSDP)
 
     t0 = time.perf_counter()
     with fabric.init_module(empty_init=True):
         model = GPT(config)
-    
-    prepare_weight_initialization(model, n_layer=config.n_layer, n_embd=config.n_embd)
+
+    initialize_weights(fabric, model, n_layer=config.n_layer, n_embd=config.n_embd)
 
     if train.tie_embeddings:
         model.transformer.wte.weight = model.lm_head.weight
     if train.max_seq_length:
         model.max_seq_length = train.max_seq_length
 
     fabric.print(f"Time to instantiate model: {time.perf_counter() - t0:.02f} seconds.")
@@ -192,21 +196,25 @@
         resume = max(out_dir.rglob("step-*/*.pth"), key=(lambda p: int(p.parent.name.split("-")[1])))
     if resume:
         fabric.print(f"Resuming training from {resume}")
         fabric.load(resume, state)
 
     train_time = time.perf_counter()
     fit(fabric, devices, state, train_dataloader, val_dataloader, out_dir, tokenizer_dir, train, eval)
+
+    # Save final checkpoint
+    save_checkpoint(fabric, state, tokenizer_dir, out_dir / "final" / "lit_model.pth")
+
     fabric.print(f"Training time: {(time.perf_counter()-train_time):.2f}s")
     if fabric.device.type == "cuda":
         fabric.print(f"Memory used: {torch.cuda.max_memory_allocated() / 1e9:.02f} GB")
 
 
 def fit(
-    fabric,
+    fabric: L.Fabric,
     devices: int,
     state: dict,
     train_dataloader: DataLoader,
     val_dataloader: DataLoader,
     out_dir: Path,
     tokenizer_dir: Optional[Path],
     train: TrainArgs,
@@ -237,15 +245,16 @@
     running_loss = RunningMean(window=train.gradient_accumulation_iters(devices), sync_on_compute=False).to(
         fabric.device
     )
     fabric.barrier()
     total_t0 = time.perf_counter()
     val_loss = "n/a"
 
-    warmup_iters = train.lr_warmup_steps * train.gradient_accumulation_iters(devices)
+    warmup_iters = train.warmup_iters(devices, max_iters, train_dataloader)
+
     for train_data in train_iterator:
         if state["iter_num"] >= max_iters:
             break
 
         # determine and set the learning rate for this iteration
         lr = get_lr(train.learning_rate, state["iter_num"], warmup_iters, max_iters, train.min_lr)
         for param_group in optimizer.param_groups:
@@ -317,23 +326,15 @@
 
             fabric.print(f"iter {state['iter_num']}: val loss {val_loss:.4f}, val time: {td * 1000:.2f} ms")
             metrics = {"val_loss": val_loss, "val_ppl": math.exp(val_loss)}
             fabric.log_dict(metrics, step=state["iter_num"] - 1)
             fabric.barrier()
 
         if train.save_interval is not None and not is_accumulating and state["step_count"] % train.save_interval == 0:
-            checkpoint_file = out_dir / f"step-{state['step_count']:08d}" / "lit_model.pth"
-            checkpoint_file.parent.mkdir(parents=True, exist_ok=True)
-            fabric.print(f"Saving checkpoint to {str(checkpoint_file)!r}")
-            fabric.save(checkpoint_file, state)
-            if fabric.global_rank == 0:
-                save_hyperparameters(setup, checkpoint_file.parent)
-                if tokenizer_dir is not None:
-                    copy_config_files(tokenizer_dir, checkpoint_file.parent)
-                save_config(model.config, checkpoint_file.parent)
+            save_checkpoint(fabric, state, tokenizer_dir, out_dir / f"step-{state['step_count']:08d}" / "lit_model.pth")
 
 
 @torch.no_grad()
 def validate(fabric: L.Fabric, model: nn.Module, val_dataloader: DataLoader, max_iters: int) -> torch.Tensor:
     fabric.barrier()
     fabric.print("Validating ...")
     model.eval()
@@ -377,15 +378,15 @@
     # 3) in between, use cosine decay down to min learning rate
     decay_ratio = (it - warmup_iters) / (max_iters - warmup_iters)
     assert 0 <= decay_ratio <= 1
     coeff = 0.5 * (1.0 + math.cos(math.pi * decay_ratio))  # coeff ranges 0..1
     return min_lr + coeff * (learning_rate - min_lr)
 
 
-def prepare_weight_initialization(model: GPT, n_layer: int, n_embd: int) -> None:
+def initialize_weights(fabric: L.Fabric, model: GPT, n_layer: int, n_embd: int) -> None:
     """GPT-NeoX weight initialization (https://arxiv.org/abs/2204.06745)."""
     # Adapted from https://github.com/jzhang38/TinyLlama
 
     def init_weights(module, std):
         nn.init.normal_(module.weight, mean=0.0, std=std)
         if getattr(module, "bias", None) is not None:
             nn.init.zeros_(module.bias)
@@ -395,19 +396,28 @@
             mod.reset_parameters = partial(init_weights, mod, std=math.sqrt(2.0 / 5 / n_embd))
 
     # need a separate loop because `mod.proj` below is a `nn.Linear` too
     for mod in model.modules():
         if isinstance(mod, (LLaMAMLP, CausalSelfAttention)):
             mod.proj.reset_parameters = partial(init_weights, mod.proj, std=(1 / math.sqrt(n_embd) / n_layer))
 
+    if not isinstance(fabric.strategy, FSDPStrategy):
+        reset_parameters(model)
+
 
-def init_out_dir(out_dir: Path) -> Path:
-    if not out_dir.is_absolute() and "LIGHTNING_ARTIFACTS_DIR" in os.environ:
-        return Path(os.getenv("LIGHTNING_ARTIFACTS_DIR")) / out_dir
-    return out_dir
+def save_checkpoint(fabric, state, tokenizer_dir, checkpoint_file):
+    model = state["model"]
+    checkpoint_file.parent.mkdir(parents=True, exist_ok=True)
+    fabric.print(f"Saving checkpoint to {str(checkpoint_file)!r}")
+    fabric.save(checkpoint_file, state)
+    if fabric.global_rank == 0:
+        save_hyperparameters(setup, checkpoint_file.parent)
+        if tokenizer_dir is not None:
+            copy_config_files(tokenizer_dir, checkpoint_file.parent)
+        save_config(model.config, checkpoint_file.parent)
 
 
 def validate_args(train: TrainArgs, eval: EvalArgs, initial_checkpoint_dir, resume) -> None:
     issues = []
     unsupported = [(train, ["max_steps", "epochs"]), (eval, ["max_new_tokens"])]
     for args, names in unsupported:
         for name in names:
```

### Comparing `litgpt-0.2.0.dev0/litgpt/prompts.py` & `litgpt-0.3.0/litgpt/prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,32 @@
             " toxic, dangerous, or illegal content. Please ensure that your responses are socially unbiased and"
             " positive in nature.\n\nIf a question does not make any sense, or is not factually coherent, explain why"
             " instead of answering something not correct. If you don't know the answer to a question, please don't"
             f" share false information.{e_sys} {prompt} {e_inst} "
         )
 
 
+class Llama3(PromptStyle):
+    def apply(self, prompt: str, **kwargs: str) -> str:
+        # https://github.com/meta-llama/llama3/blob/359887376f0aaf30e433f23e25df858d8c2a9833/llama/tokenizer.py#L202-L229
+        return (
+            "<|begin_of_text|><|start_header_id|>system<|end_header_id|>\n\n"
+            "You are a helpful assistant.<|eot_id|>\n"  # The system prompt is optional
+            "<|start_header_id|>user<|end_header_id|>\n\n"
+            f"{prompt}<|eot_id|>\n"
+            "<|start_header_id|>assistant<|end_header_id|>\n\n"
+        )
+
+    def stop_tokens(self, tokenizer: "Tokenizer") -> Tuple[List[int], ...]:
+        return (
+            [tokenizer.eos_id],
+            [tokenizer.token_to_id("<|eot_id|>")],
+        )
+
+
 class FreeWilly2(PromptStyle):
     def apply(self, prompt: str, **kwargs: str) -> str:
         return (
             "### System:\nThis is a system prompt, please behave and help the user.\n\n"
             "### User:\n"
             f"{prompt}\n\n"
             "### Assistant:\n"
@@ -247,15 +265,15 @@
             # to stop or else things like code generation wouldn't work
             # [198, 198],  # '\n', '\n'
         )
 
 
 class Phi2(PromptStyle):
     def apply(self, prompt: str, **kwargs: str) -> str:
-        return f"Instruct:{prompt}\nOutput:"
+        return f"Instruct: {prompt}\nOutput:"
 
 
 class TinyLlama(PromptStyle):
     def apply(self, prompt: str, **kwargs: str) -> str:
         return (
             "<|system|>\n"
             "You are a friendly chatbot who always gives helpful, detailed, and polite answers.</s>\n"
@@ -312,44 +330,46 @@
         return Falcon()
     if re.search(r"vicuna|longchat", model_name):
         return Vicuna()
     if re.search("Llama-2-7b-chat-hf-function-calling-v2", model_name):
         return Llama2FunctionCalling()
     if re.search("Llama-2.*-chat", model_name):
         return Llama2()
+    if re.search("Llama-3.*-Instruct", model_name):
+        return Llama3()
     if re.search("FreeWilly2", model_name):
         return FreeWilly2()
     if re.search("Platypus", model_name):
         return Platypus()
     if re.search("Nous-Hermes", model_name):
         return NousResearch()
     if re.search("CodeLlama|Mistral.*Instruct", model_name):
         return CodeLlama()
     if re.search("phi-1", model_name):
         return Phi1()
     if re.search("phi-2", model_name):
         return Phi2()
     if re.search(r"tiny-llama.*chat", model_name):
         return TinyLlama()
-    if re.search(r"Gemma.*-it", model_name):
+    if re.search(r"(Code)?Gemma.*-it", model_name):
         return Gemma()
     return Default()
 
 
 def save_prompt_style(style: Union[str, PromptStyle], checkpoint_dir: Path) -> None:
     style = PromptStyle.from_name(style) if isinstance(style, str) else style
     cls = type(style)
     # Allow saving the full module path for user-defined prompt classes
     config = {"class_path": f"{cls.__module__}.{cls.__name__}"}
-    with open(checkpoint_dir / "prompt_style.yaml", "w") as file:
+    with open(checkpoint_dir / "prompt_style.yaml", "w", encoding="utf-8") as file:
         yaml.dump(config, file)
 
 
 def load_prompt_style(checkpoint_dir: Path) -> PromptStyle:
-    with open(checkpoint_dir / "prompt_style.yaml", "r") as file:
+    with open(checkpoint_dir / "prompt_style.yaml", "r", encoding="utf-8") as file:
         config = yaml.safe_load(file)
     # Support loading the full module path for user-defined prompt classes
     full_module_path, cls_name = config["class_path"].rsplit(".", 1)
     module = importlib.import_module(full_module_path)
     cls = getattr(module, cls_name)
     return cls()
```

### Comparing `litgpt-0.2.0.dev0/litgpt/scripts/convert_hf_checkpoint.py` & `litgpt-0.3.0/litgpt/scripts/convert_hf_checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,15 +288,24 @@
 @torch.inference_mode()
 def convert_hf_checkpoint(
     *,
     checkpoint_dir: Path = Path("checkpoints/stabilityai/stablelm-base-alpha-3b"),
     model_name: Optional[str] = None,
     dtype: Optional[str] = None,
 ) -> None:
-    """Convert a Hugging Face Transformers checkpoint into a LitGPT compatible checkpoint."""
+    """
+    Convert a Hugging Face Transformers checkpoint into a LitGPT compatible checkpoint.
+
+    Arguments:
+        checkpoint_dir: Where to save the downloaded files.
+        model_name: The existing config name to load. This is useful to download alternative weights of existing
+            architectures.
+        dtype: The data type to convert the checkpoint files to. If not specified, the weights will remain in the
+            dtype they are downloaded in.
+    """
     if model_name is None:
         model_name = checkpoint_dir.name
     if dtype is not None:
         dtype = getattr(torch, dtype)
 
     config = Config.from_name(model_name)
     save_config(config, checkpoint_dir)
@@ -316,15 +325,15 @@
 
     # initialize a new empty state dict to hold our new weights
     sd = {}
 
     # Load the json file containing weight mapping
     pytorch_bin_map_json_path = checkpoint_dir / "pytorch_model.bin.index.json"
     if pytorch_bin_map_json_path.is_file():  # not all checkpoints have this file
-        with open(pytorch_bin_map_json_path) as json_map:
+        with open(pytorch_bin_map_json_path, encoding="utf-8") as json_map:
             bin_index = json.load(json_map)
         bin_files = {checkpoint_dir / bin for bin in bin_index["weight_map"].values()}
     else:
         bin_files = set(checkpoint_dir.glob("*.bin"))
         # some checkpoints serialize the training arguments
         bin_files = {f for f in bin_files if f.name != "training_args.bin"}
     if not bin_files:
@@ -334,15 +343,15 @@
         # for checkpoints that split the QKV across several files, we need to keep all the bin files
         # open, so we use `ExitStack` to close them all together at the end
         for bin_file in sorted(bin_files):
             print("Processing", bin_file)
             hf_weights = lazy_load(bin_file)
             copy_fn(sd, hf_weights, saver=saver, dtype=dtype)
         gc.collect()
-        print("Saving converted checkpoint")
+        print(f"Saving converted checkpoint to {checkpoint_dir}")
         saver.save(sd)
 
 
 if __name__ == "__main__":
     from jsonargparse import CLI
 
     CLI(convert_hf_checkpoint)
```

### Comparing `litgpt-0.2.0.dev0/litgpt/scripts/convert_lit_checkpoint.py` & `litgpt-0.3.0/litgpt/scripts/convert_lit_checkpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
     return q, k, v
 
 
 def check_conversion_supported(lit_weights: Dict[str, torch.Tensor]) -> None:
     if any("lora" in wn for wn in lit_weights):
         raise ValueError("Checkpoints with LoRA weights cannot be converted. Call `scripts/merge_lora.py` first.")
     if any("adapter" in wn or "gating_factor" in wn for wn in lit_weights):
-        raise NotImplementedError("Converting adapter models is supported.")
+        raise NotImplementedError("Converting adapter models is not supported.")
 
 
 @torch.inference_mode()
 def convert_lit_checkpoint(checkpoint_dir: Path, output_dir: Path) -> None:
     """Convert a LitGPT trained checkpoint into a Hugging Face Transformers checkpoint."""
     config = Config.from_file(checkpoint_dir / "model_config.yaml")
```

### Comparing `litgpt-0.2.0.dev0/litgpt/scripts/convert_pretrained_checkpoint.py` & `litgpt-0.3.0/litgpt/scripts/convert_pretrained_checkpoint.py`

 * *Files identical despite different names*

### Comparing `litgpt-0.2.0.dev0/litgpt/scripts/download.py` & `litgpt-0.3.0/litgpt/scripts/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,33 +18,36 @@
 def download_from_hub(
     repo_id: Optional[str] = None,
     access_token: Optional[str] = os.getenv("HF_TOKEN"),
     tokenizer_only: bool = False,
     convert_checkpoint: bool = True,
     dtype: Optional[str] = None,
     checkpoint_dir: Path = Path("checkpoints"),
+    model_name: Optional[str] = None,
 ) -> None:
     """Download weights or tokenizer data from the Hugging Face Hub.
 
     Arguments:
         repo_id: The repository ID in the format ``org/name`` or ``user/name`` as shown in Hugging Face.
         access_token: Optional API token to access models with restrictions.
         tokenizer_only: Whether to download only the tokenizer files.
         convert_checkpoint: Whether to convert the checkpoint files to the LitGPT format after downloading.
         dtype: The data type to convert the checkpoint files to. If not specified, the weights will remain in the
             dtype they are downloaded in.
         checkpoint_dir: Where to save the downloaded files.
+        model_name: The existing config name to use for this repo_id. This is useful to download alternative weights of
+            existing architectures.
     """
 
     if repo_id is None:
         from litgpt.config import configs
 
         options = [f"{config['hf_config']['org']}/{config['hf_config']['name']}" for config in configs]
         print("Please specify --repo_id <repo_id>. Available values:")
-        print("\n".join(options))
+        print("\n".join(sorted(options, key=lambda x: x.lower())))
         return
 
     from huggingface_hub import snapshot_download
 
     download_files = ["tokenizer*", "generation_config.json", "config.json"]
     from_safetensors = False
     if not tokenizer_only:
@@ -97,15 +100,15 @@
                 raise RuntimeError(f"{safetensor_path} is likely corrupted. Please try to re-download it.") from e
             print(f"{safetensor_path} --> {bin_path}")
             torch.save(result, bin_path)
             os.remove(safetensor_path)
 
     if convert_checkpoint and not tokenizer_only:
         print("Converting checkpoint files to LitGPT format.")
-        convert_hf_checkpoint(checkpoint_dir=directory, dtype=dtype)
+        convert_hf_checkpoint(checkpoint_dir=directory, dtype=dtype, model_name=model_name)
 
 
 def find_weight_files(repo_id: str, access_token: Optional[str]) -> Tuple[List[str], List[str]]:
     from huggingface_hub import repo_info
     from huggingface_hub.utils import filter_repo_objects
 
     with gated_repo_catcher(repo_id):
@@ -119,16 +122,16 @@
 @contextmanager
 def gated_repo_catcher(repo_id: str):
     try:
         yield
     except OSError as e:
         if "gated repo" in str(e):
             raise ValueError(
-                f"{repo_id} requires authentication, please set the `HF_TOKEN=your_token` environment"
-                " variable or pass --access_token=your_token. You can find your token by visiting"
+                f"https://huggingface.co/{repo_id} requires authentication, please set the `HF_TOKEN=your_token`"
+                " environment variable or pass --access_token=your_token. You can find your token by visiting"
                 " https://huggingface.co/settings/tokens"
             )
         raise e
 
 
 if __name__ == "__main__":
     CLI(download_from_hub)
```

### Comparing `litgpt-0.2.0.dev0/litgpt/scripts/merge_lora.py` & `litgpt-0.3.0/litgpt/scripts/merge_lora.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,54 +5,54 @@
 from typing import Any, Dict, Optional, Tuple
 
 import lightning as L
 import torch
 import yaml
 
 from litgpt.lora import GPT, Config, lora_filter, merge_lora_weights
-from litgpt.utils import CLI, check_valid_checkpoint_dir, lazy_load
+from litgpt.utils import CLI, check_valid_checkpoint_dir
 
 
 def merge_lora(
     checkpoint_dir: Path, pretrained_checkpoint_dir: Optional[Path] = None, precision: Optional[str] = None
 ) -> None:
     """Merges the LoRA weights with the base model. See ``litgpt finetune lora``.
 
     Creates a new ``lit_model.pth`` file by merging the LoRA weights (``lit_model.pth.lora``)
     with the original checkpoint weights.
 
     Args:
         checkpoint_dir: Path to the checkpoint directory with trained LoRA weights, which is the output of
-            ``litgpt finetune --method lora``.
+            ``litgpt finetune lora``.
         pretrained_checkpoint_dir: Optional path to the checkpoint directory with the weights of the base model
             corresponding to the LoRA checkpoint. By default, this will automatically be inferred from the metadata
             in the given `checkpoint_dir` directory. Only set this if the base model's checkpoint directory
             has moved or was renamed.
         precision: Optional precision setting to instantiate the model weights in. By default, this will
             automatically be inferred from the metadata in the given ``checkpoint_dir`` directory.
     """
-    check_valid_checkpoint_dir(checkpoint_dir, lora=True)
+    check_valid_checkpoint_dir(checkpoint_dir, model_filename="lit_model.pth.lora")
     if pretrained_checkpoint_dir is not None:
         check_valid_checkpoint_dir(pretrained_checkpoint_dir)
     if (checkpoint_dir / "lit_model.pth").is_file():
         print("LoRA weights have already been merged in this checkpoint.")
         return
 
     lora_params, pretrained_checkpoint_dir, lora_precision = load_lora_metadata(checkpoint_dir)
     precision = precision if precision is not None else lora_precision
 
     fabric = L.Fabric(devices=1, precision=precision, accelerator="cpu")
     config = Config.from_file(checkpoint_dir / "model_config.yaml", **lora_params)
 
-    with fabric.init_module(empty_init=True):
+    with fabric.init_module():
         model = GPT(config)
 
     lora_path = checkpoint_dir / "lit_model.pth.lora"
-    pretrained_checkpoint = lazy_load(pretrained_checkpoint_dir / "lit_model.pth")
-    lora_checkpoint = lazy_load(lora_path)
+    pretrained_checkpoint = torch.load(str(pretrained_checkpoint_dir / "lit_model.pth"), mmap=True)
+    lora_checkpoint = torch.load(str(lora_path), mmap=True)
 
     # Merge LoRA weights into the base model
     pretrained_checkpoint.update(lora_checkpoint.get("model", lora_checkpoint))
     model.load_state_dict(pretrained_checkpoint)
     merge_lora_weights(model)
 
     # Remove LoRA parameters and the LoRA linear substring
@@ -68,15 +68,15 @@
     if not hparams_file.is_file():
         raise FileNotFoundError(
             f"The path {str(hparams_file)!r} is not a valid checkpoint directory. It is missing a"
             f" `hyperparameters.yaml` file. Please point to the checkpoint directory that was produced by"
             f" the `litgpt/finetune/lora.py` script."
         )
 
-    with open(hparams_file, "r") as file:
+    with open(hparams_file, "r", encoding="utf-8") as file:
         hparams = yaml.safe_load(file)
 
     lora_params = {k: v for k, v in hparams.items() if k.startswith("lora_")}
     pretrained_checkpoint_dir = Path(hparams["checkpoint_dir"])
     precision = hparams.get("precision")
     return lora_params, pretrained_checkpoint_dir, precision
```

### Comparing `litgpt-0.2.0.dev0/litgpt/tokenizer.py` & `litgpt-0.3.0/litgpt/tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,22 +29,22 @@
         elif (vocabulary_path := checkpoint_dir / "tokenizer.json").is_file():
             from tokenizers import Tokenizer as HFTokenizer
 
             self.processor = HFTokenizer.from_file(str(vocabulary_path))
             self.backend = "huggingface"
 
             if (special_tokens_path := checkpoint_dir / "tokenizer_config.json").is_file():
-                with open(special_tokens_path) as fp:
+                with open(special_tokens_path, encoding="utf-8") as fp:
                     config = json.load(fp)
                 bos_token = config.get("bos_token")
                 self.bos_id = self.token_to_id(bos_token) if bos_token is not None else None
                 eos_token = config.get("eos_token")
                 self.eos_id = self.token_to_id(eos_token) if eos_token is not None else None
             if (special_tokens_path := checkpoint_dir / "generation_config.json").is_file():
-                with open(special_tokens_path) as fp:
+                with open(special_tokens_path, encoding="utf-8") as fp:
                     config = json.load(fp)
                 if self.bos_id is None:
                     self.bos_id = config.get("bos_token_id")
                 if self.eos_id is None:
                     self.eos_id = config.get("eos_token_id")
         else:
             raise NotImplementedError
@@ -67,21 +67,21 @@
         if id_ is None:
             raise ValueError(f"token {token!r} not found in the collection.")
         return id_
 
     def check_if_bos_token_used(self, checkpoint_dir: Path) -> bool:
         if not (tokenizer_config_path := checkpoint_dir / "tokenizer_config.json").is_file():
             return False
-        with open(tokenizer_config_path) as fp:
+        with open(tokenizer_config_path, encoding="utf-8") as fp:
             config = json.load(fp)
-        if any(config.get(check, False) for check in ("add_bos_token", "add_prefix_space")):
-            return True
-        # for examples that also use the Llama tokenizer, but do not have or set add_bos_token to True.
+        if "add_bos_token" in config:
+            return config["add_bos_token"]
+        # if `add_bos_token` isn't in the config file, but LLaMA tokenizer is used - return True.
         # ex: https://huggingface.co/stabilityai/StableBeluga2/blob/main/tokenizer_config.json#L2
-        return config.get("add_bos_token") is None and config.get("tokenizer_class") == "LlamaTokenizer"
+        return config.get("tokenizer_class") == "LlamaTokenizer"
 
     def encode(
         self,
         string: str,
         device: Optional[torch.device] = None,
         bos: Optional[bool] = None,
         eos: bool = False,
```

### Comparing `litgpt-0.2.0.dev0/litgpt/utils.py` & `litgpt-0.3.0/litgpt/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
 
 """Utility functions for training and inference."""
+import inspect
 import math
+import os
 import pickle
 import shutil
 import sys
-from dataclasses import asdict
+from dataclasses import asdict, is_dataclass
 from io import BytesIO
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Literal, Mapping, Optional, TypeVar, Union
 
 import lightning as L
 import torch
 import torch.nn as nn
@@ -22,14 +24,20 @@
 from torch.serialization import normalize_storage_type
 from typing_extensions import Self
 
 if TYPE_CHECKING:
     from litgpt import GPT, Config
 
 
+def init_out_dir(out_dir: Path) -> Path:
+    if not out_dir.is_absolute() and "LIGHTNING_ARTIFACTS_DIR" in os.environ:
+        return Path(os.getenv("LIGHTNING_ARTIFACTS_DIR")) / out_dir
+    return out_dir
+
+
 def find_multiple(n: int, k: int) -> int:
     assert k > 0
     if n % k == 0:
         return n
     return n + k - (n % k)
 
 
@@ -41,16 +49,22 @@
                 # bitsandbytes 4bit layer support
                 total += math.prod(p.quant_state.shape)
             else:
                 total += p.numel()
     return total
 
 
-def check_valid_checkpoint_dir(checkpoint_dir: Path, lora: bool = False) -> None:
-    model_filename = "lit_model.pth.lora" if lora else "lit_model.pth"
+def reset_parameters(module: nn.Module) -> None:
+    """Calls `reset_parameters` on the module and all its submodules."""
+    for mod in module.modules():
+        if callable(getattr(mod, "reset_parameters", None)):
+            mod.reset_parameters()
+
+
+def check_valid_checkpoint_dir(checkpoint_dir: Path, model_filename: str = "lit_model.pth") -> None:
     files = {
         model_filename: (checkpoint_dir / model_filename).is_file(),
         "model_config.yaml": (checkpoint_dir / "model_config.yaml").is_file(),
         "tokenizer.json OR tokenizer.model": (checkpoint_dir / "tokenizer.json").is_file()
         or (checkpoint_dir / "tokenizer.model").is_file(),
         "tokenizer_config.json": (checkpoint_dir / "tokenizer_config.json").is_file(),
     }
@@ -394,14 +408,29 @@
     set_config_read_mode(urls_enabled=True)
 
     kwargs.setdefault("as_positional", False)
 
     return CLI(*args, **kwargs)
 
 
+def capture_hparams() -> Dict[str, Any]:
+    """Captures the local variables ('hyperparameters') from where this function gets called."""
+    caller_frame = inspect.currentframe().f_back
+    locals_of_caller = caller_frame.f_locals
+    hparams = {}
+    for name, value in locals_of_caller.items():
+        if value is None or isinstance(value, (int, float, str, bool, Path)):
+            hparams[name] = value
+        elif is_dataclass(value):
+            hparams[name] = asdict(value)
+        else:
+            hparams[name] = str(value)
+    return hparams
+
+
 def save_hyperparameters(function: callable, checkpoint_dir: Path) -> None:
     """Captures the CLI parameters passed to `function` without running `function` and saves them to the checkpoint."""
     from jsonargparse import capture_parser
 
     # TODO: Make this more robust
     # This hack strips away the subcommands from the top-level CLI
     # to parse the file as if it was called as a script
@@ -420,15 +449,15 @@
     parser = capture_parser(lambda: CLI(function))
     config = parser.parse_args()
     parser.save(config, checkpoint_dir / "hyperparameters.yaml", overwrite=True)
 
 
 def save_config(config: "Config", checkpoint_dir: Path) -> None:
     config_dict = asdict(config)
-    with open(checkpoint_dir / "model_config.yaml", "w") as fp:
+    with open(checkpoint_dir / "model_config.yaml", "w", encoding="utf-8") as fp:
         yaml.dump(config_dict, fp)
 
 
 def parse_devices(devices: Union[str, int]) -> int:
     if devices in (-1, "auto"):
         return torch.cuda.device_count() or 1
     if isinstance(devices, int) and devices > 0:
```

### Comparing `litgpt-0.2.0.dev0/litgpt.egg-info/PKG-INFO` & `litgpt-0.3.0/litgpt.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litgpt
-Version: 0.2.0.dev0
+Version: 0.3.0
 Summary: Hackable implementation of state-of-the-art open-source LLMs
 Author-email: Lightning AI <contact@lightning.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -206,201 +206,397 @@
            limitations under the License.
         
 Project-URL: homepage, https://github.com/lightning-AI/litgpt
 Project-URL: documentation, https://github.com/lightning-AI/litgpt/tutorials
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=2.2.0
-Requires-Dist: lightning==2.3.0.dev20240318
+Requires-Dist: lightning==2.3.0.dev20240328
 Requires-Dist: jsonargparse[signatures]>=4.27.6
+Requires-Dist: litserve>=0.1.0
 Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-rerunfailures; extra == "test"
-Requires-Dist: pytest-timeout; extra == "test"
+Requires-Dist: pytest>=8.1.1; extra == "test"
+Requires-Dist: pytest-rerunfailures>=14.0; extra == "test"
+Requires-Dist: pytest-timeout>=2.3.1; extra == "test"
 Requires-Dist: transformers>=4.38.0; extra == "test"
-Requires-Dist: einops; extra == "test"
-Requires-Dist: protobuf; extra == "test"
+Requires-Dist: einops>=0.7.0; extra == "test"
+Requires-Dist: protobuf>=4.23.4; extra == "test"
+Requires-Dist: lightning-thunder==0.2.0.dev20240404; python_version >= "3.10" and extra == "test"
 Provides-Extra: all
 Requires-Dist: bitsandbytes==0.42.0; extra == "all"
-Requires-Dist: sentencepiece; extra == "all"
-Requires-Dist: tokenizers; extra == "all"
-Requires-Dist: datasets; extra == "all"
-Requires-Dist: requests; extra == "all"
-Requires-Dist: litdata; extra == "all"
-Requires-Dist: zstandard; extra == "all"
-Requires-Dist: pandas; extra == "all"
-Requires-Dist: pyarrow; extra == "all"
-Requires-Dist: tensorboard; extra == "all"
-Requires-Dist: torchmetrics; extra == "all"
+Requires-Dist: sentencepiece>=0.2.0; extra == "all"
+Requires-Dist: tokenizers>=0.15.2; extra == "all"
+Requires-Dist: requests>=2.31.0; extra == "all"
+Requires-Dist: litdata>=0.2.2; extra == "all"
+Requires-Dist: zstandard>=0.22.0; extra == "all"
+Requires-Dist: pandas>=1.9.0; extra == "all"
+Requires-Dist: pyarrow>=15.0.2; extra == "all"
+Requires-Dist: tensorboard>=2.14.0; extra == "all"
+Requires-Dist: torchmetrics>=1.3.1; extra == "all"
+Requires-Dist: datasets>=2.18.0; extra == "all"
+Requires-Dist: transformers>=4.38.0; extra == "all"
+Requires-Dist: lm-eval>=0.4.2; extra == "all"
+Requires-Dist: safetensors>=0.4.3; extra == "all"
 Requires-Dist: huggingface_hub[hf_transfer]>=0.21.0; extra == "all"
 
 <div align="center">
-<img src="https://pl-public-data.s3.amazonaws.com/assets_lightning/LitStableLM_Badge.png" alt="LitGPT" width="128"/>
 
-# ⚡ LitGPT
-
-<!--
-<p align="center">
-  <a href="https://www.lightning.ai/">Lightning.ai</a> •
-  <a href="https://lightning.ai/docs/pytorch/stable/">PyTorch Lightning</a> •
-  <a href="https://lightning.ai/docs/fabric/stable/">Fabric</a>
-</p>
--->
-
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytorch-lightning)
-![cpu-tests](https://github.com/lightning-AI/lit-stablelm/actions/workflows/cpu-tests.yml/badge.svg) [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/lit-stablelm/blob/master/LICENSE) [![Discord](https://img.shields.io/discord/1077906959069626439?style=plastic)](https://discord.gg/VptPCZkGNa)
-
-</div>
 
-&nbsp;
-
-⚡ LitGPT is a hackable [implementation](litgpt/model.py) of state-of-the-art open-source large language models released under the **Apache 2.0 license**.
-
-&nbsp;
-## LitGPT supports
-
-✅ &nbsp;[The latest model weights](tutorials/download_model_weights.md): Gemma, Mistral, Mixtral, Phi 2, Llama 2, Falcon, CodeLlama, and [many more](tutorials/download_model_weights.md).
-
-✅ &nbsp;Optimized and efficient code: Flash Attention v2, multi-GPU support via fully-sharded data parallelism, [optional CPU offloading](tutorials/oom.md#do-sharding-across-multiple-gpus), and [TPU and XLA support](./xla).
+# ⚡ LitGPT
 
-✅ &nbsp;[Pretraining](tutorials/pretraining.md), [finetuning](tutorials/finetune.md), and [inference](tutorials/inference.md) in various precision settings: FP32, FP16, BF16, and FP16/FP32 mixed.
+**Pretrain, finetune, evaluate, and deploy 20+ LLMs on your own data**
 
-✅ &nbsp;[Configuration files](config_hub) for great out-of-the-box performance.
+Uses the latest state-of-the-art techniques:
 
-✅ &nbsp;Efficient finetuning: [LoRA](tutorials/finetune_lora.md), [QLoRA](tutorials/finetune_lora.md), [Adapter](tutorials/finetune_adapter.md), and [Adapter v2](tutorials/finetune_adapter.md).
+✅ flash attention &nbsp; &nbsp;  ✅ fp4/8/16/32 &nbsp; &nbsp;  ✅ LoRA, QLoRA, Adapter (v1, v2) &nbsp; &nbsp;  ✅ FSDP &nbsp; &nbsp;  ✅ 1-1000+ GPUs/TPUs
 
-✅ &nbsp;[Quantization](tutorials/quantize.md): 4-bit floats, 8-bit integers, and double quantization.
+---
 
-✅ &nbsp;[Exporting](https://github.com/Lightning-AI/litgpt/blob/wip/tutorials/convert_lit_models.md) to other popular model weight formats.
 
-✅ &nbsp;Many popular datasets for [pretraining](tutorials/pretrain_tinyllama.md) and [finetuning](tutorials/prepare_dataset.md), and [support for custom datasets](tutorials/prepare_dataset.md#preparing-custom-datasets-for-instruction-finetuning).
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytorch-lightning)
+![cpu-tests](https://github.com/lightning-AI/lit-stablelm/actions/workflows/cpu-tests.yml/badge.svg) [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/lit-stablelm/blob/master/LICENSE) [![Discord](https://img.shields.io/discord/1077906959069626439)](https://discord.gg/VptPCZkGNa)
 
-✅ &nbsp;Readable and easy-to-modify code to experiment with the latest research ideas.
+<p align="center">
+  <a href="https://lightning.ai/">Lightning AI</a> •
+  <a href="#choose-from-20-llms">Models</a> •
+  <a href="#quick-start">Quick start</a> •
+  <a href="#use-an-llm-for-inference">Inference</a> •
+  <a href="#finetune-an-llm">Finetune</a> •
+  <a href="#finetune-an-llm">Pretrain</a> •
+    <a href="#deploy-an-llm">Deploy</a> •
+  <a href="#state-of-the-art-features">Features</a> •
+  <a href="#training-recipes">Training recipes (YAML)</a>
+</p>
 
+</div>
 
 &nbsp;
-<br>
+<img src="https://pl-bolts-doc-images.s3.us-east-2.amazonaws.com/GithubLitGPTDAG2.png" alt="LitGPT steps" width="auto"/>
 &nbsp;
 
-## Project templates
-
-The following [Lightning Studio](https://lightning.ai/lightning-ai/studios) templates provide LitGPT tutorials and projects in reproducible environments with multi-GPU and multi-node support:
-
-
-|                                                                                                                                                                                                                                                                                                                                             |                                                                                                                                                                                                                                                                                                                                                |
-|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| <p align="left">[Prepare the TinyLlama 1T token dataset](https://lightning.ai/lightning-ai/studios/prepare-the-tinyllama-1t-token-dataset) <br> [<img src="https://pl-public-data.s3.amazonaws.com/assets_litgpt/readme/3.webp" width="300"></p>](https://lightning.ai/lightning-ai/studios/prepare-the-tinyllama-1t-token-dataset)         | [Pretrain LLMs - TinyLlama 1.1B](https://lightning.ai/lightning-ai/studios/pretrain-llms-tinyllama-1-1b) <br> <p align="left">[<img src="https://pl-public-data.s3.amazonaws.com/assets_litgpt/readme/4.webp" width="300"></p>](https://lightning.ai/lightning-ai/studios/pretrain-llms-tinyllama-1-1b)                                        |
-| [Continued Pretraining with TinyLlama 1.1B](https://lightning.ai/lightning-ai/studios/continued-pretraining-with-tinyllama-1-1b) <br> <p align="left">[<img src="https://pl-public-data.s3.amazonaws.com/assets_litgpt/readme/1.webp" width="300"></p>](https://lightning.ai/lightning-ai/studios/continued-pretraining-with-tinyllama-1-1b) | [Instruction finetuning - TinyLlama 1.1B LLM](https://lightning.ai/lightning-ai/studios/instruction-finetuning-tinyllama-1-1b-llm) <br> <p align="left">[<img src="https://pl-public-data.s3.amazonaws.com/assets_litgpt/readme/2.webp" width="300"></p>](https://lightning.ai/lightning-ai/studios/instruction-finetuning-tinyllama-1-1b-llm) |
-|                                                                                                                                                                                                                                                                                                                                             |                                                                                                                                                                                                                                                                                                                                                |
+# Finetune, pretrain and deploy LLMs Lightning fast ⚡⚡   
+LitGPT is a command-line tool designed to easily [finetune](#finetune-an-llm), [pretrain](#pretrain-an-llm), [evaluate](#use-an-llm), and [deploy](#deploy-an-llm) [20+ LLMs](#choose-from-20-llms) **on your own data**. It features highly-optimized [training recipes](#training-recipes) for the world's most powerful open-source large language models (LLMs).
 
+We reimplemented all model architectures and training recipes from scratch for 4 reasons:   
 
+1. Remove all abstraction layers and have single file implementations.   
+2. Guarantee Apache 2.0 compliance to enable enterprise use without limits.    
+3. Optimized each model's architectural detail to maximize performance, reduce costs, and speed up training.    
+4. Highly-optimized [recipe configs](#training-recipes) we have tested at enterprise scale.               
+
+---
+
+&nbsp;
+
+# Choose from 20+ LLMs
+LitGPT has 🤯 **custom, from-scratch implementations** of [20+ LLMs](tutorials/download_model_weights.md) without layers of abstraction:   
+
+| Model | Model size | Author | Reference |
+|----|----|----|----|
+| Llama 3 | 8B, 70B | Meta AI | [Meta AI 2024](https://github.com/meta-llama/llama3)                                                                     |
+| Llama 2 | 7B, 13B, 70B | Meta AI | [Touvron et al. 2023](https://arxiv.org/abs/2307.09288)                                                                      |
+| Code Llama | 7B, 13B, 34B, 70B | Meta AI | [Rozière et al. 2023](https://arxiv.org/abs/2308.12950) |
+| Mistral | 7B | Mistral AI | [Mistral website](https://mistral.ai/)                                                                                       |
+| CodeGemma | 7B | Google | [Google Team, Google Deepmind](https://ai.google.dev/gemma/docs/codegemma) |
+| ... | ... | ... | ...   |
+
+<details>
+  <summary>See full list of 20+ LLMs</summary>
+
+&nbsp; 
+
+#### All models
+  
+| Model | Model size | Author | Reference |
+|----|----|----|----|
+| CodeGemma | 7B | Google | [Google Team, Google Deepmind](https://ai.google.dev/gemma/docs/codegemma) |
+| Code Llama | 7B, 13B, 34B, 70B | Meta AI | [Rozière et al. 2023](https://arxiv.org/abs/2308.12950) |
+| Dolly | 3B, 7B, 12B | Databricks | [Conover et al. 2023](https://www.databricks.com/blog/2023/04/12/dolly-first-open-commercially-viable-instruction-tuned-llm) |
+| Falcon | 7B, 40B, 180B | TII UAE | [TII 2023](https://falconllm.tii.ae)                                                                                         |
+| FreeWilly2 (Stable Beluga 2) | 70B | Stability AI | [Stability AI 2023](https://stability.ai/blog/stable-beluga-large-instruction-fine-tuned-models)                             |
+| Function Calling Llama 2 | 7B | Trelis | [Trelis et al. 2023](https://huggingface.co/Trelis/Llama-2-7b-chat-hf-function-calling-v2)                                   |
+| Gemma | 2B, 7B | Google | [Google Team, Google Deepmind](https://storage.googleapis.com/deepmind-media/gemma/gemma-report.pdf)                         |
+| Llama 2 | 7B, 13B, 70B | Meta AI | [Touvron et al. 2023](https://arxiv.org/abs/2307.09288)                                                                      |
+| Llama 3 | 8B, 70B | Meta AI | [Meta AI 2024](https://github.com/meta-llama/llama3)                                                                     |
+| LongChat | 7B, 13B | LMSYS | [LongChat Team 2023](https://lmsys.org/blog/2023-06-29-longchat/)                                                            |
+| Mistral | 7B | Mistral AI | [Mistral website](https://mistral.ai/)                                                                                       |
+| Nous-Hermes | 7B, 13B, 70B | NousResearch | [Org page](https://huggingface.co/NousResearch)                                                                              |
+| OpenLLaMA | 3B, 7B, 13B | OpenLM Research | [Geng & Liu 2023](https://github.com/openlm-research/open_llama)                                                             |
+| Phi | 1.3B, 2.7B | Microsoft Research  | [Li et al. 2023](https://arxiv.org/abs/2309.05463)                                                                           |
+| Platypus | 7B, 13B, 70B |  Lee et al. | [Lee, Hunter, and Ruiz 2023](https://arxiv.org/abs/2308.07317)                                                               |
+| Pythia | {14,31,70,160,410}M, {1,1.4,2.8,6.9,12}B | EleutherAI | [Biderman et al. 2023](https://arxiv.org/abs/2304.01373)                                                                     |
+| RedPajama-INCITE | 3B, 7B | Together | [Together 2023](https://together.ai/blog/redpajama-models-v1)                                                                |
+| StableCode | 3B | Stability AI | [Stability AI 2023](https://stability.ai/blog/stablecode-llm-generative-ai-coding)                                           |
+| StableLM  | 3B, 7B | Stability AI | [Stability AI 2023](https://github.com/Stability-AI/StableLM)                                                                |
+| StableLM Zephyr | 3B | Stability AI | [Stability AI 2023](https://stability.ai/blog/stablecode-llm-generative-ai-coding)                                           |
+| TinyLlama | 1.1B | Zhang et al. | [Zhang et al. 2023](https://github.com/jzhang38/TinyLlama)                                                                   |
+| Vicuna | 7B, 13B, 33B | LMSYS | [Li et al. 2023](https://lmsys.org/blog/2023-03-30-vicuna/)
 
+</details>
 
-
-&nbsp;
-<br>
 &nbsp;
 
+## Install LitGPT
 
-
-## Installing LitGPT
-
-You can install LitGPT with all dependencies (including CLI, quantization, tokenizers for all models, etc.) using the following pip command:
+Install LitGPT with all dependencies (including CLI, quantization, tokenizers for all models, etc.):
 
 ```bash
-pip install 'litgpt[all] @ git+https://github.com/Lightning-AI/litgpt'
+pip install 'litgpt[all]'
 ```
 
-Alternatively, can install litgpt from a cloned GitHub repository:
+<details>
+  <summary>Advanced install options</summary>
+
+&nbsp;
+
+Install from source:
 
 ```bash
 git clone https://github.com/Lightning-AI/litgpt
 cd litgpt
 pip install -e '.[all]'
 ```
+</details>
 
+---
 
 &nbsp;
+# Quick start
+After installing LitGPT, select the model and action you want to take on that model (finetune, pretrain, evaluate, deploy, etc...):    
 
-## Using LitGPT
+```bash
+# ligpt [action] [model]
+litgpt  download  meta-llama/Meta-Llama-3-8B-Instruct
+litgpt  chat      meta-llama/Meta-Llama-3-8B-Instruct
+litgpt  finetune  meta-llama/Meta-Llama-3-8B-Instruct    
+litgpt  pretrain  meta-llama/Meta-Llama-3-8B-Instruct    
+litgpt  serve     meta-llama/Meta-Llama-3-8B-Instruct    
+```
 
+&nbsp;
 
-Below is a minimal example to get started with the LitGPT command line interface (CLI), illustrating how to download and use a model:
+###  Use an LLM for inference
+Use LLMs for inference to test its chatting capabilities, run evaluations, or extract embeddings, etc...     
+Here's an example showing how to use the Mistral 7B LLM.
+
+<a target="_blank" href="https://lightning.ai/lightning-ai/studios/litgpt-chat">
+  <img src="https://pl-bolts-doc-images.s3.us-east-2.amazonaws.com/app-2/studio-badge.svg" alt="Open In Studio"/>
+</a>
 
+&nbsp;    
 
 ```bash
 # 1) Download a pretrained model
 litgpt download --repo_id mistralai/Mistral-7B-Instruct-v0.2
 
 # 2) Chat with the model
 litgpt chat \
   --checkpoint_dir checkpoints/mistralai/Mistral-7B-Instruct-v0.2
 
 >> Prompt: What do Llamas eat?
 ```
 
 For more information, refer to the [download](tutorials/download_model_weights.md) and [inference](tutorials/inference.md) tutorials.
 
-
 &nbsp;
-## Finetuning and pretraining
 
-LitGPT supports [pretraining](tutorials/pretrain_tinyllama.md) and [finetuning](tutorials/finetune.md) to optimize models on excisting or custom datasets. Below is an example showing how to finetune a model with LoRA:
+### Finetune an LLM
+[Finetune](tutorials/finetune.md) a model to specialize it on your own custom dataset:
+
+<a target="_blank" href="https://lightning.ai/lightning-ai/studios/litgpt-finetune">
+  <img src="https://pl-bolts-doc-images.s3.us-east-2.amazonaws.com/app-2/studio-badge.svg" alt="Open In Studio"/>
+</a>
+
+&nbsp; 
 
 ```bash
 # 1) Download a pretrained model
 litgpt download --repo_id microsoft/phi-2
 
 # 2) Finetune the model
-litgpt finetune lora \
+curl -L https://huggingface.co/datasets/ksaw008/finance_alpaca/resolve/main/finance_alpaca.json -o my_custom_dataset.json
+
+litgpt finetune \
   --checkpoint_dir checkpoints/microsoft/phi-2 \
-  --data Alpaca2k \
-  --out_dir out/phi-2-lora
+  --data JSON \
+  --data.json_path my_custom_dataset.json \
+  --data.val_split_fraction 0.1 \
+  --out_dir out/custom-model
 
 # 3) Chat with the model
 litgpt chat \
-  --checkpoint_dir out/phi-2-lora/final
+  --checkpoint_dir out/custom-model/final
 ```
 
 &nbsp;
-## Configuration files for enhanced performance
 
-LitGPT also allows users to use configuration files in YAML format instead of specifying settings via the command line interface and comes with a set of model-specific defaults for good out-of-the-box performance:
+### Pretrain an LLM   
+Train an LLM from scratch on your own data via pretraining:
 
+<a target="_blank" href="https://lightning.ai/lightning-ai/studios/litgpt-pretrain">
+<img src="https://pl-bolts-doc-images.s3.us-east-2.amazonaws.com/app-2/studio-badge.svg"; alt="Open In Studio"/>
+</a>
+
+&nbsp; 
 
 ```bash
-litgpt finetune lora \
-  --config https://github.com/Lightning-AI/litgpt/blob/wip/config_hub/finetune/llama-2-7b/lora.yaml
+mkdir -p custom_texts
+curl https://www.gutenberg.org/cache/epub/24440/pg24440.txt --output custom_texts/book1.txt
+curl https://www.gutenberg.org/cache/epub/26393/pg26393.txt --output custom_texts/book2.txt
+
+# 1) Download a tokenizer
+litgpt download \
+  --repo_id EleutherAI/pythia-160m \
+  --tokenizer_only True
+
+# 2) Pretrain the model
+litgpt pretrain \
+  --model_name pythia-160m \
+  --tokenizer_dir checkpoints/EleutherAI/pythia-160m \
+  --data TextFiles \
+  --data.train_data_path "custom_texts/" \
+  --train.max_tokens 10_000_000 \
+  --out_dir out/custom-model
+
+# 3) Chat with the model
+litgpt chat \
+  --checkpoint_dir out/custom-model/final
 ```
 
-For added convenience, you can also manually override config file setting via the CLI:
+&nbsp;
+
+### Continue pretraining an LLM       
+This is another way of finetuning that specializes an already pretrained model by training on custom data:    
 
 
+<a target="_blank" href="https://lightning.ai/lightning-ai/studios/litgpt-continue-pretraining">
+<img src="https://pl-bolts-doc-images.s3.us-east-2.amazonaws.com/app-2/studio-badge.svg"; alt="Open In Studio"/>
+</a>
+
+&nbsp; 
+
 ```bash
-litgpt finetune lora \
-  --config https://raw.githubusercontent.com/Lightning-AI/litgpt/main/config_hub/finetune/llama-2-7b/lora.yaml \
-  --lora_r 4
+mkdir -p custom_texts
+curl https://www.gutenberg.org/cache/epub/24440/pg24440.txt --output custom_texts/book1.txt
+curl https://www.gutenberg.org/cache/epub/26393/pg26393.txt --output custom_texts/book2.txt
+
+# 1) Download a pretrained model
+litgpt download --repo_id EleutherAI/pythia-160m
+
+# 2) Continue pretraining the model
+litgpt pretrain \
+  --model_name pythia-160m \
+  --tokenizer_dir checkpoints/EleutherAI/pythia-160m \
+  --initial_checkpoint_dir checkpoints/EleutherAI/pythia-160m \
+  --data TextFiles \
+  --data.train_data_path "custom_texts/" \
+  --train.max_tokens 10_000_000 \
+  --out_dir out/custom-model
+
+# 3) Chat with the model
+litgpt chat \
+  --checkpoint_dir out/custom-model/final
 ```
 
-You can browse the available configuration files [here](https://github.com/Lightning-AI/litgpt/tree/main/config_hub).
+&nbsp;
+
+### Deploy an LLM
+Once you're ready to deploy a finetuned LLM, run this command:   
+
+<a target="_blank" href="https://lightning.ai/lightning-ai/studios/litgpt-serve">
+  <img src="https://pl-bolts-doc-images.s3.us-east-2.amazonaws.com/app-2/studio-badge.svg" alt="Open In Studio"/>
+</a>
 
 &nbsp;
 
-> [!TIP]
-> **Run large models on smaller consumer devices:**
-> We support 4-bit quantization (as in QLoRA), (bnb.nf4, bnb.nf4-dq, bnb.fp4, bnb.fp4-dq) and 8-bit quantization (bnb.int8) for inference by following [this guide](tutorials/quantize.md).
+```bash
+# locate the checkpoint to your finetuned or pretrained model and call the `serve` command:  
+litgpt serve --checkpoint_dir path/to/your/checkpoint/microsoft/phi-2
+
+# Alternative: if you haven't finetuned, download any checkpoint to deploy it:     
+litgpt download --repo_id microsoft/phi-2
+litgpt serve --checkpoint_dir checkpoints/microsoft/phi-2
+```
 
+Test the server in a separate terminal and integrate the model API into your AI product:    
+```python
+# 3) Use the server (in a separate session)
+import requests, json
+ response = requests.post(
+     "http://127.0.0.1:8000/predict", 
+     json={"prompt": "Fix typos in the following sentence: Exampel input"}
+)
+print(response.json()["output"])
+```
 
 &nbsp;
-<br>
+
+> [!NOTE]
+> **[Read the full docs](tutorials/0_to_litgpt.md)**.
+
+&nbsp;
+
+----
+
+# State-of-the-art features
+✅ &nbsp;State-of-the-art optimizations: Flash Attention v2, multi-GPU support via fully-sharded data parallelism, [optional CPU offloading](tutorials/oom.md#do-sharding-across-multiple-gpus), and [TPU and XLA support](extensions/xla).
+
+✅ &nbsp;[Pretrain](tutorials/pretrain.md), [finetune](tutorials/finetune.md), and [deploy](tutorials/inference.md)
+
+✅ &nbsp;Reduce compute requirements with low-precision settings: FP16, BF16, and FP16/FP32 mixed.
+
+✅ &nbsp;Lower memory requirements with [quantization](tutorials/quantize.md): 4-bit floats, 8-bit integers, and double quantization.
+
+✅ &nbsp;[Configuration files](config_hub) for great out-of-the-box performance.
+
+✅ &nbsp;Parameter-efficient finetuning: [LoRA](tutorials/finetune_lora.md), [QLoRA](tutorials/finetune_lora.md), [Adapter](tutorials/finetune_adapter.md), and [Adapter v2](tutorials/finetune_adapter.md).
+
+✅ &nbsp;[Exporting](tutorials/convert_lit_models.md) to other popular model weight formats.
+
+✅ &nbsp;Many popular datasets for [pretraining](tutorials/pretrain.md) and [finetuning](tutorials/prepare_dataset.md), and [support for custom datasets](tutorials/prepare_dataset.md#preparing-custom-datasets-for-instruction-finetuning).
+
+✅ &nbsp;Readable and easy-to-modify code to experiment with the latest research ideas.
+
 &nbsp;
 
-## Customization
+---
+
+# Training recipes
 
-LitGPT supports rich and customizable [config files](config_hub) to tailor the LLM training to your dataset and hardware needs. Shown below is a configuration file for LoRA finetuning:
+LitGPT comes with validated recipes (YAML configs) to train models under different conditions.  We've generated these recipes based on the parameters we found to perform the best for different training conditions.
+
+Browse all training recipes [here](config_hub).
+
+### Example
+
+```bash
+litgpt finetune \
+  --config https://raw.githubusercontent.com/Lightning-AI/litgpt/main/config_hub/finetune/llama-2-7b/lora.yaml
+```
+
+### What is a config
+Configs let you customize training for all granular parameters like:
+
+```yaml
+# The path to the base model's checkpoint directory to load for finetuning. (type: <class 'Path'>, default: checkpoints/stabilityai/stablelm-base-alpha-3b)
+checkpoint_dir: checkpoints/meta-llama/Llama-2-7b-hf
+
+# Directory in which to save checkpoints and logs. (type: <class 'Path'>, default: out/lora)
+out_dir: out/finetune/qlora-llama2-7b
+
+# The precision to use for finetuning. Possible choices: "bf16-true", "bf16-mixed", "32-true". (type: Optional[str], default: null)
+precision: bf16-true
+
+...
+```
+
+<details>
+  <summary>Example: LoRA finetuning config</summary>
+
+&nbsp;
 
 ```yaml
 # The path to the base model's checkpoint directory to load for finetuning. (type: <class 'Path'>, default: checkpoints/stabilityai/stablelm-base-alpha-3b)
 checkpoint_dir: checkpoints/meta-llama/Llama-2-7b-hf
 
 # Directory in which to save checkpoints and logs. (type: <class 'Path'>, default: out/lora)
 out_dir: out/finetune/qlora-llama2-7b
@@ -518,33 +714,29 @@
 
 # The name of the logger to send metrics to. (type: Literal['wandb', 'tensorboard', 'csv'], default: csv)
 logger_name: csv
 
 # The random seed to use for reproducibility. (type: int, default: 1337)
 seed: 1337
 ```
+</details>
 
+### Override config params via CLI
+Override any parameter in the CLI:
 
-&nbsp;
-
-## LitGPT design principles
-
-This repository follows the main principle of **openness through clarity**.
-
-**LitGPT** is:
-
-- **Simple:** Single-file implementation without boilerplate.
-- **Correct:** Numerically equivalent to the original model.
-- **Optimized:** Runs fast on consumer hardware or at scale.
-- **Open-source:** No strings attached.
-
-Avoiding code duplication is **not** a goal. **Readability** and **hackability** are.
+```bash
+litgpt finetune \
+  --config https://raw.githubusercontent.com/Lightning-AI/litgpt/main/config_hub/finetune/llama-2-7b/lora.yaml \
+  --lora_r 4
+```
 
 &nbsp;
 
+# Community        
+
 ## Get involved!
 
 We appreciate your feedback and contributions. If you have feature requests, questions, or want to contribute code or config files, please don't hesitate to use the [GitHub Issue](https://github.com/Lightning-AI/litgpt/issues) tracker.
 
 We welcome all individual contributors, regardless of their level of experience or hardware. Your contributions are valuable, and we are excited to see what you can accomplish in this collaborative and supportive environment.
 
 &nbsp;
@@ -555,35 +747,37 @@
 If you have general questions about building with LitGPT, please [join our Discord](https://discord.gg/VptPCZkGNa).
 
 
 &nbsp;
 
 ## Tutorials, how-to guides, and docs
 
+
+> [!NOTE]
+> We recommend starting with the **[Zero to LitGPT: Getting Started with Pretraining, Finetuning, and Using LLMs](tutorials/0_to_litgpt.md)** if you are looking to get started with using LitGPT.
+
+Tutorials and in-depth feature documentation can be found below:
+
 -  Finetuning, incl. LoRA, QLoRA, and Adapters ([tutorials/finetune.md](tutorials/finetune.md))
--  Pretraining ([tutorials/pretrain_tinyllama.md](tutorials/pretrain_tinyllama.md))
+-  Pretraining ([tutorials/pretrain.md](tutorials/pretrain.md))
 -  Model evaluation ([tutorials/evaluation.md](tutorials/evaluation.md))
 -  Supported and custom datasets ([tutorials/prepare_dataset.md](tutorials/prepare_dataset.md))
 -  Quantization ([tutorials/quantize.md](tutorials/quantize.md))
 -  Tips for dealing with out-of-memory (OOM) errors ([tutorials/oom.md](tutorials/oom.md))
 
-
-
-
-
 &nbsp;
 
 ## XLA
 
-Lightning AI has partnered with Google to add first-class support for [Cloud TPUs](https://cloud.google.com/tpu) in [Lightning’s frameworks](https://github.com/Lightning-AI/lightning) and LitGPT,
+Lightning AI has partnered with Google to add first-class support for [Cloud TPUs](https://cloud.google.com/tpu) in [Lightning's frameworks](https://github.com/Lightning-AI/lightning) and LitGPT,
 helping democratize AI for millions of developers and researchers worldwide.
 
 Using TPUs with Lightning is as straightforward as changing one line of code.
 
-We provide scripts fully optimized for TPUs in the [XLA directory](xla).
+We provide scripts fully optimized for TPUs in the [XLA directory](extensions/xla).
 
 
 
 &nbsp;
 
 ## Acknowledgements
 
@@ -597,28 +791,39 @@
 
 
 &nbsp;
 
 
 ## Community showcase
 
-Check out the projects below using and building on LitGPT. If you have a project you'd like to add to this section, please don't hestiate to open a pull request.
+Check out the projects below that use and build on LitGPT. If you have a project you'd like to add to this section, please don't hesitate to open a pull request.
 
 &nbsp;
 
 **🏆 NeurIPS 2023 Large Language Model Efficiency Challenge: 1 LLM + 1 GPU + 1 Day**
 
 The LitGPT repository was the official starter kit for the [NeurIPS 2023 LLM Efficiency Challenge](https://llm-efficiency-challenge.github.io), which is a competition focused on finetuning an existing non-instruction tuned LLM for 24 hours on a single GPU.
 
 &nbsp;
 
 **🦙 TinyLlama: An Open-Source Small Language Model**
 
 LitGPT powered the [TinyLlama project](https://github.com/jzhang38/TinyLlama) and [TinyLlama: An Open-Source Small Language Model](https://arxiv.org/abs/2401.02385) research paper.
 
+&nbsp;
+
+**🍪 MicroLlama: MicroLlama-300M**
+
+[MicroLlama](https://github.com/keeeeenw/MicroLlama) is a 300M Llama model pretrained on 50B tokens powered by TinyLlama and LitGPT.
+
+&nbsp;
+
+**🔬 Pre-training Small Base LMs with Fewer Tokens**
+
+The research paper ["Pre-training Small Base LMs with Fewer Tokens"](https://arxiv.org/abs/2404.08634), which utilizes LitGPT, develops smaller base language models by inheriting a few transformer blocks from larger models and training on a tiny fraction of the data used by the larger models. It demonstrates that these smaller models can perform comparably to larger models despite using significantly less training data and resources.
 
 &nbsp;
 
 ## Citation
 
 If you use LitGPT in your research, please cite the following work:
 
@@ -632,8 +837,7 @@
 ```
 
 &nbsp;
 
 ## License
 
 LitGPT is released under the [Apache 2.0](https://github.com/Lightning-AI/litgpt/blob/main/LICENSE) license.
-
```

### Comparing `litgpt-0.2.0.dev0/litgpt.egg-info/SOURCES.txt` & `litgpt-0.3.0/litgpt.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -32,16 +32,19 @@
 litgpt/data/json_data.py
 litgpt/data/lima.py
 litgpt/data/lit_data.py
 litgpt/data/longform.py
 litgpt/data/openwebtext.py
 litgpt/data/prepare_slimpajama.py
 litgpt/data/prepare_starcoder.py
+litgpt/data/text_files.py
 litgpt/data/tinyllama.py
 litgpt/data/tinystories.py
+litgpt/deploy/serve.py
+litgpt/eval/evaluate.py
 litgpt/finetune/__init__.py
 litgpt/finetune/adapter.py
 litgpt/finetune/adapter_v2.py
 litgpt/finetune/full.py
 litgpt/finetune/lora.py
 litgpt/generate/__init__.py
 litgpt/generate/adapter.py
@@ -54,29 +57,35 @@
 litgpt/scripts/convert_hf_checkpoint.py
 litgpt/scripts/convert_lit_checkpoint.py
 litgpt/scripts/convert_pretrained_checkpoint.py
 litgpt/scripts/download.py
 litgpt/scripts/merge_lora.py
 tests/test_adapter.py
 tests/test_adapter_v2.py
+tests/test_args.py
 tests/test_chat.py
 tests/test_ci.py
 tests/test_cli.py
 tests/test_config.py
 tests/test_config_hub.py
 tests/test_convert_hf_checkpoint.py
 tests/test_convert_lit_checkpoint.py
 tests/test_convert_pretrained_checkpoint.py
+tests/test_evaluate.py
 tests/test_full.py
 tests/test_generate.py
 tests/test_generate_adapter.py
 tests/test_generate_sequentially.py
 tests/test_generate_tp.py
-tests/test_lm_eval_harness.py
 tests/test_lora.py
 tests/test_merge_lora.py
 tests/test_model.py
 tests/test_pretrain.py
 tests/test_prompts.py
 tests/test_rope.py
+tests/test_serve.py
+tests/test_thunder_ddp.py
+tests/test_thunder_fsdp.py
+tests/test_thunder_pretrain.py
 tests/test_tokenizer.py
+tests/test_unsloth_executor.py
 tests/test_utils.py
```

### Comparing `litgpt-0.2.0.dev0/tests/test_adapter.py` & `litgpt-0.3.0/tests/test_adapter.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,40 +4,46 @@
 from dataclasses import asdict
 from io import StringIO
 from unittest import mock
 from unittest.mock import Mock
 
 import pytest
 import torch
+import yaml
 from conftest import RunIf
 from lightning import Fabric
 from lightning.fabric.plugins.precision.bitsandbytes import _BITSANDBYTES_AVAILABLE, BitsandbytesPrecision
 from lightning.fabric.wrappers import _FabricOptimizer
+from torch._dynamo.backends import debugging
+from transformers.models.gemma import GemmaConfig, GemmaForCausalLM
 
+import litgpt.adapter as gpt_adapter
+import litgpt.finetune.adapter as module
+import litgpt.model as gpt
+from litgpt.adapter import GPT, Config, adapter_filter
+from litgpt.args import EvalArgs, TrainArgs
+from litgpt.data import Alpaca
+from litgpt.scripts.convert_hf_checkpoint import copy_weights_hf_llama
 
-def test_config_identical():
-    import litgpt.adapter as gpt_adapter
-    import litgpt.model as gpt
 
+def test_config_identical():
     name = "pythia-14m"
     base_config = asdict(gpt.Config.from_name(name))
     adapter_config = asdict(gpt_adapter.Config.from_name(name))
     del adapter_config["adapter_prompt_length"]
     del adapter_config["adapter_start_layer"]
     assert adapter_config == base_config
 
     with Fabric(accelerator="cpu").init_module(empty_init=True):
         base_model = gpt.GPT.from_name(name)
         adapter_model = gpt_adapter.GPT.from_name(name)
     assert adapter_model.lm_head.weight.shape == base_model.lm_head.weight.shape
 
 
 def test_adapter_filter(tmp_path):
-    from litgpt.adapter import GPT, adapter_filter
-
     fabric = Fabric(devices=1)
     model = GPT.from_name("pythia-14m", n_layer=4)
     save_path = tmp_path / "model.pth"
     fabric.save(save_path, {"model": model}, filter={"model": adapter_filter})
     saved = torch.load(save_path)["model"]
 
     expected = {
@@ -47,21 +53,16 @@
         "transformer.h.3.attn.gating_factor",
     }
     assert set(saved) == expected
 
 
 @mock.patch.dict(os.environ, {"LT_ACCELERATOR": "cpu"})
 def test_adapter_script(tmp_path, fake_checkpoint_dir, monkeypatch, alpaca_path):
-    import litgpt.finetune.adapter as module
-    from litgpt.args import EvalArgs, TrainArgs
-    from litgpt.config import name_to_config
-    from litgpt.data import Alpaca
-
     model_config = dict(block_size=128, n_layer=2, n_embd=8, n_head=4, padded_vocab_size=8, adapter_start_layer=0)
-    monkeypatch.setitem(name_to_config, "tmp", model_config)
+    (fake_checkpoint_dir / "model_config.yaml").write_text(yaml.dump(model_config))
 
     monkeypatch.setattr(module, "load_checkpoint", Mock())
 
     tokenizer_mock = Mock()
     tokenizer_mock.return_value = tokenizer_mock
     tokenizer_mock.encode = lambda *_, **__: torch.tensor([3, 2, 1])
     monkeypatch.setattr(module, "Tokenizer", tokenizer_mock)
@@ -93,42 +94,37 @@
             "hyperparameters.yaml",
             "prompt_style.yaml",
         }
     assert (out_dir / "logs" / "csv" / "version_0" / "metrics.csv").is_file()
 
     logs = stdout.getvalue()
     assert logs.count("(step)") == 6
-    assert logs.count("val loss") == 3
+    assert logs.count("val loss") == 4  # 3 validations + 1 final validation
+    assert logs.count("Final evaluation") == 1
     assert "of trainable parameters: 168" in logs
 
 
 def test_adapter_gpt_init_weights():
-    from litgpt.adapter import GPT, Config
-
     config = Config(n_layer=1, n_head=6, n_embd=12, block_size=1, vocab_size=1, adapter_start_layer=0)
     model = GPT(config)
     param = model.transformer.h[0].attn.gating_factor
 
     assert (param == 0).all()
     torch.nn.init.constant_(param, 1.23)
     assert (param != 0).any()
     model.apply(model._init_weights)
     assert (param == 0).all()
 
 
 @RunIf(dynamo=True)
 @torch.inference_mode()
 def test_adapter_compile():
-    from litgpt.adapter import GPT
-
     model = GPT.from_name("pythia-14m", n_layer=3)
     x = torch.randint(model.config.vocab_size, size=(2, model.config.block_size), dtype=torch.int64)
 
-    from torch._dynamo.backends import debugging
-
     explanation = torch._dynamo.explain(model)(x)
     assert isinstance(explanation, debugging.ExplainOutput)
     assert explanation.graph_count == 1
     assert explanation.graph_break_count == 0
 
     model = GPT(model.config)
     model.set_kv_cache(2)
@@ -137,27 +133,23 @@
     assert isinstance(explanation, debugging.ExplainOutput)
     assert explanation.graph_count == 1
     assert explanation.graph_break_count == 0
 
 
 @RunIf(min_cuda_gpus=1)
 def test_adapter_bitsandbytes(monkeypatch, tmp_path, fake_checkpoint_dir, alpaca_path):
-    import litgpt.finetune.adapter as module
-    from litgpt.config import name_to_config
-    from litgpt.data import Alpaca
-
     if not _BITSANDBYTES_AVAILABLE:
         pytest.skip("BNB not available")
 
     from bitsandbytes.optim import PagedAdamW
 
     model_config = dict(
         block_size=128, n_layer=2, n_embd=8, n_head=4, padded_vocab_size=8, adapter_start_layer=0, bias=True
     )
-    monkeypatch.setitem(name_to_config, "tmp", model_config)
+    (fake_checkpoint_dir / "model_config.yaml").write_text(yaml.dump(model_config))
 
     tokenizer_mock = Mock()
     tokenizer_mock.return_value = tokenizer_mock
     tokenizer_mock.encode = lambda *_, **__: torch.tensor([3, 2, 1])
     monkeypatch.setattr(module, "Tokenizer", tokenizer_mock)
 
     monkeypatch.setattr(module, "load_checkpoint", Mock())
@@ -238,8 +230,49 @@
             "transformer.h.1.attn.adapter_wte.weight",
             "transformer.h.1.attn.gating_factor",
         }
     }
 
     logs = stdout.getvalue()
     assert "of trainable parameters: 168" in logs
-    assert "of non trainable parameters: 1,888" in logs
+    assert "of non-trainable parameters: 1,888" in logs
+
+
+@torch.inference_mode()
+@pytest.mark.parametrize("model_name", ["gemma-2b", "gemma-7b"])
+def test_against_hf_gemma(model_name):
+    device = torch.device("cpu")
+    dtype = torch.float32
+    T = 5
+    ours_config = Config.from_name(model_name, n_layer=2, n_head=16, n_embd=32, intermediate_size=86)
+    theirs_config = GemmaConfig(
+        vocab_size=ours_config.padded_vocab_size,
+        hidden_size=ours_config.n_embd,
+        head_dim=ours_config.head_size,
+        num_attention_heads=ours_config.n_head,
+        num_hidden_layers=ours_config.n_layer,
+        intermediate_size=ours_config.intermediate_size,
+        max_position_embeddings=T,
+        rms_norm_eps=ours_config.norm_eps,
+        num_key_value_heads=ours_config.n_query_groups,
+        rope_theta=ours_config.rope_base,
+        attention_bias=ours_config.bias,
+        tie_word_embeddings=True,
+        hidden_act="gelu_pytorch_tanh",
+    )
+    assert ours_config.intermediate_size == theirs_config.intermediate_size
+
+    theirs_model = GemmaForCausalLM(theirs_config).to(device)
+    theirs_state_dict = theirs_model.state_dict()
+    # Gemma weights are shipped without `lm_head.weight`
+    theirs_state_dict.pop("lm_head.weight")
+    state_dict = {}
+    copy_weights_hf_llama(ours_config, {}, state_dict, theirs_state_dict)
+    ours_model = GPT(ours_config).to(device)
+    ours_model.load_state_dict(state_dict)
+
+    # test end to end
+    x = torch.tensor([[9856, 23, 491, 1536, 304]], dtype=torch.int32, device=device)
+    assert x.size(1) == T
+    ours_y = ours_model(x)
+    theirs_y = theirs_model(x)["logits"].to(dtype)  # HF converts logits to float
+    torch.testing.assert_close(ours_y, theirs_y)
```

### Comparing `litgpt-0.2.0.dev0/tests/test_adapter_v2.py` & `litgpt-0.3.0/tests/test_adapter_v2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
 import os
-import sys
 from contextlib import redirect_stdout
 from io import StringIO
-from pathlib import Path
 from unittest import mock
 from unittest.mock import Mock
 
 import pytest
 import torch
+import yaml
 from conftest import RunIf
 from lightning import Fabric
 from lightning.fabric.plugins.precision.bitsandbytes import _BITSANDBYTES_AVAILABLE, BitsandbytesPrecision
 from lightning.fabric.wrappers import _FabricOptimizer
-
-# support running without installing as a package
-wd = Path(__file__).parent.parent.resolve()
-sys.path.append(str(wd))
+from torch._dynamo.backends import debugging
+from transformers.models.gemma import GemmaConfig, GemmaForCausalLM
+from transformers.models.mixtral import MixtralConfig, MixtralForCausalLM
 
 import litgpt.config as config_module
+import litgpt.finetune.adapter_v2 as module
+from litgpt.adapter_v2 import GPT as AdapterV2GPT
+from litgpt.adapter_v2 import Config, adapter_filter
+from litgpt.args import EvalArgs, TrainArgs
+from litgpt.data import Alpaca
+from litgpt.model import GPT as BaseGPT
+from litgpt.scripts.convert_hf_checkpoint import copy_weights_hf_llama
 
 
 def test_config_identical():
-    import litgpt.adapter_v2 as gpt_adapter
-    import litgpt.model as gpt
-
     name = "pythia-14m"
     with Fabric(accelerator="cpu").init_module(empty_init=True):
-        base_model = gpt.GPT.from_name(name)
-        adapter_model = gpt_adapter.GPT.from_name(name)
+        base_model = BaseGPT.from_name(name)
+        adapter_model = AdapterV2GPT.from_name(name)
 
     assert not hasattr(base_model.transformer.h[2].attn.attn, "adapter_bias")
     assert not hasattr(base_model.transformer.h[2].attn.attn, "adapter_scale")
     assert hasattr(adapter_model.transformer.h[2].attn.attn, "adapter_bias")
     assert hasattr(adapter_model.transformer.h[2].attn.attn, "adapter_scale")
 
 
 def test_adapter_v2_filter(tmp_path):
-    from litgpt.adapter_v2 import GPT, adapter_filter
-
     fabric = Fabric(devices=1)
-    model = GPT.from_name("pythia-14m", n_layer=3)
+    model = AdapterV2GPT.from_name("pythia-14m", n_layer=3)
     save_path = tmp_path / "model.pth"
     fabric.save(save_path, {"model": model}, filter={"model": adapter_filter})
     saved = torch.load(save_path)["model"]
 
     expected = {
         "lm_head.adapter_bias",
         "lm_head.adapter_scale",
@@ -70,21 +70,16 @@
         ):
             expected.add(f"transformer.h.{layer}.{param}")
     assert set(saved) == expected
 
 
 @mock.patch.dict(os.environ, {"LT_ACCELERATOR": "cpu"})
 def test_adapter_v2_script(tmp_path, fake_checkpoint_dir, monkeypatch, alpaca_path):
-    import litgpt.finetune.adapter_v2 as module
-    from litgpt.args import EvalArgs, TrainArgs
-    from litgpt.config import name_to_config
-    from litgpt.data import Alpaca
-
     model_config = dict(block_size=128, n_layer=2, n_embd=8, n_head=4, padded_vocab_size=8, adapter_start_layer=0)
-    monkeypatch.setitem(name_to_config, "tmp", model_config)
+    (fake_checkpoint_dir / "model_config.yaml").write_text(yaml.dump(model_config))
 
     monkeypatch.setattr(module, "load_checkpoint", Mock())
 
     tokenizer_mock = Mock()
     tokenizer_mock.return_value = tokenizer_mock
     tokenizer_mock.encode = lambda *_, **__: torch.tensor([3, 2, 1])
     monkeypatch.setattr(module, "Tokenizer", tokenizer_mock)
@@ -116,79 +111,65 @@
             "hyperparameters.yaml",
             "prompt_style.yaml",
         }
     assert (out_dir / "logs" / "csv" / "version_0" / "metrics.csv").is_file()
 
     logs = stdout.getvalue()
     assert logs.count("(step)") == 6
-    assert logs.count("val loss") == 3
+    assert logs.count("val loss") == 4  # 3 validations + 1 final validation
+    assert logs.count("Final evaluation") == 1
     assert "of trainable parameters: 552" in logs
 
 
 def test_adapter_v2_gpt_init_weights():
-    from litgpt.adapter_v2 import GPT, Config
-
     config = Config(n_layer=1, n_head=6, n_embd=12, block_size=1, vocab_size=1, adapter_start_layer=0)
-    model = GPT(config)
+    model = AdapterV2GPT(config)
 
     for param in (model.transformer.h[0].attn.gating_factor, model.lm_head.adapter_bias):
         assert (param == 0).all()
         torch.nn.init.constant_(param, 1.23)
         assert (param != 0).any()
         model.apply(model._init_weights)
         assert (param == 0).all()
 
 
 @pytest.mark.parametrize("name", [c["name"] for c in config_module.configs])
 def test_base_model_can_be_adapter_v2_loaded(name):
-    from litgpt.adapter_v2 import GPT as AdapterV2GPT
-    from litgpt.adapter_v2 import adapter_filter
-    from litgpt.model import GPT as BaseGPT
-
     kwargs = {"n_layer": 2, "n_head": 8, "n_embd": 16, "padded_vocab_size": 32}
     base_model = BaseGPT.from_name(name, **kwargs)
     base_model_state_dict = base_model.state_dict()
     lora_model = AdapterV2GPT.from_name(name, **kwargs, adapter_start_layer=0)
     keys = lora_model.load_state_dict(base_model_state_dict, strict=False)
     assert not keys.unexpected_keys
     for k in keys.missing_keys:
         assert adapter_filter(k, None)
 
 
 @RunIf(dynamo=True)
 @torch.inference_mode()
 def test_adapter_v2_compile():
-    from litgpt.adapter_v2 import GPT
-
-    model = GPT.from_name("pythia-14m", n_layer=3)
+    model = AdapterV2GPT.from_name("pythia-14m", n_layer=3)
     x = torch.randint(model.config.vocab_size, size=(2, model.config.block_size), dtype=torch.int64)
 
-    from torch._dynamo.backends import debugging
-
     explanation = torch._dynamo.explain(model)(x)
     assert isinstance(explanation, debugging.ExplainOutput)
     assert explanation.graph_count == 1
     assert explanation.graph_break_count == 0
 
-    model = GPT(model.config)
+    model = AdapterV2GPT(model.config)
     model.set_kv_cache(2)
     input_pos = torch.arange(model.config.block_size)
     explanation = torch._dynamo.explain(model)(x, input_pos)
     assert isinstance(explanation, debugging.ExplainOutput)
     assert explanation.graph_count == 1
     assert explanation.graph_break_count == 0
 
 
 @torch.inference_mode()
 def test_against_hf_mixtral():
-    from transformers.models.mixtral import MixtralConfig, MixtralForCausalLM
-
-    from litgpt.adapter_v2 import GPT, Config
-    from litgpt.scripts.convert_hf_checkpoint import copy_weights_hf_llama
-
     device = torch.device("cpu")
     dtype = torch.float32
     ours_config = Config.from_name(
         "Mixtral-8x7B-Instruct-v0.1",
         padded_vocab_size=10000,
         n_layer=2,
         n_embd=32,
@@ -212,41 +193,78 @@
     )
     assert ours_config.intermediate_size == theirs_config.intermediate_size
 
     theirs_model = MixtralForCausalLM(theirs_config).to(device)
     theirs_state_dict = theirs_model.state_dict()
     state_dict = {}
     copy_weights_hf_llama(ours_config, {}, state_dict, theirs_state_dict)
-    ours_model = GPT(ours_config).to(device)
+    ours_model = AdapterV2GPT(ours_config).to(device)
     # strict=False because missing keys due to adapter weights not contained in state dict
     ours_model.load_state_dict(state_dict, strict=False)
 
     # test end to end
     x = torch.tensor([[9856, 23, 491, 1536, 304], [23, 345, 65, 123, 321]], dtype=torch.int32, device=device)
     assert x.size(1) == T
     ours_y = ours_model(x)
     theirs_y = theirs_model(x)["logits"].to(dtype)  # HF converts logits to float
     torch.testing.assert_close(ours_y, theirs_y)
 
 
+@torch.inference_mode()
+@pytest.mark.parametrize("model_name", ["gemma-2b", "gemma-7b"])
+def test_against_hf_gemma(model_name):
+    device = torch.device("cpu")
+    dtype = torch.float32
+    T = 5
+    ours_config = Config.from_name(model_name, n_layer=2, n_head=16, n_embd=32, intermediate_size=86)
+    theirs_config = GemmaConfig(
+        vocab_size=ours_config.padded_vocab_size,
+        hidden_size=ours_config.n_embd,
+        head_dim=ours_config.head_size,
+        num_attention_heads=ours_config.n_head,
+        num_hidden_layers=ours_config.n_layer,
+        intermediate_size=ours_config.intermediate_size,
+        max_position_embeddings=T,
+        rms_norm_eps=ours_config.norm_eps,
+        num_key_value_heads=ours_config.n_query_groups,
+        rope_theta=ours_config.rope_base,
+        attention_bias=ours_config.bias,
+        tie_word_embeddings=True,
+        hidden_act="gelu_pytorch_tanh",
+    )
+    assert ours_config.intermediate_size == theirs_config.intermediate_size
+
+    theirs_model = GemmaForCausalLM(theirs_config).to(device)
+    theirs_state_dict = theirs_model.state_dict()
+    # Gemma weights are shipped without `lm_head.weight`
+    theirs_state_dict.pop("lm_head.weight")
+    state_dict = {}
+    copy_weights_hf_llama(ours_config, {}, state_dict, theirs_state_dict)
+    ours_model = AdapterV2GPT(ours_config).to(device)
+    ours_model.load_state_dict(state_dict, strict=False)
+
+    # test end to end
+    x = torch.tensor([[9856, 23, 491, 1536, 304]], dtype=torch.int32, device=device)
+    assert x.size(1) == T
+    ours_y = ours_model(x)
+    theirs_y = theirs_model(x)["logits"].to(dtype)  # HF converts logits to float
+    torch.testing.assert_close(ours_y, theirs_y)
+
+
 @RunIf(min_cuda_gpus=1)
 def test_adapter_v2_bitsandbytes(monkeypatch, tmp_path, fake_checkpoint_dir, alpaca_path):
-    import litgpt.finetune.adapter_v2 as module
-    from litgpt.config import name_to_config
-    from litgpt.data import Alpaca
-
     if not _BITSANDBYTES_AVAILABLE:
         pytest.skip("BNB not available")
 
     from bitsandbytes.optim import PagedAdamW
 
     model_config = dict(
         block_size=128, n_layer=2, n_embd=8, n_head=4, padded_vocab_size=8, adapter_start_layer=0, bias=True
     )
-    monkeypatch.setitem(name_to_config, "tmp", model_config)
+    (fake_checkpoint_dir / "model_config.yaml").write_text(yaml.dump(model_config))
 
     tokenizer_mock = Mock()
     tokenizer_mock.return_value = tokenizer_mock
     tokenizer_mock.encode = lambda *_, **__: torch.tensor([3, 2, 1])
     monkeypatch.setattr(module, "Tokenizer", tokenizer_mock)
 
     monkeypatch.setattr(module, "load_checkpoint", Mock())
@@ -373,8 +391,8 @@
             "transformer.h.1.norm_1.weight",
             "transformer.h.1.attn.attn.adapter_scale",
         }
     }
 
     logs = stdout.getvalue()
     assert "of trainable parameters: 552" in logs
-    assert "of non trainable parameters: 1,808" in logs
+    assert "of non-trainable parameters: 1,808" in logs
```

### Comparing `litgpt-0.2.0.dev0/tests/test_chat.py` & `litgpt-0.3.0/tests/test_chat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
+import os
 import re
 import subprocess
 import sys
 from contextlib import redirect_stderr, redirect_stdout
 from io import StringIO
 from itertools import repeat
 from pathlib import Path
 from unittest.mock import ANY, MagicMock, Mock, call, patch
 
 import pytest
 import torch
 import yaml
+from lightning.fabric import Fabric
+
+import litgpt.chat.base as chat
+import litgpt.generate.base as generate
+from litgpt import Config
+from litgpt.utils import save_config
 
 
 @pytest.mark.parametrize(
     ("generated", "stop_tokens", "expected"),
     [
         (repeat(1), (), [1] * 8),
         ([1, 2, 3, 0], ([0],), [1, 2, 3]),
         ([1, 2, 3, 0], ([9], [2, 4], [1, 2, 3, 0]), []),
         ([1, 2, 3, 0, 0], ([0, 0, 0], [0, 0]), [1, 2, 3]),
         ([3, 1, 2], ([1, 2], [3]), []),
         ([1, 2, 3, 0, 3, 2, 1, 0], ([4, 3, 2, 1], [2, 4]), [1, 2, 3, 0, 3, 2, 1, 0]),
     ],
 )
 def test_generate(monkeypatch, generated, stop_tokens, expected):
-    import litgpt.chat.base as chat
-    import litgpt.generate.base as generate
-
     input_idx = torch.tensor([5, 3])
     max_returned_tokens = len(input_idx) + 8
     model = MagicMock()
     model.config.block_size = 100
     model.max_seq_length = 100
     it = iter(generated)
 
@@ -50,18 +54,14 @@
         for t in actual:
             assert t.dtype == torch.long
         assert torch.cat(actual).tolist() == expected
 
 
 @pytest.mark.parametrize("tokenizer_backend", ["huggingface", "sentencepiece"])
 def test_decode(tokenizer_backend):
-    from lightning.fabric import Fabric
-
-    import litgpt.chat.base as chat
-
     class Tokenizer:
         backend = tokenizer_backend
         id2token = {1: "foo ", 2: "bar ", 3: "baz "}
 
         def decode(self, tensor: torch.Tensor) -> str:
             tensor = [tensor] if tensor.ndim == 0 else tensor
             return "".join(self.id2token[int(value)] for value in tensor)
@@ -77,16 +77,14 @@
 
     assert out.getvalue() == "baz bar foo "
 
 
 @patch("litgpt.chat.base.input")
 @pytest.mark.parametrize("stop_iteration", [KeyboardInterrupt, ""])
 def test_main(mocked_input, stop_iteration, fake_checkpoint_dir, monkeypatch, tensor_like):
-    import litgpt.chat.base as chat
-
     # these values will be iteratively provided for each `input()` call
     mocked_input.side_effect = ["Hello", stop_iteration]
 
     config_path = fake_checkpoint_dir / "model_config.yaml"
     config = {
         "name": "Llama 3",
         "block_size": 128,
@@ -130,7 +128,30 @@
         cli_path = Path(__file__).parent.parent / "litgpt/chat/base.py"
         args = [sys.executable, cli_path, "-h"]
     else:
         args = ["litgpt", "chat", "-h"]
     output = subprocess.check_output(args)
     output = str(output.decode())
     assert "Starts a conversation" in output
+
+
+@patch("litgpt.chat.base.input")
+@patch("litgpt.chat.base.merge_lora")
+def test_merge_lora_if_needed(mocked_merge_lora, mocked_input, fake_checkpoint_dir, monkeypatch, tensor_like):
+    # these values will be iteratively provided for each `input()` call
+    mocked_input.side_effect = [""]
+
+    # pretend there is an unmerged LORA checkpoint
+    os.rename(fake_checkpoint_dir / "lit_model.pth", fake_checkpoint_dir / "lit_model.pth.lora")
+    mocked_merge_lora.side_effect = lambda _: Path(fake_checkpoint_dir / "lit_model.pth").touch()
+
+    config = Config.from_name("pythia-14m")
+    save_config(config, fake_checkpoint_dir)
+    monkeypatch.setattr(chat, "load_checkpoint", Mock())
+    monkeypatch.setattr(chat, "Tokenizer", Mock())
+
+    out, err = StringIO(), StringIO()
+    with redirect_stdout(out), redirect_stderr(err):
+        chat.main(checkpoint_dir=fake_checkpoint_dir)
+
+    assert re.match("Merging LoRA weights with the base model.", out.getvalue(), re.DOTALL)
+    mocked_merge_lora.assert_called_once()
```

### Comparing `litgpt-0.2.0.dev0/tests/test_cli.py` & `litgpt-0.3.0/tests/test_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,43 +2,33 @@
 from contextlib import redirect_stdout
 from io import StringIO
 from unittest import mock
 
 import pytest
 from packaging.version import Version
 
+from litgpt.__main__ import main
 
-def test_cli():
-    from litgpt.__main__ import main
 
+def test_cli():
     out = StringIO()
     with pytest.raises(SystemExit), redirect_stdout(out), mock.patch("sys.argv", ["litgpt", "-h"]):
         main()
     out = out.getvalue()
     assert "usage: litgpt" in out
-    assert "{download,chat,finetune,pretrain,generate,convert,merge_lora}" in out
+    assert "{download,chat,finetune,pretrain,generate,convert,merge_lora,evaluate,serve}" in out
     assert (
         """Available subcommands:
     download            Download weights or tokenizer data from the Hugging
                         Face Hub.
     chat                Chat with a model."""
         in out
     )
-
-    out = StringIO()
-    with pytest.raises(SystemExit), redirect_stdout(out), mock.patch("sys.argv", ["litgpt", "finetune", "-h"]):
-        main()
-    out = out.getvalue()
-    assert (
-        """Available subcommands:
-    lora                Finetune a model with LoRA.
-    full                Finetune a model."""
-        in out
-    )
-
+    assert """evaluate            Evaluate a model with the LM Evaluation Harness.""" in out
+    assert """serve               Serve and deploy a model with LitServe.""" in out
     out = StringIO()
     with pytest.raises(SystemExit), redirect_stdout(out), mock.patch("sys.argv", ["litgpt", "finetune", "lora", "-h"]):
         main()
     out = out.getvalue()
     assert (
         """--lora_alpha LORA_ALPHA
                         The LoRA alpha. (type: int, default: 16)"""
@@ -56,7 +46,17 @@
     print(out)
     assert (
         """--train.max_tokens MAX_TOKENS
                         Total number of tokens to train on (type:
                         Optional[int], default: 3000000000000)"""
         in out
     )
+
+
+def test_rewrite_finetune_command():
+    out1 = StringIO()
+    with pytest.raises(SystemExit), redirect_stdout(out1), mock.patch("sys.argv", ["litgpt", "fineune", "-h"]):
+        main()
+    out2 = StringIO()
+    with pytest.raises(SystemExit), redirect_stdout(out2), mock.patch("sys.argv", ["litgpt", "fineune", "lora", "-h"]):
+        main()
+    assert out1.getvalue() == out2.getvalue()
```

### Comparing `litgpt-0.2.0.dev0/tests/test_config.py` & `litgpt-0.3.0/tests/test_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,17 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
 
-import sys
-from pathlib import Path
-
 import pytest
 import yaml
 
-# support running without installing as a package
-wd = Path(__file__).parent.parent.resolve()
-sys.path.append(str(wd))
-
 import litgpt.config as config_module
+from litgpt import Config
 
 
 def test_config():
-    from litgpt import Config
-
     config = Config()
     assert config.name == ""
     assert config.block_size == 4096
 
     config = Config(block_size=2048)
     assert config.block_size == 2048
 
@@ -30,73 +22,63 @@
     assert config.block_size == 4096
 
     config = Config(hf_config={"name": "pythia-14m"})
     assert config.name == "pythia-14m"
 
 
 def test_from_hf_name():
-    from litgpt import Config
-
     # by short-hand name
     config0 = Config.from_name("tiny-llama-1.1b")
     # or by huggingface hub repo name
     config1 = Config.from_name("TinyLlama-1.1B-intermediate-step-1431k-3T")
     assert config0 == config1
 
 
 @pytest.mark.parametrize("config", config_module.configs, ids=[c["name"] for c in config_module.configs])
 def test_short_and_hf_names_are_equal_unless_on_purpose(config):
-    from litgpt import Config
-
     # by short-hand name
     config0 = Config.from_name(config["name"])
     # or by huggingface hub repo name
     config1 = Config.from_name(config["hf_config"]["name"])
     assert config0.name == config1.name
 
 
 def test_nonexisting_name():
-    from litgpt import Config
-
     with pytest.raises(ValueError, match="not a supported"):
         Config.from_name("foobar")
 
 
 def test_from_checkpoint(tmp_path):
-    from litgpt import Config
-
     # 1. Neither `lit_config.py` nor matching config exists.
     with pytest.raises(FileNotFoundError, match="neither 'model_config.yaml' nor matching config exists"):
         Config.from_checkpoint(tmp_path / "non_existing_checkpoint")
 
     # 2. If `lit_config.py` doesn't exists, but there is a matching config in `litgpt/config.py`.
     config = Config.from_checkpoint(tmp_path / "pythia-14m")
     assert config.name == "pythia-14m"
     assert config.block_size == 512
     assert config.n_layer == 6
 
     # 3. If only `lit_config.py` exists.
     config_data = {"name": "pythia-14m", "block_size": 24, "n_layer": 2}
-    with open(tmp_path / "model_config.yaml", "w") as file:
+    with open(tmp_path / "model_config.yaml", "w", encoding="utf-8") as file:
         yaml.dump(config_data, file)
     config = Config.from_checkpoint(tmp_path)
     assert config.name == "pythia-14m"
     assert config.block_size == 24
     assert config.n_layer == 2
 
     # 4. Both `lit_config.py` and a matching config exist, but `lit_config.py` supersedes matching config
     (tmp_path / "pythia-14m").mkdir()
-    with open(tmp_path / "pythia-14m/model_config.yaml", "w") as file:
+    with open(tmp_path / "pythia-14m/model_config.yaml", "w", encoding="utf-8") as file:
         yaml.dump(config_data, file)
     config = Config.from_checkpoint(tmp_path / "pythia-14m")
     assert config.name == "pythia-14m"
     assert config.block_size == 24
     assert config.n_layer == 2
 
 
 @pytest.mark.parametrize("head_size", [None, 128])
 def test_head_size(head_size):
-    from litgpt import Config
-
     config = Config(head_size)
 
     assert config.head_size == head_size or config.n_embd // config.n_head
```

### Comparing `litgpt-0.2.0.dev0/tests/test_config_hub.py` & `litgpt-0.3.0/tests/test_config_hub.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,20 +3,25 @@
 from pathlib import Path
 from unittest import mock
 from unittest.mock import Mock
 
 import pytest
 from lightning.fabric.plugins import Precision
 
+from litgpt import Config
+from litgpt.utils import CLI
 
 fixed_pairs = [
     ("litgpt/pretrain.py", "pretrain/debug.yaml"),
     ("litgpt/pretrain.py", "pretrain/tinyllama.yaml"),
     ("litgpt/pretrain.py", "pretrain/tinystories.yaml"),
-    ("litgpt/pretrain.py", "https://raw.githubusercontent.com/Lightning-AI/litgpt/main/config_hub/pretrain/tinystories.yaml"),
+    (
+        "litgpt/pretrain.py",
+        "https://raw.githubusercontent.com/Lightning-AI/litgpt/main/config_hub/pretrain/tinystories.yaml",
+    ),
 ]
 
 config_hub_path = Path(__file__).parent.parent / "config_hub" / "finetune"
 model_pairs = []
 
 for model_dir in config_hub_path.iterdir():
     if model_dir.is_dir():
@@ -27,29 +32,29 @@
             relative_yaml_path = yaml_file.relative_to(config_hub_path.parent)
             model_pairs.append((python_file, str(relative_yaml_path)))
 
 all_pairs = fixed_pairs + model_pairs
 
 
 @pytest.mark.parametrize(("script_file", "config_file"), all_pairs)
-def test_config_help(script_file, config_file):
+def test_config_help(script_file, config_file, monkeypatch):
     """Test that configs validate against the signature in the scripts."""
-    from litgpt.utils import CLI
-
     script_file = Path(__file__).parent.parent / script_file
     assert script_file.is_file()
     if "http" not in str(config_file):
         config_file = Path(__file__).parent.parent / "config_hub" / config_file
         assert config_file.is_file()
 
     spec = importlib.util.spec_from_file_location(str(script_file.parent.name), script_file)
     module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(module)
 
-    module.main = Mock()
-    module.Tokenizer = Mock()
-    module.BitsandbytesPrecision = Mock(return_value=Precision())
+    monkeypatch.setattr(module, "main", Mock())
+    monkeypatch.setattr(module, "Tokenizer", Mock())
+    monkeypatch.setattr(module, "BitsandbytesPrecision", Mock(return_value=Precision()), raising=False)
+    monkeypatch.setattr(module, "Config", Mock(return_value=Config.from_name("pythia-14m")))
+    monkeypatch.setattr(module, "check_valid_checkpoint_dir", Mock(), raising=False)
 
     with mock.patch("sys.argv", [script_file.name, "--config", str(config_file), "--devices", "1"]):
         CLI(module.setup)
 
     module.main.assert_called_once()
```

### Comparing `litgpt-0.2.0.dev0/tests/test_convert_hf_checkpoint.py` & `litgpt-0.3.0/tests/test_convert_hf_checkpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
 
 from unittest import mock
 
 import pytest
 import torch
 
+from litgpt import Config
+from litgpt.scripts.convert_hf_checkpoint import convert_hf_checkpoint, copy_weights_hf_llama
 
-def test_llama2_70b_conversion():
-    from litgpt import Config
-    from litgpt.scripts.convert_hf_checkpoint import copy_weights_hf_llama
 
+def test_llama2_70b_conversion():
     shapes = {
         "model.embed_tokens.weight": (32000, 8192),
         "model.layers.0.input_layernorm.weight": (8192,),
         "model.layers.0.mlp.down_proj.weight": (8192, 28672),
         "model.layers.0.mlp.gate_proj.weight": (28672, 8192),
         "model.layers.0.mlp.up_proj.weight": (28672, 8192),
         "model.layers.0.post_attention_layernorm.weight": (8192,),
@@ -98,25 +98,21 @@
         "transformer.h.5.mlp.fc_1.weight": (28672, 8192),
         "transformer.wte.weight": (32000, 8192),
         "lm_head.weight": (32000, 8192),  # due to weight tying lm_head is in the converted weights
     }
 
 
 def test_convert_hf_checkpoint(tmp_path):
-    from litgpt.scripts.convert_hf_checkpoint import convert_hf_checkpoint
-
     with pytest.raises(ValueError, match="to contain .bin"):
         convert_hf_checkpoint(checkpoint_dir=tmp_path, model_name="pythia-14m")
 
     bin_file = tmp_path / "foo.bin"
     bin_file.touch()
     with mock.patch("litgpt.scripts.convert_hf_checkpoint.lazy_load") as load:
         convert_hf_checkpoint(checkpoint_dir=tmp_path, model_name="pythia-14m")
     load.assert_called_with(bin_file)
 
     assert {p.name for p in tmp_path.glob("*")} == {"foo.bin", "model_config.yaml", "lit_model.pth"}
 
     # ensure that the config dict can be loaded
-    from litgpt import Config
-
     config = Config.from_file(tmp_path / "model_config.yaml")
     assert isinstance(config, Config)
```

### Comparing `litgpt-0.2.0.dev0/tests/test_convert_lit_checkpoint.py` & `litgpt-0.3.0/tests/test_convert_lit_checkpoint.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,28 +6,40 @@
 from unittest.mock import ANY
 from urllib.request import urlretrieve
 
 import pytest
 import torch
 import yaml
 from conftest import RunIf
-
-wd = Path(__file__).parent.parent.absolute()
+from transformers import AutoConfig, AutoModelForCausalLM
+from transformers.models.falcon import FalconConfig, FalconForCausalLM
+from transformers.models.gemma import GemmaConfig, GemmaForCausalLM
+from transformers.models.gpt_neox import GPTNeoXConfig, GPTNeoXForCausalLM
+from transformers.models.llama import LlamaConfig, LlamaForCausalLM
+from transformers.models.mixtral import MixtralConfig, MixtralForCausalLM
+
+from litgpt import GPT, Config
+from litgpt.scripts.convert_lit_checkpoint import (
+    check_conversion_supported,
+    convert_lit_checkpoint,
+    copy_weights_falcon,
+    copy_weights_gpt_neox,
+    copy_weights_llama,
+    copy_weights_phi,
+    qkv_split,
+)
 
 
 def test_convert_lit_checkpoint(tmp_path):
-    from litgpt import GPT, Config
-    from litgpt.scripts.convert_lit_checkpoint import convert_lit_checkpoint
-
     ours_config = Config.from_name("Llama-2-7b-hf", block_size=8, n_layer=2, n_embd=32, n_head=2, padding_multiple=128)
     ours_model = GPT(ours_config)
     checkpoint_path = tmp_path / "lit_model.pth"
     config_path = tmp_path / "model_config.yaml"
     torch.save(ours_model.state_dict(), checkpoint_path)
-    with open(config_path, "w") as fp:
+    with open(config_path, "w", encoding="utf-8") as fp:
         yaml.dump(asdict(ours_config), fp)
     output_dir = tmp_path / "out_dir"
 
     convert_lit_checkpoint(checkpoint_path.parent, output_dir)
     assert set(os.listdir(tmp_path)) == {"lit_model.pth", "model_config.yaml", "out_dir"}
     assert os.path.isfile(output_dir / "model.pth")
 
@@ -36,20 +48,14 @@
     convert_lit_checkpoint(checkpoint_path.parent, output_dir)
     converted_sd = torch.load(output_dir / "model.pth")
     assert "model" not in converted_sd
 
 
 @torch.inference_mode()
 def test_against_falcon_40b():
-    from transformers.models.falcon.configuration_falcon import FalconConfig
-    from transformers.models.falcon.modeling_falcon import FalconForCausalLM
-
-    from litgpt import GPT, Config
-    from litgpt.scripts.convert_lit_checkpoint import copy_weights_falcon as copy_to_theirs
-
     ours_config = Config.from_name("falcon-40b", n_layer=2, n_head=8, n_query_groups=4, n_embd=32)
     theirs_config = FalconConfig(
         vocab_size=ours_config.padded_vocab_size,
         hidden_size=ours_config.n_embd,
         num_hidden_layers=ours_config.n_layer,
         num_attention_heads=ours_config.n_head,
         num_kv_heads=ours_config.n_query_groups,
@@ -57,34 +63,29 @@
         parallel_attn=ours_config.parallel_residual,
         bias=ours_config.bias,
     )
 
     ours_model = GPT(ours_config)
     ours_state_dict = ours_model.state_dict()
     theirs_state_dict = {}
-    copy_to_theirs("40b", theirs_state_dict, ours_state_dict)
+    copy_weights_falcon("40b", theirs_state_dict, ours_state_dict)
 
     theirs_model = FalconForCausalLM(theirs_config)
     # assign must be set to True for torch.testing.assert_close to pass
     theirs_model.load_state_dict(theirs_state_dict, assign=True)
 
     # test end to end
     x = torch.tensor([[9856, 23, 491, 1536, 304]], dtype=torch.int32)
     ours_y = ours_model(x)
     theirs_y = theirs_model(x)["logits"]
     torch.testing.assert_close(ours_y, theirs_y)
 
 
 @torch.inference_mode()
 def test_against_original_gpt_neox():
-    from transformers import GPTNeoXConfig, GPTNeoXForCausalLM
-
-    from litgpt import GPT, Config
-    from litgpt.scripts.convert_lit_checkpoint import copy_weights_gpt_neox as copy_to_theirs
-
     ours_config = Config(block_size=64, vocab_size=100, n_layer=4, n_head=8, n_embd=16)
     assert ours_config.padded_vocab_size == 512
     theirs_config = GPTNeoXConfig(
         hidden_act="gelu",
         hidden_size=ours_config.n_embd,
         num_attention_heads=ours_config.n_head,
         num_hidden_layers=ours_config.n_layer,
@@ -97,15 +98,15 @@
         vocab_size=ours_config.padded_vocab_size,
         use_parallel_residual=ours_config.parallel_residual,
     )
 
     ours_model = GPT(ours_config)
     ours_state_dict = ours_model.state_dict()
     theirs_state_dict = {}
-    copy_to_theirs(theirs_state_dict, ours_state_dict)
+    copy_weights_gpt_neox(theirs_state_dict, ours_state_dict)
     theirs_model = GPTNeoXForCausalLM(theirs_config)
     # strict=False because we don't save the rotary embeddings inv frequency
     keys = theirs_model.load_state_dict(theirs_state_dict, strict=False)
     assert not keys.unexpected_keys
     assert all("inv_freq" in k for k in keys.missing_keys)
 
     # test end to end
@@ -116,20 +117,14 @@
 
 
 @torch.inference_mode()
 @pytest.mark.parametrize(
     "ours_kwargs", [{"name": "Llama-2-7b-hf"}, {"name": "CodeLlama-7b-hf"}, {"name": "Llama-2-70b-chat-hf"}]
 )
 def test_against_hf_llama2(ours_kwargs):
-    from transformers.models.llama.configuration_llama import LlamaConfig
-    from transformers.models.llama.modeling_llama import LlamaForCausalLM
-
-    from litgpt import GPT, Config
-    from litgpt.scripts.convert_lit_checkpoint import copy_weights_llama
-
     ours_config = Config.from_name(
         padded_vocab_size=10000, n_layer=2, n_head=8, n_embd=32, intermediate_size=86, **ours_kwargs
     )
     T = 5
     theirs_config = LlamaConfig(
         vocab_size=ours_config.padded_vocab_size,
         hidden_size=ours_config.n_embd,
@@ -155,19 +150,14 @@
     ours_y = ours_model(x)
     theirs_y = theirs_model(x)["logits"]
     torch.testing.assert_close(ours_y, theirs_y)
 
 
 @torch.inference_mode()
 def test_against_mixtral():
-    from transformers.models.mixtral import MixtralConfig, MixtralForCausalLM
-
-    from litgpt import GPT, Config
-    from litgpt.scripts.convert_lit_checkpoint import copy_weights_llama
-
     ours_config = Config.from_name(
         "Mixtral-8x7B-Instruct-v0.1",
         padded_vocab_size=10000,
         n_layer=2,
         n_embd=32,
         n_head=8,
         n_query_groups=2,
@@ -201,20 +191,14 @@
     ours_y = ours_model(x)
     theirs_y = theirs_model(x)["logits"]
     torch.testing.assert_close(ours_y, theirs_y)
 
 
 @torch.inference_mode()
 def test_against_original_open_llama_3b():
-    from transformers.models.llama.configuration_llama import LlamaConfig
-    from transformers.models.llama.modeling_llama import LlamaForCausalLM
-
-    from litgpt import GPT, Config
-    from litgpt.scripts.convert_lit_checkpoint import copy_weights_llama
-
     ours_config = Config.from_name("open_llama_3b", n_layer=2, n_head=8, n_embd=32, intermediate_size=86)
     T = 5
     theirs_config = LlamaConfig(
         hidden_size=ours_config.n_embd,
         num_attention_heads=ours_config.n_head,
         num_hidden_layers=ours_config.n_layer,
         intermediate_size=ours_config.intermediate_size,
@@ -234,85 +218,21 @@
     assert x.size(1) == T
     ours_y = ours_model(x)
     theirs_y = theirs_model(x)["logits"]
     torch.testing.assert_close(ours_y, theirs_y)
 
 
 @torch.inference_mode()
-def test_against_hf_phi_1_5():
-    workdir = wd / "tests" / "reference_models"
-    workdir.mkdir(parents=True, exist_ok=True)
-    file_paths = [workdir / "original_phi_1_5.py", workdir / "configuration_phi.py"]
-    urls = [
-        "https://huggingface.co/microsoft/phi-1_5/raw/main/modeling_phi.py",
-        "https://huggingface.co/microsoft/phi-1_5/raw/main/configuration_phi.py",
-    ]
-    for file_path, url in zip(file_paths, urls):
-        if not file_path.is_file():
-            urlretrieve(url=url, filename=file_path)
-
-    from reference_models.configuration_phi import PhiConfig
-    from reference_models.original_phi_1_5 import PhiForCausalLM
-
-    from litgpt import GPT, Config
-    from litgpt.scripts.convert_lit_checkpoint import copy_weights_phi
+@pytest.mark.parametrize("model_name", ("phi-1_5", "phi-2"))
+def test_against_hf_phi(model_name):
+    from transformers.models.phi.configuration_phi import PhiConfig
+    from transformers.models.phi.modeling_phi import PhiForCausalLM
 
     ours_config = Config.from_name(
-        "phi-1_5", padded_vocab_size=10000, n_layer=2, n_head=4, n_embd=256, rotary_percentage=0.5
-    )
-    T = 5
-    theirs_config = PhiConfig(
-        vocab_size=ours_config.padded_vocab_size,
-        max_position_embeddings=ours_config.block_size,
-        hidden_size=ours_config.n_embd,
-        intermediate_size=ours_config.intermediate_size,
-        num_attention_heads=ours_config.n_head,
-        num_hidden_layers=ours_config.n_layer,
-        partial_rotary_factor=ours_config.rotary_percentage,
-    )
-
-    ours_model = GPT(ours_config)
-    ours_state_dict = ours_model.state_dict()
-    theirs_state_dict = {}
-    copy_weights_phi(ours_config, theirs_state_dict, ours_state_dict)
-    theirs_model = PhiForCausalLM(theirs_config)
-    # strict=False because we don't save the rotary embeddings inv frequency
-    keys = theirs_model.load_state_dict(theirs_state_dict, strict=False)
-    assert not keys.unexpected_keys
-    assert all("inv_freq" in k for k in keys.missing_keys)
-
-    # test end to end
-    x = torch.tensor([[9856, 23, 491, 1536, 304]], dtype=torch.int32)
-    assert x.size(1) == T
-    ours_y = ours_model(x)
-    theirs_y = theirs_model(x)["logits"]
-    torch.testing.assert_close(ours_y, theirs_y)
-
-
-@torch.inference_mode()
-def test_against_hf_phi_2():
-    workdir = wd / "tests" / "reference_models"
-    workdir.mkdir(parents=True, exist_ok=True)
-    file_paths = [workdir / "original_phi_2.py", workdir / "configuration_phi.py"]
-    urls = [
-        "https://huggingface.co/microsoft/phi-2/raw/main/modeling_phi.py",
-        "https://huggingface.co/microsoft/phi-2/raw/main/configuration_phi.py",
-    ]
-    for file_path, url in zip(file_paths, urls):
-        if not file_path.is_file():
-            urlretrieve(url=url, filename=file_path)
-
-    from reference_models.configuration_phi import PhiConfig
-    from reference_models.original_phi_2 import PhiForCausalLM
-
-    from litgpt import GPT, Config
-    from litgpt.scripts.convert_lit_checkpoint import copy_weights_phi
-
-    ours_config = Config.from_name(
-        "phi-2", padded_vocab_size=10000, n_layer=2, n_head=4, n_embd=256, rotary_percentage=0.5
+        model_name, padded_vocab_size=10000, n_layer=2, n_head=4, n_embd=256, rotary_percentage=0.5
     )
     T = 5
     theirs_config = PhiConfig(
         vocab_size=ours_config.padded_vocab_size,
         max_position_embeddings=ours_config.block_size,
         hidden_size=ours_config.n_embd,
         intermediate_size=ours_config.intermediate_size,
@@ -337,19 +257,14 @@
     ours_y = ours_model(x)
     theirs_y = theirs_model(x)["logits"]
     torch.testing.assert_close(ours_y, theirs_y)
 
 
 @torch.inference_mode()
 def test_against_original_stablelm_zephyr_3b():
-    from transformers import AutoConfig, AutoModelForCausalLM
-
-    from litgpt import GPT, Config
-    from litgpt.scripts.convert_lit_checkpoint import copy_weights_llama
-
     T = 5
     ours_config = Config.from_name("stablelm-zephyr-3b", n_layer=2, n_head=16, n_embd=32, intermediate_size=86)
     theirs_config = AutoConfig.from_pretrained(
         "stabilityai/stablelm-zephyr-3b",
         trust_remote_code=True,
         num_hidden_layers=ours_config.n_layer,
         num_attention_heads=ours_config.n_head,
@@ -390,20 +305,14 @@
                 pytest.mark.xfail(raises=AssertionError, strict=False),
                 RunIf(min_cuda_gpus=1),
             ],
         ),
     ],
 )
 def test_against_original_gemma(model_name, device, dtype):
-    from transformers.models.gemma.configuration_gemma import GemmaConfig
-    from transformers.models.gemma.modeling_gemma import GemmaForCausalLM
-
-    from litgpt import GPT, Config
-    from litgpt.scripts.convert_lit_checkpoint import copy_weights_llama
-
     torch.set_default_dtype(dtype)
 
     T = 5
     ours_config = Config.from_name(model_name, n_layer=2, n_head=16, n_embd=32, intermediate_size=86)
     theirs_config = GemmaConfig(
         vocab_size=ours_config.padded_vocab_size,
         hidden_size=ours_config.n_embd,
@@ -435,37 +344,30 @@
     assert x.size(1) == T
     ours_y = ours_model(x)
     theirs_y = theirs_model(x)["logits"].to(dtype)  # HF converts logits to float
     torch.testing.assert_close(ours_y, theirs_y)
 
 
 def test_check_conversion_supported_adapter():
-    from litgpt.scripts.convert_lit_checkpoint import check_conversion_supported
-
     lit_weights = {"some.key.name": ANY, "error.key.gating_factor": ANY}
     with pytest.raises(NotImplementedError, match="Converting adapter"):
         check_conversion_supported(lit_weights=lit_weights)
 
     lit_weights = {"some.key.name": ANY, "error.key.adapter_bias": ANY}
     with pytest.raises(NotImplementedError, match="Converting adapter"):
         check_conversion_supported(lit_weights=lit_weights)
 
 
 def test_check_conversion_supported_lora():
-    from litgpt.scripts.convert_lit_checkpoint import check_conversion_supported
-
     lit_weights = {"some.key.name": ANY, "error.key.lora": ANY}
     with pytest.raises(ValueError, match=r"LoRA.*cannot be converted"):
         check_conversion_supported(lit_weights=lit_weights)
 
 
 def test_qkv_split():
-    from litgpt import Config
-    from litgpt.scripts.convert_lit_checkpoint import qkv_split
-
     # MHA
     config = Config(n_embd=4, n_head=4)
     qkv = torch.tensor(
         [
             [0, 1, 2, 3],
             [4, 5, 6, 7],
             [8, 9, 10, 11],
```

### Comparing `litgpt-0.2.0.dev0/tests/test_convert_pretrained_checkpoint.py` & `litgpt-0.3.0/tests/test_convert_pretrained_checkpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
 
 import os
 
 import torch
 
+from litgpt.scripts.convert_pretrained_checkpoint import convert_pretrained_checkpoint
 
-def test_convert_pretrained_checkpoint(tmp_path, fake_checkpoint_dir):
-    from litgpt.scripts.convert_pretrained_checkpoint import convert_pretrained_checkpoint
 
+def test_convert_pretrained_checkpoint(tmp_path, fake_checkpoint_dir):
     # Pretend we made a checkpoint from pretraining
     pretrained_checkpoint = {
         "model": {"some.module.weight": torch.rand(2, 2), "_orig_mod.some.other.module.weight": torch.rand(2, 2)},
         "the_optimizer": "optimizer_state",
         "other": 1,
     }
     torch.save(pretrained_checkpoint, fake_checkpoint_dir / "lit_model.pth")
```

### Comparing `litgpt-0.2.0.dev0/tests/test_full.py` & `litgpt-0.3.0/tests/test_full.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 import os
 from contextlib import redirect_stdout
 from io import StringIO
 from unittest import mock
 from unittest.mock import Mock
 
 import torch
+import yaml
+
+import litgpt.finetune.full as module
+from litgpt.args import EvalArgs, TrainArgs
+from litgpt.data import Alpaca
 
 
 @mock.patch.dict(os.environ, {"LT_ACCELERATOR": "cpu"})
 def test_full_script(tmp_path, fake_checkpoint_dir, monkeypatch, alpaca_path):
-    import litgpt.finetune.full as module
-    from litgpt.args import EvalArgs, TrainArgs
-    from litgpt.config import name_to_config
-    from litgpt.data import Alpaca
-
     model_config = dict(block_size=128, n_layer=2, n_embd=8, n_head=4, padded_vocab_size=8)
-    monkeypatch.setitem(name_to_config, "tmp", model_config)
+    (fake_checkpoint_dir / "model_config.yaml").write_text(yaml.dump(model_config))
     monkeypatch.setattr(module, "load_checkpoint", Mock())
 
     tokenizer_mock = Mock()
     tokenizer_mock.return_value = tokenizer_mock
     tokenizer_mock.encode = lambda *_, **__: torch.tensor([3, 2, 1])
     monkeypatch.setattr(module, "Tokenizer", tokenizer_mock)
 
@@ -51,15 +51,16 @@
             "hyperparameters.yaml",
             "prompt_style.yaml",
         }
     assert (out_dir / "logs" / "csv" / "version_0" / "metrics.csv").is_file()
 
     logs = stdout.getvalue()
     assert logs.count("(step)") == 6
-    assert logs.count("val loss") == 3
+    assert logs.count("val loss") == 4  # 3 validations + 1 final validation
+    assert logs.count("Final evaluation") == 1
     assert "of trainable parameters: 1,888" in logs
 
     # Resume training and do 2 steps more
     setup_kwargs["train"].max_steps = 8
     setup_kwargs["resume"] = True
     stdout = StringIO()
     with redirect_stdout(stdout), mock.patch("sys.argv", ["full.py"]):
```

### Comparing `litgpt-0.2.0.dev0/tests/test_generate.py` & `litgpt-0.3.0/tests/test_generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 from unittest import mock
 from unittest.mock import ANY, Mock, call
 
 import pytest
 import torch
 import yaml
 
+import litgpt.generate.base as generate
+from litgpt import GPT, Config
+from litgpt.generate.base import sample
+
 
 @pytest.mark.parametrize(
     "max_seq_length", (pytest.param(10, marks=pytest.mark.xfail(raises=NotImplementedError, strict=True)), 20 + 5)
 )
 def test_generate(max_seq_length):
-    import litgpt.generate.base as generate
-    from litgpt import GPT, Config
-
     T = 5
     input_idx = torch.randint(10, size=(T,))
 
     config = Config(block_size=128, vocab_size=16, n_layer=1, n_head=4, n_embd=8)
     model = GPT(config)
     model.max_seq_length = max_seq_length
     model.set_kv_cache(batch_size=1)
@@ -43,16 +44,14 @@
     multinomial_results = torch.hstack(multinomial_results)
     expected = torch.cat((input_idx, multinomial_results))
     assert out.shape == expected.shape
     torch.testing.assert_close(out, expected)
 
 
 def test_main(fake_checkpoint_dir, monkeypatch, tensor_like):
-    import litgpt.generate.base as generate
-
     config_path = fake_checkpoint_dir / "model_config.yaml"
     config = {"block_size": 128, "vocab_size": 50, "n_layer": 2, "n_head": 4, "n_embd": 8, "rotary_percentage": 1}
     config_path.write_text(yaml.dump(config))
 
     module_mock = Mock()
     module_mock.config.block_size = 128
     load_mock = Mock()
@@ -94,16 +93,14 @@
     output = subprocess.check_output(args)
     output = str(output.decode())
     assert "Generates text samples" in output
 
 
 @pytest.mark.parametrize("temperature", (0.0, 1.0, 0.5))
 def test_sample(temperature):
-    from litgpt.generate.base import sample
-
     # shape: 2x3x5
     logits = torch.tensor(
         [
             [[24, 4, 98, 77, 47], [65, 70, 32, 67, 24], [92, 32, 88, 36, 62]],
             [[85, 79, 57, 68, 50], [89, 46, 72, 45, 32], [68, 96, 68, 24, 36]],
         ]
     )
```

### Comparing `litgpt-0.2.0.dev0/tests/test_generate_adapter.py` & `litgpt-0.3.0/tests/test_generate_adapter.py`

 * *Files identical despite different names*

### Comparing `litgpt-0.2.0.dev0/tests/test_generate_sequentially.py` & `litgpt-0.3.0/tests/test_generate_sequentially.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,42 +10,42 @@
 
 import pytest
 import torch
 import yaml
 from conftest import RunIf
 from lightning import Fabric
 
+from litgpt import Config
+from litgpt.generate.sequentially import layer_to_device, replace_device, sequential
+from litgpt.model import GPT, Block
+from litgpt.scripts.download import download_from_hub
+
 
 @pytest.mark.parametrize(
     ("n_layer", "devices", "expected"),
     [
         (6, 2, {0: 0, 1: 0, 2: 0, 3: 1, 4: 1, 5: 1}),
         (6, 3, {0: 0, 1: 0, 2: 1, 3: 1, 4: 2, 5: 2}),
         (6, 1, {0: 0, 1: 0, 2: 0, 3: 0, 4: 0, 5: 0}),
     ],
 )
 def test_layer_to_device(n_layer, devices, expected):
-    from litgpt.generate.sequentially import layer_to_device
-    from litgpt.model import GPT, Block
-
     with torch.device("meta"):
         model = GPT.from_name("pythia-14m", n_layer=n_layer)
 
     actual = layer_to_device(model, Block, chunk_size=n_layer // devices)
     expected = {f"transformer.h.{i}": v for i, v in expected.items()}
     assert actual == expected
 
 
 def path_to_device(model):
     return {k: str(v.device) for k, v in itertools.chain(model.named_parameters(), model.named_buffers())}
 
 
 def test_replace_device():
-    from litgpt.generate.sequentially import replace_device
-
     class Submodule(torch.nn.Module):
         def __init__(self):
             super().__init__()
             self.register_buffer("foo", torch.tensor(1, device="cpu"))
             self.register_buffer("bar", torch.tensor(1, device="cpu"))
 
     class MyModel(torch.nn.Module):
@@ -82,17 +82,14 @@
         ValueError,
         match=escape("multiple devices: {'submodule.foo': device(type='cpu'), 'submodule.bar': device(type='meta')}"),
     ):
         replace_device(model, torch.device("cpu"), torch.device("meta"))
 
 
 def _test_model_1device(accelerator):
-    from litgpt import GPT
-    from litgpt.generate.sequentially import sequential
-
     fabric = Fabric(accelerator=accelerator, devices=1)
     with torch.device("meta"):
         model = GPT.from_name("pythia-14m", n_layer=2)
     model = sequential(model, fabric.device, 15, 1)
 
     device_str = str(fabric.device)
     assert path_to_device(model) == {
@@ -153,17 +150,14 @@
             hook_data = ("forward_hook", hook.func.__name__, hook.args, hook.keywords)
             mapping[name].append(hook_data)
     return dict(mapping)
 
 
 @RunIf(min_cuda_gpus=2)
 def test_model_forward_hooks():
-    from litgpt import GPT
-    from litgpt.generate.sequentially import sequential
-
     fabric = Fabric(accelerator="cuda", devices=1)
     with torch.device("meta"):
         model = GPT.from_name("pythia-14m")  # 6 layers
     model = sequential(model, fabric.device, max_seq_length=15, devices=2)
 
     hooks = find_forward_hooks(model)
     actual = path_to_device(model)
@@ -270,17 +264,14 @@
 
 
 root = Path(__file__).parent.parent.resolve()
 
 
 @RunIf(min_cuda_gpus=2)
 def test_base_with_sequentially(tmp_path):
-    from litgpt import GPT, Config
-    from litgpt.scripts.download import download_from_hub
-
     # download the tokenizer
     download_from_hub(repo_id="EleutherAI/pythia-14m", tokenizer_only=True, checkpoint_dir=tmp_path)
     checkpoint_dir = tmp_path / "EleutherAI/pythia-14m"
     # save the config
     config = Config.from_name("pythia-14m")
     (checkpoint_dir / "model_config.yaml").write_text(yaml.dump(asdict(config)))
     # create a state dict to load from
```

### Comparing `litgpt-0.2.0.dev0/tests/test_generate_tp.py` & `litgpt-0.3.0/tests/test_generate_tp.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 
 import pytest
 import torch
 import yaml
 from conftest import RunIf
 from test_generate_sequentially import find_forward_hooks
 
+from litgpt import GPT, Config
+from litgpt.generate.tp import tensor_parallel, tensor_parallel_linear
+from litgpt.scripts.download import download_from_hub
 
-def test_tensor_parallel_linear():
-    from litgpt.generate.tp import tensor_parallel_linear
 
+def test_tensor_parallel_linear():
     fabric = Mock()
     fabric.world_size = 4
     fabric.global_rank = 2
 
     def get_linear(bias=True):
         linear = torch.nn.Linear(8, 8, bias=bias)
         linear.weight.data = torch.arange(64, dtype=torch.float32).reshape(8, 8)
@@ -78,17 +80,14 @@
                 "transformer.h.2.mlp.experts.0": [("forward_hook", "all_reduce_output", (8,), {})],
                 "transformer.h.2.mlp.experts.1": [("forward_hook", "all_reduce_output", (8,), {})],
             },
         ),
     ],
 )
 def test_tensor_parallel_llama(name, expected):
-    from litgpt import GPT
-    from litgpt.generate.tp import tensor_parallel
-
     fabric = Mock()
     fabric.world_size = 8
     fabric.global_rank = 1
 
     with torch.device("meta"):
         model = GPT.from_name(name, n_layer=3, n_expert=2)
     config = replace(model.config)  # make a copy
@@ -104,17 +103,14 @@
 
 
 root = Path(__file__).parent.parent.resolve()
 
 
 @RunIf(min_cuda_gpus=2)
 def test_tp(tmp_path):
-    from litgpt import GPT, Config
-    from litgpt.scripts.download import download_from_hub
-
     # download the tokenizer
     download_from_hub(repo_id="EleutherAI/pythia-14m", tokenizer_only=True, checkpoint_dir=tmp_path)
     checkpoint_dir = tmp_path / "EleutherAI/pythia-14m"
     # save the config
     config = Config.from_name("pythia-14m")
     (checkpoint_dir / "model_config.yaml").write_text(yaml.dump(asdict(config)))
     # create a state dict to load from
```

### Comparing `litgpt-0.2.0.dev0/tests/test_lora.py` & `litgpt-0.3.0/tests/test_lora.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,63 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
 import os
-import sys
 from contextlib import redirect_stdout
 from io import StringIO
 from itertools import product
-from pathlib import Path
 from unittest import mock
 from unittest.mock import Mock
 
 import pytest
 import torch
+import yaml
 from conftest import RunIf
 from lightning import Fabric
 from lightning.fabric.plugins.precision.bitsandbytes import _BITSANDBYTES_AVAILABLE, BitsandbytesPrecision
 from lightning.fabric.wrappers import _FabricOptimizer
-
-# support running without installing as a package
-wd = Path(__file__).parent.parent.resolve()
-sys.path.append(str(wd))
+from torch._dynamo.backends import debugging
+from torch.nn import functional as F
+from transformers.models.gemma import GemmaConfig, GemmaForCausalLM
+from transformers.models.mixtral import MixtralConfig, MixtralForCausalLM
 
 import litgpt.config as config_module
+import litgpt.finetune.lora as module
+from litgpt.args import EvalArgs, TrainArgs
+from litgpt.data import Alpaca
+from litgpt.lora import GPT as LoRAGPT
+from litgpt.lora import CausalSelfAttention as LoRACausalSelfAttention
+from litgpt.lora import Config, LoRALinear, LoRAQKVLinear, lora_filter, mark_only_lora_as_trainable, merge_lora_weights
+from litgpt.model import GPT as BaseGPT
+from litgpt.scripts.convert_hf_checkpoint import copy_weights_hf_llama
 
 
 def test_lora_layer_replacement():
-    from litgpt.lora import GPT, Config, LoRALinear
-    from litgpt.lora import CausalSelfAttention as LoRACausalSelfAttention
-
     config = Config(n_layer=2, n_head=4, n_embd=8, block_size=8, vocab_size=8, lora_r=8, lora_alpha=8, lora_dropout=0.1)
-    model = GPT(config)
+    model = LoRAGPT(config)
 
     assert isinstance(model.transformer.h[0].attn, LoRACausalSelfAttention)
     assert isinstance(model.transformer.h[1].attn, LoRACausalSelfAttention)
     assert isinstance(model.lm_head, LoRALinear)
     assert isinstance(model.transformer.h[0].mlp.proj, LoRALinear)
 
 
 def test_lora_merge():
-    from litgpt.lora import GPT, Config, mark_only_lora_as_trainable, merge_lora_weights
-
     config = Config(
         n_layer=1,
         n_head=2,
         n_embd=8,
         block_size=8,
         vocab_size=8,
         lora_r=8,
         lora_alpha=8,
         lora_dropout=0.1,
         lora_query=True,
         lora_value=True,
         lora_projection=True,
     )
-    model = GPT(config)
+    model = LoRAGPT(config)
     model.train()
     attn_proj = model.transformer.h[0].attn.proj
 
     initial_weight = attn_proj.linear.weight.clone()
     assert torch.equal(attn_proj.linear.weight, initial_weight)
 
     # perform an update to the LoRA weights
@@ -78,31 +80,29 @@
 
     # check that `W_after = W_initial + (A x B)`
     delta_w = attn_proj.get_lora_AB()
     torch.testing.assert_close(weight_after, initial_weight + delta_w)
 
 
 def test_lora_mqa_gqa():
-    from litgpt.lora import GPT, Config
-
     # MHA
     config = Config(
         n_layer=1,
         n_head=4,
         n_embd=8,
         block_size=1,
         vocab_size=1,
         lora_r=2,
         lora_alpha=8,
         lora_dropout=0.1,
         lora_query=True,
         lora_value=True,
     )
     assert config.n_query_groups == config.n_head
-    model = GPT(config)
+    model = LoRAGPT(config)
     attn = model.transformer.h[0].attn.attn
     for p in attn.linear.parameters():
         torch.nn.init.zeros_(p)
     torch.nn.init.ones_(attn.lora_B)
     lora_ind = [0, 1, 6, 7, 12, 13, 18, 19, 4, 5, 10, 11, 16, 17, 22, 23]
     assert attn.linear.weight.shape == (24, 8)
     assert attn.lora_A.shape == (4, 8)
@@ -115,15 +115,15 @@
     out = attn(x_in)
     non_lora_ind = list(set(range(24)).difference(lora_ind))
     assert torch.count_nonzero(out[:, :, lora_ind]) == bsz * ctx_len * len(lora_ind)
     assert torch.count_nonzero(out[:, :, non_lora_ind]) == 0
 
     # MQA
     config.n_query_groups = 1
-    model = GPT(config)
+    model = LoRAGPT(config)
     attn = model.transformer.h[0].attn.attn
     for p in attn.linear.parameters():
         torch.nn.init.zeros_(p)
     torch.nn.init.ones_(attn.lora_B)
     lora_ind = [0, 1, 2, 3, 4, 5, 6, 7, 10, 11]
     assert attn.linear.weight.shape == (12, 8)
     assert attn.lora_A.shape == (4, 8)
@@ -136,15 +136,15 @@
     out = attn(x_in)
     non_lora_ind = list(set(range(12)).difference(lora_ind))
     assert torch.count_nonzero(out[:, :, lora_ind]) == bsz * ctx_len * len(lora_ind)
     assert torch.count_nonzero(out[:, :, non_lora_ind]) == 0
 
     # GQA
     config.n_query_groups = 2
-    model = GPT(config)
+    model = LoRAGPT(config)
     attn = model.transformer.h[0].attn.attn
     for p in attn.linear.parameters():
         torch.nn.init.zeros_(p)
     torch.nn.init.ones_(attn.lora_B)
     lora_ind = [0, 1, 2, 3, 8, 9, 10, 11, 6, 7, 14, 15]
     assert attn.linear.weight.shape == (16, 8)
     assert attn.lora_A.shape == (4, 8)
@@ -157,18 +157,16 @@
     out = attn(x_in)
     non_lora_ind = list(set(range(16)).difference(lora_ind))
     assert torch.count_nonzero(out[:, :, lora_ind]) == bsz * ctx_len * len(lora_ind)
     assert torch.count_nonzero(out[:, :, non_lora_ind]) == 0
 
 
 def test_lora_filter(tmp_path):
-    from litgpt.lora import GPT, lora_filter
-
     fabric = Fabric(devices=1)
-    model = GPT.from_name("pythia-14m", n_layer=3, lora_r=1, lora_query=True, lora_value=True)
+    model = LoRAGPT.from_name("pythia-14m", n_layer=3, lora_r=1, lora_query=True, lora_value=True)
     save_path = tmp_path / "model.pth"
     fabric.save(save_path, {"model": model}, filter={"model": lora_filter})
     saved = torch.load(save_path)["model"]
 
     expected = {
         "transformer.h.1.attn.attn.lora_B",
         "transformer.h.2.attn.attn.lora_B",
@@ -178,21 +176,16 @@
         "transformer.h.0.attn.attn.lora_B",
     }
     assert set(saved) == expected
 
 
 @mock.patch.dict(os.environ, {"LT_ACCELERATOR": "cpu"})
 def test_lora_script(tmp_path, fake_checkpoint_dir, monkeypatch, alpaca_path):
-    import litgpt.finetune.lora as module
-    from litgpt.args import EvalArgs, TrainArgs
-    from litgpt.config import name_to_config
-    from litgpt.data import Alpaca
-
     model_config = dict(block_size=128, n_layer=2, n_embd=8, n_head=4, padded_vocab_size=8)
-    monkeypatch.setitem(name_to_config, "tmp", model_config)
+    (fake_checkpoint_dir / "model_config.yaml").write_text(yaml.dump(model_config))
     monkeypatch.setattr(module, "load_checkpoint", Mock())
     monkeypatch.setattr(module, "merge_lora", Mock())
 
     tokenizer_mock = Mock()
     tokenizer_mock.return_value = tokenizer_mock
     tokenizer_mock.encode = lambda *_, **__: torch.tensor([3, 2, 1])
     monkeypatch.setattr(module, "Tokenizer", tokenizer_mock)
@@ -224,30 +217,29 @@
             "hyperparameters.yaml",
             "prompt_style.yaml",
         }
     assert (out_dir / "logs" / "csv" / "version_0" / "metrics.csv").is_file()
 
     logs = stdout.getvalue()
     assert logs.count("(step)") == 6
-    assert logs.count("val loss") == 3
+    assert logs.count("val loss") == 4  # 3 validations + 1 final validation
+    assert logs.count("Final evaluation") == 1
     assert "of trainable parameters: 512" in logs
 
 
 def test_lora_init_when_linear_overridden():
-    from litgpt.lora import LoRAQKVLinear
-
     class MyLinear(torch.nn.Linear):
         def __init__(self, *args, **kwargs):
             # this needs to be implemented to demonstrate the failure
             super().__init__(*args, **kwargs)
 
     original_linear = torch.nn.Linear
     # Our bnb does this sort of monkey patching
     torch.nn.Linear = MyLinear
-    layer = LoRAQKVLinear(1, 1, 1, 1)
+    layer = LoRAQKVLinear(1, 1, 1, 1, 1)
     assert isinstance(layer.linear, original_linear)
     torch.nn.Linear = original_linear
 
 
 @pytest.mark.parametrize(
     ("apply_to", "target_layer_names", "mlp_class_name"),
     (
@@ -256,30 +248,28 @@
         ("lora_head", "lm_head", "GptNeoxMLP"),
         ("lora_projection", "transformer.h.0.attn.proj", "LLaMAMLP"),
         ("lora_mlp", {"transformer.h.0.mlp.fc_1", "transformer.h.0.mlp.fc_2", "transformer.h.0.mlp.proj"}, "LLaMAMLP"),
         ("lora_head", "lm_head", "LLaMAMLP"),
     ),
 )
 def test_lora_linear_utilization(apply_to, target_layer_names, mlp_class_name):
-    from litgpt.lora import GPT, Config
-
     config = Config(
         n_layer=1,
         n_head=4,
         n_embd=8,
         block_size=1,
         vocab_size=1,
         lora_r=2,
         lora_alpha=8,
         lora_dropout=0.1,
         mlp_class_name=mlp_class_name,
         intermediate_size=8 * 3,
         **{apply_to: True},
     )
-    model = GPT(config)
+    model = LoRAGPT(config)
     state_dict = model.state_dict()
 
     if isinstance(target_layer_names, str):
         target_layer_names = {target_layer_names}
     lora_sublayers = (".lora_A", ".lora_B")
 
     # check that all the target layers have LoRA weights
@@ -294,32 +284,28 @@
 
 
 @torch.inference_mode()
 @pytest.mark.parametrize(
     "apply_to", (None, "lora_query", "lora_key", "lora_value", "lora_projection", "lora_mlp", "lora_head")
 )
 def test_lora_gpt_apply_lora_forward_no_exception(apply_to):
-    from litgpt.lora import GPT, Config
-
     config = Config(n_layer=1, n_head=4, n_embd=8, block_size=1, vocab_size=1, lora_r=2, lora_alpha=8, lora_dropout=0.1)
     if apply_to:
         setattr(config, apply_to, True)
     input_ids = torch.tensor([[1]])
-    model = GPT(config)
+    model = LoRAGPT(config)
     model.eval()
 
     model(input_ids)
 
 
 @torch.inference_mode()
 @pytest.mark.parametrize("n_query_groups", (1, 2, 3, 6))
 @pytest.mark.parametrize("apply_to", product((False, True), repeat=3))
 def test_lora_gpt_query_groups_merge_and_forward_no_exception(n_query_groups, apply_to):
-    from litgpt.lora import GPT, Config, merge_lora_weights
-
     keys = ("lora_query", "lora_key", "lora_value")
     values = apply_to
     apply_to = dict(zip(keys, values))
 
     config = Config(
         n_layer=1,
         n_head=6,
@@ -328,41 +314,40 @@
         vocab_size=1,
         lora_r=2,
         lora_alpha=8,
         lora_dropout=0.1,
         n_query_groups=n_query_groups,
         **apply_to,
     )
-    model = GPT(config)
+    model = LoRAGPT(config)
     merge_lora_weights(model)
     input_ids = torch.tensor([[1]])
     model(input_ids)
 
 
 @torch.inference_mode()
+@pytest.mark.parametrize("head_size", (1, 2, 4))
 @pytest.mark.parametrize("n_head", (1, 2, 3, 6, 12))
 @pytest.mark.parametrize(
     "enable_lora",
     [
         (False, False, True),
         (False, True, False),
         (False, True, True),
         (True, False, False),
         (True, False, True),
         (True, True, False),
         (True, True, True),
     ],
 )
-def test_lora_qkv_linear_compare_conv1d(n_head, enable_lora):
-    from torch.nn import functional as F
-
-    from litgpt.lora import LoRAQKVLinear
-
+def test_lora_qkv_linear_compare_conv1d(head_size, n_head, enable_lora):
     C = 12
-    layer = LoRAQKVLinear(C, 3 * C, n_head=n_head, n_query_groups=n_head, r=2, enable_lora=enable_lora)
+    layer = LoRAQKVLinear(
+        C, 3 * C, head_size=head_size, n_head=n_head, n_query_groups=n_head, r=2, enable_lora=enable_lora
+    )
     x = torch.randn((1, 1, C))
     a = F.linear(x, layer.lora_A).transpose(-2, -1)  # after_A
     b = layer.lora_B.data.unsqueeze(-1)
 
     # original PyTorch conv1d function output
     conv1d_pytorch = F.conv1d(a, b, groups=sum(layer.enable_lora))
 
@@ -375,60 +360,53 @@
 
     assert torch.allclose(conv1d_pytorch, conv1d_custom)
     assert torch.allclose(conv1d_pytorch, conv1d_custom_forced)
 
 
 @pytest.mark.parametrize(("rank", "expected_merged"), ((0, False), (1, True)))
 def test_lora_linear_weights_merged_status(rank, expected_merged):
-    from litgpt.lora import LoRALinear
-
     layer = LoRALinear(10, 10, r=rank)
     assert not layer.merged
     layer.merge()
     assert layer.merged == expected_merged
 
 
 @pytest.mark.parametrize(
     ("rank", "enable_lora", "expected_merged"),
     ((0, True, False), (1, True, True), (0, False, False), (1, False, False)),
 )
 def test_lora_qkv_linear_weights_merged_status(rank, enable_lora, expected_merged):
-    from litgpt.lora import LoRAQKVLinear
-
-    layer = LoRAQKVLinear(10, 3 * 10, n_head=2, n_query_groups=2, r=rank, enable_lora=enable_lora)
+    C = 10
+    layer = LoRAQKVLinear(C, 3 * C, head_size=5, n_head=2, n_query_groups=2, r=rank, enable_lora=enable_lora)
     assert not layer.merged
     layer.merge()
     assert layer.merged == expected_merged
 
 
 @RunIf(min_cuda_gpus=1)
 def test_lora_merge_with_bitsandbytes():
-    from lightning.fabric.plugins.precision.bitsandbytes import _BITSANDBYTES_AVAILABLE, BitsandbytesPrecision
-
     if not _BITSANDBYTES_AVAILABLE:
         pytest.skip("BNB not available")
     import bitsandbytes as bnb
 
-    from litgpt.lora import GPT, Config, mark_only_lora_as_trainable, merge_lora_weights
-
     config = Config(
         n_layer=1,
         n_head=2,
         n_embd=8,
         block_size=8,
         vocab_size=8,
         lora_r=8,
         lora_alpha=8,
         lora_dropout=0.1,
         lora_query=True,
         lora_value=True,
         lora_projection=True,
     )
     fabric = Fabric(devices=1, plugins=BitsandbytesPrecision("nf4", dtype=torch.bfloat16, ignore_modules={"lm_head"}))
-    model = GPT(config)
+    model = LoRAGPT(config)
     mark_only_lora_as_trainable(model)
 
     from bitsandbytes.optim import PagedAdamW
 
     optimizer = PagedAdamW(model.parameters(), lr=1.0)
     model, optimizer = fabric.setup(model, optimizer)
 
@@ -469,33 +447,27 @@
     initial_weight_data = bnb.nn.Params4bit(
         initial_weight_data.to("cpu"), requires_grad=False, **initial_weight_kwargs
     ).to(initial_weight.device)
     torch.testing.assert_close(weight_after, initial_weight_data)
 
 
 def test_lora_gpt_init_weights():
-    from litgpt.lora import GPT, Config
-
     config = Config(n_layer=1, n_head=6, n_embd=12, block_size=1, vocab_size=1, lora_r=2, lora_alpha=8, lora_head=True)
-    model = GPT(config)
+    model = LoRAGPT(config)
     param = model.lm_head.lora_B.data
 
     assert (param == 0).all()
     torch.nn.init.constant_(param, 1.23)
     assert (param != 0).any()
     model.apply(model._init_weights)
     assert (param == 0).all()
 
 
 @pytest.mark.parametrize("name", [c["name"] for c in config_module.configs])
 def test_base_model_can_be_lora_loaded(name):
-    from litgpt.lora import GPT as LoRAGPT
-    from litgpt.lora import lora_filter
-    from litgpt.model import GPT as BaseGPT
-
     kwargs = {"n_layer": 2, "n_head": 8, "n_embd": 16, "padded_vocab_size": 32}
     base_model = BaseGPT.from_name(name, **kwargs)
     base_model_state_dict = base_model.state_dict()
     lora_model = LoRAGPT.from_name(
         name,
         **kwargs,
         lora_r=1,
@@ -511,65 +483,59 @@
     for k in keys.missing_keys:
         assert lora_filter(k, None)
 
 
 @RunIf(dynamo=True)
 @torch.inference_mode()
 def test_lora_compile():
-    from litgpt.lora import GPT
-
-    model = GPT.from_name(
+    model = LoRAGPT.from_name(
         "pythia-14m",
         n_layer=3,
         lora_r=8,
         lora_alpha=8,
         lora_dropout=0.1,
         lora_query=True,
         lora_key=True,
         lora_value=True,
         lora_projection=True,
         lora_mlp=True,
         lora_head=True,
     )
     x = torch.randint(model.config.vocab_size, size=(2, model.config.block_size), dtype=torch.int64)
 
-    from torch._dynamo.backends import debugging
-
     explanation = torch._dynamo.explain(model)(x)
     assert isinstance(explanation, debugging.ExplainOutput)
     assert explanation.graph_count == 1
     assert explanation.graph_break_count == 0
 
-    model = GPT(model.config)
+    model = LoRAGPT(model.config)
     model.set_kv_cache(2)
     input_pos = torch.arange(model.config.block_size)
     explanation = torch._dynamo.explain(model)(x, input_pos)
     assert isinstance(explanation, debugging.ExplainOutput)
     assert explanation.graph_count == 1
     assert explanation.graph_break_count == 0
 
 
 @torch.inference_mode()
 def test_against_hf_mixtral():
-    from transformers.models.mixtral import MixtralConfig, MixtralForCausalLM
-
-    from litgpt.lora import GPT, Config
-    from litgpt.scripts.convert_hf_checkpoint import copy_weights_hf_llama
-
     device = torch.device("cpu")
     dtype = torch.float32
     ours_config = Config.from_name(
         "Mixtral-8x7B-Instruct-v0.1",
         padded_vocab_size=10000,
         n_layer=2,
         n_embd=32,
         n_head=8,
         n_query_groups=2,
         intermediate_size=86,
         n_expert=4,
+        lora_r=1,
+        lora_key=True,
+        lora_value=True,
     )
     T = 5
     theirs_config = MixtralConfig(
         vocab_size=ours_config.padded_vocab_size,
         hidden_size=ours_config.n_embd,
         num_attention_heads=ours_config.n_head,
         num_hidden_layers=ours_config.n_layer,
@@ -582,31 +548,85 @@
     )
     assert ours_config.intermediate_size == theirs_config.intermediate_size
 
     theirs_model = MixtralForCausalLM(theirs_config).to(device)
     theirs_state_dict = theirs_model.state_dict()
     state_dict = {}
     copy_weights_hf_llama(ours_config, {}, state_dict, theirs_state_dict)
-    ours_model = GPT(ours_config).to(device)
-    ours_model.load_state_dict(state_dict)
+    ours_model = LoRAGPT(ours_config).to(device)
+    keys = ours_model.load_state_dict(state_dict, strict=False)
+    assert not keys.unexpected_keys
+    for k in keys.missing_keys:
+        assert lora_filter(k, None)
 
     # test end to end
     x = torch.tensor([[9856, 23, 491, 1536, 304], [23, 345, 65, 123, 321]], dtype=torch.int32, device=device)
     assert x.size(1) == T
     ours_y = ours_model(x)
     theirs_y = theirs_model(x)["logits"].to(dtype)  # HF converts logits to float
     torch.testing.assert_close(ours_y, theirs_y)
 
 
+@torch.inference_mode()
+@pytest.mark.parametrize("model_name", ["gemma-2b", "gemma-7b"])
+def test_against_hf_gemma(model_name):
+    device = torch.device("cpu")
+    dtype = torch.float32
+    T = 5
+    ours_config = Config.from_name(
+        model_name,
+        n_layer=2,
+        n_head=16,
+        n_embd=32,
+        head_size=4,
+        intermediate_size=86,
+        lora_r=1,
+        lora_query=True,
+        lora_key=True,
+        lora_value=True,
+    )
+    theirs_config = GemmaConfig(
+        vocab_size=ours_config.padded_vocab_size,
+        hidden_size=ours_config.n_embd,
+        head_dim=ours_config.head_size,
+        num_attention_heads=ours_config.n_head,
+        num_hidden_layers=ours_config.n_layer,
+        intermediate_size=ours_config.intermediate_size,
+        max_position_embeddings=T,
+        rms_norm_eps=ours_config.norm_eps,
+        num_key_value_heads=ours_config.n_query_groups,
+        rope_theta=ours_config.rope_base,
+        attention_bias=ours_config.bias,
+        tie_word_embeddings=True,
+        hidden_act="gelu_pytorch_tanh",
+    )
+    assert ours_config.intermediate_size == theirs_config.intermediate_size
+
+    theirs_model = GemmaForCausalLM(theirs_config).to(device)
+    theirs_state_dict = theirs_model.state_dict()
+    # Gemma weights are shipped without `lm_head.weight`
+    theirs_state_dict.pop("lm_head.weight")
+    state_dict = {}
+    copy_weights_hf_llama(ours_config, {}, state_dict, theirs_state_dict)
+    ours_model = LoRAGPT(ours_config).to(device)
+    keys = ours_model.load_state_dict(state_dict, strict=False)
+    assert not keys.unexpected_keys
+    for k in keys.missing_keys:
+        assert lora_filter(k, None)
+
+    # test end to end
+    x = torch.tensor([[9856, 23, 491, 1536, 304]], dtype=torch.int32, device=device)
+    assert x.size(1) == T
+    ours_y = ours_model(x)
+    theirs_y = theirs_model(x)["logits"].to(dtype)  # HF converts logits to float
+    torch.testing.assert_close(ours_y, theirs_y)
+
+
 @RunIf(min_cuda_gpus=1)
 def test_lora_bitsandbytes(monkeypatch, tmp_path, fake_checkpoint_dir, alpaca_path):
-    import litgpt.finetune.lora as module
-    from litgpt.config import name_to_config
-    from litgpt.data import Alpaca
-
     if not _BITSANDBYTES_AVAILABLE:
         pytest.skip("BNB not available")
 
     from bitsandbytes.optim import PagedAdamW
 
     model_config = dict(
         block_size=128,
@@ -618,15 +638,15 @@
         lora_r=8,
         lora_alpha=8,
         lora_dropout=0.1,
         lora_query=True,
         lora_value=True,
         lora_projection=True,
     )
-    monkeypatch.setitem(name_to_config, "tmp", model_config)
+    (fake_checkpoint_dir / "model_config.yaml").write_text(yaml.dump(model_config))
 
     tokenizer_mock = Mock()
     tokenizer_mock.return_value = tokenizer_mock
     tokenizer_mock.encode = lambda *_, **__: torch.tensor([3, 2, 1])
     monkeypatch.setattr(module, "Tokenizer", tokenizer_mock)
 
     monkeypatch.setattr(module, "load_checkpoint", Mock())
@@ -708,8 +728,8 @@
             "transformer.h.0.attn.attn.lora_B",
             "transformer.h.1.attn.attn.lora_B",
         }
     }
 
     logs = stdout.getvalue()
     assert "of trainable parameters: 512" in logs
-    assert "of non trainable parameters: 1,888" in logs
+    assert "of non-trainable parameters: 1,888" in logs
```

### Comparing `litgpt-0.2.0.dev0/tests/test_merge_lora.py` & `litgpt-0.3.0/tests/test_merge_lora.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,46 +7,49 @@
 from pathlib import Path
 from unittest import mock
 
 import pytest
 import torch
 import yaml
 
+from litgpt.lora import GPT as LoRAGPT
+from litgpt.lora import lora_filter
+from litgpt.model import GPT
+from litgpt.scripts.merge_lora import load_lora_metadata, merge_lora
 
-@mock.patch.dict(os.environ, {"LT_ACCELERATOR": "cpu"})
-def test_merge_lora(tmp_path, fake_checkpoint_dir):
-    from litgpt.lora import GPT as LoRAGPT
-    from litgpt.lora import lora_filter
-    from litgpt.model import GPT
-    from litgpt.scripts.merge_lora import merge_lora
 
+@mock.patch.dict(os.environ, {"LT_ACCELERATOR": "cpu"})
+@pytest.mark.parametrize(
+    ("pretrained_dtype", "lora_dtype"), [(None, None), (torch.float16, torch.float32), (torch.float16, torch.bfloat16)]
+)
+def test_merge_lora(tmp_path, fake_checkpoint_dir, pretrained_dtype, lora_dtype):
     pretrained_checkpoint_dir = tmp_path / "pretrained"
     lora_checkpoint_dir = tmp_path / "lora"
     shutil.copytree(fake_checkpoint_dir, pretrained_checkpoint_dir)
     shutil.copytree(fake_checkpoint_dir, lora_checkpoint_dir)
     (lora_checkpoint_dir / "lit_model.pth").unlink()  # should not already exist
     shutil.rmtree(tmp_path / "checkpoints")
 
     # Create a fake pretrained checkpoint
     config = dict(block_size=128, padded_vocab_size=256, n_layer=3, n_head=8, n_embd=16)
-    with open(pretrained_checkpoint_dir / "model_config.yaml", "w") as fp:
+    with open(pretrained_checkpoint_dir / "model_config.yaml", "w", encoding="utf-8") as fp:
         yaml.dump(config, fp)
-    base_model = GPT.from_name("pythia-14m", **config)
+    base_model = GPT.from_name("pythia-14m", **config).to(dtype=pretrained_dtype)
     state_dict = base_model.state_dict()
     assert len(state_dict) == 40
     torch.save(state_dict, pretrained_checkpoint_dir / "lit_model.pth")
 
     # Create a fake LoRA checkpoint
     lora_kwargs = dict(lora_r=8, lora_alpha=16, lora_dropout=0.05, lora_query=True, lora_value=True)
-    lora_model = LoRAGPT.from_name("pythia-14m", **config, **lora_kwargs)
+    lora_model = LoRAGPT.from_name("pythia-14m", **config, **lora_kwargs).to(dtype=lora_dtype)
     state_dict = {k: v for k, v in lora_model.state_dict().items() if lora_filter(k, v)}
     assert len(state_dict) == 6
     torch.save(state_dict, lora_checkpoint_dir / "lit_model.pth.lora")
     hparams = dict(checkpoint_dir=str(pretrained_checkpoint_dir), **lora_kwargs)
-    with open(lora_checkpoint_dir / "hyperparameters.yaml", "w") as file:
+    with open(lora_checkpoint_dir / "hyperparameters.yaml", "w", encoding="utf-8") as file:
         yaml.dump(hparams, file)
     shutil.copyfile(pretrained_checkpoint_dir / "model_config.yaml", lora_checkpoint_dir / "model_config.yaml")
 
     assert set(os.listdir(tmp_path)) == {"lora", "pretrained"}
     merge_lora(lora_checkpoint_dir)
     assert set(os.listdir(tmp_path)) == {"lora", "pretrained"}
     assert set(os.listdir(lora_checkpoint_dir)) == {
@@ -68,21 +71,19 @@
     stdout = StringIO()
     with redirect_stdout(stdout):
         merge_lora(lora_checkpoint_dir)
     assert "LoRA weights have already been merged" in stdout.getvalue()
 
 
 def test_load_lora_metadata(fake_checkpoint_dir):
-    from litgpt.scripts.merge_lora import load_lora_metadata
-
     assert not (fake_checkpoint_dir / "hyperparameters.yaml").is_file()
     with pytest.raises(FileNotFoundError, match="missing a `hyperparameters.yaml` file"):
         load_lora_metadata(fake_checkpoint_dir)
 
     hparams = dict(precision="bf16-mixed", checkpoint_dir="checkpoints/meta-llama/Llama-2-7b", lora_r=8, lora_alpha=16)
-    with open(fake_checkpoint_dir / "hyperparameters.yaml", "w") as file:
+    with open(fake_checkpoint_dir / "hyperparameters.yaml", "w", encoding="utf-8") as file:
         yaml.dump(hparams, file)
 
     lora_args, pretrained_dir, precision = load_lora_metadata(fake_checkpoint_dir)
     assert lora_args == dict(lora_r=8, lora_alpha=16)
     assert pretrained_dir == Path("checkpoints/meta-llama/Llama-2-7b")
     assert precision == "bf16-mixed"
```

### Comparing `litgpt-0.2.0.dev0/tests/test_model.py` & `litgpt-0.3.0/tests/test_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,46 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
 
-import sys
 from copy import deepcopy
 from functools import partial
 from pathlib import Path
 from urllib.request import urlretrieve
 
 import pytest
 import torch
 from conftest import RunIf
 from lightning import Fabric
 from lightning.fabric.utilities.imports import _IS_WINDOWS
 from lightning.fabric.utilities.init import _materialize_meta_tensors
-
-# support running without installing as a package
-wd = Path(__file__).parent.parent.resolve()
-sys.path.append(str(wd))
+from torch._dynamo.backends import debugging
+from torch.backends.cuda import (
+    SDPAParams,
+    SDPBackend,
+    can_use_efficient_attention,
+    can_use_flash_attention,
+    flash_sdp_enabled,
+    math_sdp_enabled,
+    mem_efficient_sdp_enabled,
+)
+from transformers import AutoConfig, AutoModelForCausalLM
+from transformers.models.falcon import FalconConfig, FalconForCausalLM
+from transformers.models.gemma import GemmaConfig, GemmaForCausalLM
+from transformers.models.gpt_neox import GPTNeoXConfig, GPTNeoXForCausalLM
+from transformers.models.llama import LlamaConfig, LlamaForCausalLM
+from transformers.models.mistral import MistralConfig, MistralForCausalLM
+from transformers.models.mixtral import MixtralConfig, MixtralForCausalLM
 
 import litgpt.config as config_module
+from litgpt import GPT, Config
+from litgpt.scripts.convert_hf_checkpoint import (
+    copy_weights_falcon,
+    copy_weights_gpt_neox,
+    copy_weights_hf_llama,
+    copy_weights_phi,
+)
 
 
 @torch.inference_mode()
 @pytest.mark.parametrize("rotary_pct", (0.25, 1))
 @pytest.mark.parametrize("batch_size", (1, 3))
 @pytest.mark.parametrize("n_embd", (16, 32))
 @pytest.mark.parametrize("parallel_residual", (False, True))
@@ -38,19 +57,14 @@
                 pytest.mark.xfail(raises=AssertionError, strict=False),
                 RunIf(min_cuda_gpus=1),
             ],
         ),
     ],
 )
 def test_against_gpt_neox_model(rotary_pct, batch_size, n_embd, parallel_residual, device, dtype) -> None:
-    from transformers import GPTNeoXConfig, GPTNeoXForCausalLM
-
-    from litgpt import GPT, Config
-    from litgpt.scripts.convert_hf_checkpoint import copy_weights_gpt_neox
-
     torch.set_default_dtype(dtype)
 
     ours_config = Config(
         block_size=64,
         vocab_size=100,
         n_layer=4,
         n_head=8,
@@ -111,19 +125,14 @@
                 pytest.mark.xfail(raises=AssertionError, strict=False),
                 RunIf(min_cuda_gpus=1),
             ],
         ),
     ],
 )
 def test_against_hf_falcon(kwargs, device, dtype):
-    from transformers.models.falcon import FalconConfig, FalconForCausalLM
-
-    from litgpt import GPT, Config
-    from litgpt.scripts.convert_hf_checkpoint import copy_weights_falcon
-
     torch.set_default_dtype(dtype)
 
     ours_config = Config.from_name(**kwargs)
     theirs_config = FalconConfig(
         hidden_size=ours_config.n_embd,
         num_attention_heads=ours_config.n_head,
         num_kv_heads=ours_config.n_query_groups,
@@ -162,20 +171,14 @@
                 pytest.mark.xfail(raises=AssertionError, strict=False),
                 RunIf(min_cuda_gpus=1),
             ],
         ),
     ],
 )
 def test_against_original_open_llama_3b(device, dtype):
-    from transformers.models.llama.configuration_llama import LlamaConfig
-    from transformers.models.llama.modeling_llama import LlamaForCausalLM
-
-    from litgpt import GPT, Config
-    from litgpt.scripts.convert_hf_checkpoint import copy_weights_hf_llama
-
     torch.set_default_dtype(dtype)
 
     ours_config = Config.from_name("open_llama_3b", n_layer=2, n_head=8, n_embd=32, intermediate_size=86)
     T = 5
     theirs_config = LlamaConfig(
         hidden_size=ours_config.n_embd,
         num_attention_heads=ours_config.n_head,
@@ -199,15 +202,21 @@
     theirs_y = theirs_model(x)["logits"].to(dtype)  # HF converts logits to float
     torch.testing.assert_close(ours_y, theirs_y)
 
 
 @torch.inference_mode()
 @pytest.mark.parametrize(
     "ours_kwargs",
-    [{"name": "Llama-2-7b-hf"}, {"name": "CodeLlama-7b-hf"}, {"name": "Llama-2-70b-chat-hf", "n_query_groups": 1}],
+    [
+        {"name": "Llama-2-7b-hf"},
+        {"name": "CodeLlama-7b-hf"},
+        {"name": "Llama-2-70b-chat-hf", "n_query_groups": 1},
+        {"name": "Llama-3-8B"},
+        {"name": "Llama-3-8B-Instruct"},
+    ],
 )
 @pytest.mark.parametrize(
     ("device", "dtype"),
     [
         (torch.device("cpu"), torch.float32),
         pytest.param(
             torch.device("cuda"),
@@ -217,21 +226,15 @@
                 # is slightly different
                 pytest.mark.xfail(raises=AssertionError, strict=False),
                 RunIf(min_cuda_gpus=1),
             ],
         ),
     ],
 )
-def test_against_hf_llama2(ours_kwargs, device, dtype):
-    from transformers.models.llama.configuration_llama import LlamaConfig
-    from transformers.models.llama.modeling_llama import LlamaForCausalLM
-
-    from litgpt import GPT, Config
-    from litgpt.scripts.convert_hf_checkpoint import copy_weights_hf_llama
-
+def test_against_hf_llama_2_and_3(ours_kwargs, device, dtype):
     torch.set_default_dtype(dtype)
 
     ours_config = Config.from_name(
         padded_vocab_size=10000, n_layer=2, n_head=8, n_embd=32, intermediate_size=86, **ours_kwargs
     )
     T = 5
     theirs_config = LlamaConfig(
@@ -260,109 +263,34 @@
     assert x.size(1) == T
     ours_y = ours_model(x)
     theirs_y = theirs_model(x)["logits"].to(dtype)  # HF converts logits to float
     torch.testing.assert_close(ours_y, theirs_y)
 
 
 @torch.inference_mode()
+@pytest.mark.parametrize("model_name", ("phi-1_5", "phi-2"))
 @pytest.mark.parametrize(
     ("device", "dtype"),
     [
         (torch.device("cpu"), torch.float32),
         pytest.param(
             torch.device("cuda"),
             torch.float16,
             marks=[pytest.mark.xfail(raises=AssertionError, strict=False), RunIf(min_cuda_gpus=1)],
         ),
     ],
 )
-def test_against_hf_phi_1_5(device, dtype):
-    workdir = wd / "tests" / "reference_models"
-    workdir.mkdir(parents=True, exist_ok=True)
-    file_paths = [workdir / "original_phi_1_5.py", workdir / "configuration_phi.py"]
-    urls = [
-        "https://huggingface.co/microsoft/phi-1_5/raw/main/modeling_phi.py",
-        "https://huggingface.co/microsoft/phi-1_5/raw/main/configuration_phi.py",
-    ]
-    for file_path, url in zip(file_paths, urls):
-        if not file_path.is_file():
-            urlretrieve(url=url, filename=file_path)
-
-    from reference_models.configuration_phi import PhiConfig
-    from reference_models.original_phi_1_5 import PhiForCausalLM
-
-    from litgpt import GPT, Config
-    from litgpt.scripts.convert_hf_checkpoint import copy_weights_phi
-
-    torch.set_default_dtype(dtype)
-
-    ours_config = Config.from_name(
-        "phi-1_5", padded_vocab_size=10000, n_layer=2, n_head=4, n_embd=256, rotary_percentage=0.5
-    )
-    T = 5
-    theirs_config = PhiConfig(
-        vocab_size=ours_config.padded_vocab_size,
-        max_position_embeddings=ours_config.block_size,
-        hidden_size=ours_config.n_embd,
-        intermediate_size=ours_config.intermediate_size,
-        num_attention_heads=ours_config.n_head,
-        num_hidden_layers=ours_config.n_layer,
-        partial_rotary_factor=ours_config.rotary_percentage,
-        torch_dtype=dtype,
-    )
-
-    theirs_model = PhiForCausalLM(theirs_config).to(device)
-    theirs_state_dict = theirs_model.state_dict()
-    state_dict = {}
-    copy_weights_phi(ours_config, {}, state_dict, theirs_state_dict)
-    ours_model = GPT(ours_config).to(device)
-    ours_model.load_state_dict(state_dict)
-
-    # test end to end
-    x = torch.tensor([[9856, 23, 491, 1536, 304]], dtype=torch.int32, device=device)
-    assert x.size(1) == T
-    ours_y = ours_model(x)
-    theirs_y = theirs_model(x)["logits"].to(dtype)  # HF converts logits to float
-    torch.testing.assert_close(ours_y, theirs_y)
-
-
-@torch.inference_mode()
-@pytest.mark.parametrize(
-    ("device", "dtype"),
-    [
-        (torch.device("cpu"), torch.float32),
-        pytest.param(
-            torch.device("cuda"),
-            torch.float16,
-            marks=[pytest.mark.xfail(raises=AssertionError, strict=False), RunIf(min_cuda_gpus=1)],
-        ),
-    ],
-)
-def test_against_hf_phi_2(device, dtype):
-    workdir = wd / "tests" / "reference_models"
-    workdir.mkdir(parents=True, exist_ok=True)
-    file_paths = [workdir / "original_phi_2.py", workdir / "configuration_phi.py"]
-    urls = [
-        "https://huggingface.co/microsoft/phi-2/raw/main/modeling_phi.py",
-        "https://huggingface.co/microsoft/phi-2/raw/main/configuration_phi.py",
-    ]
-    for file_path, url in zip(file_paths, urls):
-        if not file_path.is_file():
-            urlretrieve(url=url, filename=file_path)
-
-    from reference_models.configuration_phi import PhiConfig
-    from reference_models.original_phi_2 import PhiForCausalLM
-
-    from litgpt import GPT, Config
-    from litgpt.scripts.convert_hf_checkpoint import copy_weights_phi
+def test_against_hf_phi(model_name, device, dtype):
+    from transformers.models.phi.configuration_phi import PhiConfig
+    from transformers.models.phi.modeling_phi import PhiForCausalLM
 
     torch.set_default_dtype(dtype)
 
     ours_config = Config.from_name(
-        "phi-2", padded_vocab_size=10000, n_layer=2, n_head=4, n_embd=256, rotary_percentage=0.5
+        model_name, padded_vocab_size=10000, n_layer=2, n_head=4, n_embd=256, rotary_percentage=0.5
     )
     T = 5
     theirs_config = PhiConfig(
         vocab_size=ours_config.padded_vocab_size,
         max_position_embeddings=ours_config.block_size,
         hidden_size=ours_config.n_embd,
         intermediate_size=ours_config.intermediate_size,
@@ -401,20 +329,14 @@
                 pytest.mark.xfail(raises=AssertionError, strict=False),
                 RunIf(min_cuda_gpus=1),
             ],
         ),
     ],
 )
 def test_against_hf_mistral(device, dtype):
-    from transformers.models.mistral.configuration_mistral import MistralConfig
-    from transformers.models.mistral.modeling_mistral import MistralForCausalLM
-
-    from litgpt import GPT, Config
-    from litgpt.scripts.convert_hf_checkpoint import copy_weights_hf_llama
-
     torch.set_default_dtype(dtype)
 
     ours_config = Config.from_name(
         "Mistral-7B-Instruct-v0.1",
         padded_vocab_size=10000,
         n_layer=2,
         n_embd=32,
@@ -449,19 +371,14 @@
     ours_y = ours_model(x)
     theirs_y = theirs_model(x)["logits"].to(dtype)  # HF converts logits to float
     torch.testing.assert_close(ours_y, theirs_y)
 
 
 @torch.inference_mode()
 def test_against_hf_mixtral():
-    from transformers.models.mixtral import MixtralConfig, MixtralForCausalLM
-
-    from litgpt import GPT, Config
-    from litgpt.scripts.convert_hf_checkpoint import copy_weights_hf_llama
-
     device = torch.device("cpu")
     dtype = torch.float32
     ours_config = Config.from_name(
         "Mixtral-8x7B-Instruct-v0.1",
         padded_vocab_size=10000,
         n_layer=2,
         n_embd=32,
@@ -514,19 +431,14 @@
                 pytest.mark.xfail(raises=AssertionError, strict=False),
                 RunIf(min_cuda_gpus=1),
             ],
         ),
     ],
 )
 def test_against_original_stablelm_zephyr_3b(device, dtype):
-    from transformers import AutoConfig, AutoModelForCausalLM
-
-    from litgpt import GPT, Config
-    from litgpt.scripts.convert_hf_checkpoint import copy_weights_hf_llama
-
     torch.set_default_dtype(dtype)
 
     T = 5
     ours_config = Config.from_name("stablelm-zephyr-3b", n_layer=2, n_head=16, n_embd=32, intermediate_size=86)
     theirs_config = AutoConfig.from_pretrained(
         "stabilityai/stablelm-zephyr-3b",
         trust_remote_code=True,
@@ -570,20 +482,14 @@
                 pytest.mark.xfail(raises=AssertionError, strict=False),
                 RunIf(min_cuda_gpus=1),
             ],
         ),
     ],
 )
 def test_against_original_gemma(model_name, device, dtype):
-    from transformers.models.gemma.configuration_gemma import GemmaConfig
-    from transformers.models.gemma.modeling_gemma import GemmaForCausalLM
-
-    from litgpt import GPT, Config
-    from litgpt.scripts.convert_hf_checkpoint import copy_weights_hf_llama
-
     torch.set_default_dtype(dtype)
 
     T = 5
     ours_config = Config.from_name(model_name, n_layer=2, n_head=16, n_embd=32, intermediate_size=86)
     theirs_config = GemmaConfig(
         vocab_size=ours_config.padded_vocab_size,
         hidden_size=ours_config.n_embd,
@@ -617,21 +523,17 @@
     theirs_y = theirs_model(x)["logits"].to(dtype)  # HF converts logits to float
     torch.testing.assert_close(ours_y, theirs_y)
 
 
 @RunIf(dynamo=True)
 @torch.inference_mode()
 def test_model_compile():
-    from litgpt import GPT
-
     model = GPT.from_name("pythia-14m", n_layer=3)
     x = torch.randint(model.config.vocab_size, size=(2, model.config.block_size), dtype=torch.int64)
 
-    from torch._dynamo.backends import debugging
-
     explanation = torch._dynamo.explain(model)(x)
     assert isinstance(explanation, debugging.ExplainOutput)
     assert explanation.graph_count == 1
     assert explanation.graph_break_count == 0
 
     model = GPT(model.config)
     model.set_kv_cache(2)
@@ -644,16 +546,14 @@
 
 @torch.inference_mode()
 @pytest.mark.parametrize(
     "max_seq_length", (25, pytest.param(23, marks=pytest.mark.xfail(raises=IndexError, strict=True)))
 )
 @pytest.mark.flaky(reruns=5)
 def test_kv_cache(max_seq_length):
-    from litgpt import GPT, Config
-
     config = Config(block_size=25, padded_vocab_size=5, n_layer=2, n_head=2, n_embd=8)
     model = GPT(config)
     idx = torch.randint(0, model.config.padded_vocab_size, (1, 5))
     max_new_tokens = 20
     model.max_seq_length = max_seq_length
     model.set_kv_cache(1)
 
@@ -677,16 +577,14 @@
         x_no_cache = torch.cat((x_no_cache, out_no_cache), dim=1)
         x_cache = out_cache
         input_pos = input_pos[-1:] + 1
 
 
 @torch.inference_mode()
 def test_model_kv_cache_amp():
-    from litgpt.model import GPT, Config
-
     config = Config.from_name("pythia-14m", n_layer=2)
     model = GPT(config)
     encoded = torch.arange(45)
     model.set_kv_cache(batch_size=1)
     with torch.autocast("cpu", torch.bfloat16):
         output = model(encoded.unsqueeze(0), encoded)
     assert output.dtype is torch.bfloat16
@@ -698,26 +596,14 @@
 )
 
 
 @RunIf(min_cuda_gpus=1)
 @pytest.mark.parametrize("config", deepcopy(config_module.configs), ids=[c["name"] for c in config_module.configs])
 @torch.inference_mode()
 def test_sdpa_choice(config):
-    from torch.backends.cuda import (
-        SDPAParams,
-        SDPBackend,
-        can_use_efficient_attention,
-        can_use_flash_attention,
-        flash_sdp_enabled,
-        math_sdp_enabled,
-        mem_efficient_sdp_enabled,
-    )
-
-    from litgpt import GPT
-
     torch.set_default_dtype(torch.float16)
 
     def assert_sdpa_backend(original_fn, q, k, v, mask):
         params = SDPAParams(q, k, v, mask, 0.0, True)
         if expected is SDPBackend.FLASH_ATTENTION:
             assert flash_sdp_enabled()
             assert can_use_flash_attention(params, True)
@@ -754,26 +640,14 @@
         model(x)
 
 
 @RunIf(min_cuda_gpus=1)
 @pytest.mark.parametrize("config", deepcopy(config_module.configs), ids=[c["name"] for c in config_module.configs])
 @torch.inference_mode()
 def test_sdpa_choice_kv_cache(config):
-    from torch.backends.cuda import (
-        SDPAParams,
-        SDPBackend,
-        can_use_efficient_attention,
-        can_use_flash_attention,
-        flash_sdp_enabled,
-        math_sdp_enabled,
-        mem_efficient_sdp_enabled,
-    )
-
-    from litgpt import GPT
-
     torch.set_default_dtype(torch.float16)
 
     def assert_sdpa_backend(original_fn, q, k, v, mask):
         params = SDPAParams(q, k, v, mask, 0.0, True)
         if expected is SDPBackend.FLASH_ATTENTION:
             assert flash_sdp_enabled()
             assert can_use_flash_attention(params, True)
@@ -814,17 +688,15 @@
     )
     with torch.backends.cuda.sdp_kernel(enable_flash=False):
         model(x, input_pos)
 
 
 @RunIf(min_cuda_gpus=2, standalone=True)
 def test_rope_init_under_fsdp():
-    """Check that the rope cache is properly intialized"""
-    from litgpt import GPT
-
+    """Check that the rope cache is properly initialized"""
     fabric = Fabric(devices=2, strategy="fsdp", accelerator="cuda")
     fabric.launch()
 
     with fabric.init_module(empty_init=True):
         model = GPT.from_name("pythia-14m", n_layer=1)
     assert model.cos.device.type == "meta"
     assert model.sin.device.type == "meta"
@@ -835,14 +707,12 @@
     cos, sin = model.rope_cache(device=fabric.device)
     torch.testing.assert_close(model.cos, cos)
     torch.testing.assert_close(model.sin, sin)
 
 
 @RunIf(min_cuda_gpus=1)
 def test_reset_parameters_device():
-    from litgpt import GPT
-
     with torch.device("meta"):
         model = GPT.from_name("pythia-14m", n_layer=1)
     _materialize_meta_tensors(model, torch.device("cuda"))
     model.reset_parameters()
     assert model.cos.device.type == "cuda"
```

### Comparing `litgpt-0.2.0.dev0/tests/test_pretrain.py` & `litgpt-0.3.0/tests/test_pretrain.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,32 @@
 from pathlib import Path
 from unittest import mock
 from unittest.mock import ANY, Mock
 
 import pytest
 import torch
 from conftest import RunIf
+from lightning.fabric.strategies import FSDPStrategy, SingleDeviceStrategy
 from torch.utils.data import DataLoader
 
+from test_utils import test_init_out_dir
+from litgpt import pretrain
+from litgpt.args import EvalArgs, TrainArgs
+from litgpt.config import Config
+from litgpt.pretrain import initialize_weights
+
 
 @RunIf(min_cuda_gpus=2, standalone=True)
 # Set CUDA_VISIBLE_DEVICES for FSDP hybrid-shard, if fewer GPUs are used than are available
 @mock.patch.dict(os.environ, {"CUDA_VISIBLE_DEVICES": "0,1"})
 # If we were to use `save_hyperparameters()`, we would have to patch `sys.argv` or otherwise
 # the CLI would capture pytest args, but unfortunately patching would mess with subprocess
 # launching, so we need to mock `save_hyperparameters()`
 @mock.patch("litgpt.pretrain.save_hyperparameters")
 def test_pretrain(_, tmp_path):
-    from litgpt import pretrain
-    from litgpt.args import EvalArgs, TrainArgs
-    from litgpt.config import Config
-
     model_config = Config(block_size=2, n_layer=2, n_embd=8, n_head=4, padded_vocab_size=8)
 
     dataset = torch.tensor([[0, 1, 2], [3, 4, 5], [0, 1, 2]])
     dataloader = DataLoader(dataset)
     pretrain.get_dataloaders = Mock(return_value=(dataloader, dataloader))
 
     out_dir = tmp_path / "out"
@@ -41,15 +44,15 @@
             train=TrainArgs(global_batch_size=2, max_tokens=16, save_interval=1, micro_batch_size=1, max_norm=1.0),
             eval=EvalArgs(interval=1, max_iters=1),
         )
 
     if torch.distributed.get_rank() == 0:
         # tmp_path is not the same across all ranks, run assert only on rank 0
         out_dir_contents = set(os.listdir(out_dir))
-        checkpoint_dirs = {"step-00000001", "step-00000002", "step-00000003", "step-00000004"}
+        checkpoint_dirs = {"step-00000001", "step-00000002", "step-00000003", "step-00000004", "final"}
         assert checkpoint_dirs.issubset(out_dir_contents)
         assert all((out_dir / p).is_dir() for p in checkpoint_dirs)
         for checkpoint_dir in checkpoint_dirs:
             # the `tokenizer_dir` is None by default, so only 'lit_model.pth' shows here
             assert set(os.listdir(out_dir / checkpoint_dir)) == {"lit_model.pth", "model_config.yaml"}
 
         assert (out_dir / "logs" / "tensorboard" / "version_0").is_dir()
@@ -63,42 +66,47 @@
     torch.distributed.barrier()
 
 
 @RunIf(min_cuda_gpus=2, standalone=True)
 # Set CUDA_VISIBLE_DEVICES for FSDP hybrid-shard, if fewer GPUs are used than are available
 @mock.patch.dict(os.environ, {"CUDA_VISIBLE_DEVICES": "0,1"})
 @mock.patch("litgpt.pretrain.L.Fabric.load_raw")
-def test_initial_checkpoint_dir(load_mock, tmp_path):
-    from litgpt import pretrain
-    from litgpt.config import Config
-
+# See comment in `test_pretrain` why we need to mock `save_hyperparameters()`
+@mock.patch("litgpt.pretrain.save_hyperparameters")
+def test_initial_checkpoint_dir(_, load_mock, tmp_path):
     model_config = Config(block_size=2, n_layer=2, n_embd=8, n_head=4, padded_vocab_size=8)
 
     dataset = torch.tensor([[0, 1, 2], [3, 4, 5], [0, 1, 2]])
     dataloader = DataLoader(dataset)
     pretrain.get_dataloaders = Mock(return_value=(dataloader, dataloader))
     pretrain.fit = Mock()
 
     pretrain.setup(initial_checkpoint_dir=tmp_path, devices=2, model_config=model_config, out_dir=tmp_path)
 
     load_mock.assert_called_once_with(tmp_path / "lit_model.pth", ANY)
 
 
 def test_pretrain_model_name_and_config():
-    from litgpt import pretrain
-    from litgpt.config import Config
-
     with pytest.raises(ValueError, match="Only one of `model_name` or `model_config`"):
         pretrain.setup(model_name="tiny-llama-1.1b", model_config=Config(name="tiny-llama-1.1b"))
 
 
-def test_init_out_dir(tmp_path):
-    from litgpt.pretrain import init_out_dir
-
-    relative_path = Path("./out")
-    absolute_path = tmp_path / "out"
-    assert init_out_dir(relative_path) == relative_path
-    assert init_out_dir(absolute_path) == absolute_path
-
-    with mock.patch.dict(os.environ, {"LIGHTNING_ARTIFACTS_DIR": "prefix"}):
-        assert init_out_dir(relative_path) == Path("prefix") / relative_path
-        assert init_out_dir(absolute_path) == absolute_path
+@pytest.mark.parametrize(("strategy", "expected"), [(SingleDeviceStrategy, True), (FSDPStrategy, False)])
+def test_initialize_weights(strategy, expected):
+    fabric_mock = Mock()
+    fabric_mock.strategy = Mock(spec=strategy)
+
+    class Child(torch.nn.Module):
+        pass
+
+    class Parent(torch.nn.Module):
+        def __init__(self):
+            super().__init__()
+            self.child = Child()
+
+    model = Parent()
+    model.reset_parameters = Mock()
+    model.child.reset_parameters = Mock()
+
+    initialize_weights(fabric_mock, model, n_layer=2, n_embd=8)
+    assert model.reset_parameters.call_count == int(expected)
+    assert model.child.reset_parameters.call_count == int(expected)
```

### Comparing `litgpt-0.2.0.dev0/tests/test_prompts.py` & `litgpt-0.3.0/tests/test_prompts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
 
 import yaml
 
-from litgpt.prompts import PromptStyle
+import litgpt.config
+from litgpt import Config
+from litgpt.prompts import (
+    Alpaca,
+    Default,
+    PromptStyle,
+    has_prompt_style,
+    load_prompt_style,
+    prompt_styles,
+    save_prompt_style,
+)
 
 
 def test_default_prompt_style(mock_tokenizer):
-    from litgpt.prompts import Default
-
     prompt_style = Default()
     prompt = "This is a test prompt."
     assert prompt_style.apply(prompt) == prompt
     assert prompt_style.stop_tokens(mock_tokenizer) == ([mock_tokenizer.eos_id],)
 
 
 def test_prompt_style_from_name():
-    from litgpt.prompts import PromptStyle, prompt_styles
-
     for style_name in prompt_styles:
         assert isinstance(PromptStyle.from_name(style_name), prompt_styles[style_name])
 
 
 def test_prompt_style_from_config():
-    import litgpt.config
-    from litgpt import Config
-    from litgpt.prompts import Default, PromptStyle
-
     model_names = [
         "stablelm-tuned-alpha-3b",
         "stablelm-tuned-alpha-7b",
         "stablelm-zephyr-3b",
         "stablecode-instruct-alpha-3b",
         "falcon-7b-instruct",
         "falcon-40b-instruct",
@@ -44,14 +46,16 @@
         "longchat-13b-16k",
         "Nous-Hermes-llama-2-7b",
         "Nous-Hermes-13b",
         "Nous-Hermes-Llama2-13b",
         "Llama-2-7b-chat-hf",
         "Llama-2-13b-chat-hf",
         "Llama-2-70b-chat-hf",
+        "Llama-3-8B-Instruct",
+        "Llama-3-70B-Instruct",
         "Gemma-2b-it",
         "Gemma-7b-it",
         "FreeWilly2",
         "CodeLlama-7b-Instruct-hf",
         "CodeLlama-13b-Instruct-hf",
         "CodeLlama-34b-Instruct-hf",
         "CodeLlama-70b-Instruct-hf",
@@ -70,16 +74,14 @@
 
     for model_name in model_names:
         # by asserting the returned style is not the Default, we show that at least one of the regex patterns matched
         assert not isinstance(PromptStyle.from_config(Config.from_name(model_name)), Default)
 
 
 def test_apply_prompts():
-    from litgpt.prompts import Alpaca, prompt_styles
-
     prompt = "Is a coconut a nut or a fruit?"
     inp = "Optional input"
 
     for style in prompt_styles.values():
         output = style().apply(prompt, input=inp)
         assert prompt in output
         if isinstance(style, Alpaca):
@@ -88,30 +90,28 @@
 
 class CustomPromptStyle(PromptStyle):
     def apply(self, prompt, **kwargs):
         return prompt
 
 
 def test_save_load_prompt_style(tmp_path):
-    from litgpt.prompts import Alpaca, has_prompt_style, load_prompt_style, save_prompt_style
-
     # Save and load a built-in style
     checkpoint_dir = tmp_path / "checkpoint"
     checkpoint_dir.mkdir()
     assert not has_prompt_style(checkpoint_dir)
     save_prompt_style("alpaca", checkpoint_dir)
     assert has_prompt_style(checkpoint_dir)
-    with open(checkpoint_dir / "prompt_style.yaml", "r") as file:
+    with open(checkpoint_dir / "prompt_style.yaml", "r", encoding="utf-8") as file:
         contents = yaml.safe_load(file)
     assert contents == {"class_path": "litgpt.prompts.Alpaca"}
     loaded = load_prompt_style(checkpoint_dir)
     assert isinstance(loaded, Alpaca)
 
     # Save a custom style
     checkpoint_dir = tmp_path / "custom"
     checkpoint_dir.mkdir()
     save_prompt_style(CustomPromptStyle(), checkpoint_dir)
-    with open(checkpoint_dir / "prompt_style.yaml", "r") as file:
+    with open(checkpoint_dir / "prompt_style.yaml", "r", encoding="utf-8") as file:
         contents = yaml.safe_load(file)
     assert contents == {"class_path": "test_prompts.CustomPromptStyle"}
     loaded = load_prompt_style(checkpoint_dir)
     assert isinstance(loaded, CustomPromptStyle)
```

### Comparing `litgpt-0.2.0.dev0/tests/test_rope.py` & `litgpt-0.3.0/tests/test_rope.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
 
 import torch
+from transformers.models.gpt_neox.modeling_gpt_neox import GPTNeoXRotaryEmbedding, apply_rotary_pos_emb
+
+from litgpt.model import apply_rope, build_rope_cache
 
 
 @torch.inference_mode()
 def test_rope():
-    from transformers.models.gpt_neox.modeling_gpt_neox import GPTNeoXRotaryEmbedding, apply_rotary_pos_emb
-
-    from litgpt.model import apply_rope, build_rope_cache
-
     bs, seq_len, n_head, n_embed = 1, 6, 2, 8
     head_size = n_embed // n_head
     x = torch.randint(0, 10000, size=(bs, n_head, seq_len, head_size)).float()
     position_ids = torch.arange(seq_len).unsqueeze(0)
 
     theirs = GPTNeoXRotaryEmbedding(head_size, seq_len)
     ours_cos_cached, ours_sin_cached = build_rope_cache(seq_len, head_size, device=x.device)
```

### Comparing `litgpt-0.2.0.dev0/tests/test_tokenizer.py` & `litgpt-0.3.0/tests/test_tokenizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
 
 import os
-import sys
 from pathlib import Path
 
 import pytest
 from transformers import AutoTokenizer
 from transformers.utils import cached_file
 
-# support running without installing as a package
-wd = Path(__file__).parent.parent.resolve()
-sys.path.append(str(wd))
-
 import litgpt.config as config_module
+from litgpt.tokenizer import Tokenizer
 
 
+@pytest.mark.flaky(reruns=5)
 @pytest.mark.parametrize("config", config_module.configs, ids=[c["hf_config"]["name"] for c in config_module.configs])
 def test_tokenizer_against_hf(config):
-    from litgpt.tokenizer import Tokenizer
-
     access_token = os.getenv("HF_TOKEN")
 
     config = config_module.Config(**config)
 
     repo_id = f"{config.hf_config['org']}/{config.hf_config['name']}"
     cache_dir = Path("/tmp/tokenizer_test_cache")
 
@@ -80,11 +75,9 @@
         assert [15043 if t == 10994 else t for t in actual.tolist()] == expected
     else:
         assert actual.tolist() == expected
     assert ours.decode(actual) == theirs.decode(expected, skip_special_tokens=True)
 
 
 def test_tokenizer_input_validation():
-    from litgpt.tokenizer import Tokenizer
-
     with pytest.raises(NotADirectoryError, match="The checkpoint directory does not exist"):
         Tokenizer("cocofruit")
```

### Comparing `litgpt-0.2.0.dev0/tests/test_utils.py` & `litgpt-0.3.0/tests/test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,59 @@
 # Copyright Lightning AI. Licensed under the Apache License 2.0, see LICENSE file.
+from dataclasses import asdict
 
 import os
 from contextlib import redirect_stderr
 from io import StringIO
 from pathlib import Path
 from unittest import mock
 
 import pytest
 import torch
 import torch.nn.functional as F
 import yaml
 from conftest import RunIf
 from lightning import Fabric
 from lightning.fabric.loggers import CSVLogger, TensorBoardLogger
+from lightning.fabric.plugins import BitsandbytesPrecision
 from lightning.pytorch.loggers import WandbLogger
 from lightning_utilities.core.imports import RequirementCache
 
+from litgpt import GPT
+from litgpt.args import TrainArgs
+from litgpt.utils import (
+    CLI,
+    CycleIterator,
+    capture_hparams,
+    check_valid_checkpoint_dir,
+    choose_logger,
+    chunked_cross_entropy,
+    copy_config_files,
+    find_multiple,
+    incremental_save,
+    init_out_dir,
+    num_parameters,
+    parse_devices,
+    save_hyperparameters,
+)
 
-def test_find_multiple():
-    from litgpt.utils import find_multiple
 
+def test_find_multiple():
     assert find_multiple(17, 5) == 20
     assert find_multiple(30, 7) == 35
     assert find_multiple(10, 2) == 10
     assert find_multiple(5, 10) == 10
     assert find_multiple(50254, 128) == 50304
     assert find_multiple(50254, 256) == 50432
     assert find_multiple(50254, 512) == 50688
 
 
 # match fails on windows. why did they have to use backslashes?
 @RunIf(skip_windows=True)
 def test_check_valid_checkpoint_dir(tmp_path):
-    from litgpt.utils import check_valid_checkpoint_dir
-
     os.chdir(tmp_path)
 
     out = StringIO()
     with pytest.raises(SystemExit), redirect_stderr(out):
         check_valid_checkpoint_dir(tmp_path)
     out = out.getvalue().strip()
     expected = f"""
@@ -79,16 +95,14 @@
 See all download options by running:
  litgpt download
     """.strip()
     assert out == expected
 
 
 def test_incremental_write(tmp_path):
-    from litgpt.utils import incremental_save
-
     sd = {str(k): torch.randn(5, 10) for k in range(3)}
     sd["0"].someattr = 1
     sd_expected = {k: v.clone() for k, v in sd.items()}
     fn = str(tmp_path / "test.pt")
     with incremental_save(fn) as f:
         sd["0"] = f.store_early(sd["0"])
         sd["2"] = f.store_early(sd["2"])
@@ -100,16 +114,14 @@
         v_actual = sd_actual[k]
         torch.testing.assert_close(v_expected, v_actual)
 
 
 @pytest.mark.parametrize("B", (1, 2))
 @pytest.mark.parametrize("ignore_index", (None, -1, -2, -100))
 def test_chunked_cross_entropy(ignore_index, B):
-    from litgpt.utils import chunked_cross_entropy
-
     V = 50
     T = 25
     regular_logits = torch.randn(B, T, V)
     targets = torch.randint(0, V, (B, T))
 
     if ignore_index is not None:
         targets[:, [1, 4, 10, 19]] = ignore_index
@@ -138,16 +150,14 @@
 
     chunked_loss = chunked_cross_entropy(chunked_logits, targets, chunk_size=10, ignore_index=ignore_index)
     torch.testing.assert_close(chunked_loss, regular_loss)
     torch.testing.assert_close(chunked_loss, baseline_loss)
 
 
 def test_num_parameters():
-    from litgpt.utils import num_parameters
-
     model = torch.nn.Linear(2, 2)
     assert num_parameters(model) == 6
     assert num_parameters(model, requires_grad=True) == 6
     assert num_parameters(model, requires_grad=False) == 0
 
     model = torch.nn.Linear(2, 2)
     model.bias.requires_grad = False
@@ -155,34 +165,27 @@
     assert num_parameters(model, requires_grad=True) == 4
     assert num_parameters(model, requires_grad=False) == 2
 
 
 @RunIf(min_cuda_gpus=1)
 @pytest.mark.parametrize("mode", ["nf4", "nf4-dq", "fp4", "fp4-dq", "int8", "int8-training"])
 def test_num_parameters_bitsandbytes(mode):
-    from lightning.fabric.plugins import BitsandbytesPrecision
-
-    from litgpt import GPT
-    from litgpt.utils import num_parameters
-
     plugin = BitsandbytesPrecision(mode=mode)
     fabric = Fabric(plugins=plugin, accelerator="cuda", devices=1)
 
     model = torch.nn.Linear(10, 10)
     model = fabric.setup(model)
     assert num_parameters(model) == 110
 
     with fabric.init_module(empty_init=True):
         model = GPT.from_name("pythia-14m")
     assert num_parameters(model) == 14067712
 
 
 def test_cycle_iterator():
-    from litgpt.utils import CycleIterator
-
     iterator = CycleIterator([])
     with pytest.raises(StopIteration):
         next(iterator)
 
     iterator = CycleIterator(range(3))
     assert iterator.epoch == 0
     assert next(iterator) == 0
@@ -192,16 +195,14 @@
     assert next(iterator) == 2
     assert iterator.epoch == 0
     assert next(iterator) == 0
     assert iterator.epoch == 1
 
 
 def test_parse_devices():
-    from litgpt.utils import parse_devices
-
     with pytest.raises(ValueError, match="must be 'auto' or a positive integer"):
         assert parse_devices(0)
     with pytest.raises(ValueError, match="must be 'auto' or a positive integer"):
         assert parse_devices(-2)
 
     with mock.patch("litgpt.utils.torch.cuda.device_count", return_value=0):
         assert parse_devices("auto") == 1  # CPU
@@ -212,35 +213,49 @@
         assert parse_devices("auto") == 3
         assert parse_devices(-1) == 3
 
     assert parse_devices(5) == 5
 
 
 def test_copy_config_files(fake_checkpoint_dir, tmp_path):
-    from litgpt.utils import copy_config_files
-
     copy_config_files(fake_checkpoint_dir, tmp_path)
     expected = {"model_config.yaml", "tokenizer_config.json", "tokenizer.json"}
     contents = set(os.listdir(tmp_path))
     assert expected.issubset(contents)
 
 
-def _test_function(out_dir: Path, foo: bool = False, bar: int = 1):
-    from litgpt.utils import save_hyperparameters
+def test_capture_hparams():
+    integer = 1
+    string = "string"
+    boolean = True
+    none = None
+    path = Path("/path")
+    dataclass = TrainArgs()
+    other = torch.nn.Linear(1, 1)
+    hparams = capture_hparams()
+    assert hparams == {
+        "integer": integer,
+        "string": string,
+        "boolean": boolean,
+        "none": none,
+        "path": path,
+        "dataclass": asdict(dataclass),
+        "other": str(other),
+    }
 
+
+def _test_function(out_dir: Path, foo: bool = False, bar: int = 1):
     save_hyperparameters(_test_function, out_dir)
 
 
 def test_save_hyperparameters(tmp_path):
-    from litgpt.utils import CLI
-
     with mock.patch("sys.argv", ["any.py", "--out_dir", str(tmp_path), "--foo", "True"]):
         CLI(_test_function)
 
-    with open(tmp_path / "hyperparameters.yaml", "r") as file:
+    with open(tmp_path / "hyperparameters.yaml", "r", encoding="utf-8") as file:
         hparams = yaml.full_load(file)
 
     assert hparams["out_dir"] == str(tmp_path)
     assert hparams["foo"] is True
     assert hparams["bar"] == 1
 
 
@@ -256,31 +271,38 @@
         "litgpt finetune lora",
         "litgpt finetune adapter",
         "litgpt finetune adapter_v2",
         "litgpt pretrain",
     ],
 )
 def test_save_hyperparameters_known_commands(command, tmp_path):
-    from litgpt.utils import save_hyperparameters
-
     with mock.patch("sys.argv", [*command.split(" "), "--out_dir", str(tmp_path), "--foo", "True"]):
         save_hyperparameters(_test_function2, tmp_path)
 
-    with open(tmp_path / "hyperparameters.yaml", "r") as file:
+    with open(tmp_path / "hyperparameters.yaml", "r", encoding="utf-8") as file:
         hparams = yaml.full_load(file)
 
     assert hparams["out_dir"] == str(tmp_path)
     assert hparams["foo"] is True
     assert hparams["bar"] == 1
 
 
 def test_choose_logger(tmp_path):
-    from litgpt.utils import choose_logger
-
     assert isinstance(choose_logger("csv", out_dir=tmp_path, name="csv"), CSVLogger)
     if RequirementCache("tensorboard"):
         assert isinstance(choose_logger("tensorboard", out_dir=tmp_path, name="tb"), TensorBoardLogger)
     if RequirementCache("wandb"):
         assert isinstance(choose_logger("wandb", out_dir=tmp_path, name="wandb"), WandbLogger)
 
     with pytest.raises(ValueError, match="`--logger_name=foo` is not a valid option."):
         choose_logger("foo", out_dir=tmp_path, name="foo")
+
+
+def test_init_out_dir(tmp_path):
+    relative_path = Path("./out")
+    absolute_path = tmp_path / "out"
+    assert init_out_dir(relative_path) == relative_path
+    assert init_out_dir(absolute_path) == absolute_path
+
+    with mock.patch.dict(os.environ, {"LIGHTNING_ARTIFACTS_DIR": "prefix"}):
+        assert init_out_dir(relative_path) == Path("prefix") / relative_path
+        assert init_out_dir(absolute_path) == absolute_path
```

