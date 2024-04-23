# Comparing `tmp/google-vizier-dev-0.1.16.dev20240422191908.tar.gz` & `tmp/google-vizier-dev-0.1.16.dev20240423231204.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-vizier-dev-0.1.16.dev20240422191908.tar", last modified: Mon Apr 22 19:19:08 2024, max compression
+gzip compressed data, was "google-vizier-dev-0.1.16.dev20240423231204.tar", last modified: Tue Apr 23 23:12:04 2024, max compression
```

## Comparing `google-vizier-dev-0.1.16.dev20240422191908.tar` & `google-vizier-dev-0.1.16.dev20240423231204.tar`

### file list

```diff
@@ -1,398 +1,398 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.988331 google-vizier-dev-0.1.16.dev20240422191908/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-22 19:19:08.988331 google-vizier-dev-0.1.16.dev20240422191908/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.928331 google-vizier-dev-0.1.16.dev20240422191908/google_vizier_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-22 19:19:08.000000 google-vizier-dev-0.1.16.dev20240422191908/google_vizier_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-04-22 19:19:08.000000 google-vizier-dev-0.1.16.dev20240422191908/google_vizier_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:19:08.000000 google-vizier-dev-0.1.16.dev20240422191908/google_vizier_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:19:08.000000 google-vizier-dev-0.1.16.dev20240422191908/google_vizier_dev.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-22 19:19:08.000000 google-vizier-dev-0.1.16.dev20240422191908/google_vizier_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-22 19:19:08.000000 google-vizier-dev-0.1.16.dev20240422191908/google_vizier_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 19:19:08.988331 google-vizier-dev-0.1.16.dev20240422191908/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.928331 google-vizier-dev-0.1.16.dev20240422191908/vizier/
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.928331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.928331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.928331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/classification/
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/classification/classifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/classification/classifiers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.932330 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/core/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/core/abstractions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.936331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19486 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/bocs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/bocs_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/cmaes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/cmaes_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.936331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/eagle_strategy/
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/eagle_strategy/eagle_designer_convergence_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/eagle_strategy/eagle_simplekd_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    19205 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13117 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    20990 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18184 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/eagle_strategy/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/eagle_strategy/serialization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/eagle_strategy/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/emukit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/emukit_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.940331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp/
--rw-r--r--   0 runner    (1001) docker     (127)    19338 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp/acquisitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11880 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp/acquisitions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12568 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp/gp_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    13632 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp/gp_models_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    28233 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp/output_warpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16954 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp/output_warpers_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp/transfer_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp/transfer_learning_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp/yjt.py
--rw-r--r--   0 runner    (1001) docker     (127)    22547 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp_bandit.py
--rw-r--r--   0 runner    (1001) docker     (127)    19662 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp_bandit_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    31401 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp_ucb_pe.py
--rw-r--r--   0 runner    (1001) docker     (127)    11095 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp_ucb_pe_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/grid_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/harmonica.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/harmonica_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.940331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/meta_learning/
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/meta_learning/eagle_meta_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/meta_learning/eagle_meta_learning_convergence_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10667 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/meta_learning/meta_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/meta_learning/meta_learning_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/meta_learning/meta_learning_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/meta_learning/meta_learning_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/quasi_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/quasi_random_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/random_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/scalarization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/scalarization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/scalarizing_designer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/scalarizing_designer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/scheduled_designer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/scheduled_designer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/scheduled_gp_bandit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/scheduled_gp_ucb_pe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/unsafe_as_infeasible_designer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/unsafe_as_infeasible_designer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.940331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/ensemble/ensemble_design.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/ensemble/ensemble_design_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/ensemble/ensemble_designer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/ensemble/ensemble_designer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.940331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/evolution/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/evolution/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/evolution/nsga2_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/evolution/numpy_populations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/evolution/numpy_populations_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/evolution/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.944331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/designer_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/designer_optimizer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/eagle_optimizer_convergence_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    40789 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/eagle_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23588 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/eagle_strategy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/lbfgsb_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/lbfgsb_optimizer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/random_vectorized_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/random_vectorized_optimizer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22804 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/vectorized_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13602 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/vectorized_base_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.948330 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/policies/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13561 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/policies/designer_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/policies/designer_policy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/policies/random_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/policies/random_policy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/policies/trial_caches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/policies/trial_caches_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.948330 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/random/
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/random/random_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/random/random_sample_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.948330 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/regression/
--rw-r--r--   0 runner    (1001) docker     (127)    18505 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/regression/trial_regression_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12026 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/regression/trial_regression_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.948330 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10622 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/testing/comparator_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/testing/comparator_runner_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/testing/failing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/testing/failing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/testing/optimizer_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/testing/simplekd_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/testing/test_runners.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.924331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.952331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/analyzers/
--rw-r--r--   0 runner    (1001) docker     (127)    39015 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/analyzers/convergence_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    34712 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/analyzers/convergence_curve_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/analyzers/exploration_score_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/analyzers/exploration_score_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8836 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/analyzers/plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/analyzers/plot_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/analyzers/simple_regret_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/analyzers/simple_regret_score_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/analyzers/state_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/analyzers/state_analyzer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.956331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/
--rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/atari100k_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/atari100k_experimenter_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.956331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/combo/
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/combo/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    16944 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/combo_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/combo_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/discretizing_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/discretizing_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/experimenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8472 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/experimenter_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/experimenter_factory_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.956331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/hpob/
--rw-r--r--   0 runner    (1001) docker     (127)    11646 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/hpob/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    25640 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/hpob_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/hpob_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/multiobjective_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/multiobjective_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/nasbench101_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/nasbench101_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/nasbench201_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/nasbench201_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/noisy_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/noisy_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/normalizing_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/normalizing_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/numpy_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/numpy_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/shifting_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/shifting_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/sign_flip_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/sign_flip_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/sparse_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/sparse_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/surrogate_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/surrogate_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/switch_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/switch_experimenter_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.960331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/synthetic/
--rw-r--r--   0 runner    (1001) docker     (127)    17239 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/synthetic/bbob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/synthetic/bbob_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/synthetic/branin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/synthetic/branin_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/synthetic/hartmann.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/synthetic/hartmann_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/synthetic/simplekd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/synthetic/simplekd_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.960331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/runners/
--rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/runners/benchmark_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/runners/benchmark_runner_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/runners/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/runners/benchmark_state_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.960331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/testing/
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/testing/experimenter_testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.964331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/gp_bandit_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.964331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/continuous_only_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/gaussian_process_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/gaussian_process_model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/hebo_gp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/hebo_gp_model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/mask_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/mask_features_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13214 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/multitask_tuned_gp_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/multitask_tuned_gp_models_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14954 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/tuned_gp_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    10578 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/tuned_gp_models_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.964331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/optimizers/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/optimizers/core_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10124 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/optimizers/jaxopt_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/optimizers/jaxopt_wrappers_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/optimizers/optax_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/optimizers/optax_wrappers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.964331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/optimizers/testing/
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/optimizers/testing/sinusoidal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/predictive_fns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/predictive_fns_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    37932 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/stochastic_process_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    23877 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/stochastic_process_model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/types_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/xla_pareto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/xla_pareto_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.968330 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)    19957 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    22016 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)    12830 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/converters_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13005 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/e2e_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10559 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/oss_vizier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/oss_vizier_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/performance_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/pythia.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/pythia_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    21776 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/vizier_test_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.968330 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pythia/
--rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pythia/local_policy_supporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pythia/local_policy_supporters_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8983 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pythia/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pythia/policy_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pythia/policy_supporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pythia/pythia_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.924331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.972331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/multimetric/
--rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/multimetric/hypervolume.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/multimetric/hypervolume_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9931 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/multimetric/pareto_optimal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/multimetric/pareto_optimal_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/multimetric/safety.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/multimetric/safety_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.972331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/oss/
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/oss/automated_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/oss/automated_stopping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/oss/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/oss/metadata_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/oss/metadata_util_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    33067 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/oss/proto_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/oss/proto_converters_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    16564 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/oss/study_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    36562 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/oss/study_config_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.972331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/pythia/
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/pythia/study.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.976331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/
--rw-r--r--   0 runner    (1001) docker     (127)    13424 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/base_study_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/base_study_config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24485 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    15254 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/common_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/context_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    49914 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/parameter_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    25165 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/parameter_config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/parameter_iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/parameter_iterators_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/study.py
--rw-r--r--   0 runner    (1001) docker     (127)    23543 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/trial.py
--rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/trial_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.976331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/raytune/
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/raytune/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/raytune/converters_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/raytune/run_tune.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/raytune/run_tune_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7789 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/raytune/vizier_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/raytune/vizier_search_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.980331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/
--rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/clients_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/custom_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    12366 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/datastore_test_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/grpc_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/performance_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/policy_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/pythia_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/pythia_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    15795 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/ram_datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/ram_datastore_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/resources_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/service_policy_supporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/service_policy_supporter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    20706 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/sql_datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/sql_datastore_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/stubs_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/stubs_util_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.980331 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/testing/
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/testing/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    17489 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/vizier_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12372 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/vizier_client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/vizier_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    36429 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/vizier_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    17256 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/vizier_service_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.980331 google-vizier-dev-0.1.16.dev20240422191908/vizier/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.980331 google-vizier-dev-0.1.16.dev20240422191908/vizier/algorithms/designers/
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/algorithms/designers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/algorithms/evolution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.980331 google-vizier-dev-0.1.16.dev20240422191908/vizier/algorithms/policies/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/algorithms/policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.980331 google-vizier-dev-0.1.16.dev20240422191908/vizier/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/benchmarks/analyzers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.980331 google-vizier-dev-0.1.16.dev20240422191908/vizier/benchmarks/experimenters/
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/benchmarks/experimenters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.980331 google-vizier-dev-0.1.16.dev20240422191908/vizier/benchmarks/experimenters/hpo/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/benchmarks/experimenters/hpo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.980331 google-vizier-dev-0.1.16.dev20240422191908/vizier/benchmarks/experimenters/nas/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/benchmarks/experimenters/nas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.984331 google-vizier-dev-0.1.16.dev20240422191908/vizier/benchmarks/experimenters/rl/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/benchmarks/experimenters/rl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.984331 google-vizier-dev-0.1.16.dev20240422191908/vizier/client/
--rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/client/client_abc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15891 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/client/client_abc_testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.984331 google-vizier-dev-0.1.16.dev20240422191908/vizier/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/interfaces/serializable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.984331 google-vizier-dev-0.1.16.dev20240422191908/vizier/jax/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/jax/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/jax/optimizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.984331 google-vizier-dev-0.1.16.dev20240422191908/vizier/pyglove/
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/pyglove/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/pythia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.984331 google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.984331 google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45206 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    46300 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/core_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/embedder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6145 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/embedder_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/feature_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/feature_mapper_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/input_warping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/input_warping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    15163 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/jnp_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/jnp_converters_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/padding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/padding_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    20179 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/spatio_temporal.py
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/spatio_temporal_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.984331 google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/multimetric/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/multimetric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/multimetric/xla_pareto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.984331 google-vizier-dev-0.1.16.dev20240422191908/vizier/raytune/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/raytune/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.984331 google-vizier-dev-0.1.16.dev20240422191908/vizier/service/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.984331 google-vizier-dev-0.1.16.dev20240422191908/vizier/service/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/service/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.984331 google-vizier-dev-0.1.16.dev20240422191908/vizier/service/protos/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/service/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.988331 google-vizier-dev-0.1.16.dev20240422191908/vizier/service/pyvizier/
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/service/pyvizier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.988331 google-vizier-dev-0.1.16.dev20240422191908/vizier/service/servers/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/service/servers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.988331 google-vizier-dev-0.1.16.dev20240422191908/vizier/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/testing/numpy_assertions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/testing/test_studies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:08.988331 google-vizier-dev-0.1.16.dev20240422191908/vizier/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/utils/attrs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/utils/attrs_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/utils/json_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/utils/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-22 19:18:54.000000 google-vizier-dev-0.1.16.dev20240422191908/vizier/utils/profiler_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.409995 google-vizier-dev-0.1.16.dev20240423231204/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-23 23:12:04.409995 google-vizier-dev-0.1.16.dev20240423231204/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.357995 google-vizier-dev-0.1.16.dev20240423231204/google_vizier_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-23 23:12:04.000000 google-vizier-dev-0.1.16.dev20240423231204/google_vizier_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-04-23 23:12:04.000000 google-vizier-dev-0.1.16.dev20240423231204/google_vizier_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 23:12:04.000000 google-vizier-dev-0.1.16.dev20240423231204/google_vizier_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 23:12:04.000000 google-vizier-dev-0.1.16.dev20240423231204/google_vizier_dev.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-23 23:12:04.000000 google-vizier-dev-0.1.16.dev20240423231204/google_vizier_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 23:12:04.000000 google-vizier-dev-0.1.16.dev20240423231204/google_vizier_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 23:12:04.409995 google-vizier-dev-0.1.16.dev20240423231204/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.357995 google-vizier-dev-0.1.16.dev20240423231204/vizier/
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.357995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.357995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.357995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/classification/classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/classification/classifiers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.361995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/core/abstractions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.365996 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19486 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/bocs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/bocs_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/cmaes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/cmaes_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.365996 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/eagle_strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/eagle_strategy/eagle_designer_convergence_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/eagle_strategy/eagle_simplekd_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19205 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13117 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20990 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18184 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/eagle_strategy/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/eagle_strategy/serialization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/eagle_strategy/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/emukit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/emukit_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.365996 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp/
+-rw-r--r--   0 runner    (1001) docker     (127)    19338 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp/acquisitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11880 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp/acquisitions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12568 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp/gp_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13632 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp/gp_models_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28233 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp/output_warpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16954 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp/output_warpers_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp/transfer_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp/transfer_learning_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp/yjt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22547 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp_bandit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19662 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp_bandit_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31401 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp_ucb_pe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11095 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp_ucb_pe_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/grid_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/harmonica.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/harmonica_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.369995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/meta_learning/
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/meta_learning/eagle_meta_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/meta_learning/eagle_meta_learning_convergence_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10667 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/meta_learning/meta_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/meta_learning/meta_learning_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/meta_learning/meta_learning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/meta_learning/meta_learning_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/quasi_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/quasi_random_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/scalarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/scalarization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/scalarizing_designer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/scalarizing_designer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/scheduled_designer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/scheduled_designer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/scheduled_gp_bandit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/scheduled_gp_ucb_pe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/unsafe_as_infeasible_designer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/unsafe_as_infeasible_designer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.369995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/ensemble/ensemble_design.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/ensemble/ensemble_design_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/ensemble/ensemble_designer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/ensemble/ensemble_designer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.369995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/evolution/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/evolution/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/evolution/nsga2_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/evolution/numpy_populations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/evolution/numpy_populations_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/evolution/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.373995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/designer_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/designer_optimizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/eagle_optimizer_convergence_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40789 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/eagle_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23588 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/eagle_strategy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/lbfgsb_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/lbfgsb_optimizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/random_vectorized_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/random_vectorized_optimizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22804 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/vectorized_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13602 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/vectorized_base_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.373995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13561 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/policies/designer_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/policies/designer_policy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/policies/random_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/policies/random_policy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/policies/trial_caches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/policies/trial_caches_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.373995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/random/
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/random/random_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/random/random_sample_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.373995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)    18505 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/regression/trial_regression_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12026 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/regression/trial_regression_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.373995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10622 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/testing/comparator_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/testing/comparator_runner_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/testing/failing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/testing/failing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/testing/optimizer_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/testing/simplekd_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/testing/test_runners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.353995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.377995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)    39015 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/analyzers/convergence_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34712 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/analyzers/convergence_curve_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/analyzers/exploration_score_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/analyzers/exploration_score_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8836 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/analyzers/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/analyzers/plot_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/analyzers/simple_regret_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/analyzers/simple_regret_score_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/analyzers/state_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/analyzers/state_analyzer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.381995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/
+-rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/atari100k_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/atari100k_experimenter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.381995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/combo/
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/combo/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16944 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/combo_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/combo_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/discretizing_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/discretizing_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8472 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/experimenter_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/experimenter_factory_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.381995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/hpob/
+-rw-r--r--   0 runner    (1001) docker     (127)    11646 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/hpob/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25640 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/hpob_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/hpob_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/multiobjective_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/multiobjective_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/nasbench101_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/nasbench101_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/nasbench201_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/nasbench201_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/noisy_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/noisy_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/normalizing_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/normalizing_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/numpy_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/numpy_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/shifting_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/shifting_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/sign_flip_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/sign_flip_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/sparse_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/sparse_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/surrogate_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/surrogate_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/switch_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/switch_experimenter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.385995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/synthetic/
+-rw-r--r--   0 runner    (1001) docker     (127)    17239 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/synthetic/bbob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/synthetic/bbob_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/synthetic/branin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/synthetic/branin_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/synthetic/hartmann.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/synthetic/hartmann_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/synthetic/simplekd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/synthetic/simplekd_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.385995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/runners/benchmark_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/runners/benchmark_runner_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/runners/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/runners/benchmark_state_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.385995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/testing/experimenter_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.385995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/gp_bandit_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.389995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/continuous_only_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/gaussian_process_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/gaussian_process_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/hebo_gp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/hebo_gp_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/mask_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/mask_features_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13214 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/multitask_tuned_gp_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/multitask_tuned_gp_models_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14954 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/tuned_gp_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10578 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/tuned_gp_models_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.389995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/optimizers/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/optimizers/core_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10124 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/optimizers/jaxopt_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/optimizers/jaxopt_wrappers_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/optimizers/optax_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/optimizers/optax_wrappers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.389995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/optimizers/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/optimizers/testing/sinusoidal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/predictive_fns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/predictive_fns_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37932 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/stochastic_process_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23877 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/stochastic_process_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/types_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/xla_pareto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/xla_pareto_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.389995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19957 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22016 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12830 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/converters_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13005 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/e2e_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10559 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/oss_vizier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/oss_vizier_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/performance_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/pythia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/pythia_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21776 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/vizier_test_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.393995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pythia/
+-rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pythia/local_policy_supporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pythia/local_policy_supporters_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8983 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pythia/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pythia/policy_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pythia/policy_supporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pythia/pythia_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.353995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.393995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/multimetric/
+-rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/multimetric/hypervolume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/multimetric/hypervolume_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9931 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/multimetric/pareto_optimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/multimetric/pareto_optimal_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/multimetric/safety.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/multimetric/safety_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.393995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/oss/
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/oss/automated_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/oss/automated_stopping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/oss/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/oss/metadata_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/oss/metadata_util_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33067 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/oss/proto_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/oss/proto_converters_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16564 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/oss/study_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36562 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/oss/study_config_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.393995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/pythia/
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/pythia/study.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.397995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)    13424 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/base_study_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/base_study_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24485 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15254 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/common_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/context_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49914 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/parameter_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25165 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/parameter_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/parameter_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/parameter_iterators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/study.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23543 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/trial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/trial_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.397995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/raytune/
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/raytune/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/raytune/converters_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/raytune/run_tune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/raytune/run_tune_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7789 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/raytune/vizier_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/raytune/vizier_search_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.401995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/
+-rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/clients_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/custom_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12366 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/datastore_test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/grpc_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/performance_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/policy_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/pythia_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/pythia_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15795 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/ram_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/ram_datastore_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/resources_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/service_policy_supporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/service_policy_supporter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20706 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/sql_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/sql_datastore_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/stubs_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/stubs_util_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.401995 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/testing/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17489 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/vizier_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12372 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/vizier_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/vizier_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36429 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/vizier_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17256 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/vizier_service_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.401995 google-vizier-dev-0.1.16.dev20240423231204/vizier/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.401995 google-vizier-dev-0.1.16.dev20240423231204/vizier/algorithms/designers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/algorithms/designers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/algorithms/evolution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.401995 google-vizier-dev-0.1.16.dev20240423231204/vizier/algorithms/policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/algorithms/policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.401995 google-vizier-dev-0.1.16.dev20240423231204/vizier/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/benchmarks/analyzers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.401995 google-vizier-dev-0.1.16.dev20240423231204/vizier/benchmarks/experimenters/
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/benchmarks/experimenters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.401995 google-vizier-dev-0.1.16.dev20240423231204/vizier/benchmarks/experimenters/hpo/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/benchmarks/experimenters/hpo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.405995 google-vizier-dev-0.1.16.dev20240423231204/vizier/benchmarks/experimenters/nas/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/benchmarks/experimenters/nas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.405995 google-vizier-dev-0.1.16.dev20240423231204/vizier/benchmarks/experimenters/rl/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/benchmarks/experimenters/rl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.405995 google-vizier-dev-0.1.16.dev20240423231204/vizier/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/client/client_abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15891 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/client/client_abc_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.405995 google-vizier-dev-0.1.16.dev20240423231204/vizier/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/interfaces/serializable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.405995 google-vizier-dev-0.1.16.dev20240423231204/vizier/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/jax/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/jax/optimizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.405995 google-vizier-dev-0.1.16.dev20240423231204/vizier/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/pyglove/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/pythia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.405995 google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.405995 google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45206 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46300 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/core_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/embedder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6145 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/embedder_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/feature_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/feature_mapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/input_warping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/input_warping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15163 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/jnp_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/jnp_converters_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/padding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/padding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20179 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/spatio_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/spatio_temporal_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.409995 google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/multimetric/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/multimetric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/multimetric/xla_pareto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.409995 google-vizier-dev-0.1.16.dev20240423231204/vizier/raytune/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/raytune/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.409995 google-vizier-dev-0.1.16.dev20240423231204/vizier/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.409995 google-vizier-dev-0.1.16.dev20240423231204/vizier/service/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/service/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.409995 google-vizier-dev-0.1.16.dev20240423231204/vizier/service/protos/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/service/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.409995 google-vizier-dev-0.1.16.dev20240423231204/vizier/service/pyvizier/
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/service/pyvizier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.409995 google-vizier-dev-0.1.16.dev20240423231204/vizier/service/servers/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/service/servers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.409995 google-vizier-dev-0.1.16.dev20240423231204/vizier/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/testing/numpy_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/testing/test_studies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:12:04.409995 google-vizier-dev-0.1.16.dev20240423231204/vizier/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/utils/attrs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/utils/attrs_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/utils/json_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/utils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-23 23:11:37.000000 google-vizier-dev-0.1.16.dev20240423231204/vizier/utils/profiler_test.py
```

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/LICENSE` & `google-vizier-dev-0.1.16.dev20240423231204/LICENSE`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/PKG-INFO` & `google-vizier-dev-0.1.16.dev20240423231204/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-vizier-dev
-Version: 0.1.16.dev20240422191908
+Version: 0.1.16.dev20240423231204
 Summary: Open Source Vizier: Distributed service framework for blackbox optimization and research.
 Home-page: https://github.com/google/vizier
 Author: Vizier Team
 Author-email: oss-vizier-dev@google.com
 License: Apache License 2.0
 Keywords: ai machine learning hyperparameter blackbox optimization framework
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/README.md` & `google-vizier-dev-0.1.16.dev20240423231204/README.md`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/google_vizier_dev.egg-info/PKG-INFO` & `google-vizier-dev-0.1.16.dev20240423231204/google_vizier_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-vizier-dev
-Version: 0.1.16.dev20240422191908
+Version: 0.1.16.dev20240423231204
 Summary: Open Source Vizier: Distributed service framework for blackbox optimization and research.
 Home-page: https://github.com/google/vizier
 Author: Vizier Team
 Author-email: oss-vizier-dev@google.com
 License: Apache License 2.0
 Keywords: ai machine learning hyperparameter blackbox optimization framework
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/google_vizier_dev.egg-info/SOURCES.txt` & `google-vizier-dev-0.1.16.dev20240423231204/google_vizier_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/google_vizier_dev.egg-info/requires.txt` & `google-vizier-dev-0.1.16.dev20240423231204/google_vizier_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/setup.py` & `google-vizier-dev-0.1.16.dev20240423231204/setup.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/classification/classifiers.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/classification/classifiers.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,12 +82,14 @@
 
   # TODO: separate the training and evaluation for extra speed up.
   # Currently, the classifiers we use are reasonably fast.
   def __call__(self) -> np.ndarray:
     self._check_features_and_labels_shapes()
     self._check_labels_values()
     self._check_eval_metric()
+    if self.classifier is None:
+      raise RuntimeError('Classifier is None.')
     self.classifier.fit(np.asarray(self.features), np.asarray(self.labels))
     if self.eval_metric == 'probability':
       return self.classifier.predict_proba(np.asarray(self.features_test))[:, 1]
     else:
       return self.classifier.decision_function(np.asarray(self.features_test))  # pytype:disable=attribute-error
```

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/classification/classifiers_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/classification/classifiers_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/core/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/core/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/core/abstractions.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/core/abstractions.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/bocs.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/bocs.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/bocs_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/bocs_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/cmaes.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/cmaes.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/cmaes_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/cmaes_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/eagle_strategy/eagle_designer_convergence_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/eagle_strategy/eagle_designer_convergence_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/eagle_strategy/eagle_simplekd_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/eagle_strategy/eagle_simplekd_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/eagle_strategy/serialization.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/eagle_strategy/serialization.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/eagle_strategy/serialization_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/eagle_strategy/serialization_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/eagle_strategy/testing.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/eagle_strategy/testing.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/emukit.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/emukit.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/emukit_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/emukit_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp/acquisitions.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp/acquisitions.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp/acquisitions_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp/acquisitions_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp/gp_models.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp/gp_models.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp/gp_models_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp/gp_models_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp/output_warpers.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp/output_warpers.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp/output_warpers_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp/output_warpers_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp/transfer_learning.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp/transfer_learning.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp/transfer_learning_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp/transfer_learning_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp/yjt.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp/yjt.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp_bandit.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp_bandit.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp_bandit_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp_bandit_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp_ucb_pe.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp_ucb_pe.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/gp_ucb_pe_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/gp_ucb_pe_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/grid.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/grid.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/grid_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/grid_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/harmonica.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/harmonica.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/harmonica_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/harmonica_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/meta_learning/eagle_meta_learning.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/meta_learning/eagle_meta_learning.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/meta_learning/eagle_meta_learning_convergence_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/meta_learning/eagle_meta_learning_convergence_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/meta_learning/meta_learning.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/meta_learning/meta_learning.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/meta_learning/meta_learning_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/meta_learning/meta_learning_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/meta_learning/meta_learning_utils.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/meta_learning/meta_learning_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/meta_learning/meta_learning_utils_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/meta_learning/meta_learning_utils_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/quasi_random.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/quasi_random.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/quasi_random_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/quasi_random_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/random.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/random.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/random_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/random_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/scalarization.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/scalarization.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/scalarization_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/scalarization_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/scalarizing_designer.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/scalarizing_designer.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/scalarizing_designer_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/scalarizing_designer_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/scheduled_designer.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/scheduled_designer.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/scheduled_designer_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/scheduled_designer_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/scheduled_gp_bandit.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/scheduled_gp_bandit.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/scheduled_gp_ucb_pe.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/scheduled_gp_ucb_pe.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/unsafe_as_infeasible_designer.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/unsafe_as_infeasible_designer.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/designers/unsafe_as_infeasible_designer_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/designers/unsafe_as_infeasible_designer_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/ensemble/ensemble_design.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/ensemble/ensemble_design.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/ensemble/ensemble_design_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/ensemble/ensemble_design_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/ensemble/ensemble_designer.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/ensemble/ensemble_designer.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/ensemble/ensemble_designer_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/ensemble/ensemble_designer_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/evolution/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/evolution/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/evolution/nsga2.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/evolution/nsga2.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/evolution/nsga2_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/evolution/nsga2_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/evolution/numpy_populations.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/evolution/numpy_populations.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/evolution/numpy_populations_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/evolution/numpy_populations_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/evolution/templates.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/evolution/templates.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/base.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/designer_optimizer.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/designer_optimizer.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/designer_optimizer_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/designer_optimizer_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/eagle_optimizer_convergence_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/eagle_optimizer_convergence_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/eagle_strategy.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/eagle_strategy.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/eagle_strategy_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/eagle_strategy_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/lbfgsb_optimizer.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/lbfgsb_optimizer.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/lbfgsb_optimizer_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/lbfgsb_optimizer_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/random_vectorized_optimizer.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/random_vectorized_optimizer.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/random_vectorized_optimizer_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/random_vectorized_optimizer_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/vectorized_base.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/vectorized_base.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/optimizers/vectorized_base_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/optimizers/vectorized_base_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/policies/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/policies/designer_policy.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/policies/designer_policy.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/policies/designer_policy_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/policies/designer_policy_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/policies/random_policy.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/policies/random_policy.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/policies/random_policy_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/policies/random_policy_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/policies/trial_caches.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/policies/trial_caches.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/policies/trial_caches_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/policies/trial_caches_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/random/random_sample.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/random/random_sample.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/random/random_sample_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/random/random_sample_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/regression/trial_regression_utils.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/regression/trial_regression_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/regression/trial_regression_utils_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/regression/trial_regression_utils_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/testing/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/testing/comparator_runner.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/testing/comparator_runner.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/testing/comparator_runner_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/testing/comparator_runner_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/testing/failing.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/testing/failing.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/testing/failing_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/testing/failing_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/testing/optimizer_test_utils.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/testing/optimizer_test_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/testing/simplekd_runner.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/testing/simplekd_runner.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/algorithms/testing/test_runners.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/algorithms/testing/test_runners.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/analyzers/convergence_curve.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/analyzers/convergence_curve.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/analyzers/convergence_curve_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/analyzers/convergence_curve_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/analyzers/exploration_score_utils.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/analyzers/exploration_score_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/analyzers/exploration_score_utils_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/analyzers/exploration_score_utils_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/analyzers/plot_utils.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/analyzers/plot_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/analyzers/plot_utils_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/analyzers/plot_utils_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/analyzers/simple_regret_score.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/analyzers/simple_regret_score.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/analyzers/simple_regret_score_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/analyzers/simple_regret_score_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/analyzers/state_analyzer.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/analyzers/state_analyzer.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/analyzers/state_analyzer_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/analyzers/state_analyzer_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/atari100k_experimenter.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/atari100k_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/atari100k_experimenter_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/atari100k_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/combo/common.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/combo/common.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/combo_experimenter.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/combo_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/combo_experimenter_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/combo_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/discretizing_experimenter.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/discretizing_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/discretizing_experimenter_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/discretizing_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/experimenter.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/experimenter_factory.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/experimenter_factory.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/experimenter_factory_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/experimenter_factory_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/hpob/handler.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/hpob/handler.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/hpob_experimenter.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/hpob_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/hpob_experimenter_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/hpob_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/multiobjective_experimenter.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/multiobjective_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/multiobjective_experimenter_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/multiobjective_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/nasbench101_experimenter.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/nasbench101_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/nasbench101_experimenter_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/nasbench101_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/nasbench201_experimenter.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/nasbench201_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/nasbench201_experimenter_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/nasbench201_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/noisy_experimenter.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/noisy_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/noisy_experimenter_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/noisy_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/normalizing_experimenter.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/normalizing_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/normalizing_experimenter_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/normalizing_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/numpy_experimenter.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/numpy_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/numpy_experimenter_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/numpy_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/shifting_experimenter.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/shifting_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/shifting_experimenter_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/shifting_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/sign_flip_experimenter.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/sign_flip_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/sign_flip_experimenter_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/sign_flip_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/sparse_experimenter.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/sparse_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/sparse_experimenter_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/sparse_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/surrogate_experimenter.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/surrogate_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/surrogate_experimenter_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/surrogate_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/switch_experimenter.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/switch_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/switch_experimenter_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/switch_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/synthetic/bbob.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/synthetic/bbob.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/synthetic/bbob_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/synthetic/bbob_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/synthetic/branin.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/synthetic/branin.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/synthetic/branin_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/synthetic/branin_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/synthetic/hartmann.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/synthetic/hartmann.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/synthetic/hartmann_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/synthetic/hartmann_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/synthetic/simplekd.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/synthetic/simplekd.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/experimenters/synthetic/simplekd_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/experimenters/synthetic/simplekd_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/runners/benchmark_runner.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/runners/benchmark_runner.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/runners/benchmark_runner_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/runners/benchmark_runner_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/runners/benchmark_state.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/runners/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/runners/benchmark_state_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/runners/benchmark_state_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/benchmarks/testing/experimenter_testing.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/benchmarks/testing/experimenter_testing.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/gp_bandit_utils.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/gp_bandit_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/continuous_only_kernel.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/continuous_only_kernel.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/gaussian_process_model.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/gaussian_process_model.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/gaussian_process_model_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/gaussian_process_model_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/hebo_gp_model.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/hebo_gp_model.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/hebo_gp_model_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/hebo_gp_model_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/mask_features.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/mask_features.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/mask_features_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/mask_features_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/multitask_tuned_gp_models.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/multitask_tuned_gp_models.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/multitask_tuned_gp_models_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/multitask_tuned_gp_models_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/tuned_gp_models.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/tuned_gp_models.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/models/tuned_gp_models_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/models/tuned_gp_models_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/optimizers/core.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/optimizers/core.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/optimizers/core_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/optimizers/core_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/optimizers/jaxopt_wrappers.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/optimizers/jaxopt_wrappers.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/optimizers/jaxopt_wrappers_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/optimizers/jaxopt_wrappers_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/optimizers/optax_wrappers.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/optimizers/optax_wrappers.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/optimizers/optax_wrappers_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/optimizers/optax_wrappers_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/optimizers/testing/sinusoidal.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/optimizers/testing/sinusoidal.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/predictive_fns.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/predictive_fns.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/predictive_fns_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/predictive_fns_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/stochastic_process_model.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/stochastic_process_model.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/stochastic_process_model_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/stochastic_process_model_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/types.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/types.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/types_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/types_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/xla_pareto.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/xla_pareto.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/jax/xla_pareto_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/jax/xla_pareto_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/algorithms.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/algorithms.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/backend.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/backend.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/client.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/client.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/constants.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/constants.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/converters.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/converters.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/converters_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/converters_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/core.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/core.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/e2e_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/e2e_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/oss_vizier.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/oss_vizier.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/oss_vizier_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/oss_vizier_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/performance_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/performance_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/pythia.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/pythia.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/pythia_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/pythia_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyglove/vizier_test_lib.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyglove/vizier_test_lib.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pythia/local_policy_supporters.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pythia/local_policy_supporters.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pythia/local_policy_supporters_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pythia/local_policy_supporters_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pythia/policy.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pythia/policy.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pythia/policy_factory.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pythia/policy_factory.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pythia/policy_supporter.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pythia/policy_supporter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pythia/pythia_errors.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pythia/pythia_errors.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/multimetric/hypervolume.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/multimetric/hypervolume.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/multimetric/hypervolume_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/multimetric/hypervolume_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/multimetric/pareto_optimal.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/multimetric/pareto_optimal.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/multimetric/pareto_optimal_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/multimetric/pareto_optimal_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/multimetric/safety.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/multimetric/safety.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/multimetric/safety_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/multimetric/safety_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/oss/automated_stopping.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/oss/automated_stopping.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/oss/automated_stopping_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/oss/automated_stopping_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/oss/compare.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/oss/compare.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/oss/metadata_util.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/oss/metadata_util.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/oss/metadata_util_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/oss/metadata_util_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/oss/proto_converters.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/oss/proto_converters.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/oss/proto_converters_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/oss/proto_converters_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/oss/study_config.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/oss/study_config.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/oss/study_config_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/oss/study_config_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/pythia/study.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/pythia/study.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/base_study_config.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/base_study_config.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/base_study_config_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/base_study_config_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/common.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/common.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/common_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/common_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/context.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/context.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/context_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/context_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/parameter_config.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/parameter_config.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/parameter_config_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/parameter_config_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/parameter_iterators.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/parameter_iterators.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/parameter_iterators_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/parameter_iterators_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/study.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/study.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/trial.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/trial.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/pyvizier/shared/trial_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/pyvizier/shared/trial_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/raytune/converters.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/raytune/converters.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/raytune/converters_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/raytune/converters_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/raytune/run_tune.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/raytune/run_tune.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/raytune/run_tune_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/raytune/run_tune_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/raytune/vizier_search.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/raytune/vizier_search.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/raytune/vizier_search_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/raytune/vizier_search_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/clients.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/clients.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/clients_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/clients_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/constants.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/constants.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/custom_errors.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/custom_errors.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/datastore.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/datastore.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/datastore_test_lib.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/datastore_test_lib.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/grpc_util.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/grpc_util.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/performance_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/performance_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/policy_factory.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/policy_factory.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/pythia_service.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/pythia_service.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/pythia_util.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/pythia_util.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/ram_datastore.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/ram_datastore.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/ram_datastore_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/ram_datastore_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/resources.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/resources.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/resources_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/resources_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/service_policy_supporter.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/service_policy_supporter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/service_policy_supporter_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/service_policy_supporter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/sql_datastore.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/sql_datastore.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/sql_datastore_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/sql_datastore_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/stubs_util.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/stubs_util.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/stubs_util_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/stubs_util_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/testing/util.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/testing/util.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/types.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/types.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/vizier_client.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/vizier_client.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/vizier_client_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/vizier_client_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/vizier_server.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/vizier_server.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/vizier_service.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/vizier_service.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/_src/service/vizier_service_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/_src/service/vizier_service_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/algorithms/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/algorithms/designers/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/algorithms/designers/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/algorithms/evolution.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/algorithms/evolution.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/algorithms/policies/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/algorithms/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/benchmarks/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/benchmarks/analyzers.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/benchmarks/analyzers.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/benchmarks/experimenters/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/benchmarks/experimenters/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/benchmarks/experimenters/hpo/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/benchmarks/experimenters/hpo/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/benchmarks/experimenters/nas/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/benchmarks/experimenters/nas/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/benchmarks/experimenters/rl/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/benchmarks/experimenters/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/client/client_abc.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/client/client_abc.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/client/client_abc_testing.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/client/client_abc_testing.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/interfaces/serializable.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/interfaces/serializable.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/jax/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/jax/models.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/jax/models.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/jax/optimizers.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/jax/optimizers.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/pyglove/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/pyglove/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/pythia.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/pythia.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/core.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/core.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/core_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/core_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/embedder.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/embedder.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/embedder_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/embedder_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/feature_mapper.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/feature_mapper.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/feature_mapper_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/feature_mapper_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/input_warping.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/input_warping.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/input_warping_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/input_warping_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/jnp_converters.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/jnp_converters.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/jnp_converters_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/jnp_converters_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/padding.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/padding.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/padding_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/padding_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/spatio_temporal.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/spatio_temporal.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/converters/spatio_temporal_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/converters/spatio_temporal_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/multimetric/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/multimetric/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/pyvizier/multimetric/xla_pareto.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/pyvizier/multimetric/xla_pareto.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/raytune/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/raytune/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/service/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/service/clients/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/service/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/service/protos/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/service/protos/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/service/pyvizier/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/service/pyvizier/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/service/servers/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/service/servers/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/testing/__init__.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/testing/numpy_assertions.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/testing/numpy_assertions.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/testing/test_studies.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/testing/test_studies.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/utils/attrs_utils.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/utils/attrs_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/utils/attrs_utils_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/utils/attrs_utils_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/utils/json_utils.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/utils/json_utils_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/utils/json_utils_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/utils/profiler.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `google-vizier-dev-0.1.16.dev20240422191908/vizier/utils/profiler_test.py` & `google-vizier-dev-0.1.16.dev20240423231204/vizier/utils/profiler_test.py`

 * *Files identical despite different names*

