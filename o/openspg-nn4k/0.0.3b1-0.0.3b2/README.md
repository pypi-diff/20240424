# Comparing `tmp/openspg-nn4k-0.0.3b1.tar.gz` & `tmp/openspg-nn4k-0.0.3b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openspg-nn4k-0.0.3b1.tar", last modified: Mon Apr  1 09:06:52 2024, max compression
+gzip compressed data, was "openspg-nn4k-0.0.3b2.tar", last modified: Wed Apr 24 03:11:49 2024, max compression
```

## Comparing `openspg-nn4k-0.0.3b1.tar` & `openspg-nn4k-0.0.3b2.tar`

### file list

```diff
@@ -1,86 +1,58 @@
-drwxr-xr-x   0 fuyu.bfy   (502) staff       (20)        0 2024-04-01 09:06:52.756880 openspg-nn4k-0.0.3b1/
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)      453 2024-01-26 06:38:05.000000 openspg-nn4k-0.0.3b1/LICENSE
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)       59 2024-01-06 07:37:46.000000 openspg-nn4k-0.0.3b1/MANIFEST.in
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)      163 2024-04-01 09:06:52.756512 openspg-nn4k-0.0.3b1/PKG-INFO
-drwxr-xr-x   0 fuyu.bfy   (502) staff       (20)        0 2024-04-01 09:06:52.719288 openspg-nn4k-0.0.3b1/nn4k/
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)      534 2024-04-01 09:06:51.000000 openspg-nn4k-0.0.3b1/nn4k/__init__.py
-drwxr-xr-x   0 fuyu.bfy   (502) staff       (20)        0 2024-04-01 09:06:52.719647 openspg-nn4k-0.0.3b1/nn4k/__pycache__/
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)      227 2024-03-20 03:25:08.000000 openspg-nn4k-0.0.3b1/nn4k/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 fuyu.bfy   (502) staff       (20)        0 2024-04-01 09:06:52.720549 openspg-nn4k-0.0.3b1/nn4k/consts/
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     1568 2024-04-01 07:56:35.000000 openspg-nn4k-0.0.3b1/nn4k/consts/__init__.py
-drwxr-xr-x   0 fuyu.bfy   (502) staff       (20)        0 2024-04-01 09:06:52.721233 openspg-nn4k-0.0.3b1/nn4k/consts/__pycache__/
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     1255 2024-03-14 07:37:30.000000 openspg-nn4k-0.0.3b1/nn4k/consts/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 fuyu.bfy   (502) staff       (20)        0 2024-04-01 09:06:52.723564 openspg-nn4k-0.0.3b1/nn4k/executor/
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)      559 2024-03-08 03:01:31.000000 openspg-nn4k-0.0.3b1/nn4k/executor/__init__.py
-drwxr-xr-x   0 fuyu.bfy   (502) staff       (20)        0 2024-04-01 09:06:52.725001 openspg-nn4k-0.0.3b1/nn4k/executor/__pycache__/
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)      297 2024-03-11 06:05:45.000000 openspg-nn4k-0.0.3b1/nn4k/executor/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)    10824 2024-03-11 06:05:45.000000 openspg-nn4k-0.0.3b1/nn4k/executor/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)    12021 2024-03-08 07:25:13.000000 openspg-nn4k-0.0.3b1/nn4k/executor/base.py
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)      554 2024-01-26 06:38:05.000000 openspg-nn4k-0.0.3b1/nn4k/executor/deepke.py
-drwxr-xr-x   0 fuyu.bfy   (502) staff       (20)        0 2024-04-01 09:06:52.727677 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)      618 2024-03-08 03:01:31.000000 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/__init__.py
-drwxr-xr-x   0 fuyu.bfy   (502) staff       (20)        0 2024-04-01 09:06:52.729591 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/__pycache__/
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)      361 2024-03-14 07:37:33.000000 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     2722 2024-03-14 07:37:35.000000 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/__pycache__/hf_decode_only_executor.cpython-39.pyc
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     4876 2024-03-14 07:37:35.000000 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/__pycache__/nn_hf_trainer.cpython-39.pyc
-drwxr-xr-x   0 fuyu.bfy   (502) staff       (20)        0 2024-04-01 09:06:52.731643 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/base/
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)      470 2024-03-08 03:01:31.000000 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/base/__init__.py
-drwxr-xr-x   0 fuyu.bfy   (502) staff       (20)        0 2024-04-01 09:06:52.733243 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/base/__pycache__/
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)      188 2024-03-14 07:37:33.000000 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/base/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     4706 2024-03-14 07:37:35.000000 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/base/__pycache__/hf_args.cpython-39.pyc
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     9452 2024-03-14 07:37:33.000000 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/base/__pycache__/hf_llm_executor.cpython-39.pyc
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     5437 2024-03-08 07:25:13.000000 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/base/hf_args.py
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)    13178 2024-03-08 07:25:13.000000 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/base/hf_llm_executor.py
-drwxr-xr-x   0 fuyu.bfy   (502) staff       (20)        0 2024-04-01 09:06:52.733721 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/default_config/
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)      470 2024-03-08 03:01:31.000000 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/default_config/__init__.py
-drwxr-xr-x   0 fuyu.bfy   (502) staff       (20)        0 2024-04-01 09:06:52.736400 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/default_config/decodeonly/
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)      470 2024-03-08 03:01:31.000000 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/default_config/decodeonly/__init__.py
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     1030 2024-03-08 03:01:31.000000 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/default_config/decodeonly/env_init.sh
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)      534 2024-03-08 07:25:13.000000 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/default_config/decodeonly/local_infer.json5
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     1997 2024-03-08 03:01:31.000000 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/default_config/decodeonly/local_sft.json5
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     1207 2024-03-08 07:25:13.000000 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/default_config/decodeonly/task_entry.py
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     4484 2024-03-08 03:01:31.000000 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/hf_decode_only_executor.py
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     2254 2024-03-08 07:25:13.000000 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/hf_embedding_executor.py
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     8813 2024-03-08 03:01:31.000000 openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/nn_hf_trainer.py
-drwxr-xr-x   0 fuyu.bfy   (502) staff       (20)        0 2024-04-01 09:06:52.738755 openspg-nn4k-0.0.3b1/nn4k/invoker/
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)      523 2024-01-26 06:38:05.000000 openspg-nn4k-0.0.3b1/nn4k/invoker/__init__.py
-drwxr-xr-x   0 fuyu.bfy   (502) staff       (20)        0 2024-04-01 09:06:52.742005 openspg-nn4k-0.0.3b1/nn4k/invoker/__pycache__/
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)      242 2024-01-26 07:37:33.000000 openspg-nn4k-0.0.3b1/nn4k/invoker/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     7381 2024-03-11 06:05:45.000000 openspg-nn4k-0.0.3b1/nn4k/invoker/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     2511 2024-01-15 02:38:53.000000 openspg-nn4k-0.0.3b1/nn4k/invoker/__pycache__/openai.cpython-39.pyc
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     2479 2024-01-06 04:39:55.000000 openspg-nn4k-0.0.3b1/nn4k/invoker/__pycache__/openai_invoker.cpython-39.pyc
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     8433 2024-03-08 07:25:13.000000 openspg-nn4k-0.0.3b1/nn4k/invoker/base.py
-drwxr-xr-x   0 fuyu.bfy   (502) staff       (20)        0 2024-04-01 09:06:52.716639 openspg-nn4k-0.0.3b1/nn4k/invoker/default_config/
-drwxr-xr-x   0 fuyu.bfy   (502) staff       (20)        0 2024-04-01 09:06:52.743588 openspg-nn4k-0.0.3b1/nn4k/invoker/default_config/remote_infer/
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)      497 2024-04-01 07:56:35.000000 openspg-nn4k-0.0.3b1/nn4k/invoker/default_config/remote_infer/remote_infer.json5
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)      654 2024-04-01 07:56:35.000000 openspg-nn4k-0.0.3b1/nn4k/invoker/default_config/remote_infer/remote_infer.py
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     3284 2024-04-01 07:56:35.000000 openspg-nn4k-0.0.3b1/nn4k/invoker/hub_invoker.py
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     5233 2024-02-15 09:28:00.000000 openspg-nn4k-0.0.3b1/nn4k/invoker/openai.py
-drwxr-xr-x   0 fuyu.bfy   (502) staff       (20)        0 2024-04-01 09:06:52.744198 openspg-nn4k-0.0.3b1/nn4k/nnhub/
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     8097 2024-04-01 07:56:35.000000 openspg-nn4k-0.0.3b1/nn4k/nnhub/__init__.py
-drwxr-xr-x   0 fuyu.bfy   (502) staff       (20)        0 2024-04-01 09:06:52.744654 openspg-nn4k-0.0.3b1/nn4k/nnhub/__pycache__/
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     6836 2024-03-14 07:37:30.000000 openspg-nn4k-0.0.3b1/nn4k/nnhub/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 fuyu.bfy   (502) staff       (20)        0 2024-04-01 09:06:52.747439 openspg-nn4k-0.0.3b1/nn4k/utils/
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)      470 2024-01-26 06:38:05.000000 openspg-nn4k-0.0.3b1/nn4k/utils/__init__.py
-drwxr-xr-x   0 fuyu.bfy   (502) staff       (20)        0 2024-04-01 09:06:52.750492 openspg-nn4k-0.0.3b1/nn4k/utils/__pycache__/
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)      168 2024-03-11 06:05:45.000000 openspg-nn4k-0.0.3b1/nn4k/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     1859 2024-03-11 06:05:45.000000 openspg-nn4k-0.0.3b1/nn4k/utils/__pycache__/args_utils.cpython-39.pyc
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     1804 2024-03-11 06:05:45.000000 openspg-nn4k-0.0.3b1/nn4k/utils/__pycache__/class_importing.cpython-39.pyc
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     3823 2024-03-14 07:37:30.000000 openspg-nn4k-0.0.3b1/nn4k/utils/__pycache__/config_parsing.cpython-39.pyc
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     1513 2024-01-15 02:38:53.000000 openspg-nn4k-0.0.3b1/nn4k/utils/__pycache__/invoker_checking.cpython-39.pyc
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     2152 2024-03-08 07:25:13.000000 openspg-nn4k-0.0.3b1/nn4k/utils/args_utils.py
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     2154 2024-01-26 06:38:05.000000 openspg-nn4k-0.0.3b1/nn4k/utils/class_importing.py
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     4326 2024-03-08 07:25:13.000000 openspg-nn4k-0.0.3b1/nn4k/utils/config_parsing.py
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     2949 2024-04-01 07:56:35.000000 openspg-nn4k-0.0.3b1/nn4k/utils/invoker_checking.py
-drwxr-xr-x   0 fuyu.bfy   (502) staff       (20)        0 2024-04-01 09:06:52.752776 openspg-nn4k-0.0.3b1/nn4k/utils/io/
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)      470 2024-03-08 03:01:31.000000 openspg-nn4k-0.0.3b1/nn4k/utils/io/__init__.py
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     2481 2024-03-08 03:01:31.000000 openspg-nn4k-0.0.3b1/nn4k/utils/io/dataset_utils.py
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)      656 2024-03-08 03:01:31.000000 openspg-nn4k-0.0.3b1/nn4k/utils/io/file_utils.py
-drwxr-xr-x   0 fuyu.bfy   (502) staff       (20)        0 2024-04-01 09:06:52.755829 openspg-nn4k-0.0.3b1/openspg_nn4k.egg-info/
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)      163 2024-04-01 09:06:52.000000 openspg-nn4k-0.0.3b1/openspg_nn4k.egg-info/PKG-INFO
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     2584 2024-04-01 09:06:52.000000 openspg-nn4k-0.0.3b1/openspg_nn4k.egg-info/SOURCES.txt
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)        1 2024-04-01 09:06:52.000000 openspg-nn4k-0.0.3b1/openspg_nn4k.egg-info/dependency_links.txt
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)       25 2024-04-01 09:06:52.000000 openspg-nn4k-0.0.3b1/openspg_nn4k.egg-info/requires.txt
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)        5 2024-04-01 09:06:52.000000 openspg-nn4k-0.0.3b1/openspg_nn4k.egg-info/top_level.txt
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)       38 2024-04-01 09:06:52.757023 openspg-nn4k-0.0.3b1/setup.cfg
--rw-r--r--   0 fuyu.bfy   (502) staff       (20)     1980 2024-01-26 06:38:05.000000 openspg-nn4k-0.0.3b1/setup.py
+drwxr-xr-x   0 yangjin    (502) admin       (80)        0 2024-04-24 03:11:49.127376 openspg-nn4k-0.0.3b2/
+-rw-r--r--   0 yangjin    (502) admin       (80)      453 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/LICENSE
+-rw-r--r--   0 yangjin    (502) admin       (80)       59 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/MANIFEST.in
+-rw-r--r--   0 yangjin    (502) admin       (80)      206 2024-04-24 03:11:49.126489 openspg-nn4k-0.0.3b2/PKG-INFO
+drwxr-xr-x   0 yangjin    (502) admin       (80)        0 2024-04-24 03:11:49.109499 openspg-nn4k-0.0.3b2/nn4k/
+-rw-r--r--   0 yangjin    (502) admin       (80)      534 2024-04-24 03:11:48.000000 openspg-nn4k-0.0.3b2/nn4k/__init__.py
+drwxr-xr-x   0 yangjin    (502) admin       (80)        0 2024-04-24 03:11:49.109854 openspg-nn4k-0.0.3b2/nn4k/consts/
+-rw-r--r--   0 yangjin    (502) admin       (80)     1568 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/consts/__init__.py
+drwxr-xr-x   0 yangjin    (502) admin       (80)        0 2024-04-24 03:11:49.111797 openspg-nn4k-0.0.3b2/nn4k/executor/
+-rw-r--r--   0 yangjin    (502) admin       (80)      559 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/executor/__init__.py
+-rw-r--r--   0 yangjin    (502) admin       (80)    12041 2024-04-19 07:14:30.000000 openspg-nn4k-0.0.3b2/nn4k/executor/base.py
+-rw-r--r--   0 yangjin    (502) admin       (80)      554 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/executor/deepke.py
+drwxr-xr-x   0 yangjin    (502) admin       (80)        0 2024-04-24 03:11:49.113772 openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/
+-rw-r--r--   0 yangjin    (502) admin       (80)      618 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/__init__.py
+drwxr-xr-x   0 yangjin    (502) admin       (80)        0 2024-04-24 03:11:49.115315 openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/base/
+-rw-r--r--   0 yangjin    (502) admin       (80)      470 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/base/__init__.py
+-rw-r--r--   0 yangjin    (502) admin       (80)     5437 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/base/hf_args.py
+-rw-r--r--   0 yangjin    (502) admin       (80)    13466 2024-04-19 07:14:30.000000 openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/base/hf_llm_executor.py
+drwxr-xr-x   0 yangjin    (502) admin       (80)        0 2024-04-24 03:11:49.115767 openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/default_config/
+-rw-r--r--   0 yangjin    (502) admin       (80)      470 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/default_config/__init__.py
+drwxr-xr-x   0 yangjin    (502) admin       (80)        0 2024-04-24 03:11:49.117664 openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/default_config/decodeonly/
+-rw-r--r--   0 yangjin    (502) admin       (80)      470 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/default_config/decodeonly/__init__.py
+-rw-r--r--   0 yangjin    (502) admin       (80)     1030 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/default_config/decodeonly/env_init.sh
+-rw-r--r--   0 yangjin    (502) admin       (80)      534 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/default_config/decodeonly/local_infer.json5
+-rw-r--r--   0 yangjin    (502) admin       (80)     1997 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/default_config/decodeonly/local_sft.json5
+-rw-r--r--   0 yangjin    (502) admin       (80)     1207 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/default_config/decodeonly/task_entry.py
+-rw-r--r--   0 yangjin    (502) admin       (80)     4543 2024-04-19 07:14:30.000000 openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/hf_decode_only_executor.py
+-rw-r--r--   0 yangjin    (502) admin       (80)     2285 2024-04-19 07:14:30.000000 openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/hf_embedding_executor.py
+-rw-r--r--   0 yangjin    (502) admin       (80)     8813 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/nn_hf_trainer.py
+drwxr-xr-x   0 yangjin    (502) admin       (80)        0 2024-04-24 03:11:49.119748 openspg-nn4k-0.0.3b2/nn4k/invoker/
+-rw-r--r--   0 yangjin    (502) admin       (80)      523 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/invoker/__init__.py
+-rw-r--r--   0 yangjin    (502) admin       (80)     8433 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/invoker/base.py
+drwxr-xr-x   0 yangjin    (502) admin       (80)        0 2024-04-24 03:11:49.107199 openspg-nn4k-0.0.3b2/nn4k/invoker/default_config/
+drwxr-xr-x   0 yangjin    (502) admin       (80)        0 2024-04-24 03:11:49.120553 openspg-nn4k-0.0.3b2/nn4k/invoker/default_config/remote_infer/
+-rw-r--r--   0 yangjin    (502) admin       (80)      497 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/invoker/default_config/remote_infer/remote_infer.json5
+-rw-r--r--   0 yangjin    (502) admin       (80)      654 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/invoker/default_config/remote_infer/remote_infer.py
+-rw-r--r--   0 yangjin    (502) admin       (80)     3284 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/invoker/hub_invoker.py
+-rw-r--r--   0 yangjin    (502) admin       (80)     5233 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/invoker/openai.py
+drwxr-xr-x   0 yangjin    (502) admin       (80)        0 2024-04-24 03:11:49.120968 openspg-nn4k-0.0.3b2/nn4k/nnhub/
+-rw-r--r--   0 yangjin    (502) admin       (80)     8097 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/nnhub/__init__.py
+drwxr-xr-x   0 yangjin    (502) admin       (80)        0 2024-04-24 03:11:49.122781 openspg-nn4k-0.0.3b2/nn4k/utils/
+-rw-r--r--   0 yangjin    (502) admin       (80)      470 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/utils/__init__.py
+-rw-r--r--   0 yangjin    (502) admin       (80)     2152 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/utils/args_utils.py
+-rw-r--r--   0 yangjin    (502) admin       (80)     2154 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/utils/class_importing.py
+-rw-r--r--   0 yangjin    (502) admin       (80)     4326 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/utils/config_parsing.py
+-rw-r--r--   0 yangjin    (502) admin       (80)     2949 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/utils/invoker_checking.py
+drwxr-xr-x   0 yangjin    (502) admin       (80)        0 2024-04-24 03:11:49.123984 openspg-nn4k-0.0.3b2/nn4k/utils/io/
+-rw-r--r--   0 yangjin    (502) admin       (80)      470 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/utils/io/__init__.py
+-rw-r--r--   0 yangjin    (502) admin       (80)     2481 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/utils/io/dataset_utils.py
+-rw-r--r--   0 yangjin    (502) admin       (80)      656 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/nn4k/utils/io/file_utils.py
+drwxr-xr-x   0 yangjin    (502) admin       (80)        0 2024-04-24 03:11:49.125620 openspg-nn4k-0.0.3b2/openspg_nn4k.egg-info/
+-rw-r--r--   0 yangjin    (502) admin       (80)      206 2024-04-24 03:11:48.000000 openspg-nn4k-0.0.3b2/openspg_nn4k.egg-info/PKG-INFO
+-rw-r--r--   0 yangjin    (502) admin       (80)     1485 2024-04-24 03:11:48.000000 openspg-nn4k-0.0.3b2/openspg_nn4k.egg-info/SOURCES.txt
+-rw-r--r--   0 yangjin    (502) admin       (80)        1 2024-04-24 03:11:48.000000 openspg-nn4k-0.0.3b2/openspg_nn4k.egg-info/dependency_links.txt
+-rw-r--r--   0 yangjin    (502) admin       (80)       13 2024-04-24 03:11:48.000000 openspg-nn4k-0.0.3b2/openspg_nn4k.egg-info/requires.txt
+-rw-r--r--   0 yangjin    (502) admin       (80)        5 2024-04-24 03:11:48.000000 openspg-nn4k-0.0.3b2/openspg_nn4k.egg-info/top_level.txt
+-rw-r--r--   0 yangjin    (502) admin       (80)       38 2024-04-24 03:11:49.127616 openspg-nn4k-0.0.3b2/setup.cfg
+-rw-r--r--   0 yangjin    (502) admin       (80)     1980 2024-04-07 08:04:26.000000 openspg-nn4k-0.0.3b2/setup.py
```

### Comparing `openspg-nn4k-0.0.3b1/nn4k/__init__.py` & `openspg-nn4k-0.0.3b2/nn4k/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied.
 
 
 __package_name__ = "openspg-nn4k"
-__version__ = "0.0.3-beta1"
+__version__ = "0.0.3-beta2"
```

### Comparing `openspg-nn4k-0.0.3b1/nn4k/consts/__init__.py` & `openspg-nn4k-0.0.3b2/nn4k/consts/__init__.py`

 * *Files identical despite different names*

### Comparing `openspg-nn4k-0.0.3b1/nn4k/executor/__init__.py` & `openspg-nn4k-0.0.3b2/nn4k/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `openspg-nn4k-0.0.3b1/nn4k/executor/base.py` & `openspg-nn4k-0.0.3b2/nn4k/executor/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     def inference(self, inputs, **kwargs):
         """
         The entry point of inference. Usually for local invokers or model services.
         """
         raise NotImplementedError()
 
     @abstractmethod
-    def load_model(self, args=None, mode=None, **kwargs):
+    def load_model(self, args=None, mode=None, model_to_cuda=True, **kwargs):
         """
         Implement model loading logic in derived executor classes.
 
         Implementer should initialize `self._model` and `self._tokenizer`.
 
         This method will be called by several entry methods in executors and invokers.
         """
```

### Comparing `openspg-nn4k-0.0.3b1/nn4k/executor/deepke.py` & `openspg-nn4k-0.0.3b2/nn4k/executor/deepke.py`

 * *Files identical despite different names*

### Comparing `openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/__init__.py` & `openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/base/hf_args.py` & `openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/base/hf_args.py`

 * *Files identical despite different names*

### Comparing `openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/base/hf_llm_executor.py` & `openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/base/hf_llm_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,23 +40,26 @@
         """
         executor = cls(nn_config)
         return executor
 
     def execute_sft(self, args: dict = None, callbacks=None, **kwargs):
         args = args or self.init_args
 
-        self.load_model(args=args, mode="train")
-
         # parse args into HFSftArgs dataclass for more convenient features
         from transformers import HfArgumentParser
 
         parser = HfArgumentParser(HFSftArgs)
         hf_sft_args: HFSftArgs
         hf_sft_args, *_ = parser.parse_dict(args, allow_extra_keys=True)
 
+        model_to_cuda = (
+            False if hf_sft_args.deepspeed else True
+        )  # if using deepspeed, don't load model to cuda in nn4k
+        self.load_model(args=args, mode="train", model_to_cuda=model_to_cuda)
+
         # load checkpoint path if necessary.
         resume_from_checkpoint_path = self._get_last_checkpoint(hf_sft_args)
 
         # load and map dataset
         train_dataset, eval_dataset = self._init_dataset(hf_sft_args)
 
         # init trainer
@@ -173,15 +176,15 @@
             return train_dataset, eval_dataset
 
     def _load_dataset(self, data_path, split="train"):  # noqa
         from nn4k.utils.io.dataset_utils import DatasetUtils
 
         return DatasetUtils.auto_dataset(data_path, split)
 
-    def load_model(self, args: dict = None, mode=None, **kwargs):
+    def load_model(self, args: dict = None, mode=None, model_to_cuda=True, **kwargs):
         """
         load model and tokenizer. If the model with the same mode is already loaded, will not load again.
         """
 
         assert (
             mode is not None
         ), f"mode should be either 'train' or 'inference' for HFLLMExecutor, {mode} is illegal."
@@ -197,15 +200,18 @@
         parser = HfArgumentParser(HFModelArgs)
         hf_model_args: HFModelArgs
         hf_model_args, *_ = parser.parse_dict(args, allow_extra_keys=True)
 
         self.model_mode = mode
         self._tokenizer = self._hf_tokenizer_loader(hf_model_args)
         self._model = self._hf_model_loader(
-            args=hf_model_args, mode=mode, device=hf_model_args.nn_device
+            args=hf_model_args,
+            mode=mode,
+            device=hf_model_args.nn_device,
+            model_to_cuda=model_to_cuda,
         )
 
         if self.tokenizer.eos_token_id is None:
             self.tokenizer.eos_token_id = self.model.config.eos_token_id
         if self.tokenizer.pad_token_id is None:
             self.tokenizer.pad_token_id = self.tokenizer.eos_token_id
         if hf_model_args.padding_side is not None:
@@ -272,14 +278,15 @@
     @abstractmethod
     def _hf_model_loader(
         self,
         args: HFModelArgs,
         mode,
         resume_from_checkpoint=False,
         device=None,
+        model_to_cuda=True,
         **kwargs,
     ):
         """
         load model into given device for hugging face.
         """
         pass
```

### Comparing `openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/default_config/decodeonly/env_init.sh` & `openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/default_config/decodeonly/env_init.sh`

 * *Files identical despite different names*

### Comparing `openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/default_config/decodeonly/local_infer.json5` & `openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/default_config/decodeonly/local_infer.json5`

 * *Files identical despite different names*

### Comparing `openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/default_config/decodeonly/local_sft.json5` & `openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/default_config/decodeonly/local_sft.json5`

 * *Files identical despite different names*

### Comparing `openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/default_config/decodeonly/task_entry.py` & `openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/default_config/decodeonly/task_entry.py`

 * *Files identical despite different names*

### Comparing `openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/hf_decode_only_executor.py` & `openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/hf_decode_only_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
     def _hf_model_loader(
         self,
         args: HFModelArgs,
         mode,
         resume_from_checkpoint=False,
         device=None,
+        model_to_cuda=True,
         **kwargs,
     ):
         if device is None or "auto":
             device = "cuda" if torch.cuda.is_available() else "cpu"
 
         # load base model
         model_config = self._hf_model_config_loader(args, **kwargs)
@@ -100,15 +101,17 @@
                     "a training, or provide a adapter_config to train a adapter from scratch or resume a "
                     "adapter training from checkpoint."
                 )
             model.print_trainable_parameters()
 
         if mode == "inference":
             model.eval()
-        model.to(device)
+
+        if model_to_cuda:
+            model.to(device)
 
         return model
 
     def _data_collator(self, return_tensors="pt", **kwargs):
         return transformers.DataCollatorForSeq2Seq(
             self.tokenizer,
             pad_to_multiple_of=8,
```

### Comparing `openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/hf_embedding_executor.py` & `openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/hf_embedding_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def from_config(cls, nn_config: dict) -> "HFEmbeddingExecutor":
         """
         Create an HFEmbeddingExecutor instance from `nn_config`.
         """
         executor = cls(nn_config)
         return executor
 
-    def load_model(self, args=None, **kwargs):
+    def load_model(self, args=None, mode=None, model_to_cuda=True, **kwargs):
         import torch
         from sentence_transformers import SentenceTransformer
         from nn4k.consts import NN_NAME_KEY, NN_NAME_TEXT
         from nn4k.consts import NN_VERSION_KEY, NN_VERSION_TEXT
         from nn4k.consts import NN_DEVICE_KEY
         from nn4k.utils.config_parsing import get_string_field
```

### Comparing `openspg-nn4k-0.0.3b1/nn4k/executor/huggingface/nn_hf_trainer.py` & `openspg-nn4k-0.0.3b2/nn4k/executor/huggingface/nn_hf_trainer.py`

 * *Files identical despite different names*

### Comparing `openspg-nn4k-0.0.3b1/nn4k/invoker/__init__.py` & `openspg-nn4k-0.0.3b2/nn4k/invoker/__init__.py`

 * *Files identical despite different names*

### Comparing `openspg-nn4k-0.0.3b1/nn4k/invoker/base.py` & `openspg-nn4k-0.0.3b2/nn4k/invoker/base.py`

 * *Files identical despite different names*

### Comparing `openspg-nn4k-0.0.3b1/nn4k/invoker/default_config/remote_infer/remote_infer.py` & `openspg-nn4k-0.0.3b2/nn4k/invoker/default_config/remote_infer/remote_infer.py`

 * *Files identical despite different names*

### Comparing `openspg-nn4k-0.0.3b1/nn4k/invoker/hub_invoker.py` & `openspg-nn4k-0.0.3b2/nn4k/invoker/hub_invoker.py`

 * *Files identical despite different names*

### Comparing `openspg-nn4k-0.0.3b1/nn4k/invoker/openai.py` & `openspg-nn4k-0.0.3b2/nn4k/invoker/openai.py`

 * *Files identical despite different names*

### Comparing `openspg-nn4k-0.0.3b1/nn4k/nnhub/__init__.py` & `openspg-nn4k-0.0.3b2/nn4k/nnhub/__init__.py`

 * *Files identical despite different names*

### Comparing `openspg-nn4k-0.0.3b1/nn4k/utils/args_utils.py` & `openspg-nn4k-0.0.3b2/nn4k/utils/args_utils.py`

 * *Files identical despite different names*

### Comparing `openspg-nn4k-0.0.3b1/nn4k/utils/class_importing.py` & `openspg-nn4k-0.0.3b2/nn4k/utils/class_importing.py`

 * *Files identical despite different names*

### Comparing `openspg-nn4k-0.0.3b1/nn4k/utils/config_parsing.py` & `openspg-nn4k-0.0.3b2/nn4k/utils/config_parsing.py`

 * *Files identical despite different names*

### Comparing `openspg-nn4k-0.0.3b1/nn4k/utils/invoker_checking.py` & `openspg-nn4k-0.0.3b2/nn4k/utils/invoker_checking.py`

 * *Files identical despite different names*

### Comparing `openspg-nn4k-0.0.3b1/nn4k/utils/io/dataset_utils.py` & `openspg-nn4k-0.0.3b2/nn4k/utils/io/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `openspg-nn4k-0.0.3b1/nn4k/utils/io/file_utils.py` & `openspg-nn4k-0.0.3b2/nn4k/utils/io/file_utils.py`

 * *Files identical despite different names*

### Comparing `openspg-nn4k-0.0.3b1/setup.py` & `openspg-nn4k-0.0.3b2/setup.py`

 * *Files identical despite different names*

