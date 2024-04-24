# Comparing `tmp/REaLTabFormer-0.1.5.tar.gz` & `tmp/REaLTabFormer-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "REaLTabFormer-0.1.5.tar", last modified: Mon Nov 20 03:16:08 2023, max compression
+gzip compressed data, was "REaLTabFormer-0.1.6.tar", last modified: Wed Apr 24 18:17:52 2024, max compression
```

## Comparing `REaLTabFormer-0.1.5.tar` & `REaLTabFormer-0.1.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-11-20 03:16:08.265047 REaLTabFormer-0.1.5/
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-11-20 03:16:08.211890 REaLTabFormer-0.1.5/.github/
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-11-20 03:16:08.221095 REaLTabFormer-0.1.5/.github/workflows/
--rw-r--r--   0 avsolatorio   (501) staff       (20)      777 2023-06-08 18:14:30.000000 REaLTabFormer-0.1.5/.github/workflows/gh-pages.yml
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1856 2023-02-06 02:24:24.000000 REaLTabFormer-0.1.5/.gitignore
--rw-r--r--   0 avsolatorio   (501) staff       (20)     3042 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.5/.pre-commit-config.yaml
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-11-20 03:16:08.221858 REaLTabFormer-0.1.5/.vscode/
--rw-r--r--   0 avsolatorio   (501) staff       (20)      254 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.5/.vscode/settings.json
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1075 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.5/LICENSE
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1263 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.5/Makefile
--rw-r--r--   0 avsolatorio   (501) staff       (20)    11731 2023-11-20 03:16:08.259908 REaLTabFormer-0.1.5/PKG-INFO
--rw-r--r--   0 avsolatorio   (501) staff       (20)     9450 2023-08-07 20:26:33.000000 REaLTabFormer-0.1.5/README.md
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-11-20 03:16:08.222991 REaLTabFormer-0.1.5/colab/
--rw-r--r--   0 avsolatorio   (501) staff       (20)   264453 2023-02-08 20:37:53.000000 REaLTabFormer-0.1.5/colab/REaLTabFormer_GeoValidator_Example.ipynb
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-11-20 03:16:08.225621 REaLTabFormer-0.1.5/devtools/
--rw-r--r--   0 avsolatorio   (501) staff       (20)      723 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.5/devtools/print_env.sh
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-11-20 03:16:08.228515 REaLTabFormer-0.1.5/docs/
--rw-r--r--   0 avsolatorio   (501) staff       (20)      646 2023-06-08 18:14:30.000000 REaLTabFormer-0.1.5/docs/Makefile
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1124 2023-06-08 18:14:30.000000 REaLTabFormer-0.1.5/docs/conf.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)      371 2023-06-08 18:14:30.000000 REaLTabFormer-0.1.5/docs/index.rst
--rw-r--r--   0 avsolatorio   (501) staff       (20)      110 2023-06-08 18:14:30.000000 REaLTabFormer-0.1.5/docs/requirements.txt
--rw-r--r--   0 avsolatorio   (501) staff       (20)      122 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.5/environment.yml
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-11-20 03:16:08.233235 REaLTabFormer-0.1.5/img/
--rw-r--r--   0 avsolatorio   (501) staff       (20)   123234 2023-02-06 22:11:22.000000 REaLTabFormer-0.1.5/img/CA-housing-raw-samples.png
--rw-r--r--   0 avsolatorio   (501) staff       (20)   126314 2023-02-06 22:11:52.000000 REaLTabFormer-0.1.5/img/CA-housing-validated-samples.png
--rw-r--r--   0 avsolatorio   (501) staff       (20)   490438 2023-02-06 19:49:48.000000 REaLTabFormer-0.1.5/img/REalTabFormer_Final_EQ.png
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1392 2023-07-13 15:57:03.000000 REaLTabFormer-0.1.5/pyproject.toml
--rw-r--r--   0 avsolatorio   (501) staff       (20)       38 2023-11-20 03:16:08.265167 REaLTabFormer-0.1.5/setup.cfg
--rw-r--r--   0 avsolatorio   (501) staff       (20)      129 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.5/setup.py
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-11-20 03:16:08.213388 REaLTabFormer-0.1.5/src/
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-11-20 03:16:08.238960 REaLTabFormer-0.1.5/src/REaLTabFormer.egg-info/
--rw-r--r--   0 avsolatorio   (501) staff       (20)    11731 2023-11-20 03:16:08.000000 REaLTabFormer-0.1.5/src/REaLTabFormer.egg-info/PKG-INFO
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1149 2023-11-20 03:16:08.000000 REaLTabFormer-0.1.5/src/REaLTabFormer.egg-info/SOURCES.txt
--rw-r--r--   0 avsolatorio   (501) staff       (20)        1 2023-11-20 03:16:08.000000 REaLTabFormer-0.1.5/src/REaLTabFormer.egg-info/dependency_links.txt
--rw-r--r--   0 avsolatorio   (501) staff       (20)      152 2023-11-20 03:16:08.000000 REaLTabFormer-0.1.5/src/REaLTabFormer.egg-info/requires.txt
--rw-r--r--   0 avsolatorio   (501) staff       (20)       14 2023-11-20 03:16:08.000000 REaLTabFormer-0.1.5/src/REaLTabFormer.egg-info/top_level.txt
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-11-20 03:16:08.252546 REaLTabFormer-0.1.5/src/realtabformer/
--rw-r--r--   0 avsolatorio   (501) staff       (20)        6 2023-11-20 03:08:06.000000 REaLTabFormer-0.1.5/src/realtabformer/VERSION
--rw-r--r--   0 avsolatorio   (501) staff       (20)      504 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.5/src/realtabformer/__init__.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)      272 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.5/src/realtabformer/__main__.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)    24418 2023-08-07 20:25:51.000000 REaLTabFormer-0.1.5/src/realtabformer/data_utils.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)    66865 2023-11-20 03:05:21.000000 REaLTabFormer-0.1.5/src/realtabformer/realtabformer.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)    29164 2023-02-08 20:37:30.000000 REaLTabFormer-0.1.5/src/realtabformer/rtf_analyze.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)     3233 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.5/src/realtabformer/rtf_datacollator.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)      843 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.5/src/realtabformer/rtf_exceptions.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)    41790 2023-11-20 02:58:46.000000 REaLTabFormer-0.1.5/src/realtabformer/rtf_sampler.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)     4201 2023-11-20 03:06:19.000000 REaLTabFormer-0.1.5/src/realtabformer/rtf_trainer.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1960 2023-02-08 20:37:30.000000 REaLTabFormer-0.1.5/src/realtabformer/rtf_validators.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)      297 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.5/test_requirements.txt
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-11-20 03:16:08.213862 REaLTabFormer-0.1.5/tests/
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-11-20 03:16:08.259119 REaLTabFormer-0.1.5/tests/realtabformer/
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1310 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.5/tests/realtabformer/fixtures.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)    10899 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.5/tests/realtabformer/test_data_utils.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)     7648 2023-11-09 02:35:35.000000 REaLTabFormer-0.1.5/tests/realtabformer/test_realtabformer.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1724 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.5/tests/realtabformer/test_rtf_sampler.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)       88 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.5/trufflehog-ignore.txt
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2024-04-24 18:17:52.622421 REaLTabFormer-0.1.6/
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2024-04-24 18:17:52.477226 REaLTabFormer-0.1.6/.github/
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2024-04-24 18:17:52.506146 REaLTabFormer-0.1.6/.github/workflows/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      804 2023-11-20 03:46:16.000000 REaLTabFormer-0.1.6/.github/workflows/gh-pages.yml
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1856 2023-02-06 02:24:24.000000 REaLTabFormer-0.1.6/.gitignore
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     3042 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.6/.pre-commit-config.yaml
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2024-04-24 18:17:52.512901 REaLTabFormer-0.1.6/.vscode/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      254 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.6/.vscode/settings.json
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1075 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.6/LICENSE
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1263 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.6/Makefile
+-rw-r--r--   0 avsolatorio   (501) staff       (20)    11731 2024-04-24 18:17:52.621011 REaLTabFormer-0.1.6/PKG-INFO
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     9450 2023-08-07 20:26:33.000000 REaLTabFormer-0.1.6/README.md
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2024-04-24 18:17:52.515178 REaLTabFormer-0.1.6/colab/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)   264453 2023-02-08 20:37:53.000000 REaLTabFormer-0.1.6/colab/REaLTabFormer_GeoValidator_Example.ipynb
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2024-04-24 18:17:52.520588 REaLTabFormer-0.1.6/devtools/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      723 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.6/devtools/print_env.sh
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2024-04-24 18:17:52.570649 REaLTabFormer-0.1.6/docs/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      646 2023-06-08 18:14:30.000000 REaLTabFormer-0.1.6/docs/Makefile
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1124 2023-06-08 18:14:30.000000 REaLTabFormer-0.1.6/docs/conf.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      371 2023-06-08 18:14:30.000000 REaLTabFormer-0.1.6/docs/index.rst
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      128 2023-11-20 03:54:06.000000 REaLTabFormer-0.1.6/docs/requirements.txt
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      122 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.6/environment.yml
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2024-04-24 18:17:52.581510 REaLTabFormer-0.1.6/img/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)   123234 2023-02-06 22:11:22.000000 REaLTabFormer-0.1.6/img/CA-housing-raw-samples.png
+-rw-r--r--   0 avsolatorio   (501) staff       (20)   126314 2023-02-06 22:11:52.000000 REaLTabFormer-0.1.6/img/CA-housing-validated-samples.png
+-rw-r--r--   0 avsolatorio   (501) staff       (20)   490438 2023-02-06 19:49:48.000000 REaLTabFormer-0.1.6/img/REalTabFormer_Final_EQ.png
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1392 2023-07-13 15:57:03.000000 REaLTabFormer-0.1.6/pyproject.toml
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       38 2024-04-24 18:17:52.622544 REaLTabFormer-0.1.6/setup.cfg
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      129 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.6/setup.py
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2024-04-24 18:17:52.483879 REaLTabFormer-0.1.6/src/
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2024-04-24 18:17:52.618974 REaLTabFormer-0.1.6/src/REaLTabFormer.egg-info/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)    11731 2024-04-24 18:17:52.000000 REaLTabFormer-0.1.6/src/REaLTabFormer.egg-info/PKG-INFO
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1149 2024-04-24 18:17:52.000000 REaLTabFormer-0.1.6/src/REaLTabFormer.egg-info/SOURCES.txt
+-rw-r--r--   0 avsolatorio   (501) staff       (20)        1 2024-04-24 18:17:52.000000 REaLTabFormer-0.1.6/src/REaLTabFormer.egg-info/dependency_links.txt
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      152 2024-04-24 18:17:52.000000 REaLTabFormer-0.1.6/src/REaLTabFormer.egg-info/requires.txt
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       14 2024-04-24 18:17:52.000000 REaLTabFormer-0.1.6/src/REaLTabFormer.egg-info/top_level.txt
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2024-04-24 18:17:52.612739 REaLTabFormer-0.1.6/src/realtabformer/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)        6 2024-04-24 18:13:56.000000 REaLTabFormer-0.1.6/src/realtabformer/VERSION
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      504 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.6/src/realtabformer/__init__.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      272 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.6/src/realtabformer/__main__.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)    24580 2024-04-24 18:13:56.000000 REaLTabFormer-0.1.6/src/realtabformer/data_utils.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)    66865 2023-11-20 03:22:01.000000 REaLTabFormer-0.1.6/src/realtabformer/realtabformer.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)    29164 2023-02-08 20:37:30.000000 REaLTabFormer-0.1.6/src/realtabformer/rtf_analyze.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     3233 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.6/src/realtabformer/rtf_datacollator.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      843 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.6/src/realtabformer/rtf_exceptions.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)    41790 2023-11-20 03:22:01.000000 REaLTabFormer-0.1.6/src/realtabformer/rtf_sampler.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     4201 2023-11-20 03:22:01.000000 REaLTabFormer-0.1.6/src/realtabformer/rtf_trainer.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1960 2023-02-08 20:37:30.000000 REaLTabFormer-0.1.6/src/realtabformer/rtf_validators.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      297 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.6/test_requirements.txt
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2024-04-24 18:17:52.495461 REaLTabFormer-0.1.6/tests/
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2024-04-24 18:17:52.616375 REaLTabFormer-0.1.6/tests/realtabformer/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1310 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.6/tests/realtabformer/fixtures.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)    10899 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.6/tests/realtabformer/test_data_utils.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     7648 2023-11-09 02:35:35.000000 REaLTabFormer-0.1.6/tests/realtabformer/test_realtabformer.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1724 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.6/tests/realtabformer/test_rtf_sampler.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       88 2023-02-06 02:20:56.000000 REaLTabFormer-0.1.6/trufflehog-ignore.txt
```

### Comparing `REaLTabFormer-0.1.5/.github/workflows/gh-pages.yml` & `REaLTabFormer-0.1.6/.github/workflows/gh-pages.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 name: Publish Documentation on GitHub Pages
 
 on:
   push:
     tags:
       - '*'
+    branches:
+      - main
 
 jobs:
   build:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
```

### Comparing `REaLTabFormer-0.1.5/.gitignore` & `REaLTabFormer-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/.pre-commit-config.yaml` & `REaLTabFormer-0.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/LICENSE` & `REaLTabFormer-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/Makefile` & `REaLTabFormer-0.1.6/Makefile`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/PKG-INFO` & `REaLTabFormer-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REaLTabFormer
-Version: 0.1.5
+Version: 0.1.6
 Summary: A novel method for generating tabular and relational data using language models.
 Author-email: "Aivin V. Solatorio" <asolatorio@worldbank.org>
 License: MIT License
         
         Copyright (c) 2022 Aivin V. Solatorio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: REaLTabFormer Version: 0.1.5 Summary: A novel
+Metadata-Version: 2.1 Name: REaLTabFormer Version: 0.1.6 Summary: A novel
 method for generating tabular and relational data using language models.
 Author-email: "Aivin V. Solatorio"
 worldbank.org> License: MIT License Copyright (c) 2022 Aivin V. Solatorio
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `REaLTabFormer-0.1.5/README.md` & `REaLTabFormer-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/colab/REaLTabFormer_GeoValidator_Example.ipynb` & `REaLTabFormer-0.1.6/colab/REaLTabFormer_GeoValidator_Example.ipynb`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/devtools/print_env.sh` & `REaLTabFormer-0.1.6/devtools/print_env.sh`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/docs/Makefile` & `REaLTabFormer-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/docs/conf.py` & `REaLTabFormer-0.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/img/CA-housing-raw-samples.png` & `REaLTabFormer-0.1.6/img/CA-housing-raw-samples.png`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/img/CA-housing-validated-samples.png` & `REaLTabFormer-0.1.6/img/CA-housing-validated-samples.png`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/img/REalTabFormer_Final_EQ.png` & `REaLTabFormer-0.1.6/img/REalTabFormer_Final_EQ.png`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/pyproject.toml` & `REaLTabFormer-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/src/REaLTabFormer.egg-info/PKG-INFO` & `REaLTabFormer-0.1.6/src/REaLTabFormer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REaLTabFormer
-Version: 0.1.5
+Version: 0.1.6
 Summary: A novel method for generating tabular and relational data using language models.
 Author-email: "Aivin V. Solatorio" <asolatorio@worldbank.org>
 License: MIT License
         
         Copyright (c) 2022 Aivin V. Solatorio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: REaLTabFormer Version: 0.1.5 Summary: A novel
+Metadata-Version: 2.1 Name: REaLTabFormer Version: 0.1.6 Summary: A novel
 method for generating tabular and relational data using language models.
 Author-email: "Aivin V. Solatorio"
 worldbank.org> License: MIT License Copyright (c) 2022 Aivin V. Solatorio
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `REaLTabFormer-0.1.5/src/REaLTabFormer.egg-info/SOURCES.txt` & `REaLTabFormer-0.1.6/src/REaLTabFormer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/src/realtabformer/data_utils.py` & `REaLTabFormer-0.1.6/src/realtabformer/data_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,18 +252,27 @@
 
     # Convert the datetimes to
     # their equivalent timestamp values.
 
     # Make sure that we don't convert the NaT
     # to some integer.
     series = series.copy()
-    series.loc[series.notnull()] = (series[series.notnull()].view(int) / 1e9).astype(
-        int
-    )
-    series = series.fillna(pd.NA)
+
+    # Track null values (NaT)
+    null_idx = series.isnull()
+
+    # Convert to the numerical representation
+    # of the datetime (UNIX timestamp)
+    series = (series.astype(int) / 1e9)
+
+    # Fill NA
+    series.loc[null_idx] = pd.NA
+
+    # Cast as integer type
+    series = series.astype("Int64")
 
     # Take the mean value to re-align the data.
     # This will help reduce the scale of the numeric
     # data that will need to be generated. Let's just
     # add this offset back later before casting.
     mean_date = None
```

### Comparing `REaLTabFormer-0.1.5/src/realtabformer/realtabformer.py` & `REaLTabFormer-0.1.6/src/realtabformer/realtabformer.py`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/src/realtabformer/rtf_analyze.py` & `REaLTabFormer-0.1.6/src/realtabformer/rtf_analyze.py`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/src/realtabformer/rtf_datacollator.py` & `REaLTabFormer-0.1.6/src/realtabformer/rtf_datacollator.py`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/src/realtabformer/rtf_exceptions.py` & `REaLTabFormer-0.1.6/src/realtabformer/rtf_exceptions.py`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/src/realtabformer/rtf_sampler.py` & `REaLTabFormer-0.1.6/src/realtabformer/rtf_sampler.py`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/src/realtabformer/rtf_trainer.py` & `REaLTabFormer-0.1.6/src/realtabformer/rtf_trainer.py`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/src/realtabformer/rtf_validators.py` & `REaLTabFormer-0.1.6/src/realtabformer/rtf_validators.py`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/tests/realtabformer/fixtures.py` & `REaLTabFormer-0.1.6/tests/realtabformer/fixtures.py`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/tests/realtabformer/test_data_utils.py` & `REaLTabFormer-0.1.6/tests/realtabformer/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/tests/realtabformer/test_realtabformer.py` & `REaLTabFormer-0.1.6/tests/realtabformer/test_realtabformer.py`

 * *Files identical despite different names*

### Comparing `REaLTabFormer-0.1.5/tests/realtabformer/test_rtf_sampler.py` & `REaLTabFormer-0.1.6/tests/realtabformer/test_rtf_sampler.py`

 * *Files identical despite different names*

