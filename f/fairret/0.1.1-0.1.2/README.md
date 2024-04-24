# Comparing `tmp/fairret-0.1.1.tar.gz` & `tmp/fairret-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairret-0.1.1.tar", last modified: Tue Apr 23 16:02:20 2024, max compression
+gzip compressed data, was "fairret-0.1.2.tar", last modified: Wed Apr 24 14:48:24 2024, max compression
```

## Comparing `fairret-0.1.1.tar` & `fairret-0.1.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.201058 fairret-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.189058 fairret-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.193059 fairret-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-23 16:02:14.000000 fairret-0.1.1/.github/workflows/pypi_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-23 16:02:14.000000 fairret-0.1.1/.github/workflows/sphinx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-23 16:02:14.000000 fairret-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-23 16:02:14.000000 fairret-0.1.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-23 16:02:14.000000 fairret-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-23 16:02:20.201058 fairret-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-23 16:02:14.000000 fairret-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.193059 fairret-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-23 16:02:14.000000 fairret-0.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-23 16:02:14.000000 fairret-0.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 16:02:14.000000 fairret-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.193059 fairret-0.1.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.193059 fairret-0.1.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    39520 2024-04-23 16:02:14.000000 fairret-0.1.1/docs/source/_static/Overview_fairret.png
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-23 16:02:14.000000 fairret-0.1.1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.193059 fairret-0.1.1/docs/source/generated/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-23 16:02:14.000000 fairret-0.1.1/docs/source/generated/fairret.loss.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-23 16:02:14.000000 fairret-0.1.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-23 16:02:14.000000 fairret-0.1.1/docs/source/loss.rst
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-23 16:02:14.000000 fairret-0.1.1/docs/source/metric.rst
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-23 16:02:14.000000 fairret-0.1.1/docs/source/statistic.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.197059 fairret-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    88620 2024-04-23 16:02:14.000000 fairret-0.1.1/examples/complex_sensitive_features.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    17921 2024-04-23 16:02:14.000000 fairret-0.1.1/examples/custom_statistic.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    28213 2024-04-23 16:02:14.000000 fairret-0.1.1/examples/simple_pipeline.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    16306 2024-04-23 16:02:14.000000 fairret-0.1.1/examples/stacked_statistic.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.197059 fairret-0.1.1/fairret/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:14.000000 fairret-0.1.1/fairret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.197059 fairret-0.1.1/fairret/loss/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-23 16:02:14.000000 fairret-0.1.1/fairret/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-23 16:02:14.000000 fairret-0.1.1/fairret/loss/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17905 2024-04-23 16:02:14.000000 fairret-0.1.1/fairret/loss/projection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-04-23 16:02:14.000000 fairret-0.1.1/fairret/loss/violation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-23 16:02:14.000000 fairret-0.1.1/fairret/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.197059 fairret-0.1.1/fairret/statistic/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-23 16:02:14.000000 fairret-0.1.1/fairret/statistic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-23 16:02:14.000000 fairret-0.1.1/fairret/statistic/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    22496 2024-04-23 16:02:14.000000 fairret-0.1.1/fairret/statistic/linear_fractional.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-23 16:02:14.000000 fairret-0.1.1/fairret/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.201058 fairret-0.1.1/fairret.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-23 16:02:20.000000 fairret-0.1.1/fairret.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-23 16:02:20.000000 fairret-0.1.1/fairret.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:02:20.000000 fairret-0.1.1/fairret.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 16:02:20.000000 fairret-0.1.1/fairret.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 16:02:20.000000 fairret-0.1.1/fairret.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-23 16:02:14.000000 fairret-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:02:20.201058 fairret-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:02:20.201058 fairret-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-23 16:02:14.000000 fairret-0.1.1/test/test_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-23 16:02:14.000000 fairret-0.1.1/test/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-23 16:02:14.000000 fairret-0.1.1/test/test_statistic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.010423 fairret-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:23.998423 fairret-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.002423 fairret-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-24 14:48:19.000000 fairret-0.1.2/.github/workflows/pypi_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-24 14:48:19.000000 fairret-0.1.2/.github/workflows/sphinx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-24 14:48:19.000000 fairret-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-24 14:48:19.000000 fairret-0.1.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-24 14:48:19.000000 fairret-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-24 14:48:24.010423 fairret-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-24 14:48:19.000000 fairret-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.002423 fairret-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-24 14:48:19.000000 fairret-0.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-24 14:48:19.000000 fairret-0.1.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 14:48:19.000000 fairret-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.002423 fairret-0.1.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.006423 fairret-0.1.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    39520 2024-04-24 14:48:19.000000 fairret-0.1.2/docs/source/_static/Overview_fairret.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-24 14:48:19.000000 fairret-0.1.2/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.006423 fairret-0.1.2/docs/source/generated/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-24 14:48:19.000000 fairret-0.1.2/docs/source/generated/fairret.loss.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-24 14:48:19.000000 fairret-0.1.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-24 14:48:19.000000 fairret-0.1.2/docs/source/loss.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-24 14:48:19.000000 fairret-0.1.2/docs/source/metric.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-24 14:48:19.000000 fairret-0.1.2/docs/source/statistic.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.006423 fairret-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    88620 2024-04-24 14:48:19.000000 fairret-0.1.2/examples/complex_sensitive_features.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    17921 2024-04-24 14:48:19.000000 fairret-0.1.2/examples/custom_statistic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    28213 2024-04-24 14:48:19.000000 fairret-0.1.2/examples/simple_pipeline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16306 2024-04-24 14:48:19.000000 fairret-0.1.2/examples/stacked_statistic.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.006423 fairret-0.1.2/fairret/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:19.000000 fairret-0.1.2/fairret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.006423 fairret-0.1.2/fairret/loss/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-24 14:48:19.000000 fairret-0.1.2/fairret/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-24 14:48:19.000000 fairret-0.1.2/fairret/loss/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17955 2024-04-24 14:48:19.000000 fairret-0.1.2/fairret/loss/projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-24 14:48:19.000000 fairret-0.1.2/fairret/loss/violation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-24 14:48:19.000000 fairret-0.1.2/fairret/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.010423 fairret-0.1.2/fairret/statistic/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-24 14:48:19.000000 fairret-0.1.2/fairret/statistic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-24 14:48:19.000000 fairret-0.1.2/fairret/statistic/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26353 2024-04-24 14:48:19.000000 fairret-0.1.2/fairret/statistic/linear_fractional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-24 14:48:19.000000 fairret-0.1.2/fairret/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.010423 fairret-0.1.2/fairret.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-24 14:48:23.000000 fairret-0.1.2/fairret.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-24 14:48:23.000000 fairret-0.1.2/fairret.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:48:23.000000 fairret-0.1.2/fairret.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 14:48:23.000000 fairret-0.1.2/fairret.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 14:48:23.000000 fairret-0.1.2/fairret.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-24 14:48:19.000000 fairret-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:48:24.010423 fairret-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:48:24.010423 fairret-0.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-24 14:48:19.000000 fairret-0.1.2/test/test_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-24 14:48:19.000000 fairret-0.1.2/test/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-24 14:48:19.000000 fairret-0.1.2/test/test_statistic.py
```

### Comparing `fairret-0.1.1/.github/workflows/pypi_release.yml` & `fairret-0.1.2/.github/workflows/pypi_release.yml`

 * *Files identical despite different names*

### Comparing `fairret-0.1.1/.github/workflows/sphinx.yml` & `fairret-0.1.2/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `fairret-0.1.1/.gitignore` & `fairret-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fairret-0.1.1/CITATION.cff` & `fairret-0.1.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `fairret-0.1.1/LICENSE` & `fairret-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fairret-0.1.1/PKG-INFO` & `fairret-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairret
-Version: 0.1.1
+Version: 0.1.2
 Summary: A fairness library in PyTorch.
 Author-email: Maarten Buyl <maarten.buyl@ugent.be>, MaryBeth Defrance <marybeth.defrance@ugent.be>
 License: MIT License
         
         Copyright (c) 2024 Ghent University Artificial Intelligence & Data Analytics Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -45,25 +45,24 @@
 1. *flexible* in how fairness is defined and pursued.
 2. *easy* to integrate into existing PyTorch pipelines.
 3. *clear* in what its tools can and cannot do.
 
 The central to the library is the paradigm of the _fairness regularization term_ (fairrets) that quantify unfairness as differentiable PyTorch loss functions. 
 These can then be optimized together with e.g. the binary cross-entropy error such that the classifier improves both its accuracy and fairness.
 
-**The library is still in very early development.** Documentation, installation instructions, and more examples will be added in the near future.
-
 ## Installation
 The fairret library can be installed via PyPi:
 
 ```
 pip install fairret
 ```
 
-### Dependencies
-A minimal list of dependencies is provided in [pyproject.toml](https://github.com/aida-ugent/fairret/blob/main/pyproject.toml). If the library is installed locally, the required packages can be installed via `pip install .`
+A minimal list of dependencies is provided in [pyproject.toml](https://github.com/aida-ugent/fairret/blob/main/pyproject.toml). 
+
+If the library is installed locally, the required packages can be installed via `pip install .`
 
 ## Quickstart
 
 It suffices to simply choose a statistic that should be equalized across groups and a fairret that quantifies the gap. The model can then be trained as follows:
 
 ```python
 import torch.nn.functional as F
```

### Comparing `fairret-0.1.1/README.md` & `fairret-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,24 @@
 1. *flexible* in how fairness is defined and pursued.
 2. *easy* to integrate into existing PyTorch pipelines.
 3. *clear* in what its tools can and cannot do.
 
 The central to the library is the paradigm of the _fairness regularization term_ (fairrets) that quantify unfairness as differentiable PyTorch loss functions. 
 These can then be optimized together with e.g. the binary cross-entropy error such that the classifier improves both its accuracy and fairness.
 
-**The library is still in very early development.** Documentation, installation instructions, and more examples will be added in the near future.
-
 ## Installation
 The fairret library can be installed via PyPi:
 
 ```
 pip install fairret
 ```
 
-### Dependencies
-A minimal list of dependencies is provided in [pyproject.toml](https://github.com/aida-ugent/fairret/blob/main/pyproject.toml). If the library is installed locally, the required packages can be installed via `pip install .`
+A minimal list of dependencies is provided in [pyproject.toml](https://github.com/aida-ugent/fairret/blob/main/pyproject.toml). 
+
+If the library is installed locally, the required packages can be installed via `pip install .`
 
 ## Quickstart
 
 It suffices to simply choose a statistic that should be equalized across groups and a fairret that quantifies the gap. The model can then be trained as follows:
 
 ```python
 import torch.nn.functional as F
```

### Comparing `fairret-0.1.1/docs/Makefile` & `fairret-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fairret-0.1.1/docs/make.bat` & `fairret-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fairret-0.1.1/docs/source/_static/Overview_fairret.png` & `fairret-0.1.2/docs/source/_static/Overview_fairret.png`

 * *Files identical despite different names*

### Comparing `fairret-0.1.1/docs/source/conf.py` & `fairret-0.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fairret-0.1.1/docs/source/index.rst` & `fairret-0.1.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `fairret-0.1.1/examples/complex_sensitive_features.ipynb` & `fairret-0.1.2/examples/complex_sensitive_features.ipynb`

 * *Files identical despite different names*

### Comparing `fairret-0.1.1/examples/custom_statistic.ipynb` & `fairret-0.1.2/examples/custom_statistic.ipynb`

 * *Files identical despite different names*

### Comparing `fairret-0.1.1/examples/simple_pipeline.ipynb` & `fairret-0.1.2/examples/simple_pipeline.ipynb`

 * *Files identical despite different names*

### Comparing `fairret-0.1.1/examples/stacked_statistic.ipynb` & `fairret-0.1.2/examples/stacked_statistic.ipynb`

 * *Files identical despite different names*

### Comparing `fairret-0.1.1/fairret/loss/base.py` & `fairret-0.1.2/fairret/loss/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,17 +14,17 @@
         """
         Abstract method that should be implemented by subclasses to calculate the loss.
         
         Args:
             pred (torch.Tensor): Predictions of shape :math:`(N, 1)`, as we assume to be performing binary
                 classification or regression.
             sens (torch.Tensor): Sensitive features of shape :math:`(N, S)` with `S` the number of sensitive features.
-            *stat_args: Any further arguments used to compute the statistic.
+            *stat_args: All arguments used by the statistic that this loss minimizes.
             pred_as_logit (bool): Whether the `pred` tensor should be interpreted as logits. Though most losses are
                 will simply take the sigmoid of `pred` if `pred_as_logit` is `True`, some losses benefit from improved
                 numerical stability if they handle the conversion themselves.
-            **stat_kwargs: Any keyword arguments used to compute the statistic.
+            **stat_kwargs: All keyword arguments used by the statistic that this loss computes.
 
         Returns:
             torch.Tensor: The calculated loss as a scalar tensor.
         """
         raise NotImplementedError
```

### Comparing `fairret-0.1.1/fairret/loss/projection.py` & `fairret-0.1.2/fairret/loss/projection.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,19 +153,19 @@
         Calculate the fairness loss by projecting the predictions onto the fair set and computing the statistical
         distance between the predictions and the projection.
 
         Args:
             pred (torch.Tensor): Predictions of shape :math:`(N, 1)`, as we assume to be performing binary
                 classification or regression.
             sens (torch.Tensor): Sensitive features of shape :math:`(N, S)` with `S` the number of sensitive features.
-            *stat_args: Any further arguments used to compute the statistic.
+            *stat_args: All arguments used by the statistic that this loss minimizes.
             pred_as_logit (bool): Whether the `pred` tensor should be interpreted as logits. Though most losses are
                 will simply take the sigmoid of `pred` if `pred_as_logit` is `True`, some losses benefit from improved
                 numerical stability if they handle the conversion themselves.
-            **stat_kwargs: Any keyword arguments used to compute the statistic.
+            **stat_kwargs: All keyword arguments used by the statistic that this loss computes.
 
         Returns:
             torch.Tensor: The calculated loss as a scalar tensor.
         """
 
         if pred_as_logit:
             prob_pred = torch.sigmoid(pred)
@@ -230,16 +230,16 @@
         Iterate over the cvxpy problem to find the projection of the predictions onto the fair set.
 
         Args:
             pred (torch.Tensor): Predictions of shape :math:`(N, 2)`. The predicted distribution in shape (N,2). As we
                 assume binary classification, the first column is the probability of the negative class and the second
                 column is the probability of the positive class.
             sens (torch.Tensor): Sensitive features of shape :math:`(N, S)` with `S` the number of sensitive features.
-            *stat_args: Any further arguments used to compute the statistic.
-            **stat_kwargs: Any keyword arguments used to compute the statistic.
+            *stat_args: All arguments used by the statistic that this loss minimizes.
+            **stat_kwargs: All keyword arguments used by the statistic that this loss computes.
 
         Returns:
             torch.Tensor: The projection of the predictions onto the fair set in the shape (N, 2).
         """
 
         pred = pred.detach()
```

### Comparing `fairret-0.1.1/fairret/loss/violation.py` & `fairret-0.1.2/fairret/loss/violation.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,21 +45,21 @@
         Calculate the violation vector in relation to the `target_statistic` and penalize this violation using the
         :func:`~violation.ViolationLoss.penalize_violation` method implemented by the subclass.
 
         Args:
             pred (torch.Tensor): Predictions of shape :math:`(N, 1)`, as we assume to be performing binary
                 classification or regression.
             sens (torch.Tensor): Sensitive features of shape :math:`(N, S)` with `S` the number of sensitive features.
-            *stat_args: Any further arguments used to compute the statistic.
+            *stat_args: All arguments used by the statistic that this loss minimizes.
             pred_as_logit (bool): Whether the `pred` tensor should be interpreted as logits. Though most losses are
                 will simply take the sigmoid of `pred` if `pred_as_logit` is `True`, some losses benefit from improved
                 numerical stability if they handle the conversion themselves.
             target_statistic (Optional[torch.Tensor]): The target statistic as a scalar tensor. If not provided for a
                 LinearFractionalStatistic, the overall statistic will be used by default.
-            **stat_kwargs: Any keyword arguments used to compute the statistic.
+            **stat_kwargs: All keyword arguments used by the statistic that this loss computes.
 
         Returns:
             torch.Tensor: The calculated loss as a scalar tensor.
         """
 
         if pred_as_logit:
             pred = torch.sigmoid(pred)
```

### Comparing `fairret-0.1.1/fairret/metric.py` & `fairret-0.1.2/fairret/metric.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,16 +99,16 @@
         Update the running sums for the numerator and denominator of the groupwise and overall statistics with a new
         batch of predictions and sensitive features.
 
         Args:
             pred (torch.Tensor): Predictions of shape :math:`(N, 1)`, as we assume to be performing binary
                 classification or regression.
             sens (torch.Tensor): Sensitive features of shape :math:`(N, S)` with `S` the number of sensitive features.
-            *stat_args: Any further arguments used to compute the statistic.
-            **stat_kwargs: Any keyword arguments used to compute the statistic.
+            *stat_args: All arguments used by the statistic that this metric computes.
+            **stat_kwargs: All keyword arguments used by the statistic that this metric computes.
         """
 
         if sens.shape[1] != self.stat_shape[-1]:
             raise ValueError(f"Expected sens to have shape (N, {self.stat_shape[-1]}, got {sens.shape}")
 
         self.num += self.stat.num(pred, sens, *stat_args, **stat_kwargs)
         self.denom += self.stat.denom(pred, sens, *stat_args, **stat_kwargs)
```

### Comparing `fairret-0.1.1/fairret/statistic/base.py` & `fairret-0.1.2/fairret/statistic/base.py`

 * *Files identical despite different names*

### Comparing `fairret-0.1.1/fairret/utils.py` & `fairret-0.1.2/fairret/utils.py`

 * *Files identical despite different names*

### Comparing `fairret-0.1.1/fairret.egg-info/PKG-INFO` & `fairret-0.1.2/fairret.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairret
-Version: 0.1.1
+Version: 0.1.2
 Summary: A fairness library in PyTorch.
 Author-email: Maarten Buyl <maarten.buyl@ugent.be>, MaryBeth Defrance <marybeth.defrance@ugent.be>
 License: MIT License
         
         Copyright (c) 2024 Ghent University Artificial Intelligence & Data Analytics Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -45,25 +45,24 @@
 1. *flexible* in how fairness is defined and pursued.
 2. *easy* to integrate into existing PyTorch pipelines.
 3. *clear* in what its tools can and cannot do.
 
 The central to the library is the paradigm of the _fairness regularization term_ (fairrets) that quantify unfairness as differentiable PyTorch loss functions. 
 These can then be optimized together with e.g. the binary cross-entropy error such that the classifier improves both its accuracy and fairness.
 
-**The library is still in very early development.** Documentation, installation instructions, and more examples will be added in the near future.
-
 ## Installation
 The fairret library can be installed via PyPi:
 
 ```
 pip install fairret
 ```
 
-### Dependencies
-A minimal list of dependencies is provided in [pyproject.toml](https://github.com/aida-ugent/fairret/blob/main/pyproject.toml). If the library is installed locally, the required packages can be installed via `pip install .`
+A minimal list of dependencies is provided in [pyproject.toml](https://github.com/aida-ugent/fairret/blob/main/pyproject.toml). 
+
+If the library is installed locally, the required packages can be installed via `pip install .`
 
 ## Quickstart
 
 It suffices to simply choose a statistic that should be equalized across groups and a fairret that quantifies the gap. The model can then be trained as follows:
 
 ```python
 import torch.nn.functional as F
```

### Comparing `fairret-0.1.1/fairret.egg-info/SOURCES.txt` & `fairret-0.1.2/fairret.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fairret-0.1.1/pyproject.toml` & `fairret-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fairret-0.1.1/test/test_loss.py` & `fairret-0.1.2/test/test_loss.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pytest
 import torch
 
-from fairret.statistic import Accuracy, StackedLinearFractionalStatistic, TruePositiveRate, FalsePositiveRate
+from fairret.statistic import (PositiveRate, Accuracy, StackedLinearFractionalStatistic, TruePositiveRate,
+                               FalsePositiveRate)
 from fairret.loss import (NormLoss, LSELoss, KLProjectionLoss, JensenShannonProjectionLoss,
                           TotalVariationProjectionLoss, SquaredEuclideanProjectionLoss)
 
 
 @pytest.fixture
 def easy_data():
     return (
@@ -23,14 +24,40 @@
         torch.nn.ReLU(),
         torch.nn.Linear(4, 1)
     )
 
 
 @pytest.mark.parametrize("loss_cls", [NormLoss, LSELoss, KLProjectionLoss, JensenShannonProjectionLoss,
                                       TotalVariationProjectionLoss, SquaredEuclideanProjectionLoss])
+def test_loss_positive_rate(loss_cls, easy_data, net):
+    feat, sens, _ = easy_data
+    feat_backup = feat.clone()
+    sens_backup = sens.clone()
+
+    fairret = loss_cls(PositiveRate())
+    nb_tries = 5
+
+    # Calculate loss multiple times as some losses are stateful
+    for _ in range(nb_tries):
+        logit = net(feat)
+        loss = fairret(logit, sens)
+        assert loss.item() >= 0  # fairret should be nonnegative
+        loss.backward()
+        for p in net.parameters():
+            assert p.grad is not None
+            assert torch.all(torch.isfinite(p.grad))
+            p.grad.zero_()
+
+    # Check that the data was not modified
+    assert torch.all(feat == feat_backup)
+    assert torch.all(sens == sens_backup)
+
+
+@pytest.mark.parametrize("loss_cls", [NormLoss, LSELoss, KLProjectionLoss, JensenShannonProjectionLoss,
+                                      TotalVariationProjectionLoss, SquaredEuclideanProjectionLoss])
 def test_loss_accuracy(loss_cls, easy_data, net):
     feat, sens, label = easy_data
     feat_backup = feat.clone()
     sens_backup = sens.clone()
     label_backup = label.clone()
 
     fairret = loss_cls(Accuracy())
```

### Comparing `fairret-0.1.1/test/test_metric.py` & `fairret-0.1.2/test/test_metric.py`

 * *Files identical despite different names*

### Comparing `fairret-0.1.1/test/test_statistic.py` & `fairret-0.1.2/test/test_statistic.py`

 * *Files identical despite different names*

