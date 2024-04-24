# Comparing `tmp/pyepo-0.3.7.tar.gz` & `tmp/pyepo-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyepo-0.3.7.tar", last modified: Fri Apr 19 05:03:49 2024, max compression
+gzip compressed data, was "pyepo-0.3.8.tar", last modified: Wed Apr 24 20:57:05 2024, max compression
```

## Comparing `pyepo-0.3.7.tar` & `pyepo-0.3.8.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:03:49.517354 pyepo-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-19 05:03:49.517354 pyepo-0.3.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:03:49.509354 pyepo-0.3.7/pyepo/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/EPO.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:03:49.509354 pyepo-0.3.7/pyepo/data/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/data/knapsack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/data/shortestpath.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/data/tsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:03:49.509354 pyepo-0.3.7/pyepo/func/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/func/abcmodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/func/blackbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/func/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (127)    19095 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/func/perturbed.py
--rw-r--r--   0 runner    (1001) docker     (127)     9118 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/func/rank.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/func/spoplus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/func/utlis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:03:49.513354 pyepo-0.3.7/pyepo/metric/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/metric/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/metric/mse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/metric/regret.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/metric/unambregret.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:03:49.513354 pyepo-0.3.7/pyepo/model/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:03:49.513354 pyepo-0.3.7/pyepo/model/copt/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/copt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/copt/coptmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/copt/knapsack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/copt/shortestpath.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:03:49.513354 pyepo-0.3.7/pyepo/model/grb/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/grb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/grb/grbmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/grb/knapsack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/grb/shortestpath.py
--rw-r--r--   0 runner    (1001) docker     (127)    15414 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/grb/tsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:03:49.513354 pyepo-0.3.7/pyepo/model/omo/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/omo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/omo/knapsack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/omo/omomodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/omo/shortestpath.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/model/opt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:03:49.517354 pyepo-0.3.7/pyepo/twostage/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/twostage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/twostage/autosklearnpred.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/twostage/sklearnpred.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-19 05:03:40.000000 pyepo-0.3.7/pyepo/utlis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:03:49.517354 pyepo-0.3.7/pyepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-19 05:03:49.000000 pyepo-0.3.7/pyepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-19 05:03:49.000000 pyepo-0.3.7/pyepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 05:03:49.000000 pyepo-0.3.7/pyepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 05:03:49.000000 pyepo-0.3.7/pyepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 05:03:49.000000 pyepo-0.3.7/pyepo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 05:03:49.517354 pyepo-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-19 05:03:40.000000 pyepo-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:57:05.652554 pyepo-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-24 20:57:05.652554 pyepo-0.3.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:57:05.644554 pyepo-0.3.8/pyepo/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/EPO.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:57:05.644554 pyepo-0.3.8/pyepo/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/data/knapsack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/data/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/data/shortestpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/data/tsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:57:05.648554 pyepo-0.3.8/pyepo/func/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/func/abcmodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/func/blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/func/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18951 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/func/perturbed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8775 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/func/rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/func/spoplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/func/utlis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:57:05.648554 pyepo-0.3.8/pyepo/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/metric/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/metric/mse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/metric/regret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/metric/unambregret.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:57:05.648554 pyepo-0.3.8/pyepo/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:57:05.648554 pyepo-0.3.8/pyepo/model/copt/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/copt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/copt/coptmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/copt/knapsack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/copt/shortestpath.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:57:05.652554 pyepo-0.3.8/pyepo/model/grb/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/grb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/grb/grbmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/grb/knapsack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/grb/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/grb/shortestpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15414 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/grb/tsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:57:05.652554 pyepo-0.3.8/pyepo/model/omo/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/omo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/omo/knapsack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/omo/omomodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/omo/shortestpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/model/opt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:57:05.652554 pyepo-0.3.8/pyepo/twostage/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/twostage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/twostage/autosklearnpred.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/twostage/sklearnpred.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-24 20:57:00.000000 pyepo-0.3.8/pyepo/utlis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:57:05.652554 pyepo-0.3.8/pyepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-24 20:57:05.000000 pyepo-0.3.8/pyepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-24 20:57:05.000000 pyepo-0.3.8/pyepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:57:05.000000 pyepo-0.3.8/pyepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 20:57:05.000000 pyepo-0.3.8/pyepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 20:57:05.000000 pyepo-0.3.8/pyepo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 20:57:05.652554 pyepo-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-24 20:57:00.000000 pyepo-0.3.8/setup.py
```

### Comparing `pyepo-0.3.7/PKG-INFO` & `pyepo-0.3.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyepo
-Version: 0.3.7
+Version: 0.3.8
 Summary: PyTorch-based End-to-End Predict-then-Optimize Tool
 Home-page: https://github.com/khalil-research/PyEPO
 Author: Bo Tang
 Author-email: bolucas.tang@mail.utoronto.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pyepo-0.3.7/pyepo/data/dataset.py` & `pyepo-0.3.8/pyepo/data/dataset.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.7/pyepo/data/knapsack.py` & `pyepo-0.3.8/pyepo/data/knapsack.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.7/pyepo/data/shortestpath.py` & `pyepo-0.3.8/pyepo/data/shortestpath.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.7/pyepo/data/tsp.py` & `pyepo-0.3.8/pyepo/data/tsp.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.7/pyepo/func/abcmodule.py` & `pyepo-0.3.8/pyepo/func/abcmodule.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,7 +62,16 @@
     @abstractmethod
     def forward(self, pred_cost, true_cost):
         """
         Forward pass
         """
         # convert tensor
         pass
+
+    def _update_solution_pool(self, sol):
+        """
+        Add new solutions to solution pool
+        """
+        # add into solpool
+        self.solpool = np.concatenate((self.solpool, sol))
+        # remove duplicate
+        self.solpool = np.unique(self.solpool, axis=0)
```

### Comparing `pyepo-0.3.7/pyepo/func/blackbox.py` & `pyepo-0.3.8/pyepo/func/blackbox.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import numpy as np
 import torch
 from torch.autograd import Function
 
 from pyepo.func.abcmodule import optModule
 from pyepo import EPO
-from pyepo.func.utlis import _solveWithObj4Par, _solve_in_pass, _cache_in_pass
+from pyepo.func.utlis import _solve_or_cache
 
 
 class blackboxOpt(optModule):
     """
     An autograd module for differentiable black-box optimizer, which yield
     an optimal solution and derive a gradient.
 
@@ -69,36 +69,26 @@
             module (optModule): blackboxOpt module
 
         Returns:
             torch.tensor: predicted solutions
         """
         # get device
         device = pred_cost.device
-        # convert tenstor
+        # convert tensor
         cp = pred_cost.detach().to("cpu").numpy()
         # solve
-        rand_sigma = np.random.uniform()
-        if rand_sigma <= module.solve_ratio:
-            sol, _ = _solve_in_pass(cp, module.optmodel, module.processes, module.pool)
-            if module.solve_ratio < 1:
-                # add into solpool
-                module.solpool = np.concatenate((module.solpool, sol))
-                # remove duplicate
-                module.solpool = np.unique(module.solpool, axis=0)
-        else:
-            sol, _ = _cache_in_pass(cp, module.optmodel, module.solpool)
+        sol, _ = _solve_or_cache(cp, module)
         # convert to tensor
-        sol = np.array(sol)
-        pred_sol = torch.FloatTensor(sol).to(device)
+        sol = torch.FloatTensor(sol).to(device)
         # save
-        ctx.save_for_backward(pred_cost, pred_sol)
+        ctx.save_for_backward(pred_cost, sol)
         # add other objects to ctx
         ctx.lambd = module.lambd
         ctx.module = module
-        return pred_sol
+        return sol
 
     @staticmethod
     def backward(ctx, grad_output):
         """
         Backward pass for DBB
         """
         pred_cost, pred_sol = ctx.saved_tensors
@@ -109,24 +99,15 @@
         # convert tenstor
         cp = pred_cost.detach().to("cpu").numpy()
         wp = pred_sol.detach().to("cpu").numpy()
         dl = grad_output.detach().to("cpu").numpy()
         # perturbed costs
         cq = cp + lambd * dl
         # solve
-        rand_sigma = np.random.uniform()
-        if rand_sigma <= module.solve_ratio:
-            sol, _ = _solve_in_pass(cq, module.optmodel, module.processes, module.pool)
-            if module.solve_ratio < 1:
-                # add into solpool
-                module.solpool = np.concatenate((module.solpool, sol))
-                # remove duplicate
-                module.solpool = np.unique(module.solpool, axis=0)
-        else:
-            sol, _ = _cache_in_pass(cq, module.optmodel, module.solpool)
+        sol, _ = _solve_or_cache(cq, module)
         # get gradient
         grad = (sol - wp) / module.lambd
         # convert to tensor
         grad = torch.FloatTensor(grad).to(device)
         return grad, None
 
 
@@ -185,29 +166,20 @@
             torch.tensor: predicted solutions
         """
         # get device
         device = pred_cost.device
         # convert tenstor
         cp = pred_cost.detach().to("cpu").numpy()
         # solve
-        rand_sigma = np.random.uniform()
-        if rand_sigma <= module.solve_ratio:
-            sol, _ = _solve_in_pass(cp, module.optmodel, module.processes, module.pool)
-            if module.solve_ratio < 1:
-                # add into solpool
-                module.solpool = np.concatenate((module.solpool, sol))
-                # remove duplicate
-                module.solpool = np.unique(module.solpool, axis=0)
-        else:
-            sol, _ = _cache_in_pass(cp, module.optmodel, module.solpool)
+        sol, _ = _solve_or_cache(cp, module)
         # convert to tensor
-        pred_sol = torch.FloatTensor(np.array(sol)).to(device)
+        sol = torch.FloatTensor(sol).to(device)
         # add other objects to ctx
         ctx.optmodel = module.optmodel
-        return pred_sol
+        return sol
 
     @staticmethod
     def backward(ctx, grad_output):
         """
         Backward pass for NID
         """
         optmodel = ctx.optmodel
```

### Comparing `pyepo-0.3.7/pyepo/func/contrastive.py` & `pyepo-0.3.8/pyepo/func/contrastive.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import numpy as np
 import torch
 
 from pyepo import EPO
 from pyepo.func.abcmodule import optModule
 from pyepo.data.dataset import optDataset
-from pyepo.func.utlis import _solveWithObj4Par, _solve_in_pass, _cache_in_pass
+from pyepo.func.utlis import _solveWithObj4Par, _solve_in_pass
 
 
 class NCE(optModule):
     """
     An autograd module for noise contrastive estimation as surrogate loss
     functions, based on viewing suboptimal solutions as negative examples.
 
@@ -49,17 +49,15 @@
         device = pred_cost.device
         # convert tensor
         cp = pred_cost.detach().to("cpu").numpy()
         # solve
         if np.random.uniform() <= self.solve_ratio:
             sol, _ = _solve_in_pass(cp, self.optmodel, self.processes, self.pool)
             # add into solpool
-            self.solpool = np.concatenate((self.solpool, sol))
-            # remove duplicate
-            self.solpool = np.unique(self.solpool, axis=0)
+            self._update_solution_pool(sol)
         solpool = torch.from_numpy(self.solpool.astype(np.float32)).to(device)
         # get current obj
         obj_cp = torch.einsum("bd,bd->b", pred_cost, true_sol).unsqueeze(1)
         # get obj for solpool
         objpool_cp = torch.einsum("bd,nd->bn", pred_cost, solpool)
         # get loss
         if self.optmodel.modelSense == EPO.MINIMIZE:
@@ -114,17 +112,15 @@
         device = pred_cost.device
         # convert tensor
         cp = pred_cost.detach().to("cpu").numpy()
         # solve
         if np.random.uniform() <= self.solve_ratio:
             sol, _ = _solve_in_pass(cp, self.optmodel, self.processes, self.pool)
             # add into solpool
-            self.solpool = np.concatenate((self.solpool, sol))
-            # remove duplicate
-            self.solpool = np.unique(self.solpool, axis=0)
+            self._update_solution_pool(sol)
         solpool = torch.from_numpy(self.solpool.astype(np.float32)).to(device)
         # get current obj
         obj_cp = torch.einsum("bd,bd->b", pred_cost, true_sol).unsqueeze(1)
         # get obj for solpool
         objpool_cp = torch.einsum("bd,nd->bn", pred_cost, solpool)
         # get loss
         if self.optmodel.modelSense == EPO.MINIMIZE:
```

### Comparing `pyepo-0.3.7/pyepo/func/perturbed.py` & `pyepo-0.3.8/pyepo/func/perturbed.py`

 * *Files 1% similar despite different names*

```diff
@@ -449,24 +449,21 @@
             module.alpha += module.step
         else:
             module.alpha -= module.step
         return grad, None, None
 
 
 def _solve_or_cache(ptb_c, module):
-    rand_sigma = np.random.uniform()
     # solve optimization
-    if rand_sigma <= module.solve_ratio:
+    if np.random.uniform() <= module.solve_ratio:
         ptb_sols = _solve_in_pass(ptb_c, module.optmodel, module.processes, module.pool)
         if module.solve_ratio < 1:
             sols = ptb_sols.reshape(-1, cp.shape[1])
             # add into solpool
-            module.solpool = np.concatenate((module.solpool, sols))
-            # remove duplicate
-            module.solpool = np.unique(module.solpool, axis=0)
+            module._update_solution_pool(sol)
     # best cached solution
     else:
         ptb_sols = _cache_in_pass(ptb_c, optmodel, module.solpool)
     return ptb_sols
 
 
 def _solve_in_pass(ptb_c, optmodel, processes, pool):
```

### Comparing `pyepo-0.3.7/pyepo/func/rank.py` & `pyepo-0.3.8/pyepo/func/rank.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import torch
 import torch.nn.functional as F
 from torch import nn
 
 from pyepo import EPO
 from pyepo.func.abcmodule import optModule
 from pyepo.data.dataset import optDataset
-from pyepo.func.utlis import _solveWithObj4Par, _solve_in_pass, _cache_in_pass
+from pyepo.func.utlis import _solveWithObj4Par, _solve_in_pass
 
 
 class listwiseLTR(optModule):
     """
     An autograd module for listwise learning to rank, where the goal is to learn
     an objective function that ranks a pool of feasible solutions correctly.
 
@@ -52,17 +52,15 @@
         device = pred_cost.device
         # convert tensor
         cp = pred_cost.detach().to("cpu").numpy()
         # solve
         if np.random.uniform() <= self.solve_ratio:
             sol, _ = _solve_in_pass(cp, self.optmodel, self.processes, self.pool)
             # add into solpool
-            self.solpool = np.concatenate((self.solpool, sol))
-            # remove duplicate
-            self.solpool = np.unique(self.solpool, axis=0)
+            self._update_solution_pool(sol)
         # convert tensor
         solpool = torch.from_numpy(self.solpool.astype(np.float32)).to(device)
         # obj for solpool
         objpool_c = true_cost @ solpool.T # true cost
         objpool_cp = pred_cost @ solpool.T # pred cost
         # cross entropy loss
         if self.optmodel.modelSense == EPO.MINIMIZE:
@@ -120,17 +118,15 @@
         device = pred_cost.device
         # convert tensor
         cp = pred_cost.detach().to("cpu").numpy()
         # solve
         if np.random.uniform() <= self.solve_ratio:
             sol, _ = _solve_in_pass(cp, self.optmodel, self.processes, self.pool)
             # add into solpool
-            self.solpool = np.concatenate((self.solpool, sol))
-            # remove duplicate
-            self.solpool = np.unique(self.solpool, axis=0)
+            self._update_solution_pool(sol)
         # convert tensor
         solpool = torch.from_numpy(self.solpool.astype(np.float32)).to(device)
         # obj for solpool
         objpool_c = torch.einsum("bd,nd->bn", true_cost, solpool) # true cost
         objpool_cp = torch.einsum("bd,nd->bn", pred_cost, solpool) # pred cost
         # init relu as max(0,x)
         relu = nn.ReLU()
@@ -202,17 +198,15 @@
         device = pred_cost.device
         # convert tensor
         cp = pred_cost.detach().to("cpu").numpy()
         # solve
         if np.random.uniform() <= self.solve_ratio:
             sol, _ = _solve_in_pass(cp, self.optmodel, self.processes, self.pool)
             # add into solpool
-            self.solpool = np.concatenate((self.solpool, sol))
-            # remove duplicate
-            self.solpool = np.unique(self.solpool, axis=0)
+            self._update_solution_pool(sol)
         # convert tensor
         solpool = torch.from_numpy(self.solpool.astype(np.float32)).to(device)
         # obj for solpool as score
         objpool_c = true_cost @ solpool.T # true cost
         objpool_cp = pred_cost @ solpool.T # pred cost
         # squared loss
         loss = (objpool_c - objpool_cp).square().mean(axis=1)
```

### Comparing `pyepo-0.3.7/pyepo/func/spoplus.py` & `pyepo-0.3.8/pyepo/func/spoplus.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import numpy as np
 import torch
 from torch.autograd import Function
 
 from pyepo import EPO
 from pyepo.func.abcmodule import optModule
-from pyepo.func.utlis import _solveWithObj4Par, _solve_in_pass, _cache_in_pass
+from pyepo.func.utlis import _solve_or_cache
 
 class SPOPlus(optModule):
     """
     An autograd module for SPO+ Loss, as a surrogate loss function of SPO Loss,
     which measures the decision error of the optimization problem.
 
     For SPO/SPO+ Loss, the objective function is linear and constraints are
@@ -83,35 +83,26 @@
         cp = pred_cost.detach().to("cpu").numpy()
         c = true_cost.detach().to("cpu").numpy()
         w = true_sol.detach().to("cpu").numpy()
         z = true_obj.detach().to("cpu").numpy()
         # check sol
         #_check_sol(c, w, z)
         # solve
-        if np.random.uniform() <= module.solve_ratio:
-            sol, obj = _solve_in_pass(2*cp-c, module.optmodel, module.processes, module.pool)
-            if module.solve_ratio < 1:
-                # add into solpool
-                module.solpool = np.concatenate((module.solpool, sol))
-                # remove duplicate
-                module.solpool = np.unique(module.solpool, axis=0)
-        else:
-            sol, obj = _cache_in_pass(2*cp-c, module.optmodel, module.solpool)
+        sol, obj = _solve_or_cache(2 * cp - c, module)
         # calculate loss
         loss = []
         for i in range(len(cp)):
             loss.append(- obj[i] + 2 * np.dot(cp[i], w[i]) - z[i])
         # sense
         if module.optmodel.modelSense == EPO.MINIMIZE:
             loss = np.array(loss)
         if module.optmodel.modelSense == EPO.MAXIMIZE:
             loss = - np.array(loss)
         # convert to tensor
         loss = torch.FloatTensor(loss).to(device)
-        sol = np.array(sol)
         sol = torch.FloatTensor(sol).to(device)
         # save solutions
         ctx.save_for_backward(true_sol, sol)
         # add other objects to ctx
         ctx.optmodel = module.optmodel
         return loss
```

### Comparing `pyepo-0.3.7/pyepo/func/utlis.py` & `pyepo-0.3.8/pyepo/func/utlis.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,30 @@
 
 import numpy as np
 
 from pyepo import EPO
 from pyepo.utlis import getArgs
 
 
+def _solve_or_cache(cp, module):
+    """
+    A function to get optimization solution in the forward/backward pass
+    """
+    # solve optimization
+    if np.random.uniform() <= module.solve_ratio:
+        sol, obj = _solve_in_pass(cp, module.optmodel, module.processes, module.pool)
+        if module.solve_ratio < 1:
+            # add into solpool
+            module._update_solution_pool(sol)
+    # best cached solution
+    else:
+        sol, obj = _cache_in_pass(cp, module.optmodel, module.solpool)
+    return sol, obj
+
+
 def _solve_in_pass(cp, optmodel, processes, pool):
     """
     A function to solve optimization in the forward/backward pass
     """
     # number of instance
     ins_num = len(cp)
     # single-core
@@ -22,14 +38,17 @@
         obj = []
         for i in range(ins_num):
             # solve
             optmodel.setObj(cp[i])
             solp, objp = optmodel.solve()
             sol.append(solp)
             obj.append(objp)
+        # to numpy
+        sol = np.array(sol)
+        obj = np.array(obj)
     # multi-core
     else:
         # get class
         model_type = type(optmodel)
         # get args
         args = getArgs(optmodel)
         # parallel computing
```

### Comparing `pyepo-0.3.7/pyepo/metric/metrics.py` & `pyepo-0.3.8/pyepo/metric/metrics.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.7/pyepo/metric/mse.py` & `pyepo-0.3.8/pyepo/metric/mse.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.7/pyepo/metric/regret.py` & `pyepo-0.3.8/pyepo/metric/regret.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.7/pyepo/metric/unambregret.py` & `pyepo-0.3.8/pyepo/metric/unambregret.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.7/pyepo/model/copt/coptmodel.py` & `pyepo-0.3.8/pyepo/model/copt/coptmodel.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.7/pyepo/model/copt/knapsack.py` & `pyepo-0.3.8/pyepo/model/copt/knapsack.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.7/pyepo/model/copt/shortestpath.py` & `pyepo-0.3.8/pyepo/model/copt/shortestpath.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.7/pyepo/model/grb/grbmodel.py` & `pyepo-0.3.8/pyepo/model/grb/grbmodel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python
 # coding: utf-8
 """
 Abstract optimization model based on GurobiPy
 """
 
 from copy import copy
+
+import numpy as np
 import gurobipy as gp
 from gurobipy import GRB
 
 from pyepo import EPO
 from pyepo.model.opt import optModel
 
 
@@ -30,36 +32,55 @@
             self.modelSense = EPO.MAXIMIZE
         # turn off output
         self._model.Params.outputFlag = 0
 
     def __repr__(self):
         return "optGRBModel " + self.__class__.__name__
 
+    @property
+    def num_cost(self):
+        """
+        number of cost to be predicted
+        """
+        return self.x.size if isinstance(self.x, gp.MVar) else len(self.x)
+
     def setObj(self, c):
         """
         A method to set objective function
 
         Args:
             c (np.ndarray / list): cost of objective function
         """
         if len(c) != self.num_cost:
             raise ValueError("Size of cost vector cannot match vars.")
-        obj = gp.quicksum(c[i] * self.x[k] for i, k in enumerate(self.x))
+        # mvar
+        if isinstance(self.x, gp.MVar):
+            obj = np.array(c) @ self.x
+        # vars
+        else:
+            obj = gp.quicksum(c[i] * self.x[k] for i, k in enumerate(self.x))
         self._model.setObjective(obj)
 
     def solve(self):
         """
         A method to solve model
 
         Returns:
             tuple: optimal solution (list) and objective value (float)
         """
         self._model.update()
         self._model.optimize()
-        return [self.x[k].x for k in self.x], self._model.objVal
+        # solution
+        if isinstance(self.x, gp.MVar):
+            sol = self.x.x
+        else:
+            sol = [self.x[k].x for k in self.x]
+        # objective value
+        obj = self._model.objVal
+        return sol, obj
 
     def copy(self):
         """
         A method to copy model
 
         Returns:
             optModel: new copied model
@@ -67,15 +88,15 @@
         new_model = copy(self)
         # update model
         self._model.update()
         # new model
         new_model._model = self._model.copy()
         # variables for new model
         x = new_model._model.getVars()
-        new_model.x = {key: x[i] for i, key in enumerate(self.x)}
+        new_model.x = {key: x[i] for i, key in enumerate(x)}
         return new_model
 
     def addConstr(self, coefs, rhs):
         """
         A method to add new constraint
 
         Args:
```

### Comparing `pyepo-0.3.7/pyepo/model/grb/knapsack.py` & `pyepo-0.3.8/pyepo/model/grb/knapsack.py`

 * *Files 24% similar despite different names*

```diff
@@ -26,34 +26,32 @@
         """
         Args:
             weights (np.ndarray / list): weights of items
             capacity (np.ndarray / list): total capacity
         """
         self.weights = np.array(weights)
         self.capacity = np.array(capacity)
-        self.items = list(range(self.weights.shape[1]))
+        self.items = self.weights.shape[1]
         super().__init__()
 
     def _getModel(self):
         """
         A method to build Gurobi model
 
         Returns:
             tuple: optimization model and variables
         """
         # ceate a model
         m = gp.Model("knapsack")
         # varibles
-        x = m.addVars(self.items, name="x", vtype=GRB.BINARY)
+        x = m.addMVar(self.items, name="x", vtype=GRB.BINARY)
         # sense
         m.modelSense = GRB.MAXIMIZE
         # constraints
-        for i in range(len(self.capacity)):
-            m.addConstr(gp.quicksum(self.weights[i,j] * x[j]
-                        for j in self.items) <= self.capacity[i])
+        m.addConstr(self.weights @ x <= self.capacity)
         return m, x
 
     def relax(self):
         """
         A method to get linear relaxation model
         """
         # copy
@@ -71,61 +69,58 @@
         A method to build Gurobi
         """
         # ceate a model
         m = gp.Model("knapsack")
         # turn off output
         m.Params.outputFlag = 0
         # varibles
-        x = m.addVars(self.items, name="x", ub=1)
+        x = m.addMVar(self.items, name="x", ub=1)
         # sense
         m.modelSense = GRB.MAXIMIZE
         # constraints
-        for i in range(len(self.capacity)):
-            m.addConstr(gp.quicksum(self.weights[i,j] * x[j]
-                        for j in self.items) <= self.capacity[i])
+        m.addConstr(self.weights @ x <= self.capacity)
         return m, x
 
     def relax(self):
         """
         A forbidden method to relax MIP model
         """
         raise RuntimeError("Model has already been relaxed.")
-        
-        
+
+
 if __name__ == "__main__":
-    
-    import random
+
     # random seed
-    random.seed(42)
+    np.random.seed(42)
     # set random cost for test
-    cost = [random.random() for _ in range(16)]
+    cost = np.random.random(16)
     weights = np.random.choice(range(300, 800), size=(2,16)) / 100
     capacity = [20, 20]
-    
+
     # solve model
     optmodel = knapsackModel(weights=weights, capacity=capacity) # init model
     optmodel = optmodel.copy()
     optmodel.setObj(cost) # set objective function
     sol, obj = optmodel.solve() # solve
     # print res
     print('Obj: {}'.format(obj))
     for i in range(16):
         if sol[i] > 1e-3:
             print(i)
-            
+
     # relax
     optmodel = optmodel.relax()
     optmodel.setObj(cost) # set objective function
     sol, obj = optmodel.solve() # solve
     # print res
     print('Obj: {}'.format(obj))
     for i in range(16):
         if sol[i] > 1e-3:
             print(i)
-            
+
     # add constraint
     optmodel = optmodel.addConstr([weights[0,i] for i in range(16)], 10)
     optmodel.setObj(cost) # set objective function
     sol, obj = optmodel.solve() # solve
     # print res
     print('Obj: {}'.format(obj))
     for i in range(16):
```

### Comparing `pyepo-0.3.7/pyepo/model/grb/shortestpath.py` & `pyepo-0.3.8/pyepo/model/grb/shortestpath.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.7/pyepo/model/grb/tsp.py` & `pyepo-0.3.8/pyepo/model/grb/tsp.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.7/pyepo/model/omo/knapsack.py` & `pyepo-0.3.8/pyepo/model/omo/knapsack.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.7/pyepo/model/omo/omomodel.py` & `pyepo-0.3.8/pyepo/model/omo/omomodel.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.7/pyepo/model/omo/shortestpath.py` & `pyepo-0.3.8/pyepo/model/omo/shortestpath.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.7/pyepo/model/opt.py` & `pyepo-0.3.8/pyepo/model/opt.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.7/pyepo/twostage/autosklearnpred.py` & `pyepo-0.3.8/pyepo/twostage/autosklearnpred.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.7/pyepo/utlis.py` & `pyepo-0.3.8/pyepo/utlis.py`

 * *Files identical despite different names*

### Comparing `pyepo-0.3.7/pyepo.egg-info/PKG-INFO` & `pyepo-0.3.8/pyepo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyepo
-Version: 0.3.7
+Version: 0.3.8
 Summary: PyTorch-based End-to-End Predict-then-Optimize Tool
 Home-page: https://github.com/khalil-research/PyEPO
 Author: Bo Tang
 Author-email: bolucas.tang@mail.utoronto.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pyepo-0.3.7/pyepo.egg-info/SOURCES.txt` & `pyepo-0.3.8/pyepo.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 pyepo.egg-info/SOURCES.txt
 pyepo.egg-info/dependency_links.txt
 pyepo.egg-info/requires.txt
 pyepo.egg-info/top_level.txt
 pyepo/data/__init__.py
 pyepo/data/dataset.py
 pyepo/data/knapsack.py
+pyepo/data/portfolio.py
 pyepo/data/shortestpath.py
 pyepo/data/tsp.py
 pyepo/func/__init__.py
 pyepo/func/abcmodule.py
 pyepo/func/blackbox.py
 pyepo/func/contrastive.py
 pyepo/func/perturbed.py
@@ -30,14 +31,15 @@
 pyepo/model/copt/__init__.py
 pyepo/model/copt/coptmodel.py
 pyepo/model/copt/knapsack.py
 pyepo/model/copt/shortestpath.py
 pyepo/model/grb/__init__.py
 pyepo/model/grb/grbmodel.py
 pyepo/model/grb/knapsack.py
+pyepo/model/grb/portfolio.py
 pyepo/model/grb/shortestpath.py
 pyepo/model/grb/tsp.py
 pyepo/model/omo/__init__.py
 pyepo/model/omo/knapsack.py
 pyepo/model/omo/omomodel.py
 pyepo/model/omo/shortestpath.py
 pyepo/twostage/__init__.py
```

### Comparing `pyepo-0.3.7/setup.py` & `pyepo-0.3.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     # project dir
     packages = setuptools.find_packages(),
     # description
     description = "PyTorch-based End-to-End Predict-then-Optimize Tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # version
-    version = "0.3.7",
+    version = "0.3.8",
     # Github repo
     url = "https://github.com/khalil-research/PyEPO",
     # author name
     author = "Bo Tang",
     # mail address
     author_email = "bolucas.tang@mail.utoronto.ca",
     # dependencies
```

