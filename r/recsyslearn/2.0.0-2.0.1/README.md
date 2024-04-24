# Comparing `tmp/recsyslearn-2.0.0.tar.gz` & `tmp/recsyslearn-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recsyslearn-2.0.0.tar", last modified: Wed Dec 20 16:41:25 2023, max compression
+gzip compressed data, was "recsyslearn-2.0.1.tar", last modified: Wed Apr 24 10:28:22 2024, max compression
```

## Comparing `recsyslearn-2.0.0.tar` & `recsyslearn-2.0.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 16:41:25.834183 recsyslearn-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2023-12-20 16:41:25.834183 recsyslearn-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 16:41:25.826183 recsyslearn-2.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/docs/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 16:41:25.826183 recsyslearn-2.0.0/docs/api_ref/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/docs/api_ref/dataset.rst
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/docs/api_ref/errors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      253 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/docs/api_ref/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      332 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/docs/api_ref/metrics.rst
--rw-r--r--   0 runner    (1001) docker     (127)      440 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 16:41:25.830183 recsyslearn-2.0.0/docs/user/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/docs/user/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/docs/user/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/docs/user/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 16:41:25.830183 recsyslearn-2.0.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 16:41:25.830183 recsyslearn-2.0.0/examples/__assets__/
--rw-r--r--   0 runner    (1001) docker     (127)    11215 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/examples/__assets__/test_dataset.csv
--rw-r--r--   0 runner    (1001) docker     (127)    92496 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/examples/__assets__/top_k.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1156793 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/examples/__assets__/train_dataset.csv
--rw-r--r--   0 runner    (1001) docker     (127)      456 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/examples/accuracy_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/examples/beyond_accuracy_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/examples/fairness_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/examples/segmentations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 16:41:25.830183 recsyslearn-2.0.0/recsyslearn/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/recsyslearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 16:41:25.834183 recsyslearn-2.0.0/recsyslearn/accuracy/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/recsyslearn/accuracy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/recsyslearn/accuracy/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 16:41:25.834183 recsyslearn-2.0.0/recsyslearn/beyond_accuracy/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/recsyslearn/beyond_accuracy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/recsyslearn/beyond_accuracy/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 16:41:25.834183 recsyslearn-2.0.0/recsyslearn/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/recsyslearn/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8525 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/recsyslearn/dataset/segmentations.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/recsyslearn/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 16:41:25.834183 recsyslearn-2.0.0/recsyslearn/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/recsyslearn/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/recsyslearn/errors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 16:41:25.834183 recsyslearn-2.0.0/recsyslearn/fairness/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/recsyslearn/fairness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/recsyslearn/fairness/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/recsyslearn/fairness/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/recsyslearn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 16:41:25.834183 recsyslearn-2.0.0/recsyslearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2023-12-20 16:41:25.000000 recsyslearn-2.0.0/recsyslearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2023-12-20 16:41:25.000000 recsyslearn-2.0.0/recsyslearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 16:41:25.000000 recsyslearn-2.0.0/recsyslearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 16:41:25.000000 recsyslearn-2.0.0/recsyslearn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-20 16:41:25.000000 recsyslearn-2.0.0/recsyslearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-20 16:41:25.000000 recsyslearn-2.0.0/recsyslearn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      491 2023-12-20 16:41:25.834183 recsyslearn-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 16:41:25.834183 recsyslearn-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/tests/test_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/tests/test_beyond_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/tests/test_fairness.py
--rw-r--r--   0 runner    (1001) docker     (127)     8955 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/tests/test_segmentations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11407 2023-12-20 16:41:15.000000 recsyslearn-2.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:28:22.529186 recsyslearn-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-24 10:28:22.529186 recsyslearn-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:28:22.521186 recsyslearn-2.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/docs/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:28:22.521186 recsyslearn-2.0.1/docs/api_ref/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/docs/api_ref/dataset.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/docs/api_ref/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/docs/api_ref/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/docs/api_ref/metrics.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:28:22.521186 recsyslearn-2.0.1/docs/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/docs/user/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/docs/user/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/docs/user/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:28:22.521186 recsyslearn-2.0.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:28:22.525186 recsyslearn-2.0.1/examples/__assets__/
+-rw-r--r--   0 runner    (1001) docker     (127)    11215 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/examples/__assets__/test_dataset.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    92496 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/examples/__assets__/top_k.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1156793 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/examples/__assets__/train_dataset.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/examples/accuracy_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/examples/beyond_accuracy_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/examples/fairness_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/examples/segmentations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:28:22.525186 recsyslearn-2.0.1/recsyslearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/recsyslearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:28:22.525186 recsyslearn-2.0.1/recsyslearn/accuracy/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/recsyslearn/accuracy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/recsyslearn/accuracy/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:28:22.525186 recsyslearn-2.0.1/recsyslearn/beyond_accuracy/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/recsyslearn/beyond_accuracy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/recsyslearn/beyond_accuracy/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:28:22.529186 recsyslearn-2.0.1/recsyslearn/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/recsyslearn/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8525 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/recsyslearn/dataset/segmentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/recsyslearn/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:28:22.529186 recsyslearn-2.0.1/recsyslearn/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/recsyslearn/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/recsyslearn/errors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:28:22.529186 recsyslearn-2.0.1/recsyslearn/fairness/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/recsyslearn/fairness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/recsyslearn/fairness/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/recsyslearn/fairness/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/recsyslearn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:28:22.529186 recsyslearn-2.0.1/recsyslearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-24 10:28:22.000000 recsyslearn-2.0.1/recsyslearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-24 10:28:22.000000 recsyslearn-2.0.1/recsyslearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:28:22.000000 recsyslearn-2.0.1/recsyslearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:28:22.000000 recsyslearn-2.0.1/recsyslearn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 10:28:22.000000 recsyslearn-2.0.1/recsyslearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 10:28:22.000000 recsyslearn-2.0.1/recsyslearn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-24 10:28:22.529186 recsyslearn-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:28:22.529186 recsyslearn-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/tests/test_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/tests/test_beyond_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/tests/test_fairness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/tests/test_segmentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11407 2024-04-24 10:28:16.000000 recsyslearn-2.0.1/tests/test_utils.py
```

### Comparing `recsyslearn-2.0.0/LICENSE` & `recsyslearn-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/PKG-INFO` & `recsyslearn-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recsyslearn
-Version: 2.0.0
+Version: 2.0.1
 Summary: A library to compute fairness of recommender systems.
 Home-page: https://github.com/giuliowaitforitdavide/recsyslearn
 Author: Giulio Davide Carparelli
 Author-email: giulio.davide.97@gmail.com
 License: GNU General Public License v3
 Keywords: recsyslearn
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `recsyslearn-2.0.0/README.rst` & `recsyslearn-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/docs/.DS_Store` & `recsyslearn-2.0.1/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/docs/Makefile` & `recsyslearn-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/docs/make.bat` & `recsyslearn-2.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/docs/requirements.txt` & `recsyslearn-2.0.1/docs/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 alabaster==0.7.13
 Babel==2.13.1
 certifi==2023.11.17
 charset-normalizer==3.3.2
 docutils==0.18.1
 idna==3.6
 imagesize==1.4.1
-Jinja2==3.1.2
+Jinja2==3.1.3
 MarkupSafe==2.1.3
 numpy==1.26.2
 packaging==23.2
 pandas==2.1.3
 Pygments==2.17.2
 python-dateutil==2.8.2
 pytz==2023.3.post1
```

### Comparing `recsyslearn-2.0.0/docs/user/install.rst` & `recsyslearn-2.0.1/docs/user/install.rst`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/docs/user/quickstart.rst` & `recsyslearn-2.0.1/docs/user/quickstart.rst`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/examples/__assets__/test_dataset.csv` & `recsyslearn-2.0.1/examples/__assets__/test_dataset.csv`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/examples/__assets__/top_k.csv` & `recsyslearn-2.0.1/examples/__assets__/top_k.csv`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/examples/__assets__/train_dataset.csv` & `recsyslearn-2.0.1/examples/__assets__/train_dataset.csv`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/examples/beyond_accuracy_evaluation.py` & `recsyslearn-2.0.1/examples/beyond_accuracy_evaluation.py`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/examples/fairness_evaluation.py` & `recsyslearn-2.0.1/examples/fairness_evaluation.py`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/examples/segmentations.py` & `recsyslearn-2.0.1/examples/segmentations.py`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/recsyslearn/accuracy/metrics.py` & `recsyslearn-2.0.1/recsyslearn/accuracy/metrics.py`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/recsyslearn/beyond_accuracy/metrics.py` & `recsyslearn-2.0.1/recsyslearn/beyond_accuracy/metrics.py`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/recsyslearn/dataset/segmentations.py` & `recsyslearn-2.0.1/recsyslearn/dataset/segmentations.py`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/recsyslearn/dataset/utils.py` & `recsyslearn-2.0.1/recsyslearn/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/recsyslearn/errors/errors.py` & `recsyslearn-2.0.1/recsyslearn/errors/errors.py`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/recsyslearn/fairness/metrics.py` & `recsyslearn-2.0.1/recsyslearn/fairness/metrics.py`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/recsyslearn/fairness/utils.py` & `recsyslearn-2.0.1/recsyslearn/fairness/utils.py`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/recsyslearn/utils.py` & `recsyslearn-2.0.1/recsyslearn/utils.py`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/recsyslearn.egg-info/PKG-INFO` & `recsyslearn-2.0.1/recsyslearn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recsyslearn
-Version: 2.0.0
+Version: 2.0.1
 Summary: A library to compute fairness of recommender systems.
 Home-page: https://github.com/giuliowaitforitdavide/recsyslearn
 Author: Giulio Davide Carparelli
 Author-email: giulio.davide.97@gmail.com
 License: GNU General Public License v3
 Keywords: recsyslearn
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `recsyslearn-2.0.0/recsyslearn.egg-info/SOURCES.txt` & `recsyslearn-2.0.1/recsyslearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/setup.py` & `recsyslearn-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,10 +29,10 @@
     include_package_data=True,
     keywords="recsyslearn",
     name="recsyslearn",
     packages=find_packages(include=["recsyslearn", "recsyslearn.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/giuliowaitforitdavide/recsyslearn",
-    version="2.0.0",
+    version="2.0.1",
     zip_safe=False,
 )
```

### Comparing `recsyslearn-2.0.0/tests/test_accuracy.py` & `recsyslearn-2.0.1/tests/test_accuracy.py`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/tests/test_beyond_accuracy.py` & `recsyslearn-2.0.1/tests/test_beyond_accuracy.py`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/tests/test_errors.py` & `recsyslearn-2.0.1/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/tests/test_fairness.py` & `recsyslearn-2.0.1/tests/test_fairness.py`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/tests/test_segmentations.py` & `recsyslearn-2.0.1/tests/test_segmentations.py`

 * *Files identical despite different names*

### Comparing `recsyslearn-2.0.0/tests/test_utils.py` & `recsyslearn-2.0.1/tests/test_utils.py`

 * *Files identical despite different names*

