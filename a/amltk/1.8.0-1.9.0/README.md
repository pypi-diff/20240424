# Comparing `tmp/amltk-1.8.0.tar.gz` & `tmp/amltk-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amltk-1.8.0.tar", last modified: Mon Jan 22 10:21:51 2024, max compression
+gzip compressed data, was "amltk-1.9.0.tar", last modified: Fri Jan 26 07:49:33 2024, max compression
```

## Comparing `amltk-1.8.0.tar` & `amltk-1.9.0.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:51.695579 amltk-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-01-22 10:21:39.000000 amltk-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-01-22 10:21:51.695579 amltk-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-01-22 10:21:39.000000 amltk-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-01-22 10:21:40.000000 amltk-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 10:21:51.695579 amltk-1.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:51.671579 amltk-1.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:51.679579 amltk-1.8.0/src/amltk/
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/_asyncm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)    12558 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/_functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:51.679579 amltk-1.8.0/src/amltk/_richutil/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/_richutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/_richutil/renderable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:51.679579 amltk-1.8.0/src/amltk/_richutil/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/_richutil/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/_richutil/renderers/_make_column_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/_richutil/renderers/executors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/_richutil/renderers/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/_richutil/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:51.679579 amltk-1.8.0/src/amltk/data/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/data/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/data/dtype_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/data/measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/distances.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:51.679579 amltk-1.8.0/src/amltk/ensembling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/ensembling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/ensembling/weighted_ensemble_caruana.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:51.683579 amltk-1.8.0/src/amltk/metalearning/
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/metalearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/metalearning/dataset_distances.py
--rw-r--r--   0 runner    (1001) docker     (127)    31848 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/metalearning/metafeatures.py
--rw-r--r--   0 runner    (1001) docker     (127)    10199 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/metalearning/portfolio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:51.683579 amltk-1.8.0/src/amltk/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20728 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/optimization/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/optimization/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/optimization/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:51.683579 amltk-1.8.0/src/amltk/optimization/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/optimization/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17519 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/optimization/optimizers/neps.py
--rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/optimization/optimizers/optuna.py
--rw-r--r--   0 runner    (1001) docker     (127)    13726 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/optimization/optimizers/smac.py
--rw-r--r--   0 runner    (1001) docker     (127)    46515 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/optimization/trial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:51.683579 amltk-1.8.0/src/amltk/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:51.683579 amltk-1.8.0/src/amltk/pipeline/builders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/pipeline/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12620 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/pipeline/builders/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (127)    41929 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/pipeline/components.py
--rw-r--r--   0 runner    (1001) docker     (127)    26437 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/pipeline/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/pipeline/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:51.687579 amltk-1.8.0/src/amltk/pipeline/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/pipeline/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10317 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/pipeline/parsers/configspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/pipeline/parsers/optuna.py
--rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/pipeline/xgboost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:51.687579 amltk-1.8.0/src/amltk/profiling/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/profiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9228 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/profiling/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/profiling/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/profiling/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/randomness.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:51.687579 amltk-1.8.0/src/amltk/scheduling/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23271 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/scheduling/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:51.687579 amltk-1.8.0/src/amltk/scheduling/executors/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/scheduling/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12636 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/scheduling/executors/dask_jobqueue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/scheduling/executors/sequential_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:51.691579 amltk-1.8.0/src/amltk/scheduling/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/scheduling/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24766 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/scheduling/plugins/comm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/scheduling/plugins/emissions_tracker_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/scheduling/plugins/limiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/scheduling/plugins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    17046 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/scheduling/plugins/pynisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/scheduling/plugins/threadpoolctl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/scheduling/plugins/wandb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/scheduling/plugins/warning_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/scheduling/queue_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    67296 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/scheduling/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    15602 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/scheduling/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/scheduling/termination_strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:51.691579 amltk-1.8.0/src/amltk/sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/sklearn/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/sklearn/estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/sklearn/voting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:51.691579 amltk-1.8.0/src/amltk/store/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/store/bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/store/drop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/store/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:51.691579 amltk-1.8.0/src/amltk/store/paths/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/store/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7778 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/store/paths/path_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    16456 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/store/paths/path_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/store/stored_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-01-22 10:21:40.000000 amltk-1.8.0/src/amltk/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:51.691579 amltk-1.8.0/src/amltk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-01-22 10:21:51.000000 amltk-1.8.0/src/amltk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-01-22 10:21:51.000000 amltk-1.8.0/src/amltk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 10:21:51.000000 amltk-1.8.0/src/amltk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-01-22 10:21:51.000000 amltk-1.8.0/src/amltk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-22 10:21:51.000000 amltk-1.8.0/src/amltk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:21:51.691579 amltk-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-01-22 10:21:40.000000 amltk-1.8.0/tests/test_distances.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-01-22 10:21:40.000000 amltk-1.8.0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-01-22 10:21:40.000000 amltk-1.8.0/tests/test_randomness.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:33.187842 amltk-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-01-26 07:49:13.000000 amltk-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13491 2024-01-26 07:49:33.187842 amltk-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-01-26 07:49:13.000000 amltk-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7690 2024-01-26 07:49:13.000000 amltk-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-26 07:49:33.187842 amltk-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:33.163842 amltk-1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:33.167842 amltk-1.9.0/src/amltk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/_asyncm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12558 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:33.171842 amltk-1.9.0/src/amltk/_richutil/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/_richutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/_richutil/renderable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:33.171842 amltk-1.9.0/src/amltk/_richutil/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/_richutil/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/_richutil/renderers/_make_column_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/_richutil/renderers/executors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/_richutil/renderers/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/_richutil/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:33.171842 amltk-1.9.0/src/amltk/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/data/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/data/dtype_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/data/measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/distances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:33.171842 amltk-1.9.0/src/amltk/ensembling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/ensembling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/ensembling/weighted_ensemble_caruana.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:33.171842 amltk-1.9.0/src/amltk/metalearning/
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/metalearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/metalearning/dataset_distances.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31848 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/metalearning/metafeatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10199 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/metalearning/portfolio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:33.175842 amltk-1.9.0/src/amltk/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20728 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/optimization/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/optimization/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/optimization/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:33.175842 amltk-1.9.0/src/amltk/optimization/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/optimization/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17963 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/optimization/optimizers/neps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/optimization/optimizers/optuna.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/optimization/optimizers/smac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46515 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/optimization/trial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:33.175842 amltk-1.9.0/src/amltk/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/pipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:33.175842 amltk-1.9.0/src/amltk/pipeline/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/pipeline/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12620 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/pipeline/builders/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34704 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/pipeline/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26949 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/pipeline/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/pipeline/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:33.175842 amltk-1.9.0/src/amltk/pipeline/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/pipeline/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10317 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/pipeline/parsers/configspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/pipeline/parsers/optuna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/pipeline/xgboost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:33.175842 amltk-1.9.0/src/amltk/profiling/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/profiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9228 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/profiling/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/profiling/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/profiling/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/randomness.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:33.179842 amltk-1.9.0/src/amltk/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23271 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/scheduling/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:33.179842 amltk-1.9.0/src/amltk/scheduling/executors/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/scheduling/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12636 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/scheduling/executors/dask_jobqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/scheduling/executors/sequential_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:33.179842 amltk-1.9.0/src/amltk/scheduling/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/scheduling/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24766 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/scheduling/plugins/comm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/scheduling/plugins/emissions_tracker_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/scheduling/plugins/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/scheduling/plugins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17547 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/scheduling/plugins/pynisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/scheduling/plugins/threadpoolctl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/scheduling/plugins/wandb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/scheduling/plugins/warning_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/scheduling/queue_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67296 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/scheduling/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15602 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/scheduling/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/scheduling/termination_strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:33.179842 amltk-1.9.0/src/amltk/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/sklearn/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/sklearn/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/sklearn/voting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:33.183842 amltk-1.9.0/src/amltk/store/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/store/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/store/drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/store/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:33.183842 amltk-1.9.0/src/amltk/store/paths/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/store/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7778 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/store/paths/path_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16456 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/store/paths/path_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/store/stored_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-01-26 07:49:13.000000 amltk-1.9.0/src/amltk/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:33.183842 amltk-1.9.0/src/amltk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13491 2024-01-26 07:49:33.000000 amltk-1.9.0/src/amltk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-01-26 07:49:33.000000 amltk-1.9.0/src/amltk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 07:49:33.000000 amltk-1.9.0/src/amltk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-01-26 07:49:33.000000 amltk-1.9.0/src/amltk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-26 07:49:33.000000 amltk-1.9.0/src/amltk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 07:49:33.183842 amltk-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-01-26 07:49:13.000000 amltk-1.9.0/tests/test_distances.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-01-26 07:49:13.000000 amltk-1.9.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-01-26 07:49:13.000000 amltk-1.9.0/tests/test_randomness.py
```

### Comparing `amltk-1.8.0/LICENSE` & `amltk-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/PKG-INFO` & `amltk-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amltk
-Version: 1.8.0
+Version: 1.9.0
 Summary: AutoML Toolkit: a toolkit for building automl system
 Author-email: Eddie Bergman <eddiebergmanhs@gmail.com>
 License: Copyright 2023 AutoML-Freiburg-Hannover-Tübingen
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -63,14 +63,15 @@
 Requires-Dist: mkdocstrings[python]; extra == "doc"
 Requires-Dist: markdown-exec[ansi]; extra == "doc"
 Requires-Dist: matplotlib; extra == "doc"
 Requires-Dist: rich; extra == "doc"
 Requires-Dist: mike; extra == "doc"
 Requires-Dist: pillow; extra == "doc"
 Requires-Dist: cairosvg; extra == "doc"
+Requires-Dist: black; extra == "doc"
 Provides-Extra: sklearn
 Requires-Dist: scikit-learn; extra == "sklearn"
 Requires-Dist: threadpoolctl; extra == "sklearn"
 Provides-Extra: smac
 Requires-Dist: smac>=2.0; extra == "smac"
 Requires-Dist: amltk[configspace]; extra == "smac"
 Provides-Extra: optuna
```

### Comparing `amltk-1.8.0/README.md` & `amltk-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/pyproject.toml` & `amltk-1.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "amltk"
-version = "1.8.0"
+version = "1.9.0"
 dependencies = [
   "typing_extensions", # Better typing
   "more_itertools",    # Better iteration
   "psutil",            # Used for process termination of executors
   "pandas",
   "numpy",
 ]
@@ -43,14 +43,15 @@
   "mkdocstrings[python]",
   "markdown-exec[ansi]",
   "matplotlib",
   "rich",
   "mike",
   "pillow",
   "cairosvg",
+  "black",  # This allows mkdocstrings to format signatures in the docs
 ]
 # --- Optional user dependancies
 sklearn = ["scikit-learn", "threadpoolctl"]
 smac = ["smac>=2.0", "amltk[configspace]"]
 optuna = ["optuna"]
 configspace = ["configspace>=0.6"]
 loky = ["loky"]
@@ -93,15 +94,15 @@
   '\.\.\.',
   "raise NotImplementedError",
   "if TYPE_CHECKING",
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.8.0"
+version = "1.9.0"
 update_changelog_on_bump = true
 version_files = ["pyproject.toml:version", "src/amltk/__version__.py"]
 changelog_start_rev = "1.0.0"
 
 # https://github.com/charliermarsh/ruff
 [tool.ruff]
 target-version = "py310"
```

### Comparing `amltk-1.8.0/src/amltk/__init__.py` & `amltk-1.9.0/src/amltk/__init__.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/_asyncm.py` & `amltk-1.9.0/src/amltk/_asyncm.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/_doc.py` & `amltk-1.9.0/src/amltk/_doc.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/_functional.py` & `amltk-1.9.0/src/amltk/_functional.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/_richutil/renderable.py` & `amltk-1.9.0/src/amltk/_richutil/renderable.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/_richutil/renderers/_make_column_selector.py` & `amltk-1.9.0/src/amltk/_richutil/renderers/_make_column_selector.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/_richutil/renderers/executors.py` & `amltk-1.9.0/src/amltk/_richutil/renderers/executors.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/_richutil/renderers/function.py` & `amltk-1.9.0/src/amltk/_richutil/renderers/function.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/_richutil/util.py` & `amltk-1.9.0/src/amltk/_richutil/util.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/data/conversions.py` & `amltk-1.9.0/src/amltk/data/conversions.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/data/dtype_reduction.py` & `amltk-1.9.0/src/amltk/data/dtype_reduction.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/data/measure.py` & `amltk-1.9.0/src/amltk/data/measure.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/distances.py` & `amltk-1.9.0/src/amltk/distances.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/ensembling/weighted_ensemble_caruana.py` & `amltk-1.9.0/src/amltk/ensembling/weighted_ensemble_caruana.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/exceptions.py` & `amltk-1.9.0/src/amltk/exceptions.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/metalearning/__init__.py` & `amltk-1.9.0/src/amltk/metalearning/__init__.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/metalearning/dataset_distances.py` & `amltk-1.9.0/src/amltk/metalearning/dataset_distances.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/metalearning/metafeatures.py` & `amltk-1.9.0/src/amltk/metalearning/metafeatures.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/metalearning/portfolio.py` & `amltk-1.9.0/src/amltk/metalearning/portfolio.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/optimization/history.py` & `amltk-1.9.0/src/amltk/optimization/history.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/optimization/metric.py` & `amltk-1.9.0/src/amltk/optimization/metric.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/optimization/optimizer.py` & `amltk-1.9.0/src/amltk/optimization/optimizer.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,17 +12,25 @@
 method should return either a `parser` function or a string that can be used
 with [`node.search_space(parser=..._)`][amltk.pipeline.Node.search_space] to
 extract the search space for the optimizer.
 """
 from __future__ import annotations
 
 from abc import abstractmethod
-from collections.abc import Callable, Sequence
+from collections.abc import Callable, Iterable, Sequence
 from datetime import datetime
-from typing import TYPE_CHECKING, Any, Concatenate, Generic, ParamSpec, TypeVar
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Concatenate,
+    Generic,
+    ParamSpec,
+    TypeVar,
+    overload,
+)
 
 from more_itertools import all_unique
 
 from amltk.store.paths.path_bucket import PathBucket
 
 if TYPE_CHECKING:
     from amltk.optimization.metric import Metric
@@ -77,18 +85,31 @@
     def tell(self, report: Trial.Report[I]) -> None:
         """Tell the optimizer the report for an asked trial.
 
         Args:
             report: The report for a trial
         """
 
+    @overload
     @abstractmethod
-    def ask(self) -> Trial[I]:
+    def ask(self, n: int) -> Iterable[Trial[I]]:
+        ...
+
+    @overload
+    @abstractmethod
+    def ask(self, n: None = None) -> Trial[I]:
+        ...
+
+    @abstractmethod
+    def ask(self, n: int | None = None) -> Trial[I] | Iterable[Trial[I]]:
         """Ask the optimizer for a trial to evaluate.
 
+        Args:
+            n: The number of trials to ask for. If `None`, ask for a single trial.
+
         Returns:
             A config to sample.
         """
         ...
 
     @classmethod
     def preferred_parser(
```

### Comparing `amltk-1.8.0/src/amltk/optimization/optimizers/neps.py` & `amltk-1.9.0/src/amltk/optimization/optimizers/neps.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,21 +115,21 @@
     Write an example demonstrating NEPS with its graph search spaces
 
 """  # noqa: E501
 from __future__ import annotations
 
 import logging
 import shutil
-from collections.abc import Mapping, Sequence
+from collections.abc import Iterable, Mapping, Sequence
 from copy import deepcopy
 from dataclasses import dataclass
 from datetime import datetime
 from functools import partial
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Protocol
+from typing import TYPE_CHECKING, Any, Protocol, overload
 from typing_extensions import override
 
 import metahyper.api
 from ConfigSpace import ConfigurationSpace
 from metahyper import instance_from_map
 from more_itertools import first_true
 from neps.optimizers import SearcherMapping
@@ -387,21 +387,36 @@
             seed=seed,
             loss_metric=metrics,
             cost_metric=cost_metric,
             optimizer=searcher,
             working_dir=working_dir,
         )
 
+    @overload
+    def ask(self, n: int) -> Iterable[Trial[NEPSTrialInfo]]:
+        ...
+
+    @overload
+    def ask(self, n: None = None) -> Trial[NEPSTrialInfo]:
+        ...
+
     @override
-    def ask(self) -> Trial[NEPSTrialInfo]:
+    def ask(
+        self,
+        n: int | None = None,
+    ) -> Trial[NEPSTrialInfo] | Iterable[Trial[NEPSTrialInfo]]:
         """Ask the optimizer for a new config.
 
         Returns:
             The trial info for the new config.
         """
+        # TODO: Ask neps people if there's a good way to batch sample rather than 1 by 1
+        if n is not None:
+            return (self.ask(n=None) for _ in range(n))
+
         with self.optimizer.using_state(self.optimizer_state_file, self.serializer):
             (
                 config_id,
                 config,
                 pipeline_directory,
                 previous_pipeline_directory,
             ) = metahyper.api._sample_config(  # type: ignore
```

### Comparing `amltk-1.8.0/src/amltk/optimization/optimizers/optuna.py` & `amltk-1.9.0/src/amltk/optimization/optimizers/optuna.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,18 +97,18 @@
 !!! todo "Some more documentation"
 
     Sorry!
 
 """  # noqa: E501
 from __future__ import annotations
 
-from collections.abc import Sequence
+from collections.abc import Iterable, Sequence
 from datetime import datetime
 from pathlib import Path
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, overload
 from typing_extensions import Self, override
 
 import optuna
 from more_itertools import first_true
 from optuna.samplers import BaseSampler, NSGAIISampler, TPESampler
 from optuna.study import Study, StudyDirection
 from optuna.trial import (
@@ -261,21 +261,35 @@
                 case Metric():
                     sampler = TPESampler(seed=sampler_seed)  # from `create_study()`
                 case metrics:
                     sampler = NSGAIISampler(seed=sampler_seed)  # from `create_study()`
 
         return cls(study=study, metrics=metrics, space=space, bucket=bucket, seed=seed)
 
+    @overload
+    def ask(self, n: int) -> Iterable[Trial[OptunaTrial]]:
+        ...
+
+    @overload
+    def ask(self, n: None = None) -> Trial[OptunaTrial]:
+        ...
+
     @override
-    def ask(self) -> Trial[OptunaTrial]:
+    def ask(
+        self,
+        n: int | None = None,
+    ) -> Trial[OptunaTrial] | Iterable[Trial[OptunaTrial]]:
         """Ask the optimizer for a new config.
 
         Returns:
             The trial info for the new config.
         """
+        if n is not None:
+            return (self.ask(n=None) for _ in range(n))
+
         optuna_trial: optuna.Trial = self.study.ask(self.space)
         config = optuna_trial.params
         trial_number = optuna_trial.number
         unique_name = f"{trial_number=}"
         metrics = [self.metrics] if isinstance(self.metrics, Metric) else self.metrics
         return Trial(
             name=unique_name,
```

### Comparing `amltk-1.8.0/src/amltk/optimization/optimizers/smac.py` & `amltk-1.9.0/src/amltk/optimization/optimizers/smac.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 print(history.df())
 optimizer.bucket.rmdir()  # markdown-exec: hide
 ```
 """  # noqa: E501
 from __future__ import annotations
 
 import logging
-from collections.abc import Mapping, Sequence
+from collections.abc import Iterable, Mapping, Sequence
 from datetime import datetime
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Literal, overload
 from typing_extensions import override
 
 import numpy as np
 from more_itertools import first_true
@@ -245,21 +245,39 @@
             logging_level=logging_level,
             multi_objective_algorithm=facade_cls.get_multi_objective_algorithm(
                 scenario=scenario,
             ),
         )
         return cls(facade=facade, fidelities=fidelities, bucket=bucket, metrics=metrics)
 
+    @overload
+    def ask(self, n: int) -> Iterable[Trial[SMACTrialInfo]]:
+        ...
+
+    @overload
+    def ask(self, n: None = None) -> Trial[SMACTrialInfo]:
+        ...
+
     @override
-    def ask(self) -> Trial[SMACTrialInfo]:
+    def ask(
+        self,
+        n: int | None = None,
+    ) -> Trial[SMACTrialInfo] | Iterable[Trial[SMACTrialInfo]]:
         """Ask the optimizer for a new config.
 
+        Args:
+            n: The number of configs to ask for. If `None`, ask for a single config.
+
+
         Returns:
             The trial info for the new config.
         """
+        if n is not None:
+            return (self.ask(n=None) for _ in range(n))
+
         smac_trial_info = self.facade.ask()
         config = smac_trial_info.config
         budget = smac_trial_info.budget
         instance = smac_trial_info.instance
         seed = smac_trial_info.seed
 
         if self.fidelities and budget:
```

### Comparing `amltk-1.8.0/src/amltk/optimization/trial.py` & `amltk-1.9.0/src/amltk/optimization/trial.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/options.py` & `amltk-1.9.0/src/amltk/options.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/pipeline/builders/sklearn.py` & `amltk-1.9.0/src/amltk/pipeline/builders/sklearn.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/pipeline/components.py` & `amltk-1.9.0/src/amltk/pipeline/components.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,77 +1,15 @@
-"""You can use the various different node types to build a pipeline.
-
-You can connect these nodes together using either the constructors explicitly,
-as shown in the examples. We also provide some index operators:
-
-* `>>` - Connect nodes together to form a [`Sequential`][amltk.pipeline.components.Sequential]
-* `&` - Connect nodes together to form a [`Join`][amltk.pipeline.components.Join]
-* `|` - Connect nodes together to form a [`Choice`][amltk.pipeline.components.Choice]
-
-There is also another short-hand that you may find useful to know:
-
-* `{comp1, comp2, comp3}` - This will automatically be converted into a
-    [`Choice`][amltk.pipeline.Choice] between the given components.
-* `(comp1, comp2, comp3)` - This will automatically be converted into a
-    [`Join`][amltk.pipeline.Join] between the given components.
-* `[comp1, comp2, comp3]` - This will automatically be converted into a
-    [`Sequential`][amltk.pipeline.Sequential] between the given components.
-
-For each of these components we will show examples using
-the [`#! "sklearn"` builder][amltk.pipeline.builders.sklearn.build]
-
-The components are:
-
-### Component
-
-::: amltk.pipeline.components.Component
-    options:
-        members: false
-
-### Sequential
-
-::: amltk.pipeline.components.Sequential
-    options:
-        members: false
-
-### Choice
-
-::: amltk.pipeline.components.Choice
-    options:
-        members: false
-
-### Split
-
-::: amltk.pipeline.components.Split
-    options:
-        members: false
-
-### Join
-
-::: amltk.pipeline.components.Join
-    options:
-        members: false
-
-### Fixed
-
-::: amltk.pipeline.components.Fixed
-    options:
-        members: false
-
-### Searchable
-
-::: amltk.pipeline.components.Searchable
-    options:
-        members: false
-"""  # noqa: E501
+"""The provided subclasses of a [`Node`][amltk.pipeline.node.Node]
+that can be used can be assembled into a pipeline.
+"""
 from __future__ import annotations
 
 import inspect
 from collections.abc import Callable, Iterator, Mapping, Sequence
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, ClassVar, TypeVar, overload
 from typing_extensions import Self, override
 
 from more_itertools import all_unique, first_true
 
 from amltk._functional import entity_name, mapping_select
 from amltk.exceptions import (
@@ -155,148 +93,411 @@
         case thing if (inspect.isfunction(thing) or inspect.ismethod(thing)):
             return Component(thing, name=name)
         case _:
             return Fixed(thing, name=name)
 
 
 @dataclass(init=False, frozen=True, eq=True)
-class Join(Node[Item, Space]):
-    """[`Join`][amltk.pipeline.Join] together different parts of the pipeline.
+class Component(Node[Item, Space]):
+    """A [`Component`][amltk.pipeline.Component] of the pipeline with
+    a possible item and **no children**.
 
-    This indicates the different children in
-    [`.nodes`][amltk.pipeline.Node.nodes] should act in tandem with one
-    another, for example, concatenating the outputs of the various members of the
-    `Join`.
+    This is the basic building block of most pipelines, it accepts
+    as it's [`item=`][amltk.pipeline.node.Node.item] some function that will be
+    called with [`build_item()`][amltk.pipeline.components.Component.build_item] to
+    build that one part of the pipeline.
+
+    When [`build_item()`][amltk.pipeline.Component.build_item] is called, whatever
+    the config of the component is at that time, will be used to construct the item.
+
+    A common pattern is to use a [`Component`][amltk.pipeline.Component] to
+    wrap a constructor, specifying the [`space=`][amltk.pipeline.node.Node.space]
+    and [`config=`][amltk.pipeline.node.Node.config] to be used when building the
+    item.
 
     ```python exec="true" source="material-block" html="true"
-    from amltk.pipeline import Join, Component
-    from sklearn.decomposition import PCA
-    from sklearn.feature_selection import SelectKBest
+    from amltk.pipeline import Component
+    from sklearn.ensemble import RandomForestClassifier
 
-    pca = Component(PCA, space={"n_components": (1, 3)})
-    kbest = Component(SelectKBest, space={"k": (1, 3)})
+    rf = Component(
+        RandomForestClassifier,
+        config={"max_depth": 3},
+        space={"n_estimators": (10, 100)}
+    )
+    from amltk._doc import doc_print; doc_print(print, rf)  # markdown-exec: hide
 
-    join = Join(pca, kbest, name="my_feature_union")
-    from amltk._doc import doc_print; doc_print(print, join)  # markdown-exec: hide
+    config = {"n_estimators": 50}  # Sample from some space or something
+    configured_rf = rf.configure(config)
 
-    space = join.search_space("configspace")
-    from amltk._doc import doc_print; doc_print(print, space)  # markdown-exec: hide
+    estimator = configured_rf.build_item()
+    from amltk._doc import doc_print; doc_print(print, estimator)  # markdown-exec: hide
+    ```
 
-    pipeline = join.build("sklearn")
-    from amltk._doc import doc_print; doc_print(print, pipeline)  # markdown-exec: hide
+    See Also:
+        * [`Node`][amltk.pipeline.node.Node]
+    """
+
+    item: Callable[..., Item]
+    """A node which constructs an item in the pipeline."""
+
+    nodes: tuple[()]
+    """A component has no children."""
+
+    RICH_OPTIONS: ClassVar[RichOptions] = RichOptions(panel_color="#E6AF2E")
+
+    _NODES_INIT: ClassVar = None
+
+    def __init__(
+        self,
+        item: Callable[..., Item],
+        *,
+        name: str | None = None,
+        config: Config | None = None,
+        space: Space | None = None,
+        fidelities: Mapping[str, Any] | None = None,
+        config_transform: Callable[[Config, Any], Config] | None = None,
+        meta: Mapping[str, Any] | None = None,
+    ):
+        """Initialize a component.
+
+        Args:
+            item: The item attached to this node.
+            name: The name of the node. If not specified, the name will be
+                generated from the item.
+            config: The configuration for this node.
+            space: The search space for this node. This will be used when
+                [`search_space()`][amltk.pipeline.node.Node.search_space] is called.
+            fidelities: The fidelities for this node.
+            config_transform: A function that transforms the `config=` parameter
+                during [`configure(config)`][amltk.pipeline.node.Node.configure]
+                before return the new configured node. Useful for times where
+                you need to combine multiple parameters into one.
+            meta: Any meta information about this node.
+        """
+        super().__init__(
+            name=name if name is not None else entity_name(item),
+            item=item,
+            config=config,
+            space=space,
+            fidelities=fidelities,
+            config_transform=config_transform,
+            meta=meta,
+        )
+
+    def build_item(self, **kwargs: Any) -> Item:
+        """Build the item attached to this component.
+
+        Args:
+            **kwargs: Any additional arguments to pass to the item
+
+        Returns:
+            Item
+                The built item
+        """
+        config = self.config or {}
+        try:
+            return self.item(**{**config, **kwargs})
+        except TypeError as e:
+            new_msg = f"Failed to build `{self.item=}` with `{self.config=}`.\n"
+            if any(kwargs):
+                new_msg += f"Extra {kwargs=} were also provided.\n"
+            new_msg += (
+                "If the item failed to initialize, a common reason can be forgetting"
+                " to call `configure()` on the `Component` or the pipeline it is in or"
+                " not calling `build()`/`build_item()` on the **returned** value of"
+                " `configure()`.\n"
+                "Reasons may also include not having fully specified the `config`"
+                " initially, it having not being configured fully from `configure()`"
+                " or from misspecfying parameters in the `space`."
+            )
+            raise ComponentBuildError(new_msg) from e
+
+
+@dataclass(init=False, frozen=True, eq=True)
+class Searchable(Node[None, Space]):  # type: ignore
+    """A [`Searchable`][amltk.pipeline.Searchable]
+    node of the pipeline which just represents a search space, no item attached.
+
+    While not usually applicable to pipelines you want to build, this node
+    is useful for creating a search space, especially if the real pipeline you
+    want to optimize can not be built directly. For example, if you are optimize
+    a script, you may wish to use a `Searchable` to represent the search space
+    of that script.
+
+    ```python exec="true" source="material-block" html="true"
+    from amltk.pipeline import Searchable
+
+    script_space = Searchable({"mode": ["orange", "blue", "red"], "n": (10, 100)})
+    from amltk._doc import doc_print; doc_print(print, script_space)  # markdown-exec: hide
     ```
 
-    You may also just join together nodes using an infix operator `&` if you prefer:
+    See Also:
+        * [`Node`][amltk.pipeline.node.Node]
+    """  # noqa: E501
+
+    item: None = None
+    """A searchable has no item."""
+
+    nodes: tuple[()] = ()
+    """A searchable has no children."""
+
+    RICH_OPTIONS: ClassVar[RichOptions] = RichOptions(panel_color="light_steel_blue")
+
+    _NODES_INIT: ClassVar = None
+
+    def __init__(
+        self,
+        space: Space | None = None,
+        *,
+        name: str | None = None,
+        config: Config | None = None,
+        fidelities: Mapping[str, Any] | None = None,
+        config_transform: Callable[[Config, Any], Config] | None = None,
+        meta: Mapping[str, Any] | None = None,
+    ):
+        """Initialize a choice.
+
+        Args:
+            space: The search space for this node. This will be used when
+                [`search_space()`][amltk.pipeline.node.Node.search_space] is called.
+            name: The name of the node. If not specified, a random one will
+                be generated.
+            config: The configuration for this node. Useful for setting some
+                default values.
+            fidelities: The fidelities for this node.
+            config_transform: A function that transforms the `config=` parameter
+                during [`configure(config)`][amltk.pipeline.node.Node.configure]
+                before return the new configured node. Useful for times where
+                you need to combine multiple parameters into one.
+            meta: Any meta information about this node.
+        """
+        if name is None:
+            name = f"Searchable-{randuid(8)}"
+
+        super().__init__(
+            name=name,
+            config=config,
+            space=space,
+            fidelities=fidelities,
+            config_transform=config_transform,
+            meta=meta,
+        )
+
+
+@dataclass(init=False, frozen=True, eq=True)
+class Fixed(Node[Item, None]):  # type: ignore
+    """A [`Fixed`][amltk.pipeline.Fixed] part of the pipeline that
+    represents something that can not be configured and used directly as is.
+
+    It consists of an [`.item`][amltk.pipeline.node.Node.item] that is fixed,
+    non-configurable and non-searchable. It also has no children.
+
+    This is useful for representing parts of the pipeline that are fixed, for example
+    if you have a pipeline that is a `Sequential` of nodes, but you want to
+    fix the first component to be a `PCA` with `n_components=3`, you can use a `Fixed`
+    to represent that.
 
     ```python exec="true" source="material-block" html="true"
-    from amltk.pipeline import Join, Component
+    from amltk.pipeline import Component, Fixed, Sequential
+    from sklearn.ensemble import RandomForestClassifier
     from sklearn.decomposition import PCA
-    from sklearn.feature_selection import SelectKBest
 
-    pca = Component(PCA, space={"n_components": (1, 3)})
-    kbest = Component(SelectKBest, space={"k": (1, 3)})
-
-    # Can not parametrize or name the join
-    join = pca & kbest
-    from amltk._doc import doc_print; doc_print(print, join)  # markdown-exec: hide
+    rf = Component(RandomForestClassifier, space={"n_estimators": (10, 100)})
+    pca = Fixed(PCA(n_components=3))
 
-    # With a parametrized join
-    join = (
-        Join(name="my_feature_union") & pca & kbest
-    )
-    item = join.build("sklearn")
-    print(item._repr_html_())  # markdown-exec: hide
+    pipeline = Sequential(pca, rf, name="my_pipeline")
+    from amltk._doc import doc_print; doc_print(print, pipeline)  # markdown-exec: hide
     ```
 
-    Whenever some other node sees a tuple, i.e. `(comp1, comp2, comp3)`, this
-    will automatically be converted into a `Join`.
+    See Also:
+        * [`Node`][amltk.pipeline.node.Node]
+    """
+
+    item: Item
+    """The fixed item that this node represents."""
+
+    space: None = None
+    """A fixed node has no search space."""
+
+    fidelities: None = None
+    """A fixed node has no search space."""
+
+    config: None = None
+    """A fixed node has no config."""
+
+    config_transform: None = None
+    """A fixed node has no config so no transform."""
+
+    nodes: tuple[()] = ()
+    """A fixed node has no children."""
+
+    RICH_OPTIONS: ClassVar[RichOptions] = RichOptions(panel_color="#56351E")
+
+    _NODES_INIT: ClassVar = None
+
+    def __init__(  # noqa: D417
+        self,
+        item: Item,
+        *,
+        name: str | None = None,
+        config: None = None,
+        space: None = None,
+        fidelities: None = None,
+        config_transform: None = None,
+        meta: Mapping[str, Any] | None = None,
+    ):
+        """Initialize a fixed node.
+
+        Args:
+            item: The item attached to this node. Will be fixed and can not
+                be configured.
+            name: The name of the node. If not specified, the name will be
+                generated from the item.
+            meta: Any meta information about this node.
+        """
+        super().__init__(
+            name=name if name is not None else entity_name(item),
+            item=item,
+            config=config,
+            space=space,
+            fidelities=fidelities,
+            config_transform=config_transform,
+            meta=meta,
+        )
+
+
+@dataclass(init=False, frozen=True, eq=True)
+class Sequential(Node[Item, Space]):
+    """A [`Sequential`][amltk.pipeline.Sequential] set of operations in a pipeline.
+
+    This indicates the different children in
+    [`.nodes`][amltk.pipeline.Node.nodes] should act one after
+    another, feeding the output of one into the next.
 
     ```python exec="true" source="material-block" html="true"
-    from amltk.pipeline import Sequential, Component
+    from amltk.pipeline import Component, Sequential
     from sklearn.decomposition import PCA
-    from sklearn.feature_selection import SelectKBest
     from sklearn.ensemble import RandomForestClassifier
 
-    pca = Component(PCA, space={"n_components": (1, 3)})
-    kbest = Component(SelectKBest, space={"k": (1, 3)})
-
-    # Can not parametrize or name the join
-    join = Sequential(
-        (pca, kbest),
-        RandomForestClassifier(n_estimators=5),
-        name="my_feature_union",
+    pipeline = Sequential(
+        PCA(n_components=3),
+        Component(RandomForestClassifier, space={"n_estimators": (10, 100)}),
+        name="my_pipeline"
     )
-    from amltk._doc import doc_print; doc_print(print, join)  # markdown-exec: hide
+    from amltk._doc import doc_print; doc_print(print, pipeline)  # markdown-exec: hide
     ```
 
-    Like all [`Node`][amltk.pipeline.node.Node]s, a `Join` accepts an explicit
-    [`name=`][amltk.pipeline.node.Node.name],
-    [`item=`][amltk.pipeline.node.Node.item],
-    [`config=`][amltk.pipeline.node.Node.config],
-    [`space=`][amltk.pipeline.node.Node.space],
-    [`fidelities=`][amltk.pipeline.node.Node.fidelities],
-    [`config_transform=`][amltk.pipeline.node.Node.config_transform] and
-    [`meta=`][amltk.pipeline.node.Node.meta].
-
     See Also:
         * [`Node`][amltk.pipeline.node.Node]
     """
 
     nodes: tuple[Node, ...]
-    """The nodes that this node leads to."""
-
-    RICH_OPTIONS: ClassVar[RichOptions] = RichOptions(panel_color="#7E6B8F")
+    """The nodes ordered in series."""
 
+    RICH_OPTIONS: ClassVar[RichOptions] = RichOptions(
+        panel_color="#7E6B8F",
+        node_orientation="vertical",
+    )
     _NODES_INIT: ClassVar = "args"
 
     def __init__(
         self,
         *nodes: Node | NodeLike,
         name: str | None = None,
         item: Item | Callable[[Item], Item] | None = None,
         config: Config | None = None,
         space: Space | None = None,
         fidelities: Mapping[str, Any] | None = None,
         config_transform: Callable[[Config, Any], Config] | None = None,
         meta: Mapping[str, Any] | None = None,
     ):
-        """See [`Node`][amltk.pipeline.node.Node] for details."""
+        """Initialize a sequential node.
+
+        Args:
+            nodes: The nodes that this node leads to. In the case of a `Sequential`,
+                the order here matters and it signifies that data should first
+                be passed through the first node, then the second, etc.
+            item: The item attached to this node (if any).
+            name: The name of the node. If not specified, the name will be
+                randomly generated.
+            config: The configuration for this node.
+            space: The search space for this node. This will be used when
+                [`search_space()`][amltk.pipeline.node.Node.search_space] is called.
+            fidelities: The fidelities for this node.
+            config_transform: A function that transforms the `config=` parameter
+                during [`configure(config)`][amltk.pipeline.node.Node.configure]
+                before return the new configured node. Useful for times where
+                you need to combine multiple parameters into one.
+            meta: Any meta information about this node.
+        """
         _nodes = tuple(as_node(n) for n in nodes)
+
+        # Perhaps we need to do a deeper check on this...
         if not all_unique(_nodes, key=lambda node: node.name):
-            raise ValueError(
-                f"Can't handle nodes they do not all contain unique names, {nodes=}."
-                "\nAll nodes must have a unique name. Please provide a `name=` to them",
-            )
+            raise DuplicateNamesError(self)
 
         if name is None:
-            name = f"Join-{randuid(8)}"
+            name = f"Seq-{randuid(8)}"
 
         super().__init__(
             *_nodes,
             name=name,
             item=item,
             config=config,
             space=space,
             fidelities=fidelities,
             config_transform=config_transform,
             meta=meta,
         )
 
+    @property
+    def tail(self) -> Node:
+        """The last step in the pipeline."""
+        return self.nodes[-1]
+
+    def __len__(self) -> int:
+        """Get the number of nodes in the pipeline."""
+        return len(self.nodes)
+
     @override
-    def __and__(self, other: Node | NodeLike) -> Join:
+    def __rshift__(self, other: Node | NodeLike) -> Sequential:
         other_node = as_node(other)
         if any(other_node.name == node.name for node in self.nodes):
             raise ValueError(
                 f"Can't handle node with name '{other_node.name} as"
                 f" there is already a node called '{other_node.name}' in {self.name}",
             )
 
         nodes = (*tuple(as_node(n) for n in self.nodes), other_node)
         return self.mutate(name=self.name, nodes=nodes)
 
+    @override
+    def walk(
+        self,
+        path: Sequence[Node] | None = None,
+    ) -> Iterator[tuple[list[Node], Node]]:
+        """Walk the nodes in this chain.
+
+        Args:
+            path: The current path to this node
+
+        Yields:
+            The parents of the node and the node itself
+        """
+        path = list(path) if path is not None else []
+        yield path, self
+
+        path = [*path, self]
+        for node in self.nodes:
+            yield from node.walk(path=path)
+
+            # Append the previous node so that the next node in the sequence is
+            # lead to from the previous node
+            path = [*path, node]
+
 
 @dataclass(init=False, frozen=True, eq=True)
 class Choice(Node[Item, Space]):
     """A [`Choice`][amltk.pipeline.Choice] between different subcomponents.
 
     This indicates that a choice should be made between the different children in
     [`.nodes`][amltk.pipeline.Node.nodes], usually done when you
@@ -309,90 +510,30 @@
     from sklearn.neural_network import MLPClassifier
 
     rf = Component(RandomForestClassifier, space={"n_estimators": (10, 100)})
     mlp = Component(MLPClassifier, space={"activation": ["logistic", "relu", "tanh"]})
 
     estimator_choice = Choice(rf, mlp, name="estimator")
     from amltk._doc import doc_print; doc_print(print, estimator_choice)  # markdown-exec: hide
-
-    space = estimator_choice.search_space("configspace")
-    from amltk._doc import doc_print; doc_print(print, space)  # markdown-exec: hide
-
-    config = space.sample_configuration()
-    from amltk._doc import doc_print; doc_print(print, config)  # markdown-exec: hide
-
-    configured_choice = estimator_choice.configure(config)
-    from amltk._doc import doc_print; doc_print(print, configured_choice)  # markdown-exec: hide
-
-    chosen_estimator = configured_choice.chosen()
-    from amltk._doc import doc_print; doc_print(print, chosen_estimator)  # markdown-exec: hide
-
-    estimator = chosen_estimator.build_item()
-    from amltk._doc import doc_print; doc_print(print, estimator)  # markdown-exec: hide
-    ```
-
-    You may also just add nodes to a `Choice` using an infix operator `|` if you prefer:
-
-    ```python exec="true" source="material-block" html="true"
-    from amltk.pipeline import Choice, Component
-    from sklearn.ensemble import RandomForestClassifier
-    from sklearn.neural_network import MLPClassifier
-
-    rf = Component(RandomForestClassifier, space={"n_estimators": (10, 100)})
-    mlp = Component(MLPClassifier, space={"activation": ["logistic", "relu", "tanh"]})
-
-    estimator_choice = (
-        Choice(name="estimator") | mlp | rf
-    )
-    from amltk._doc import doc_print; doc_print(print, estimator_choice)  # markdown-exec: hide
-    ```
-
-    Whenever some other node sees a set, i.e. `{comp1, comp2, comp3}`, this
-    will automatically be converted into a `Choice`.
-
-    ```python exec="true" source="material-block" html="true"
-    from amltk.pipeline import Choice, Component, Sequential
-    from sklearn.ensemble import RandomForestClassifier
-    from sklearn.neural_network import MLPClassifier
-    from sklearn.impute import SimpleImputer
-
-    rf = Component(RandomForestClassifier, space={"n_estimators": (10, 100)})
-    mlp = Component(MLPClassifier, space={"activation": ["logistic", "relu", "tanh"]})
-
-    pipeline = Sequential(
-        SimpleImputer(fill_value=0),
-        {mlp, rf},
-        name="my_pipeline",
-    )
-    from amltk._doc import doc_print; doc_print(print, pipeline)  # markdown-exec: hide
     ```
 
-    Like all [`Node`][amltk.pipeline.node.Node]s, a `Choice` accepts an explicit
-    [`name=`][amltk.pipeline.node.Node.name],
-    [`item=`][amltk.pipeline.node.Node.item],
-    [`config=`][amltk.pipeline.node.Node.config],
-    [`space=`][amltk.pipeline.node.Node.space],
-    [`fidelities=`][amltk.pipeline.node.Node.fidelities],
-    [`config_transform=`][amltk.pipeline.node.Node.config_transform] and
-    [`meta=`][amltk.pipeline.node.Node.meta].
-
     !!! warning "Order of nodes"
 
         The given nodes of a choice are always ordered according
         to their name, so indexing `choice.nodes` may not be reliable
         if modifying the choice dynamically.
 
         Please use `choice["name"]` to access the nodes instead.
 
     See Also:
         * [`Node`][amltk.pipeline.node.Node]
     """  # noqa: E501
 
     nodes: tuple[Node, ...]
-    """The nodes that this node leads to."""
+    """The choice of possible nodes that this choice could take."""
 
     RICH_OPTIONS: ClassVar[RichOptions] = RichOptions(panel_color="#FF4500")
     _NODES_INIT: ClassVar = "args"
 
     def __init__(
         self,
         *nodes: Node | NodeLike,
@@ -400,15 +541,31 @@
         item: Item | Callable[[Item], Item] | None = None,
         config: Config | None = None,
         space: Space | None = None,
         fidelities: Mapping[str, Any] | None = None,
         config_transform: Callable[[Config, Any], Config] | None = None,
         meta: Mapping[str, Any] | None = None,
     ):
-        """See [`Node`][amltk.pipeline.node.Node] for details."""
+        """Initialize a choice node.
+
+        Args:
+            nodes: The nodes that should be chosen between for this node.
+            item: The item attached to this node (if any).
+            name: The name of the node. If not specified, the name will be
+                randomly generated.
+            config: The configuration for this node.
+            space: The search space for this node. This will be used when
+                [`search_space()`][amltk.pipeline.node.Node.search_space] is called.
+            fidelities: The fidelities for this node.
+            config_transform: A function that transforms the `config=` parameter
+                during [`configure(config)`][amltk.pipeline.node.Node.configure]
+                before return the new configured node. Useful for times where
+                you need to combine multiple parameters into one.
+            meta: Any meta information about this node.
+        """
         _nodes: tuple[Node, ...] = tuple(
             sorted((as_node(n) for n in nodes), key=lambda n: n.name),
         )
         if not all_unique(_nodes, key=lambda node: node.name):
             raise ValueError(
                 f"Can't handle nodes as we can not generate a __choice__ for {nodes=}."
                 "\nAll nodes must have a unique name. Please provide a `name=` to them",
@@ -579,180 +736,14 @@
         if len(this_config) > 0:
             _kwargs["config"] = dict(this_config)
 
         return self.mutate(**_kwargs)
 
 
 @dataclass(init=False, frozen=True, eq=True)
-class Sequential(Node[Item, Space]):
-    """A [`Sequential`][amltk.pipeline.Sequential] set of operations in a pipeline.
-
-    This indicates the different children in
-    [`.nodes`][amltk.pipeline.Node.nodes] should act one after
-    another, feeding the output of one into the next.
-
-    ```python exec="true" source="material-block" html="true"
-    from amltk.pipeline import Component, Sequential
-    from sklearn.decomposition import PCA
-    from sklearn.ensemble import RandomForestClassifier
-
-    pipeline = Sequential(
-        PCA(n_components=3),
-        Component(RandomForestClassifier, space={"n_estimators": (10, 100)}),
-        name="my_pipeline"
-    )
-    from amltk._doc import doc_print; doc_print(print, pipeline)  # markdown-exec: hide
-
-    space = pipeline.search_space("configspace")
-    from amltk._doc import doc_print; doc_print(print, space)  # markdown-exec: hide
-
-    configuration = space.sample_configuration()
-    from amltk._doc import doc_print; doc_print(print, configuration)  # markdown-exec: hide
-
-    configured_pipeline = pipeline.configure(configuration)
-    from amltk._doc import doc_print; doc_print(print, configured_pipeline)  # markdown-exec: hide
-
-    sklearn_pipeline = pipeline.build("sklearn")
-    print(sklearn_pipeline._repr_html_())  # markdown-exec: hide
-    ```
-
-    You may also just chain together nodes using an infix operator `>>` if you prefer:
-
-    ```python exec="true" source="material-block" html="true"
-    from amltk.pipeline import Join, Component, Sequential
-    from sklearn.decomposition import PCA
-    from sklearn.ensemble import RandomForestClassifier
-
-    pipeline = (
-        Sequential(name="my_pipeline")
-        >> PCA(n_components=3)
-        >> Component(RandomForestClassifier, space={"n_estimators": (10, 100)})
-    )
-    from amltk._doc import doc_print; doc_print(print, pipeline)  # markdown-exec: hide
-    ```
-
-    Whenever some other node sees a list, i.e. `[comp1, comp2, comp3]`, this
-    will automatically be converted into a `Sequential`.
-
-    ```python exec="true" source="material-block" html="true"
-    from amltk.pipeline import Choice
-    from sklearn.impute import SimpleImputer
-    from sklearn.preprocessing import StandardScaler
-    from sklearn.ensemble import RandomForestClassifier
-    from sklearn.neural_network import MLPClassifier
-
-    pipeline_choice = Choice(
-        [SimpleImputer(), RandomForestClassifier()],
-        [StandardScaler(), MLPClassifier()],
-        name="pipeline_choice"
-    )
-    from amltk._doc import doc_print; doc_print(print, pipeline_choice)  # markdown-exec: hide
-    ```
-
-    Like all [`Node`][amltk.pipeline.node.Node]s, a `Sequential` accepts an explicit
-    [`name=`][amltk.pipeline.node.Node.name],
-    [`item=`][amltk.pipeline.node.Node.item],
-    [`config=`][amltk.pipeline.node.Node.config],
-    [`space=`][amltk.pipeline.node.Node.space],
-    [`fidelities=`][amltk.pipeline.node.Node.fidelities],
-    [`config_transform=`][amltk.pipeline.node.Node.config_transform] and
-    [`meta=`][amltk.pipeline.node.Node.meta].
-
-    See Also:
-        * [`Node`][amltk.pipeline.node.Node]
-    """  # noqa: E501
-
-    nodes: tuple[Node, ...]
-    """The nodes in series."""
-
-    RICH_OPTIONS: ClassVar[RichOptions] = RichOptions(
-        panel_color="#7E6B8F",
-        node_orientation="vertical",
-    )
-    _NODES_INIT: ClassVar = "args"
-
-    def __init__(
-        self,
-        *nodes: Node | NodeLike,
-        name: str | None = None,
-        item: Item | Callable[[Item], Item] | None = None,
-        config: Config | None = None,
-        space: Space | None = None,
-        fidelities: Mapping[str, Any] | None = None,
-        config_transform: Callable[[Config, Any], Config] | None = None,
-        meta: Mapping[str, Any] | None = None,
-    ):
-        """See [`Node`][amltk.pipeline.node.Node] for details."""
-        _nodes = tuple(as_node(n) for n in nodes)
-
-        # Perhaps we need to do a deeper check on this...
-        if not all_unique(_nodes, key=lambda node: node.name):
-            raise DuplicateNamesError(self)
-
-        if name is None:
-            name = f"Seq-{randuid(8)}"
-
-        super().__init__(
-            *_nodes,
-            name=name,
-            item=item,
-            config=config,
-            space=space,
-            fidelities=fidelities,
-            config_transform=config_transform,
-            meta=meta,
-        )
-
-    @property
-    def tail(self) -> Node:
-        """The last step in the pipeline."""
-        return self.nodes[-1]
-
-    def __len__(self) -> int:
-        """Get the number of nodes in the pipeline."""
-        return len(self.nodes)
-
-    @override
-    def __rshift__(self, other: Node | NodeLike) -> Sequential:
-        other_node = as_node(other)
-        if any(other_node.name == node.name for node in self.nodes):
-            raise ValueError(
-                f"Can't handle node with name '{other_node.name} as"
-                f" there is already a node called '{other_node.name}' in {self.name}",
-            )
-
-        nodes = (*tuple(as_node(n) for n in self.nodes), other_node)
-        return self.mutate(name=self.name, nodes=nodes)
-
-    @override
-    def walk(
-        self,
-        path: Sequence[Node] | None = None,
-    ) -> Iterator[tuple[list[Node], Node]]:
-        """Walk the nodes in this chain.
-
-        Args:
-            path: The current path to this node
-
-        Yields:
-            The parents of the node and the node itself
-        """
-        path = list(path) if path is not None else []
-        yield path, self
-
-        path = [*path, self]
-        for node in self.nodes:
-            yield from node.walk(path=path)
-
-            # Append the previous node so that the next node in the sequence is
-            # lead to from the previous node
-            path = [*path, node]
-
-
-@dataclass(init=False, frozen=True, eq=True)
 class Split(Node[Item, Space]):
     """A [`Split`][amltk.pipeline.Split] of data in a pipeline.
 
     This indicates the different children in
     [`.nodes`][amltk.pipeline.Node.nodes] should
     act in parallel but on different subsets of data.
 
@@ -770,61 +761,26 @@
 
     preprocessor = Split(
         {
             "categories": categorical_pipeline,
             "numerical": numerical_pipeline,
         },
         config={
-            # This is how you would configure the split for the sklearn builder in particular
             "categories": make_column_selector(dtype_include="category"),
             "numerical": make_column_selector(dtype_exclude="category"),
         },
         name="my_split"
     )
     from amltk._doc import doc_print; doc_print(print, preprocessor)  # markdown-exec: hide
-
-    space = preprocessor.search_space("configspace")
-    from amltk._doc import doc_print; doc_print(print, space)  # markdown-exec: hide
-
-    configuration = space.sample_configuration()
-    from amltk._doc import doc_print; doc_print(print, configuration)  # markdown-exec: hide
-
-    configured_preprocessor = preprocessor.configure(configuration)
-    from amltk._doc import doc_print; doc_print(print, configured_preprocessor)  # markdown-exec: hide
-
-    built_preprocessor = configured_preprocessor.build("sklearn")
-    print(built_preprocessor._repr_html_())  # markdown-exec: hide
     ```
 
-    The split is a slight oddity when compared to the other kinds of components in that
-    it allows a `dict` as it's first argument, where the keys are the names of the
-    different paths through which data will go and the values are the actual nodes that
-    will receive the data.
-
-    If nodes are passed in as they are for all other components, usually the name of the
-    first node will be important for any builder trying to make sense of how
-    to use the `Split`
-
-
-    Like all [`Node`][amltk.pipeline.node.Node]s, a `Split` accepts an explicit
-    [`name=`][amltk.pipeline.node.Node.name],
-    [`item=`][amltk.pipeline.node.Node.item],
-    [`config=`][amltk.pipeline.node.Node.config],
-    [`space=`][amltk.pipeline.node.Node.space],
-    [`fidelities=`][amltk.pipeline.node.Node.fidelities],
-    [`config_transform=`][amltk.pipeline.node.Node.config_transform] and
-    [`meta=`][amltk.pipeline.node.Node.meta].
-
     See Also:
         * [`Node`][amltk.pipeline.node.Node]
     """  # noqa: E501
 
-    nodes: tuple[Node, ...]
-    """The nodes that this node leads to."""
-
     RICH_OPTIONS: ClassVar[RichOptions] = RichOptions(
         panel_color="#777DA7",
         node_orientation="horizontal",
     )
 
     _NODES_INIT: ClassVar = "args"
 
@@ -835,15 +791,34 @@
         item: Item | Callable[[Item], Item] | None = None,
         config: Config | None = None,
         space: Space | None = None,
         fidelities: Mapping[str, Any] | None = None,
         config_transform: Callable[[Config, Any], Config] | None = None,
         meta: Mapping[str, Any] | None = None,
     ):
-        """See [`Node`][amltk.pipeline.node.Node] for details."""
+        """Initialize a split node.
+
+        Args:
+            nodes: The nodes that this node leads to. You may also provide
+                a dictionary where the keys are the names of the nodes and
+                the values are the nodes or list of nodes themselves.
+            item: The item attached to this node. The object created by `item`
+                should be capable of figuring out how to deal with its child nodes.
+            name: The name of the node. If not specified, the name will be
+                generated from the item.
+            config: The configuration for this split.
+            space: The search space for this node. This will be used when
+                [`search_space()`][amltk.pipeline.node.Node.search_space] is called.
+            fidelities: The fidelities for this node.
+            config_transform: A function that transforms the `config=` parameter
+                during [`configure(config)`][amltk.pipeline.node.Node.configure]
+                before return the new configured node. Useful for times where
+                you need to combine multiple parameters into one.
+            meta: Any meta information about this node.
+        """
         if any(isinstance(n, dict) for n in nodes):
             if len(nodes) > 1:
                 raise ValueError(
                     "Can't handle multiple nodes with a dictionary as a node.\n"
                     f"{nodes=}",
                 )
             _node = nodes[0]
@@ -880,293 +855,97 @@
             fidelities=fidelities,
             config_transform=config_transform,
             meta=meta,
         )
 
 
 @dataclass(init=False, frozen=True, eq=True)
-class Component(Node[Item, Space]):
-    """A [`Component`][amltk.pipeline.Component] of the pipeline with
-    a possible item and **no children**.
-
-    This is the basic building block of most pipelines, it accepts
-    as it's [`item=`][amltk.pipeline.node.Node.item] some function that will be
-    called with [`build_item()`][amltk.pipeline.components.Component.build_item] to
-    build that one part of the pipeline.
-
-    When [`build_item()`][amltk.pipeline.Component.build_item] is called,
-    The [`.config`][amltk.pipeline.node.Node.config] on this node will be passed
-    to the function to build the item.
+class Join(Node[Item, Space]):
+    """[`Join`][amltk.pipeline.Join] together different parts of the pipeline.
 
-    A common pattern is to use a [`Component`][amltk.pipeline.Component] to
-    wrap a constructor, specifying the [`space=`][amltk.pipeline.node.Node.space]
-    and [`config=`][amltk.pipeline.node.Node.config] to be used when building the
-    item.
+    This indicates the different children in
+    [`.nodes`][amltk.pipeline.Node.nodes] should act in tandem with one
+    another, for example, concatenating the outputs of the various members of the
+    `Join`.
 
     ```python exec="true" source="material-block" html="true"
-    from amltk.pipeline import Component
-    from sklearn.ensemble import RandomForestClassifier
-
-    rf = Component(
-        RandomForestClassifier,
-        config={"max_depth": 3},
-        space={"n_estimators": (10, 100)}
-    )
-    from amltk._doc import doc_print; doc_print(print, rf)  # markdown-exec: hide
-
-    config = {"n_estimators": 50}  # Sample from some space or something
-    configured_rf = rf.configure(config)
-
-    estimator = configured_rf.build_item()
-    from amltk._doc import doc_print; doc_print(print, estimator)  # markdown-exec: hide
-    ```
-
-    Whenever some other node sees a function/constructor, i.e. `RandomForestClassifier`,
-    this will automatically be converted into a `Component`.
+    from amltk.pipeline import Join, Component
+    from sklearn.decomposition import PCA
+    from sklearn.feature_selection import SelectKBest
 
-    ```python exec="true" source="material-block" html="true"
-    from amltk.pipeline import Sequential
-    from sklearn.ensemble import RandomForestClassifier
+    pca = Component(PCA, space={"n_components": (1, 3)})
+    kbest = Component(SelectKBest, space={"k": (1, 3)})
 
-    pipeline = Sequential(RandomForestClassifier, name="my_pipeline")
-    from amltk._doc import doc_print; doc_print(print, pipeline)  # markdown-exec: hide
+    join = Join(pca, kbest, name="my_feature_union")
+    from amltk._doc import doc_print; doc_print(print, join)  # markdown-exec: hide
     ```
 
-    The default `.name` of a component is the name of the class/function that it will
-    use. You can explicitly set the `name=` if you want to when constructing the
-    component.
-
-    Like all [`Node`][amltk.pipeline.node.Node]s, a `Component` accepts an explicit
-    [`name=`][amltk.pipeline.node.Node.name],
-    [`item=`][amltk.pipeline.node.Node.item],
-    [`config=`][amltk.pipeline.node.Node.config],
-    [`space=`][amltk.pipeline.node.Node.space],
-    [`fidelities=`][amltk.pipeline.node.Node.fidelities],
-    [`config_transform=`][amltk.pipeline.node.Node.config_transform] and
-    [`meta=`][amltk.pipeline.node.Node.meta].
-
     See Also:
         * [`Node`][amltk.pipeline.node.Node]
     """
 
-    item: Callable[..., Item]
-    """A node which constructs an item in the pipeline."""
-
-    nodes: tuple[()]
-    """A component has no children."""
-
-    RICH_OPTIONS: ClassVar[RichOptions] = RichOptions(panel_color="#E6AF2E")
+    nodes: tuple[Node, ...]
+    """The nodes that should be joined together in parallel."""
 
-    _NODES_INIT: ClassVar = None
+    RICH_OPTIONS: ClassVar[RichOptions] = RichOptions(panel_color="#7E6B8F")
+    _NODES_INIT: ClassVar = "args"
 
     def __init__(
         self,
-        item: Callable[..., Item],
-        *,
+        *nodes: Node | NodeLike,
         name: str | None = None,
+        item: Item | Callable[[Item], Item] | None = None,
         config: Config | None = None,
         space: Space | None = None,
         fidelities: Mapping[str, Any] | None = None,
         config_transform: Callable[[Config, Any], Config] | None = None,
         meta: Mapping[str, Any] | None = None,
     ):
-        """See [`Node`][amltk.pipeline.node.Node] for details."""
-        super().__init__(
-            name=name if name is not None else entity_name(item),
-            item=item,
-            config=config,
-            space=space,
-            fidelities=fidelities,
-            config_transform=config_transform,
-            meta=meta,
-        )
-
-    def build_item(self, **kwargs: Any) -> Item:
-        """Build the item attached to this component.
+        """Initialize a join node.
 
         Args:
-            **kwargs: Any additional arguments to pass to the item
-
-        Returns:
-            Item
-                The built item
+            nodes: The nodes that should be joined together in parallel.
+            item: The item attached to this node (if any).
+            name: The name of the node. If not specified, the name will be
+                randomly generated.
+            config: The configuration for this node.
+            space: The search space for this node. This will be used when
+                [`search_space()`][amltk.pipeline.node.Node.search_space] is called.
+            fidelities: The fidelities for this node.
+            config_transform: A function that transforms the `config=` parameter
+                during [`configure(config)`][amltk.pipeline.node.Node.configure]
+                before return the new configured node. Useful for times where
+                you need to combine multiple parameters into one.
+            meta: Any meta information about this node.
         """
-        config = self.config or {}
-        try:
-            return self.item(**{**config, **kwargs})
-        except TypeError as e:
-            new_msg = f"Failed to build `{self.item=}` with `{self.config=}`.\n"
-            if any(kwargs):
-                new_msg += f"Extra {kwargs=} were also provided.\n"
-            new_msg += (
-                "If the item failed to initialize, a common reason can be forgetting"
-                " to call `configure()` on the `Component` or the pipeline it is in or"
-                " not calling `build()`/`build_item()` on the **returned** value of"
-                " `configure()`.\n"
-                "Reasons may also include not having fully specified the `config`"
-                " initially, it having not being configured fully from `configure()`"
-                " or from misspecfying parameters in the `space`."
+        _nodes = tuple(as_node(n) for n in nodes)
+        if not all_unique(_nodes, key=lambda node: node.name):
+            raise ValueError(
+                f"Can't handle nodes they do not all contain unique names, {nodes=}."
+                "\nAll nodes must have a unique name. Please provide a `name=` to them",
             )
-            raise ComponentBuildError(new_msg) from e
-
-
-@dataclass(init=False, frozen=True, eq=True)
-class Searchable(Node[None, Space]):  # type: ignore
-    """A [`Searchable`][amltk.pipeline.Searchable]
-    node of the pipeline which just represents a search space, no item attached.
-
-    While not usually applicable to pipelines you want to build, this component
-    is useful for creating a search space, especially if the real pipeline you
-    want to optimize can not be built directly. For example, if you are optimize
-    a script, you may wish to use a `Searchable` to represent the search space
-    of that script.
-
-    ```python exec="true" source="material-block" html="true"
-    from amltk.pipeline import Searchable
-
-    script_space = Searchable({"mode": ["orange", "blue", "red"], "n": (10, 100)})
-    from amltk._doc import doc_print; doc_print(print, script_space)  # markdown-exec: hide
-    ```
-
-    A `Searchable` explicitly does not allow for `item=` to be set, nor can it have
-    any children. A `Searchable` accepts an explicit
-    [`name=`][amltk.pipeline.node.Node.name],
-    [`config=`][amltk.pipeline.node.Node.config],
-    [`space=`][amltk.pipeline.node.Node.space],
-    [`fidelities=`][amltk.pipeline.node.Node.fidelities],
-    [`config_transform=`][amltk.pipeline.node.Node.config_transform] and
-    [`meta=`][amltk.pipeline.node.Node.meta].
-
-    See Also:
-        * [`Node`][amltk.pipeline.node.Node]
-    """  # noqa: E501
-
-    item: None = None
-    """A searchable has no item."""
 
-    nodes: tuple[()] = ()
-    """A component has no children."""
-
-    RICH_OPTIONS: ClassVar[RichOptions] = RichOptions(panel_color="light_steel_blue")
-
-    _NODES_INIT: ClassVar = None
-
-    def __init__(
-        self,
-        space: Space | None = None,
-        *,
-        name: str | None = None,
-        config: Config | None = None,
-        fidelities: Mapping[str, Any] | None = None,
-        config_transform: Callable[[Config, Any], Config] | None = None,
-        meta: Mapping[str, Any] | None = None,
-    ):
-        """See [`Node`][amltk.pipeline.node.Node] for details."""
         if name is None:
-            name = f"Searchable-{randuid(8)}"
+            name = f"Join-{randuid(8)}"
 
         super().__init__(
+            *_nodes,
             name=name,
+            item=item,
             config=config,
             space=space,
             fidelities=fidelities,
             config_transform=config_transform,
             meta=meta,
         )
 
+    @override
+    def __and__(self, other: Node | NodeLike) -> Join:
+        other_node = as_node(other)
+        if any(other_node.name == node.name for node in self.nodes):
+            raise ValueError(
+                f"Can't handle node with name '{other_node.name} as"
+                f" there is already a node called '{other_node.name}' in {self.name}",
+            )
 
-@dataclass(init=False, frozen=True, eq=True)
-class Fixed(Node[Item, None]):  # type: ignore
-    """A [`Fixed`][amltk.pipeline.Fixed] part of the pipeline that
-    represents something that can not be configured and used directly as is.
-
-    It consists of an [`.item`][amltk.pipeline.node.Node.item] that is fixed,
-    non-configurable and non-searchable. It also has no children.
-
-    This is useful for representing parts of the pipeline that are fixed, for example
-    if you have a pipeline that is a `Sequential` of nodes, but you want to
-    fix the first component to be a `PCA` with `n_components=3`, you can use a `Fixed`
-    to represent that.
-
-    ```python exec="true" source="material-block" html="true"
-    from amltk.pipeline import Component, Fixed, Sequential
-    from sklearn.ensemble import RandomForestClassifier
-    from sklearn.decomposition import PCA
-
-    rf = Component(RandomForestClassifier, space={"n_estimators": (10, 100)})
-    pca = Fixed(PCA(n_components=3))
-
-    pipeline = Sequential(pca, rf, name="my_pipeline")
-    from amltk._doc import doc_print; doc_print(print, pipeline)  # markdown-exec: hide
-    ```
-
-    Whenever some other node sees an instance of something, i.e. something that can't be
-    called, this will automatically be converted into a `Fixed`.
-
-    ```python exec="true" source="material-block" html="true"
-    from amltk.pipeline import Sequential
-    from sklearn.ensemble import RandomForestClassifier
-    from sklearn.decomposition import PCA
-
-    pipeline = Sequential(
-        PCA(n_components=3),
-        RandomForestClassifier(n_estimators=50),
-        name="my_pipeline",
-    )
-    from amltk._doc import doc_print; doc_print(print, pipeline)  # markdown-exec: hide
-    ```
-
-    The default `.name` of a component is the class name of the item that it will
-    use. You can explicitly set the `name=` if you want to when constructing the
-    component.
-
-    A `Fixed` accepts only an explicit [`name=`][amltk.pipeline.node.Node.name],
-    [`item=`][amltk.pipeline.node.Node.item],
-    [`meta=`][amltk.pipeline.node.Node.meta].
-
-    See Also:
-        * [`Node`][amltk.pipeline.node.Node]
-    """
-
-    item: Item = field()
-    """The fixed item that this node represents."""
-
-    space: None = None
-    """A frozen node has no search space."""
-
-    fidelities: None = None
-    """A frozen node has no search space."""
-
-    config: None = None
-    """A frozen node has no config."""
-
-    config_transform: None = None
-    """A frozen node has no config so no transform."""
-
-    nodes: tuple[()] = ()
-    """A component has no children."""
-
-    RICH_OPTIONS: ClassVar[RichOptions] = RichOptions(panel_color="#56351E")
-
-    _NODES_INIT: ClassVar = None
-
-    def __init__(
-        self,
-        item: Item,
-        *,
-        name: str | None = None,
-        config: None = None,
-        space: None = None,
-        fidelities: None = None,
-        config_transform: None = None,
-        meta: Mapping[str, Any] | None = None,
-    ):
-        """See [`Node`][amltk.pipeline.node.Node] for details."""
-        super().__init__(
-            name=name if name is not None else entity_name(item),
-            item=item,
-            config=config,
-            space=space,
-            fidelities=fidelities,
-            config_transform=config_transform,
-            meta=meta,
-        )
+        nodes = (*tuple(as_node(n) for n in self.nodes), other_node)
+        return self.mutate(name=self.name, nodes=nodes)
```

### Comparing `amltk-1.8.0/src/amltk/pipeline/node.py` & `amltk-1.9.0/src/amltk/pipeline/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,53 +156,65 @@
     """The configuration for this node"""
 
     space: Space | None = field(hash=False)
     """The search space for this node"""
 
     fidelities: Mapping[str, Any] | None = field(hash=False)
     """The fidelities for this node"""
+
     config_transform: Callable[[Config, Any], Config] | None = field(hash=False)
     """A function that transforms the configuration of this node"""
 
     meta: Mapping[str, Any] | None = field(hash=False)
     """Any meta information about this node"""
 
     _NODES_INIT: ClassVar[Literal["args", "kwargs"] | None] = "args"
     """Whether __init__ takes nodes as positional args, kwargs or does not accept it."""
 
     RICH_OPTIONS: ClassVar[RichOptions] = RichOptions(
         panel_color="default",
         node_orientation="horizontal",
     )
-    """Options for rich printing"""
+    """How to display this node in rich."""
 
     def __init__(
         self,
         *nodes: Node,
         name: str,
         item: Item | Callable[[Item], Item] | None = None,
         config: Config | None = None,
         space: Space | None = None,
         fidelities: Mapping[str, Any] | None = None,
         config_transform: Callable[[Config, Any], Config] | None = None,
         meta: Mapping[str, Any] | None = None,
     ):
-        """Initialize a choice."""
+        """Initialize a choice.
+
+        Args:
+            nodes: The nodes that this node leads to
+            name: The name of the node
+            item: The item attached to this node
+            config: The configuration for this node
+            space: The search space for this node
+            fidelities: The fidelities for this node
+            config_transform: A function that transforms the configuration of this node
+            meta: Any meta information about this node
+        """
         super().__init__()
         object.__setattr__(self, "name", name)
         object.__setattr__(self, "item", item)
         object.__setattr__(self, "config", config)
         object.__setattr__(self, "space", space)
         object.__setattr__(self, "fidelities", fidelities)
         object.__setattr__(self, "config_transform", config_transform)
         object.__setattr__(self, "meta", meta)
         object.__setattr__(self, "nodes", nodes)
 
     def __getitem__(self, key: str) -> Node:
-        """Get the node with the given name."""
+        """Get the first from [`.nodes`][amltk.pipeline.node.Node.nodes] with `key`."""
         found = first_true(
             self.nodes,
             None,
             lambda node: node.name == key,
         )
         if found is None:
             raise KeyError(
```

### Comparing `amltk-1.8.0/src/amltk/pipeline/ops.py` & `amltk-1.9.0/src/amltk/pipeline/ops.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/pipeline/parsers/configspace.py` & `amltk-1.9.0/src/amltk/pipeline/parsers/configspace.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/pipeline/parsers/optuna.py` & `amltk-1.9.0/src/amltk/pipeline/parsers/optuna.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/pipeline/xgboost.py` & `amltk-1.9.0/src/amltk/pipeline/xgboost.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/profiling/memory.py` & `amltk-1.9.0/src/amltk/profiling/memory.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/profiling/profiler.py` & `amltk-1.9.0/src/amltk/profiling/profiler.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/profiling/timing.py` & `amltk-1.9.0/src/amltk/profiling/timing.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/randomness.py` & `amltk-1.9.0/src/amltk/randomness.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/scheduling/events.py` & `amltk-1.9.0/src/amltk/scheduling/events.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/scheduling/executors/dask_jobqueue.py` & `amltk-1.9.0/src/amltk/scheduling/executors/dask_jobqueue.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/scheduling/executors/sequential_executor.py` & `amltk-1.9.0/src/amltk/scheduling/executors/sequential_executor.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/scheduling/plugins/comm.py` & `amltk-1.9.0/src/amltk/scheduling/plugins/comm.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/scheduling/plugins/emissions_tracker_plugin.py` & `amltk-1.9.0/src/amltk/scheduling/plugins/emissions_tracker_plugin.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/scheduling/plugins/limiter.py` & `amltk-1.9.0/src/amltk/scheduling/plugins/limiter.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/scheduling/plugins/plugin.py` & `amltk-1.9.0/src/amltk/scheduling/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/scheduling/plugins/pynisher.py` & `amltk-1.9.0/src/amltk/scheduling/plugins/pynisher.py`

 * *Files 3% similar despite different names*

```diff
@@ -374,14 +374,27 @@
                     task_two.submit(..., trial=trial)
 
                     # Will not auto-detect
                     task_one.submit(42, trial)
                     ```
         """
         super().__init__()
+
+        for limit, name in [
+            (memory_limit, "memory"),
+            (cputime_limit, "cpu_time"),
+            (walltime_limit, "wall_time"),
+        ]:
+            if limit is not None and not self.supports(name):  # type: ignore
+                raise RuntimeError(
+                    f"Your platform does not support {name} limits."
+                    " Please see pynisher documentation for more:"
+                    "\nhttps://github.com/automl/pynisher#features",
+                )
+
         self.memory_limit = memory_limit
         self.cputime_limit = cputime_limit
         self.walltime_limit = walltime_limit
         self.context = context
         self.disable_trial_handling = disable_trial_handling
 
         self.task: Task
```

### Comparing `amltk-1.8.0/src/amltk/scheduling/plugins/threadpoolctl.py` & `amltk-1.9.0/src/amltk/scheduling/plugins/threadpoolctl.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/scheduling/plugins/wandb.py` & `amltk-1.9.0/src/amltk/scheduling/plugins/wandb.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/scheduling/plugins/warning_filter.py` & `amltk-1.9.0/src/amltk/scheduling/plugins/warning_filter.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/scheduling/queue_monitor.py` & `amltk-1.9.0/src/amltk/scheduling/queue_monitor.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/scheduling/scheduler.py` & `amltk-1.9.0/src/amltk/scheduling/scheduler.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/scheduling/task.py` & `amltk-1.9.0/src/amltk/scheduling/task.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/scheduling/termination_strategies.py` & `amltk-1.9.0/src/amltk/scheduling/termination_strategies.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/sklearn/data.py` & `amltk-1.9.0/src/amltk/sklearn/data.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/sklearn/estimators.py` & `amltk-1.9.0/src/amltk/sklearn/estimators.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/sklearn/voting.py` & `amltk-1.9.0/src/amltk/sklearn/voting.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/store/__init__.py` & `amltk-1.9.0/src/amltk/store/__init__.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/store/bucket.py` & `amltk-1.9.0/src/amltk/store/bucket.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/store/drop.py` & `amltk-1.9.0/src/amltk/store/drop.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/store/loader.py` & `amltk-1.9.0/src/amltk/store/loader.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/store/paths/path_bucket.py` & `amltk-1.9.0/src/amltk/store/paths/path_bucket.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/store/paths/path_loaders.py` & `amltk-1.9.0/src/amltk/store/paths/path_loaders.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/store/stored_value.py` & `amltk-1.9.0/src/amltk/store/stored_value.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk/types.py` & `amltk-1.9.0/src/amltk/types.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk.egg-info/PKG-INFO` & `amltk-1.9.0/src/amltk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amltk
-Version: 1.8.0
+Version: 1.9.0
 Summary: AutoML Toolkit: a toolkit for building automl system
 Author-email: Eddie Bergman <eddiebergmanhs@gmail.com>
 License: Copyright 2023 AutoML-Freiburg-Hannover-Tübingen
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -63,14 +63,15 @@
 Requires-Dist: mkdocstrings[python]; extra == "doc"
 Requires-Dist: markdown-exec[ansi]; extra == "doc"
 Requires-Dist: matplotlib; extra == "doc"
 Requires-Dist: rich; extra == "doc"
 Requires-Dist: mike; extra == "doc"
 Requires-Dist: pillow; extra == "doc"
 Requires-Dist: cairosvg; extra == "doc"
+Requires-Dist: black; extra == "doc"
 Provides-Extra: sklearn
 Requires-Dist: scikit-learn; extra == "sklearn"
 Requires-Dist: threadpoolctl; extra == "sklearn"
 Provides-Extra: smac
 Requires-Dist: smac>=2.0; extra == "smac"
 Requires-Dist: amltk[configspace]; extra == "smac"
 Provides-Extra: optuna
```

### Comparing `amltk-1.8.0/src/amltk.egg-info/SOURCES.txt` & `amltk-1.9.0/src/amltk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/src/amltk.egg-info/requires.txt` & `amltk-1.9.0/src/amltk.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 mkdocstrings[python]
 markdown-exec[ansi]
 matplotlib
 rich
 mike
 pillow
 cairosvg
+black
 
 [examples]
 openml
 amltk[dask,loky,optuna,path_loaders,pynisher,rich,sklearn,smac,wandb,xgboost]
 
 [loky]
 loky
```

### Comparing `amltk-1.8.0/tests/test_distances.py` & `amltk-1.9.0/tests/test_distances.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/tests/test_examples.py` & `amltk-1.9.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `amltk-1.8.0/tests/test_randomness.py` & `amltk-1.9.0/tests/test_randomness.py`

 * *Files identical despite different names*

