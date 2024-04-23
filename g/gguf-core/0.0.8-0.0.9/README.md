# Comparing `tmp/gguf_core-0.0.8.tar.gz` & `tmp/gguf_core-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gguf_core-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gguf_core-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gguf_core-0.0.8.tar` & `gguf_core-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1095 2024-01-21 23:59:42.278418 gguf_core-0.0.8/LICENSE
--rw-r--r--   0        0        0     1280 2024-02-13 07:48:43.344576 gguf_core-0.0.8/README.md
--rw-r--r--   0        0        0      590 2024-02-11 04:19:27.550011 gguf_core-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    10822 2024-02-13 07:47:28.331736 gguf_core-0.0.8/src/gguf_core/__init__.py
--rw-r--r--   0        0        0      458 2024-02-06 01:55:02.809858 gguf_core-0.0.8/src/gguf_core/data.json
--rw-r--r--   0        0        0      742 2024-01-08 04:10:18.194979 gguf_core-0.0.8/src/gguf_core/logo.png
--rw-r--r--   0        0        0     1646 1970-01-01 00:00:00.000000 gguf_core-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-01-21 23:59:42.278418 gguf_core-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1335 2024-02-13 23:27:09.275433 gguf_core-0.0.9/README.md
+-rw-r--r--   0        0        0      590 2024-02-11 04:19:27.550011 gguf_core-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    10822 2024-02-13 23:28:13.392380 gguf_core-0.0.9/src/gguf_core/__init__.py
+-rw-r--r--   0        0        0      458 2024-02-06 01:55:02.809858 gguf_core-0.0.9/src/gguf_core/data.json
+-rw-r--r--   0        0        0      742 2024-01-08 04:10:18.194979 gguf_core-0.0.9/src/gguf_core/logo.png
+-rw-r--r--   0        0        0     1700 1970-01-01 00:00:00.000000 gguf_core-0.0.9/PKG-INFO
```

### Comparing `gguf_core-0.0.8/LICENSE` & `gguf_core-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gguf_core-0.0.8/README.md` & `gguf_core-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -42,8 +42,9 @@
 You can now load your PDF file(s) straight into the model for generating digested summary; try it out by:
 ```
 gguf p
 ```
 #### webpage (alpha)
 ```
 https://gguf.us
-```
+```
+Paste it (gguf.us) to browser instead of cmd console.
```

### Comparing `gguf_core-0.0.8/pyproject.toml` & `gguf_core-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gguf_core-0.0.8/src/gguf_core/__init__.py` & `gguf_core-0.0.9/src/gguf_core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # !/usr/bin/env python3
 
-__version__="0.0.8"
+__version__="0.0.9"
 
 import argparse, json, os.path, urllib.request
 from tqdm import tqdm
 from tkinter import *
 
 def pdf_handler(llm):
     import os
```

### Comparing `gguf_core-0.0.8/src/gguf_core/logo.png` & `gguf_core-0.0.9/src/gguf_core/logo.png`

 * *Files identical despite different names*

### Comparing `gguf_core-0.0.8/PKG-INFO` & `gguf_core-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gguf-core
-Version: 0.0.8
+Version: 0.0.9
 Summary: a simple way to interact llama with gguf
 Author-email: calcuis <calculatics@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: llama-core
 Requires-Dist: pypdf
 Project-URL: Homepage, https://github.com/calcuis/gguf-core
@@ -55,7 +55,8 @@
 ```
 gguf p
 ```
 #### webpage (alpha)
 ```
 https://gguf.us
 ```
+Paste it (gguf.us) to browser instead of cmd console.
```

