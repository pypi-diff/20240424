# Comparing `tmp/litdata-0.2.3.tar.gz` & `tmp/litdata-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litdata-0.2.3.tar", last modified: Wed Apr  3 09:19:15 2024, max compression
+gzip compressed data, was "litdata-0.2.4.tar", last modified: Wed Apr 24 16:14:16 2024, max compression
```

## Comparing `litdata-0.2.3.tar` & `litdata-0.2.4.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:19:15.409219 litdata-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-03 09:19:05.000000 litdata-0.2.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-04-03 09:19:05.000000 litdata-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-03 09:19:05.000000 litdata-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20638 2024-04-03 09:19:15.409219 litdata-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18917 2024-04-03 09:19:05.000000 litdata-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 09:19:05.000000 litdata-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 09:19:15.409219 litdata-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-03 09:19:05.000000 litdata-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:19:15.401219 litdata-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:19:15.401219 litdata-0.2.3/src/litdata/
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:19:15.405219 litdata-0.2.3/src/litdata/processing/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42556 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/processing/data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17136 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/processing/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/processing/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/processing/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:19:15.405219 litdata-0.2.3/src/litdata/streaming/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/combined.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    25854 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/item_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9749 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    14520 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (127)    18051 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:19:15.409219 litdata-0.2.3/src/litdata/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/utilities/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/utilities/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/utilities/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/utilities/packing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/utilities/shuffle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:19:15.409219 litdata-0.2.3/src/litdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20638 2024-04-03 09:19:15.000000 litdata-0.2.3/src/litdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-03 09:19:15.000000 litdata-0.2.3/src/litdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:19:15.000000 litdata-0.2.3/src/litdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:19:15.000000 litdata-0.2.3/src/litdata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 09:19:15.000000 litdata-0.2.3/src/litdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 09:19:15.000000 litdata-0.2.3/src/litdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:14:16.085019 litdata-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-24 16:14:06.000000 litdata-0.2.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-04-24 16:14:06.000000 litdata-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-24 16:14:06.000000 litdata-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20638 2024-04-24 16:14:16.085019 litdata-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18917 2024-04-24 16:14:06.000000 litdata-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-24 16:14:06.000000 litdata-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 16:14:16.085019 litdata-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-24 16:14:06.000000 litdata-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:14:16.077019 litdata-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:14:16.081019 litdata-0.2.4/src/litdata/
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:14:16.081019 litdata-0.2.4/src/litdata/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42470 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/processing/data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17078 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/processing/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/processing/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/processing/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:14:16.085019 litdata-0.2.4/src/litdata/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/combined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25796 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8731 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/item_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9749 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14520 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17993 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:14:16.085019 litdata-0.2.4/src/litdata/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52973 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/utilities/_pytree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/utilities/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/utilities/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/utilities/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/utilities/packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/utilities/shuffle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:14:16.085019 litdata-0.2.4/src/litdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20638 2024-04-24 16:14:16.000000 litdata-0.2.4/src/litdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-24 16:14:16.000000 litdata-0.2.4/src/litdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:14:16.000000 litdata-0.2.4/src/litdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:14:16.000000 litdata-0.2.4/src/litdata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-24 16:14:16.000000 litdata-0.2.4/src/litdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 16:14:16.000000 litdata-0.2.4/src/litdata.egg-info/top_level.txt
```

### Comparing `litdata-0.2.3/LICENSE` & `litdata-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/MANIFEST.in` & `litdata-0.2.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/PKG-INFO` & `litdata-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litdata
-Version: 0.2.3
+Version: 0.2.4
 Summary: The Deep Learning framework to train, deploy, and ship AI products Lightning fast.
 Home-page: https://github.com/Lightning-AI/lit-data
 Download-URL: https://github.com/Lightning-AI/litdata
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/litdata/issues
@@ -52,15 +52,15 @@
 
 # ⚡ Welcome to LitData
 
 With LitData, users can transform and optimize their data in cloud storage environments efficiently and intuitively, at any scale. 
 
 Once optimized, efficient distributed training becomes practical regardless of where the data is located, enabling users to seamlessly stream data of any size to one or multiple machines.
 
-LitData supports **images, text, video, audio, geo-spatial, and multimodal data** types, is already adopted by frameworks such as [Lit-GPT](https://github.com/Lightning-AI/lit-gpt/blob/main/pretrain/tinyllama.py) to pretrain LLMs and integrates smoothly with [PyTorch Lightning](https://lightning.ai/docs/pytorch/stable/), [Lightning Fabric](https://lightning.ai/docs/fabric/stable/), and [PyTorch](https://pytorch.org/docs/stable/index.html).
+LitData supports **images, text, video, audio, geo-spatial, and multimodal data** types, is already adopted by frameworks such as [LitGPT](https://github.com/Lightning-AI/litgpt/blob/main/litgpt/data/lit_data.py) to pretrain LLMs and integrates smoothly with [PyTorch Lightning](https://lightning.ai/docs/pytorch/stable/), [Lightning Fabric](https://lightning.ai/docs/fabric/stable/), and [PyTorch](https://pytorch.org/docs/stable/index.html).
 
 [Runnable templates](#runnable-templates) published on the [Lightning.AI Platform](https://lightning.ai) are available at the end, **reproducible in 1-click**.
 
 ### Table of Contents
 
 - [Getting started](#getting-started)
     - [Installation](#installation)
```

### Comparing `litdata-0.2.3/README.md` & `litdata-0.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 # ⚡ Welcome to LitData
 
 With LitData, users can transform and optimize their data in cloud storage environments efficiently and intuitively, at any scale. 
 
 Once optimized, efficient distributed training becomes practical regardless of where the data is located, enabling users to seamlessly stream data of any size to one or multiple machines.
 
-LitData supports **images, text, video, audio, geo-spatial, and multimodal data** types, is already adopted by frameworks such as [Lit-GPT](https://github.com/Lightning-AI/lit-gpt/blob/main/pretrain/tinyllama.py) to pretrain LLMs and integrates smoothly with [PyTorch Lightning](https://lightning.ai/docs/pytorch/stable/), [Lightning Fabric](https://lightning.ai/docs/fabric/stable/), and [PyTorch](https://pytorch.org/docs/stable/index.html).
+LitData supports **images, text, video, audio, geo-spatial, and multimodal data** types, is already adopted by frameworks such as [LitGPT](https://github.com/Lightning-AI/litgpt/blob/main/litgpt/data/lit_data.py) to pretrain LLMs and integrates smoothly with [PyTorch Lightning](https://lightning.ai/docs/pytorch/stable/), [Lightning Fabric](https://lightning.ai/docs/fabric/stable/), and [PyTorch](https://pytorch.org/docs/stable/index.html).
 
 [Runnable templates](#runnable-templates) published on the [Lightning.AI Platform](https://lightning.ai) are available at the end, **reproducible in 1-click**.
 
 ### Table of Contents
 
 - [Getting started](#getting-started)
     - [Installation](#installation)
```

### Comparing `litdata-0.2.3/setup.py` & `litdata-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata/__about__.py` & `litdata-0.2.4/src/litdata/__about__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import time
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 __author__ = "Lightning AI et al."
 __author_email__ = "pytorch@lightning.ai"
 __license__ = "Apache-2.0"
 __copyright__ = f"Copyright (c) 2023-{time.strftime('%Y')}, {__author__}."
 __homepage__ = "https://github.com/Lightning-AI/lit-data"
 __docs_url__ = "https://lightning.ai/docs/pytorch/stable/"
 # this has to be simple string, see: https://github.com/pypa/twine/issues/522
```

### Comparing `litdata-0.2.3/src/litdata/__init__.py` & `litdata-0.2.4/src/litdata/__init__.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata/constants.py` & `litdata-0.2.4/src/litdata/constants.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata/imports.py` & `litdata-0.2.4/src/litdata/imports.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata/processing/__init__.py` & `litdata-0.2.4/src/litdata/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata/processing/data_processor.py` & `litdata-0.2.4/src/litdata/processing/data_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,35 +35,32 @@
 
 from litdata.constants import (
     _BOTO3_AVAILABLE,
     _DEFAULT_FAST_DEV_RUN_ITEMS,
     _INDEX_FILENAME,
     _IS_IN_STUDIO,
     _LIGHTNING_CLOUD_AVAILABLE,
-    _TORCH_GREATER_EQUAL_2_1_0,
 )
 from litdata.imports import RequirementCache
 from litdata.processing.readers import BaseReader, StreamingDataLoaderReader
 from litdata.processing.utilities import _create_dataset
 from litdata.streaming import Cache
 from litdata.streaming.cache import Dir
 from litdata.streaming.client import S3Client
 from litdata.streaming.dataloader import StreamingDataLoader
 from litdata.streaming.resolver import _resolve_dir
+from litdata.utilities._pytree import tree_flatten, tree_unflatten, treespec_loads
 from litdata.utilities.broadcast import broadcast_object
 from litdata.utilities.packing import _pack_greedily
 
 _TQDM_AVAILABLE = RequirementCache("tqdm")
 
 if _TQDM_AVAILABLE:
     from tqdm.auto import tqdm as _tqdm
 
-if _TORCH_GREATER_EQUAL_2_1_0:
-    from torch.utils._pytree import tree_flatten, tree_unflatten, treespec_loads
-
 if _LIGHTNING_CLOUD_AVAILABLE:
     from lightning_cloud.openapi import V1DatasetType
 
 
 if _BOTO3_AVAILABLE:
     import botocore
 
@@ -1015,15 +1012,15 @@
         if num_nodes == 1:
             for w in self.workers:
                 w.join(0)
 
         print("Workers are finished.")
         result = data_recipe._done(len(user_items), self.delete_cached_files, self.output_dir)
 
-        if num_nodes == node_rank + 1 and self.output_dir.url and _IS_IN_STUDIO and self.input_dir.path:
+        if num_nodes == node_rank + 1 and self.output_dir.url and _IS_IN_STUDIO:
             assert self.output_dir.path
             _create_dataset(
                 input_dir=self.input_dir.path,
                 storage_dir=self.output_dir.path,
                 dataset_type=V1DatasetType.CHUNKED
                 if isinstance(data_recipe, DataChunkRecipe)
                 else V1DatasetType.TRANSFORMED,
```

### Comparing `litdata-0.2.3/src/litdata/processing/functions.py` & `litdata-0.2.4/src/litdata/processing/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,29 +18,27 @@
 from functools import partial
 from pathlib import Path
 from types import FunctionType
 from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
 
 import torch
 
-from litdata.constants import _IS_IN_STUDIO, _TORCH_GREATER_EQUAL_2_1_0
+from litdata.constants import _IS_IN_STUDIO
 from litdata.processing.data_processor import DataChunkRecipe, DataProcessor, DataTransformRecipe
 from litdata.processing.readers import BaseReader
 from litdata.processing.utilities import optimize_dns_context
 from litdata.streaming.dataloader import StreamingDataLoader
 from litdata.streaming.resolver import (
     Dir,
     _assert_dir_has_index_file,
     _assert_dir_is_empty,
     _execute,
     _resolve_dir,
 )
-
-if _TORCH_GREATER_EQUAL_2_1_0:
-    from torch.utils._pytree import tree_flatten
+from litdata.utilities._pytree import tree_flatten
 
 
 def _get_indexed_paths(data: Any) -> Dict[int, str]:
     flattened_item, _ = tree_flatten(data)
 
     return {
         index: element
```

### Comparing `litdata-0.2.3/src/litdata/processing/readers.py` & `litdata-0.2.4/src/litdata/processing/readers.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata/processing/utilities.py` & `litdata-0.2.4/src/litdata/processing/utilities.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata/streaming/__init__.py` & `litdata-0.2.4/src/litdata/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata/streaming/cache.py` & `litdata-0.2.4/src/litdata/streaming/cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 import logging
 import os
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from litdata.constants import (
     _INDEX_FILENAME,
-    _TORCH_GREATER_EQUAL_2_1_0,
 )
 from litdata.streaming.item_loader import BaseItemLoader
 from litdata.streaming.reader import BinaryReader
 from litdata.streaming.resolver import Dir, _resolve_dir
 from litdata.streaming.sampler import ChunkedIndex
 from litdata.streaming.serializers import Serializer
 from litdata.streaming.writer import BinaryWriter
@@ -52,17 +51,14 @@
             chunk_size: The maximum number of items within a chunk.
             item_loader: The object responsible to generate the chunk intervals and load an item froma chunk.
             max_cache_size: The maximum cache size used by the reader when fetching the chunks.
             serializers: Provide your own serializers.
 
         """
         super().__init__()
-        if not _TORCH_GREATER_EQUAL_2_1_0:
-            raise ModuleNotFoundError("PyTorch version 2.1 or higher is required to use the cache.")
-
         input_dir = _resolve_dir(input_dir)
         self._cache_dir = input_dir.path
         assert self._cache_dir
         self._writer = BinaryWriter(
             self._cache_dir,
             chunk_size=chunk_size,
             chunk_bytes=chunk_bytes,
```

### Comparing `litdata-0.2.3/src/litdata/streaming/client.py` & `litdata-0.2.4/src/litdata/streaming/client.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata/streaming/combined.py` & `litdata-0.2.4/src/litdata/streaming/combined.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata/streaming/compression.py` & `litdata-0.2.4/src/litdata/streaming/compression.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata/streaming/config.py` & `litdata-0.2.4/src/litdata/streaming/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,23 +11,21 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import os
 from typing import Any, Dict, List, Optional, Tuple
 
-from litdata.constants import _INDEX_FILENAME, _TORCH_GREATER_EQUAL_2_1_0
+from litdata.constants import _INDEX_FILENAME
 from litdata.streaming.compression import _COMPRESSORS, Compressor
 from litdata.streaming.downloader import get_downloader_cls
 from litdata.streaming.item_loader import BaseItemLoader, PyTreeLoader, TokensLoader
 from litdata.streaming.sampler import ChunkedIndex
 from litdata.streaming.serializers import Serializer
-
-if _TORCH_GREATER_EQUAL_2_1_0:
-    from torch.utils._pytree import tree_unflatten, treespec_loads
+from litdata.utilities._pytree import tree_unflatten, treespec_loads
 
 
 class ChunksConfig:
     def __init__(
         self,
         cache_dir: str,
         serializers: Dict[str, Serializer],
@@ -79,15 +77,15 @@
         local_chunkpath = os.path.join(self._cache_dir, chunk_filename)
 
         if os.path.exists(local_chunkpath):
             self.try_decompress(local_chunkpath)
             return
 
         if self._downloader is None:
-            raise RuntimeError("The downloader should be defined.")
+            return
 
         self._downloader.download_chunk_from_index(chunk_index)
 
         self.try_decompress(local_chunkpath)
 
     def try_decompress(self, local_chunkpath: str) -> None:
         if self._compressor is None:
@@ -97,15 +95,17 @@
 
         if os.path.exists(target_local_chunkpath):
             return
 
         with open(local_chunkpath, "rb") as f:
             data = f.read()
 
-        os.remove(local_chunkpath)
+        # delete the files only if they were downloaded
+        if self._downloader is not None:
+            os.remove(local_chunkpath)
 
         data = self._compressor.decompress(data)
 
         with open(target_local_chunkpath, "wb") as f:
             f.write(data)
 
     @property
```

### Comparing `litdata-0.2.3/src/litdata/streaming/dataloader.py` & `litdata-0.2.4/src/litdata/streaming/dataloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,28 +29,26 @@
     _BaseDataLoaderIter,
     _DatasetKind,
     _MultiProcessingDataLoaderIter,
     _SingleProcessDataLoaderIter,
 )
 from torch.utils.data.sampler import BatchSampler, Sampler
 
-from litdata.constants import _DEFAULT_CHUNK_BYTES, _TORCH_GREATER_EQUAL_2_1_0, _VIZ_TRACKER_AVAILABLE
+from litdata.constants import _DEFAULT_CHUNK_BYTES, _VIZ_TRACKER_AVAILABLE
 from litdata.streaming import Cache
 from litdata.streaming.combined import (
     __NUM_SAMPLES_YIELDED_KEY__,
     __SAMPLES_KEY__,
     CombinedStreamingDataset,
 )
 from litdata.streaming.dataset import StreamingDataset
 from litdata.streaming.sampler import CacheBatchSampler
+from litdata.utilities._pytree import tree_flatten
 from litdata.utilities.env import _DistributedEnv
 
-if _TORCH_GREATER_EQUAL_2_1_0:
-    from torch.utils._pytree import tree_flatten
-
 logger = logging.Logger(__name__)
 
 
 def _equal_items(data_1: Any, data_2: Any) -> bool:
     data_1_flattened, _ = tree_flatten(data_1)
     data_2_flattened, _ = tree_flatten(data_2)
```

### Comparing `litdata-0.2.3/src/litdata/streaming/dataset.py` & `litdata-0.2.4/src/litdata/streaming/dataset.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata/streaming/downloader.py` & `litdata-0.2.4/src/litdata/streaming/downloader.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata/streaming/item_loader.py` & `litdata-0.2.4/src/litdata/streaming/item_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,29 +18,42 @@
 from typing import Any, Dict, List, Optional, Tuple
 
 import numpy as np
 import torch
 
 from litdata.constants import (
     _TORCH_DTYPES_MAPPING,
-    _TORCH_GREATER_EQUAL_2_1_0,
 )
 from litdata.streaming.serializers import Serializer
-
-if _TORCH_GREATER_EQUAL_2_1_0:
-    from torch.utils._pytree import PyTree, tree_unflatten
+from litdata.utilities._pytree import PyTree, tree_unflatten
 
 
 class BaseItemLoader(ABC):
     """The base item loader is responsible to decide how the items within a chunk are loaded."""
 
     def setup(self, config: Dict, chunks: List, serializers: Dict[str, Serializer]) -> None:
         self._config = config
         self._chunks = chunks
         self._serializers = serializers
+        self._data_format = self._config["data_format"]
+        self._shift_idx = len(self._data_format) * 4
+
+        # setup the serializers on restart
+        for data_format in self._data_format:
+            serializer = self._serializers[self._data_format_to_key(data_format)]
+            serializer.setup(data_format)
+
+    @functools.lru_cache(maxsize=128)
+    def _data_format_to_key(self, data_format: str) -> str:
+        if ":" in data_format:
+            serialier, serializer_sub_type = data_format.split(":")
+            if serializer_sub_type in self._serializers:
+                return serializer_sub_type
+            return serialier
+        return data_format
 
     def state_dict(self) -> Dict:
         return {}
 
     @abstractmethod
     def generate_intervals(self) -> List[Tuple[int, int]]:
         """Returns a list of tuple describing the indexes intervals of the chunks."""
@@ -105,29 +118,20 @@
             pair = fp.read(8)
             begin, end = np.frombuffer(pair, np.uint32)
             fp.seek(begin)
             data = fp.read(end - begin)
 
         return self.deserialize(data)
 
-    @functools.lru_cache(maxsize=128)
-    def _data_format_to_key(self, data_format: str) -> str:
-        if ":" in data_format:
-            serialier, serializer_sub_type = data_format.split(":")
-            if serializer_sub_type in self._serializers:
-                return serializer_sub_type
-            return serialier
-        return data_format
-
     def deserialize(self, raw_item_data: bytes) -> "PyTree":
         """Deserialize the raw bytes into their python equivalent."""
-        idx = len(self._config["data_format"]) * 4
+        idx = self._shift_idx
         sizes = np.frombuffer(raw_item_data[:idx], np.uint32)
         data = []
-        for size, data_format in zip(sizes, self._config["data_format"]):
+        for size, data_format in zip(sizes, self._data_format):
             serializer = self._serializers[self._data_format_to_key(data_format)]
             data_bytes = raw_item_data[idx : idx + size]
             data.append(serializer.deserialize(data_bytes))
             idx += size
         return tree_unflatten(data, self._config["data_spec"])
 
     def delete(self, chunk_index: int, chunk_filepath: str) -> None:
```

### Comparing `litdata-0.2.3/src/litdata/streaming/reader.py` & `litdata-0.2.4/src/litdata/streaming/reader.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata/streaming/resolver.py` & `litdata-0.2.4/src/litdata/streaming/resolver.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata/streaming/sampler.py` & `litdata-0.2.4/src/litdata/streaming/sampler.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata/streaming/serializers.py` & `litdata-0.2.4/src/litdata/streaming/serializers.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata/streaming/shuffle.py` & `litdata-0.2.4/src/litdata/streaming/shuffle.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata/streaming/writer.py` & `litdata-0.2.4/src/litdata/streaming/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,22 @@
 from dataclasses import dataclass
 from time import sleep
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import torch
 
-from litdata.constants import _INDEX_FILENAME, _TORCH_GREATER_EQUAL_2_1_0
+from litdata.constants import _INDEX_FILENAME
 from litdata.processing.utilities import get_worker_rank
 from litdata.streaming.compression import _COMPRESSORS, Compressor
 from litdata.streaming.serializers import Serializer, _get_serializers
+from litdata.utilities._pytree import PyTree, tree_flatten, treespec_dumps
 from litdata.utilities.env import _DistributedEnv, _WorkerEnv
 from litdata.utilities.format import _convert_bytes_to_int, _human_readable_bytes
 
-if _TORCH_GREATER_EQUAL_2_1_0:
-    from torch.utils._pytree import PyTree, tree_flatten, treespec_dumps
-
 
 @dataclass
 class Item:
     index: int
     data: bytes
     bytes: int
     dim: Optional[int] = None
```

### Comparing `litdata-0.2.3/src/litdata/utilities/__init__.py` & `litdata-0.2.4/src/litdata/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata/utilities/broadcast.py` & `litdata-0.2.4/src/litdata/utilities/broadcast.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata/utilities/env.py` & `litdata-0.2.4/src/litdata/utilities/env.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata/utilities/format.py` & `litdata-0.2.4/src/litdata/utilities/format.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata/utilities/packing.py` & `litdata-0.2.4/src/litdata/utilities/packing.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata/utilities/shuffle.py` & `litdata-0.2.4/src/litdata/utilities/shuffle.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.3/src/litdata.egg-info/PKG-INFO` & `litdata-0.2.4/src/litdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litdata
-Version: 0.2.3
+Version: 0.2.4
 Summary: The Deep Learning framework to train, deploy, and ship AI products Lightning fast.
 Home-page: https://github.com/Lightning-AI/lit-data
 Download-URL: https://github.com/Lightning-AI/litdata
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/litdata/issues
@@ -52,15 +52,15 @@
 
 # ⚡ Welcome to LitData
 
 With LitData, users can transform and optimize their data in cloud storage environments efficiently and intuitively, at any scale. 
 
 Once optimized, efficient distributed training becomes practical regardless of where the data is located, enabling users to seamlessly stream data of any size to one or multiple machines.
 
-LitData supports **images, text, video, audio, geo-spatial, and multimodal data** types, is already adopted by frameworks such as [Lit-GPT](https://github.com/Lightning-AI/lit-gpt/blob/main/pretrain/tinyllama.py) to pretrain LLMs and integrates smoothly with [PyTorch Lightning](https://lightning.ai/docs/pytorch/stable/), [Lightning Fabric](https://lightning.ai/docs/fabric/stable/), and [PyTorch](https://pytorch.org/docs/stable/index.html).
+LitData supports **images, text, video, audio, geo-spatial, and multimodal data** types, is already adopted by frameworks such as [LitGPT](https://github.com/Lightning-AI/litgpt/blob/main/litgpt/data/lit_data.py) to pretrain LLMs and integrates smoothly with [PyTorch Lightning](https://lightning.ai/docs/pytorch/stable/), [Lightning Fabric](https://lightning.ai/docs/fabric/stable/), and [PyTorch](https://pytorch.org/docs/stable/index.html).
 
 [Runnable templates](#runnable-templates) published on the [Lightning.AI Platform](https://lightning.ai) are available at the end, **reproducible in 1-click**.
 
 ### Table of Contents
 
 - [Getting started](#getting-started)
     - [Installation](#installation)
```

### Comparing `litdata-0.2.3/src/litdata.egg-info/SOURCES.txt` & `litdata-0.2.4/src/litdata.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,12 +32,13 @@
 src/litdata/streaming/reader.py
 src/litdata/streaming/resolver.py
 src/litdata/streaming/sampler.py
 src/litdata/streaming/serializers.py
 src/litdata/streaming/shuffle.py
 src/litdata/streaming/writer.py
 src/litdata/utilities/__init__.py
+src/litdata/utilities/_pytree.py
 src/litdata/utilities/broadcast.py
 src/litdata/utilities/env.py
 src/litdata/utilities/format.py
 src/litdata/utilities/packing.py
 src/litdata/utilities/shuffle.py
```

