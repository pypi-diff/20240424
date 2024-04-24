# Comparing `tmp/soft-moe-pytorch-0.1.7.tar.gz` & `tmp/soft_moe_pytorch-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soft-moe-pytorch-0.1.7.tar", last modified: Thu Feb 29 15:34:22 2024, max compression
+gzip compressed data, was "soft_moe_pytorch-0.1.8.tar", last modified: Wed Apr 24 15:24:24 2024, max compression
```

## Comparing `soft-moe-pytorch-0.1.7.tar` & `soft_moe_pytorch-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:34:22.535491 soft-moe-pytorch-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-29 15:34:13.000000 soft-moe-pytorch-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-02-29 15:34:22.535491 soft-moe-pytorch-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-02-29 15:34:13.000000 soft-moe-pytorch-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 15:34:22.535491 soft-moe-pytorch-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-02-29 15:34:13.000000 soft-moe-pytorch-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:34:22.531491 soft-moe-pytorch-0.1.7/soft_moe_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-29 15:34:13.000000 soft-moe-pytorch-0.1.7/soft_moe_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-02-29 15:34:13.000000 soft-moe-pytorch-0.1.7/soft_moe_pytorch/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-02-29 15:34:13.000000 soft-moe-pytorch-0.1.7/soft_moe_pytorch/soft_moe.py
--rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-02-29 15:34:13.000000 soft-moe-pytorch-0.1.7/soft_moe_pytorch/soft_moe_with_dynamic_slots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:34:22.535491 soft-moe-pytorch-0.1.7/soft_moe_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-02-29 15:34:22.000000 soft-moe-pytorch-0.1.7/soft_moe_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-29 15:34:22.000000 soft-moe-pytorch-0.1.7/soft_moe_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 15:34:22.000000 soft-moe-pytorch-0.1.7/soft_moe_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-29 15:34:22.000000 soft-moe-pytorch-0.1.7/soft_moe_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 15:34:22.000000 soft-moe-pytorch-0.1.7/soft_moe_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:24:24.528495 soft_moe_pytorch-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-24 15:24:16.000000 soft_moe_pytorch-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-24 15:24:24.528495 soft_moe_pytorch-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-24 15:24:16.000000 soft_moe_pytorch-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:24:24.528495 soft_moe_pytorch-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-24 15:24:16.000000 soft_moe_pytorch-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:24:24.528495 soft_moe_pytorch-0.1.8/soft_moe_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-24 15:24:16.000000 soft_moe_pytorch-0.1.8/soft_moe_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-24 15:24:16.000000 soft_moe_pytorch-0.1.8/soft_moe_pytorch/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10962 2024-04-24 15:24:16.000000 soft_moe_pytorch-0.1.8/soft_moe_pytorch/soft_moe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-04-24 15:24:16.000000 soft_moe_pytorch-0.1.8/soft_moe_pytorch/soft_moe_with_dynamic_slots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:24:24.528495 soft_moe_pytorch-0.1.8/soft_moe_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-24 15:24:24.000000 soft_moe_pytorch-0.1.8/soft_moe_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-24 15:24:24.000000 soft_moe_pytorch-0.1.8/soft_moe_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:24:24.000000 soft_moe_pytorch-0.1.8/soft_moe_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 15:24:24.000000 soft_moe_pytorch-0.1.8/soft_moe_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 15:24:24.000000 soft_moe_pytorch-0.1.8/soft_moe_pytorch.egg-info/top_level.txt
```

### Comparing `soft-moe-pytorch-0.1.7/LICENSE` & `soft_moe_pytorch-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `soft-moe-pytorch-0.1.7/PKG-INFO` & `soft_moe_pytorch-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soft-moe-pytorch
-Version: 0.1.7
+Version: 0.1.8
 Summary: Soft MoE - Pytorch
 Home-page: https://github.com/lucidrains/soft-moe-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,mixture of experts
 Classifier: Development Status :: 4 - Beta
```

### Comparing `soft-moe-pytorch-0.1.7/README.md` & `soft_moe_pytorch-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `soft-moe-pytorch-0.1.7/setup.py` & `soft_moe_pytorch-0.1.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'soft-moe-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.1.7',
+  version = '0.1.8',
   license='MIT',
   description = 'Soft MoE - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/soft-moe-pytorch',
   keywords = [
```

### Comparing `soft-moe-pytorch-0.1.7/soft_moe_pytorch/distributed.py` & `soft_moe_pytorch-0.1.8/soft_moe_pytorch/distributed.py`

 * *Files identical despite different names*

### Comparing `soft-moe-pytorch-0.1.7/soft_moe_pytorch/soft_moe.py` & `soft_moe_pytorch-0.1.8/soft_moe_pytorch/soft_moe.py`

 * *Files 4% similar despite different names*

```diff
@@ -285,15 +285,18 @@
         is_distributed = None,
         offload_unused_experts_to_cpu = True,
         use_layernorm = False
     ):
         super().__init__()
         assert exists(seq_len) ^ exists(num_slots), 'either seq_len, or num_slots must be passed into SoftMoE'
 
-        num_slots = default(num_slots, seq_len // num_experts)
+        if exists(seq_len):
+            num_slots = default(num_slots, seq_len // num_experts)
+        elif exists(num_slots):
+            seq_len = num_slots * num_experts
 
         norm_klass = LayerNorm if use_layernorm else RMSNorm
         self.norm = norm_klass(dim)
 
         self.slot_norm = norm_klass(dim)
         self.slot_embeds = nn.Parameter(torch.randn(num_experts, num_slots, dim))
```

### Comparing `soft-moe-pytorch-0.1.7/soft_moe_pytorch/soft_moe_with_dynamic_slots.py` & `soft_moe_pytorch-0.1.8/soft_moe_pytorch/soft_moe_with_dynamic_slots.py`

 * *Files identical despite different names*

### Comparing `soft-moe-pytorch-0.1.7/soft_moe_pytorch.egg-info/PKG-INFO` & `soft_moe_pytorch-0.1.8/soft_moe_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soft-moe-pytorch
-Version: 0.1.7
+Version: 0.1.8
 Summary: Soft MoE - Pytorch
 Home-page: https://github.com/lucidrains/soft-moe-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,mixture of experts
 Classifier: Development Status :: 4 - Beta
```

