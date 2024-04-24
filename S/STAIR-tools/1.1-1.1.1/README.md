# Comparing `tmp/STAIR-tools-1.1.tar.gz` & `tmp/STAIR-tools-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STAIR-tools-1.1.tar", last modified: Sat Dec 23 14:27:55 2023, max compression
+gzip compressed data, was "STAIR-tools-1.1.1.tar", last modified: Wed Apr 24 13:14:22 2024, max compression
```

## Comparing `STAIR-tools-1.1.tar` & `STAIR-tools-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2023-12-23 14:27:55.561057 STAIR-tools-1.1/
--rw-r--r--   0 yuanyuan   (501) staff       (20)      251 2023-12-23 14:27:55.560868 STAIR-tools-1.1/PKG-INFO
--rw-------   0 yuanyuan   (501) staff       (20)       91 2023-12-23 14:27:27.000000 STAIR-tools-1.1/README.md
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2023-12-23 14:27:55.559982 STAIR-tools-1.1/STAIR/
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8661 2023-12-23 11:23:09.000000 STAIR-tools-1.1/STAIR/ABA_annotation.py
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1/STAIR/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    18469 2023-12-23 11:23:09.000000 STAIR-tools-1.1/STAIR/emb_alignment.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12304 2023-12-23 11:23:12.000000 STAIR-tools-1.1/STAIR/loc_alignment.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    14182 2023-12-23 11:23:11.000000 STAIR-tools-1.1/STAIR/loc_prediction.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)      174 2023-12-23 11:23:13.000000 STAIR-tools-1.1/STAIR/test.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2821 2023-12-23 11:23:13.000000 STAIR-tools-1.1/STAIR/utils.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2023-12-23 14:27:55.560656 STAIR-tools-1.1/STAIR_tools.egg-info/
--rw-r--r--   0 yuanyuan   (501) staff       (20)      251 2023-12-23 14:27:55.000000 STAIR-tools-1.1/STAIR_tools.egg-info/PKG-INFO
--rw-r--r--   0 yuanyuan   (501) staff       (20)      299 2023-12-23 14:27:55.000000 STAIR-tools-1.1/STAIR_tools.egg-info/SOURCES.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)        1 2023-12-23 14:27:55.000000 STAIR-tools-1.1/STAIR_tools.egg-info/dependency_links.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)        6 2023-12-23 14:27:55.000000 STAIR-tools-1.1/STAIR_tools.egg-info/top_level.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)       38 2023-12-23 14:27:55.561137 STAIR-tools-1.1/setup.cfg
--rw-------   0 yuanyuan   (501) staff       (20)      315 2023-12-23 14:27:11.000000 STAIR-tools-1.1/setup.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-24 13:14:22.369000 STAIR-tools-1.1.1/
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      173 2024-04-24 13:14:22.368776 STAIR-tools-1.1.1/PKG-INFO
+-rwxr-xr-x   0 yuanyuan   (501) staff       (20)     1320 2023-12-25 02:00:08.000000 STAIR-tools-1.1.1/README.md
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-24 13:14:22.362587 STAIR-tools-1.1.1/STAIR/
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8661 2023-12-23 11:23:09.000000 STAIR-tools-1.1.1/STAIR/ABA_annotation.py
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1.1/STAIR/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    18463 2024-04-24 10:10:43.000000 STAIR-tools-1.1.1/STAIR/emb_alignment.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12304 2023-12-23 11:23:12.000000 STAIR-tools-1.1.1/STAIR/loc_alignment.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    14182 2023-12-23 11:23:11.000000 STAIR-tools-1.1.1/STAIR/loc_prediction.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)      174 2023-12-23 11:23:13.000000 STAIR-tools-1.1.1/STAIR/test.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2821 2023-12-23 11:23:13.000000 STAIR-tools-1.1.1/STAIR/utils.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-24 13:14:22.368563 STAIR-tools-1.1.1/STAIR_tools.egg-info/
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      173 2024-04-24 13:14:22.000000 STAIR-tools-1.1.1/STAIR_tools.egg-info/PKG-INFO
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      299 2024-04-24 13:14:22.000000 STAIR-tools-1.1.1/STAIR_tools.egg-info/SOURCES.txt
+-rw-------   0 yuanyuan   (501) staff       (20)        1 2024-04-24 13:14:22.000000 STAIR-tools-1.1.1/STAIR_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)        6 2024-04-24 13:14:22.000000 STAIR-tools-1.1.1/STAIR_tools.egg-info/top_level.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)       38 2024-04-24 13:14:22.369058 STAIR-tools-1.1.1/setup.cfg
+-rw-------   0 yuanyuan   (501) staff       (20)      317 2024-04-24 10:17:33.000000 STAIR-tools-1.1.1/setup.py
```

### Comparing `STAIR-tools-1.1/STAIR/ABA_annotation.py` & `STAIR-tools-1.1.1/STAIR/ABA_annotation.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1/STAIR/emb_alignment.py` & `STAIR-tools-1.1.1/STAIR/emb_alignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from tqdm import tqdm
 import matplotlib.pyplot as plt
 
 import torch
 from torch.utils.data import DataLoader
 import torch.nn.functional as F
 
-from .embedding.module_ae import ae_dict
-from .embedding.module_hgat import HGAT
-from .embedding.dataset_ae import MyDataset
-from .embedding.dataset_hgat import hgat_data
-from .embedding.loss import nll_loss
+from embedding.module_ae import ae_dict
+from embedding.module_hgat import HGAT
+from embedding.dataset_ae import MyDataset
+from embedding.dataset_hgat import hgat_data
+from embedding.loss import nll_loss
 
-from .utils import MakeLogClass
+from utils import MakeLogClass
 
 
 class Emb_Align(object):
 
     """
     
     Spatial embedding alignment of multiplt ST slices, including CE alignment and SE alignment.
```

### Comparing `STAIR-tools-1.1/STAIR/loc_alignment.py` & `STAIR-tools-1.1.1/STAIR/loc_alignment.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1/STAIR/loc_prediction.py` & `STAIR-tools-1.1.1/STAIR/loc_prediction.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1/STAIR/utils.py` & `STAIR-tools-1.1.1/STAIR/utils.py`

 * *Files identical despite different names*

