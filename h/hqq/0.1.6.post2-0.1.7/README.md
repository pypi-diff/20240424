# Comparing `tmp/hqq-0.1.6.post2.tar.gz` & `tmp/hqq-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hqq-0.1.6.post2.tar", last modified: Tue Mar 19 18:15:23 2024, max compression
+gzip compressed data, was "hqq-0.1.7.tar", last modified: Wed Apr 24 08:56:07 2024, max compression
```

## Comparing `hqq-0.1.6.post2.tar` & `hqq-0.1.7.tar`

### file list

```diff
@@ -1,54 +1,63 @@
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-03-19 18:15:23.303822 hqq-0.1.6.post2/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    11360 2023-12-02 17:25:57.000000 hqq-0.1.6.post2/LICENSE
--rw-r--r--   0 hicham    (1009) hicham    (1009)      436 2024-03-19 18:15:23.303822 hqq-0.1.6.post2/PKG-INFO
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-03-19 18:15:23.299822 hqq-0.1.6.post2/hqq/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)       93 2024-03-19 18:15:00.000000 hqq-0.1.6.post2/hqq/__init__.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-03-19 18:15:23.299822 hqq-0.1.6.post2/hqq/core/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-01 10:59:22.000000 hqq-0.1.6.post2/hqq/core/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     8299 2024-03-15 08:58:01.000000 hqq-0.1.6.post2/hqq/core/bitpack.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     9102 2024-03-18 11:04:14.000000 hqq-0.1.6.post2/hqq/core/optimize.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    17172 2024-03-18 15:34:02.000000 hqq-0.1.6.post2/hqq/core/peft.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    28645 2024-03-19 12:54:05.000000 hqq-0.1.6.post2/hqq/core/quantize.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)      639 2024-03-15 08:58:01.000000 hqq-0.1.6.post2/hqq/core/utils.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-03-19 18:15:23.303822 hqq-0.1.6.post2/hqq/engine/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.6.post2/hqq/engine/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3036 2024-03-15 12:03:48.000000 hqq-0.1.6.post2/hqq/engine/base.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2568 2024-03-15 09:12:21.000000 hqq-0.1.6.post2/hqq/engine/hf.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2458 2024-03-15 09:09:35.000000 hqq-0.1.6.post2/hqq/engine/timm.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     5287 2024-03-15 12:03:22.000000 hqq-0.1.6.post2/hqq/engine/vllm.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-03-19 18:15:23.303822 hqq-0.1.6.post2/hqq/kernels/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)       87 2024-03-15 10:04:14.000000 hqq-0.1.6.post2/hqq/kernels/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2670 2024-03-19 10:48:12.000000 hqq-0.1.6.post2/hqq/kernels/hqq_aten_cuda.cpp
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    17843 2024-03-19 10:48:11.000000 hqq-0.1.6.post2/hqq/kernels/hqq_aten_cuda_kernel.cu
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3412 2024-02-21 11:27:07.000000 hqq-0.1.6.post2/hqq/kernels/hqq_aten_torch.cpp
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)      494 2024-03-19 10:48:06.000000 hqq-0.1.6.post2/hqq/kernels/setup_cuda.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)      292 2024-03-14 16:26:18.000000 hqq-0.1.6.post2/hqq/kernels/setup_torch.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-03-19 18:15:23.303822 hqq-0.1.6.post2/hqq/models/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-01 10:59:32.000000 hqq-0.1.6.post2/hqq/models/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    12537 2024-03-18 15:33:23.000000 hqq-0.1.6.post2/hqq/models/base.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-03-19 18:15:23.303822 hqq-0.1.6.post2/hqq/models/hf/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.6.post2/hqq/models/hf/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     1057 2024-03-14 15:51:30.000000 hqq-0.1.6.post2/hqq/models/hf/base.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2703 2024-03-14 15:51:30.000000 hqq-0.1.6.post2/hqq/models/hf/llama.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2703 2024-03-14 15:51:30.000000 hqq-0.1.6.post2/hqq/models/hf/mistral.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3464 2024-03-14 15:51:30.000000 hqq-0.1.6.post2/hqq/models/hf/mixtral.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2487 2024-03-14 15:51:30.000000 hqq-0.1.6.post2/hqq/models/hf/phi.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2361 2024-03-14 15:51:30.000000 hqq-0.1.6.post2/hqq/models/hf/phi_opt.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-03-19 18:15:23.303822 hqq-0.1.6.post2/hqq/models/timm/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.6.post2/hqq/models/timm/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)      750 2024-03-14 15:52:37.000000 hqq-0.1.6.post2/hqq/models/timm/base.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2815 2024-03-14 15:53:15.000000 hqq-0.1.6.post2/hqq/models/timm/vit_clip.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-03-19 18:15:23.303822 hqq-0.1.6.post2/hqq/models/vllm/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.6.post2/hqq/models/vllm/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     6114 2024-03-15 12:07:03.000000 hqq-0.1.6.post2/hqq/models/vllm/base.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    16480 2024-03-14 15:55:27.000000 hqq-0.1.6.post2/hqq/models/vllm/llama.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-03-19 18:15:23.299822 hqq-0.1.6.post2/hqq.egg-info/
--rw-r--r--   0 hicham    (1009) hicham    (1009)      436 2024-03-19 18:15:18.000000 hqq-0.1.6.post2/hqq.egg-info/PKG-INFO
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)      944 2024-03-19 18:15:18.000000 hqq-0.1.6.post2/hqq.egg-info/SOURCES.txt
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        1 2024-03-19 18:15:18.000000 hqq-0.1.6.post2/hqq.egg-info/dependency_links.txt
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)       90 2024-03-19 18:15:18.000000 hqq-0.1.6.post2/hqq.egg-info/requires.txt
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        4 2024-03-19 18:15:18.000000 hqq-0.1.6.post2/hqq.egg-info/top_level.txt
--rw-rw-r--   0 hicham    (1009) hicham    (1009)       38 2024-03-19 18:15:23.303822 hqq-0.1.6.post2/setup.cfg
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     1577 2024-03-19 18:14:57.000000 hqq-0.1.6.post2/setup.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-03-19 18:15:23.303822 hqq-0.1.6.post2/tests/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    11302 2024-03-01 10:40:44.000000 hqq-0.1.6.post2/tests/test_quantize.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.294434 hqq-0.1.7/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    11360 2023-12-02 17:25:57.000000 hqq-0.1.7/LICENSE
+-rw-r--r--   0 hicham    (1009) hicham    (1009)      432 2024-04-24 08:56:07.294434 hqq-0.1.7/PKG-INFO
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.270433 hqq-0.1.7/hqq/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)       87 2024-04-16 08:24:14.000000 hqq-0.1.7/hqq/__init__.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.270433 hqq-0.1.7/hqq/backends/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2024-04-16 10:04:12.000000 hqq-0.1.7/hqq/backends/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3228 2024-04-19 12:02:43.000000 hqq-0.1.7/hqq/backends/marlin.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    10514 2024-04-24 08:49:06.000000 hqq-0.1.7/hqq/backends/torchao.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.274433 hqq-0.1.7/hqq/core/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-01 10:59:22.000000 hqq-0.1.7/hqq/core/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     5195 2024-04-10 14:29:15.000000 hqq-0.1.7/hqq/core/bitpack.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    14118 2024-04-16 18:00:28.000000 hqq-0.1.7/hqq/core/optimize.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    17172 2024-03-18 15:34:02.000000 hqq-0.1.7/hqq/core/peft.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    28563 2024-04-16 17:51:09.000000 hqq-0.1.7/hqq/core/quantize.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)      639 2024-03-15 08:58:01.000000 hqq-0.1.7/hqq/core/utils.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.278433 hqq-0.1.7/hqq/engine/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7/hqq/engine/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3131 2024-03-25 11:05:14.000000 hqq-0.1.7/hqq/engine/base.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2568 2024-03-15 09:12:21.000000 hqq-0.1.7/hqq/engine/hf.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2458 2024-03-15 09:09:35.000000 hqq-0.1.7/hqq/engine/timm.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     5287 2024-03-15 12:03:22.000000 hqq-0.1.7/hqq/engine/vllm.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.278433 hqq-0.1.7/hqq/kernels/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)       87 2024-03-15 10:04:14.000000 hqq-0.1.7/hqq/kernels/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2670 2024-03-25 10:15:39.000000 hqq-0.1.7/hqq/kernels/hqq_aten_cuda.cpp
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    17933 2024-04-08 11:30:33.000000 hqq-0.1.7/hqq/kernels/hqq_aten_cuda_kernel.cu
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3412 2024-02-21 11:27:07.000000 hqq-0.1.7/hqq/kernels/hqq_aten_torch.cpp
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)      494 2024-03-19 10:48:06.000000 hqq-0.1.7/hqq/kernels/setup_cuda.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)      292 2024-03-14 16:26:18.000000 hqq-0.1.7/hqq/kernels/setup_torch.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.278433 hqq-0.1.7/hqq/models/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-01 10:59:32.000000 hqq-0.1.7/hqq/models/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    17314 2024-04-22 18:40:37.000000 hqq-0.1.7/hqq/models/base.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.282434 hqq-0.1.7/hqq/models/hf/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7/hqq/models/hf/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     1057 2024-03-14 15:51:30.000000 hqq-0.1.7/hqq/models/hf/base.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2703 2024-03-14 15:51:30.000000 hqq-0.1.7/hqq/models/hf/llama.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2703 2024-03-14 15:51:30.000000 hqq-0.1.7/hqq/models/hf/mistral.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3464 2024-03-14 15:51:30.000000 hqq-0.1.7/hqq/models/hf/mixtral.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2487 2024-03-14 15:51:30.000000 hqq-0.1.7/hqq/models/hf/phi.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2361 2024-03-14 15:51:30.000000 hqq-0.1.7/hqq/models/hf/phi_opt.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.282434 hqq-0.1.7/hqq/models/timm/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7/hqq/models/timm/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)      750 2024-03-14 15:52:37.000000 hqq-0.1.7/hqq/models/timm/base.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2815 2024-03-14 15:53:15.000000 hqq-0.1.7/hqq/models/timm/vit_clip.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.290434 hqq-0.1.7/hqq/models/vllm/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7/hqq/models/vllm/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     6114 2024-03-15 12:07:03.000000 hqq-0.1.7/hqq/models/vllm/base.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    16480 2024-03-14 15:55:27.000000 hqq-0.1.7/hqq/models/vllm/llama.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.290434 hqq-0.1.7/hqq/utils/
+-rw-rw-r--   0 hicham    (1009) hicham    (1009)        0 2024-04-16 10:04:22.000000 hqq-0.1.7/hqq/utils/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    10844 2024-04-23 16:50:10.000000 hqq-0.1.7/hqq/utils/generation_hf.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     6066 2024-04-22 17:00:27.000000 hqq-0.1.7/hqq/utils/patching.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.270433 hqq-0.1.7/hqq.egg-info/
+-rw-r--r--   0 hicham    (1009) hicham    (1009)      432 2024-04-24 08:54:01.000000 hqq-0.1.7/hqq.egg-info/PKG-INFO
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     1109 2024-04-24 08:54:01.000000 hqq-0.1.7/hqq.egg-info/SOURCES.txt
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        1 2024-04-24 08:54:01.000000 hqq-0.1.7/hqq.egg-info/dependency_links.txt
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)       92 2024-04-24 08:54:01.000000 hqq-0.1.7/hqq.egg-info/requires.txt
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        4 2024-04-24 08:54:01.000000 hqq-0.1.7/hqq.egg-info/top_level.txt
+-rw-rw-r--   0 hicham    (1009) hicham    (1009)       38 2024-04-24 08:56:07.294434 hqq-0.1.7/setup.cfg
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     1700 2024-04-16 09:50:06.000000 hqq-0.1.7/setup.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-04-24 08:56:07.290434 hqq-0.1.7/tests/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3689 2024-03-25 10:44:50.000000 hqq-0.1.7/tests/test_bitpack.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    11302 2024-03-01 10:40:44.000000 hqq-0.1.7/tests/test_quantize.py
```

### Comparing `hqq-0.1.6.post2/LICENSE` & `hqq-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hqq-0.1.6.post2/hqq/core/peft.py` & `hqq-0.1.7/hqq/core/peft.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.6.post2/hqq/core/quantize.py` & `hqq-0.1.7/hqq/core/quantize.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,29 +105,24 @@
 
         # Round zero as in: https://github.com/casper-hansen/AutoAWQ/blob/main/awq/quantize/quantizer.py#L42C9-L42C14
         if round_zero:
             zero = torch.round(zero)
 
         # Fine-tune weights
         if optimize:
-            scale, zero = Quantizer.optimize_weights(
+            W_q, scale, zero = Quantizer.optimize_weights(
                 tensor=W,
                 scale=scale,
                 zero=zero,
                 min_max=min_max,
                 axis=axis,
                 device=device,
             )
-
-        # Quantize
-        scale, zero = (
-            scale.clone(),
-            zero.clone(),
-        )  # Necessary for fake quantization backprop
-        W_q = torch.round(W * scale + zero).clamp(min_max[0], min_max[1])
+        else:
+            W_q = torch.round(W * scale + zero).clamp(min_max[0], min_max[1])
 
         # Store meta-data (we invert the scale for dequantization)
         meta = {
             "nbits": nbits,
             "group_size": group_size,
             "shape": shape,
             "scale": 1.0 / scale,
@@ -158,15 +153,15 @@
     # Main dequantization: bit_unpacking > (W_q - z)*s > reshape
     @classmethod
     def dequantize(cls, W_q: Tensor, meta: dict) -> Tensor:
         compute_dtype = meta["compute_dtype"] if ("compute_dtype" in meta) else float16
         if meta["packing"]:
             if meta["view_as_float"]:
                 W_q = W_q.view(meta["unpack_view_dtype"])
-            W_r = Quantizer.unpack[meta["packing"]](W_q).to(compute_dtype)
+            W_r = Quantizer.unpack[meta["packing"]](W_q, dtype=compute_dtype)
             if (meta["group_size"] is not None) and (meta["nbits"] == 3):
                 W_r = (
                     W_r[: meta["group_size"]]
                     if (meta["axis"] == 0)
                     else W_r[:, : meta["group_size"]]
                 )
         else:
@@ -276,15 +271,15 @@
         grad_input = grad_weight = grad_bias = None
 
         if ctx.needs_input_grad[0]:
             grad_input = torch.matmul(grad_output, ctx.dequantize())
 
         # weight grad for frozen quantized weights not defined
         # if ctx.needs_input_grad[1]:
-        # 	grad_weight = torch.matmul(grad_output.t(), x)
+        #   grad_weight = torch.matmul(grad_output.t(), x)
 
         if bias is not None and ctx.needs_input_grad[2]:
             grad_bias = grad_output.sum(0)
 
         return grad_input, grad_weight, grad_bias
 
 
@@ -309,15 +304,15 @@
         grad_input = grad_weight = grad_bias = None
 
         if ctx.needs_input_grad[0]:
             grad_input = ctx.matmul(grad_output, transpose=False)
 
         # weight grad for frozen quantized weights not defined
         # if ctx.needs_input_grad[1]:
-        # 	grad_weight = torch.matmul(grad_output.t(), x)
+        #   grad_weight = torch.matmul(grad_output.t(), x)
 
         if bias is not None and ctx.needs_input_grad[2]:
             grad_bias = grad_output.sum(0)
 
         return grad_input, grad_weight, grad_bias
 
 
@@ -817,28 +812,30 @@
 def hqq_base_quant_config(
     nbits: int = 4,
     group_size: int = 64,
     quant_zero: bool = True,
     quant_scale: bool = False,
     offload_meta: bool = False,  # meta-data should be quantized with the same settings to use offload_meta
     view_as_float: bool = False,
+    axis: int = 0,
 ):
     assert (
         nbits in Quantizer.SUPPORTED_BITS
     ), "nbits value not supported. Check Quantizer.SUPPORTED_BITS."
     if group_size is not None:
         assert is_divisible(
             group_size, 8
         ), "Invalid group_size param: the value should be a multiple of 8."
     weight_quant_params = {
         "nbits": nbits,
         "channel_wise": True,
         "group_size": group_size,
         "optimize": True,
         "round_zero": True if nbits == 4 else False,
+        "axis": axis,
         "view_as_float": view_as_float,
     }
 
     if offload_meta:
         if quant_scale != quant_zero:
             # print(colored("quant_zero and quant_scale must be the same when offload_meta is set to True. Setting quant_scale=quant_zero." , 'yellow'))
             quant_scale = quant_zero
```

### Comparing `hqq-0.1.6.post2/hqq/core/utils.py` & `hqq-0.1.7/hqq/core/utils.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.6.post2/hqq/engine/base.py` & `hqq-0.1.7/hqq/engine/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -72,22 +72,27 @@
     @classmethod
     def from_quantized(
         cls,
         save_dir_or_hub,
         compute_dtype: torch.dtype = float16,
         device="cuda",
         cache_dir: str = "",
+        adapter: str = None,
     ):
         # Both local and hub-support
         save_dir = BaseHQQModel.try_snapshot_download(save_dir_or_hub)
         arch_key = cls._get_arch_key_from_save_dir(save_dir)
         cls._check_arch_support(arch_key)
 
         model = cls._get_hqq_class(arch_key).from_quantized(
-            save_dir, compute_dtype=compute_dtype, device=device, cache_dir=cache_dir
+            save_dir,
+            compute_dtype=compute_dtype,
+            device=device,
+            cache_dir=cache_dir,
+            adapter=adapter,
         )
 
         cls._make_quantizable(model, quantized=True)
         return model
 
     @classmethod
     def get_linear_tags(cls, model):
```

### Comparing `hqq-0.1.6.post2/hqq/engine/hf.py` & `hqq-0.1.7/hqq/engine/hf.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.6.post2/hqq/engine/timm.py` & `hqq-0.1.7/hqq/engine/timm.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.6.post2/hqq/engine/vllm.py` & `hqq-0.1.7/hqq/engine/vllm.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.6.post2/hqq/kernels/hqq_aten_cuda.cpp` & `hqq-0.1.7/hqq/kernels/hqq_aten_cuda.cpp`

 * *Files identical despite different names*

### Comparing `hqq-0.1.6.post2/hqq/kernels/hqq_aten_cuda_kernel.cu` & `hqq-0.1.7/hqq/kernels/hqq_aten_cuda_kernel.cu`

 * *Files 0% similar despite different names*

```diff
@@ -404,15 +404,17 @@
 	CHECK_INPUT(Wq_packed);
 
 	int r = 10; //number of elements packed
 	int h = Wq_packed.size(0);
 	int w = Wq_packed.size(1);
 	int n = h*w; //num rows as a packed tensor
 
-	auto Wq_unpacked = torch::empty({h*r, w}, Wq_packed.options()); 
+	auto dev   = Wq_packed.device();
+	auto dtype = torch::kByte;
+	auto Wq_unpacked = torch::empty({r*h, w}, torch::TensorOptions().dtype(dtype).device(dev)); 
 
 	int blocks = cdiv(n, BLOCK_SIZE);
 	unpack_3bit_32_kernel<<<blocks, BLOCK_SIZE>>>(Wq_packed.data_ptr<int32_t>(), Wq_unpacked.data_ptr<unsigned char>(), n);	
 
 	C10_CUDA_KERNEL_LAUNCH_CHECK();
 	//cudaDeviceSynchronize();
```

### Comparing `hqq-0.1.6.post2/hqq/kernels/hqq_aten_torch.cpp` & `hqq-0.1.7/hqq/kernels/hqq_aten_torch.cpp`

 * *Files identical despite different names*

### Comparing `hqq-0.1.6.post2/hqq/models/base.py` & `hqq-0.1.7/hqq/models/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Written by Dr. Hicham Badri @Mobius Labs GmbH - 2023
 #####################################################
+import os
+import gc
 import torch
 from torch import nn
 from torch import float16
-import gc
-import os
 from os.path import join as pjoin
 from typing import Callable
 from tqdm import tqdm
 from abc import abstractmethod
+from functools import partial
 
 from huggingface_hub import snapshot_download
 from ..core.quantize import HQQLinear
+from ..core.peft import PeftUtils
 
 # Defined what is qualified as "linear layer"
 _QUANT_LAYERS = [nn.Linear]
 _IGNORE_LINEAR = ["lm_head"]
 
 
 # Cleanup GPU vram
@@ -45,23 +47,48 @@
             n
             for n in name.split(".")
             if ((n not in ["model", "layers"]) and (not n.isnumeric()))
         ]
     )
 
 
+# returns all children nodes from model
+def get_all_children_from_model(model, ignore: list = []) -> list:
+    tags = []
+    for name, module in model.named_modules():
+        if is_leaf_module(module) and (name.split(".")[-1] not in ignore):
+            tags.append(name)
+    return tags
+
+
 # Get all linear tags available
 def get_linear_tags_from_model(model, ignore: list) -> list:
     linear_tags = set()
     for name, module in model.named_modules():
         if (type(module) in _QUANT_LAYERS) and (name.split(".")[-1] not in ignore):
             linear_tags.add(name_to_linear_tag(name))
     return list(linear_tags)
 
 
+def forward_device_hooked(self, *args, **kwargs):
+    args = list(args)
+
+    #eddit this to make torch.compile compatible
+    for i in range(len(args)):
+        if(isinstance(args[i], (torch.Tensor, torch.nn.Parameter))):#if hasattr(args[i], "to"):
+            args[i] = args[i].to(self.device)
+
+    for i in kwargs:
+        if(isinstance(kwargs[i], (torch.Tensor, torch.nn.Parameter))):#if hasattr(kwargs[i], "to"):
+            kwargs[i] = kwargs[i].to(self.device)
+
+    # return self.__class__.forward(self, *args, **kwargs)
+    return self.forward_orig(*args, **kwargs)
+
+
 # Base patching class. Patching defines how nn.Linear and other layers are replaced via a patching function.
 class BasePatch:
     # Override these OR override the main patch_model() function
     ############################################
     # This method iterates through layers of the model that are NOT nn.Linear and processes them via new_nodule = patch_fct(module, params)
     @classmethod
     def patch_nonlinearlayers(
@@ -196,51 +223,130 @@
     # Main function to quantize a model. Basically goes through the linear layers specfied in the patching function and replaces them with HQQLinear
     @classmethod
     def quantize_model(
         cls,
         model,
         quant_config: dict,
         compute_dtype: torch.dtype = float16,
-        device="cuda",
+        device: str | list | dict = "cuda",
     ):
         # Set linear tags automatically
+        cls.autoname_modules(model)
         cls.set_auto_linear_tags(model)
 
         # Use the same quantization config for all linear layers. Use None to skip quantizing a specfic layer.
         if True in [(key in cls.get_linear_tags()) for key in quant_config.keys()]:
             # If the user doesn't specify a key from get_linear_tags, the layer is not quantized via (key, None)
             patch_params = {key: None for key in cls.get_linear_tags()}
             patch_params.update(quant_config)
         else:
             # Same quant_config for all layers
             patch_params = {k: quant_config for k in cls.get_linear_tags()}
 
+        # Get list of all nodes in order
+        all_nodes = get_all_children_from_model(model, [])  # ordered nodes
+        try:
+            # Extract block names: This is following Hugging Face models.
+            num_blocks = (
+                len(model.model.layers)
+                if hasattr(model, "model")
+                else len(model.layers)
+            )
+            all_blocks = ["model.layers." + str(i) for i in range(num_blocks)]
+        except Exception:
+            all_blocks = None
+            print(
+                "Default model structure not supported. Make sure you feed device as dictionary as {name_block: device}"
+            )
+
+        if isinstance(
+            device, dict
+        ):  # input as {module block name (str): device (str | torch.device)}
+            device_map = device
+            num_devices = len(set([device_map[k] for k in device_map]))
+            all_blocks = list(device_map.keys())
+
+        node_to_block = {}
+        for node in all_nodes:
+            res = [block for block in all_blocks if (block in node)]
+            node_to_block[node] = res[-1] if (len(res) > 0) else node
+
+        # Set device-map
+        if isinstance(device, str):  # single device as str
+            device_map = {k: device for k in all_blocks + all_nodes}
+            num_devices = 1
+
+        if isinstance(device, list):  # list of devices
+            num_devices = len(device)
+            device_map = {}
+            for node in all_nodes:
+                if ".layers" in node:
+                    break
+                device_map[node] = device[0]
+
+            for node in all_nodes[::-1]:
+                if ".layers" in node:
+                    break
+                device_map[node] = device[-1]
+
+            step, k = len(all_blocks) // num_devices, 0
+            for i in range(0, len(all_blocks), step):
+                for j in range(i, i + step):
+                    device_map[all_blocks[min(j, len(all_blocks) - 1)]] = device[
+                        min(k, num_devices - 1)
+                    ]
+                k += 1
+
+        # Map nodes to block devices
+        for node in all_nodes:
+            device_map[node] = device_map[node_to_block[node]]
+
         # We replace the nn.Linear layers with HQQLinear
         def _patch_linear(linear_layer, quant_config):
+            current_device = device_map[linear_layer.name]
+
             if quant_config is not None:
                 out_module = HQQLinear(
                     linear_layer,
                     quant_config,
                     compute_dtype=compute_dtype,
-                    device=device,
+                    device=current_device,
                 )
             else:
-                out_module = linear_layer.to(
-                    device=device, dtype=compute_dtype, non_blocking=True
-                )
+                out_module = linear_layer.to(device=current_device, dtype=compute_dtype)
+
+            out_module.device = current_device
             return out_module
 
-        cls.patch_model(
-            model,
-            lambda layer: layer.to(
-                device=device, dtype=compute_dtype, non_blocking=True
-            ),
-            _patch_linear,
-            patch_params,
-        )
+        def _patch_other(layer):
+            current_device = device_map[layer.name]
+            layer.device = current_device
+            return layer.to(device=current_device, dtype=compute_dtype)
+
+        cls.patch_model(model, _patch_other, _patch_linear, patch_params)
+
+        # Insert device switcher
+        if num_devices > 1:
+            core_model = model if hasattr(model, "layers") else model.model
+
+            # Make sure the input (first node) has the input in the right device during generation
+            input_node_child_name = all_nodes[0].split(".")[-1]
+            input_node = getattr(core_model, input_node_child_name)
+            input_node.device = device_map[all_nodes[0]]
+            input_node.forward_orig = input_node.forward
+            input_node.forward = partial(forward_device_hooked, input_node)
+            setattr(core_model, input_node_child_name, input_node)
+
+            # Make sure all inputs to the blocks are in the right device
+            for i in range(len(core_model.layers)):
+                core_model.layers[i].device = device_map[core_model.layers[i].name]
+                core_model.layers[i].forward_orig = core_model.layers[i].forward
+                core_model.layers[i].forward = partial(
+                    forward_device_hooked, core_model.layers[i]
+                )
 
         # Set base class
         model.base_class = cls
 
         # Sync
         torch.cuda.synchronize()
 
@@ -301,21 +407,25 @@
     @classmethod
     def from_quantized(
         cls,
         save_dir_or_hub,
         compute_dtype: torch.dtype = float16,
         device="cuda",
         cache_dir: str = "",
+        adapter: str = None,
     ):
         # Get directory path
         save_dir = cls.try_snapshot_download(save_dir_or_hub, cache_dir)
 
         # Load model from config
         model = cls.create_model(save_dir)
 
+        # Track save directory
+        model.save_dir = save_dir
+
         # Name the layers
         cls.autoname_modules(model)
 
         # Set linear tags automatically
         cls.set_auto_linear_tags(model)
 
         # Load weights
@@ -362,11 +472,19 @@
 
         # Load other weights that are not part of any module
         cls.post_module_load(model, weights)
 
         # Set base class
         model.base_class = cls
 
+        # Add adapter
+        if adapter is not None:
+            try:
+                PeftUtils.load_lora_weights(model, filename=pjoin(save_dir, adapter))
+                PeftUtils.cast_lora_weights(model, dtype=compute_dtype)
+            except Exception as e:
+                print("Skipping adapter loading...", str(e))
+
         # Sync
         torch.cuda.synchronize()
 
         return model
```

### Comparing `hqq-0.1.6.post2/hqq/models/hf/base.py` & `hqq-0.1.7/hqq/models/hf/base.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.6.post2/hqq/models/hf/llama.py` & `hqq-0.1.7/hqq/models/hf/llama.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.6.post2/hqq/models/hf/mistral.py` & `hqq-0.1.7/hqq/models/hf/mistral.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.6.post2/hqq/models/hf/mixtral.py` & `hqq-0.1.7/hqq/models/hf/mixtral.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.6.post2/hqq/models/hf/phi.py` & `hqq-0.1.7/hqq/models/hf/phi.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.6.post2/hqq/models/hf/phi_opt.py` & `hqq-0.1.7/hqq/models/hf/phi_opt.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.6.post2/hqq/models/timm/base.py` & `hqq-0.1.7/hqq/models/timm/base.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.6.post2/hqq/models/timm/vit_clip.py` & `hqq-0.1.7/hqq/models/timm/vit_clip.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.6.post2/hqq/models/vllm/base.py` & `hqq-0.1.7/hqq/models/vllm/base.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.6.post2/hqq/models/vllm/llama.py` & `hqq-0.1.7/hqq/models/vllm/llama.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.6.post2/setup.py` & `hqq-0.1.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Written by Dr. Hicham Badri @Mobius Labs GmbH - 2023
+#####################################################
+
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from setuptools.command.develop import develop
 from setuptools.command.egg_info import egg_info
 import os
 
 
@@ -36,15 +39,15 @@
     def run(self):
         egg_info.run(self)
         run_setup_cuda()
 
 
 setup(
     name="hqq",
-    version="0.1.6.post2",
+    version="0.1.7",
     description="Half-Quadratic Quantization (HQQ)",
     url="https://github.com/mobiusml/hqq/",
     author="Dr. Hicham Badri",
     author_email="hicham@mobiuslabs.com",
     license="Apache 2",
     packages=find_packages(include=["hqq", "hqq.*"]),
     package_data={
@@ -55,14 +58,15 @@
         "install": InstallCommand,
         "develop": DevelopCommand,
         "egg_info": EgginfoCommand,
     },
     install_requires=[
         "numpy>=1.24.4",
         "tqdm>=4.64.1",
-        "huggingface_hub",
+        "einops",
         "accelerate",
-        "timm",
         "transformers>=4.36.1",
+        "huggingface_hub",
         "termcolor",
+        #"timm",
     ],
 )
```

### Comparing `hqq-0.1.6.post2/tests/test_quantize.py` & `hqq-0.1.7/tests/test_quantize.py`

 * *Files identical despite different names*

