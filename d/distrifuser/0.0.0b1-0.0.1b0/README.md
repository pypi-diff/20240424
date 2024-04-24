# Comparing `tmp/distrifuser-0.0.0b1.tar.gz` & `tmp/distrifuser-0.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distrifuser-0.0.0b1.tar", last modified: Tue Mar  5 21:49:24 2024, max compression
+gzip compressed data, was "distrifuser-0.0.1b0.tar", last modified: Wed Apr 24 19:29:10 2024, max compression
```

## Comparing `distrifuser-0.0.0b1.tar` & `distrifuser-0.0.1b0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-03-05 21:49:24.855883 distrifuser-0.0.0b1/
--rw-r--r--   0 lmxyy      (501) staff       (20)     1068 2024-02-28 21:20:49.000000 distrifuser-0.0.0b1/LICENSE.txt
--rw-r--r--   0 lmxyy      (501) staff       (20)    10481 2024-03-05 21:49:24.855533 distrifuser-0.0.0b1/PKG-INFO
--rw-r--r--   0 lmxyy      (501) staff       (20)     9934 2024-03-05 21:48:45.000000 distrifuser-0.0.0b1/README.md
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-03-05 21:49:24.849768 distrifuser-0.0.0b1/distrifuser/
--rw-r--r--   0 lmxyy      (501) staff       (20)        0 2023-12-12 16:42:09.000000 distrifuser-0.0.0b1/distrifuser/__init__.py
--rw-r--r--   0 lmxyy      (501) staff       (20)       27 2024-03-05 21:48:21.000000 distrifuser-0.0.0b1/distrifuser/__version__.py
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-03-05 21:49:24.852086 distrifuser-0.0.0b1/distrifuser/models/
--rw-r--r--   0 lmxyy      (501) staff       (20)        0 2024-02-04 21:34:52.000000 distrifuser-0.0.0b1/distrifuser/models/__init__.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     1774 2024-02-06 06:15:38.000000 distrifuser-0.0.0b1/distrifuser/models/base_model.py
--rw-r--r--   0 lmxyy      (501) staff       (20)    10770 2024-02-09 03:08:09.000000 distrifuser-0.0.0b1/distrifuser/models/distri_sdxl_unet_pp.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     9997 2024-02-14 07:07:48.000000 distrifuser-0.0.0b1/distrifuser/models/distri_sdxl_unet_tp.py
--rw-r--r--   0 lmxyy      (501) staff       (20)    10684 2024-02-07 23:00:18.000000 distrifuser-0.0.0b1/distrifuser/models/naive_patch_sdxl.py
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-03-05 21:49:24.852570 distrifuser-0.0.0b1/distrifuser/modules/
--rw-r--r--   0 lmxyy      (501) staff       (20)        0 2023-12-12 18:11:45.000000 distrifuser-0.0.0b1/distrifuser/modules/__init__.py
--rw-r--r--   0 lmxyy      (501) staff       (20)      670 2024-02-06 06:15:38.000000 distrifuser-0.0.0b1/distrifuser/modules/base_module.py
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-03-05 21:49:24.853652 distrifuser-0.0.0b1/distrifuser/modules/pp/
--rw-r--r--   0 lmxyy      (501) staff       (20)        0 2024-02-06 06:15:38.000000 distrifuser-0.0.0b1/distrifuser/modules/pp/__init__.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     7309 2024-02-28 17:20:17.000000 distrifuser-0.0.0b1/distrifuser/modules/pp/attn.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     5242 2024-02-14 05:29:38.000000 distrifuser-0.0.0b1/distrifuser/modules/pp/conv2d.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     4880 2024-02-28 20:53:36.000000 distrifuser-0.0.0b1/distrifuser/modules/pp/groupnorm.py
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-03-05 21:49:24.855147 distrifuser-0.0.0b1/distrifuser/modules/tp/
--rw-r--r--   0 lmxyy      (501) staff       (20)        0 2024-02-06 06:15:38.000000 distrifuser-0.0.0b1/distrifuser/modules/tp/__init__.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     7032 2024-02-14 06:26:15.000000 distrifuser-0.0.0b1/distrifuser/modules/tp/attention.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     2209 2024-02-14 06:26:15.000000 distrifuser-0.0.0b1/distrifuser/modules/tp/conv2d.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     3533 2024-02-14 06:26:15.000000 distrifuser-0.0.0b1/distrifuser/modules/tp/feed_forward.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     7627 2024-02-14 06:26:15.000000 distrifuser-0.0.0b1/distrifuser/modules/tp/resnet.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     6465 2024-03-05 21:46:29.000000 distrifuser-0.0.0b1/distrifuser/pipelines.py
--rw-r--r--   0 lmxyy      (501) staff       (20)     7172 2024-02-28 19:42:01.000000 distrifuser-0.0.0b1/distrifuser/utils.py
-drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-03-05 21:49:24.850754 distrifuser-0.0.0b1/distrifuser.egg-info/
--rw-r--r--   0 lmxyy      (501) staff       (20)    10481 2024-03-05 21:49:24.000000 distrifuser-0.0.0b1/distrifuser.egg-info/PKG-INFO
--rw-r--r--   0 lmxyy      (501) staff       (20)      866 2024-03-05 21:49:24.000000 distrifuser-0.0.0b1/distrifuser.egg-info/SOURCES.txt
--rw-r--r--   0 lmxyy      (501) staff       (20)        1 2024-03-05 21:49:24.000000 distrifuser-0.0.0b1/distrifuser.egg-info/dependency_links.txt
--rw-r--r--   0 lmxyy      (501) staff       (20)       47 2024-03-05 21:49:24.000000 distrifuser-0.0.0b1/distrifuser.egg-info/requires.txt
--rw-r--r--   0 lmxyy      (501) staff       (20)       12 2024-03-05 21:49:24.000000 distrifuser-0.0.0b1/distrifuser.egg-info/top_level.txt
--rw-r--r--   0 lmxyy      (501) staff       (20)       38 2024-03-05 21:49:24.855991 distrifuser-0.0.0b1/setup.cfg
--rw-r--r--   0 lmxyy      (501) staff       (20)     1079 2024-02-28 07:29:18.000000 distrifuser-0.0.0b1/setup.py
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-04-24 19:29:10.597840 distrifuser-0.0.1b0/
+-rw-r--r--   0 lmxyy      (501) staff       (20)     1068 2024-02-28 21:20:49.000000 distrifuser-0.0.1b0/LICENSE.txt
+-rw-r--r--   0 lmxyy      (501) staff       (20)    10759 2024-04-24 19:29:10.597610 distrifuser-0.0.1b0/PKG-INFO
+-rw-r--r--   0 lmxyy      (501) staff       (20)    10213 2024-04-24 19:18:01.000000 distrifuser-0.0.1b0/README.md
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-04-24 19:29:10.592328 distrifuser-0.0.1b0/distrifuser/
+-rw-r--r--   0 lmxyy      (501) staff       (20)        0 2023-12-12 16:42:09.000000 distrifuser-0.0.1b0/distrifuser/__init__.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)       27 2024-04-24 18:40:16.000000 distrifuser-0.0.1b0/distrifuser/__version__.py
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-04-24 19:29:10.594329 distrifuser-0.0.1b0/distrifuser/models/
+-rw-r--r--   0 lmxyy      (501) staff       (20)        0 2024-02-04 21:34:52.000000 distrifuser-0.0.1b0/distrifuser/models/__init__.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     1774 2024-02-06 06:15:38.000000 distrifuser-0.0.1b0/distrifuser/models/base_model.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)    10944 2024-04-24 18:20:45.000000 distrifuser-0.0.1b0/distrifuser/models/distri_sdxl_unet_pp.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)    10171 2024-04-24 18:19:27.000000 distrifuser-0.0.1b0/distrifuser/models/distri_sdxl_unet_tp.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)    10866 2024-04-24 18:36:01.000000 distrifuser-0.0.1b0/distrifuser/models/naive_patch_sdxl.py
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-04-24 19:29:10.594664 distrifuser-0.0.1b0/distrifuser/modules/
+-rw-r--r--   0 lmxyy      (501) staff       (20)        0 2023-12-12 18:11:45.000000 distrifuser-0.0.1b0/distrifuser/modules/__init__.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)      670 2024-02-06 06:15:38.000000 distrifuser-0.0.1b0/distrifuser/modules/base_module.py
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-04-24 19:29:10.595589 distrifuser-0.0.1b0/distrifuser/modules/pp/
+-rw-r--r--   0 lmxyy      (501) staff       (20)        0 2024-02-06 06:15:38.000000 distrifuser-0.0.1b0/distrifuser/modules/pp/__init__.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     7309 2024-02-28 17:20:17.000000 distrifuser-0.0.1b0/distrifuser/modules/pp/attn.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     5242 2024-02-14 05:29:38.000000 distrifuser-0.0.1b0/distrifuser/modules/pp/conv2d.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     4880 2024-04-24 19:10:39.000000 distrifuser-0.0.1b0/distrifuser/modules/pp/groupnorm.py
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-04-24 19:29:10.597208 distrifuser-0.0.1b0/distrifuser/modules/tp/
+-rw-r--r--   0 lmxyy      (501) staff       (20)        0 2024-02-06 06:15:38.000000 distrifuser-0.0.1b0/distrifuser/modules/tp/__init__.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     7032 2024-02-14 06:26:15.000000 distrifuser-0.0.1b0/distrifuser/modules/tp/attention.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     2209 2024-02-14 06:26:15.000000 distrifuser-0.0.1b0/distrifuser/modules/tp/conv2d.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     3533 2024-02-14 06:26:15.000000 distrifuser-0.0.1b0/distrifuser/modules/tp/feed_forward.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     7627 2024-02-14 06:26:15.000000 distrifuser-0.0.1b0/distrifuser/modules/tp/resnet.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)    11405 2024-04-24 19:18:01.000000 distrifuser-0.0.1b0/distrifuser/pipelines.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     7172 2024-04-24 19:07:33.000000 distrifuser-0.0.1b0/distrifuser/utils.py
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2024-04-24 19:29:10.593118 distrifuser-0.0.1b0/distrifuser.egg-info/
+-rw-r--r--   0 lmxyy      (501) staff       (20)    10759 2024-04-24 19:29:10.000000 distrifuser-0.0.1b0/distrifuser.egg-info/PKG-INFO
+-rw-r--r--   0 lmxyy      (501) staff       (20)      866 2024-04-24 19:29:10.000000 distrifuser-0.0.1b0/distrifuser.egg-info/SOURCES.txt
+-rw-r--r--   0 lmxyy      (501) staff       (20)        1 2024-04-24 19:29:10.000000 distrifuser-0.0.1b0/distrifuser.egg-info/dependency_links.txt
+-rw-r--r--   0 lmxyy      (501) staff       (20)       47 2024-04-24 19:29:10.000000 distrifuser-0.0.1b0/distrifuser.egg-info/requires.txt
+-rw-r--r--   0 lmxyy      (501) staff       (20)       12 2024-04-24 19:29:10.000000 distrifuser-0.0.1b0/distrifuser.egg-info/top_level.txt
+-rw-r--r--   0 lmxyy      (501) staff       (20)       38 2024-04-24 19:29:10.597887 distrifuser-0.0.1b0/setup.cfg
+-rw-r--r--   0 lmxyy      (501) staff       (20)     1079 2024-04-24 18:09:21.000000 distrifuser-0.0.1b0/setup.py
```

### Comparing `distrifuser-0.0.0b1/LICENSE.txt` & `distrifuser-0.0.1b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.0b1/PKG-INFO` & `distrifuser-0.0.1b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: distrifuser
-Version: 0.0.0b1
+Version: 0.0.1b0
 Summary: DistriFusion: Distributed Parallel Inference for High-Resolution Diffusion Models
 Home-page: https://github.com/mit-han-lab/distrifuser
 Author: Muyang Li, Tianle Cai, Jiaxin Cao, Qinsheng Zhang, Han Cai, Junjie Bai, Yangqing Jia, Ming-Yu Liu, Kai Li and Song Han
 Author-email: muyangli@mit.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # DistriFusion: Distributed Parallel Inference for High-Resolution Diffusion Models
 
 ### [Paper](http://arxiv.org/abs/2402.19481) | [Project](https://hanlab.mit.edu/projects/distrifusion) | [Blog](https://hanlab.mit.edu/blog/distrifusion)
 
+**[NEW!]** DistriFusion is selected as a **highlight** poster in CVPR 2024!
+
 **[NEW!]** DistriFusion is accepted by CVPR 2024! Our code is publicly available!
 
 ![teaser](https://github.com/mit-han-lab/distrifuser/blob/main/assets/teaser.jpg)
 *We introduce DistriFusion, a training-free algorithm to harness multiple GPUs to accelerate diffusion model inference without sacrificing image quality. Naïve Patch (Overview (b)) suffers from the fragmentation issue due to the lack of patch interaction. The presented examples are generated with SDXL using a 50-step Euler sampler at 1280×1920 resolution, and latency is measured on A100 GPUs.*
 
 DistriFusion: Distributed Parallel Inference for High-Resolution Diffusion Models</br>
 [Muyang Li](https://lmxyy.me/)\*, [Tianle Cai](https://www.tianle.website/)\*, [Jiaxin Cao](https://www.linkedin.com/in/jiaxin-cao-2166081b3/), [Qinsheng Zhang](https://qsh-zh.github.io), [Han Cai](https://han-cai.github.io), [Junjie Bai](https://www.linkedin.com/in/junjiebai/), [Yangqing Jia](https://daggerfs.com), [Ming-Yu Liu](https://mingyuliu.net), [Kai Li](https://www.cs.princeton.edu/~li/), and [Song Han](https://hanlab.mit.edu/songhan)</br>
@@ -111,14 +113,16 @@
 
 ```shell
 torchrun --nproc_per_node=$N_GPUS scripts/sdxl_example.py
 ```
 
 where `$N_GPUS` is the number GPUs you want to use.
 
+We also provide a minimal script for running SD1.4/2 with DistriFusion in [`scripts/sd_example.py`](https://github.com/mit-han-lab/distrifuser/blob/main/scripts/sd_example.py). The usage is the same.
+
 ### Benchmark
 
 Our benchmark results are using [PyTorch](https://pytorch.org) 2.2 and [diffusers](https://github.com/huggingface/diffusers) 0.24.0. First, you may need to install some additional dependencies:
 
 ```shell
 pip install git+https://github.com/zhijian-liu/torchprofile datasets torchmetrics dominate clean-fid
 ```
```

### Comparing `distrifuser-0.0.0b1/README.md` & `distrifuser-0.0.1b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # DistriFusion: Distributed Parallel Inference for High-Resolution Diffusion Models
 
 ### [Paper](http://arxiv.org/abs/2402.19481) | [Project](https://hanlab.mit.edu/projects/distrifusion) | [Blog](https://hanlab.mit.edu/blog/distrifusion)
 
+**[NEW!]** DistriFusion is selected as a **highlight** poster in CVPR 2024!
+
 **[NEW!]** DistriFusion is accepted by CVPR 2024! Our code is publicly available!
 
 ![teaser](https://github.com/mit-han-lab/distrifuser/blob/main/assets/teaser.jpg)
 *We introduce DistriFusion, a training-free algorithm to harness multiple GPUs to accelerate diffusion model inference without sacrificing image quality. Naïve Patch (Overview (b)) suffers from the fragmentation issue due to the lack of patch interaction. The presented examples are generated with SDXL using a 50-step Euler sampler at 1280×1920 resolution, and latency is measured on A100 GPUs.*
 
 DistriFusion: Distributed Parallel Inference for High-Resolution Diffusion Models</br>
 [Muyang Li](https://lmxyy.me/)\*, [Tianle Cai](https://www.tianle.website/)\*, [Jiaxin Cao](https://www.linkedin.com/in/jiaxin-cao-2166081b3/), [Qinsheng Zhang](https://qsh-zh.github.io), [Han Cai](https://han-cai.github.io), [Junjie Bai](https://www.linkedin.com/in/junjiebai/), [Yangqing Jia](https://daggerfs.com), [Ming-Yu Liu](https://mingyuliu.net), [Kai Li](https://www.cs.princeton.edu/~li/), and [Song Han](https://hanlab.mit.edu/songhan)</br>
@@ -98,14 +100,16 @@
 
 ```shell
 torchrun --nproc_per_node=$N_GPUS scripts/sdxl_example.py
 ```
 
 where `$N_GPUS` is the number GPUs you want to use.
 
+We also provide a minimal script for running SD1.4/2 with DistriFusion in [`scripts/sd_example.py`](https://github.com/mit-han-lab/distrifuser/blob/main/scripts/sd_example.py). The usage is the same.
+
 ### Benchmark
 
 Our benchmark results are using [PyTorch](https://pytorch.org) 2.2 and [diffusers](https://github.com/huggingface/diffusers) 0.24.0. First, you may need to install some additional dependencies:
 
 ```shell
 pip install git+https://github.com/zhijian-liu/torchprofile datasets torchmetrics dominate clean-fid
 ```
@@ -167,8 +171,8 @@
 }
 ```
 
 ## Acknowledgments
 
 Our code is developed based on [huggingface/diffusers](https://github.com/huggingface/diffusers) and [lmxyy/sige](https://github.com/lmxyy/sige). We thank [torchprofile](https://github.com/zhijian-liu/torchprofile) for MACs measurement, [clean-fid](https://github.com/GaParmar/clean-fid) for FID computation and [Lightning-AI/torchmetrics](https://github.com/Lightning-AI/torchmetrics) for PSNR and LPIPS.
 
-We thank Jun-Yan Zhu and Ligeng Zhu for their helpful discussion and valuable feedback. The project is supported by MIT-IBM Watson AI Lab, Amazon, MIT Science Hub, and National Science Foundation.
+We thank Jun-Yan Zhu and Ligeng Zhu for their helpful discussion and valuable feedback. The project is supported by MIT-IBM Watson AI Lab, Amazon, MIT Science Hub, and National Science Foundation.
```

### Comparing `distrifuser-0.0.0b1/distrifuser/models/base_model.py` & `distrifuser-0.0.1b0/distrifuser/models/base_model.py`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.0b1/distrifuser/models/distri_sdxl_unet_pp.py` & `distrifuser-0.0.1b0/distrifuser/models/distri_sdxl_unet_pp.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from distrifuser.modules.pp.attn import DistriCrossAttentionPP, DistriSelfAttentionPP
 from distrifuser.modules.base_module import BaseModule
 from distrifuser.modules.pp.conv2d import DistriConv2dPP
 from distrifuser.modules.pp.groupnorm import DistriGroupNorm
 from ..utils import DistriConfig
 
 
-class DistriSDXLUNetPP(BaseModel):  # for Patch Parallelism
+class DistriUNetPP(BaseModel):  # for Patch Parallelism
     def __init__(self, model: UNet2DConditionModel, distri_config: DistriConfig):
         assert isinstance(model, UNet2DConditionModel)
         if distri_config.world_size > 1 and distri_config.n_device_per_batch > 1:
             for name, module in model.named_modules():
                 if isinstance(module, BaseModule):
                     continue
                 for subname, submodule in module.named_children():
@@ -35,15 +35,15 @@
                             assert subname == "attn2"
                             wrapped_submodule = DistriCrossAttentionPP(submodule, distri_config)
                         setattr(module, subname, wrapped_submodule)
                     elif isinstance(submodule, nn.GroupNorm):
                         wrapped_submodule = DistriGroupNorm(submodule, distri_config)
                         setattr(module, subname, wrapped_submodule)
 
-        super(DistriSDXLUNetPP, self).__init__(model, distri_config)
+        super(DistriUNetPP, self).__init__(model, distri_config)
 
     def forward(
         self,
         sample: torch.FloatTensor,
         timestep: torch.Tensor or float or int,
         encoder_hidden_states: torch.Tensor,
         class_labels: torch.Tensor or None = None,
@@ -78,16 +78,17 @@
                 assert b == 2
                 batch_idx = distri_config.batch_idx()
                 sample = sample[batch_idx : batch_idx + 1]
                 timestep = (
                     timestep[batch_idx : batch_idx + 1] if torch.is_tensor(timestep) and timestep.ndim > 0 else timestep
                 )
                 encoder_hidden_states = encoder_hidden_states[batch_idx : batch_idx + 1]
-                for k in added_cond_kwargs:
-                    added_cond_kwargs[k] = added_cond_kwargs[k][batch_idx : batch_idx + 1]
+                if added_cond_kwargs is not None:
+                    for k in added_cond_kwargs:
+                        added_cond_kwargs[k] = added_cond_kwargs[k][batch_idx : batch_idx + 1]
 
             assert static_inputs["sample"].shape == sample.shape
             static_inputs["sample"].copy_(sample)
             if torch.is_tensor(timestep):
                 if timestep.ndim == 0:
                     for b in range(static_inputs["timestep"].shape[0]):
                         static_inputs["timestep"][b] = timestep.item()
@@ -95,17 +96,18 @@
                     assert static_inputs["timestep"].shape == timestep.shape
                     static_inputs["timestep"].copy_(timestep)
             else:
                 for b in range(static_inputs["timestep"].shape[0]):
                     static_inputs["timestep"][b] = timestep
             assert static_inputs["encoder_hidden_states"].shape == encoder_hidden_states.shape
             static_inputs["encoder_hidden_states"].copy_(encoder_hidden_states)
-            for k in added_cond_kwargs:
-                assert static_inputs["added_cond_kwargs"][k].shape == added_cond_kwargs[k].shape
-                static_inputs["added_cond_kwargs"][k].copy_(added_cond_kwargs[k])
+            if added_cond_kwargs is not None:
+                for k in added_cond_kwargs:
+                    assert static_inputs["added_cond_kwargs"][k].shape == added_cond_kwargs[k].shape
+                    static_inputs["added_cond_kwargs"][k].copy_(added_cond_kwargs[k])
 
             if self.counter <= distri_config.warmup_steps:
                 graph_idx = 0
             elif self.counter == distri_config.warmup_steps + 1:
                 graph_idx = 1
             else:
                 graph_idx = 2
@@ -133,18 +135,19 @@
                 assert b == 2
                 batch_idx = distri_config.batch_idx()
                 sample = sample[batch_idx : batch_idx + 1]
                 timestep = (
                     timestep[batch_idx : batch_idx + 1] if torch.is_tensor(timestep) and timestep.ndim > 0 else timestep
                 )
                 encoder_hidden_states = encoder_hidden_states[batch_idx : batch_idx + 1]
-                new_added_cond_kwargs = {}
-                for k in added_cond_kwargs:
-                    new_added_cond_kwargs[k] = added_cond_kwargs[k][batch_idx : batch_idx + 1]
-                added_cond_kwargs = new_added_cond_kwargs
+                if added_cond_kwargs is not None:
+                    new_added_cond_kwargs = {}
+                    for k in added_cond_kwargs:
+                        new_added_cond_kwargs[k] = added_cond_kwargs[k][batch_idx : batch_idx + 1]
+                    added_cond_kwargs = new_added_cond_kwargs
                 output = self.model(
                     sample,
                     timestep,
                     encoder_hidden_states,
                     class_labels=class_labels,
                     timestep_cond=timestep_cond,
                     attention_mask=attention_mask,
```

### Comparing `distrifuser-0.0.0b1/distrifuser/models/distri_sdxl_unet_tp.py` & `distrifuser-0.0.1b0/distrifuser/models/distri_sdxl_unet_tp.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from ..modules.tp.attention import DistriAttentionTP
 from ..modules.tp.conv2d import DistriConv2dTP
 from ..modules.tp.feed_forward import DistriFeedForwardTP
 from ..modules.tp.resnet import DistriResnetBlock2DTP
 from ..utils import DistriConfig
 
 
-class DistriSDXLUNetTP(BaseModel):  # for Patch Parallelism
+class DistriUNetTP(BaseModel):  # for Patch Parallelism
     def __init__(self, model: UNet2DConditionModel, distri_config: DistriConfig):
         assert isinstance(model, UNet2DConditionModel)
         if distri_config.world_size > 1 and distri_config.n_device_per_batch > 1:
             for name, module in model.named_modules():
                 if isinstance(module, BaseModule):
                     continue
                 for subname, submodule in module.named_children():
@@ -33,15 +33,15 @@
                         setattr(module, subname, wrapped_submodule)
                     elif isinstance(submodule, nn.Conv2d) and (
                         subname == "conv_out" or "downsamplers" in name or "upsamplers" in name
                     ):
                         wrapped_submodule = DistriConv2dTP(submodule, distri_config)
                         setattr(module, subname, wrapped_submodule)
 
-        super(DistriSDXLUNetTP, self).__init__(model, distri_config)
+        super(DistriUNetTP, self).__init__(model, distri_config)
 
     def forward(
         self,
         sample: torch.FloatTensor,
         timestep: torch.Tensor or float or int,
         encoder_hidden_states: torch.Tensor,
         class_labels: torch.Tensor or None = None,
@@ -76,16 +76,17 @@
                 assert b == 2
                 batch_idx = distri_config.batch_idx()
                 sample = sample[batch_idx : batch_idx + 1]
                 timestep = (
                     timestep[batch_idx : batch_idx + 1] if torch.is_tensor(timestep) and timestep.ndim > 0 else timestep
                 )
                 encoder_hidden_states = encoder_hidden_states[batch_idx : batch_idx + 1]
-                for k in added_cond_kwargs:
-                    added_cond_kwargs[k] = added_cond_kwargs[k][batch_idx : batch_idx + 1]
+                if added_cond_kwargs is not None:
+                    for k in added_cond_kwargs:
+                        added_cond_kwargs[k] = added_cond_kwargs[k][batch_idx : batch_idx + 1]
 
             assert static_inputs["sample"].shape == sample.shape
             static_inputs["sample"].copy_(sample)
             if torch.is_tensor(timestep):
                 if timestep.ndim == 0:
                     for b in range(static_inputs["timestep"].shape[0]):
                         static_inputs["timestep"][b] = timestep.item()
@@ -93,17 +94,18 @@
                     assert static_inputs["timestep"].shape == timestep.shape
                     static_inputs["timestep"].copy_(timestep)
             else:
                 for b in range(static_inputs["timestep"].shape[0]):
                     static_inputs["timestep"][b] = timestep
             assert static_inputs["encoder_hidden_states"].shape == encoder_hidden_states.shape
             static_inputs["encoder_hidden_states"].copy_(encoder_hidden_states)
-            for k in added_cond_kwargs:
-                assert static_inputs["added_cond_kwargs"][k].shape == added_cond_kwargs[k].shape
-                static_inputs["added_cond_kwargs"][k].copy_(added_cond_kwargs[k])
+            if added_cond_kwargs is not None:
+                for k in added_cond_kwargs:
+                    assert static_inputs["added_cond_kwargs"][k].shape == added_cond_kwargs[k].shape
+                    static_inputs["added_cond_kwargs"][k].copy_(added_cond_kwargs[k])
 
             graph_idx = 0
 
             self.cuda_graphs[graph_idx].replay()
             output = self.static_outputs[graph_idx]
         else:
             if distri_config.world_size == 1:
@@ -126,18 +128,19 @@
                 assert b == 2
                 batch_idx = distri_config.batch_idx()
                 sample = sample[batch_idx : batch_idx + 1]
                 timestep = (
                     timestep[batch_idx : batch_idx + 1] if torch.is_tensor(timestep) and timestep.ndim > 0 else timestep
                 )
                 encoder_hidden_states = encoder_hidden_states[batch_idx : batch_idx + 1]
-                new_added_cond_kwargs = {}
-                for k in added_cond_kwargs:
-                    new_added_cond_kwargs[k] = added_cond_kwargs[k][batch_idx : batch_idx + 1]
-                added_cond_kwargs = new_added_cond_kwargs
+                if added_cond_kwargs is not None:
+                    new_added_cond_kwargs = {}
+                    for k in added_cond_kwargs:
+                        new_added_cond_kwargs[k] = added_cond_kwargs[k][batch_idx : batch_idx + 1]
+                    added_cond_kwargs = new_added_cond_kwargs
                 output = self.model(
                     sample,
                     timestep,
                     encoder_hidden_states,
                     class_labels=class_labels,
                     timestep_cond=timestep_cond,
                     attention_mask=attention_mask,
```

### Comparing `distrifuser-0.0.0b1/distrifuser/models/naive_patch_sdxl.py` & `distrifuser-0.0.1b0/distrifuser/models/naive_patch_sdxl.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from diffusers.models.unet_2d_condition import UNet2DConditionOutput
 from torch import distributed as dist
 
 from .base_model import BaseModel
 from ..utils import DistriConfig
 
 
-class NaivePatchSDXL(BaseModel):  # for Patch Parallelism
+class NaivePatchUNet(BaseModel):  # for Patch Parallelism
     def __init__(self, model: UNet2DConditionModel, distri_config: DistriConfig):
         assert isinstance(model, UNet2DConditionModel)
-        super(NaivePatchSDXL, self).__init__(model, distri_config)
+        super(NaivePatchUNet, self).__init__(model, distri_config)
 
     def forward(
         self,
         sample: torch.FloatTensor,
         timestep: torch.Tensor or float or int,
         encoder_hidden_states: torch.Tensor,
         class_labels: torch.Tensor or None = None,
@@ -49,16 +49,17 @@
                 assert b == 2
                 batch_idx = distri_config.batch_idx()
                 sample = sample[batch_idx : batch_idx + 1]
                 timestep = (
                     timestep[batch_idx : batch_idx + 1] if torch.is_tensor(timestep) and timestep.ndim > 0 else timestep
                 )
                 encoder_hidden_states = encoder_hidden_states[batch_idx : batch_idx + 1]
-                for k in added_cond_kwargs:
-                    added_cond_kwargs[k] = added_cond_kwargs[k][batch_idx : batch_idx + 1]
+                if added_cond_kwargs is not None:
+                    for k in added_cond_kwargs:
+                        added_cond_kwargs[k] = added_cond_kwargs[k][batch_idx : batch_idx + 1]
 
             assert static_inputs["sample"].shape == sample.shape
             static_inputs["sample"].copy_(sample)
             if torch.is_tensor(timestep):
                 if timestep.ndim == 0:
                     for b in range(static_inputs["timestep"].shape[0]):
                         static_inputs["timestep"][b] = timestep.item()
@@ -66,17 +67,18 @@
                     assert static_inputs["timestep"].shape == timestep.shape
                     static_inputs["timestep"].copy_(timestep)
             else:
                 for b in range(static_inputs["timestep"].shape[0]):
                     static_inputs["timestep"][b] = timestep
             assert static_inputs["encoder_hidden_states"].shape == encoder_hidden_states.shape
             static_inputs["encoder_hidden_states"].copy_(encoder_hidden_states)
-            for k in added_cond_kwargs:
-                assert static_inputs["added_cond_kwargs"][k].shape == added_cond_kwargs[k].shape
-                static_inputs["added_cond_kwargs"][k].copy_(added_cond_kwargs[k])
+            if added_cond_kwargs is not None:
+                for k in added_cond_kwargs:
+                    assert static_inputs["added_cond_kwargs"][k].shape == added_cond_kwargs[k].shape
+                    static_inputs["added_cond_kwargs"][k].copy_(added_cond_kwargs[k])
 
             graph_idx = 0
             if distri_config.split_scheme == "alternate":
                 graph_idx = self.counter % 2
             self.cuda_graphs[graph_idx].replay()
             output = self.static_outputs[graph_idx]
         else:
@@ -100,18 +102,19 @@
                 assert b == 2
                 batch_idx = distri_config.batch_idx()
                 sample = sample[batch_idx : batch_idx + 1]
                 timestep = (
                     timestep[batch_idx : batch_idx + 1] if torch.is_tensor(timestep) and timestep.ndim > 0 else timestep
                 )
                 encoder_hidden_states = encoder_hidden_states[batch_idx : batch_idx + 1]
-                new_added_cond_kwargs = {}
-                for k in added_cond_kwargs:
-                    new_added_cond_kwargs[k] = added_cond_kwargs[k][batch_idx : batch_idx + 1]
-                added_cond_kwargs = new_added_cond_kwargs
+                if added_cond_kwargs is not None:
+                    new_added_cond_kwargs = {}
+                    for k in added_cond_kwargs:
+                        new_added_cond_kwargs[k] = added_cond_kwargs[k][batch_idx : batch_idx + 1]
+                    added_cond_kwargs = new_added_cond_kwargs
 
                 if distri_config.split_scheme == "row":
                     split_dim = 2
                 elif distri_config.split_scheme == "col":
                     split_dim = 3
                 elif distri_config.split_scheme == "alternate":
                     split_dim = 2 if self.counter % 2 == 0 else 3
```

### Comparing `distrifuser-0.0.0b1/distrifuser/modules/base_module.py` & `distrifuser-0.0.1b0/distrifuser/modules/base_module.py`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.0b1/distrifuser/modules/pp/attn.py` & `distrifuser-0.0.1b0/distrifuser/modules/pp/attn.py`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.0b1/distrifuser/modules/pp/conv2d.py` & `distrifuser-0.0.1b0/distrifuser/modules/pp/conv2d.py`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.0b1/distrifuser/modules/pp/groupnorm.py` & `distrifuser-0.0.1b0/distrifuser/modules/pp/groupnorm.py`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.0b1/distrifuser/modules/tp/attention.py` & `distrifuser-0.0.1b0/distrifuser/modules/tp/attention.py`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.0b1/distrifuser/modules/tp/conv2d.py` & `distrifuser-0.0.1b0/distrifuser/modules/tp/conv2d.py`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.0b1/distrifuser/modules/tp/feed_forward.py` & `distrifuser-0.0.1b0/distrifuser/modules/tp/feed_forward.py`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.0b1/distrifuser/modules/tp/resnet.py` & `distrifuser-0.0.1b0/distrifuser/modules/tp/resnet.py`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.0b1/distrifuser/pipelines.py` & `distrifuser-0.0.1b0/distrifuser/pipelines.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
-from diffusers import StableDiffusionXLPipeline, UNet2DConditionModel
+from diffusers import StableDiffusionPipeline, StableDiffusionXLPipeline, UNet2DConditionModel
 
-from .models.distri_sdxl_unet_pp import DistriSDXLUNetPP
-from .models.distri_sdxl_unet_tp import DistriSDXLUNetTP
-from .models.naive_patch_sdxl import NaivePatchSDXL
+from .models.distri_sdxl_unet_pp import DistriUNetPP
+from .models.distri_sdxl_unet_tp import DistriUNetTP
+from .models.naive_patch_sdxl import NaivePatchUNet
 from .utils import DistriConfig, PatchParallelismCommManager
 
 
 class DistriSDXLPipeline:
     def __init__(self, pipeline: StableDiffusionXLPipeline, module_config: DistriConfig):
         self.pipeline = pipeline
         self.distri_config = module_config
@@ -24,19 +24,19 @@
         )
         torch_dtype = kwargs.pop("torch_dtype", torch.float16)
         unet = UNet2DConditionModel.from_pretrained(
             pretrained_model_name_or_path, torch_dtype=torch_dtype, subfolder="unet"
         ).to(device)
 
         if distri_config.parallelism == "patch":
-            unet = DistriSDXLUNetPP(unet, distri_config)
+            unet = DistriUNetPP(unet, distri_config)
         elif distri_config.parallelism == "tensor":
-            unet = DistriSDXLUNetTP(unet, distri_config)
+            unet = DistriUNetTP(unet, distri_config)
         elif distri_config.parallelism == "naive_patch":
-            unet = NaivePatchSDXL(unet, distri_config)
+            unet = NaivePatchUNet(unet, distri_config)
         else:
             raise ValueError(f"Unknown parallelism: {distri_config.parallelism}")
 
         pipeline = StableDiffusionXLPipeline.from_pretrained(
             pretrained_model_name_or_path, torch_dtype=torch_dtype, unet=unet, **kwargs
         ).to(device)
         return DistriSDXLPipeline(pipeline, distri_config)
@@ -125,14 +125,141 @@
 
         # Used to create communication buffer
         comm_manager = None
         if distri_config.n_device_per_batch > 1:
             comm_manager = PatchParallelismCommManager(distri_config)
             pipeline.unet.set_comm_manager(comm_manager)
 
+            # Only used for creating the communication buffer
+            pipeline.unet.set_counter(0)
+            pipeline.unet(**static_inputs, return_dict=False, record=True)
+            if comm_manager.numel > 0:
+                comm_manager.create_buffer()
+
+        # Pre-run
+        pipeline.unet.set_counter(0)
+        pipeline.unet(**static_inputs, return_dict=False, record=True)
+
+        if distri_config.use_cuda_graph:
+            if comm_manager is not None:
+                comm_manager.clear()
+            if distri_config.parallelism == "naive_patch":
+                counters = [0, 1]
+            elif distri_config.parallelism == "patch":
+                counters = [0, distri_config.warmup_steps + 1, distri_config.warmup_steps + 2]
+            elif distri_config.parallelism == "tensor":
+                counters = [0]
+            else:
+                raise ValueError(f"Unknown parallelism: {distri_config.parallelism}")
+            for counter in counters:
+                graph = torch.cuda.CUDAGraph()
+                with torch.cuda.graph(graph):
+                    pipeline.unet.set_counter(counter)
+                    output = pipeline.unet(**static_inputs, return_dict=False, record=True)[0]
+                    static_outputs.append(output)
+                cuda_graphs.append(graph)
+            pipeline.unet.setup_cuda_graph(static_outputs, cuda_graphs)
+
+        self.static_inputs = static_inputs
+
+
+class DistriSDPipeline:
+    def __init__(self, pipeline: StableDiffusionPipeline, module_config: DistriConfig):
+        self.pipeline = pipeline
+        self.distri_config = module_config
+
+        self.static_inputs = None
+
+        self.prepare()
+
+    @staticmethod
+    def from_pretrained(distri_config: DistriConfig, **kwargs):
+        device = distri_config.device
+        pretrained_model_name_or_path = kwargs.pop("pretrained_model_name_or_path", "CompVis/stable-diffusion-v1-4")
+        torch_dtype = kwargs.pop("torch_dtype", torch.float16)
+        unet = UNet2DConditionModel.from_pretrained(
+            pretrained_model_name_or_path, torch_dtype=torch_dtype, subfolder="unet"
+        ).to(device)
+
+        if distri_config.parallelism == "patch":
+            unet = DistriUNetPP(unet, distri_config)
+        elif distri_config.parallelism == "tensor":
+            unet = DistriUNetTP(unet, distri_config)
+        elif distri_config.parallelism == "naive_patch":
+            unet = NaivePatchUNet(unet, distri_config)
+        else:
+            raise ValueError(f"Unknown parallelism: {distri_config.parallelism}")
+
+        pipeline = StableDiffusionPipeline.from_pretrained(
+            pretrained_model_name_or_path, torch_dtype=torch_dtype, unet=unet, **kwargs
+        ).to(device)
+        return DistriSDPipeline(pipeline, distri_config)
+
+    def set_progress_bar_config(self, **kwargs):
+        self.pipeline.set_progress_bar_config(**kwargs)
+
+    @torch.no_grad()
+    def __call__(self, *args, **kwargs):
+        assert "height" not in kwargs, "height should not be in kwargs"
+        assert "width" not in kwargs, "width should not be in kwargs"
+        config = self.distri_config
+        self.pipeline.unet.set_counter(0)
+        return self.pipeline(height=config.height, width=config.width, *args, **kwargs)
+
+    @torch.no_grad()
+    def prepare(self, **kwargs):
+        distri_config = self.distri_config
+
+        static_inputs = {}
+        static_outputs = []
+        cuda_graphs = []
+        pipeline = self.pipeline
+
+        height = distri_config.height
+        width = distri_config.width
+        assert height % 8 == 0 and width % 8 == 0
+
+        device = distri_config.device
+
+        prompt_embeds, negative_prompt_embeds = pipeline.encode_prompt(
+            "",
+            device,
+            num_images_per_prompt=1,
+            do_classifier_free_guidance=False,
+            negative_prompt=None,
+            prompt_embeds=None,
+            negative_prompt_embeds=None,
+            lora_scale=None,
+            clip_skip=kwargs.get("clip_skip", None),
+        )
+
+        batch_size = 2 if distri_config.do_classifier_free_guidance else 1
+
+        num_channels_latents = pipeline.unet.config.in_channels
+        latents = pipeline.prepare_latents(
+            batch_size, num_channels_latents, height, width, prompt_embeds.dtype, device, None
+        )
+
+        prompt_embeds = prompt_embeds.to(device)
+
+        if batch_size > 1:
+            prompt_embeds = prompt_embeds.repeat(batch_size, 1, 1)
+
+        t = torch.zeros([batch_size], device=device, dtype=torch.long)
+
+        static_inputs["sample"] = latents
+        static_inputs["timestep"] = t
+        static_inputs["encoder_hidden_states"] = prompt_embeds
+
+        # Used to create communication buffer
+        comm_manager = None
+        if distri_config.n_device_per_batch > 1:
+            comm_manager = PatchParallelismCommManager(distri_config)
+            pipeline.unet.set_comm_manager(comm_manager)
+
             # Only used for creating the communication buffer
             pipeline.unet.set_counter(0)
             pipeline.unet(**static_inputs, return_dict=False, record=True)
             if comm_manager.numel > 0:
                 comm_manager.create_buffer()
 
         # Pre-run
```

### Comparing `distrifuser-0.0.0b1/distrifuser/utils.py` & `distrifuser-0.0.1b0/distrifuser/utils.py`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.0b1/distrifuser.egg-info/PKG-INFO` & `distrifuser-0.0.1b0/distrifuser.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: distrifuser
-Version: 0.0.0b1
+Version: 0.0.1b0
 Summary: DistriFusion: Distributed Parallel Inference for High-Resolution Diffusion Models
 Home-page: https://github.com/mit-han-lab/distrifuser
 Author: Muyang Li, Tianle Cai, Jiaxin Cao, Qinsheng Zhang, Han Cai, Junjie Bai, Yangqing Jia, Ming-Yu Liu, Kai Li and Song Han
 Author-email: muyangli@mit.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # DistriFusion: Distributed Parallel Inference for High-Resolution Diffusion Models
 
 ### [Paper](http://arxiv.org/abs/2402.19481) | [Project](https://hanlab.mit.edu/projects/distrifusion) | [Blog](https://hanlab.mit.edu/blog/distrifusion)
 
+**[NEW!]** DistriFusion is selected as a **highlight** poster in CVPR 2024!
+
 **[NEW!]** DistriFusion is accepted by CVPR 2024! Our code is publicly available!
 
 ![teaser](https://github.com/mit-han-lab/distrifuser/blob/main/assets/teaser.jpg)
 *We introduce DistriFusion, a training-free algorithm to harness multiple GPUs to accelerate diffusion model inference without sacrificing image quality. Naïve Patch (Overview (b)) suffers from the fragmentation issue due to the lack of patch interaction. The presented examples are generated with SDXL using a 50-step Euler sampler at 1280×1920 resolution, and latency is measured on A100 GPUs.*
 
 DistriFusion: Distributed Parallel Inference for High-Resolution Diffusion Models</br>
 [Muyang Li](https://lmxyy.me/)\*, [Tianle Cai](https://www.tianle.website/)\*, [Jiaxin Cao](https://www.linkedin.com/in/jiaxin-cao-2166081b3/), [Qinsheng Zhang](https://qsh-zh.github.io), [Han Cai](https://han-cai.github.io), [Junjie Bai](https://www.linkedin.com/in/junjiebai/), [Yangqing Jia](https://daggerfs.com), [Ming-Yu Liu](https://mingyuliu.net), [Kai Li](https://www.cs.princeton.edu/~li/), and [Song Han](https://hanlab.mit.edu/songhan)</br>
@@ -111,14 +113,16 @@
 
 ```shell
 torchrun --nproc_per_node=$N_GPUS scripts/sdxl_example.py
 ```
 
 where `$N_GPUS` is the number GPUs you want to use.
 
+We also provide a minimal script for running SD1.4/2 with DistriFusion in [`scripts/sd_example.py`](https://github.com/mit-han-lab/distrifuser/blob/main/scripts/sd_example.py). The usage is the same.
+
 ### Benchmark
 
 Our benchmark results are using [PyTorch](https://pytorch.org) 2.2 and [diffusers](https://github.com/huggingface/diffusers) 0.24.0. First, you may need to install some additional dependencies:
 
 ```shell
 pip install git+https://github.com/zhijian-liu/torchprofile datasets torchmetrics dominate clean-fid
 ```
```

### Comparing `distrifuser-0.0.0b1/distrifuser.egg-info/SOURCES.txt` & `distrifuser-0.0.1b0/distrifuser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `distrifuser-0.0.0b1/setup.py` & `distrifuser-0.0.1b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     version = eval(fp.strip().split()[-1])
 
     setup(
         name="distrifuser",
         author="Muyang Li, Tianle Cai, Jiaxin Cao, Qinsheng Zhang, Han Cai, Junjie Bai, Yangqing Jia, Ming-Yu Liu, Kai Li and Song Han",
         author_email="muyangli@mit.edu",
         packages=find_packages(),
-        install_requires=["torch>=2.2", "diffusers>=0.24.0", "transformers", "tqdm"],
+        install_requires=["torch>=2.2", "diffusers==0.24.0", "transformers", "tqdm"],
         url="https://github.com/mit-han-lab/distrifuser",
         description="DistriFusion: Distributed Parallel Inference for High-Resolution Diffusion Models",
         long_description=long_description,
         long_description_content_type="text/markdown",
         version=version,
         classifiers=[
             "Programming Language :: Python :: 3",
```

