# Comparing `tmp/wedap-1.0.0.tar.gz` & `tmp/wedap-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wedap-1.0.0.tar", last modified: Tue Apr 23 20:11:17 2024, max compression
+gzip compressed data, was "wedap-1.0.1.tar", last modified: Wed Apr 24 17:18:08 2024, max compression
```

## Comparing `wedap-1.0.0.tar` & `wedap-1.0.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.615585 wedap-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-23 20:10:54.000000 wedap-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-04-23 20:11:17.615585 wedap-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-04-23 20:10:54.000000 wedap-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.607585 wedap-1.0.0/mdap/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-23 20:10:55.000000 wedap-1.0.0/mdap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-23 20:10:55.000000 wedap-1.0.0/mdap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22751 2024-04-23 20:10:55.000000 wedap-1.0.0/mdap/command_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     9851 2024-04-23 20:10:55.000000 wedap-1.0.0/mdap/md_pdist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-23 20:10:55.000000 wedap-1.0.0/mdap/md_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.607585 wedap-1.0.0/mdap/styles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:10:55.000000 wedap-1.0.0/mdap/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-23 20:10:55.000000 wedap-1.0.0/mdap/styles/default.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.611585 wedap-1.0.0/mdap/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 20:10:55.000000 wedap-1.0.0/mdap/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-23 20:10:55.000000 wedap-1.0.0/mdap/tests/make_md_pdist_test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-23 20:10:55.000000 wedap-1.0.0/mdap/tests/test_md_pdist.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 20:11:17.615585 wedap-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-23 20:10:55.000000 wedap-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.611585 wedap-1.0.0/styles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:10:55.000000 wedap-1.0.0/styles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.611585 wedap-1.0.0/wedap/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-23 20:10:55.000000 wedap-1.0.0/wedap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-04-23 20:10:55.000000 wedap-1.0.0/wedap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28147 2024-04-23 20:10:55.000000 wedap-1.0.0/wedap/command_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-23 20:10:56.000000 wedap-1.0.0/wedap/h5_gif.py
--rw-r--r--   0 runner    (1001) docker     (127)    69160 2024-04-23 20:10:56.000000 wedap-1.0.0/wedap/h5_pdist.py
--rw-r--r--   0 runner    (1001) docker     (127)    31441 2024-04-23 20:10:56.000000 wedap-1.0.0/wedap/h5_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.611585 wedap-1.0.0/wedap/styles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:10:56.000000 wedap-1.0.0/wedap/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-23 20:10:56.000000 wedap-1.0.0/wedap/styles/default.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.615585 wedap-1.0.0/wedap/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 20:10:56.000000 wedap-1.0.0/wedap/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-23 20:10:56.000000 wedap-1.0.0/wedap/tests/make_h5_pdist_test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-23 20:10:56.000000 wedap-1.0.0/wedap/tests/make_h5_plot_test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-04-23 20:10:56.000000 wedap-1.0.0/wedap/tests/test_h5_pdist.py
--rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-04-23 20:10:56.000000 wedap-1.0.0/wedap/tests/test_h5_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.615585 wedap-1.0.0/wedap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-04-23 20:11:17.000000 wedap-1.0.0/wedap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-23 20:11:17.000000 wedap-1.0.0/wedap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:11:17.000000 wedap-1.0.0/wedap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 20:11:17.000000 wedap-1.0.0/wedap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-23 20:11:17.000000 wedap-1.0.0/wedap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 20:11:17.000000 wedap-1.0.0/wedap.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.615585 wedap-1.0.0/wekap/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/command_line.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.615585 wedap-1.0.0/wekap/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/data/ppf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.615585 wedap-1.0.0/wekap/error/
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/error/GetAvg_CR.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/error/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)    21856 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/kinetics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:11:17.615585 wedap-1.0.0/wekap/styles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-23 20:10:56.000000 wedap-1.0.0/wekap/styles/default.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.118682 wedap-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-24 17:17:50.000000 wedap-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11158 2024-04-24 17:18:08.118682 wedap-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-04-24 17:17:50.000000 wedap-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.110682 wedap-1.0.1/mdap/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-24 17:17:50.000000 wedap-1.0.1/mdap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-24 17:17:50.000000 wedap-1.0.1/mdap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22751 2024-04-24 17:17:50.000000 wedap-1.0.1/mdap/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9887 2024-04-24 17:17:51.000000 wedap-1.0.1/mdap/md_pdist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-24 17:17:51.000000 wedap-1.0.1/mdap/md_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.110682 wedap-1.0.1/mdap/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:17:51.000000 wedap-1.0.1/mdap/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-24 17:17:51.000000 wedap-1.0.1/mdap/styles/default.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.110682 wedap-1.0.1/mdap/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-24 17:17:51.000000 wedap-1.0.1/mdap/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-24 17:17:51.000000 wedap-1.0.1/mdap/tests/make_md_pdist_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-24 17:17:51.000000 wedap-1.0.1/mdap/tests/test_md_pdist.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 17:18:08.118682 wedap-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-24 17:17:51.000000 wedap-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.110682 wedap-1.0.1/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:17:51.000000 wedap-1.0.1/styles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.114682 wedap-1.0.1/wedap/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28147 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/h5_gif.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69160 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/h5_pdist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31441 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/h5_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.114682 wedap-1.0.1/wedap/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/styles/default.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.114682 wedap-1.0.1/wedap/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/tests/make_h5_pdist_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/tests/make_h5_plot_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/tests/test_h5_pdist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/tests/test_h5_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.118682 wedap-1.0.1/wedap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11158 2024-04-24 17:18:08.000000 wedap-1.0.1/wedap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-24 17:18:08.000000 wedap-1.0.1/wedap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 17:18:08.000000 wedap-1.0.1/wedap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-24 17:18:08.000000 wedap-1.0.1/wedap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-24 17:18:08.000000 wedap-1.0.1/wedap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 17:18:08.000000 wedap-1.0.1/wedap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.114682 wedap-1.0.1/wekap/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/command_line.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.114682 wedap-1.0.1/wekap/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/data/ppf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.114682 wedap-1.0.1/wekap/error/
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/error/GetAvg_CR.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/error/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21856 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/kinetics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.118682 wedap-1.0.1/wekap/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/styles/default.mplstyle
```

### Comparing `wedap-1.0.0/LICENSE` & `wedap-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wedap-1.0.0/PKG-INFO` & `wedap-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wedap
-Version: 1.0.0
+Version: 1.0.1
 Summary: Weighted Ensemble Data Analysis and Plotting
 Home-page: https://github.com/darianyang/wedap
 Author: Darian T. Yang
 Author-email: dty7@pitt.edu
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Darian Yang
@@ -52,15 +52,15 @@
     <img src="https://github.com/darianyang/wedap/blob/main/docs/_static/wedap_logo.png?raw=true" alt="wedap logo" width="400">
 </p>
 
 ![tests](https://github.com/darianyang/wedap/actions/workflows/tests.yml/badge.svg)
 [![docs](https://img.shields.io/website?label=docs&up_color=brightgreen&up_message=online&url=https%3A%2F%2Fdarianyang.github.io%2Fwedap%2Fdocs%2Fhtml%2Findex.html)](https://darianyang.github.io/wedap/docs/html/index.html)
 [![PyPI version](https://badge.fury.io/py/wedap.svg)](https://badge.fury.io/py/wedap)
 [![Downloads](https://static.pepy.tech/badge/wedap)](https://pepy.tech/project/wedap)
-[![GitHub license](https://img.shields.io/github/license/darianyang/wedap)](https://github.com/darianyang/wedap/blob/master/LICENSE)
+[![DOI](https://zenodo.org/badge/405205357.svg)](https://zenodo.org/doi/10.5281/zenodo.11051656)
 
 **WEDAP** : **w**eighted **e**nsemble **d**ata **a**nalysis and **p**lotting (pronounced we-dap)
 
 `wedap` is primarily used to plot H5 files produced from running [WESTPA](https://github.com/westpa/westpa).
 
 `mdap` can be used to plot data files from analysis of standard MD simulations.
```

### Comparing `wedap-1.0.0/README.md` & `wedap-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     <img src="https://github.com/darianyang/wedap/blob/main/docs/_static/wedap_logo.png?raw=true" alt="wedap logo" width="400">
 </p>
 
 ![tests](https://github.com/darianyang/wedap/actions/workflows/tests.yml/badge.svg)
 [![docs](https://img.shields.io/website?label=docs&up_color=brightgreen&up_message=online&url=https%3A%2F%2Fdarianyang.github.io%2Fwedap%2Fdocs%2Fhtml%2Findex.html)](https://darianyang.github.io/wedap/docs/html/index.html)
 [![PyPI version](https://badge.fury.io/py/wedap.svg)](https://badge.fury.io/py/wedap)
 [![Downloads](https://static.pepy.tech/badge/wedap)](https://pepy.tech/project/wedap)
-[![GitHub license](https://img.shields.io/github/license/darianyang/wedap)](https://github.com/darianyang/wedap/blob/master/LICENSE)
+[![DOI](https://zenodo.org/badge/405205357.svg)](https://zenodo.org/doi/10.5281/zenodo.11051656)
 
 **WEDAP** : **w**eighted **e**nsemble **d**ata **a**nalysis and **p**lotting (pronounced we-dap)
 
 `wedap` is primarily used to plot H5 files produced from running [WESTPA](https://github.com/westpa/westpa).
 
 `mdap` can be used to plot data files from analysis of standard MD simulations.
```

### Comparing `wedap-1.0.0/mdap/__main__.py` & `wedap-1.0.1/mdap/__main__.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.0/mdap/command_line.py` & `wedap-1.0.1/mdap/command_line.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.0/mdap/md_pdist.py` & `wedap-1.0.1/mdap/md_pdist.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,17 +244,17 @@
         if self.data_type == "time":
             X, Y = self.timeseries()
             return X, Y, np.ones((X.shape[0]))
         # return pdist data
         # TODO: t/e block to catch mismatched data lengths and print lengths?
         elif self.data_type == "pdist":
             # for 3D datasets, e.g. scatter
-            if self.Yname and self.Zname:
+            if self.Yname is not None and self.Zname is not None:
                 return self.pdist_3d()
             # if 2D, return 2D dataset
-            if self.Yname:
+            if self.Yname is not None:
                 return self.pdist_2d()
             # otherwise return 1D
             else:
                 X, Y = self.pdist_1d()
                 # TODO: fake 3D output for now to accomodate main.py
                 return X, Y, np.ones(X.shape[0])
```

### Comparing `wedap-1.0.0/mdap/md_plot.py` & `wedap-1.0.1/mdap/md_plot.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.0/mdap/tests/make_md_pdist_test_data.py` & `wedap-1.0.1/mdap/tests/make_md_pdist_test_data.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.0/mdap/tests/test_md_pdist.py` & `wedap-1.0.1/mdap/tests/test_md_pdist.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.0/setup.py` & `wedap-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open('./LICENSE') as f:
     lic = f.read()
 
 packages = find_packages()
 
 setup(
     name='wedap',
-    version='1.0.0',
+    version='1.0.1',
     description='Weighted Ensemble Data Analysis and Plotting',
     long_description=readme,
     long_description_content_type="text/markdown",
     author='Darian T. Yang',
     author_email='dty7@pitt.edu',
     install_requires=['numpy', 'matplotlib', 'h5py', 'gif', 'tqdm'],
     url='https://github.com/darianyang/wedap',
```

### Comparing `wedap-1.0.0/wedap/__main__.py` & `wedap-1.0.1/wedap/__main__.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.0/wedap/command_line.py` & `wedap-1.0.1/wedap/command_line.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.0/wedap/h5_gif.py` & `wedap-1.0.1/wedap/h5_gif.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.0/wedap/h5_pdist.py` & `wedap-1.0.1/wedap/h5_pdist.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.0/wedap/h5_plot.py` & `wedap-1.0.1/wedap/h5_plot.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.0/wedap/tests/make_h5_pdist_test_data.py` & `wedap-1.0.1/wedap/tests/make_h5_pdist_test_data.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.0/wedap/tests/make_h5_plot_test_data.py` & `wedap-1.0.1/wedap/tests/make_h5_plot_test_data.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.0/wedap/tests/test_h5_pdist.py` & `wedap-1.0.1/wedap/tests/test_h5_pdist.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.0/wedap/tests/test_h5_plot.py` & `wedap-1.0.1/wedap/tests/test_h5_plot.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.0/wedap.egg-info/PKG-INFO` & `wedap-1.0.1/wedap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wedap
-Version: 1.0.0
+Version: 1.0.1
 Summary: Weighted Ensemble Data Analysis and Plotting
 Home-page: https://github.com/darianyang/wedap
 Author: Darian T. Yang
 Author-email: dty7@pitt.edu
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Darian Yang
@@ -52,15 +52,15 @@
     <img src="https://github.com/darianyang/wedap/blob/main/docs/_static/wedap_logo.png?raw=true" alt="wedap logo" width="400">
 </p>
 
 ![tests](https://github.com/darianyang/wedap/actions/workflows/tests.yml/badge.svg)
 [![docs](https://img.shields.io/website?label=docs&up_color=brightgreen&up_message=online&url=https%3A%2F%2Fdarianyang.github.io%2Fwedap%2Fdocs%2Fhtml%2Findex.html)](https://darianyang.github.io/wedap/docs/html/index.html)
 [![PyPI version](https://badge.fury.io/py/wedap.svg)](https://badge.fury.io/py/wedap)
 [![Downloads](https://static.pepy.tech/badge/wedap)](https://pepy.tech/project/wedap)
-[![GitHub license](https://img.shields.io/github/license/darianyang/wedap)](https://github.com/darianyang/wedap/blob/master/LICENSE)
+[![DOI](https://zenodo.org/badge/405205357.svg)](https://zenodo.org/doi/10.5281/zenodo.11051656)
 
 **WEDAP** : **w**eighted **e**nsemble **d**ata **a**nalysis and **p**lotting (pronounced we-dap)
 
 `wedap` is primarily used to plot H5 files produced from running [WESTPA](https://github.com/westpa/westpa).
 
 `mdap` can be used to plot data files from analysis of standard MD simulations.
```

### Comparing `wedap-1.0.0/wedap.egg-info/SOURCES.txt` & `wedap-1.0.1/wedap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wedap-1.0.0/wekap/__main__.py` & `wedap-1.0.1/wekap/__main__.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.0/wekap/bootstrap.py` & `wedap-1.0.1/wekap/bootstrap.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.0/wekap/command_line.py` & `wedap-1.0.1/wekap/command_line.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.0/wekap/error/GetAvg_CR.py` & `wedap-1.0.1/wekap/error/GetAvg_CR.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.0/wekap/error/bootstrap.py` & `wedap-1.0.1/wekap/error/bootstrap.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.0/wekap/kinetics.py` & `wedap-1.0.1/wekap/kinetics.py`

 * *Files identical despite different names*

