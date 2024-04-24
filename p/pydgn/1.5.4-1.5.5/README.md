# Comparing `tmp/pydgn-1.5.4.tar.gz` & `tmp/pydgn-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydgn-1.5.4.tar", last modified: Tue Apr 23 16:41:12 2024, max compression
+gzip compressed data, was "pydgn-1.5.5.tar", last modified: Wed Apr 24 09:06:04 2024, max compression
```

## Comparing `pydgn-1.5.4.tar` & `pydgn-1.5.5.tar`

### file list

```diff
@@ -1,69 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.833507 pydgn-1.5.4/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1520 2024-04-23 16:41:08.000000 pydgn-1.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-04-23 16:41:12.833507 pydgn-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-23 16:41:08.000000 pydgn-1.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.825507 pydgn-1.5.4/pydgn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.825507 pydgn-1.5.4/pydgn/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29660 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    40962 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/data/provider.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      960 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/data/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    46462 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/data/splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/data/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/data/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.825507 pydgn-1.5.4/pydgn/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/evaluation/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    40108 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/evaluation/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/evaluation/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/evaluation/random_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    17069 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/evaluation/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.829507 pydgn-1.5.4/pydgn/experiment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17117 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/experiment/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/experiment/semi_supervised_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/experiment/supervised_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/experiment/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.829507 pydgn-1.5.4/pydgn/log/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/log/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1090 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/log/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.829507 pydgn-1.5.4/pydgn/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.829507 pydgn-1.5.4/pydgn/model/dgn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/model/dgn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/model/dgn/toy_dgn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/model/dgn/toy_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/model/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.829507 pydgn-1.5.4/pydgn/model/readout/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/model/readout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/model/readout/graph_readout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/model/readout/link_readout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/model/readout/node_readout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.833507 pydgn-1.5.4/pydgn/pydgn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-04-23 16:41:12.000000 pydgn-1.5.4/pydgn/pydgn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-23 16:41:12.000000 pydgn-1.5.4/pydgn/pydgn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:41:12.000000 pydgn-1.5.4/pydgn/pydgn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 16:41:12.000000 pydgn-1.5.4/pydgn/pydgn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-23 16:41:12.000000 pydgn-1.5.4/pydgn/pydgn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 16:41:12.000000 pydgn-1.5.4/pydgn/pydgn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.829507 pydgn-1.5.4/pydgn/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.833507 pydgn-1.5.4/pydgn/training/callback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/callback/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/callback/engine_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/callback/gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (127)    47277 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/callback/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/callback/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/callback/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/callback/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    41785 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:12.833507 pydgn-1.5.4/pydgn/training/event/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/event/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/event/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/event/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-23 16:41:08.000000 pydgn-1.5.4/pydgn/training/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-23 16:41:08.000000 pydgn-1.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:41:12.833507 pydgn-1.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:04.560570 pydgn-1.5.5/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1520 2024-04-24 09:06:00.000000 pydgn-1.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-04-24 09:06:04.560570 pydgn-1.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-24 09:06:00.000000 pydgn-1.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:04.552570 pydgn-1.5.5/pydgn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/build_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:04.552570 pydgn-1.5.5/pydgn/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29660 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40962 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/data/provider.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      960 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/data/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46462 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/data/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/data/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/data/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:04.552570 pydgn-1.5.5/pydgn/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/evaluation/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40108 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/evaluation/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/evaluation/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/evaluation/random_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17069 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/evaluation/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:04.556570 pydgn-1.5.5/pydgn/experiment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17117 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/experiment/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/experiment/semi_supervised_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/experiment/supervised_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/experiment/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8269 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/launch_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:04.556570 pydgn-1.5.5/pydgn/log/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/log/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1090 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/log/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:04.556570 pydgn-1.5.5/pydgn/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:04.556570 pydgn-1.5.5/pydgn/model/dgn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/model/dgn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/model/dgn/toy_dgn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/model/dgn/toy_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/model/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:04.556570 pydgn-1.5.5/pydgn/model/readout/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/model/readout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/model/readout/graph_readout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/model/readout/link_readout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/model/readout/node_readout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:04.556570 pydgn-1.5.5/pydgn/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:04.560570 pydgn-1.5.5/pydgn/training/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/training/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/training/callback/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/training/callback/engine_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/training/callback/gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47277 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/training/callback/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/training/callback/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/training/callback/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/training/callback/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41785 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/training/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:04.560570 pydgn-1.5.5/pydgn/training/event/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/training/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/training/event/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/training/event/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/training/event/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/training/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-24 09:06:00.000000 pydgn-1.5.5/pydgn/training/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:06:04.560570 pydgn-1.5.5/pydgn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-04-24 09:06:04.000000 pydgn-1.5.5/pydgn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-24 09:06:04.000000 pydgn-1.5.5/pydgn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 09:06:04.000000 pydgn-1.5.5/pydgn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-24 09:06:04.000000 pydgn-1.5.5/pydgn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-24 09:06:04.000000 pydgn-1.5.5/pydgn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 09:06:04.000000 pydgn-1.5.5/pydgn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-24 09:06:00.000000 pydgn-1.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 09:06:04.560570 pydgn-1.5.5/setup.cfg
```

### Comparing `pydgn-1.5.4/LICENSE` & `pydgn-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/PKG-INFO` & `pydgn-1.5.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: pydgn
-Version: 1.5.4
-Summary: A Python Package for Deep Graph Networks
-Author-email: Federico Errica <f.errica@protonmail.com>
-Project-URL: Homepage, https://pydgn.readthedocs.io/en/latest/
-Keywords: deep-graph-networks,evaluation-framework,deep-learning-for-graphs
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: PyYAML>=5.4
-Requires-Dist: tqdm>=4.66.1
-Requires-Dist: Requests>=2.31.0
-Requires-Dist: scikit_learn>=1.3.0
-Requires-Dist: tensorboard>=2.11.0
-Requires-Dist: tqdm>=4.47.0
-Requires-Dist: ogb>=1.2.0
-Requires-Dist: ray>=2.6.0
-Requires-Dist: torch>=2.0.0
-Requires-Dist: torch-geometric>=2.3.0
-
 <p align="center">
   <img src="https://github.com/diningphil/PyDGN/blob/main/docs/_static/pydgn-logo.png"  width="300"/>
 </p>
 
 # PyDGN: a research library for Deep Graph Networks 
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-gray.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Documentation Status](https://readthedocs.org/projects/pydgn/badge/?version=latest)](https://pydgn.readthedocs.io/en/latest/?badge=latest)
@@ -85,14 +61,38 @@
 
 To debug your code you can add `--debug` to the command above, but the "GUI" will be disabled.
 
 To stop the computation, use ``CTRL-C`` to send a ``SIGINT`` signal, and consider using the command ``ray stop`` to stop
 all Ray processes. **Warning:** ``ray stop`` stops **all** ray processes you have launched, including those of other
 experiments in progress, if any.
 
+### Using the Trained Models
+
+It's very easy to load the model from the experiments (see also the [Tutorial](https://pydgn.readthedocs.io/en/latest/tutorial.html)):
+
+    from pydgn.evaluation.util import *
+
+    config = retrieve_best_configuration('RESULTS/supervised_grid_search_toy_NCI1/MODEL_ASSESSMENT/OUTER_FOLD_1/MODEL_SELECTION/')
+    splits_filepath = 'examples/DATA_SPLITS/CHEMICAL/NCI1/NCI1_outer10_inner1.splits'
+    device = 'cpu'
+
+    # instantiate dataset
+    dataset = instantiate_dataset_from_config(config)
+
+    # instantiate model
+    model = instantiate_model_from_config(config, dataset, config_type="supervised_config")
+
+    # load model's checkpoint, assuming the best configuration has been loaded
+    checkpoint_location = 'RESULTS/supervised_grid_search_toy_NCI1/MODEL_ASSESSMENT/OUTER_FOLD_1/final_run1/best_checkpoint.pth'
+    load_checkpoint(checkpoint_location, model, device=device)
+
+    # you can now call the forward method of your model
+    y, embeddings = model(dataset[0])
+
+
 ## Projects using PyDGN
 
 - [Infinite Contextual Graph Markov Model (ICML 2022)](https://github.com/diningphil/iCGMM)
 - [Graph Mixture Density Networks (ICML 2021)](https://github.com/diningphil/graph-mixture-density-networks)
 - [Contextual Graph Markov Model (ICML 2018, JMLR 2020)](https://github.com/diningphil/CGMM)
 - [Extended Contextual Graph Markov Model (IJCNN 2021)](https://github.com/diningphil/E-CGMM)
 - [Continual Learning Benchmark for Graphs (WWW Workshop 2021, spotlight)](https://github.com/diningphil/continual_learning_for_graphs)
```

### Comparing `pydgn-1.5.4/pydgn/data/dataset.py` & `pydgn-1.5.5/pydgn/data/dataset.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/data/provider.py` & `pydgn-1.5.5/pydgn/data/provider.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/data/sampler.py` & `pydgn-1.5.5/pydgn/data/sampler.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/data/splitter.py` & `pydgn-1.5.5/pydgn/data/splitter.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/data/transform.py` & `pydgn-1.5.5/pydgn/data/transform.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/data/util.py` & `pydgn-1.5.5/pydgn/data/util.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/evaluation/config.py` & `pydgn-1.5.5/pydgn/evaluation/config.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/evaluation/evaluator.py` & `pydgn-1.5.5/pydgn/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/evaluation/grid.py` & `pydgn-1.5.5/pydgn/evaluation/grid.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/evaluation/random_search.py` & `pydgn-1.5.5/pydgn/evaluation/random_search.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/evaluation/util.py` & `pydgn-1.5.5/pydgn/evaluation/util.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/experiment/experiment.py` & `pydgn-1.5.5/pydgn/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/experiment/semi_supervised_task.py` & `pydgn-1.5.5/pydgn/experiment/semi_supervised_task.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/experiment/supervised_task.py` & `pydgn-1.5.5/pydgn/experiment/supervised_task.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/log/logger.py` & `pydgn-1.5.5/pydgn/log/logger.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/model/dgn/toy_dgn.py` & `pydgn-1.5.5/pydgn/model/dgn/toy_dgn.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/model/dgn/toy_mlp.py` & `pydgn-1.5.5/pydgn/model/dgn/toy_mlp.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/model/interface.py` & `pydgn-1.5.5/pydgn/model/interface.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/model/readout/graph_readout.py` & `pydgn-1.5.5/pydgn/model/readout/graph_readout.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/model/readout/link_readout.py` & `pydgn-1.5.5/pydgn/model/readout/link_readout.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/model/readout/node_readout.py` & `pydgn-1.5.5/pydgn/model/readout/node_readout.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/pydgn.egg-info/PKG-INFO` & `pydgn-1.5.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydgn
-Version: 1.5.4
+Version: 1.5.5
 Summary: A Python Package for Deep Graph Networks
 Author-email: Federico Errica <f.errica@protonmail.com>
 Project-URL: Homepage, https://pydgn.readthedocs.io/en/latest/
 Keywords: deep-graph-networks,evaluation-framework,deep-learning-for-graphs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -85,14 +85,38 @@
 
 To debug your code you can add `--debug` to the command above, but the "GUI" will be disabled.
 
 To stop the computation, use ``CTRL-C`` to send a ``SIGINT`` signal, and consider using the command ``ray stop`` to stop
 all Ray processes. **Warning:** ``ray stop`` stops **all** ray processes you have launched, including those of other
 experiments in progress, if any.
 
+### Using the Trained Models
+
+It's very easy to load the model from the experiments (see also the [Tutorial](https://pydgn.readthedocs.io/en/latest/tutorial.html)):
+
+    from pydgn.evaluation.util import *
+
+    config = retrieve_best_configuration('RESULTS/supervised_grid_search_toy_NCI1/MODEL_ASSESSMENT/OUTER_FOLD_1/MODEL_SELECTION/')
+    splits_filepath = 'examples/DATA_SPLITS/CHEMICAL/NCI1/NCI1_outer10_inner1.splits'
+    device = 'cpu'
+
+    # instantiate dataset
+    dataset = instantiate_dataset_from_config(config)
+
+    # instantiate model
+    model = instantiate_model_from_config(config, dataset, config_type="supervised_config")
+
+    # load model's checkpoint, assuming the best configuration has been loaded
+    checkpoint_location = 'RESULTS/supervised_grid_search_toy_NCI1/MODEL_ASSESSMENT/OUTER_FOLD_1/final_run1/best_checkpoint.pth'
+    load_checkpoint(checkpoint_location, model, device=device)
+
+    # you can now call the forward method of your model
+    y, embeddings = model(dataset[0])
+
+
 ## Projects using PyDGN
 
 - [Infinite Contextual Graph Markov Model (ICML 2022)](https://github.com/diningphil/iCGMM)
 - [Graph Mixture Density Networks (ICML 2021)](https://github.com/diningphil/graph-mixture-density-networks)
 - [Contextual Graph Markov Model (ICML 2018, JMLR 2020)](https://github.com/diningphil/CGMM)
 - [Extended Contextual Graph Markov Model (IJCNN 2021)](https://github.com/diningphil/E-CGMM)
 - [Continual Learning Benchmark for Graphs (WWW Workshop 2021, spotlight)](https://github.com/diningphil/continual_learning_for_graphs)
```

### Comparing `pydgn-1.5.4/pydgn/pydgn.egg-info/SOURCES.txt` & `pydgn-1.5.5/pydgn.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 LICENSE
 README.md
 pyproject.toml
+pydgn/__init__.py
+pydgn/build_dataset.py
+pydgn/launch_experiment.py
+pydgn/static.py
+pydgn.egg-info/PKG-INFO
+pydgn.egg-info/SOURCES.txt
+pydgn.egg-info/dependency_links.txt
+pydgn.egg-info/entry_points.txt
+pydgn.egg-info/requires.txt
+pydgn.egg-info/top_level.txt
 pydgn/data/__init__.py
 pydgn/data/dataset.py
 pydgn/data/provider.py
 pydgn/data/sampler.py
 pydgn/data/splitter.py
 pydgn/data/transform.py
 pydgn/data/util.py
@@ -26,20 +36,14 @@
 pydgn/model/dgn/__init__.py
 pydgn/model/dgn/toy_dgn.py
 pydgn/model/dgn/toy_mlp.py
 pydgn/model/readout/__init__.py
 pydgn/model/readout/graph_readout.py
 pydgn/model/readout/link_readout.py
 pydgn/model/readout/node_readout.py
-pydgn/pydgn.egg-info/PKG-INFO
-pydgn/pydgn.egg-info/SOURCES.txt
-pydgn/pydgn.egg-info/dependency_links.txt
-pydgn/pydgn.egg-info/entry_points.txt
-pydgn/pydgn.egg-info/requires.txt
-pydgn/pydgn.egg-info/top_level.txt
 pydgn/training/__init__.py
 pydgn/training/engine.py
 pydgn/training/profiler.py
 pydgn/training/util.py
 pydgn/training/callback/__init__.py
 pydgn/training/callback/early_stopping.py
 pydgn/training/callback/engine_callback.py
```

### Comparing `pydgn-1.5.4/pydgn/training/callback/early_stopping.py` & `pydgn-1.5.5/pydgn/training/callback/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/training/callback/engine_callback.py` & `pydgn-1.5.5/pydgn/training/callback/engine_callback.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/training/callback/gradient_clipping.py` & `pydgn-1.5.5/pydgn/training/callback/gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/training/callback/metric.py` & `pydgn-1.5.5/pydgn/training/callback/metric.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/training/callback/optimizer.py` & `pydgn-1.5.5/pydgn/training/callback/optimizer.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/training/callback/plotter.py` & `pydgn-1.5.5/pydgn/training/callback/plotter.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/training/callback/scheduler.py` & `pydgn-1.5.5/pydgn/training/callback/scheduler.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/training/engine.py` & `pydgn-1.5.5/pydgn/training/engine.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/training/event/dispatcher.py` & `pydgn-1.5.5/pydgn/training/event/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/training/event/handler.py` & `pydgn-1.5.5/pydgn/training/event/handler.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/training/event/state.py` & `pydgn-1.5.5/pydgn/training/event/state.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/training/profiler.py` & `pydgn-1.5.5/pydgn/training/profiler.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pydgn/training/util.py` & `pydgn-1.5.5/pydgn/training/util.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.5.4/pyproject.toml` & `pydgn-1.5.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
-[tool.setuptools.packages.find]
-where = ["pydgn"]
-
 [project]
 name = "pydgn"
-version = "1.5.4"
+version = "1.5.5"
 description = "A Python Package for Deep Graph Networks"
 authors = [ { name="Federico Errica", email="f.errica@protonmail.com" } ]
 readme = "README.md"
 keywords = ["deep-graph-networks", "evaluation-framework", "deep-learning-for-graphs"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
```

