# Comparing `tmp/stable-audio-tools-0.0.8.tar.gz` & `tmp/stable-audio-tools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-audio-tools-0.0.8.tar", last modified: Mon Nov 27 06:06:37 2023, max compression
+gzip compressed data, was "stable-audio-tools-0.0.9.tar", last modified: Fri Dec 29 23:30:05 2023, max compression
```

## Comparing `stable-audio-tools-0.0.8.tar` & `stable-audio-tools-0.0.9.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-11-27 06:06:37.000000 stable-audio-tools-0.0.8/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1069 2023-09-28 01:32:48.000000 stable-audio-tools-0.0.8/LICENSE
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1364 2023-11-27 06:06:37.000000 stable-audio-tools-0.0.8/PKG-INFO
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     5942 2023-11-27 05:24:30.000000 stable-audio-tools-0.0.8/README.md
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       80 2023-07-13 19:16:59.000000 stable-audio-tools-0.0.8/pyproject.toml
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       38 2023-11-27 06:06:37.000000 stable-audio-tools-0.0.8/setup.cfg
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1331 2023-11-27 06:05:45.000000 stable-audio-tools-0.0.8/setup.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-11-27 06:06:37.000000 stable-audio-tools-0.0.8/stable_audio_tools/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-10-11 19:19:45.000000 stable-audio-tools-0.0.8/stable_audio_tools/__init__.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-11-27 06:06:37.000000 stable-audio-tools-0.0.8/stable_audio_tools/data/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-10-11 19:19:45.000000 stable-audio-tools-0.0.8/stable_audio_tools/data/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    22523 2023-11-27 06:05:45.000000 stable-audio-tools-0.0.8/stable_audio_tools/data/dataset.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     3235 2023-11-27 06:05:45.000000 stable-audio-tools-0.0.8/stable_audio_tools/data/utils.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-11-27 06:06:37.000000 stable-audio-tools-0.0.8/stable_audio_tools/inference/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-10-11 19:19:45.000000 stable-audio-tools-0.0.8/stable_audio_tools/inference/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    10563 2023-11-27 06:05:45.000000 stable-audio-tools-0.0.8/stable_audio_tools/inference/generation.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     7388 2023-11-27 06:05:45.000000 stable-audio-tools-0.0.8/stable_audio_tools/inference/sampling.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      858 2023-11-27 05:29:05.000000 stable-audio-tools-0.0.8/stable_audio_tools/inference/utils.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-11-27 06:06:37.000000 stable-audio-tools-0.0.8/stable_audio_tools/interface/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-10-11 19:19:45.000000 stable-audio-tools-0.0.8/stable_audio_tools/interface/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    21581 2023-11-27 06:05:45.000000 stable-audio-tools-0.0.8/stable_audio_tools/interface/gradio.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-11-27 06:06:37.000000 stable-audio-tools-0.0.8/stable_audio_tools/models/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       45 2023-10-11 19:19:45.000000 stable-audio-tools-0.0.8/stable_audio_tools/models/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    52788 2023-11-27 06:05:45.000000 stable-audio-tools-0.0.8/stable_audio_tools/models/adp.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    23230 2023-11-27 06:05:45.000000 stable-audio-tools-0.0.8/stable_audio_tools/models/autoencoders.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     7367 2023-11-27 06:05:45.000000 stable-audio-tools-0.0.8/stable_audio_tools/models/blocks.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     7536 2023-11-27 06:05:45.000000 stable-audio-tools-0.0.8/stable_audio_tools/models/bottleneck.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    14761 2023-11-27 06:05:45.000000 stable-audio-tools-0.0.8/stable_audio_tools/models/conditioners.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    33339 2023-11-27 06:05:45.000000 stable-audio-tools-0.0.8/stable_audio_tools/models/diffusion.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    17583 2023-11-27 05:36:26.000000 stable-audio-tools-0.0.8/stable_audio_tools/models/discriminators.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     5524 2023-11-27 06:05:45.000000 stable-audio-tools-0.0.8/stable_audio_tools/models/factory.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     8144 2023-11-27 06:05:45.000000 stable-audio-tools-0.0.8/stable_audio_tools/models/local_attention.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     5498 2023-11-27 05:38:03.000000 stable-audio-tools-0.0.8/stable_audio_tools/models/musicgen.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    13238 2023-11-27 06:05:45.000000 stable-audio-tools-0.0.8/stable_audio_tools/models/pqmf.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     4284 2023-11-27 06:05:45.000000 stable-audio-tools-0.0.8/stable_audio_tools/models/pretransforms.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      290 2023-11-27 06:05:45.000000 stable-audio-tools-0.0.8/stable_audio_tools/models/utils.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     3240 2023-11-27 05:38:55.000000 stable-audio-tools-0.0.8/stable_audio_tools/models/wavelets.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-11-27 06:06:37.000000 stable-audio-tools-0.0.8/stable_audio_tools/training/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       91 2023-10-11 19:19:45.000000 stable-audio-tools-0.0.8/stable_audio_tools/training/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    17331 2023-11-27 06:05:46.000000 stable-audio-tools-0.0.8/stable_audio_tools/training/autoencoders.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    39687 2023-11-27 06:05:46.000000 stable-audio-tools-0.0.8/stable_audio_tools/training/diffusion.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     9102 2023-11-27 06:05:46.000000 stable-audio-tools-0.0.8/stable_audio_tools/training/factory.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     2929 2023-11-27 06:05:46.000000 stable-audio-tools-0.0.8/stable_audio_tools/training/losses.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     8615 2023-11-27 05:41:48.000000 stable-audio-tools-0.0.8/stable_audio_tools/training/musicgen.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     3931 2023-11-27 05:41:54.000000 stable-audio-tools-0.0.8/stable_audio_tools/training/utils.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-11-27 06:06:37.000000 stable-audio-tools-0.0.8/stable_audio_tools.egg-info/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1364 2023-11-27 06:06:37.000000 stable-audio-tools-0.0.8/stable_audio_tools.egg-info/PKG-INFO
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1491 2023-11-27 06:06:37.000000 stable-audio-tools-0.0.8/stable_audio_tools.egg-info/SOURCES.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        1 2023-11-27 06:06:37.000000 stable-audio-tools-0.0.8/stable_audio_tools.egg-info/dependency_links.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      614 2023-11-27 06:06:37.000000 stable-audio-tools-0.0.8/stable_audio_tools.egg-info/requires.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       19 2023-11-27 06:06:37.000000 stable-audio-tools-0.0.8/stable_audio_tools.egg-info/top_level.txt
+drwxr-xr-x   0 fauno    (1879805201) Domain Users (1879800513)        0 2023-12-29 23:30:05.922809 stable-audio-tools-0.0.9/
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)     1069 2023-12-03 23:43:56.000000 stable-audio-tools-0.0.9/LICENSE
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)     1361 2023-12-29 23:30:05.916809 stable-audio-tools-0.0.9/PKG-INFO
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)     5942 2023-12-03 23:43:56.000000 stable-audio-tools-0.0.9/README.md
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)       80 2023-12-03 23:43:56.000000 stable-audio-tools-0.0.9/pyproject.toml
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)       38 2023-12-29 23:30:05.921736 stable-audio-tools-0.0.9/setup.cfg
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)     1328 2023-12-29 23:19:45.000000 stable-audio-tools-0.0.9/setup.py
+drwxr-xr-x   0 fauno    (1879805201) Domain Users (1879800513)        0 2023-12-29 23:30:05.806517 stable-audio-tools-0.0.9/stable_audio_tools/
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)      135 2023-12-29 23:10:15.000000 stable-audio-tools-0.0.9/stable_audio_tools/__init__.py
+drwxr-xr-x   0 fauno    (1879805201) Domain Users (1879800513)        0 2023-12-29 23:30:05.824292 stable-audio-tools-0.0.9/stable_audio_tools/data/
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)        0 2023-12-03 23:43:56.000000 stable-audio-tools-0.0.9/stable_audio_tools/data/__init__.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)    22742 2023-12-29 23:19:45.000000 stable-audio-tools-0.0.9/stable_audio_tools/data/dataset.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)     3235 2023-12-03 23:43:56.000000 stable-audio-tools-0.0.9/stable_audio_tools/data/utils.py
+drwxr-xr-x   0 fauno    (1879805201) Domain Users (1879800513)        0 2023-12-29 23:30:05.842373 stable-audio-tools-0.0.9/stable_audio_tools/inference/
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)        0 2023-12-03 23:43:56.000000 stable-audio-tools-0.0.9/stable_audio_tools/inference/__init__.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)    10563 2023-12-03 23:43:56.000000 stable-audio-tools-0.0.9/stable_audio_tools/inference/generation.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)     2002 2023-12-29 23:19:45.000000 stable-audio-tools-0.0.9/stable_audio_tools/inference/priors.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)     7388 2023-12-03 23:43:56.000000 stable-audio-tools-0.0.9/stable_audio_tools/inference/sampling.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)      979 2023-12-29 23:19:45.000000 stable-audio-tools-0.0.9/stable_audio_tools/inference/utils.py
+drwxr-xr-x   0 fauno    (1879805201) Domain Users (1879800513)        0 2023-12-29 23:30:05.849417 stable-audio-tools-0.0.9/stable_audio_tools/interface/
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)        0 2023-12-03 23:43:56.000000 stable-audio-tools-0.0.9/stable_audio_tools/interface/__init__.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)    23925 2023-12-29 23:19:45.000000 stable-audio-tools-0.0.9/stable_audio_tools/interface/gradio.py
+drwxr-xr-x   0 fauno    (1879805201) Domain Users (1879800513)        0 2023-12-29 23:30:05.889845 stable-audio-tools-0.0.9/stable_audio_tools/models/
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)       76 2023-12-29 23:10:15.000000 stable-audio-tools-0.0.9/stable_audio_tools/models/__init__.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)    52788 2023-12-03 23:43:57.000000 stable-audio-tools-0.0.9/stable_audio_tools/models/adp.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)    23446 2023-12-29 23:19:45.000000 stable-audio-tools-0.0.9/stable_audio_tools/models/autoencoders.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)     7367 2023-12-03 23:43:57.000000 stable-audio-tools-0.0.9/stable_audio_tools/models/blocks.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)     7503 2023-12-29 23:19:45.000000 stable-audio-tools-0.0.9/stable_audio_tools/models/bottleneck.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)    21076 2023-12-29 23:19:45.000000 stable-audio-tools-0.0.9/stable_audio_tools/models/conditioners.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)    35700 2023-12-29 23:19:45.000000 stable-audio-tools-0.0.9/stable_audio_tools/models/diffusion.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)    17583 2023-12-03 23:43:57.000000 stable-audio-tools-0.0.9/stable_audio_tools/models/discriminators.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)     5718 2023-12-29 23:10:15.000000 stable-audio-tools-0.0.9/stable_audio_tools/models/factory.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)     8500 2023-12-29 23:19:45.000000 stable-audio-tools-0.0.9/stable_audio_tools/models/local_attention.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)     5498 2023-12-03 23:43:57.000000 stable-audio-tools-0.0.9/stable_audio_tools/models/musicgen.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)    13238 2023-12-03 23:43:57.000000 stable-audio-tools-0.0.9/stable_audio_tools/models/pqmf.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)      837 2023-12-29 23:10:15.000000 stable-audio-tools-0.0.9/stable_audio_tools/models/pretrained.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)     4493 2023-12-29 23:19:45.000000 stable-audio-tools-0.0.9/stable_audio_tools/models/pretransforms.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)      290 2023-12-03 23:43:57.000000 stable-audio-tools-0.0.9/stable_audio_tools/models/utils.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)     3240 2023-12-03 23:43:57.000000 stable-audio-tools-0.0.9/stable_audio_tools/models/wavelets.py
+drwxr-xr-x   0 fauno    (1879805201) Domain Users (1879800513)        0 2023-12-29 23:30:05.911994 stable-audio-tools-0.0.9/stable_audio_tools/training/
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)       91 2023-12-03 23:43:57.000000 stable-audio-tools-0.0.9/stable_audio_tools/training/__init__.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)    18453 2023-12-29 23:19:45.000000 stable-audio-tools-0.0.9/stable_audio_tools/training/autoencoders.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)    40441 2023-12-29 23:19:45.000000 stable-audio-tools-0.0.9/stable_audio_tools/training/diffusion.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)     9194 2023-12-29 23:19:45.000000 stable-audio-tools-0.0.9/stable_audio_tools/training/factory.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)     2929 2023-12-03 23:43:57.000000 stable-audio-tools-0.0.9/stable_audio_tools/training/losses.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)     8615 2023-12-03 23:43:57.000000 stable-audio-tools-0.0.9/stable_audio_tools/training/musicgen.py
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)     3931 2023-12-03 23:43:57.000000 stable-audio-tools-0.0.9/stable_audio_tools/training/utils.py
+drwxr-xr-x   0 fauno    (1879805201) Domain Users (1879800513)        0 2023-12-29 23:30:05.919507 stable-audio-tools-0.0.9/stable_audio_tools.egg-info/
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)     1361 2023-12-29 23:30:05.000000 stable-audio-tools-0.0.9/stable_audio_tools.egg-info/PKG-INFO
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)     1570 2023-12-29 23:30:05.000000 stable-audio-tools-0.0.9/stable_audio_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)        1 2023-12-29 23:30:05.000000 stable-audio-tools-0.0.9/stable_audio_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)      611 2023-12-29 23:30:05.000000 stable-audio-tools-0.0.9/stable_audio_tools.egg-info/requires.txt
+-rw-r--r--   0 fauno    (1879805201) Domain Users (1879800513)       19 2023-12-29 23:30:05.000000 stable-audio-tools-0.0.9/stable_audio_tools.egg-info/top_level.txt
```

### Comparing `stable-audio-tools-0.0.8/LICENSE` & `stable-audio-tools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-audio-tools-0.0.8/PKG-INFO` & `stable-audio-tools-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: stable-audio-tools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Training and inference tools for generative audio models from Stability AI
 Home-page: https://github.com/Stability-AI/stable-audio-tools.git
 Author: Stability AI
 License-File: LICENSE
 Requires-Dist: audiocraft==1.0.0
 Requires-Dist: aeiou==0.0.20
 Requires-Dist: alias-free-torch==0.0.6
 Requires-Dist: auraloss==0.4.0
 Requires-Dist: descript-audio-codec==1.0.0
 Requires-Dist: einops==0.7.0
 Requires-Dist: einops-exts==0.0.4
 Requires-Dist: ema-pytorch==0.2.3
 Requires-Dist: encodec==0.1.1
 Requires-Dist: gradio==3.42.0
+Requires-Dist: huggingface_hub
 Requires-Dist: importlib-resources==5.12.0
 Requires-Dist: k-diffusion==0.1.1
 Requires-Dist: laion-clap==1.1.4
 Requires-Dist: local-attention==1.8.6
-Requires-Dist: nwt-pytorch==0.0.4
 Requires-Dist: pandas==2.0.2
 Requires-Dist: pedalboard==0.7.4
 Requires-Dist: prefigure==0.0.9
 Requires-Dist: pytorch_lightning==2.1.0
 Requires-Dist: PyWavelets==1.4.1
 Requires-Dist: safetensors
 Requires-Dist: sentencepiece==0.1.99
```

### Comparing `stable-audio-tools-0.0.8/README.md` & `stable-audio-tools-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/data/dataset.py` & `stable-audio-tools-0.0.9/stable_audio_tools/data/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import importlib
 import numpy as np
+import io
 import os
 import posixpath
 import random
 import re
 import subprocess
 import time
 import torch
@@ -14,14 +15,16 @@
 from os import path
 from pedalboard.io import AudioFile
 from torchaudio import transforms as T
 from typing import Optional, Callable, List
 
 from .utils import Stereo, Mono, PhaseFlipper, PadCrop_Normalized_T
 
+AUDIO_KEYS = ("flac", "wav", "mp3", "m4a", "ogg", "opus")
+
 # fast_scandir implementation by Scott Hawley originally in https://github.com/zqevans/audio-diffusion/blob/main/dataset/dataset.py
 
 def fast_scandir(
     dir:str,  # top-level directory at which to begin scanning
     ext:list,  # list of allowed file extensions,
     #max_size = 1 * 1000 * 1000 * 1000 # Only files < 1 GB
     ):
@@ -87,15 +90,15 @@
         subfolders.extend(sf)
         files.extend(f)
     return subfolders, files
 
 def get_audio_filenames(
     paths: list,  # directories in which to search
     keywords=None,
-    exts=['.wav', '.mp3', '.flac', '.ogg', '.aif']
+    exts=['.wav', '.mp3', '.flac', '.ogg', '.aif', '.opus']
 ):
     "recursively get a list of audio filenames"
     filenames = []
     if type(paths) is str:
         paths = [paths]
     for path in paths:               # get a list of relevant filenames
         if keywords is not None:
@@ -370,14 +373,23 @@
             s3_url_prefix=None,
             recursive=True,
             profiles={self.s3_path: self.profile} if self.profile else {},
         )
 
         return self.urls
 
+def audio_decoder(key, value):
+    # Get file extension from key
+    ext = key.split(".")[-1]
+
+    if ext in AUDIO_KEYS:
+        return torchaudio.load(io.BytesIO(value))
+    else:
+        return None
+
 def collation_fn(samples):
         batched = list(zip(*samples))
         result = []
         for b in batched:
             if isinstance(b[0], (int, float)):
                 b = np.array(b)
             elif isinstance(b[0], torch.Tensor):
@@ -416,30 +428,28 @@
 
         # Flatten the list of lists of URLs
         urls = [url for dataset_urls in urls for url in dataset_urls]
 
         self.dataset = wds.DataPipeline(
             wds.ResampledShards(urls),
             wds.tarfile_to_samples(handler=log_and_continue),
-            wds.decode(wds.torch_audio, handler=log_and_continue),
+            wds.decode(audio_decoder, handler=log_and_continue),
             wds.map(self.wds_preprocess, handler=log_and_continue),
             wds.select(is_valid_sample),
             wds.to_tuple("audio", "json", handler=log_and_continue),
             wds.batched(batch_size, partial=False, collation_fn=collation_fn),
         ).with_epoch(epoch_steps//num_workers if num_workers > 0 else epoch_steps)
 
         self.data_loader = wds.WebLoader(self.dataset, num_workers=num_workers, **data_loader_kwargs)
 
     def wds_preprocess(self, sample):
 
-        audio_keys = ("flac", "wav", "mp3", "m4a", "ogg")
-
         found_key, rewrite_key = '', ''
         for k, v in sample.items():  # print the all entries in dict
-            for akey in audio_keys:
+            for akey in AUDIO_KEYS:
                 if k.endswith(akey):
                     # to rename long/weird key with its simpler counterpart
                     found_key, rewrite_key = k, akey
                     break
             if '' != found_key:
                 break
         if '' == found_key:  # got no audio!
```

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/data/utils.py` & `stable-audio-tools-0.0.9/stable_audio_tools/data/utils.py`

 * *Files identical despite different names*

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/inference/generation.py` & `stable-audio-tools-0.0.9/stable_audio_tools/inference/generation.py`

 * *Files identical despite different names*

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/inference/sampling.py` & `stable-audio-tools-0.0.9/stable_audio_tools/inference/sampling.py`

 * *Files identical despite different names*

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/inference/utils.py` & `stable-audio-tools-0.0.9/stable_audio_tools/inference/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 from ..data.utils import PadCrop
 
 from torchaudio import transforms as T
 
+def set_audio_channels(audio, target_channels):
+    if target_channels == 1:
+        # Convert to mono
+        audio = audio.mean(1, keepdim=True)
+    elif target_channels == 2:
+        # Convert to stereo
+        if audio.shape[1] == 1:
+            audio = audio.repeat(1, 2, 1)
+        elif audio.shape[1] > 2:
+            audio = audio[:, :2, :]
+    return audio
+
 def prepare_audio(audio, in_sr, target_sr, target_length, target_channels, device):
     
     audio = audio.to(device)
 
     if in_sr != target_sr:
         resample_tf = T.Resample(in_sr, target_sr).to(device)
         audio = resample_tf(audio)
@@ -14,18 +26,10 @@
 
     # Add batch dimension
     if audio.dim() == 1:
         audio = audio.unsqueeze(0).unsqueeze(0)
     elif audio.dim() == 2:
         audio = audio.unsqueeze(0)
 
-    if target_channels == 1:
-        # Convert to mono
-        audio = audio.mean(1, keepdim=True)
-    elif target_channels == 2:
-        # Convert to stereo
-        if audio.shape[1] == 1:
-            audio = audio.repeat(1, 2, 1)
-        elif audio.shape[1] > 2:
-            audio = audio[:, :2, :]
+    audio = set_audio_channels(audio, target_channels)
 
     return audio
```

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/interface/gradio.py` & `stable-audio-tools-0.0.9/stable_audio_tools/interface/gradio.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from einops import rearrange
 from safetensors.torch import load_file
 from torch.nn import functional as F
 from torchaudio import transforms as T
 
 
 from ..inference.generation import generate_diffusion_cond, generate_diffusion_uncond
+from ..inference.priors import generate_mono_to_stereo
 from ..models.factory import create_model_from_config
 from ..models.pretrained import get_pretrained_model
 from ..models.utils import load_ckpt_state_dict
 from ..inference.utils import prepare_audio
 from ..training.utils import copy_state_dict
 
 model = None
@@ -357,15 +358,15 @@
                 has_seconds_total = True
 
     with gr.Row(equal_height=False):
         with gr.Column():
             with gr.Row(visible = has_seconds_start or has_seconds_total):
                 # Timing controls
                 seconds_start_slider = gr.Slider(minimum=0, maximum=512, step=1, value=0, label="Seconds start", visible=has_seconds_start)
-                seconds_total_slider = gr.Slider(minimum=0, maximum=512, step=1, value=95, label="Seconds total", visible=has_seconds_total)
+                seconds_total_slider = gr.Slider(minimum=0, maximum=512, step=1, value=sample_size//sample_rate, label="Seconds total", visible=has_seconds_total)
             
             with gr.Row():
                 # Steps slider
                 steps_slider = gr.Slider(minimum=1, maximum=500, step=1, value=100, label="Steps")
 
                 # Preview Every slider
                 preview_every_slider = gr.Slider(minimum=0, maximum=100, step=1, value=0, label="Preview Every")
@@ -374,20 +375,20 @@
                 cfg_scale_slider = gr.Slider(minimum=0.0, maximum=25.0, step=0.1, value=7.0, label="CFG scale")
 
             with gr.Accordion("Sampler params", open=False):
             
                 # Seed
                 seed_textbox = gr.Textbox(label="Seed (set to -1 for random seed)", value="-1")
 
-            # Sampler params
+                # Sampler params
                 with gr.Row():
                     sampler_type_dropdown = gr.Dropdown(["dpmpp-2m-sde", "dpmpp-3m-sde", "k-heun", "k-lms", "k-dpmpp-2s-ancestral", "k-dpm-2", "k-dpm-fast"], label="Sampler type", value="dpmpp-2m-sde")
                     sigma_min_slider = gr.Slider(minimum=0.0, maximum=2.0, step=0.01, value=0.03, label="Sigma min")
                     sigma_max_slider = gr.Slider(minimum=0.0, maximum=200.0, step=0.1, value=80, label="Sigma max")
-                    cfg_rescale_slider = gr.Slider(minimum=0.0, maximum=1, step=0.01, value=0.4, label="CFG rescale amount")
+                    cfg_rescale_slider = gr.Slider(minimum=0.0, maximum=1, step=0.01, value=0.2, label="CFG rescale amount")
 
             if inpainting: 
                 # Inpainting Tab
                 with gr.Accordion("Inpainting", open=False):
                     sigma_max_slider.maximum=1000
                     
                     init_audio_checkbox = gr.Checkbox(label="Do inpainting")
@@ -477,15 +478,15 @@
 
 def create_diffusion_uncond_ui(model_config):
     with gr.Blocks() as ui:
         create_uncond_sampling_ui(model_config)
     
     return ui
 
-def autoencoder_process(audio, n_quantizers):
+def autoencoder_process(audio, latent_noise, n_quantizers):
 
     if torch.cuda.is_available():
         torch.cuda.empty_cache()
     gc.collect()
 
     #Get the device from the model
     device = next(model.parameters()).device
@@ -500,14 +501,17 @@
         audio = audio.transpose(0, 1)
 
     if n_quantizers > 0:
         latents = model.encode_audio(audio, in_sr, n_quantizers=n_quantizers)
     else:
         latents = model.encode_audio(audio, in_sr)
 
+    if latent_noise > 0:
+        latents = latents + torch.randn_like(latents) * latent_noise
+
     audio = model.decode_audio(latents)
 
     audio = rearrange(audio, "b d n -> d (b n)")
 
     audio = audio.clamp(-1, 1).mul(32767).to(torch.int16).cpu()
 
     torchaudio.save("output.wav", audio, sample_rate)
@@ -523,19 +527,64 @@
     else:
         n_quantizers = 0
 
     with gr.Blocks() as ui:
         input_audio = gr.Audio(label="Input audio")
         output_audio = gr.Audio(label="Output audio", interactive=False)
         n_quantizers_slider = gr.Slider(minimum=1, maximum=n_quantizers, step=1, value=n_quantizers, label="# quantizers", visible=is_dac_rvq)
+        latent_noise_slider = gr.Slider(minimum=0.0, maximum=10.0, step=0.001, value=0.0, label="Add latent noise")
         process_button = gr.Button("Process", variant='primary', scale=1)
-        process_button.click(fn=autoencoder_process, inputs=[input_audio, n_quantizers_slider], outputs=output_audio, api_name="process")
+        process_button.click(fn=autoencoder_process, inputs=[input_audio, latent_noise_slider, n_quantizers_slider], outputs=output_audio, api_name="process")
 
     return ui
 
+def diffusion_prior_process(audio, steps, sampler_type, sigma_min, sigma_max):
+
+    if torch.cuda.is_available():
+        torch.cuda.empty_cache()
+    gc.collect()
+
+    #Get the device from the model
+    device = next(model.parameters()).device
+
+    in_sr, audio = audio
+
+    audio = torch.from_numpy(audio).float().div(32767).to(device)
+    
+    if audio.dim() == 1:
+        audio = audio.unsqueeze(0) # [1, n]
+    elif audio.dim() == 2:
+        audio = audio.transpose(0, 1) # [n, 2] -> [2, n]
+
+    audio = audio.unsqueeze(0)
+
+    audio = generate_mono_to_stereo(model, audio, in_sr, steps, sampler_kwargs={"sampler_type": sampler_type, "sigma_min": sigma_min, "sigma_max": sigma_max})
+
+    audio = rearrange(audio, "b d n -> d (b n)")
+
+    audio = audio.clamp(-1, 1).mul(32767).to(torch.int16).cpu()
+
+    torchaudio.save("output.wav", audio, sample_rate)
+
+    return "output.wav"
+
+def create_diffusion_prior_ui(model_config):
+    with gr.Blocks() as ui:
+        input_audio = gr.Audio(label="Input audio")
+        output_audio = gr.Audio(label="Output audio", interactive=False)
+        # Sampler params
+        with gr.Row():
+            steps_slider = gr.Slider(minimum=1, maximum=500, step=1, value=100, label="Steps")
+            sampler_type_dropdown = gr.Dropdown(["dpmpp-2m-sde", "dpmpp-3m-sde", "k-heun", "k-lms", "k-dpmpp-2s-ancestral", "k-dpm-2", "k-dpm-fast"], label="Sampler type", value="dpmpp-2m-sde")
+            sigma_min_slider = gr.Slider(minimum=0.0, maximum=2.0, step=0.01, value=0.03, label="Sigma min")
+            sigma_max_slider = gr.Slider(minimum=0.0, maximum=200.0, step=0.1, value=80, label="Sigma max")
+        process_button = gr.Button("Process", variant='primary', scale=1)
+        process_button.click(fn=diffusion_prior_process, inputs=[input_audio, steps_slider, sampler_type_dropdown, sigma_min_slider, sigma_max_slider], outputs=output_audio, api_name="process")    
+
+    return ui
 
 def create_ui(model_config_path=None, ckpt_path=None, pretrained_name=None, pretransform_ckpt_path=None):
 
     assert (pretrained_name is not None) ^ (model_config_path is not None and ckpt_path is not None), "Must specify either pretrained name or provide a model config and checkpoint, but not both"
 
     if model_config_path is not None:
         # Load config from json file
@@ -551,10 +600,11 @@
 
     if model_type == "diffusion_cond":
         ui = create_txt2audio_ui(model_config)
     elif model_type == "diffusion_uncond":
         ui = create_diffusion_uncond_ui(model_config)
     elif model_type == "autoencoder" or model_type == "diffusion_autoencoder":
         ui = create_autoencoder_ui(model_config)
+    elif model_type == "diffusion_prior":
+        ui = create_diffusion_prior_ui(model_config)
         
-
     return ui
```

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/models/adp.py` & `stable-audio-tools-0.0.9/stable_audio_tools/models/adp.py`

 * *Files identical despite different names*

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/models/autoencoders.py` & `stable-audio-tools-0.0.9/stable_audio_tools/models/autoencoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,15 +272,16 @@
         latent_dim,
         downsampling_ratio,
         sample_rate,
         io_channels=2,
         bottleneck: Bottleneck = None,
         pretransform: Pretransform = None,
         in_channels = None,
-        out_channels = None
+        out_channels = None,
+        soft_clip = False
     ):
         super().__init__()
 
         self.downsampling_ratio = downsampling_ratio
         self.sample_rate = sample_rate
 
         self.latent_dim = latent_dim
@@ -299,35 +300,37 @@
         self.bottleneck = bottleneck
 
         self.encoder = encoder
 
         self.decoder = decoder
 
         self.pretransform = pretransform
+
+        self.soft_clip = soft_clip
  
     def encode(self, audio, return_info=False, skip_pretransform=False, iterate_batch=False, **kwargs):
 
         info = {}
 
         if self.pretransform is not None and not skip_pretransform:
             if self.pretransform.enable_grad:
                 if iterate_batch:
-                    audio = []
+                    audios = []
                     for i in range(audio.shape[0]):
-                        audio.append(self.pretransform.encode(audio[i:i+1]))
-                    audio = torch.cat(audio, dim=0)
+                        audios.append(self.pretransform.encode(audio[i:i+1]))
+                    audio = torch.cat(audios, dim=0)
                 else:
                     audio = self.pretransform.encode(audio)
             else:
                 with torch.no_grad():
                     if iterate_batch:
-                        audio = []
+                        audios = []
                         for i in range(audio.shape[0]):
-                            audio.append(self.pretransform.encode(audio[i:i+1]))
-                        audio = torch.cat(audio, dim=0)
+                            audios.append(self.pretransform.encode(audio[i:i+1]))
+                        audio = torch.cat(audios, dim=0)
                     else:
                         audio = self.pretransform.encode(audio)
 
         if self.encoder is not None:
             if iterate_batch:
                 latents = []
                 for i in range(audio.shape[0]):
@@ -339,15 +342,15 @@
             latents = audio
 
         if self.bottleneck is not None:
             # TODO: Add iterate batch logic, needs to merge the info dicts
             latents, bottleneck_info = self.bottleneck.encode(latents, return_info=True, **kwargs)
 
             info.update(bottleneck_info)
-                
+        
         if return_info:
             return latents, info
 
         return latents
 
     def decode(self, latents, iterate_batch=False, **kwargs):
 
@@ -367,29 +370,32 @@
             decoded = torch.cat(decoded, dim=0)
         else:
             decoded = self.decoder(latents, **kwargs)
 
         if self.pretransform is not None:
             if self.pretransform.enable_grad:
                 if iterate_batch:
-                    decoded = []
-                    for i in range(latents.shape[0]):
-                        decoded.append(self.pretransform.decode(decoded[i:i+1]))
-                    decoded = torch.cat(decoded, dim=0)
+                    decodeds = []
+                    for i in range(decoded.shape[0]):
+                        decodeds.append(self.pretransform.decode(decoded[i:i+1]))
+                    decoded = torch.cat(decodeds, dim=0)
                 else:
                     decoded = self.pretransform.decode(decoded)
             else:
                 with torch.no_grad():
                     if iterate_batch:
-                        decoded = []
+                        decodeds = []
                         for i in range(latents.shape[0]):
-                            decoded.append(self.pretransform.decode(decoded[i:i+1]))
-                        decoded = torch.cat(decoded, dim=0)
+                            decodeds.append(self.pretransform.decode(decoded[i:i+1]))
+                        decoded = torch.cat(decodeds, dim=0)
                     else:
                         decoded = self.pretransform.decode(decoded)
+
+        if self.soft_clip:
+            decoded = torch.tanh(decoded)
         
         return decoded
     
     def encode_audio(self, audio, in_sr, **kwargs):
         '''
         Encode single audio tensor to latents, including preprocessing the audio to be compatible with the model
         '''
@@ -437,15 +443,15 @@
         if self.encoder is not None:
             # Shrink the initial encoder parameters to avoid saturated latents
             with torch.no_grad():
                 for param in self.encoder.parameters():
                     param *= 0.5
 
     def decode(self, latents, steps=100):
-        
+
         upsampled_length = latents.shape[2] * self.downsampling_ratio
 
         if self.bottleneck is not None:
             latents = self.bottleneck.decode(latents)
 
         if self.decoder is not None:
             latents = self.decode(latents)
@@ -568,26 +574,29 @@
     pretransform = ae_config.get("pretransform", None)
 
     if pretransform is not None:
         pretransform = create_pretransform_from_config(pretransform, sample_rate)
 
     if bottleneck is not None:
         bottleneck = create_bottleneck_from_config(bottleneck)
-    
+
+    soft_clip = ae_config["decoder"].get("soft_clip", False)
+
     return AudioAutoencoder(
         encoder,
         decoder,
         io_channels=io_channels,
         latent_dim=latent_dim,
         downsampling_ratio=downsampling_ratio,
         sample_rate=sample_rate,
         bottleneck=bottleneck,
         pretransform=pretransform,
         in_channels=in_channels,
-        out_channels=out_channels
+        out_channels=out_channels,
+        soft_clip=soft_clip
     )
 
 def create_diffAE_from_config(config: Dict[str, Any]):
     
     diffae_config = config["model"]
 
     if "encoder" in diffae_config:
```

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/models/blocks.py` & `stable-audio-tools-0.0.9/stable_audio_tools/models/blocks.py`

 * *Files identical despite different names*

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/models/bottleneck.py` & `stable-audio-tools-0.0.9/stable_audio_tools/models/bottleneck.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import torch
 from torch import nn
 from torch.nn import functional as F
 
 from einops import rearrange
 from vector_quantize_pytorch import ResidualVQ, FSQ
-from nwt_pytorch import Memcodes
 from dac.nn.quantize import ResidualVectorQuantize as DACResidualVQ
 
 class Bottleneck(nn.Module):
     def __init__(self):
         super().__init__()
 
     def encode(self, x, return_info=False, **kwargs):
```

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/models/diffusion.py` & `stable-audio-tools-0.0.9/stable_audio_tools/models/diffusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import x_transformers
 from x_transformers import ContinuousTransformerWrapper, Encoder
 from einops import rearrange
 
 from .blocks import ResConvBlock, FourierFeatures, Upsample1d, Upsample1d_2, Downsample1d, Downsample1d_2, SelfAttention1d, SkipBlock, expand_to_planes
 from .conditioners import MultiConditioner, create_multi_conditioner_from_conditioning_config
 from .factory import create_pretransform_from_config
+from .local_attention import ContinuousLocalTransformer
 from .pretransforms import Pretransform
 from ..inference.generation import generate_diffusion_cond
 
 from .adp import UNetCFG1d, UNet1d
 
 from time import time
 
@@ -47,15 +48,15 @@
     def __init__(
                 self,
                 model: DiffusionModel,
                 io_channels,
                 sample_size,
                 sample_rate,
                 min_input_length,
-                pretransform: Pretransform = None,
+                pretransform: tp.Optional[Pretransform] = None,
     ):
         super().__init__()
         self.io_channels = io_channels
         self.sample_size = sample_size
         self.sample_rate = sample_rate
         self.min_input_length = min_input_length
 
@@ -106,15 +107,15 @@
     def __init__(
             self, 
             model: ConditionedDiffusionModel,
             conditioner: MultiConditioner,
             io_channels,
             sample_rate,
             min_input_length: int,
-            pretransform: Pretransform = None,
+            pretransform: tp.Optional[Pretransform] = None,
             cross_attn_cond_ids: tp.List[str] = [],
             global_cond_ids: tp.List[str] = [],
             input_concat_ids: tp.List[str] = [],
             prepend_cond_ids: tp.List[str] = [],
             ):
         super().__init__()
 
@@ -259,18 +260,35 @@
                 param *= 0.5
 
     def forward(self, 
                 x, 
                 t, 
                 input_concat_cond=None, 
                 global_cond=None, 
+                cross_attn_cond=None,
+                cross_attn_mask=None,
+                prepend_cond=None,
+                prepend_cond_mask=None,
+                cfg_scale=1.0,
+                cfg_dropout_prob: float = 0.0,
+                batch_cfg: bool = False,
+                rescale_cfg: bool = False,
+                negative_cross_attn_cond=None,
+                negative_cross_attn_mask=None,
+                negative_global_cond=None,
+                negative_input_concat_cond=None,
                 **kwargs):
 
         channels_list = None
         if input_concat_cond is not None:
+            
+            # Interpolate input_concat_cond to the same length as x
+            if input_concat_cond.shape[2] != x.shape[2]:
+                input_concat_cond = F.interpolate(input_concat_cond, (x.shape[2], ), mode='nearest')
+
             channels_list = [input_concat_cond]
 
         outputs = self.model(
             x, 
             t, 
             features=global_cond, 
             channels_list=channels_list,
@@ -527,14 +545,15 @@
         embed_dim=768,
         cond_token_dim=0,
         global_cond_dim=0,
         input_concat_dim=0,
         prepend_cond_dim=0,
         depth=12,
         num_heads=8,
+        transformer_type: tp.Literal["local_attn", "x-transformers"] = "x-transformers",
         **kwargs):
 
         super().__init__()
         
         self.cond_token_dim = cond_token_dim
 
         # Timestep embeddings
@@ -572,63 +591,51 @@
                 nn.Linear(embed_dim, embed_dim, bias=False)
             )
 
         self.input_concat_dim = input_concat_dim
 
         dim_in = io_channels + self.input_concat_dim
 
-        # RoPE monkey patch fix
-
-        def rotate_half(x):
-            x = rearrange(x, '... (j d) -> ... j d', j = 2)
-            x1, x2 = x.unbind(dim = -2)
-            return torch.cat((-x2, x1), dim = -1)
-
-        def apply_rotary_pos_emb(t, freqs, scale = 1):
-            out_dtype = t.dtype
-            dtype = reduce(torch.promote_types, (t.dtype, freqs.dtype, torch.float32))
-
-            rot_dim, seq_len = freqs.shape[-1], t.shape[-2]
-            freqs = freqs[-seq_len:, :]
-
-            if t.ndim == 4 and freqs.ndim == 3:
-                freqs = rearrange(freqs, 'b n d -> b 1 n d')
-
-            t, freqs = t.to(dtype), freqs.to(dtype)
-
-            # partial rotary embeddings, Wang et al. GPT-J
-            t, t_unrotated = t[..., :rot_dim], t[..., rot_dim:]
-            t = (t * freqs.cos() * scale) + (rotate_half(t) * freqs.sin() * scale)
-
-            t, t_unrotated = t.to(out_dtype), t_unrotated.to(out_dtype)
-
-            return torch.cat((t, t_unrotated), dim = -1) 
-
-        x_transformers.x_transformers.apply_rotary_pos_emb = torch.compile(apply_rotary_pos_emb)
-
         # Transformer
 
-        self.transformer = ContinuousTransformerWrapper(
-            dim_in=dim_in,
-            dim_out=io_channels,
-            max_seq_len=0, #Not relevant without absolute positional embeds
-            attn_layers = Encoder(
+        self.transformer_type = transformer_type
+
+        if self.transformer_type == "local_attn":
+            self.transformer = ContinuousLocalTransformer(
                 dim=embed_dim,
+                dim_in=dim_in,
+                dim_out=io_channels,
                 depth=depth,
                 heads=num_heads,
-                attn_flash = True,
-                cross_attend = cond_token_dim > 0,
-                zero_init_branch_output=True,
-                use_abs_pos_emb = False,
-                rotary_pos_emb=True,
-                ff_swish = True,
-                ff_glu = True,
+                cond_dim=embed_dim if global_cond_dim > 0 else 0,
+                cross_attn_cond_dim=embed_dim if cond_token_dim > 0 else 0,
                 **kwargs
             )
-        )
+
+        elif self.transformer_type == "x-transformers":
+            self.transformer = ContinuousTransformerWrapper(
+                dim_in=dim_in,
+                dim_out=io_channels,
+                max_seq_len=0, #Not relevant without absolute positional embeds
+                attn_layers = Encoder(
+                    dim=embed_dim,
+                    depth=depth,
+                    heads=num_heads,
+                    attn_flash = True,
+                    cross_attend = cond_token_dim > 0,
+                    zero_init_branch_output=True,
+                    use_abs_pos_emb = False,
+                    rotary_pos_emb=True,
+                    ff_swish = True,
+                    ff_glu = True,
+                    **kwargs
+                )
+            )
+        else:
+            raise ValueError(f"Unknown transformer type: {self.transformer_type}")
 
         self.preprocess_conv = nn.Conv1d(dim_in, dim_in, 1, bias=False)
         nn.init.zeros_(self.preprocess_conv.weight)
         self.postprocess_conv = nn.Conv1d(io_channels, io_channels, 1, bias=False)
         nn.init.zeros_(self.postprocess_conv.weight)
 
     def _forward(
@@ -677,21 +684,31 @@
                 prepend_mask = torch.cat([prepend_mask, prepend_cond_mask], dim=1)
             else:
                 prepend_mask = torch.cat([prepend_mask, torch.ones((x.shape[0], prepend_cond.shape[1]), device=x.device, dtype=torch.bool)], dim=1)
 
         prepend_length = prepend_inputs.shape[1]
 
         if input_concat_cond is not None:
+
+            # Interpolate input_concat_cond to the same length as x
+            if input_concat_cond.shape[2] != x.shape[2]:
+                input_concat_cond = F.interpolate(input_concat_cond, (x.shape[2], ), mode='nearest')
+
             x = torch.cat([x, input_concat_cond], dim=1)
 
         x = self.preprocess_conv(x) + x
 
         x = rearrange(x, "b c t -> b t c")
 
-        output = self.transformer(x, prepend_embeds=prepend_inputs, context=cross_attn_cond, context_mask=cross_attn_cond_mask, mask=mask, prepend_mask=prepend_mask, **kwargs)
+        if self.transformer_type == "local_attn":
+            if mask is not None:
+                mask = torch.cat([prepend_mask, mask], dim=1)
+            output = self.transformer(x, prepend_cond=prepend_inputs, cross_attn_cond=cross_attn_cond, cross_attn_cond_mask=cross_attn_cond_mask, mask=mask, **kwargs)
+        else:
+            output = self.transformer(x, prepend_embeds=prepend_inputs, context=cross_attn_cond, context_mask=cross_attn_cond_mask, mask=mask, prepend_mask=prepend_mask, **kwargs)
 
         output = rearrange(output, "b t c -> b c t")[:,:,prepend_length:]
 
         output = self.postprocess_conv(output) + output
 
         return output
 
@@ -720,74 +737,93 @@
             cross_attn_cond_mask = cross_attn_cond_mask.bool()
 
             cross_attn_cond_mask = None # Temporarily disabling conditioning masks due to kernel issue for flash attention
 
         if prepend_cond_mask is not None:
             prepend_cond_mask = prepend_cond_mask.bool()
 
-        if cross_attn_cond is not None:
-
-            # CFG dropout
-            if cfg_dropout_prob > 0.0:
+        # CFG dropout
+        if cfg_dropout_prob > 0.0:
+            if cross_attn_cond is not None:
                 null_embed = torch.zeros_like(cross_attn_cond, device=cross_attn_cond.device)
                 dropout_mask = torch.bernoulli(torch.full((cross_attn_cond.shape[0], 1, 1), cfg_dropout_prob, device=cross_attn_cond.device)).to(torch.bool)
                 cross_attn_cond = torch.where(dropout_mask, null_embed, cross_attn_cond)
 
-        if cross_attn_cond is not None and cfg_scale != 1.0:
+            if prepend_cond is not None:
+                null_embed = torch.zeros_like(prepend_cond, device=prepend_cond.device)
+                dropout_mask = torch.bernoulli(torch.full((prepend_cond.shape[0], 1, 1), cfg_dropout_prob, device=prepend_cond.device)).to(torch.bool)
+                prepend_cond = torch.where(dropout_mask, null_embed, prepend_cond)
+
+
+        if cfg_scale != 1.0 and (cross_attn_cond is not None or prepend_cond is not None):
             # Classifier-free guidance
             # Concatenate conditioned and unconditioned inputs on the batch dimension            
             batch_inputs = torch.cat([x, x], dim=0)
-            
-            null_embed = torch.zeros_like(cross_attn_cond, device=cross_attn_cond.device)
-
             batch_timestep = torch.cat([t, t], dim=0)
 
             if global_embed is not None:
                 batch_global_cond = torch.cat([global_embed, global_embed], dim=0)
             else:
                 batch_global_cond = None
 
-            if prepend_cond is not None:
-                batch_prepend_cond = torch.cat([prepend_cond, prepend_cond], dim=0)
+            if input_concat_cond is not None:
+                batch_input_concat_cond = torch.cat([input_concat_cond, input_concat_cond], dim=0)
             else:
-                batch_prepend_cond = None
+                batch_input_concat_cond = None
 
-            if prepend_cond_mask is not None:
-                batch_prepend_cond_mask = torch.cat([prepend_cond_mask, prepend_cond_mask], dim=0)
-            else:
-                batch_prepend_cond_mask = None
+            batch_cond = None
+            batch_cond_masks = None
+            
+            # Handle CFG for cross-attention conditioning
+            if cross_attn_cond is not None:
 
-            if negative_cross_attn_cond is not None:
-                if negative_cross_attn_mask is not None:
-                    negative_cross_attn_mask = negative_cross_attn_mask.to(torch.bool).unsqueeze(2)
+                null_embed = torch.zeros_like(cross_attn_cond, device=cross_attn_cond.device)
 
-                    negative_cross_attn_cond = torch.where(negative_cross_attn_mask, negative_cross_attn_cond, null_embed)
-                
-                batch_cond = torch.cat([cross_attn_cond, negative_cross_attn_cond], dim=0)
+                # For negative cross-attention conditioning, replace the null embed with the negative cross-attention conditioning
+                if negative_cross_attn_cond is not None:
 
-            else:
-                batch_cond = torch.cat([cross_attn_cond, null_embed], dim=0)
+                    # If there's a negative cross-attention mask, set the masked tokens to the null embed
+                    if negative_cross_attn_mask is not None:
+                        negative_cross_attn_mask = negative_cross_attn_mask.to(torch.bool).unsqueeze(2)
+
+                        negative_cross_attn_cond = torch.where(negative_cross_attn_mask, negative_cross_attn_cond, null_embed)
+                    
+                    batch_cond = torch.cat([cross_attn_cond, negative_cross_attn_cond], dim=0)
 
-            if cross_attn_cond_mask is not None:
-                batch_cond_masks = torch.cat([cross_attn_cond_mask, cross_attn_cond_mask], dim=0)
-            else:
-                batch_cond_masks = None
+                else:
+                    batch_cond = torch.cat([cross_attn_cond, null_embed], dim=0)
+
+                if cross_attn_cond_mask is not None:
+                    batch_cond_masks = torch.cat([cross_attn_cond_mask, cross_attn_cond_mask], dim=0)
+               
+            batch_prepend_cond = None
+            batch_prepend_cond_mask = None
+
+            if prepend_cond is not None:
+
+                null_embed = torch.zeros_like(prepend_cond, device=prepend_cond.device)
+
+                batch_prepend_cond = torch.cat([prepend_cond, null_embed], dim=0)
+                           
+                if prepend_cond_mask is not None:
+                    batch_prepend_cond_mask = torch.cat([prepend_cond_mask, prepend_cond_mask], dim=0)
+         
 
             if mask is not None:
                 batch_masks = torch.cat([mask, mask], dim=0)
             else:
                 batch_masks = None
             
             batch_output = self._forward(
                 batch_inputs, 
                 batch_timestep, 
                 cross_attn_cond=batch_cond, 
                 cross_attn_cond_mask=batch_cond_masks, 
                 mask = batch_masks, 
-                input_concat_cond=input_concat_cond, 
+                input_concat_cond=batch_input_concat_cond, 
                 global_embed = batch_global_cond,
                 prepend_cond = batch_prepend_cond,
                 prepend_cond_mask = batch_prepend_cond_mask,
                 **kwargs)
 
             cond_output, uncond_output = torch.chunk(batch_output, 2, dim=0)
             cfg_output = uncond_output + (cond_output - uncond_output) * cfg_scale
@@ -880,14 +916,16 @@
     assert diffusion_model_type is not None, "Must specify diffusion model type"
     
     diffusion_model_config = diffusion_config.get('config', None)
     assert diffusion_model_config is not None, "Must specify diffusion model config"
 
     if diffusion_model_type == 'adp_cfg_1d':
         diffusion_model = UNetCFG1DWrapper(**diffusion_model_config)
+    elif diffusion_model_type == 'adp_1d':
+        diffusion_model = UNet1DCondWrapper(**diffusion_model_config)
     elif diffusion_model_type == 'dit':
         diffusion_model = DiTWrapper(**diffusion_model_config)
 
     io_channels = model_config.get('io_channels', None)
     assert io_channels is not None, "Must specify io_channels in model config"
 
     sample_rate = config.get('sample_rate', None)
@@ -908,15 +946,15 @@
     
     if pretransform is not None:
         pretransform = create_pretransform_from_config(pretransform, sample_rate)
         min_input_length = pretransform.downsampling_ratio
     else:
         min_input_length = 1
 
-    if diffusion_model_type == "adp_cfg_1d":
+    if diffusion_model_type == "adp_cfg_1d" or diffusion_model_type == "adp_1d":
         min_input_length *= np.prod(diffusion_model_config["factors"])
     elif diffusion_model_type == "dit":
         min_input_length = min_input_length # There's no downsampling in DiT
 
     return ConditionedDiffusionModelWrapper(
         diffusion_model, 
         conditioner,
```

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/models/discriminators.py` & `stable-audio-tools-0.0.9/stable_audio_tools/models/discriminators.py`

 * *Files identical despite different names*

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/models/factory.py` & `stable-audio-tools-0.0.9/stable_audio_tools/models/factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import json
+
 def create_model_from_config(model_config):
     model_type = model_config.get('model_type', None)
 
     assert model_type is not None, 'model_type must be specified in model config'
 
     if model_type == 'autoencoder':
         from .autoencoders import create_autoencoder_from_config
@@ -16,15 +18,21 @@
         from .autoencoders import create_diffAE_from_config
         return create_diffAE_from_config(model_config)
     elif model_type == 'musicgen':
         from .musicgen import create_musicgen_from_config
         return create_musicgen_from_config(model_config)
     else:
         raise NotImplementedError(f'Unknown model type: {model_type}')
+
+def create_model_from_config_path(model_config_path):
+    with open(model_config_path) as f:
+        model_config = json.load(f)
     
+    return create_model_from_config(model_config)
+
 def create_pretransform_from_config(pretransform_config, sample_rate):
     pretransform_type = pretransform_config.get('type', None)
 
     assert pretransform_type is not None, 'type must be specified in pretransform config'
 
     if pretransform_type == 'autoencoder':
         from .autoencoders import create_autoencoder_from_config
```

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/models/local_attention.py` & `stable-audio-tools-0.0.9/stable_audio_tools/models/local_attention.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import torch
+
 from einops import rearrange
 from torch import nn
 from local_attention.transformer import LocalMHA, FeedForward
 
 from .adp import Attention
 from .blocks import AdaRMSNorm
 
@@ -19,14 +21,15 @@
         heads = 8,
         ff_mult = 4,
         attn_dropout = 0.,
         ff_dropout = 0.,
         use_conv = True,
         cond_dim = 0,
         cross_attn_cond_dim = 0,
+        use_rotary_pos_emb = False,
         **kwargs
     ):
         super().__init__()
         
         dim_head = dim//heads
 
         qk_scale = dim_head ** 0.5
@@ -45,39 +48,48 @@
 
         self.cross_attn_cond_dim = cross_attn_cond_dim
        
         for _ in range(depth):
 
             self.layers.append(nn.ModuleList([
                 AdaRMSNorm(dim, cond_dim, eps=1e-8) if cond_dim > 0 else nn.LayerNorm(dim, eps=1e-8),
-                LocalMHA(dim = dim, dim_head = dim_head, heads = heads, qk_scale=qk_scale, dropout = attn_dropout, causal = causal, window_size = local_attn_window_size, prenorm = False, **kwargs),
+                LocalMHA(
+                    dim = dim, 
+                    dim_head = dim_head, 
+                    heads = heads, 
+                    qk_scale=qk_scale, 
+                    dropout = attn_dropout, 
+                    causal = causal, 
+                    window_size = local_attn_window_size, 
+                    prenorm = False, 
+                    use_rotary_pos_emb = use_rotary_pos_emb,
+                    **kwargs),
                 Attention(features=dim, num_heads=heads, head_features=dim_head, context_features=self.cross_attn_cond_dim) if self.cross_attn_cond_dim > 0 else nn.Identity(),
                 nn.Conv1d(dim, dim, kernel_size=3, padding=1) if use_conv else nn.Identity(),
                 FeedForward(dim = dim, mult = ff_mult, dropout = ff_dropout)
             ]))
 
-            if use_conv:
-                # Zero-init conv layers
-                nn.init.zeros_(self.layers[-1][1].weight)
-
-    def forward(self, x, mask = None, cond = None, cross_attn_cond = None):
-    
+    def forward(self, x, mask = None, cond = None, cross_attn_cond = None, cross_attn_cond_mask = None, prepend_cond = None):
+ 
         x = self.project_in(x)
 
+        if prepend_cond is not None:
+            x = torch.cat([prepend_cond, x], dim=1)
+
         for norm, attn, xattn, conv, ff in self.layers:
 
             if cond is not None:
                 x = norm(x, cond)
             else:
                 x = norm(x)
 
             x = attn(x, mask = mask) + x
 
             if cross_attn_cond is not None:
-                x = xattn(x, cross_attn_cond) + x
+                x = xattn(x, context=cross_attn_cond, context_mask=cross_attn_cond_mask) + x
 
             if self.use_conv:
                 x = rearrange(x, "b n c -> b c n")
                 x = conv(x) + x
                 x = rearrange(x, "b c n -> b n c")
                 
             x = ff(x) + x
```

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/models/musicgen.py` & `stable-audio-tools-0.0.9/stable_audio_tools/models/musicgen.py`

 * *Files identical despite different names*

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/models/pqmf.py` & `stable-audio-tools-0.0.9/stable_audio_tools/models/pqmf.py`

 * *Files identical despite different names*

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/models/pretransforms.py` & `stable-audio-tools-0.0.9/stable_audio_tools/models/pretransforms.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from torch import nn
 
 class Pretransform(nn.Module):
     def __init__(self, enable_grad=False, io_channels=2, ):
         super().__init__()
 
         self.io_channels = io_channels
+        self.encoded_channels = None
         self.downsampling_ratio = None
 
         self.enable_grad = enable_grad
 
     def encode(self, x):
         return x
 
@@ -25,14 +26,16 @@
         self.downsampling_ratio = model.downsampling_ratio
         self.io_channels = model.io_channels
         self.sample_rate = model.sample_rate
         
         self.model_half = model_half
         self.iterate_batch = iterate_batch
 
+        self.encoded_channels = model.latent_dim
+
         if self.model_half:
             self.model.half()
     
     def encode(self, x, **kwargs):
         
         if self.model_half:
             x = x.half()
@@ -67,14 +70,15 @@
         from .wavelets import WaveletEncode1d, WaveletDecode1d
 
         self.encoder = WaveletEncode1d(channels, levels, wavelet)
         self.decoder = WaveletDecode1d(channels, levels, wavelet)
 
         self.downsampling_ratio = 2 ** levels
         self.io_channels = channels
+        self.encoded_channels = channels * self.downsampling_ratio
     
     def encode(self, x):
         return self.encoder(x)
     
     def decode(self, z):
         return self.decoder(z)
     
@@ -117,14 +121,16 @@
 
         self.io_channels = 1
 
         self.scale = scale
 
         self.chunked = chunked
 
+        self.encoded_channels = self.model.latent_dim
+
     def encode(self, x):
 
         latents = self.model.encoder(x)
 
         if self.quantize_on_decode:
             output = latents
         else:
```

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/models/wavelets.py` & `stable-audio-tools-0.0.9/stable_audio_tools/models/wavelets.py`

 * *Files identical despite different names*

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/training/autoencoders.py` & `stable-audio-tools-0.0.9/stable_audio_tools/training/autoencoders.py`

 * *Files 6% similar despite different names*

```diff
@@ -123,14 +123,15 @@
        
         # Spectral reconstruction loss
 
         stft_loss_args = loss_config['spectral']['config']
 
         if self.autoencoder.out_channels == 2:
             self.sdstft = auraloss.freq.SumAndDifferenceSTFTLoss(sample_rate=sample_rate, **stft_loss_args)
+            self.lrstft = auraloss.freq.MultiResolutionSTFTLoss(sample_rate=sample_rate, **stft_loss_args)
         else:
             self.sdstft = auraloss.freq.MultiResolutionSTFTLoss(sample_rate=sample_rate, **stft_loss_args)
 
         # Discriminator
 
         if loss_config['discriminator']['type'] == 'oobleck':
             self.discriminator = OobleckDiscriminator(**loss_config['discriminator']['config'])
@@ -161,14 +162,26 @@
         else:
 
             # Reconstruction loss
             self.gen_loss_modules += [
                 AuralossLoss(self.sdstft, 'reals', 'decoded', name='mrstft_loss', weight=self.loss_config['spectral']['weights']['mrstft']),
             ]
 
+            if self.autoencoder.out_channels == 2:
+
+                # Add left and right channel reconstruction losses in addition to the sum and difference
+                self.gen_loss_modules += [
+                    AuralossLoss(self.lrstft, 'reals_left', 'decoded_left', name='stft_loss_left', weight=self.loss_config['spectral']['weights']['mrstft']/2),
+                    AuralossLoss(self.lrstft, 'reals_right', 'decoded_right', name='stft_loss_right', weight=self.loss_config['spectral']['weights']['mrstft']/2),
+                ]
+
+            self.gen_loss_modules += [
+                AuralossLoss(self.sdstft, 'reals', 'decoded', name='mrstft_loss', weight=self.loss_config['spectral']['weights']['mrstft']),
+            ]
+
         if self.loss_config['time']['weights']['l1'] > 0.0:
             self.gen_loss_modules.append(L1Loss(key_a='reals', key_b='decoded', weight=self.loss_config['time']['weights']['l1'], name='l1_time_loss'))
 
         if self.autoencoder.bottleneck is not None:
             self.gen_loss_modules += create_loss_modules_from_bottleneck(self.autoencoder.bottleneck, self.loss_config)
 
         self.losses_gen = MultiLoss(self.gen_loss_modules)
@@ -252,14 +265,20 @@
             mask = torch.rand_like(latents) < self.latent_mask_ratio
             latents = torch.where(mask, torch.zeros_like(latents), latents)
 
         decoded = self.autoencoder.decode(latents)
 
         loss_info["decoded"] = decoded
 
+        if self.autoencoder.out_channels == 2:
+            loss_info["decoded_left"] = decoded[:, 0:1, :]
+            loss_info["decoded_right"] = decoded[:, 1:2, :]
+            loss_info["reals_left"] = reals[:, 0:1, :]
+            loss_info["reals_right"] = reals[:, 1:2, :]
+
         # Distillation
         if self.teacher_model is not None:
             with torch.no_grad():
                 teacher_decoded = self.teacher_model.decode(teacher_latents)
                 own_latents_teacher_decoded = self.teacher_model.decode(latents) #Distilled model's latents decoded by teacher
                 teacher_latents_own_decoded = self.autoencoder.decode(teacher_latents) #Teacher's latents decoded by distilled model
```

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/training/diffusion.py` & `stable-audio-tools-0.0.9/stable_audio_tools/training/diffusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         loss_info["audio_reals"] = diffusion_input
 
         if self.diffusion.pretransform is not None:
             with torch.set_grad_enabled(self.diffusion.pretransform.enable_grad):
                 diffusion_input = self.diffusion.pretransform.encode(diffusion_input)
                 loss_info["reals"] = diffusion_input
 
-        # Combine the ground truth images and the noise
+        # Combine the ground truth data and the noise
         alphas = alphas[:, None, None]
         sigmas = sigmas[:, None, None]
         noise = torch.randn_like(diffusion_input)
         noised_inputs = diffusion_input * alphas + noise * sigmas
         targets = noise * alphas - diffusion_input * sigmas
 
         with torch.cuda.amp.autocast():
@@ -209,28 +209,32 @@
     '''
     def __init__(
             self,
             model: ConditionedDiffusionModelWrapper,
             lr: float = 1e-4,
             causal_dropout: float = 0.0,
             mask_padding: bool = False,
-            mask_padding_dropout: float = 0.2
+            mask_padding_dropout: float = 0.2,
+            use_ema: bool = True
     ):
         super().__init__()
 
         self.diffusion = model
         
-        self.diffusion_ema = EMA(
-            self.diffusion.model,
-            beta=0.9999,
-            power=3/4,
-            update_every=1,
-            update_after_step=1,
-            include_online_model=False
-        )
+        if use_ema:
+            self.diffusion_ema = EMA(
+                self.diffusion.model,
+                beta=0.9999,
+                power=3/4,
+                update_every=1,
+                update_after_step=1,
+                include_online_model=False
+            )
+        else:
+            self.diffusion_ema = None
 
         self.mask_padding = mask_padding
         self.mask_padding_dropout = mask_padding_dropout
 
         self.lr = lr
 
         self.rng = torch.quasirandom.SobolEngine(1, scramble=True)
@@ -292,15 +296,15 @@
                 p.tick("pretransform")
 
                 # If mask_padding is on, interpolate the padding masks to the size of the pretransformed input
                 if use_padding_mask:
                     padding_masks = F.interpolate(padding_masks.unsqueeze(1).float(), size=diffusion_input.shape[2], mode="nearest").squeeze(1).bool()
 
 
-        # Combine the ground truth images and the noise
+        # Combine the ground truth data and the noise
         alphas = alphas[:, None, None]
         sigmas = sigmas[:, None, None]
         noise = torch.randn_like(diffusion_input)
         noised_inputs = diffusion_input * alphas + noise * sigmas
         targets = noise * alphas - diffusion_input * sigmas
 
         p.tick("noise")
@@ -336,18 +340,20 @@
 
         self.log_dict(log_dict, prog_bar=True, on_step=True)
         p.tick("log")
         #print(f"Profiler: {p}")
         return loss
     
     def on_before_zero_grad(self, *args, **kwargs):
-        self.diffusion_ema.update()
+        if self.diffusion_ema is not None:
+            self.diffusion_ema.update()
 
     def export_model(self, path, use_safetensors=False):
-        self.diffusion.model = self.diffusion_ema.ema_model
+        if self.diffusion_ema is not None:
+            self.diffusion.model = self.diffusion_ema.ema_model
         
         if use_safetensors:
             save_file(self.diffusion.state_dict(), path)
         else:
             torch.save({"state_dict": self.diffusion.state_dict()}, path)
 
 class DiffusionCondDemoCallback(pl.Callback):
@@ -425,15 +431,17 @@
                 trainer.logger.experiment.log(log_dict)
 
             for cfg_scale in self.demo_cfg_scales:
 
                 print(f"Generating demo for cfg scale {cfg_scale}")
                 
                 with torch.cuda.amp.autocast():
-                    fakes = sample(module.diffusion_ema.model, noise, self.demo_steps, 0, **cond_inputs, cfg_scale=cfg_scale, batch_cfg=True)
+                    model = module.diffusion_ema.model if module.diffusion_ema is not None else module.diffusion.model
+
+                    fakes = sample(model, noise, self.demo_steps, 0, **cond_inputs, cfg_scale=cfg_scale, batch_cfg=True)
                     if module.diffusion.pretransform is not None:
                         fakes = module.diffusion.pretransform.decode(fakes)
 
                 # Put the demos together
                 fakes = rearrange(fakes, 'b d n -> d (b n)')
 
                 log_dict = {}
@@ -463,14 +471,15 @@
     '''
     Wrapper for training a conditional audio diffusion model.
     '''
     def __init__(
             self,
             model: ConditionedDiffusionModelWrapper,
             lr: float = 1e-4,
+            max_mask_segments = 10
     ):
         super().__init__()
 
         self.diffusion = model
         
         self.diffusion_ema = EMA(
             self.diffusion.model,
@@ -478,75 +487,69 @@
             power=3/4,
             update_every=1,
             update_after_step=1,
             include_online_model=False
         )
 
         self.lr = lr
+        self.max_mask_segments = max_mask_segments
 
         self.rng = torch.quasirandom.SobolEngine(1, scramble=True)
 
         self.loss_modules = [
             MSELoss("v", 
                    "targets", 
                    weight=1.0, 
-                   mask_key="padding_mask" if self.mask_padding else None, 
                    name="mse_loss"
             )
         ]
 
         self.losses = MultiLoss(self.loss_modules)
 
     def configure_optimizers(self):
         return optim.Adam([*self.diffusion.parameters()], lr=self.lr)
 
     def random_mask(self, sequence, max_mask_length):
-
         b, _, sequence_length = sequence.size()
 
         # Create a mask tensor for each batch element
         masks = []
-       # for i in range(b):
-        mask_type = random.randint(0, 2)
 
-        if mask_type == 0: # Random mask
-            # Randomly choose the length and starting index of the mask
-            mask_length = random.randint(1, max_mask_length)
-            mask_start = random.randint(0, sequence_length-mask_length)
-
-            # Create the mask tensor
-            mask = torch.ones((1, 1, sequence_length))
-            mask[:, :, mask_start:mask_start+mask_length] = 0
-            mask = mask.to(sequence.device)
+        for i in range(b):
+            mask_type = random.randint(0, 2)
 
-            masks.append(mask)
-            causal = False
+            if mask_type == 0:  # Random mask with multiple segments
+                num_segments = random.randint(1, self.max_mask_segments)
+                max_segment_length = max_mask_length // num_segments
+
+                segment_lengths = random.sample(range(1, max_segment_length + 1), num_segments)
+               
+                mask = torch.ones((1, 1, sequence_length))
+                for length in segment_lengths:
+                    mask_start = random.randint(0, sequence_length - length)
+                    mask[:, :, mask_start:mask_start + length] = 0
+
+            elif mask_type == 1:  # Full mask
+                mask = torch.zeros((1, 1, sequence_length))
+
+            elif mask_type == 2:  # Causal mask
+                mask = torch.ones((1, 1, sequence_length))
+                mask_length = random.randint(1, max_mask_length)
+                mask[:, :, -mask_length:] = 0
 
-        elif mask_type == 1: # Full mask
-            mask = torch.zeros((1, 1, sequence_length)).to(sequence.device)
+            mask = mask.to(sequence.device)
             masks.append(mask)
-            causal = False
 
-        elif mask_type == 2: # Causal mask
-            mask = torch.ones((1, 1, sequence_length)).to(sequence.device)
-            mask_length = random.randint(1, max_mask_length)
-            mask[:, :, -mask_length:] = 0
-            masks.append(mask)
-            causal = True
-                
-        # Repeat masks to batch size
-        masks = masks * b
-        
         # Concatenate the mask tensors into a single tensor
         mask = torch.cat(masks, dim=0).to(sequence.device)
 
         # Apply the mask to the sequence tensor for each batch element
         masked_sequence = sequence * mask
 
-        return masked_sequence, mask, causal
+        return masked_sequence, mask
 
     def training_step(self, batch, batch_idx):
         reals, metadata = batch
 
         p = Profiler()
 
         if reals.ndim == 4 and reals.shape[0] == 1:
@@ -573,31 +576,31 @@
                 diffusion_input = self.diffusion.pretransform.encode(diffusion_input)
                 p.tick("pretransform")
 
         # Max mask size is the full sequence length
         max_mask_length = diffusion_input.shape[2]
 
         # Create a mask of random length for a random slice of the input
-        masked_input, mask, causal = self.random_mask(diffusion_input, max_mask_length)
+        masked_input, mask = self.random_mask(diffusion_input, max_mask_length)
 
         conditioning['inpaint_mask'] = [mask]
         conditioning['inpaint_masked_input'] = [masked_input]
 
-        # Combine the ground truth images and the noise
+        # Combine the ground truth data and the noise
         alphas = alphas[:, None, None]
         sigmas = sigmas[:, None, None]
         noise = torch.randn_like(diffusion_input)
         noised_inputs = diffusion_input * alphas + noise * sigmas
         targets = noise * alphas - diffusion_input * sigmas
 
         p.tick("noise")
 
         with torch.cuda.amp.autocast():
             p.tick("amp")
-            v = self.diffusion(noised_inputs, t, cond=conditioning, cfg_dropout_prob = 0.1, causal=causal)
+            v = self.diffusion(noised_inputs, t, cond=conditioning, cfg_dropout_prob = 0.1)
             p.tick("diffusion")
 
             loss_info = {
                 "v": v,
                 "targets": targets
             }
 
@@ -673,15 +676,15 @@
                     demo_reals = module.diffusion.pretransform.encode(demo_reals)
 
             demo_samples = demo_reals.shape[2]
 
             # Get conditioning
             conditioning = module.diffusion.conditioner(metadata, module.device)
 
-            masked_input, mask, causal = module.random_mask(demo_reals, demo_reals.shape[2])
+            masked_input, mask = module.random_mask(demo_reals, demo_reals.shape[2])
 
             conditioning['inpaint_mask'] = [mask]
             conditioning['inpaint_masked_input'] = [masked_input]
 
             if module.diffusion.pretransform is not None:
                 log_dict[f'demo_masked_input'] = wandb.Image(tokens_spectrogram_image(masked_input.cpu()))
             else:
@@ -692,15 +695,15 @@
             noise = torch.randn([demo_reals.shape[0], module.diffusion.io_channels, demo_samples]).to(module.device)
 
             trainer.logger.experiment.log(log_dict)
 
             for cfg_scale in self.demo_cfg_scales:
                 
                 print(f"Generating demo for cfg scale {cfg_scale}")
-                fakes = sample(module.diffusion_ema.model, noise, self.demo_steps, 0, **cond_inputs, cfg_scale=cfg_scale, batch_cfg=True, causal=causal)
+                fakes = sample(module.diffusion_ema.model, noise, self.demo_steps, 0, **cond_inputs, cfg_scale=cfg_scale, batch_cfg=True)
 
                 if module.diffusion.pretransform is not None:
                     with torch.cuda.amp.autocast():
                         fakes = module.diffusion.pretransform.decode(fakes)
 
                 # Put the demos together
                 fakes = rearrange(fakes, 'b d n -> d (b n)')
@@ -831,15 +834,15 @@
 
         # Draw uniformly distributed continuous timesteps
         t = self.rng.draw(reals.shape[0])[:, 0].to(self.device)
 
         # Calculate the noise schedule parameters for those timesteps
         alphas, sigmas = get_alphas_sigmas(t)
 
-        # Combine the ground truth images and the noise
+        # Combine the ground truth data and the noise
         alphas = alphas[:, None, None]
         sigmas = sigmas[:, None, None]
         noise = torch.randn_like(reals)
         noised_reals = reals * alphas + noise * sigmas
         targets = noise * alphas - reals * sigmas
 
         with torch.cuda.amp.autocast():
@@ -872,16 +875,22 @@
 
         self.log_dict(log_dict, prog_bar=True, on_step=True)
         return loss
     
     def on_before_zero_grad(self, *args, **kwargs):
         self.diffae_ema.update()
 
-    def export_model(self, path):        
-        save_file(self.diffae_ema.ema_model.state_dict(), path)
+    def export_model(self, path, use_safetensors=False):
+
+        model = self.diffae_ema.ema_model
+        
+        if use_safetensors:
+            save_file(model.state_dict(), path)
+        else:
+            torch.save({"state_dict": model.state_dict()}, path)
 
 class DiffusionAutoencoderDemoCallback(pl.Callback):
     def __init__(
         self, 
         demo_dl, 
         demo_every=2000,
         demo_steps=250,
@@ -961,14 +970,16 @@
 
         trainer.logger.experiment.log(log_dict)
 
 
 class DiffusionPriorTrainingWrapper(pl.LightningModule):
     '''
     Wrapper for training a diffusion prior for inverse problems
+    Prior types:
+        mono_stereo: The prior is conditioned on a mono version of the audio to generate a stereo version
     '''
     def __init__(
             self,
             model: ConditionedDiffusionModelWrapper,
             lr: float = 1e-4,
             ema_copy = None,
             prior_type: tp.Literal["mono_stereo"] = "mono_stereo"
@@ -985,16 +996,14 @@
             update_every=1,
             update_after_step=1,
             include_online_model=False
         )
 
         self.lr = lr
 
-        self.prior_type = prior_type
-
         self.rng = torch.quasirandom.SobolEngine(1, scramble=True)
 
         loss_modules = [
             MSELoss("v",
                     "targets",
                     weight=1.0,
                     name="mse_loss"
@@ -1019,25 +1028,27 @@
         if self.prior_type == "mono_stereo":
             source = reals.mean(dim=1, keepdim=True).repeat(1, reals.shape[1], 1).to(self.device)
             loss_info["audio_reals_mono"] = source
         
         if self.diffusion.pretransform is not None:
             with torch.no_grad():
                 reals = self.diffusion.pretransform.encode(reals)
-                source = self.diffusion.pretransform.encode(source)
+
+                if self.prior_type == "mono_stereo":
+                    source = self.diffusion.pretransform.encode(source)
 
         loss_info["reals"] = reals
 
         # Draw uniformly distributed continuous timesteps
         t = self.rng.draw(reals.shape[0])[:, 0].to(self.device)
 
         # Calculate the noise schedule parameters for those timesteps
         alphas, sigmas = get_alphas_sigmas(t)
 
-        # Combine the ground truth images and the noise
+        # Combine the ground truth data and the noise
         alphas = alphas[:, None, None]
         sigmas = sigmas[:, None, None]
         noise = torch.randn_like(reals)
         noised_reals = reals * alphas + noise * sigmas
         targets = noise * alphas - reals * sigmas
 
         with torch.cuda.amp.autocast():
@@ -1061,16 +1072,23 @@
 
         self.log_dict(log_dict, prog_bar=True, on_step=True)
         return loss
     
     def on_before_zero_grad(self, *args, **kwargs):
         self.diffusion_ema.update()
 
-    def export_model(self, path):        
-        save_file(self.diffusion_ema.ema_model.state_dict(), path)
+    def export_model(self, path, use_safetensors=False):
+
+        #model = self.diffusion_ema.ema_model
+        model = self.diffusion
+        
+        if use_safetensors:
+            save_file(model.state_dict(), path)
+        else:
+            torch.save({"state_dict": model.state_dict()}, path)
 
 class DiffusionPriorDemoCallback(pl.Callback):
     def __init__(
         self, 
         demo_dl, 
         demo_every=2000,
         demo_steps=250,
@@ -1105,16 +1123,17 @@
 
         with torch.no_grad() and torch.cuda.amp.autocast():
             if module.prior_type == "mono_stereo" and encoder_input.shape[1] > 1:
                 source = encoder_input.mean(dim=1, keepdim=True).repeat(1, encoder_input.shape[1], 1).to(module.device)
             
                 if module.diffusion.pretransform is not None:
                         source = module.diffusion.pretransform.encode(source)
-                        encoder_input = module.diffusion.pretransform.encode(encoder_input)
 
+            if module.diffusion.pretransform is not None:
+                    encoder_input = module.diffusion.pretransform.encode(encoder_input)
 
             fakes = sample(module.diffusion_ema.model, torch.randn_like(encoder_input), self.demo_steps, 0, cond={"source": [source]})
 
             if module.diffusion.pretransform is not None:
                 fakes = module.diffusion.pretransform.decode(fakes)
 
         #Interleave reals and fakes
```

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/training/factory.py` & `stable-audio-tools-0.0.9/stable_audio_tools/training/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,32 +62,35 @@
     elif model_type == 'diffusion_cond':
         from .diffusion import DiffusionCondTrainingWrapper
         return DiffusionCondTrainingWrapper(
             model, 
             lr=training_config["learning_rate"],
             causal_dropout=training_config.get("causal_dropout", 0.0),
             mask_padding=training_config.get("mask_padding", False),
+            use_ema = training_config.get("use_ema", True),
         )
     elif model_type == 'diffusion_prior':
         from .diffusion import DiffusionPriorTrainingWrapper
 
         ema_copy = create_model_from_config(model_config)
         
         # Copy each weight to the ema copy
         for name, param in model.state_dict().items():
             if isinstance(param, Parameter):
                 # backwards compatibility for serialized parameters
                 param = param.data
             ema_copy.state_dict()[name].copy_(param)
 
+        prior_type = training_config.get("prior_type", "mono_stereo")
+
         return DiffusionPriorTrainingWrapper(
             model, 
             lr=training_config["learning_rate"],
             ema_copy=ema_copy,
-            prior_type=training_config.get("prior_type", "mono_stereo"),
+            prior_type=prior_type
         )
     elif model_type == 'diffusion_cond_inpaint':
         from .diffusion import DiffusionCondInpaintTrainingWrapper
         return DiffusionCondInpaintTrainingWrapper(
             model, 
             lr=training_config["learning_rate"]
         )
```

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/training/losses.py` & `stable-audio-tools-0.0.9/stable_audio_tools/training/losses.py`

 * *Files identical despite different names*

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/training/musicgen.py` & `stable-audio-tools-0.0.9/stable_audio_tools/training/musicgen.py`

 * *Files identical despite different names*

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools/training/utils.py` & `stable-audio-tools-0.0.9/stable_audio_tools/training/utils.py`

 * *Files identical despite different names*

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools.egg-info/PKG-INFO` & `stable-audio-tools-0.0.9/stable_audio_tools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: stable-audio-tools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Training and inference tools for generative audio models from Stability AI
 Home-page: https://github.com/Stability-AI/stable-audio-tools.git
 Author: Stability AI
 License-File: LICENSE
 Requires-Dist: audiocraft==1.0.0
 Requires-Dist: aeiou==0.0.20
 Requires-Dist: alias-free-torch==0.0.6
 Requires-Dist: auraloss==0.4.0
 Requires-Dist: descript-audio-codec==1.0.0
 Requires-Dist: einops==0.7.0
 Requires-Dist: einops-exts==0.0.4
 Requires-Dist: ema-pytorch==0.2.3
 Requires-Dist: encodec==0.1.1
 Requires-Dist: gradio==3.42.0
+Requires-Dist: huggingface_hub
 Requires-Dist: importlib-resources==5.12.0
 Requires-Dist: k-diffusion==0.1.1
 Requires-Dist: laion-clap==1.1.4
 Requires-Dist: local-attention==1.8.6
-Requires-Dist: nwt-pytorch==0.0.4
 Requires-Dist: pandas==2.0.2
 Requires-Dist: pedalboard==0.7.4
 Requires-Dist: prefigure==0.0.9
 Requires-Dist: pytorch_lightning==2.1.0
 Requires-Dist: PyWavelets==1.4.1
 Requires-Dist: safetensors
 Requires-Dist: sentencepiece==0.1.99
```

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools.egg-info/SOURCES.txt` & `stable-audio-tools-0.0.9/stable_audio_tools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 stable_audio_tools.egg-info/requires.txt
 stable_audio_tools.egg-info/top_level.txt
 stable_audio_tools/data/__init__.py
 stable_audio_tools/data/dataset.py
 stable_audio_tools/data/utils.py
 stable_audio_tools/inference/__init__.py
 stable_audio_tools/inference/generation.py
+stable_audio_tools/inference/priors.py
 stable_audio_tools/inference/sampling.py
 stable_audio_tools/inference/utils.py
 stable_audio_tools/interface/__init__.py
 stable_audio_tools/interface/gradio.py
 stable_audio_tools/models/__init__.py
 stable_audio_tools/models/adp.py
 stable_audio_tools/models/autoencoders.py
@@ -25,14 +26,15 @@
 stable_audio_tools/models/conditioners.py
 stable_audio_tools/models/diffusion.py
 stable_audio_tools/models/discriminators.py
 stable_audio_tools/models/factory.py
 stable_audio_tools/models/local_attention.py
 stable_audio_tools/models/musicgen.py
 stable_audio_tools/models/pqmf.py
+stable_audio_tools/models/pretrained.py
 stable_audio_tools/models/pretransforms.py
 stable_audio_tools/models/utils.py
 stable_audio_tools/models/wavelets.py
 stable_audio_tools/training/__init__.py
 stable_audio_tools/training/autoencoders.py
 stable_audio_tools/training/diffusion.py
 stable_audio_tools/training/factory.py
```

### Comparing `stable-audio-tools-0.0.8/stable_audio_tools.egg-info/requires.txt` & `stable-audio-tools-0.0.9/stable_audio_tools.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 auraloss==0.4.0
 descript-audio-codec==1.0.0
 einops==0.7.0
 einops-exts==0.0.4
 ema-pytorch==0.2.3
 encodec==0.1.1
 gradio==3.42.0
+huggingface_hub
 importlib-resources==5.12.0
 k-diffusion==0.1.1
 laion-clap==1.1.4
 local-attention==1.8.6
-nwt-pytorch==0.0.4
 pandas==2.0.2
 pedalboard==0.7.4
 prefigure==0.0.9
 pytorch_lightning==2.1.0
 PyWavelets==1.4.1
 safetensors
 sentencepiece==0.1.99
```

