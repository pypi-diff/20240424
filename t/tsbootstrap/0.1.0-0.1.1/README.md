# Comparing `tmp/tsbootstrap-0.1.0.tar.gz` & `tmp/tsbootstrap-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsbootstrap-0.1.0.tar", last modified: Wed Mar 20 18:26:54 2024, max compression
+gzip compressed data, was "tsbootstrap-0.1.1.tar", last modified: Tue Apr 23 22:21:34 2024, max compression
```

## Comparing `tsbootstrap-0.1.0.tar` & `tsbootstrap-0.1.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:26:54.754843 tsbootstrap-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    27655 2024-03-20 18:26:54.754843 tsbootstrap-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23895 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 18:26:54.754843 tsbootstrap-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:26:54.742843 tsbootstrap-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:26:54.746843 tsbootstrap-0.1.0/src/tsbootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31740 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/base_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)    22281 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/base_bootstrap_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)    44911 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/block_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)    21320 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/block_bootstrap_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18410 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/block_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5953 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/block_length_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    19096 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/block_resampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    38638 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)    37658 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/markov_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/ranklags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:26:54.746843 tsbootstrap-0.1.0/src/tsbootstrap/registry/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/registry/_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/registry/_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:26:54.746843 tsbootstrap-0.1.0/src/tsbootstrap/registry/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/registry/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/registry/tests/test_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:26:54.746843 tsbootstrap-0.1.0/src/tsbootstrap/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:26:54.750843 tsbootstrap-0.1.0/src/tsbootstrap/tests/scenarios/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/tests/scenarios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10386 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/tests/scenarios/scenarios.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/tests/scenarios/scenarios_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/tests/scenarios/scenarios_getter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9479 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/tests/test_all_bootstraps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/tests/test_all_estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/tests/test_class_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/tests/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)    18914 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/time_series_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15578 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/time_series_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    33554 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/tsfit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:26:54.750843 tsbootstrap-0.1.0/src/tsbootstrap/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/utils/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/utils/estimator_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10216 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/utils/odds_and_ends.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    24394 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/src/tsbootstrap/utils/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:26:54.754843 tsbootstrap-0.1.0/src/tsbootstrap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27655 2024-03-20 18:26:54.000000 tsbootstrap-0.1.0/src/tsbootstrap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-20 18:26:54.000000 tsbootstrap-0.1.0/src/tsbootstrap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 18:26:54.000000 tsbootstrap-0.1.0/src/tsbootstrap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-20 18:26:54.000000 tsbootstrap-0.1.0/src/tsbootstrap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-20 18:26:54.000000 tsbootstrap-0.1.0/src/tsbootstrap.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:26:54.754843 tsbootstrap-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    24364 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/tests/test_base_bootstrap_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17313 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/tests/test_block_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)    18866 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/tests/test_block_bootstrap_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15236 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/tests/test_block_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/tests/test_block_length_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    19044 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/tests/test_block_resampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    67344 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)    44323 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/tests/test_markov_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/tests/test_odds_and_ends.py
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/tests/test_ranklags.py
--rw-r--r--   0 runner    (1001) docker     (127)    20440 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/tests/test_time_series_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    31589 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/tests/test_time_series_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    28338 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/tests/test_tsfit.py
--rw-r--r--   0 runner    (1001) docker     (127)    25106 2024-03-20 18:26:48.000000 tsbootstrap-0.1.0/tests/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:21:34.700382 tsbootstrap-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    28664 2024-04-23 22:21:34.700382 tsbootstrap-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24350 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 22:21:34.700382 tsbootstrap-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:21:34.684382 tsbootstrap-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:21:34.688382 tsbootstrap-0.1.1/src/tsbootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35434 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/base_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22345 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/base_bootstrap_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47867 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/block_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21494 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/block_bootstrap_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19042 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/block_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/block_length_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21433 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/block_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37989 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38239 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/markov_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/ranklags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:21:34.692382 tsbootstrap-0.1.1/src/tsbootstrap/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/registry/_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/registry/_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:21:34.692382 tsbootstrap-0.1.1/src/tsbootstrap/registry/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/registry/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/registry/tests/test_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:21:34.692382 tsbootstrap-0.1.1/src/tsbootstrap/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:21:34.692382 tsbootstrap-0.1.1/src/tsbootstrap/tests/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/tests/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10386 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/tests/scenarios/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/tests/scenarios/scenarios_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/tests/scenarios/scenarios_getter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10700 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/tests/test_all_bootstraps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/tests/test_all_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/tests/test_class_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/tests/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19121 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/time_series_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15811 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/time_series_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33554 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/tsfit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:21:34.692382 tsbootstrap-0.1.1/src/tsbootstrap/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/utils/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/utils/estimator_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10327 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/utils/odds_and_ends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24567 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/src/tsbootstrap/utils/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:21:34.696382 tsbootstrap-0.1.1/src/tsbootstrap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28664 2024-04-23 22:21:34.000000 tsbootstrap-0.1.1/src/tsbootstrap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-23 22:21:34.000000 tsbootstrap-0.1.1/src/tsbootstrap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 22:21:34.000000 tsbootstrap-0.1.1/src/tsbootstrap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-23 22:21:34.000000 tsbootstrap-0.1.1/src/tsbootstrap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 22:21:34.000000 tsbootstrap-0.1.1/src/tsbootstrap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:21:34.696382 tsbootstrap-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    24339 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/tests/test_base_bootstrap_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17184 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/tests/test_block_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18866 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/tests/test_block_bootstrap_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15152 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/tests/test_block_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/tests/test_block_length_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18398 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/tests/test_block_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67344 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/tests/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44323 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/tests/test_markov_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/tests/test_odds_and_ends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/tests/test_ranklags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20407 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/tests/test_time_series_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32475 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/tests/test_time_series_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28178 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/tests/test_tsfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25106 2024-04-23 22:21:19.000000 tsbootstrap-0.1.1/tests/test_validate.py
```

### Comparing `tsbootstrap-0.1.0/LICENSE` & `tsbootstrap-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tsbootstrap-0.1.0/PKG-INFO` & `tsbootstrap-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsbootstrap
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package to generate bootstrapped time series
 Author-email: Sankalp Gilda <sankalp.gilda@gmail.com>
 Maintainer-email: Sankalp Gilda <sankalp.gilda@gmail.com>, Franz Kiraly <franz.kiraly@sktime.net>, Benedikt Heidrich <benedikt.heidrich@sktime.net>
 License: MIT License
         
         Copyright (c) 2023 Sankalp Gilda
         
@@ -49,36 +49,48 @@
 Requires-Dist: packaging
 Provides-Extra: all-extras
 Requires-Dist: arch<6.0.0,>=5.0.0; extra == "all-extras"
 Requires-Dist: hmmlearn<0.3.2,>=0.3.0; extra == "all-extras"
 Requires-Dist: pyclustering<0.11.0,>=0.10.0; extra == "all-extras"
 Requires-Dist: scikit_learn_extra<0.4.0,>=0.3.0; extra == "all-extras"
 Requires-Dist: statsmodels<0.15.0,>=0.12.1; extra == "all-extras"
+Requires-Dist: dtaidistance; python_version < "3.10" and extra == "all-extras"
 Provides-Extra: docs
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: jupyter; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: nbsphinx>=0.8.6; extra == "docs"
 Requires-Dist: numpydoc; extra == "docs"
 Requires-Dist: pydata-sphinx-theme; extra == "docs"
 Requires-Dist: Sphinx!=7.2.0,<8.0.0; extra == "docs"
 Requires-Dist: sphinx-rtd-theme>=1.3.0; extra == "docs"
-Requires-Dist: sphinx-copybutton; extra == "docs"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "docs"
 Requires-Dist: sphinx-design<0.6.0; extra == "docs"
 Requires-Dist: sphinx-gallery<0.15.0; extra == "docs"
 Requires-Dist: sphinx-issues<4.0.0; extra == "docs"
 Requires-Dist: sphinx-version-warning; extra == "docs"
-Requires-Dist: tabulate; extra == "docs"
+Requires-Dist: tabulate>=0.9.0; extra == "docs"
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
+Requires-Dist: black>=24.3.0; extra == "dev"
 Requires-Dist: blacken-docs; extra == "dev"
 Requires-Dist: hypothesis; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: github-actions; extra == "dev"
+Requires-Dist: importlib-metadata; extra == "dev"
+Requires-Dist: pip-tools; extra == "dev"
+Requires-Dist: pyright; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: autoflake; extra == "dev"
+Requires-Dist: typos; extra == "dev"
+Requires-Dist: tox; extra == "dev"
+Requires-Dist: tox-gh-actions; extra == "dev"
+Requires-Dist: pycobertura; extra == "dev"
+Requires-Dist: tomlkit; extra == "dev"
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/github/all-contributors/astrogilda/tsbootstrap?color=ee8449&style=flat-square)](#contributors)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 
 <div align="center">
@@ -103,127 +115,117 @@
     <a href="https://pepy.tech/project/tsbootstrap">
         <img src="https://static.pepy.tech/badge/tsbootstrap" alt="Downloads"/>
     </a>
     <img src="https://img.shields.io/github/license/eli64s/readme-ai?color=5D6D7E" alt="github-license" />
     </a>
     <img src="https://github.com/astrogilda/tsbootstrap/workflows/CI/badge.svg" alt="Build Status"/>
     <a href="https://codecov.io/gh/astrogilda/tsbootstrap"><img src="https://codecov.io/gh/astrogilda/tsbootstrap/branch/main/graph/badge.svg" alt="codecov"/></a>
-    <a href="https://doi.org/10.5281/zenodo.8226496"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.8226496.svg" alt="DOI"/></a>
+    <a href="https://doi.org/10.5281/zenodo.8226495"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.8226495.svg" alt="DOI"/></a>
     <a href="https://codeclimate.com/github/astrogilda/tsbootstrap/maintainability"><img src="https://api.codeclimate.com/v1/badges/d80a0615a8c00f31565c/maintainability" alt="Code Quality"/></a>
     <img src="https://img.shields.io/github/last-commit/astrogilda/tsbootstrap" alt="Last Commit"/>
     <img src="https://img.shields.io/github/issues/astrogilda/tsbootstrap" alt="Issues"/>
     <img src="https://img.shields.io/github/issues-pr/astrogilda/tsbootstrap" alt="Pull Requests"/>
     <img src="https://img.shields.io/github/v/tag/astrogilda/tsbootstrap" alt="Tag"/>
 </div>
 
 
 
 ## 📒 Table of Contents
-1. [📍 Time Series Bootstrapping](#time-series-bootstrapping)
-    - [Overview](#overview)
-    - [Bootstrapping Methodology](#bootstrapping-methodology)
-    - [Block Bootstrap](#block-bootstrap)
-        - [Moving Block Bootstrap](#moving-block-bootstrap)
-        - [Circular Block Bootstrap](#circular-block-bootstrap)
-        - [Stationary Block Bootstrap](#stationary-block-bootstrap)
-        - [NonOverlapping Block Bootstrap](#nonoverlapping-block-bootstrap)
-        - [Bartletts Bootstrap](#bartletts-bootstrap)
-        - [Blackman Bootstrap](#blackman-bootstrap)
-        - [Hamming Bootstrap](#hamming-bootstrap)
-        - [Hanning Bootstrap](#hanning-bootstrap)
-        - [Tukey Bootstrap](#tukey-bootstrap)
-    - [Residual Bootstrap](#residual-bootstrap)
-    - [Bias Corrected Bootstrap](#bias-corrected-bootstrap)
-    - [Distribution Bootstrap](#distribution-bootstrap)
-    - [Markov Bootstrap](#markov-bootstrap)
-    - [Sieve Bootstrap](#sieve-bootstrap)
-3. [🧩 Modules](#-modules)
-4. [🚀 Getting Started](#-getting-started)
-5. [🗺 Roadmap](#-roadmap)
-6. [🤝 Contributing](#-contributing)
-7. [📄 License](#-license)
-8. [👏 Acknowledgments](#-acknowledgments)
 
+1. [🚀 Getting Started](#-getting-started)
+2. [🧩 Modules](#-modules)
+3. [🗺 Roadmap](#-roadmap)
+4. [🤝 Contributing](#-contributing)
+5. [📄 License](#-license)
+6. [📍 Time Series Bootstrapping Methods intro](#time-series-bootstrapping)
+7. [👏 Contributors](#-contributors)
 
----
 
 
-## 📍 Time Series Bootstrapping
-`tsbootstrap` is a comprehensive project designed to implement an array of bootstrapping techniques specifically tailored for time series data. This project is targeted towards data scientists, statisticians, economists, and other professionals or researchers who regularly work with time series data and require robust methods for generating bootstrapped copies of univariate and multivariate time series data.
+---
 
-### Overview
-Time series bootstrapping is a nuanced resampling method that is applied to time-dependent data. Traditional bootstrapping methods often assume independence between data points, which is an assumption that does not hold true for time series data where a data point is often dependent on previous data points. Time series bootstrapping techniques respect the chronological order and correlations of the data, providing more accurate estimates of uncertainty or variability.
+## 🚀 Getting Started
 
-### Bootstrapping Methodology
-The `tsbootstrap` project offers a diverse set of bootstrapping techniques that can be applied to either the entire input time series (classes prefixed with `Whole`), or after partitioning the data into blocks (classes prefixed with `Block`). These methodologies can be applied directly to the raw input data or to the residuals obtained after fitting one of the five statistical models defined in `time_series_model.py` (classes with `Residual` in their names).
 
-### Block Bootstrap
-Block Bootstrap is a prevalent approach in time series bootstrapping. It involves resampling blocks of consecutive data points, thus respecting the internal structures of the data. There are several techniques under Block Bootstrap, each with its unique approach. `tsbootstrap` provides highly flexible block bootstrapping, allowing the user to specify the block length sampling, block generation, and block resampling strategies. For additional details, refer to `block_length_sampler.py`, `block_generator.py`, and `block_resampler.py`.
+### 🎮 Using tsbootstrap
 
-The Moving Block Bootstrap, Circular Block Bootstrap, Stationary Block Bootstrap, and NonOverlapping Block Bootstrap methods are all variations of the Block Bootstrap that use different methods to sample the data, maintaining various types of dependencies.
+`tsbootstrap` provides a unified, `sklearn`-like interface to all bootstrap methods.
 
-Bartlett's, Blackman's, Hamming's, Hanning's, and Tukey's Bootstrap methods are specific implementations of the Block Bootstrap that use different window shapes to taper the data, reducing the influence of data points far from the center. In `tsbootstrap`, these methods inherit from `MovingBlockBootstrap`, but can easily be modified to inherit from any of the other three base block bootstrapping classes.
+Example using a `MovingBlockBootstrap` - all bootstrap algorithms follow
+the same interface!
 
-Each method comes with its distinct strengths and weaknesses. The choice of method should be based on the characteristics of the data and the specific requirements of the analysis.
+```python
+from tsbootstrap import MovingBlockBootstrap
+import numpy as np
 
-#### (i) Moving Block Bootstrap
-This method is implemented in `MovingBlockBootstrap` and is used for time series data where blocks of data are resampled to maintain the dependency structure within the blocks. It's useful when the data has dependencies that need to be preserved. It's not recommended when the data does not have any significant dependencies.
+# Create custom time series data. While below is for univariate time series, the bootstraps can handle multivariate time series as well.
+n_samples = 10
+X = np.arange(n_samples)
 
-#### (ii) Circular Block Bootstrap
-This method is implemented in `CircularBlockBootstrap` and treats the data as if it is circular (the end of the data is next to the beginning of the data). It's useful when the data is cyclical or seasonal in nature. It's not recommended when the data does not have a cyclical or seasonal component.
+# Instantiate the bootstrap object
+n_bootstraps = 3
+block_length = 3
+rng = 42
+mbb = MovingBlockBootstrap(n_bootstraps=n_bootstraps, rng=rng, block_length=block_length)
+
+# Generate bootstrapped samples
+return_indices = False
+bootstrapped_samples = mbb.bootstrap(
+    X, return_indices=return_indices)
+
+# Collect bootstrap samples
+X_bootstrapped = []
+for data in bootstrapped_samples:
+    X_bootstrapped.append(data)
 
-#### (iii) Stationary Block Bootstrap
-This method is implemented in `StationaryBlockBootstrap` and randomly resamples blocks of data with block lengths that follow a geometric distribution. It's useful for time series data where the degree of dependency needs to be preserved, and it doesn't require strict stationarity of the underlying process. It's not recommended when the data has strong seasonality or trend components which violate the weak dependence assumption.
+X_bootstrapped = np.array(X_bootstrapped)
+```
 
-#### (iv) NonOverlapping Block Bootstrap
- This method is implemented in `NonOverlappingBlockBootstrap` and resamples blocks of data without overlap. It's useful when the data has dependencies that need to be preserved and when overfitting is a concern. It's not recommended when the data does not have any significant dependencies or when the introduction of bias due to non-overlapping selection is a concern.
+### 📦 Installation and Setup
 
-#### (v) Bartlett's Bootstrap
- Bartlett's method is a time series bootstrap method that uses a window or filter that tapers off as you move away from the center of the window. It's useful when you have a large amount of data and you want to reduce the influence of the data points far away from the center. This method is not advised when the tapering of data points is not desired or when the dataset is small as the tapered data points might contain valuable information. It is implemented in `BartlettsBootstrap`.
+``tsbootstrap`` is installed via ``pip``, either from PyPI or locally.
 
-#### (vi) Blackman Bootstrap
-Similar to Bartlett's method, Blackman's method uses a window that tapers off as you move away from the center of the window. The key difference is the shape of the window (Blackman window has a different shape than Bartlett). It's useful when you want to reduce the influence of the data points far from the center with a different window shape. It's not recommended when the dataset is small or tapering of data points is not desired. It is implemented in `BlackmanBootstrap`.
+#### ✔️ Prerequisites
 
-#### (vii) Hamming Bootstrap
- Similar to the Bartlett and Blackman methods, the Hamming method uses a specific type of window function. It's useful when you want to reduce the influence of the data points far from the center with the Hamming window shape. It's not recommended for small datasets or when tapering of data points is not desired. It is implemented in `HammingBootstrap`.
+- Python (3.8 or higher)
+- `pip` (latest version recommended), plus suitable environment manager (`venv`, `conda`)
 
-#### (viii) Hanning Bootstrap
-This method also uses a specific type of window function. It's useful when you want to reduce the influence of the data points far from the center with the Hanning window shape. It's not recommended for small datasets or when tapering of data points is not desired. It is implemented in `HanningBootstrap`.
+You can also consider using ``uv`` to speed up environment setu.
 
-#### (ix) Tukey Bootstrap
-Similar to the Bartlett, Blackman, Hamming, and Hanning methods, the Tukey method uses a specific type of window function. It's useful when you want to reduce the influence of the data points far from the center with the Tukey window shape. It's not recommended for small datasets or when tapering of data points is not desired. It is implemented in `TukeyBootstrap`.
+#### Installing from PyPI
 
-### Residual Bootstrap
-Residual Bootstrap is a method designed for time series data where a model is fit to the data, and the residuals (the difference between the observed and predicted data) are bootstrapped. It's particularly useful when a good model fit is available for the data. However, it's not recommended when a model fit is not available or is poor. `tsbootstrap` provides four time series models to fit to the input data -- `AutoReg`, `ARIMA`, `SARIMA`, and `VAR` (for multivariate input time series data). For more details, refer to `time_series_model.py` and `tsfit.py`.
+To install the latest release of `tsbootstrap` directly from PyPI, run:
 
-### Statistic-Preserving Bootstrap
-Statistic-Preserving Bootstrap is a unique method designed to generate bootstrapped time series data while preserving a specific statistic of the original data. This method can be beneficial in scenarios where it's important to maintain the original data's characteristics in the bootstrapped samples. It is implemented in `StatisticPreservingBootstrap`.
+```sh
+pip install tsbootstrap
+```
 
-### Distribution Bootstrap
-Distribution Bootstrap generates bootstrapped samples by fitting a distribution to the residuals and then generating new residuals from the fitted distribution. The new residuals are then added to the fitted values to create the bootstrapped samples. This method is based on the assumption that the residuals follow a specific distribution (like Gaussian, Poisson, etc). It's not recommended when the distribution of residuals is unknown or hard to determine. It is implemented in `DistributionBootstrap`.
+To install with all optional dependencies:
 
-### Markov Bootstrap
-Markov Bootstrap is used for bootstrapping time series data where the residuals of the data are presumed to follow a Markov process. This method is especially useful in scenarios where the current residual primarily depends on the previous one, with little to no dependency on residuals from further in the past. Markov Bootstrap technique is designed to preserve this dependency structure in the bootstrapped samples, making it particularly valuable for time series data that exhibits Markov properties. However, it's not advisable when the residuals of the time series data exhibit long-range dependencies, as the Markov assumption of limited dependency may not hold true. It is implemented in `MarkovBootstrap`. See `markov_sampler.py` for implementation details.
+```
+pip install "tsbootstrap[all_extras]"
+```
+---
 
-### Sieve Bootstrap
-Sieve Bootstrap is designed for handling dependent data, where the residuals of the time series data follow an autoregressive process. This method aims to preserve and simulate the dependencies inherent in the original data within the bootstrapped samples. It operates by approximating the autoregressive process ofthe residuals using a finite order autoregressive model. The order of the model is determined based on the data, and the residuals are then bootstrapped. The Sieve Bootstrap technique is particularly valuable for time series data that exhibits autoregressive properties. However, it's not advisable when the residuals of the time series data do not follow an autoregressive process. It is implemented in `SieveBootstrap`. See `time_series_simulator.py` for implementations details.
+Bootstrap algorithms manage their own dependencies - if an extra is needed but not
+present, the object will raise this at construction.
 
 ## 🧩 Modules
 The `tsbootstrap` package contains various modules that handle tasks such as bootstrapping, time series simulation, and utility functions. This modular approach ensures flexibility, extensibility, and ease of maintenance.
 
 
 <details closed><summary>root</summary>
 
 | File                                                                                       | Summary                   |
 | ---                                                                                        | ---                       |
 | [setup.sh](https://github.com/astrogilda/tsbootstrap/blob/main/setup.sh)                         | Shell script for initial setup and environment configuration. |
 | [commitlint.config.js](https://github.com/astrogilda/tsbootstrap/blob/main/commitlint.config.js) | Configuration for enforcing conventional commit messages. |
 | [CITATION.cff](https://github.com/astrogilda/tsbootstrap/blob/main/CITATION.cff)                 | Citation metadata for the project. |
 | [CODE_OF_CONDUCT.md](https://github.com/astrogilda/tsbootstrap/blob/main/CODE_OF_CONDUCT.md)                 | Guidelines for community conduct and interactions. |
-| [CONTRIBUTING.md](https://github.com/astrogilda/tsbootstrap/blob/main/CITATION.md)                 | Instructions for contributing to the project. |
+| [CONTRIBUTING.md](https://github.com/astrogilda/tsbootstrap/blob/main/CONTRIBUTING.md)                 | Instructions for contributing to the project. |
 | [.codeclimate.yml](https://github.com/astrogilda/tsbootstrap/blob/main/.codeclimate.yml)                 | Configuration for Code Climate quality checks. |
 | [.gitignore](https://github.com/astrogilda/tsbootstrap/blob/main/.gitignore)                 | Specifies files and folders to be ignored by Git. |
 | [.pre-commit-config.yaml](https://github.com/astrogilda/tsbootstrap/blob/main/.pre-commit-config.yaml)                 | Configuration for pre-commit hooks. |
 | [poetry.toml](https://github.com/astrogilda/tsbootstrap/blob/main/poetry.toml)                 | Configuration file for Poetry package management. |
 | [tsbootstrap_logo.png](https://github.com/astrogilda/tsbootstrap/blob/main/tsbootstrap_logo.png)                 | Project logo image. |
 
 </details>
@@ -257,116 +259,76 @@
 | ---                                                                                                | ---                       |
 | [types.py](https://github.com/astrogilda/tsbootstrap/blob/main/src/tsbootstrap/utils/types.py)                 | Defines custom types used across the project. |
 | [validate.py](https://github.com/astrogilda/tsbootstrap/blob/main/src/tsbootstrap/utils/validate.py)           | Contains validation utilities. |
 | [odds_and_ends.py](https://github.com/astrogilda/tsbootstrap/blob/main/src/tsbootstrap/utils/odds_and_ends.py) | Contains miscellaneous utility functions. |
 
 </details>
 
----
 
-## 🚀 Getting Started
+## 🗺 Roadmap
 
-### ✔️ Prerequisites
+This is an abridged version; for the complete and evolving list of plans and improvements, see [Issue #144](https://github.com/astrogilda/tsbootstrap/issues/144).
 
-Before you begin, ensure that you have the following prerequisites installed:
-> - `ℹ️ Requirement 1`
-> - `ℹ️ Requirement 2`
-> - `ℹ️ ...`
+### Performance and Scaling
+ -handling large datasets, distributed backend integration (`Dask`, `Spark`, `Ray`), profiling/optimization
+### Tuning and AutoML
+ -adaptive block length, adaptive resampling, evaluation based parameter selection
+### Real-time and Stream Data
+ -stream bootstraps, data update interface
+### Stage 2 `sktime` Integration
+ -evaluation module, datasets, benchmarks, sktime forecasters in bootstraps
+### API and Capability Extension
+ -panel/hierarchical data, exogenous data, update/stream, model state management
+### Scope Extension (TBD)
+ -time series augmentation, fully probabilistic models
 
-### 📦 Installation and Setup
+## 🤝 Contributing
 
-This project comes with a `setup.sh` script to ease the setup process. The script will create a new Python virtual environment, install the necessary dependencies, and handle some version-specific installations.
+Contributions are always welcome!
 
-Here are the steps to follow:
+See our [good first issues ](https://github.com/astrogilda/tsbootstrap/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
+for getting started.
 
-1. Ensure that you have Python, Poetry, and Bash installed on your system. If not, you can install them using the links below:
-    - [Python](https://www.python.org/downloads/)
-    - [Poetry](https://python-poetry.org/docs/#installation)
-    - [Bash](https://www.gnu.org/software/bash/)
+Below is a quick start guide to contributing.
 
-2. Clone the tsbootstrap repository:
-```sh
-git clone https://github.com/astrogilda/tsbootstrap
-```
+### Developer setup
 
-3. Change to the project directory:
-```sh
-cd tsbootstrap
-```
+1. Fork the tsbootstrap repository
 
-4. Make the `setup.sh` script executable:
+2. Clone the fork to local:
 ```sh
-chmod +x setup.sh
+git clone https://github.com/astrogilda/tsbootstrap
 ```
 
-5. Run the `setup.sh` script:
-```sh
-./setup.sh
-```
+3. In the local repository root, set up a python environment, e.g., `venv` or `conda`.
 
-The `setup.sh` script sets up a Python environment using Poetry, locks and installs the necessary dependencies, and installs `dtaidistance` if the Python version is 3.9 or lower.
 
-6. Activate the python shell:
-```sh
-poetry shell
+4. Editable install via `pip`, including developer dependencies:
+```
+pip install -e .[dev]
 ```
 
-That's it! You are now set up and ready to go.
-
-### 🎮 Using tsbootstrap
-
-Here's a basic example using the Moving Block Bootstrap method:
-
-```python
-from tsbootstrap import MovingBlockBootstrap, MovingBlockBootstrapConfig
-import numpy as np
-
-np.random.seed(0)
-
-# Create custom time series data
-
-n_samples = 1000
-
-y = np.random.normal(0, 1, n_samples).cumsum()
-
-x1 = np.arange(1, n_samples + 1).reshape(-1, 1)
-x2 = np.random.normal(0, 1, (n_samples, 1))
-exog = np.concatenate([x1, x2], axis=1)
+The editable install ensures that changes to the package are reflected in
+your environment.
 
-# Instantiate the bootstrap object
-mbb_config = MovingBlockBootstrapConfig(
-    n_bootstraps=1000, rng=42, block_length=10
-)
-mbb = MovingBlockBootstrap(config=mbb_config)
+### Verifying the Installation
 
-# Generate the generator for 1000 bootstrapped samples
-bootstrapped_samples = bootstrap.bootstrap(n=1000)
+After installation, you can verify that tsbootstrap has been installed correctly by checking its version or by trying to import it in Python:
 ```
-
-### 🧪 Running Tests
-```sh
-pytest tests/
+python -c "import tsbootstrap; print(tsbootstrap.__version__)"
 ```
 
----
-
-
-## 🗺 Roadmap
-
-> - [ ] `ℹ️  Task 1: in distributionbootstrap, allow mixture of distributions`
-> - [ ] `ℹ️  Task 2: allow fractional block_length`
-> - [ ] `ℹ️  Task 3: enable multi-processing`
-> - [ ] `ℹ️  Task 4: test -- for biascorrectblockbootstrap, see if the statistic on the bootstrapped sample is close to the statistic on the original sample`
+This command should output the version number of tsbootstrap without any errors, indicating that the installation was successful.
 
+That's it! You are now set up and ready to go. You can start using tsbootstrap for your time series bootstrapping needs.
 
-## 🤝 Contributing
+### Contribution workflow
 
 Contributions are always welcome! Please follow these steps:
-1. Fork the project repository. This creates a copy of the project on your account that you can modify without affecting the original project.
-2. Clone the forked repository to your local machine using a Git client like Git or GitHub Desktop.
+
 3. Create a new branch with a descriptive name (e.g., `new-feature-branch` or `bugfix-issue-123`).
 ```sh
 git checkout -b new-feature-branch
 ```
 4. Make changes to the project's codebase.
 5. Commit your changes to your local branch with a clear commit message that explains the changes you've made.
 ```sh
@@ -375,14 +337,33 @@
 6. Push your changes to your forked repository on GitHub using the following command
 ```sh
 git push origin new-feature-branch
 ```
 7. Create a new pull request to the original project repository. In the pull request, describe the changes you've made and why they're necessary.
 The project maintainers will review your changes and provide feedback or merge them into the main branch.
 
+### 🧪 Running Tests
+
+To run all tests, in your developer environment, run:
+
+```sh
+pytest tests/
+```
+
+Individual bootstrap algorithms can be tested as follows:
+
+```python
+from tsbootstrap.utils import check_estimator
+
+check_estimator(my_bootstrap_algo)
+```
+
+### Contribution guide
+
+For more detailed information on how to contribute, please refer to our [CONTRIBUTING.md](https://github.com/astrogilda/tsbootstrap/blob/main/CONTRIBUTING.md)  guide.
 ---
 
 ## 📄 License
 
 This project is licensed under the `ℹ️  MIT` License. See the [LICENSE](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository) file for additional info.
 
 ---
@@ -396,7 +377,71 @@
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+
+
+---
+
+
+## 📍 Time Series Bootstrapping
+`tsbootstrap` is a comprehensive project designed to implement an array of bootstrapping techniques specifically tailored for time series data. This project is targeted towards data scientists, statisticians, economists, and other professionals or researchers who regularly work with time series data and require robust methods for generating bootstrapped copies of univariate and multivariate time series data.
+
+### Overview
+Time series bootstrapping is a nuanced resampling method that is applied to time-dependent data. Traditional bootstrapping methods often assume independence between data points, which is an assumption that does not hold true for time series data where a data point is often dependent on previous data points. Time series bootstrapping techniques respect the chronological order and correlations of the data, providing more accurate estimates of uncertainty or variability.
+
+### Bootstrapping Methodology
+The `tsbootstrap` project offers a diverse set of bootstrapping techniques that can be applied to either the entire input time series (classes prefixed with `Whole`), or after partitioning the data into blocks (classes prefixed with `Block`). These methodologies can be applied directly to the raw input data or to the residuals obtained after fitting one of the five statistical models defined in `time_series_model.py` (classes with `Residual` in their names).
+
+### Block Bootstrap
+Block Bootstrap is a prevalent approach in time series bootstrapping. It involves resampling blocks of consecutive data points, thus respecting the internal structures of the data. There are several techniques under Block Bootstrap, each with its unique approach. `tsbootstrap` provides highly flexible block bootstrapping, allowing the user to specify the block length sampling, block generation, and block resampling strategies. For additional details, refer to `block_length_sampler.py`, `block_generator.py`, and `block_resampler.py`.
+
+The Moving Block Bootstrap, Circular Block Bootstrap, Stationary Block Bootstrap, and NonOverlapping Block Bootstrap methods are all variations of the Block Bootstrap that use different methods to sample the data, maintaining various types of dependencies.
+
+Bartlett's, Blackman's, Hamming's, Hanning's, and Tukey's Bootstrap methods are specific implementations of the Block Bootstrap that use different window shapes to taper the data, reducing the influence of data points far from the center. In `tsbootstrap`, these methods inherit from `MovingBlockBootstrap`, but can easily be modified to inherit from any of the other three base block bootstrapping classes.
+
+Each method comes with its distinct strengths and weaknesses. The choice of method should be based on the characteristics of the data and the specific requirements of the analysis.
+
+#### (i) Moving Block Bootstrap
+This method is implemented in `MovingBlockBootstrap` and is used for time series data where blocks of data are resampled to maintain the dependency structure within the blocks. It's useful when the data has dependencies that need to be preserved. It's not recommended when the data does not have any significant dependencies.
+
+#### (ii) Circular Block Bootstrap
+This method is implemented in `CircularBlockBootstrap` and treats the data as if it is circular (the end of the data is next to the beginning of the data). It's useful when the data is cyclical or seasonal in nature. It's not recommended when the data does not have a cyclical or seasonal component.
+
+#### (iii) Stationary Block Bootstrap
+This method is implemented in `StationaryBlockBootstrap` and randomly resamples blocks of data with block lengths that follow a geometric distribution. It's useful for time series data where the degree of dependency needs to be preserved, and it doesn't require strict stationarity of the underlying process. It's not recommended when the data has strong seasonality or trend components which violate the weak dependence assumption.
+
+#### (iv) NonOverlapping Block Bootstrap
+ This method is implemented in `NonOverlappingBlockBootstrap` and resamples blocks of data without overlap. It's useful when the data has dependencies that need to be preserved and when overfitting is a concern. It's not recommended when the data does not have any significant dependencies or when the introduction of bias due to non-overlapping selection is a concern.
+
+#### (v) Bartlett's Bootstrap
+ Bartlett's method is a time series bootstrap method that uses a window or filter that tapers off as you move away from the center of the window. It's useful when you have a large amount of data and you want to reduce the influence of the data points far away from the center. This method is not advised when the tapering of data points is not desired or when the dataset is small as the tapered data points might contain valuable information. It is implemented in `BartlettsBootstrap`.
+
+#### (vi) Blackman Bootstrap
+Similar to Bartlett's method, Blackman's method uses a window that tapers off as you move away from the center of the window. The key difference is the shape of the window (Blackman window has a different shape than Bartlett). It's useful when you want to reduce the influence of the data points far from the center with a different window shape. It's not recommended when the dataset is small or tapering of data points is not desired. It is implemented in `BlackmanBootstrap`.
+
+#### (vii) Hamming Bootstrap
+ Similar to the Bartlett and Blackman methods, the Hamming method uses a specific type of window function. It's useful when you want to reduce the influence of the data points far from the center with the Hamming window shape. It's not recommended for small datasets or when tapering of data points is not desired. It is implemented in `HammingBootstrap`.
+
+#### (viii) Hanning Bootstrap
+This method also uses a specific type of window function. It's useful when you want to reduce the influence of the data points far from the center with the Hanning window shape. It's not recommended for small datasets or when tapering of data points is not desired. It is implemented in `HanningBootstrap`.
+
+#### (ix) Tukey Bootstrap
+Similar to the Bartlett, Blackman, Hamming, and Hanning methods, the Tukey method uses a specific type of window function. It's useful when you want to reduce the influence of the data points far from the center with the Tukey window shape. It's not recommended for small datasets or when tapering of data points is not desired. It is implemented in `TukeyBootstrap`.
+
+### Residual Bootstrap
+Residual Bootstrap is a method designed for time series data where a model is fit to the data, and the residuals (the difference between the observed and predicted data) are bootstrapped. It's particularly useful when a good model fit is available for the data. However, it's not recommended when a model fit is not available or is poor. `tsbootstrap` provides four time series models to fit to the input data -- `AutoReg`, `ARIMA`, `SARIMA`, and `VAR` (for multivariate input time series data). For more details, refer to `time_series_model.py` and `tsfit.py`.
+
+### Statistic-Preserving Bootstrap
+Statistic-Preserving Bootstrap is a unique method designed to generate bootstrapped time series data while preserving a specific statistic of the original data. This method can be beneficial in scenarios where it's important to maintain the original data's characteristics in the bootstrapped samples. It is implemented in `StatisticPreservingBootstrap`.
+
+### Distribution Bootstrap
+Distribution Bootstrap generates bootstrapped samples by fitting a distribution to the residuals and then generating new residuals from the fitted distribution. The new residuals are then added to the fitted values to create the bootstrapped samples. This method is based on the assumption that the residuals follow a specific distribution (like Gaussian, Poisson, etc). It's not recommended when the distribution of residuals is unknown or hard to determine. It is implemented in `DistributionBootstrap`.
+
+### Markov Bootstrap
+Markov Bootstrap is used for bootstrapping time series data where the residuals of the data are presumed to follow a Markov process. This method is especially useful in scenarios where the current residual primarily depends on the previous one, with little to no dependency on residuals from further in the past. Markov Bootstrap technique is designed to preserve this dependency structure in the bootstrapped samples, making it particularly valuable for time series data that exhibits Markov properties. However, it's not advisable when the residuals of the time series data exhibit long-range dependencies, as the Markov assumption of limited dependency may not hold true. It is implemented in `MarkovBootstrap`. See `markov_sampler.py` for implementation details.
+
+### Sieve Bootstrap
+Sieve Bootstrap is designed for handling dependent data, where the residuals of the time series data follow an autoregressive process. This method aims to preserve and simulate the dependencies inherent in the original data within the bootstrapped samples. It operates by approximating the autoregressive process ofthe residuals using a finite order autoregressive model. The order of the model is determined based on the data, and the residuals are then bootstrapped. The Sieve Bootstrap technique is particularly valuable for time series data that exhibits autoregressive properties. However, it's not advisable when the residuals of the time series data do not follow an autoregressive process. It is implemented in `SieveBootstrap`. See `time_series_simulator.py` for implementations details.
```

### Comparing `tsbootstrap-0.1.0/README.md` & `tsbootstrap-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -25,127 +25,117 @@
     <a href="https://pepy.tech/project/tsbootstrap">
         <img src="https://static.pepy.tech/badge/tsbootstrap" alt="Downloads"/>
     </a>
     <img src="https://img.shields.io/github/license/eli64s/readme-ai?color=5D6D7E" alt="github-license" />
     </a>
     <img src="https://github.com/astrogilda/tsbootstrap/workflows/CI/badge.svg" alt="Build Status"/>
     <a href="https://codecov.io/gh/astrogilda/tsbootstrap"><img src="https://codecov.io/gh/astrogilda/tsbootstrap/branch/main/graph/badge.svg" alt="codecov"/></a>
-    <a href="https://doi.org/10.5281/zenodo.8226496"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.8226496.svg" alt="DOI"/></a>
+    <a href="https://doi.org/10.5281/zenodo.8226495"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.8226495.svg" alt="DOI"/></a>
     <a href="https://codeclimate.com/github/astrogilda/tsbootstrap/maintainability"><img src="https://api.codeclimate.com/v1/badges/d80a0615a8c00f31565c/maintainability" alt="Code Quality"/></a>
     <img src="https://img.shields.io/github/last-commit/astrogilda/tsbootstrap" alt="Last Commit"/>
     <img src="https://img.shields.io/github/issues/astrogilda/tsbootstrap" alt="Issues"/>
     <img src="https://img.shields.io/github/issues-pr/astrogilda/tsbootstrap" alt="Pull Requests"/>
     <img src="https://img.shields.io/github/v/tag/astrogilda/tsbootstrap" alt="Tag"/>
 </div>
 
 
 
 ## 📒 Table of Contents
-1. [📍 Time Series Bootstrapping](#time-series-bootstrapping)
-    - [Overview](#overview)
-    - [Bootstrapping Methodology](#bootstrapping-methodology)
-    - [Block Bootstrap](#block-bootstrap)
-        - [Moving Block Bootstrap](#moving-block-bootstrap)
-        - [Circular Block Bootstrap](#circular-block-bootstrap)
-        - [Stationary Block Bootstrap](#stationary-block-bootstrap)
-        - [NonOverlapping Block Bootstrap](#nonoverlapping-block-bootstrap)
-        - [Bartletts Bootstrap](#bartletts-bootstrap)
-        - [Blackman Bootstrap](#blackman-bootstrap)
-        - [Hamming Bootstrap](#hamming-bootstrap)
-        - [Hanning Bootstrap](#hanning-bootstrap)
-        - [Tukey Bootstrap](#tukey-bootstrap)
-    - [Residual Bootstrap](#residual-bootstrap)
-    - [Bias Corrected Bootstrap](#bias-corrected-bootstrap)
-    - [Distribution Bootstrap](#distribution-bootstrap)
-    - [Markov Bootstrap](#markov-bootstrap)
-    - [Sieve Bootstrap](#sieve-bootstrap)
-3. [🧩 Modules](#-modules)
-4. [🚀 Getting Started](#-getting-started)
-5. [🗺 Roadmap](#-roadmap)
-6. [🤝 Contributing](#-contributing)
-7. [📄 License](#-license)
-8. [👏 Acknowledgments](#-acknowledgments)
 
+1. [🚀 Getting Started](#-getting-started)
+2. [🧩 Modules](#-modules)
+3. [🗺 Roadmap](#-roadmap)
+4. [🤝 Contributing](#-contributing)
+5. [📄 License](#-license)
+6. [📍 Time Series Bootstrapping Methods intro](#time-series-bootstrapping)
+7. [👏 Contributors](#-contributors)
 
----
 
 
-## 📍 Time Series Bootstrapping
-`tsbootstrap` is a comprehensive project designed to implement an array of bootstrapping techniques specifically tailored for time series data. This project is targeted towards data scientists, statisticians, economists, and other professionals or researchers who regularly work with time series data and require robust methods for generating bootstrapped copies of univariate and multivariate time series data.
+---
 
-### Overview
-Time series bootstrapping is a nuanced resampling method that is applied to time-dependent data. Traditional bootstrapping methods often assume independence between data points, which is an assumption that does not hold true for time series data where a data point is often dependent on previous data points. Time series bootstrapping techniques respect the chronological order and correlations of the data, providing more accurate estimates of uncertainty or variability.
+## 🚀 Getting Started
 
-### Bootstrapping Methodology
-The `tsbootstrap` project offers a diverse set of bootstrapping techniques that can be applied to either the entire input time series (classes prefixed with `Whole`), or after partitioning the data into blocks (classes prefixed with `Block`). These methodologies can be applied directly to the raw input data or to the residuals obtained after fitting one of the five statistical models defined in `time_series_model.py` (classes with `Residual` in their names).
 
-### Block Bootstrap
-Block Bootstrap is a prevalent approach in time series bootstrapping. It involves resampling blocks of consecutive data points, thus respecting the internal structures of the data. There are several techniques under Block Bootstrap, each with its unique approach. `tsbootstrap` provides highly flexible block bootstrapping, allowing the user to specify the block length sampling, block generation, and block resampling strategies. For additional details, refer to `block_length_sampler.py`, `block_generator.py`, and `block_resampler.py`.
+### 🎮 Using tsbootstrap
 
-The Moving Block Bootstrap, Circular Block Bootstrap, Stationary Block Bootstrap, and NonOverlapping Block Bootstrap methods are all variations of the Block Bootstrap that use different methods to sample the data, maintaining various types of dependencies.
+`tsbootstrap` provides a unified, `sklearn`-like interface to all bootstrap methods.
 
-Bartlett's, Blackman's, Hamming's, Hanning's, and Tukey's Bootstrap methods are specific implementations of the Block Bootstrap that use different window shapes to taper the data, reducing the influence of data points far from the center. In `tsbootstrap`, these methods inherit from `MovingBlockBootstrap`, but can easily be modified to inherit from any of the other three base block bootstrapping classes.
+Example using a `MovingBlockBootstrap` - all bootstrap algorithms follow
+the same interface!
 
-Each method comes with its distinct strengths and weaknesses. The choice of method should be based on the characteristics of the data and the specific requirements of the analysis.
+```python
+from tsbootstrap import MovingBlockBootstrap
+import numpy as np
 
-#### (i) Moving Block Bootstrap
-This method is implemented in `MovingBlockBootstrap` and is used for time series data where blocks of data are resampled to maintain the dependency structure within the blocks. It's useful when the data has dependencies that need to be preserved. It's not recommended when the data does not have any significant dependencies.
+# Create custom time series data. While below is for univariate time series, the bootstraps can handle multivariate time series as well.
+n_samples = 10
+X = np.arange(n_samples)
 
-#### (ii) Circular Block Bootstrap
-This method is implemented in `CircularBlockBootstrap` and treats the data as if it is circular (the end of the data is next to the beginning of the data). It's useful when the data is cyclical or seasonal in nature. It's not recommended when the data does not have a cyclical or seasonal component.
+# Instantiate the bootstrap object
+n_bootstraps = 3
+block_length = 3
+rng = 42
+mbb = MovingBlockBootstrap(n_bootstraps=n_bootstraps, rng=rng, block_length=block_length)
+
+# Generate bootstrapped samples
+return_indices = False
+bootstrapped_samples = mbb.bootstrap(
+    X, return_indices=return_indices)
+
+# Collect bootstrap samples
+X_bootstrapped = []
+for data in bootstrapped_samples:
+    X_bootstrapped.append(data)
 
-#### (iii) Stationary Block Bootstrap
-This method is implemented in `StationaryBlockBootstrap` and randomly resamples blocks of data with block lengths that follow a geometric distribution. It's useful for time series data where the degree of dependency needs to be preserved, and it doesn't require strict stationarity of the underlying process. It's not recommended when the data has strong seasonality or trend components which violate the weak dependence assumption.
+X_bootstrapped = np.array(X_bootstrapped)
+```
 
-#### (iv) NonOverlapping Block Bootstrap
- This method is implemented in `NonOverlappingBlockBootstrap` and resamples blocks of data without overlap. It's useful when the data has dependencies that need to be preserved and when overfitting is a concern. It's not recommended when the data does not have any significant dependencies or when the introduction of bias due to non-overlapping selection is a concern.
+### 📦 Installation and Setup
 
-#### (v) Bartlett's Bootstrap
- Bartlett's method is a time series bootstrap method that uses a window or filter that tapers off as you move away from the center of the window. It's useful when you have a large amount of data and you want to reduce the influence of the data points far away from the center. This method is not advised when the tapering of data points is not desired or when the dataset is small as the tapered data points might contain valuable information. It is implemented in `BartlettsBootstrap`.
+``tsbootstrap`` is installed via ``pip``, either from PyPI or locally.
 
-#### (vi) Blackman Bootstrap
-Similar to Bartlett's method, Blackman's method uses a window that tapers off as you move away from the center of the window. The key difference is the shape of the window (Blackman window has a different shape than Bartlett). It's useful when you want to reduce the influence of the data points far from the center with a different window shape. It's not recommended when the dataset is small or tapering of data points is not desired. It is implemented in `BlackmanBootstrap`.
+#### ✔️ Prerequisites
 
-#### (vii) Hamming Bootstrap
- Similar to the Bartlett and Blackman methods, the Hamming method uses a specific type of window function. It's useful when you want to reduce the influence of the data points far from the center with the Hamming window shape. It's not recommended for small datasets or when tapering of data points is not desired. It is implemented in `HammingBootstrap`.
+- Python (3.8 or higher)
+- `pip` (latest version recommended), plus suitable environment manager (`venv`, `conda`)
 
-#### (viii) Hanning Bootstrap
-This method also uses a specific type of window function. It's useful when you want to reduce the influence of the data points far from the center with the Hanning window shape. It's not recommended for small datasets or when tapering of data points is not desired. It is implemented in `HanningBootstrap`.
+You can also consider using ``uv`` to speed up environment setu.
 
-#### (ix) Tukey Bootstrap
-Similar to the Bartlett, Blackman, Hamming, and Hanning methods, the Tukey method uses a specific type of window function. It's useful when you want to reduce the influence of the data points far from the center with the Tukey window shape. It's not recommended for small datasets or when tapering of data points is not desired. It is implemented in `TukeyBootstrap`.
+#### Installing from PyPI
 
-### Residual Bootstrap
-Residual Bootstrap is a method designed for time series data where a model is fit to the data, and the residuals (the difference between the observed and predicted data) are bootstrapped. It's particularly useful when a good model fit is available for the data. However, it's not recommended when a model fit is not available or is poor. `tsbootstrap` provides four time series models to fit to the input data -- `AutoReg`, `ARIMA`, `SARIMA`, and `VAR` (for multivariate input time series data). For more details, refer to `time_series_model.py` and `tsfit.py`.
+To install the latest release of `tsbootstrap` directly from PyPI, run:
 
-### Statistic-Preserving Bootstrap
-Statistic-Preserving Bootstrap is a unique method designed to generate bootstrapped time series data while preserving a specific statistic of the original data. This method can be beneficial in scenarios where it's important to maintain the original data's characteristics in the bootstrapped samples. It is implemented in `StatisticPreservingBootstrap`.
+```sh
+pip install tsbootstrap
+```
 
-### Distribution Bootstrap
-Distribution Bootstrap generates bootstrapped samples by fitting a distribution to the residuals and then generating new residuals from the fitted distribution. The new residuals are then added to the fitted values to create the bootstrapped samples. This method is based on the assumption that the residuals follow a specific distribution (like Gaussian, Poisson, etc). It's not recommended when the distribution of residuals is unknown or hard to determine. It is implemented in `DistributionBootstrap`.
+To install with all optional dependencies:
 
-### Markov Bootstrap
-Markov Bootstrap is used for bootstrapping time series data where the residuals of the data are presumed to follow a Markov process. This method is especially useful in scenarios where the current residual primarily depends on the previous one, with little to no dependency on residuals from further in the past. Markov Bootstrap technique is designed to preserve this dependency structure in the bootstrapped samples, making it particularly valuable for time series data that exhibits Markov properties. However, it's not advisable when the residuals of the time series data exhibit long-range dependencies, as the Markov assumption of limited dependency may not hold true. It is implemented in `MarkovBootstrap`. See `markov_sampler.py` for implementation details.
+```
+pip install "tsbootstrap[all_extras]"
+```
+---
 
-### Sieve Bootstrap
-Sieve Bootstrap is designed for handling dependent data, where the residuals of the time series data follow an autoregressive process. This method aims to preserve and simulate the dependencies inherent in the original data within the bootstrapped samples. It operates by approximating the autoregressive process ofthe residuals using a finite order autoregressive model. The order of the model is determined based on the data, and the residuals are then bootstrapped. The Sieve Bootstrap technique is particularly valuable for time series data that exhibits autoregressive properties. However, it's not advisable when the residuals of the time series data do not follow an autoregressive process. It is implemented in `SieveBootstrap`. See `time_series_simulator.py` for implementations details.
+Bootstrap algorithms manage their own dependencies - if an extra is needed but not
+present, the object will raise this at construction.
 
 ## 🧩 Modules
 The `tsbootstrap` package contains various modules that handle tasks such as bootstrapping, time series simulation, and utility functions. This modular approach ensures flexibility, extensibility, and ease of maintenance.
 
 
 <details closed><summary>root</summary>
 
 | File                                                                                       | Summary                   |
 | ---                                                                                        | ---                       |
 | [setup.sh](https://github.com/astrogilda/tsbootstrap/blob/main/setup.sh)                         | Shell script for initial setup and environment configuration. |
 | [commitlint.config.js](https://github.com/astrogilda/tsbootstrap/blob/main/commitlint.config.js) | Configuration for enforcing conventional commit messages. |
 | [CITATION.cff](https://github.com/astrogilda/tsbootstrap/blob/main/CITATION.cff)                 | Citation metadata for the project. |
 | [CODE_OF_CONDUCT.md](https://github.com/astrogilda/tsbootstrap/blob/main/CODE_OF_CONDUCT.md)                 | Guidelines for community conduct and interactions. |
-| [CONTRIBUTING.md](https://github.com/astrogilda/tsbootstrap/blob/main/CITATION.md)                 | Instructions for contributing to the project. |
+| [CONTRIBUTING.md](https://github.com/astrogilda/tsbootstrap/blob/main/CONTRIBUTING.md)                 | Instructions for contributing to the project. |
 | [.codeclimate.yml](https://github.com/astrogilda/tsbootstrap/blob/main/.codeclimate.yml)                 | Configuration for Code Climate quality checks. |
 | [.gitignore](https://github.com/astrogilda/tsbootstrap/blob/main/.gitignore)                 | Specifies files and folders to be ignored by Git. |
 | [.pre-commit-config.yaml](https://github.com/astrogilda/tsbootstrap/blob/main/.pre-commit-config.yaml)                 | Configuration for pre-commit hooks. |
 | [poetry.toml](https://github.com/astrogilda/tsbootstrap/blob/main/poetry.toml)                 | Configuration file for Poetry package management. |
 | [tsbootstrap_logo.png](https://github.com/astrogilda/tsbootstrap/blob/main/tsbootstrap_logo.png)                 | Project logo image. |
 
 </details>
@@ -179,116 +169,76 @@
 | ---                                                                                                | ---                       |
 | [types.py](https://github.com/astrogilda/tsbootstrap/blob/main/src/tsbootstrap/utils/types.py)                 | Defines custom types used across the project. |
 | [validate.py](https://github.com/astrogilda/tsbootstrap/blob/main/src/tsbootstrap/utils/validate.py)           | Contains validation utilities. |
 | [odds_and_ends.py](https://github.com/astrogilda/tsbootstrap/blob/main/src/tsbootstrap/utils/odds_and_ends.py) | Contains miscellaneous utility functions. |
 
 </details>
 
----
 
-## 🚀 Getting Started
+## 🗺 Roadmap
 
-### ✔️ Prerequisites
+This is an abridged version; for the complete and evolving list of plans and improvements, see [Issue #144](https://github.com/astrogilda/tsbootstrap/issues/144).
 
-Before you begin, ensure that you have the following prerequisites installed:
-> - `ℹ️ Requirement 1`
-> - `ℹ️ Requirement 2`
-> - `ℹ️ ...`
+### Performance and Scaling
+ -handling large datasets, distributed backend integration (`Dask`, `Spark`, `Ray`), profiling/optimization
+### Tuning and AutoML
+ -adaptive block length, adaptive resampling, evaluation based parameter selection
+### Real-time and Stream Data
+ -stream bootstraps, data update interface
+### Stage 2 `sktime` Integration
+ -evaluation module, datasets, benchmarks, sktime forecasters in bootstraps
+### API and Capability Extension
+ -panel/hierarchical data, exogenous data, update/stream, model state management
+### Scope Extension (TBD)
+ -time series augmentation, fully probabilistic models
 
-### 📦 Installation and Setup
+## 🤝 Contributing
 
-This project comes with a `setup.sh` script to ease the setup process. The script will create a new Python virtual environment, install the necessary dependencies, and handle some version-specific installations.
+Contributions are always welcome!
 
-Here are the steps to follow:
+See our [good first issues ](https://github.com/astrogilda/tsbootstrap/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
+for getting started.
 
-1. Ensure that you have Python, Poetry, and Bash installed on your system. If not, you can install them using the links below:
-    - [Python](https://www.python.org/downloads/)
-    - [Poetry](https://python-poetry.org/docs/#installation)
-    - [Bash](https://www.gnu.org/software/bash/)
+Below is a quick start guide to contributing.
 
-2. Clone the tsbootstrap repository:
-```sh
-git clone https://github.com/astrogilda/tsbootstrap
-```
+### Developer setup
 
-3. Change to the project directory:
-```sh
-cd tsbootstrap
-```
+1. Fork the tsbootstrap repository
 
-4. Make the `setup.sh` script executable:
+2. Clone the fork to local:
 ```sh
-chmod +x setup.sh
+git clone https://github.com/astrogilda/tsbootstrap
 ```
 
-5. Run the `setup.sh` script:
-```sh
-./setup.sh
-```
+3. In the local repository root, set up a python environment, e.g., `venv` or `conda`.
 
-The `setup.sh` script sets up a Python environment using Poetry, locks and installs the necessary dependencies, and installs `dtaidistance` if the Python version is 3.9 or lower.
 
-6. Activate the python shell:
-```sh
-poetry shell
+4. Editable install via `pip`, including developer dependencies:
+```
+pip install -e .[dev]
 ```
 
-That's it! You are now set up and ready to go.
-
-### 🎮 Using tsbootstrap
-
-Here's a basic example using the Moving Block Bootstrap method:
-
-```python
-from tsbootstrap import MovingBlockBootstrap, MovingBlockBootstrapConfig
-import numpy as np
-
-np.random.seed(0)
-
-# Create custom time series data
-
-n_samples = 1000
-
-y = np.random.normal(0, 1, n_samples).cumsum()
-
-x1 = np.arange(1, n_samples + 1).reshape(-1, 1)
-x2 = np.random.normal(0, 1, (n_samples, 1))
-exog = np.concatenate([x1, x2], axis=1)
+The editable install ensures that changes to the package are reflected in
+your environment.
 
-# Instantiate the bootstrap object
-mbb_config = MovingBlockBootstrapConfig(
-    n_bootstraps=1000, rng=42, block_length=10
-)
-mbb = MovingBlockBootstrap(config=mbb_config)
+### Verifying the Installation
 
-# Generate the generator for 1000 bootstrapped samples
-bootstrapped_samples = bootstrap.bootstrap(n=1000)
+After installation, you can verify that tsbootstrap has been installed correctly by checking its version or by trying to import it in Python:
 ```
-
-### 🧪 Running Tests
-```sh
-pytest tests/
+python -c "import tsbootstrap; print(tsbootstrap.__version__)"
 ```
 
----
-
-
-## 🗺 Roadmap
-
-> - [ ] `ℹ️  Task 1: in distributionbootstrap, allow mixture of distributions`
-> - [ ] `ℹ️  Task 2: allow fractional block_length`
-> - [ ] `ℹ️  Task 3: enable multi-processing`
-> - [ ] `ℹ️  Task 4: test -- for biascorrectblockbootstrap, see if the statistic on the bootstrapped sample is close to the statistic on the original sample`
+This command should output the version number of tsbootstrap without any errors, indicating that the installation was successful.
 
+That's it! You are now set up and ready to go. You can start using tsbootstrap for your time series bootstrapping needs.
 
-## 🤝 Contributing
+### Contribution workflow
 
 Contributions are always welcome! Please follow these steps:
-1. Fork the project repository. This creates a copy of the project on your account that you can modify without affecting the original project.
-2. Clone the forked repository to your local machine using a Git client like Git or GitHub Desktop.
+
 3. Create a new branch with a descriptive name (e.g., `new-feature-branch` or `bugfix-issue-123`).
 ```sh
 git checkout -b new-feature-branch
 ```
 4. Make changes to the project's codebase.
 5. Commit your changes to your local branch with a clear commit message that explains the changes you've made.
 ```sh
@@ -297,14 +247,33 @@
 6. Push your changes to your forked repository on GitHub using the following command
 ```sh
 git push origin new-feature-branch
 ```
 7. Create a new pull request to the original project repository. In the pull request, describe the changes you've made and why they're necessary.
 The project maintainers will review your changes and provide feedback or merge them into the main branch.
 
+### 🧪 Running Tests
+
+To run all tests, in your developer environment, run:
+
+```sh
+pytest tests/
+```
+
+Individual bootstrap algorithms can be tested as follows:
+
+```python
+from tsbootstrap.utils import check_estimator
+
+check_estimator(my_bootstrap_algo)
+```
+
+### Contribution guide
+
+For more detailed information on how to contribute, please refer to our [CONTRIBUTING.md](https://github.com/astrogilda/tsbootstrap/blob/main/CONTRIBUTING.md)  guide.
 ---
 
 ## 📄 License
 
 This project is licensed under the `ℹ️  MIT` License. See the [LICENSE](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository) file for additional info.
 
 ---
@@ -318,7 +287,71 @@
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+
+
+---
+
+
+## 📍 Time Series Bootstrapping
+`tsbootstrap` is a comprehensive project designed to implement an array of bootstrapping techniques specifically tailored for time series data. This project is targeted towards data scientists, statisticians, economists, and other professionals or researchers who regularly work with time series data and require robust methods for generating bootstrapped copies of univariate and multivariate time series data.
+
+### Overview
+Time series bootstrapping is a nuanced resampling method that is applied to time-dependent data. Traditional bootstrapping methods often assume independence between data points, which is an assumption that does not hold true for time series data where a data point is often dependent on previous data points. Time series bootstrapping techniques respect the chronological order and correlations of the data, providing more accurate estimates of uncertainty or variability.
+
+### Bootstrapping Methodology
+The `tsbootstrap` project offers a diverse set of bootstrapping techniques that can be applied to either the entire input time series (classes prefixed with `Whole`), or after partitioning the data into blocks (classes prefixed with `Block`). These methodologies can be applied directly to the raw input data or to the residuals obtained after fitting one of the five statistical models defined in `time_series_model.py` (classes with `Residual` in their names).
+
+### Block Bootstrap
+Block Bootstrap is a prevalent approach in time series bootstrapping. It involves resampling blocks of consecutive data points, thus respecting the internal structures of the data. There are several techniques under Block Bootstrap, each with its unique approach. `tsbootstrap` provides highly flexible block bootstrapping, allowing the user to specify the block length sampling, block generation, and block resampling strategies. For additional details, refer to `block_length_sampler.py`, `block_generator.py`, and `block_resampler.py`.
+
+The Moving Block Bootstrap, Circular Block Bootstrap, Stationary Block Bootstrap, and NonOverlapping Block Bootstrap methods are all variations of the Block Bootstrap that use different methods to sample the data, maintaining various types of dependencies.
+
+Bartlett's, Blackman's, Hamming's, Hanning's, and Tukey's Bootstrap methods are specific implementations of the Block Bootstrap that use different window shapes to taper the data, reducing the influence of data points far from the center. In `tsbootstrap`, these methods inherit from `MovingBlockBootstrap`, but can easily be modified to inherit from any of the other three base block bootstrapping classes.
+
+Each method comes with its distinct strengths and weaknesses. The choice of method should be based on the characteristics of the data and the specific requirements of the analysis.
+
+#### (i) Moving Block Bootstrap
+This method is implemented in `MovingBlockBootstrap` and is used for time series data where blocks of data are resampled to maintain the dependency structure within the blocks. It's useful when the data has dependencies that need to be preserved. It's not recommended when the data does not have any significant dependencies.
+
+#### (ii) Circular Block Bootstrap
+This method is implemented in `CircularBlockBootstrap` and treats the data as if it is circular (the end of the data is next to the beginning of the data). It's useful when the data is cyclical or seasonal in nature. It's not recommended when the data does not have a cyclical or seasonal component.
+
+#### (iii) Stationary Block Bootstrap
+This method is implemented in `StationaryBlockBootstrap` and randomly resamples blocks of data with block lengths that follow a geometric distribution. It's useful for time series data where the degree of dependency needs to be preserved, and it doesn't require strict stationarity of the underlying process. It's not recommended when the data has strong seasonality or trend components which violate the weak dependence assumption.
+
+#### (iv) NonOverlapping Block Bootstrap
+ This method is implemented in `NonOverlappingBlockBootstrap` and resamples blocks of data without overlap. It's useful when the data has dependencies that need to be preserved and when overfitting is a concern. It's not recommended when the data does not have any significant dependencies or when the introduction of bias due to non-overlapping selection is a concern.
+
+#### (v) Bartlett's Bootstrap
+ Bartlett's method is a time series bootstrap method that uses a window or filter that tapers off as you move away from the center of the window. It's useful when you have a large amount of data and you want to reduce the influence of the data points far away from the center. This method is not advised when the tapering of data points is not desired or when the dataset is small as the tapered data points might contain valuable information. It is implemented in `BartlettsBootstrap`.
+
+#### (vi) Blackman Bootstrap
+Similar to Bartlett's method, Blackman's method uses a window that tapers off as you move away from the center of the window. The key difference is the shape of the window (Blackman window has a different shape than Bartlett). It's useful when you want to reduce the influence of the data points far from the center with a different window shape. It's not recommended when the dataset is small or tapering of data points is not desired. It is implemented in `BlackmanBootstrap`.
+
+#### (vii) Hamming Bootstrap
+ Similar to the Bartlett and Blackman methods, the Hamming method uses a specific type of window function. It's useful when you want to reduce the influence of the data points far from the center with the Hamming window shape. It's not recommended for small datasets or when tapering of data points is not desired. It is implemented in `HammingBootstrap`.
+
+#### (viii) Hanning Bootstrap
+This method also uses a specific type of window function. It's useful when you want to reduce the influence of the data points far from the center with the Hanning window shape. It's not recommended for small datasets or when tapering of data points is not desired. It is implemented in `HanningBootstrap`.
+
+#### (ix) Tukey Bootstrap
+Similar to the Bartlett, Blackman, Hamming, and Hanning methods, the Tukey method uses a specific type of window function. It's useful when you want to reduce the influence of the data points far from the center with the Tukey window shape. It's not recommended for small datasets or when tapering of data points is not desired. It is implemented in `TukeyBootstrap`.
+
+### Residual Bootstrap
+Residual Bootstrap is a method designed for time series data where a model is fit to the data, and the residuals (the difference between the observed and predicted data) are bootstrapped. It's particularly useful when a good model fit is available for the data. However, it's not recommended when a model fit is not available or is poor. `tsbootstrap` provides four time series models to fit to the input data -- `AutoReg`, `ARIMA`, `SARIMA`, and `VAR` (for multivariate input time series data). For more details, refer to `time_series_model.py` and `tsfit.py`.
+
+### Statistic-Preserving Bootstrap
+Statistic-Preserving Bootstrap is a unique method designed to generate bootstrapped time series data while preserving a specific statistic of the original data. This method can be beneficial in scenarios where it's important to maintain the original data's characteristics in the bootstrapped samples. It is implemented in `StatisticPreservingBootstrap`.
+
+### Distribution Bootstrap
+Distribution Bootstrap generates bootstrapped samples by fitting a distribution to the residuals and then generating new residuals from the fitted distribution. The new residuals are then added to the fitted values to create the bootstrapped samples. This method is based on the assumption that the residuals follow a specific distribution (like Gaussian, Poisson, etc). It's not recommended when the distribution of residuals is unknown or hard to determine. It is implemented in `DistributionBootstrap`.
+
+### Markov Bootstrap
+Markov Bootstrap is used for bootstrapping time series data where the residuals of the data are presumed to follow a Markov process. This method is especially useful in scenarios where the current residual primarily depends on the previous one, with little to no dependency on residuals from further in the past. Markov Bootstrap technique is designed to preserve this dependency structure in the bootstrapped samples, making it particularly valuable for time series data that exhibits Markov properties. However, it's not advisable when the residuals of the time series data exhibit long-range dependencies, as the Markov assumption of limited dependency may not hold true. It is implemented in `MarkovBootstrap`. See `markov_sampler.py` for implementation details.
+
+### Sieve Bootstrap
+Sieve Bootstrap is designed for handling dependent data, where the residuals of the time series data follow an autoregressive process. This method aims to preserve and simulate the dependencies inherent in the original data within the bootstrapped samples. It operates by approximating the autoregressive process ofthe residuals using a finite order autoregressive model. The order of the model is determined based on the data, and the residuals are then bootstrapped. The Sieve Bootstrap technique is particularly valuable for time series data that exhibits autoregressive properties. However, it's not advisable when the residuals of the time series data do not follow an autoregressive process. It is implemented in `SieveBootstrap`. See `time_series_simulator.py` for implementations details.
```

#### html2text {}

```diff
@@ -4,73 +4,194 @@
       ******** GGeenneerraattee bboooottssttrraappppeedd ssaammpplleess ffrroomm ttiimmee--sseerriieess ddaattaa.. TThhee ffuullll
                      ddooccuummeennttaattiioonn iiss aavvaaiillaabbllee _hh_ee_rr_ee.. ********
 
                       [Markdown][Python][pytest][actions]
         _[_p_y_p_i_-_v_e_r_s_i_o_n_]_[_p_y_p_i_-_p_y_t_h_o_n_-_v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_][github-license]
 [Build Status]_[_c_o_d_e_c_o_v_]_[_D_O_I_]_[_C_o_d_e_ _Q_u_a_l_i_t_y_][Last Commit][Issues][Pull Requests]
 [Tag]
-## ð Table of Contents 1. [ð Time Series Bootstrapping](#time-series-
-bootstrapping) - [Overview](#overview) - [Bootstrapping Methodology]
-(#bootstrapping-methodology) - [Block Bootstrap](#block-bootstrap) - [Moving
-Block Bootstrap](#moving-block-bootstrap) - [Circular Block Bootstrap]
-(#circular-block-bootstrap) - [Stationary Block Bootstrap](#stationary-block-
-bootstrap) - [NonOverlapping Block Bootstrap](#nonoverlapping-block-bootstrap)
-- [Bartletts Bootstrap](#bartletts-bootstrap) - [Blackman Bootstrap](#blackman-
-bootstrap) - [Hamming Bootstrap](#hamming-bootstrap) - [Hanning Bootstrap]
-(#hanning-bootstrap) - [Tukey Bootstrap](#tukey-bootstrap) - [Residual
-Bootstrap](#residual-bootstrap) - [Bias Corrected Bootstrap](#bias-corrected-
-bootstrap) - [Distribution Bootstrap](#distribution-bootstrap) - [Markov
-Bootstrap](#markov-bootstrap) - [Sieve Bootstrap](#sieve-bootstrap) 3. [ð§©
-Modules](#-modules) 4. [ð Getting Started](#-getting-started) 5. [ðº
-Roadmap](#-roadmap) 6. [ð¤ Contributing](#-contributing) 7. [ð License](#-
-license) 8. [ð Acknowledgments](#-acknowledgments) --- ## ð Time Series
-Bootstrapping `tsbootstrap` is a comprehensive project designed to implement an
-array of bootstrapping techniques specifically tailored for time series data.
-This project is targeted towards data scientists, statisticians, economists,
-and other professionals or researchers who regularly work with time series data
-and require robust methods for generating bootstrapped copies of univariate and
-multivariate time series data. ### Overview Time series bootstrapping is a
-nuanced resampling method that is applied to time-dependent data. Traditional
-bootstrapping methods often assume independence between data points, which is
-an assumption that does not hold true for time series data where a data point
-is often dependent on previous data points. Time series bootstrapping
-techniques respect the chronological order and correlations of the data,
-providing more accurate estimates of uncertainty or variability. ###
-Bootstrapping Methodology The `tsbootstrap` project offers a diverse set of
-bootstrapping techniques that can be applied to either the entire input time
-series (classes prefixed with `Whole`), or after partitioning the data into
-blocks (classes prefixed with `Block`). These methodologies can be applied
-directly to the raw input data or to the residuals obtained after fitting one
-of the five statistical models defined in `time_series_model.py` (classes with
-`Residual` in their names). ### Block Bootstrap Block Bootstrap is a prevalent
-approach in time series bootstrapping. It involves resampling blocks of
-consecutive data points, thus respecting the internal structures of the data.
-There are several techniques under Block Bootstrap, each with its unique
-approach. `tsbootstrap` provides highly flexible block bootstrapping, allowing
-the user to specify the block length sampling, block generation, and block
-resampling strategies. For additional details, refer to
-`block_length_sampler.py`, `block_generator.py`, and `block_resampler.py`. The
-Moving Block Bootstrap, Circular Block Bootstrap, Stationary Block Bootstrap,
-and NonOverlapping Block Bootstrap methods are all variations of the Block
-Bootstrap that use different methods to sample the data, maintaining various
-types of dependencies. Bartlett's, Blackman's, Hamming's, Hanning's, and
-Tukey's Bootstrap methods are specific implementations of the Block Bootstrap
-that use different window shapes to taper the data, reducing the influence of
-data points far from the center. In `tsbootstrap`, these methods inherit from
-`MovingBlockBootstrap`, but can easily be modified to inherit from any of the
-other three base block bootstrapping classes. Each method comes with its
-distinct strengths and weaknesses. The choice of method should be based on the
-characteristics of the data and the specific requirements of the analysis. ####
-(i) Moving Block Bootstrap This method is implemented in `MovingBlockBootstrap`
-and is used for time series data where blocks of data are resampled to maintain
-the dependency structure within the blocks. It's useful when the data has
-dependencies that need to be preserved. It's not recommended when the data does
-not have any significant dependencies. #### (ii) Circular Block Bootstrap This
-method is implemented in `CircularBlockBootstrap` and treats the data as if it
-is circular (the end of the data is next to the beginning of the data). It's
+## ð Table of Contents 1. [ð Getting Started](#-getting-started) 2. [ð§©
+Modules](#-modules) 3. [ðº Roadmap](#-roadmap) 4. [ð¤ Contributing](#-
+contributing) 5. [ð License](#-license) 6. [ð Time Series Bootstrapping
+Methods intro](#time-series-bootstrapping) 7. [ð Contributors](#-
+contributors) --- ## ð Getting Started ### ð® Using tsbootstrap
+`tsbootstrap` provides a unified, `sklearn`-like interface to all bootstrap
+methods. Example using a `MovingBlockBootstrap` - all bootstrap algorithms
+follow the same interface! ```python from tsbootstrap import
+MovingBlockBootstrap import numpy as np # Create custom time series data. While
+below is for univariate time series, the bootstraps can handle multivariate
+time series as well. n_samples = 10 X = np.arange(n_samples) # Instantiate the
+bootstrap object n_bootstraps = 3 block_length = 3 rng = 42 mbb =
+MovingBlockBootstrap(n_bootstraps=n_bootstraps, rng=rng,
+block_length=block_length) # Generate bootstrapped samples return_indices =
+False bootstrapped_samples = mbb.bootstrap( X, return_indices=return_indices) #
+Collect bootstrap samples X_bootstrapped = [] for data in bootstrapped_samples:
+X_bootstrapped.append(data) X_bootstrapped = np.array(X_bootstrapped) ``` ###
+ð¦ Installation and Setup ``tsbootstrap`` is installed via ``pip``, either
+from PyPI or locally. #### âï¸ Prerequisites - Python (3.8 or higher) -
+`pip` (latest version recommended), plus suitable environment manager (`venv`,
+`conda`) You can also consider using ``uv`` to speed up environment setu. ####
+Installing from PyPI To install the latest release of `tsbootstrap` directly
+from PyPI, run: ```sh pip install tsbootstrap ``` To install with all optional
+dependencies: ``` pip install "tsbootstrap[all_extras]" ``` --- Bootstrap
+algorithms manage their own dependencies - if an extra is needed but not
+present, the object will raise this at construction. ## ð§© Modules The
+`tsbootstrap` package contains various modules that handle tasks such as
+bootstrapping, time series simulation, and utility functions. This modular
+approach ensures flexibility, extensibility, and ease of maintenance. root |
+File | Summary | | --- | --- | | [setup.sh](https://github.com/astrogilda/
+tsbootstrap/blob/main/setup.sh) | Shell script for initial setup and
+environment configuration. | | [commitlint.config.js](https://github.com/
+astrogilda/tsbootstrap/blob/main/commitlint.config.js) | Configuration for
+enforcing conventional commit messages. | | [CITATION.cff](https://github.com/
+astrogilda/tsbootstrap/blob/main/CITATION.cff) | Citation metadata for the
+project. | | [CODE_OF_CONDUCT.md](https://github.com/astrogilda/tsbootstrap/
+blob/main/CODE_OF_CONDUCT.md) | Guidelines for community conduct and
+interactions. | | [CONTRIBUTING.md](https://github.com/astrogilda/tsbootstrap/
+blob/main/CONTRIBUTING.md) | Instructions for contributing to the project. | |
+[.codeclimate.yml](https://github.com/astrogilda/tsbootstrap/blob/
+main/.codeclimate.yml) | Configuration for Code Climate quality checks. | |
+[.gitignore](https://github.com/astrogilda/tsbootstrap/blob/main/.gitignore) |
+Specifies files and folders to be ignored by Git. | | [.pre-commit-config.yaml]
+(https://github.com/astrogilda/tsbootstrap/blob/main/.pre-commit-config.yaml) |
+Configuration for pre-commit hooks. | | [poetry.toml](https://github.com/
+astrogilda/tsbootstrap/blob/main/poetry.toml) | Configuration file for Poetry
+package management. | | [tsbootstrap_logo.png](https://github.com/astrogilda/
+tsbootstrap/blob/main/tsbootstrap_logo.png) | Project logo image. | tsbootstrap
+| File | Summary | | --- | --- | | [block_generator.py](https://github.com/
+astrogilda/tsbootstrap/blob/main/src/tsbootstrap/block_generator.py) |
+Generates blocks for bootstrapping. | | [markov_sampler.py](https://github.com/
+astrogilda/tsbootstrap/blob/main/src/tsbootstrap/markov_sampler.py) |
+Implements sampling methods based on Markov models. | | [time_series_model.py]
+(https://github.com/astrogilda/tsbootstrap/blob/main/src/tsbootstrap/
+time_series_model.py) | Defines base and specific time series models. | |
+[block_length_sampler.py](https://github.com/astrogilda/tsbootstrap/blob/main/
+src/tsbootstrap/block_length_sampler.py) | Samples block lengths for block
+bootstrapping methods. | | [base_bootstrap.py](https://github.com/astrogilda/
+tsbootstrap/blob/main/src/tsbootstrap/bootstrap.py) | Contains the
+implementation for different types of base, abstract bootstrapping classes for
+time series data. | | [base_bootstrap_configs.py](https://github.com/
+astrogilda/tsbootstrap/blob/main/src/tsbootstrap/bootstrap_configs.py) |
+Provides configuration classes for different base, abstract bootstrapping
+classes. | | [block_bootstrap.py](https://github.com/astrogilda/tsbootstrap/
+blob/main/src/tsbootstrap/bootstrap.py) | Contains the implementation for
+different types of block bootstrapping methods for time series data. | |
+[block_bootstrap_configs.py](https://github.com/astrogilda/tsbootstrap/blob/
+main/src/tsbootstrap/bootstrap_configs.py) | Provides configuration classes for
+different block bootstrapping methods. | | [bootstrap.py](https://github.com/
+astrogilda/tsbootstrap/blob/main/src/tsbootstrap/bootstrap.py) | Contains the
+implementation for different types of bootstrapping methods for time series
+data, including residual, distribution, markov, statistic-preserving, and
+sieve. | | [time_series_simulator.py](https://github.com/astrogilda/
+tsbootstrap/blob/main/src/tsbootstrap/time_series_simulator.py) | Simulates
+time series data based on various models. | | [block_resampler.py](https://
+github.com/astrogilda/tsbootstrap/blob/main/src/tsbootstrap/block_resampler.py)
+| Implements methods for block resampling in time series. | | [tsfit.py](https:
+//github.com/astrogilda/tsbootstrap/blob/main/src/tsbootstrap/tsfit.py) | Fits
+time series models to data. | | [ranklags.py](https://github.com/astrogilda/
+tsbootstrap/blob/main/src/tsbootstrap/ranklags.py) | Provides functionalities
+to rank lags in a time series. | utils | File | Summary | | --- | --- | |
+[types.py](https://github.com/astrogilda/tsbootstrap/blob/main/src/tsbootstrap/
+utils/types.py) | Defines custom types used across the project. | |
+[validate.py](https://github.com/astrogilda/tsbootstrap/blob/main/src/
+tsbootstrap/utils/validate.py) | Contains validation utilities. | |
+[odds_and_ends.py](https://github.com/astrogilda/tsbootstrap/blob/main/src/
+tsbootstrap/utils/odds_and_ends.py) | Contains miscellaneous utility functions.
+| ## ðº Roadmap This is an abridged version; for the complete and evolving
+list of plans and improvements, see [Issue #144](https://github.com/astrogilda/
+tsbootstrap/issues/144). ### Performance and Scaling -handling large datasets,
+distributed backend integration (`Dask`, `Spark`, `Ray`), profiling/
+optimization ### Tuning and AutoML -adaptive block length, adaptive resampling,
+evaluation based parameter selection ### Real-time and Stream Data -stream
+bootstraps, data update interface ### Stage 2 `sktime` Integration -evaluation
+module, datasets, benchmarks, sktime forecasters in bootstraps ### API and
+Capability Extension -panel/hierarchical data, exogenous data, update/stream,
+model state management ### Scope Extension (TBD) -time series augmentation,
+fully probabilistic models ## ð¤ Contributing Contributions are always
+welcome! See our [good first issues ](https://github.com/astrogilda/
+tsbootstrap/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22) for
+getting started. Below is a quick start guide to contributing. ### Developer
+setup 1. Fork the tsbootstrap repository 2. Clone the fork to local: ```sh git
+clone https://github.com/astrogilda/tsbootstrap ``` 3. In the local repository
+root, set up a python environment, e.g., `venv` or `conda`. 4. Editable install
+via `pip`, including developer dependencies: ``` pip install -e .[dev] ``` The
+editable install ensures that changes to the package are reflected in your
+environment. ### Verifying the Installation After installation, you can verify
+that tsbootstrap has been installed correctly by checking its version or by
+trying to import it in Python: ``` python -c "import tsbootstrap; print
+(tsbootstrap.__version__)" ``` This command should output the version number of
+tsbootstrap without any errors, indicating that the installation was
+successful. That's it! You are now set up and ready to go. You can start using
+tsbootstrap for your time series bootstrapping needs. ### Contribution workflow
+Contributions are always welcome! Please follow these steps: 3. Create a new
+branch with a descriptive name (e.g., `new-feature-branch` or `bugfix-issue-
+123`). ```sh git checkout -b new-feature-branch ``` 4. Make changes to the
+project's codebase. 5. Commit your changes to your local branch with a clear
+commit message that explains the changes you've made. ```sh git commit -
+m 'Implemented new feature.' ``` 6. Push your changes to your forked repository
+on GitHub using the following command ```sh git push origin new-feature-branch
+``` 7. Create a new pull request to the original project repository. In the
+pull request, describe the changes you've made and why they're necessary. The
+project maintainers will review your changes and provide feedback or merge them
+into the main branch. ### ð§ª Running Tests To run all tests, in your
+developer environment, run: ```sh pytest tests/ ``` Individual bootstrap
+algorithms can be tested as follows: ```python from tsbootstrap.utils import
+check_estimator check_estimator(my_bootstrap_algo) ``` ### Contribution guide
+For more detailed information on how to contribute, please refer to our
+[CONTRIBUTING.md](https://github.com/astrogilda/tsbootstrap/blob/main/
+CONTRIBUTING.md) guide. --- ## ð License This project is licensed under the
+`â¹ï¸ MIT` License. See the [LICENSE](https://docs.github.com/en/communities/
+setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-
+repository) file for additional info. --- ## ð Contributors Thanks goes to
+these wonderful people: This project follows the [all-contributors](https://
+github.com/all-contributors/all-contributors) specification. Contributions of
+any kind welcome! --- ## ð Time Series Bootstrapping `tsbootstrap` is a
+comprehensive project designed to implement an array of bootstrapping
+techniques specifically tailored for time series data. This project is targeted
+towards data scientists, statisticians, economists, and other professionals or
+researchers who regularly work with time series data and require robust methods
+for generating bootstrapped copies of univariate and multivariate time series
+data. ### Overview Time series bootstrapping is a nuanced resampling method
+that is applied to time-dependent data. Traditional bootstrapping methods often
+assume independence between data points, which is an assumption that does not
+hold true for time series data where a data point is often dependent on
+previous data points. Time series bootstrapping techniques respect the
+chronological order and correlations of the data, providing more accurate
+estimates of uncertainty or variability. ### Bootstrapping Methodology The
+`tsbootstrap` project offers a diverse set of bootstrapping techniques that can
+be applied to either the entire input time series (classes prefixed with
+`Whole`), or after partitioning the data into blocks (classes prefixed with
+`Block`). These methodologies can be applied directly to the raw input data or
+to the residuals obtained after fitting one of the five statistical models
+defined in `time_series_model.py` (classes with `Residual` in their names). ###
+Block Bootstrap Block Bootstrap is a prevalent approach in time series
+bootstrapping. It involves resampling blocks of consecutive data points, thus
+respecting the internal structures of the data. There are several techniques
+under Block Bootstrap, each with its unique approach. `tsbootstrap` provides
+highly flexible block bootstrapping, allowing the user to specify the block
+length sampling, block generation, and block resampling strategies. For
+additional details, refer to `block_length_sampler.py`, `block_generator.py`,
+and `block_resampler.py`. The Moving Block Bootstrap, Circular Block Bootstrap,
+Stationary Block Bootstrap, and NonOverlapping Block Bootstrap methods are all
+variations of the Block Bootstrap that use different methods to sample the
+data, maintaining various types of dependencies. Bartlett's, Blackman's,
+Hamming's, Hanning's, and Tukey's Bootstrap methods are specific
+implementations of the Block Bootstrap that use different window shapes to
+taper the data, reducing the influence of data points far from the center. In
+`tsbootstrap`, these methods inherit from `MovingBlockBootstrap`, but can
+easily be modified to inherit from any of the other three base block
+bootstrapping classes. Each method comes with its distinct strengths and
+weaknesses. The choice of method should be based on the characteristics of the
+data and the specific requirements of the analysis. #### (i) Moving Block
+Bootstrap This method is implemented in `MovingBlockBootstrap` and is used for
+time series data where blocks of data are resampled to maintain the dependency
+structure within the blocks. It's useful when the data has dependencies that
+need to be preserved. It's not recommended when the data does not have any
+significant dependencies. #### (ii) Circular Block Bootstrap This method is
+implemented in `CircularBlockBootstrap` and treats the data as if it is
+circular (the end of the data is next to the beginning of the data). It's
 useful when the data is cyclical or seasonal in nature. It's not recommended
 when the data does not have a cyclical or seasonal component. #### (iii)
 Stationary Block Bootstrap This method is implemented in
 `StationaryBlockBootstrap` and randomly resamples blocks of data with block
 lengths that follow a geometric distribution. It's useful for time series data
 where the degree of dependency needs to be preserved, and it doesn't require
 strict stationarity of the underlying process. It's not recommended when the
@@ -145,121 +266,8 @@
 data within the bootstrapped samples. It operates by approximating the
 autoregressive process ofthe residuals using a finite order autoregressive
 model. The order of the model is determined based on the data, and the
 residuals are then bootstrapped. The Sieve Bootstrap technique is particularly
 valuable for time series data that exhibits autoregressive properties. However,
 it's not advisable when the residuals of the time series data do not follow an
 autoregressive process. It is implemented in `SieveBootstrap`. See
-`time_series_simulator.py` for implementations details. ## ð§© Modules The
-`tsbootstrap` package contains various modules that handle tasks such as
-bootstrapping, time series simulation, and utility functions. This modular
-approach ensures flexibility, extensibility, and ease of maintenance. root |
-File | Summary | | --- | --- | | [setup.sh](https://github.com/astrogilda/
-tsbootstrap/blob/main/setup.sh) | Shell script for initial setup and
-environment configuration. | | [commitlint.config.js](https://github.com/
-astrogilda/tsbootstrap/blob/main/commitlint.config.js) | Configuration for
-enforcing conventional commit messages. | | [CITATION.cff](https://github.com/
-astrogilda/tsbootstrap/blob/main/CITATION.cff) | Citation metadata for the
-project. | | [CODE_OF_CONDUCT.md](https://github.com/astrogilda/tsbootstrap/
-blob/main/CODE_OF_CONDUCT.md) | Guidelines for community conduct and
-interactions. | | [CONTRIBUTING.md](https://github.com/astrogilda/tsbootstrap/
-blob/main/CITATION.md) | Instructions for contributing to the project. | |
-[.codeclimate.yml](https://github.com/astrogilda/tsbootstrap/blob/
-main/.codeclimate.yml) | Configuration for Code Climate quality checks. | |
-[.gitignore](https://github.com/astrogilda/tsbootstrap/blob/main/.gitignore) |
-Specifies files and folders to be ignored by Git. | | [.pre-commit-config.yaml]
-(https://github.com/astrogilda/tsbootstrap/blob/main/.pre-commit-config.yaml) |
-Configuration for pre-commit hooks. | | [poetry.toml](https://github.com/
-astrogilda/tsbootstrap/blob/main/poetry.toml) | Configuration file for Poetry
-package management. | | [tsbootstrap_logo.png](https://github.com/astrogilda/
-tsbootstrap/blob/main/tsbootstrap_logo.png) | Project logo image. | tsbootstrap
-| File | Summary | | --- | --- | | [block_generator.py](https://github.com/
-astrogilda/tsbootstrap/blob/main/src/tsbootstrap/block_generator.py) |
-Generates blocks for bootstrapping. | | [markov_sampler.py](https://github.com/
-astrogilda/tsbootstrap/blob/main/src/tsbootstrap/markov_sampler.py) |
-Implements sampling methods based on Markov models. | | [time_series_model.py]
-(https://github.com/astrogilda/tsbootstrap/blob/main/src/tsbootstrap/
-time_series_model.py) | Defines base and specific time series models. | |
-[block_length_sampler.py](https://github.com/astrogilda/tsbootstrap/blob/main/
-src/tsbootstrap/block_length_sampler.py) | Samples block lengths for block
-bootstrapping methods. | | [base_bootstrap.py](https://github.com/astrogilda/
-tsbootstrap/blob/main/src/tsbootstrap/bootstrap.py) | Contains the
-implementation for different types of base, abstract bootstrapping classes for
-time series data. | | [base_bootstrap_configs.py](https://github.com/
-astrogilda/tsbootstrap/blob/main/src/tsbootstrap/bootstrap_configs.py) |
-Provides configuration classes for different base, abstract bootstrapping
-classes. | | [block_bootstrap.py](https://github.com/astrogilda/tsbootstrap/
-blob/main/src/tsbootstrap/bootstrap.py) | Contains the implementation for
-different types of block bootstrapping methods for time series data. | |
-[block_bootstrap_configs.py](https://github.com/astrogilda/tsbootstrap/blob/
-main/src/tsbootstrap/bootstrap_configs.py) | Provides configuration classes for
-different block bootstrapping methods. | | [bootstrap.py](https://github.com/
-astrogilda/tsbootstrap/blob/main/src/tsbootstrap/bootstrap.py) | Contains the
-implementation for different types of bootstrapping methods for time series
-data, including residual, distribution, markov, statistic-preserving, and
-sieve. | | [time_series_simulator.py](https://github.com/astrogilda/
-tsbootstrap/blob/main/src/tsbootstrap/time_series_simulator.py) | Simulates
-time series data based on various models. | | [block_resampler.py](https://
-github.com/astrogilda/tsbootstrap/blob/main/src/tsbootstrap/block_resampler.py)
-| Implements methods for block resampling in time series. | | [tsfit.py](https:
-//github.com/astrogilda/tsbootstrap/blob/main/src/tsbootstrap/tsfit.py) | Fits
-time series models to data. | | [ranklags.py](https://github.com/astrogilda/
-tsbootstrap/blob/main/src/tsbootstrap/ranklags.py) | Provides functionalities
-to rank lags in a time series. | utils | File | Summary | | --- | --- | |
-[types.py](https://github.com/astrogilda/tsbootstrap/blob/main/src/tsbootstrap/
-utils/types.py) | Defines custom types used across the project. | |
-[validate.py](https://github.com/astrogilda/tsbootstrap/blob/main/src/
-tsbootstrap/utils/validate.py) | Contains validation utilities. | |
-[odds_and_ends.py](https://github.com/astrogilda/tsbootstrap/blob/main/src/
-tsbootstrap/utils/odds_and_ends.py) | Contains miscellaneous utility functions.
-| --- ## ð Getting Started ### âï¸ Prerequisites Before you begin, ensure
-that you have the following prerequisites installed: > - `â¹ï¸ Requirement 1`
-> - `â¹ï¸ Requirement 2` > - `â¹ï¸ ...` ### ð¦ Installation and Setup
-This project comes with a `setup.sh` script to ease the setup process. The
-script will create a new Python virtual environment, install the necessary
-dependencies, and handle some version-specific installations. Here are the
-steps to follow: 1. Ensure that you have Python, Poetry, and Bash installed on
-your system. If not, you can install them using the links below: - [Python]
-(https://www.python.org/downloads/) - [Poetry](https://python-poetry.org/docs/
-#installation) - [Bash](https://www.gnu.org/software/bash/) 2. Clone the
-tsbootstrap repository: ```sh git clone https://github.com/astrogilda/
-tsbootstrap ``` 3. Change to the project directory: ```sh cd tsbootstrap ``` 4.
-Make the `setup.sh` script executable: ```sh chmod +x setup.sh ``` 5. Run the
-`setup.sh` script: ```sh ./setup.sh ``` The `setup.sh` script sets up a Python
-environment using Poetry, locks and installs the necessary dependencies, and
-installs `dtaidistance` if the Python version is 3.9 or lower. 6. Activate the
-python shell: ```sh poetry shell ``` That's it! You are now set up and ready to
-go. ### ð® Using tsbootstrap Here's a basic example using the Moving Block
-Bootstrap method: ```python from tsbootstrap import MovingBlockBootstrap,
-MovingBlockBootstrapConfig import numpy as np np.random.seed(0) # Create custom
-time series data n_samples = 1000 y = np.random.normal(0, 1, n_samples).cumsum
-() x1 = np.arange(1, n_samples + 1).reshape(-1, 1) x2 = np.random.normal(0, 1,
-(n_samples, 1)) exog = np.concatenate([x1, x2], axis=1) # Instantiate the
-bootstrap object mbb_config = MovingBlockBootstrapConfig( n_bootstraps=1000,
-rng=42, block_length=10 ) mbb = MovingBlockBootstrap(config=mbb_config) #
-Generate the generator for 1000 bootstrapped samples bootstrapped_samples =
-bootstrap.bootstrap(n=1000) ``` ### ð§ª Running Tests ```sh pytest tests/ ```
---- ## ðº Roadmap > - [ ] `â¹ï¸ Task 1: in distributionbootstrap, allow
-mixture of distributions` > - [ ] `â¹ï¸ Task 2: allow fractional
-block_length` > - [ ] `â¹ï¸ Task 3: enable multi-processing` > - [ ] `â¹ï¸
-Task 4: test -- for biascorrectblockbootstrap, see if the statistic on the
-bootstrapped sample is close to the statistic on the original sample` ## ð¤
-Contributing Contributions are always welcome! Please follow these steps: 1.
-Fork the project repository. This creates a copy of the project on your account
-that you can modify without affecting the original project. 2. Clone the forked
-repository to your local machine using a Git client like Git or GitHub Desktop.
-3. Create a new branch with a descriptive name (e.g., `new-feature-branch` or
-`bugfix-issue-123`). ```sh git checkout -b new-feature-branch ``` 4. Make
-changes to the project's codebase. 5. Commit your changes to your local branch
-with a clear commit message that explains the changes you've made. ```sh git
-commit -m 'Implemented new feature.' ``` 6. Push your changes to your forked
-repository on GitHub using the following command ```sh git push origin new-
-feature-branch ``` 7. Create a new pull request to the original project
-repository. In the pull request, describe the changes you've made and why
-they're necessary. The project maintainers will review your changes and provide
-feedback or merge them into the main branch. --- ## ð License This project
-is licensed under the `â¹ï¸ MIT` License. See the [LICENSE](https://
-docs.github.com/en/communities/setting-up-your-project-for-healthy-
-contributions/adding-a-license-to-a-repository) file for additional info. --
-- ## ð Contributors Thanks goes to these wonderful people: This project
-follows the [all-contributors](https://github.com/all-contributors/all-
-contributors) specification. Contributions of any kind welcome!
+`time_series_simulator.py` for implementations details.
```

### Comparing `tsbootstrap-0.1.0/pyproject.toml` & `tsbootstrap-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tsbootstrap"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Python package to generate bootstrapped time series"
 maintainers = [
     { name = "Sankalp Gilda", email = "sankalp.gilda@gmail.com" },
     { name = "Franz Kiraly", email = "franz.kiraly@sktime.net"},
     { name = "Benedikt Heidrich", email = "benedikt.heidrich@sktime.net"},
 ]
 authors = [
@@ -35,87 +35,60 @@
     "scikit-learn>=0.24,<1.5.0",
     "scipy>=1.2,<2.0.0",
     "packaging",
 ]
 
 [project.optional-dependencies]
 
-all_extras = [
+all-extras = [
     "arch>=5.0.0,<6.0.0",
     "hmmlearn>=0.3.0,<0.3.2",
     "pyclustering>=0.10.0,<0.11.0",
     "scikit_learn_extra>=0.3.0,<0.4.0",
     "statsmodels>=0.12.1,<0.15.0",
+    "dtaidistance; python_version < '3.10'",
 ]
 
 docs = [
     "furo",
     "jupyter",
     "myst-parser",
     "nbsphinx>=0.8.6",
     "numpydoc",
     "pydata-sphinx-theme",
     "Sphinx!=7.2.0,<8.0.0",
     "sphinx-rtd-theme>=1.3.0",
-    "sphinx-copybutton",
+    "sphinx-copybutton>=0.5.2",
     "sphinx-design<0.6.0",
     "sphinx-gallery<0.15.0",
     "sphinx-issues<4.0.0",
     "sphinx-version-warning",
-    "tabulate",
+    "tabulate>=0.9.0",
 ]
 
 dev = [
-    "black",
+    "black>=24.3.0",
     "blacken-docs",
     "hypothesis",
     "pre-commit",
     "pytest",
     "pytest-cov",
+    "github-actions",
+    "importlib-metadata",
+    "pip-tools",
+    "pyright",
+    "ruff",
+    "autoflake",
+    "typos",
+    "tox",
+    "tox-gh-actions",
+    "pycobertura",
+    "tomlkit"
 ]
 
-[tool.poetry.dev-dependencies]
-# Add your dev dependencies here, e.g.
-black = "~23.10"
-blacken-docs = "~1.16"
-cython = "~3.0"
-github-actions = "~0.0"
-hypothesis = "~6.88"
-importlib-metadata = "~6.8"
-pip-tools = "~7.3"
-pre-commit = "~3.5"
-pytest = "~7.4"
-pytest-cov = "~4.1"
-pyright = "~1.1"
-ruff = "~0.1"
-typos = "~1.16"
-tox = "~4.11"
-tox-gh-actions = "~3.1"
-pycobertura = "~3.2"
-sphinx = "~7.2"
-sphinx-rtd-theme = "^1.3.0"
-tomlkit = "~0.12"
-
-[tool.poetry.group.dev.dependencies]
-bumpversion = "^0.6.0"
-furo = "^2023.7.26"
-jupyter = "*"
-myst-parser = "*"
-nbsphinx = "~0.8"
-numpydoc = "*"
-pydata-sphinx-theme = "*"
-sphinx = "~7.2"
-sphinx-copybutton = "*"
-sphinx-design = "<0.6.0"
-sphinx-gallery = "<0.15.0"
-sphinx-issues = "<4.0.0"
-sphinx-rtd-theme = "^1.3.0"
-sphinx-version-warning = "*"
-tabulate = "*"
-
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-ra -q"
 testpaths = [
     "tests",
 ]
 
@@ -178,14 +151,18 @@
     "N802",  # Function name should be lowercase; overly strict
     "N803",  # Argument name should be lowercase; overly strict
     "N806",  # Variable in function should be lowercase; overly strict
     "N816",  # Variable in class scope should not be mixedCase; overly strict
     "PGH003",  # Use of "eval"; overly strict
     "SIM115",  # open-file-with-context-handler; overly strict
     "TRY003",  # Avoid specifying messages outside exception class; overly strict, especially for ValueError
+    "UP038", # Use `X | Y` in `isinstance` call instead of `(X, Y)`; overly strict
+    "UP007", # Use `X | Y` for type annotationsRuffUP007; overly strict
+    "UP006", # Use `list` instead of `List` for type annotations; overly strict
+    "UP035", # `typing.List` is deprecated, use `list` instead; overly strict
 ]
 line-length = 79  # Must agree with Black
 
 [tool.ruff.isort]
 order-by-type = true
 relative-imports-order = "closest-to-furthest"
 extra-standard-library = ["typing"]
@@ -208,14 +185,28 @@
     "D100",
     "D101",
     "D102",
     "D103",
     "D104",
     "D105",
     "D106",
+    "D107",
+    "S101",  # use of "assert"
+    "S102",  # use of "exec"
+    "S106",  # possible hardcoded password.
+    "PGH001",  # use of "eval"
+]
+"src/tsbootstrap/tests/*.py" = [
+    "D100",
+    "D101",
+    "D102",
+    "D103",
+    "D104",
+    "D105",
+    "D106",
     "D107",
     "S101",  # use of "assert"
     "S102",  # use of "exec"
     "S106",  # possible hardcoded password.
     "PGH001",  # use of "eval"
 ]
```

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/__init__.py` & `tsbootstrap-0.1.1/src/tsbootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/base_bootstrap.py` & `tsbootstrap-0.1.1/src/tsbootstrap/base_bootstrap.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import inspect
 from collections.abc import Callable
 from numbers import Integral
+from typing import Optional
 
 import numpy as np
 from skbase.base import BaseObject
 
 from tsbootstrap.base_bootstrap_configs import (
     BaseDistributionBootstrapConfig,
     BaseMarkovBootstrapConfig,
@@ -66,15 +67,15 @@
             )
 
     def bootstrap(
         self,
         X: np.ndarray,
         return_indices: bool = False,
         y=None,
-        test_ratio: float = 0.0,
+        test_ratio: Optional[float] = None,  # noqa: UP007
     ):
         """Generate indices to split data into training and test set.
 
         Parameters
         ----------
         X : 2D array-like of shape (n_timepoints, n_features)
             The endogenous time series to bootstrap.
@@ -95,41 +96,69 @@
         X_boot_i : 2D np.ndarray-like of shape (n_timepoints_boot_i, n_features)
             i-th bootstrapped sample of X.
         indices_i : 1D np.nparray of shape (n_timepoints_boot_i,) integer values,
             only returned if return_indices=True.
             Index references for the i-th bootstrapped sample of X.
             Indexed values do are not necessarily identical with bootstrapped values.
         """
-        X = np.asarray(X)
-        if len(X.shape) < 2:
-            X = np.expand_dims(X, 1)
+        X, y = self._check_X_y(X, y)
 
-        self._check_input(X)
-
-        X_train, X_test = time_series_split(X, test_ratio=test_ratio)
-
-        if y is not None:
-            self._check_input(y, enforce_univariate=False)
-            exog_train, _ = time_series_split(y, test_ratio=test_ratio)
+        if test_ratio is not None:
+            X_inner, _ = time_series_split(X, test_ratio=test_ratio)
+            if y is not None:
+                y_inner, _ = time_series_split(y, test_ratio=test_ratio)
+            else:
+                y_inner = None
         else:
-            exog_train = None
+            X_inner = X
+            y_inner = y
 
-        tuple_iter = self._generate_samples(
-            X=X_train, return_indices=return_indices, y=exog_train
+        yield from self._bootstrap(
+            X=X_inner, return_indices=return_indices, y=y_inner
         )
 
-        yield from tuple_iter
+    def _bootstrap(self, X: np.ndarray, return_indices: bool = False, y=None):
+        """Generate indices to split data into training and test set.
+
+        Private method to be implemented by derived classes.
+        Input validation is not required in this method.
+
+        Parameters
+        ----------
+        X : 2D array-like of shape (n_timepoints, n_features)
+            The endogenous time series to bootstrap.
+            Dimension 0 is assumed to be the time dimension, ordered
+        return_indices : bool, default=False
+            If True, a second output is retured, integer locations of
+            index references for the bootstrap sample, in reference to original indices.
+            Indexed values do are not necessarily identical with bootstrapped values.
+        y : array-like of shape (n_timepoints, n_features_exog), default=None
+            Exogenous time series to use in bootstrapping.
+
+        Yields
+        ------
+        X_boot_i : 2D np.ndarray-like of shape (n_timepoints_boot_i, n_features)
+            i-th bootstrapped sample of X.
+        indices_i : 1D np.nparray of shape (n_timepoints_boot_i,) integer values,
+            only returned if return_indices=True.
+            Index references for the i-th bootstrapped sample of X.
+            Indexed values do are not necessarily identical with bootstrapped values.
+        """
+        # default implementation for current classes using config
+        yield from self._generate_samples(
+            X=X, return_indices=return_indices, y=y
+        )
 
     def _generate_samples(
         self,
         X: np.ndarray,
         return_indices: bool = False,
         y=None,
     ):
-        """Generates bootstrapped samples directly.
+        """Generate bootstrapped samples directly.
 
         Parameters
         ----------
         X : array-like of shape (n_samples, n_features)
             The input samples.
 
         Yields
@@ -149,42 +178,103 @@
 
             if return_indices:
                 yield data, indices  # type: ignore
             else:
                 yield data
 
     def _generate_samples_single_bootstrap(self, X: np.ndarray, y=None):
-        """Generates list of bootstrapped indices and samples for a single bootstrap iteration.
+        """Generate list of bootstraps for a single bootstrap iteration."""
+        raise NotImplementedError("abstract method")
+
+    def _check_X_y(self, X, y):
+        """Check X and y inputs, for bootstrap and get_n_bootstraps methods.
+
+        Checks X to be a 2D array-like, and y to be a 2D array-like or None.
+        If X is 1D np.ndarray, it is expanded to 2D via np.expand_dims.
+
+        Parameters
+        ----------
+        X : checked 2D array-like of shape (n_timepoints, n_features)
+            The endogenous time series to bootstrap.
+            Dimension 0 is assumed to be the time dimension, ordered
+        y : checked array-like of shape (n_timepoints, n_features_exog), default=None
+            Exogenous time series to use in bootstrapping.
 
-        Should be implemented in derived classes.
+        Returns
+        -------
+        X : np.ndarray, coerced to 2D array-like of shape (n_timepoints, n_features)
+            The checked endogenous time series.
+        y : np.ndarray or None, identical with y
+            The checked exogenous time series.
+
+        Raises
+        ------
+        ValueError : If the input is not valid.
         """
-        raise NotImplementedError("abstract method")
+        if X is not None:
+            X = np.asarray(X)
+            if len(X.shape) < 2:
+                print(X)
+                X = np.expand_dims(X, 1)
+
+            X = self._check_input(X)
+        if y is not None:
+            y = self._check_input(y, enforce_univariate=False)
+
+        return X, y
 
     def _check_input(self, X, enforce_univariate=True):
-        """Checks if the input is valid."""
+        """Checks if the input is valid.
+
+        Parameters
+        ----------
+        X : list of np.ndarray
+            The input to check.
+        enforce_univariate : bool, default=True
+            Whether to enforce univariate input.
+
+        Returns
+        -------
+        object : The input object if it is valid.
+
+        Raises
+        ------
+        ValueError
+            If the input is not valid.
+        """
         if np.any(np.diff([len(x) for x in X]) != 0):
             raise ValueError("All time series must be of the same length.")
 
         self_can_only_univariate = not self.get_tag("capability:multivariate")
         check_univariate = enforce_univariate and self_can_only_univariate
         if check_univariate and X.shape[1] > 1:
             raise ValueError(
                 f"Unsupported input type: the estimator {type(self)} "
                 "does not support multivariate endogeneous time series (X argument). "
                 "Pass an 1D np.array, or a 2D np.array with a single column."
             )
 
-    def get_n_bootstraps(
-        self,
-        X=None,
-        y=None,
-        groups=None,
-    ) -> Integral:
-        """Returns the number of bootstrapping iterations."""
-        return self.config.n_bootstraps  # type: ignore
+        return X
+
+    def get_n_bootstraps(self, X=None, y=None) -> int:
+        """Returns the number of bootstrap instances produced by the bootstrap.
+
+        Parameters
+        ----------
+        X : 2D array-like of shape (n_timepoints, n_features)
+            The endogenous time series to bootstrap.
+            Dimension 0 is assumed to be the time dimension, ordered
+        y : array-like of shape (n_timepoints, n_features_exog), default=None
+            Exogenous time series to use in bootstrapping.
+
+        Returns
+        -------
+        int : The number of bootstrap instances produced by the bootstrap.
+        """
+        return self.n_bootstraps  # type: ignore
 
 
 class BaseResidualBootstrap(BaseTimeSeriesBootstrap):
     """Base class for residual bootstrap.
 
     Parameters
     ----------
@@ -234,15 +324,15 @@
 
     def __init__(
         self,
         n_bootstraps: Integral = 10,  # type: ignore
         rng=None,
         model_type: ModelTypesWithoutArch = "ar",
         model_params=None,
-        order: OrderTypes = None,
+        order: OrderTypes = None,  # type: ignore
         save_models: bool = False,
     ):
         """
         Initialize self.
 
         Parameters
         ----------
@@ -385,17 +475,17 @@
         method: BlockCompressorTypes = "middle",
         apply_pca_flag: bool = False,
         pca=None,
         n_iter_hmm: Integral = 10,  # type: ignore
         n_fits_hmm: Integral = 1,  # type: ignore
         blocks_as_hidden_states_flag: bool = False,
         n_states: Integral = 2,  # type: ignore
-        model_type="ar",
+        model_type: ModelTypesWithoutArch = "ar",
         model_params=None,
-        order: OrderTypes = None,
+        order: OrderTypes = None,  # type: ignore
         save_models: bool = False,
         rng=None,
         **kwargs,
     ):
         """
         Initialize self.
 
@@ -492,15 +582,15 @@
     __init__ : Initialize the BaseStatisticPreservingBootstrap class.
     _calculate_statistic(X: np.ndarray) -> np.ndarray : Calculate the statistic from the input data.
     """
 
     def __init__(
         self,
         n_bootstraps: Integral = 10,  # type: ignore
-        statistic: Callable = None,
+        statistic: Optional[Callable] = None,  # noqa: UP007
         statistic_axis: Integral = 0,  # type: ignore
         statistic_keepdims: bool = False,
         rng=None,
     ) -> None:
         """
         Initialize the BaseStatisticPreservingBootstrap class.
 
@@ -609,17 +699,17 @@
     """
 
     def __init__(
         self,
         n_bootstraps: Integral = 10,  # type: ignore
         distribution: str = "normal",
         refit: bool = False,
-        model_type="ar",
+        model_type: ModelTypesWithoutArch = "ar",
         model_params=None,
-        order: OrderTypes = None,
+        order: OrderTypes = None,  # type: ignore
         save_models: bool = False,
         rng=None,
         **kwargs,
     ) -> None:
         """
         Initialize the BaseStatisticPreservingBootstrap class.
 
@@ -738,15 +828,15 @@
         rng=None,
         resids_model_type: ModelTypes = "ar",
         resids_order=None,
         save_resids_models: bool = False,
         kwargs_base_sieve=None,
         model_type: ModelTypesWithoutArch = "ar",
         model_params=None,
-        order: OrderTypes = None,
+        order: OrderTypes = None,  # type: ignore
         **kwargs_base_residual,
     ) -> None:
         """
         Initialize the BaseSieveBootstrap class.
 
         Parameters
         ----------
```

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/base_bootstrap_configs.py` & `tsbootstrap-0.1.1/src/tsbootstrap/base_bootstrap_configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
     @property
     def rng(self) -> np.random.Generator:
         """Getter for rng."""
         return self._rng
 
     @rng.setter
-    def rng(self, value: RngTypes) -> None:
+    def rng(self, value: RngTypes) -> None:  # type: ignore
         """Setter for rng. Performs validation on assignment."""
         self._rng = validate_rng(value)
 
     @property
     def n_bootstraps(self) -> Integral:
         """Getter for n_bootstraps."""
         return self._n_bootstraps
@@ -164,15 +164,15 @@
     def model_type(self, value: str) -> None:
         """Setter for model_type. Performs validation on assignment."""
         value = value.lower()
         validate_literal_type(value, ModelTypesWithoutArch)  # type: ignore
         self._model_type = value
 
     @property
-    def order(self) -> OrderTypes:
+    def order(self) -> OrderTypes:  # type: ignore
         """Getter for order."""
         return self._order
 
     @order.setter
     def order(self, value) -> None:
         """Setter for order. Performs validation on assignment."""
         validate_order(value)
@@ -505,15 +505,15 @@
         rng=None,
         resids_model_type: ModelTypes = "ar",
         resids_order=None,
         save_resids_models: bool = False,
         kwargs_base_sieve=None,
         model_type: ModelTypesWithoutArch = "ar",
         model_params=None,
-        order: OrderTypes = None,
+        order: OrderTypes = None,  # type: ignore
         **kwargs_base_residual,
     ) -> None:
         """
         Initialize the BaseSieveBootstrap class.
 
         Parameters
         ----------
@@ -583,15 +583,15 @@
         if value == "var" and self.model_type != "var":
             raise ValueError(
                 "resids_model_type can be 'var' only if model_type is also 'var'."
             )
         self._resids_model_type = value
 
     @property
-    def resids_order(self) -> OrderTypes:
+    def resids_order(self) -> OrderTypes:  # type: ignore
         return self._resids_order
 
     @resids_order.setter
     def resids_order(self, value) -> None:
         """
         Set the order of residuals.
```

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/block_bootstrap.py` & `tsbootstrap-0.1.1/src/tsbootstrap/block_bootstrap.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from collections.abc import Callable
 from numbers import Integral
+from typing import Optional
 
 import numpy as np
 
 from tsbootstrap.base_bootstrap import BaseTimeSeriesBootstrap
 from tsbootstrap.block_bootstrap_configs import (
     BartlettsBootstrapConfig,
     BaseBlockBootstrapConfig,
@@ -60,23 +61,23 @@
     """
 
     _tags = {"bootstrap_type": "block"}
 
     def __init__(
         self,
         n_bootstraps: Integral = 10,  # type: ignore
-        block_length: Integral = None,
-        block_length_distribution: str = None,
+        block_length: Optional[Integral] = None,
+        block_length_distribution: Optional[str] = None,
         wrap_around_flag: bool = False,
         overlap_flag: bool = False,
         combine_generation_and_sampling_flag: bool = False,
         block_weights=None,
-        tapered_weights: Callable = None,
-        overlap_length: Integral = None,
-        min_block_length: Integral = None,
+        tapered_weights: Optional[Callable] = None,
+        overlap_length: Optional[Integral] = None,
+        min_block_length: Optional[Integral] = None,
         rng=None,
     ):
         """
         Block Bootstrap class for time series data.
         """
         self.n_bootstraps = n_bootstraps
         self.block_length = block_length
@@ -108,16 +109,15 @@
             )
 
         super().__init__(n_bootstraps=n_bootstraps, rng=rng)
 
         self.blocks = None
         self.block_resampler = None
 
-    def _check_input(self, X: np.ndarray, enforce_univariate=True) -> None:
-        super()._check_input(X=X, enforce_univariate=enforce_univariate)
+    def _check_input_bb(self, X: np.ndarray, enforce_univariate=True) -> None:
         if self.config.block_length is not None and self.config.block_length > X.shape[0]:  # type: ignore
             raise ValueError(
                 "block_length cannot be greater than the size of the input array X."
             )
 
     def _generate_blocks(self, X: np.ndarray):
         """Generates blocks of indices.
@@ -129,14 +129,15 @@
 
         Returns
         -------
         blocks : list of arrays
             The generated blocks.
 
         """
+        self._check_input_bb(X)
         block_length_sampler = BlockLengthSampler(
             avg_block_length=(
                 self.config.block_length
                 if self.config.block_length is not None
                 else int(np.sqrt(X.shape[0]))
             ),  # type: ignore
             block_length_distribution=self.config.block_length_distribution,
@@ -203,44 +204,25 @@
 
 class BaseBlockBootstrap(BlockBootstrap):
     """
     Base class for block bootstrapping.
 
     Parameters
     ----------
-    n_bootstraps : Integral, default=10
-        The number of bootstrap samples to create.
-    block_length : Integral, default=None
-        The length of the blocks to sample. If None, the block length is automatically set to the square root of the number of observations.
-    block_length_distribution : str, default=None
-        The block length distribution function to use. If None, the block length distribution is not utilized.
-    wrap_around_flag : bool, default=False
-        Whether to wrap around the data when generating blocks.
-    overlap_flag : bool, default=False
-        Whether to allow blocks to overlap.
-    combine_generation_and_sampling_flag : bool, default=False
-        Whether to combine the block generation and sampling steps.
-    block_weights : array-like of shape (n_blocks,), default=None
-        The weights to use when sampling blocks.
-    tapered_weights : callable, default=None
-        The tapered weights to use when sampling blocks.
-    overlap_length : Integral, default=None
-        The length of the overlap between blocks.
-    min_block_length : Integral, default=None
-        The minimum length of the blocks.
-    rng : Integral or np.random.Generator, default=np.random.default_rng()
-        The random number generator or seed used to generate the bootstrap samples.
-    bootstrap_type : str, default=None
+    bootstrap_type : str, default="moving"
         The type of block bootstrap to use.
         Must be one of "nonoverlapping", "moving", "stationary", or "circular".
+    kwargs
+        Additional keyword arguments to pass to the BaseBlockBootstrapConfig class.
+        See the documentation for BaseBlockBootstrapConfig for more information.
     """
 
     def __init__(
         self,
-        bootstrap_type: str = None,
+        bootstrap_type: str = "moving",
         **kwargs,
     ):
         # def __init__(
         #     self,
         #     n_bootstraps: Integral = 10,  # type: ignore
         #     block_length: Integral = None,
         #     block_length_distribution: str = None,
@@ -291,15 +273,15 @@
             # tapered_weights=tapered_weights,
             # overlap_length=overlap_length,
             # min_block_length=min_block_length,
             # rng=rng,
             **kwargs,
         )
 
-        self.bootstrap_instance: BlockBootstrap = None
+        self.bootstrap_instance: Optional[BlockBootstrap] = None
 
         if config.bootstrap_type:
             bcls = BLOCK_BOOTSTRAP_TYPES_DICT[config.bootstrap_type]
             # self_params = self.get_params()
             # if "bootstrap_type" in self_params:
             #    self_params.pop("bootstrap_type")
             # bcls_params = bcls.get_param_names()
@@ -400,23 +382,23 @@
     ----------
     .. [^1^] https://en.wikipedia.org/wiki/Bootstrapping_(statistics)#Moving_block_bootstrap
     """
 
     def __init__(
         self,
         n_bootstraps: Integral = 10,  # type: ignore
-        block_length: Integral = None,
-        block_length_distribution: str = None,
+        block_length: Optional[Integral] = None,
+        block_length_distribution: Optional[str] = None,
         wrap_around_flag: bool = False,
         overlap_flag: bool = False,
         combine_generation_and_sampling_flag: bool = False,
         block_weights=None,
-        tapered_weights: Callable = None,
-        overlap_length: Integral = None,
-        min_block_length: Integral = None,
+        tapered_weights: Optional[Callable] = None,
+        overlap_length: Optional[Integral] = None,
+        min_block_length: Optional[Integral] = None,
         rng=None,
         **kwargs,
     ):
         self.config = MovingBlockBootstrapConfig(
             block_length=block_length,
             block_length_distribution=block_length_distribution,
             wrap_around_flag=wrap_around_flag,
@@ -498,23 +480,23 @@
     ----------
     .. [^1^] https://en.wikipedia.org/wiki/Bootstrapping_(statistics)#Moving_block_bootstrap
     """
 
     def __init__(
         self,
         n_bootstraps: Integral = 10,  # type: ignore
-        block_length: Integral = None,
-        block_length_distribution: str = None,
+        block_length: Optional[Integral] = None,
+        block_length_distribution: Optional[str] = None,
         wrap_around_flag: bool = False,
         overlap_flag: bool = False,
         combine_generation_and_sampling_flag: bool = False,
         block_weights=None,
-        tapered_weights: Callable = None,
-        overlap_length: Integral = None,
-        min_block_length: Integral = None,
+        tapered_weights: Optional[Callable] = None,
+        overlap_length: Optional[Integral] = None,
+        min_block_length: Optional[Integral] = None,
         rng=None,
         **kwargs,
     ):
         self.config = StationaryBlockBootstrapConfig(
             block_length=block_length,
             block_length_distribution=block_length_distribution,
             wrap_around_flag=wrap_around_flag,
@@ -597,23 +579,23 @@
     ----------
     .. [^1^] https://en.wikipedia.org/wiki/Bootstrapping_(statistics)#Moving_block_bootstrap
     """
 
     def __init__(
         self,
         n_bootstraps: Integral = 10,  # type: ignore
-        block_length: Integral = None,
-        block_length_distribution: str = None,
+        block_length: Optional[Integral] = None,
+        block_length_distribution: Optional[str] = None,
         wrap_around_flag: bool = False,
         overlap_flag: bool = False,
         combine_generation_and_sampling_flag: bool = False,
         block_weights=None,
-        tapered_weights: Callable = None,
-        overlap_length: Integral = None,
-        min_block_length: Integral = None,
+        tapered_weights: Optional[Callable] = None,
+        overlap_length: Optional[Integral] = None,
+        min_block_length: Optional[Integral] = None,
         rng=None,
         **kwargs,
     ):
         self.config = CircularBlockBootstrapConfig(
             block_length=block_length,
             block_length_distribution=block_length_distribution,
             wrap_around_flag=wrap_around_flag,
@@ -701,23 +683,23 @@
     ----------
     .. [^1^] https://en.wikipedia.org/wiki/Bootstrapping_(statistics)#Moving_block_bootstrap
     """
 
     def __init__(
         self,
         n_bootstraps: Integral = 10,  # type: ignore
-        block_length: Integral = None,
-        block_length_distribution: str = None,
+        block_length: Optional[Integral] = None,
+        block_length_distribution: Optional[str] = None,
         wrap_around_flag: bool = False,
         overlap_flag: bool = False,
         combine_generation_and_sampling_flag: bool = False,
         block_weights=None,
-        tapered_weights: Callable = None,
-        overlap_length: Integral = None,
-        min_block_length: Integral = None,
+        tapered_weights: Optional[Callable] = None,
+        overlap_length: Optional[Integral] = None,
+        min_block_length: Optional[Integral] = None,
         rng=None,
         **kwargs,
     ):
         super().__init__(
             n_bootstraps=n_bootstraps,
             block_length=block_length,
             block_length_distribution=block_length_distribution,
@@ -745,15 +727,15 @@
         )
 
 
 # Be cautious when using the default windowing functions from numpy, as they drop to 0 at the edges.This could be particularly problematic for smaller block_lengths. In the current implementation, we have clipped the min to 0.1, in block_resampler.py.
 
 
 class BartlettsBootstrap(BaseBlockBootstrap):
-    """Bartlett's Bootstrap class for time series data.
+    r"""Bartlett's Bootstrap class for time series data.
 
     This class is a specialized bootstrapping class that uses
     Bartlett's window for tapered weights.
 
     Parameters
     ----------
     n_bootstraps : Integral, default=10
@@ -776,40 +758,55 @@
         The tapered weights to use when sampling blocks.
     overlap_length : Integral, default=None
         The length of the overlap between blocks.
     min_block_length : Integral, default=None
         The minimum length of the blocks.
     rng : Integral or np.random.Generator, default=np.random.default_rng()
         The random number generator or seed used to generate the bootstrap samples.
+
+    Notes
+    -----
+    The Bartlett window is defined as:
+
+    .. math::
+        w(n) = 1 - \\frac{|n - (N - 1) / 2|}{(N - 1) / 2}
+
+    where :math:`N` is the block length.
+
+    References
+    ----------
+    .. [^1^] https://en.wikipedia.org/wiki/Window_function#Triangular_window
     """
 
     def __init__(
         self,
         n_bootstraps: Integral = 10,  # type: ignore
-        block_length: Integral = None,
-        block_length_distribution: str = None,
+        block_length: Optional[Integral] = None,
+        block_length_distribution: Optional[str] = None,
         wrap_around_flag: bool = False,
         overlap_flag: bool = False,
         combine_generation_and_sampling_flag: bool = False,
         block_weights=None,
-        tapered_weights: Callable = None,
-        overlap_length: Integral = None,
-        min_block_length: Integral = None,
+        tapered_weights: Optional[Callable] = None,
+        overlap_length: Optional[Integral] = None,
+        min_block_length: Optional[Integral] = None,
+        bootstrap_type: str = "moving",
         rng=None,
         **kwargs,
     ):
         self.config = BartlettsBootstrapConfig(
             block_length=block_length,
             block_length_distribution=block_length_distribution,
             wrap_around_flag=wrap_around_flag,
             overlap_flag=overlap_flag,
             combine_generation_and_sampling_flag=combine_generation_and_sampling_flag,
             block_weights=block_weights,
             tapered_weights=tapered_weights,
             overlap_length=overlap_length,
+            bootstrap_type=bootstrap_type,
             min_block_length=min_block_length,
             rng=rng,
         )
 
         super().__init__(
             n_bootstraps=n_bootstraps,
             block_length=block_length,
@@ -817,14 +814,15 @@
             wrap_around_flag=wrap_around_flag,
             overlap_flag=overlap_flag,
             combine_generation_and_sampling_flag=combine_generation_and_sampling_flag,
             block_weights=block_weights,
             tapered_weights=tapered_weights,
             overlap_length=overlap_length,
             min_block_length=min_block_length,
+            bootstrap_type=bootstrap_type,
             rng=rng,
             **kwargs,
         )
 
 
 class HammingBootstrap(BaseBlockBootstrap):
     r"""
@@ -867,56 +865,59 @@
     .. math::
         w(n) = 0.54 - 0.46 \\cos\\left(\\frac{2\\pi n}{N - 1}\\right)
 
     where :math:`N` is the block length.
 
     References
     ----------
-    .. [^1^] https://en.wikipedia.org/wiki/Bootstrapping_(statistics)#Moving_block_bootstrap
+    .. [^1^] https://en.wikipedia.org/wiki/Window_function#Hann_and_Hamming_windows
     """
 
     def __init__(
         self,
         n_bootstraps: Integral = 10,  # type: ignore
-        block_length: Integral = None,
-        block_length_distribution: str = None,
+        block_length: Optional[Integral] = None,
+        block_length_distribution: Optional[str] = None,
         wrap_around_flag: bool = False,
         overlap_flag: bool = False,
         combine_generation_and_sampling_flag: bool = False,
         block_weights=None,
-        tapered_weights: Callable = None,
-        overlap_length: Integral = None,
-        min_block_length: Integral = None,
+        tapered_weights: Optional[Callable] = None,
+        overlap_length: Optional[Integral] = None,
+        min_block_length: Optional[Integral] = None,
+        bootstrap_type: str = "moving",
         rng=None,
         **kwargs,
     ):
         self.config = HammingBootstrapConfig(
             block_length=block_length,
             block_length_distribution=block_length_distribution,
             wrap_around_flag=wrap_around_flag,
             overlap_flag=overlap_flag,
             combine_generation_and_sampling_flag=combine_generation_and_sampling_flag,
             block_weights=block_weights,
             tapered_weights=tapered_weights,
             overlap_length=overlap_length,
             min_block_length=min_block_length,
+            bootstrap_type=bootstrap_type,
             rng=rng,
         )
 
         super().__init__(
             n_bootstraps=n_bootstraps,
             block_length=block_length,
             block_length_distribution=block_length_distribution,
             wrap_around_flag=wrap_around_flag,
             overlap_flag=overlap_flag,
             combine_generation_and_sampling_flag=combine_generation_and_sampling_flag,
             block_weights=block_weights,
             tapered_weights=tapered_weights,
             overlap_length=overlap_length,
             min_block_length=min_block_length,
+            bootstrap_type=bootstrap_type,
             rng=rng,
             **kwargs,
         )
 
 
 class HanningBootstrap(BaseBlockBootstrap):
     r"""
@@ -945,15 +946,15 @@
         The weights to use when sampling blocks.
     tapered_weights : callable, default=None
         The tapered weights to use when sampling blocks.
     overlap_length : Integral, default=None
         The length of the overlap between blocks.
     min_block_length : Integral, default=None
         The minimum length of the blocks.
-    bootstrap_type : str, default=None
+    bootstrap_type : str, default="moving"
         The type of block bootstrap to use.
         Must be one of "nonoverlapping", "moving", "stationary", or "circular".
     rng : Integral or np.random.Generator, default=np.random.default_rng()
         The random number generator or seed used to generate the bootstrap samples.
 
     Notes
     -----
@@ -962,43 +963,44 @@
     .. math::
         w(n) = 0.5 - 0.5 \\cos\\left(\\frac{2\\pi n}{N - 1}\\right)
 
     where :math:`N` is the block length.
 
     References
     ----------
-    .. [^1^] https://en.wikipedia.org/wiki/Bootstrapping_(statistics)#Moving_block_bootstrap
+    .. [^1^] https://en.wikipedia.org/wiki/Window_function#Hann_and_Hamming_windows
     """
 
     def __init__(
         self,
         n_bootstraps: Integral = 10,  # type: ignore
-        block_length: Integral = None,
-        block_length_distribution: str = None,
+        block_length: Optional[Integral] = None,
+        block_length_distribution: Optional[str] = None,
         wrap_around_flag: bool = False,
         overlap_flag: bool = False,
         combine_generation_and_sampling_flag: bool = False,
         block_weights=None,
-        tapered_weights: Callable = None,
-        overlap_length: Integral = None,
-        min_block_length: Integral = None,
-        bootstrap_type: str = None,
+        tapered_weights: Optional[Callable] = None,
+        overlap_length: Optional[Integral] = None,
+        min_block_length: Optional[Integral] = None,
+        bootstrap_type: str = "moving",
         rng=None,
         **kwargs,
     ):
         self.config = HanningBootstrapConfig(
             block_length=block_length,
             block_length_distribution=block_length_distribution,
             wrap_around_flag=wrap_around_flag,
             overlap_flag=overlap_flag,
             combine_generation_and_sampling_flag=combine_generation_and_sampling_flag,
             block_weights=block_weights,
             tapered_weights=tapered_weights,
             overlap_length=overlap_length,
             min_block_length=min_block_length,
+            bootstrap_type=bootstrap_type,
             rng=rng,
         )
 
         super().__init__(
             n_bootstraps=n_bootstraps,
             block_length=block_length,
             block_length_distribution=block_length_distribution,
@@ -1018,133 +1020,197 @@
 class BlackmanBootstrap(BaseBlockBootstrap):
     r"""
     Blackman Bootstrap class for time series data.
 
     This class is a specialized bootstrapping class that uses
     Blackman window for tapered weights.
 
+    Parameters
+    ----------
+    n_bootstraps : Integral, default=10
+        The number of bootstrap samples to create.
+    block_length : Integral, default=None
+        The length of the blocks to sample.
+        If None, the block length is the square root of the number of observations.
+    block_length_distribution : str, default=None
+        The block length distribution function to use.
+        If None, the block length distribution is not utilized.
+    wrap_around_flag : bool, default=False
+        Whether to wrap around the data when generating blocks.
+    overlap_flag : bool, default=False
+        Whether to allow blocks to overlap.
+    combine_generation_and_sampling_flag : bool, default=False
+        Whether to combine the block generation and sampling steps.
+    block_weights : array-like of shape (n_blocks,), default=None
+        The weights to use when sampling blocks.
+    tapered_weights : callable, default=None
+        The tapered weights to use when sampling blocks.
+    overlap_length : Integral, default=None
+        The length of the overlap between blocks.
+    min_block_length : Integral, default=None
+        The minimum length of the blocks.
+    rng : Integral or np.random.Generator, default=np.random.default_rng()
+        The random number generator or seed used to generate the bootstrap samples.
+
     Notes
     -----
     The Blackman window is defined as:
 
     .. math::
         w(n) = 0.42 - 0.5 \\cos\\left(\\frac{2\\pi n}{N - 1}\\right) + 0.08 \\cos\\left(\\frac{4\\pi n}{N - 1}\\right)
 
     where :math:`N` is the block length.
 
     References
     ----------
-    .. [^1^] https://en.wikipedia.org/wiki/Bootstrapping_(statistics)#Moving_block_bootstrap
+    .. [^1^] https://en.wikipedia.org/wiki/Window_function#Blackman_window
     """
 
     def __init__(
         self,
         n_bootstraps: Integral = 10,  # type: ignore
-        block_length: Integral = None,
-        block_length_distribution: str = None,
+        block_length: Optional[Integral] = None,
+        block_length_distribution: Optional[str] = None,
         wrap_around_flag: bool = False,
         overlap_flag: bool = False,
         combine_generation_and_sampling_flag: bool = False,
         block_weights=None,
-        tapered_weights: Callable = None,
-        overlap_length: Integral = None,
-        min_block_length: Integral = None,
+        tapered_weights: Optional[Callable] = None,
+        overlap_length: Optional[Integral] = None,
+        min_block_length: Optional[Integral] = None,
+        bootstrap_type: str = "moving",
         rng=None,
         **kwargs,
     ):
         self.config = BlackmanBootstrapConfig(
             block_length=block_length,
             block_length_distribution=block_length_distribution,
             wrap_around_flag=wrap_around_flag,
             overlap_flag=overlap_flag,
             combine_generation_and_sampling_flag=combine_generation_and_sampling_flag,
             block_weights=block_weights,
             tapered_weights=tapered_weights,
             overlap_length=overlap_length,
             min_block_length=min_block_length,
+            bootstrap_type=bootstrap_type,
             rng=rng,
         )
 
         super().__init__(
             n_bootstraps=n_bootstraps,
             block_length=block_length,
             block_length_distribution=block_length_distribution,
             wrap_around_flag=wrap_around_flag,
             overlap_flag=overlap_flag,
             combine_generation_and_sampling_flag=combine_generation_and_sampling_flag,
             block_weights=block_weights,
             tapered_weights=tapered_weights,
             overlap_length=overlap_length,
             min_block_length=min_block_length,
+            bootstrap_type=bootstrap_type,
             rng=rng,
             **kwargs,
         )
 
 
 class TukeyBootstrap(BaseBlockBootstrap):
     r"""
     Tukey Bootstrap class for time series data.
 
     This class is a specialized bootstrapping class that uses
     Tukey window for tapered weights.
 
+    Parameters
+    ----------
+    n_bootstraps : Integral, default=10
+        The number of bootstrap samples to create.
+    block_length : Integral, default=None
+        The length of the blocks to sample.
+        If None, the block length is the square root of the number of observations.
+    block_length_distribution : str, default=None
+        The block length distribution function to use.
+        If None, the block length distribution is not utilized.
+    wrap_around_flag : bool, default=False
+        Whether to wrap around the data when generating blocks.
+    overlap_flag : bool, default=False
+        Whether to allow blocks to overlap.
+    combine_generation_and_sampling_flag : bool, default=False
+        Whether to combine the block generation and sampling steps.
+    block_weights : array-like of shape (n_blocks,), default=None
+        The weights to use when sampling blocks.
+    tapered_weights : callable, default=None
+        The tapered weights to use when sampling blocks.
+    overlap_length : Integral, default=None
+        The length of the overlap between blocks.
+    min_block_length : Integral, default=None
+        The minimum length of the blocks.
+    rng : Integral or np.random.Generator, default=np.random.default_rng()
+        The random number generator or seed used to generate the bootstrap samples.
+
     Notes
     -----
     The Tukey window is defined as:
 
     .. math::
         w(n) = \\begin{cases}
             0.5\\left[1 + \\cos\\left(\\frac{2\\pi n}{\\alpha(N - 1)}\\right)\\right], & \\text{if } n < \\frac{\\alpha(N - 1)}{2}\\\\
             1, & \\text{if } \\frac{\\alpha(N - 1)}{2} \\leq n \\leq (N - 1)\\left(1 - \\frac{\\alpha}{2}\\right)\\\\
             0.5\\left[1 + \\cos\\left(\\frac{2\\pi n}{\\alpha(N - 1)}\\right)\\right], & \\text{if } n > (N - 1)\\left(1 - \\frac{\\alpha}{2}\\right)
         \\end{cases}
 
     where :math:`N` is the block length and :math:`\\alpha` is the parameter
     controlling the shape of the window.
+
+    References
+    ----------
+    .. [^1^] https://en.wikipedia.org/wiki/Window_function#Tukey_window
     """
 
     def __init__(
         self,
         n_bootstraps: Integral = 10,  # type: ignore
-        block_length: Integral = None,
-        block_length_distribution: str = None,
+        block_length: Optional[Integral] = None,
+        block_length_distribution: Optional[str] = None,
         wrap_around_flag: bool = False,
         overlap_flag: bool = False,
         combine_generation_and_sampling_flag: bool = False,
         block_weights=None,
-        tapered_weights: Callable = None,
-        overlap_length: Integral = None,
-        min_block_length: Integral = None,
+        tapered_weights: Optional[Callable] = None,
+        overlap_length: Optional[Integral] = None,
+        min_block_length: Optional[Integral] = None,
+        bootstrap_type: str = "moving",
         rng=None,
         **kwargs,
     ):
         self.config = TukeyBootstrapConfig(
             block_length=block_length,
             block_length_distribution=block_length_distribution,
             wrap_around_flag=wrap_around_flag,
             overlap_flag=overlap_flag,
             combine_generation_and_sampling_flag=combine_generation_and_sampling_flag,
             block_weights=block_weights,
             tapered_weights=tapered_weights,
             overlap_length=overlap_length,
             min_block_length=min_block_length,
+            bootstrap_type=bootstrap_type,
             rng=rng,
         )
 
         super().__init__(
             n_bootstraps=n_bootstraps,
             block_length=block_length,
             block_length_distribution=block_length_distribution,
             wrap_around_flag=wrap_around_flag,
             overlap_flag=overlap_flag,
             combine_generation_and_sampling_flag=combine_generation_and_sampling_flag,
             block_weights=block_weights,
             tapered_weights=tapered_weights,
             overlap_length=overlap_length,
             min_block_length=min_block_length,
+            bootstrap_type=bootstrap_type,
             rng=rng,
             **kwargs,
         )
 
 
 BLOCK_BOOTSTRAP_TYPES_DICT = {
     "nonoverlapping": NonOverlappingBlockBootstrap,
```

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/block_bootstrap_configs.py` & `tsbootstrap-0.1.1/src/tsbootstrap/block_bootstrap_configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from collections.abc import Callable
 from functools import partial
 from numbers import Integral
+from typing import Optional
 
 import numpy as np
 from scipy.signal.windows import tukey
 
 from tsbootstrap.base_bootstrap_configs import BaseTimeSeriesBootstrapConfig
 from tsbootstrap.utils.validate import validate_single_integer
 
@@ -14,23 +15,23 @@
 class BlockBootstrapConfig(BaseTimeSeriesBootstrapConfig):
     """
     Block Bootstrap base class for time series data.
     """
 
     def __init__(
         self,
-        block_length: Integral = None,
-        block_length_distribution: str = None,
+        block_length: Optional[Integral] = None,
+        block_length_distribution: Optional[str] = None,
         wrap_around_flag: bool = False,
         overlap_flag: bool = False,
         combine_generation_and_sampling_flag: bool = False,
         block_weights=None,
-        tapered_weights: Callable = None,
-        overlap_length: Integral = None,
-        min_block_length: Integral = None,
+        tapered_weights: Optional[Callable] = None,
+        overlap_length: Optional[Integral] = None,
+        min_block_length: Optional[Integral] = None,
         n_bootstraps: Integral = 10,  # type: ignore
         rng=None,
     ) -> None:
         """
         Block Bootstrap class for time series data.
 
         Parameters
@@ -85,15 +86,15 @@
         Setter for block_length. Performs validation on assignment.
 
         Parameters
         ----------
         value : Integral or None.
         """
         if value is not None:
-            validate_single_integer(value, min_value=1)
+            validate_single_integer(value, min_value=1)  # type: ignore
         self._block_length = value
 
     @property
     def block_length_distribution(self) -> str:
         """Getter for block_length_distribution."""
         return self._block_length_distribution
 
@@ -221,15 +222,15 @@
         Setter for overlap_length. Performs validation on assignment.
 
         Parameters
         ----------
         value : Integral or None.
         """
         if value is not None:
-            validate_single_integer(value, min_value=1)
+            validate_single_integer(value, min_value=1)  # type: ignore
         self._overlap_length = value
 
     @property
     def min_block_length(self):
         """Getter for min_block_length."""
         return self._min_block_length
 
@@ -239,38 +240,38 @@
         Setter for min_block_length. Performs validation on assignment.
 
         Parameters
         ----------
         value : Integral or None.
         """
         if value is not None:
-            validate_single_integer(value, min_value=1)
+            validate_single_integer(value, min_value=1)  # type: ignore
         self._min_block_length = value
 
 
 class BaseBlockBootstrapConfig(BlockBootstrapConfig):
     """
     Configuration class for BaseBlockBootstrap.
 
     This class is a specialized configuration class that allows for the
     `bootstrap_type` parameter to be set. The `bootstrap_type` parameter
     determines the type of block bootstrap to use.
     """
 
     def __init__(
         self,
-        bootstrap_type: str = None,
+        bootstrap_type: str = "moving",
         **kwargs,
     ) -> None:
         """
         Initialize self.
 
         Parameters
         ----------
-        bootstrap_type : str, default=None
+        bootstrap_type : str, default="moving"
             The type of block bootstrap to use.
             Must be one of "nonoverlapping", "moving", "stationary", or "circular".
         kwargs
             Additional keyword arguments to pass to the parent BlockBootstrapConfig class.
             See the documentation for BlockBootstrapConfig for more information.
         """
         self.bootstrap_type = bootstrap_type
@@ -299,15 +300,15 @@
     This class is a specialized configuration class that sets
     `wrap_around_flag` to False, `overlap_flag` to True, and
     `block_length_distribution` to None.
     """
 
     def __init__(
         self,
-        block_length: Integral = None,
+        block_length: Optional[Integral] = None,
         **kwargs,
     ) -> None:
         """
         Initialize self.
 
         Parameters
         ----------
@@ -339,15 +340,15 @@
     This class is a specialized configuration class that sets
     `wrap_around_flag` to False, `overlap_flag` to True, and
     `block_length_distribution` to "geometric".
     """
 
     def __init__(
         self,
-        block_length: Integral,
+        block_length: Optional[Integral],
         **kwargs,
     ) -> None:
         """
         Initialize self.
 
         Parameters
         ----------
@@ -379,15 +380,15 @@
     This class is a specialized configuration class that sets
     `wrap_around_flag` to True, `overlap_flag` to True, and
     `block_length_distribution` to None.
     """
 
     def __init__(
         self,
-        block_length: Integral = None,
+        block_length: Optional[Integral] = None,
         **kwargs,
     ) -> None:
         """
         Initialize self.
 
         Parameters
         ----------
@@ -419,15 +420,15 @@
     This class is a specialized configuration class that sets
     `wrap_around_flag` to False, `overlap_flag` to False, and
     `block_length_distribution` to None.
     """
 
     def __init__(
         self,
-        block_length: Integral,
+        block_length: Optional[Integral],
         **kwargs,
     ) -> None:
         """
         Initialize self.
 
         Parameters
         ----------
```

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/block_generator.py` & `tsbootstrap-0.1.1/src/tsbootstrap/block_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+import logging
 import warnings
 from numbers import Integral
 from typing import Optional
 
 import numpy as np
 from numpy.random import Generator
 
 from tsbootstrap.block_length_sampler import BlockLengthSampler
 from tsbootstrap.utils.validate import (
     validate_block_indices,
     validate_integers,
 )
 
+# create logger
+logger = logging.getLogger("tsbootstrap")
+
 
 class BlockGenerator:
     """
     A class that generates blocks of indices.
 
     Methods
     -------
@@ -29,17 +33,17 @@
     """
 
     def __init__(
         self,
         block_length_sampler: BlockLengthSampler,
         input_length: Integral,
         wrap_around_flag: bool = False,
-        rng: Optional[Generator] = None,  # noqa: UP007
-        overlap_length: Optional[Integral] = None,  # noqa: UP007
-        min_block_length: Optional[Integral] = None,  # noqa: UP007
+        rng: Optional[Generator] = None,
+        overlap_length: Optional[Integral] = None,
+        min_block_length: Optional[Integral] = None,
     ):
         """
         Initialize the BlockGenerator with the given parameters.
 
         Parameters
         ----------
         block_length_sampler : BlockLengthSampler
@@ -79,20 +83,20 @@
 
     @property
     def rng(self) -> Generator:
         """The random number generator."""
         return self._rng
 
     @property
-    def overlap_length(self):
+    def overlap_length(self) -> Integral:
         """The length of overlap between consecutive blocks."""
-        return self._overlap_length  # type: ignore
+        return self._overlap_length
 
     @property
-    def min_block_length(self):
+    def min_block_length(self) -> Integral:
         """The minimum length of a block."""
         return self._min_block_length
 
     @input_length.setter
     def input_length(self, value: Integral) -> None:
         """Set the length of the input time series."""
         self._validate_input_length(value)
@@ -108,52 +112,52 @@
     def wrap_around_flag(self, value: bool) -> None:
         """Set the wrap-around flag."""
         if not isinstance(value, bool):
             raise TypeError("'wrap_around_flag' must be a boolean.")
         self._wrap_around_flag = value
 
     @rng.setter
-    def rng(self, value: Generator) -> None:
+    def rng(self, value: Optional[Generator]) -> None:
         """Set the random number generator."""
         if value is None:
             value = np.random.default_rng()
         elif not isinstance(value, Generator):
             raise TypeError(
                 "'rng' must be an instance of the Generator class."
             )
         self._rng = value
 
     @overlap_length.setter
-    def overlap_length(self, value: Integral) -> None:
+    def overlap_length(self, value: Optional[Integral]) -> None:
         """Set the length of overlap between consecutive blocks."""
         self._overlap_length = self._validate_overlap_length(value)
 
     @min_block_length.setter
-    def min_block_length(self, value: Integral) -> None:
+    def min_block_length(self, value: Optional[Integral]) -> None:
         """Set the minimum length of a block."""
         self._min_block_length = self._validate_min_block_length(value)
 
     def _validate_input_length(self, value: Integral) -> None:
         """Private method to validate input length."""
-        validate_integers(value, min_value=3)
+        validate_integers(value, min_value=3)  # type: ignore
 
     def _validate_block_length_sampler(
         self, sampler: BlockLengthSampler
     ) -> None:
         """Private method to validate block length sampler."""
         if not isinstance(sampler, BlockLengthSampler):
             raise TypeError(
                 "The block length sampler must be an instance of the BlockLengthSampler class."
             )
         if sampler.avg_block_length > self.input_length:
             raise ValueError(
                 f"'sampler.avg_block_length' must be less than or equal to 'input_length'. Got 'sampler.avg_block_length' = {sampler.avg_block_length} and 'input_length' = {self.input_length}."
             )
 
-    def _validate_overlap_length(self, value):
+    def _validate_overlap_length(self, value: Optional[Integral]) -> Integral:
         """Private method to validate overlap length.
 
         Parameters
         ----------
         value : Optional[Integral]
             The input overlap length.
 
@@ -165,18 +169,28 @@
         if value is not None:
             validate_integers(value)
             if value < 1:
                 warnings.warn(
                     "'overlap_length' should be >= 1. Setting it to 1.",
                     stacklevel=2,
                 )
-                return 1
+                return 1  # type: ignore
+            if value >= self.input_length:
+                warnings.warn(
+                    f"'overlap_length' should be < 'input_length'. Setting it to {self.input_length - 1}.",
+                    stacklevel=2,
+                )
+                return self.input_length - 1  # type: ignore
+        else:
+            return self.block_length_sampler.avg_block_length // 2  # type: ignore
         return value
 
-    def _validate_min_block_length(self, value):
+    def _validate_min_block_length(
+        self, value: Optional[Integral]
+    ) -> Integral:
         """Private method to validate minimum block length, possibly correcting the value.
 
         Parameters
         ----------
         value : Optional[Integral]
             The input minimum block length.
 
@@ -190,30 +204,30 @@
         if value is not None:
             validate_integers(value)
             if value < MIN_BLOCK_LENGTH:
                 warnings.warn(
                     f"'min_block_length' should be >= {MIN_BLOCK_LENGTH}. Setting it to {MIN_BLOCK_LENGTH}.",
                     stacklevel=2,
                 )
-                value = MIN_BLOCK_LENGTH
+                value = MIN_BLOCK_LENGTH  # type: ignore
 
             if value > self.block_length_sampler.avg_block_length:
                 warnings.warn(
                     f"'min_block_length' should be <= the 'avg_block_length' from 'block_length_sampler'. Setting it to {self.block_length_sampler.avg_block_length}.",
                     stacklevel=2,
                 )
                 value = self.block_length_sampler.avg_block_length
 
-            print(
+            logger.debug(
                 f"min_block_length from blockgenerator, value is not none: {value}\n"
             )
         else:
-            value = MIN_BLOCK_LENGTH
-        print(f"min_block_length from blockgenerator: {value}\n")
-        return value
+            value = MIN_BLOCK_LENGTH  # type: ignore
+        logger.debug(f"min_block_length from blockgenerator: {value}\n")
+        return value  # type: ignore
 
     def _create_block(
         self, start_index: Integral, block_length: Integral
     ) -> np.ndarray:
         """
         Create a block of indices.
 
@@ -291,15 +305,15 @@
 
         Returns
         -------
         Integral
             The total length covered so far.
         """
         # if not self.wrap_around_flag:
-        return block_length - overlap_length
+        return block_length - overlap_length  # type: ignore
         # return 0
 
     def _get_next_block_length(
         self, sampled_block_length: Integral, total_length_covered: Integral
     ) -> Integral:
         """
         Get the next block length after considering wrap-around and total length covered.
@@ -314,15 +328,15 @@
         Returns
         -------
         Integral
             The adjusted block length.
         """
         if not self.wrap_around_flag:
             return min(
-                sampled_block_length, self.input_length - total_length_covered
+                sampled_block_length, self.input_length - total_length_covered  # type: ignore
             )
         return sampled_block_length
 
     def _calculate_next_start_index(
         self,
         start_index: Integral,
         block_length: Integral,
@@ -343,15 +357,15 @@
         Returns
         -------
         Integral
             The start index for the next block.
         """
         next_start_index = start_index + block_length - overlap_length
         next_start_index = next_start_index % self.input_length
-        return next_start_index
+        return next_start_index  # type: ignore
 
     def generate_non_overlapping_blocks(self):
         """
         Generate non-overlapping block indices in the time series.
 
         Returns
         -------
@@ -378,26 +392,26 @@
         ValueError
             If the block length sampler is not set.
         """
         block_indices = []
         start_index = self._calculate_start_index()
         total_length = 0
 
-        while total_length < self.input_length:
+        while total_length < self.input_length:  # type: ignore
             sampled_block_length = (
                 self.block_length_sampler.sample_block_length()
             )
             block_length = self._get_next_block_length(
-                sampled_block_length, total_length
+                sampled_block_length, total_length  # type: ignore
             )
             block = self._create_block(start_index, block_length)
             block_indices.append(block)
             total_length += block_length
             start_index = self._calculate_next_start_index(
-                start_index, block_length, overlap_length=0
+                start_index, block_length, overlap_length=0  # type: ignore
             )
 
         validate_block_indices(block_indices, self.input_length)
         return block_indices
 
     def generate_overlapping_blocks(self):
         """
@@ -439,42 +453,40 @@
         The starting index is then wrapped around if the wrap-around flag is set to True.
         """
         block_indices = []
         start_index = self._calculate_start_index()
         total_length_covered = 0
         start_indices = []
 
-        while total_length_covered < self.input_length:
+        while total_length_covered < self.input_length:  # type: ignore
             start_indices.append(start_index)
             sampled_block_length = (
                 self.block_length_sampler.sample_block_length()
             )
-            print(f"sampled_block_length: {sampled_block_length}\n")
+            logger.debug(f"sampled_block_length: {sampled_block_length}\n")
             block_length = self._get_next_block_length(
-                sampled_block_length, total_length_covered
+                sampled_block_length, total_length_covered  # type: ignore
             )
             if block_length < self.min_block_length:
-                # print(f"block_length: {block_length}, min_block_length: {self.min_block_length}\n")
-                # block_length = self.min_block_length
                 break
             overlap_length = self._calculate_overlap_length(block_length)
 
             block = self._create_block(start_index, block_length)
             block_indices.append(block)
 
             total_length_covered += self._get_total_length_covered(
-                len(block), overlap_length
+                len(block), overlap_length  # type: ignore
             )
             start_index = self._calculate_next_start_index(
                 start_index, block_length, overlap_length
             )
 
             if start_index in start_indices:
                 break
-            print(
+            logger.debug(
                 f"input_length: {self.input_length}, block_length: {block_length}, overlap_length: {overlap_length}, total_length_covered: {total_length_covered}, start_index: {start_index}, block: {block}\n"
             )
 
         validate_block_indices(block_indices, self.input_length)
         return block_indices
 
     def generate_blocks(self, overlap_flag: bool = False):
```

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/block_length_sampler.py` & `tsbootstrap-0.1.1/src/tsbootstrap/block_length_sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,24 +143,24 @@
         """
         validate_integers(value)
         if value < MIN_AVG_BLOCK_LENGTH:
             warnings.warn(
                 f"avg_block_length should be an integer greater than or equal to {MIN_AVG_BLOCK_LENGTH}. Setting to {MIN_AVG_BLOCK_LENGTH}.",
                 stacklevel=3,
             )
-            return MIN_AVG_BLOCK_LENGTH
+            return MIN_AVG_BLOCK_LENGTH  # type: ignore
         return value
 
     @property
     def rng(self) -> Generator:
         """Getter for rng."""
         return self._rng
 
     @rng.setter
-    def rng(self, value: RngTypes) -> None:
+    def rng(self, value: RngTypes) -> None:  # type: ignore
         """
         Setter for rng. Performs validation on assignment.
 
         Parameters
         ----------
         value : int or np.random.Generator
             The random seed for reproducibility. If None, the global random state is used.
```

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/block_resampler.py` & `tsbootstrap-0.1.1/src/tsbootstrap/block_resampler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+import logging
 import warnings
 from collections.abc import Callable
 from numbers import Integral
+from typing import List, Optional, Union
 
 import numpy as np
 from numpy.random import Generator
 
 from tsbootstrap.utils.types import RngTypes
 from tsbootstrap.utils.validate import (
     validate_block_indices,
     validate_rng,
     validate_weights,
 )
 
+logger = logging.getLogger("tsbootstrap")
+
 
 class BlockResampler:
     """
     A class to perform block resampling.
 
     Methods
     -------
@@ -23,19 +27,19 @@
         Resamples blocks and their corresponding tapered_weights with replacement to create a new list of blocks and tapered_weights with total length equal to n.
     resample_block_indices_and_data()
         Generate block indices and corresponding data for the input data array X.
     """
 
     def __init__(
         self,
-        blocks,
+        blocks: List[np.ndarray],
         X: np.ndarray,
-        block_weights=None,
-        tapered_weights: Callable = None,
-        rng: RngTypes = None,
+        block_weights: Optional[Union[Callable, np.ndarray]] = None,
+        tapered_weights: Optional[Union[Callable, np.ndarray]] = None,
+        rng: RngTypes = None,  # type: ignore
     ):
         """
         Initialize the BlockResampler with the selected distribution and average block length.
 
         Parameters
         ----------
         blocks : List[np.ndarray]
@@ -108,16 +112,18 @@
                 )
                 value = value.reshape(-1, 1)
             elif value.ndim > 2:
                 raise ValueError("'X' must be a 1D or 2D numpy array.")
         self._X = value
 
     @property
-    def blocks(self):
-        """A list of numpy arrays where each array represents the indices of a block in the time series."""
+    def blocks(self) -> List[np.ndarray]:
+        """
+        A list of numpy arrays where each array represents the indices of a block in the time series.
+        """
         return self._blocks
 
     @blocks.setter
     def blocks(self, value) -> None:
         """
         Set the list of blocks.
 
@@ -144,15 +150,15 @@
 
     @property
     def rng(self) -> Generator:
         """Generator for reproducibility."""
         return self._rng
 
     @rng.setter
-    def rng(self, value: RngTypes) -> None:
+    def rng(self, value: RngTypes) -> None:  # type: ignore
         """
         Set the random number generator.
 
         Parameters
         ----------
         value : RngTypes
             Generator for reproducibility.
@@ -169,24 +175,30 @@
 
     @property
     def block_weights(self) -> np.ndarray:
         """An array of normalized block_weights."""
         return self._block_weights
 
     @block_weights.setter
-    def block_weights(self, value) -> None:
+    def block_weights(
+        self, value: Optional[Union[Callable, np.ndarray]]
+    ) -> None:
         """
         Set the block_weights array.
 
         Parameters
         ----------
-        value : Union[np.ndarray, Callable]
+        value : Optional[Union[np.ndarray, Callable]]
             An array of weights or a callable function to generate weights.
             If None, then the default uniform weights are used.
 
+        Attributes
+        ----------
+        block_weights : np.ndarray
+            An array of normalized block_weights.
 
         Raises
         ------
         TypeError
             If the block_weights array is not a numpy array or a callable function.
         ValueError
             If the block_weights array is a numpy array but it is empty or if it contains non-integer arrays.
@@ -196,66 +208,50 @@
 
     @property
     def tapered_weights(self):
         """A list of normalized weights."""
         return self._tapered_weights
 
     @tapered_weights.setter
-    def tapered_weights(self, value: Callable) -> None:
+    def tapered_weights(
+        self, value: Optional[Union[Callable, np.ndarray]]
+    ) -> None:
         """
         Set the tapered_weights array.
 
         Parameters
         ----------
         value : Optional[Callable]
             A callable function to generate weights.
             If None, then the default uniform weights are used.
 
+        Attributes
+        ----------
+        tapered_weights : List[np.ndarray]
+            A list of normalized weights.
+
         Raises
         ------
         TypeError
             If the tapered_weights array is not a callable function.
         ValueError
             If the tapered_weights array is a callable function but the output is not a 1D array of length 'size'.
         """
         self._tapered_weights = self._prepare_tapered_weights(value)
 
-    @staticmethod
-    def _normalize_array(array: np.ndarray) -> np.ndarray:
-        """
-        Normalize the weights array.
-
-        Parameters
-        ----------
-        array : np.ndarray
-            n-dimensional array.
-
-        Returns
-        -------
-        np.ndarray
-            An array of normalized values, with the same shape as the input array.
-        """
-        sum_array = np.sum(array, axis=0, keepdims=True)
-        zero_mask = sum_array != 0
-        normalized_array = np.where(
-            zero_mask, array / sum_array, 1.0 / array.shape[0]
-        )
-        return normalized_array
-
-    def _prepare_tapered_weights(self, tapered_weights: Callable = None):
+    def _prepare_tapered_weights(
+        self, tapered_weights: Optional[Union[Callable, np.ndarray]] = None
+    ) -> List[np.ndarray]:
         """
         Prepare the tapered weights array by normalizing it or generating it.
 
         Parameters
         ----------
-        tapered_weights : Union[np.ndarray, Callable]
+        tapered_weights : Optional[Union[Callable, np.ndarray]], optional
             An array of weights or a callable function to generate weights.
-        size : int, optional
-            The size of the weights array (required for "tapered_weights").
-            If None, then the size is the same as the block length.
 
         Returns
         -------
         np.ndarray or List[np.ndarray]
             An array or list of normalized weights.
         """
         block_lengths = np.array([len(block) for block in self.blocks])
@@ -281,85 +277,47 @@
             )
 
         for weights in tapered_weights_arr:
             validate_weights(weights)
 
         return tapered_weights_arr
 
-    def _prepare_block_weights(self, block_weights=None) -> np.ndarray:
-        """
-        Prepare the block_weights array by normalizing it or generating it based on the callable function provided.
-
-        Parameters
-        ----------
-        block_weights : Union[np.ndarray, Callable], optional
-            An array of weights or a callable function to generate weights. Defaults to None.
-
-        Returns
-        -------
-        np.ndarray
-            An array of normalized block_weights.
-        """
-        size = self.X.shape[0]
-
-        if callable(block_weights):
-            block_weights_arr = self._handle_callable_weights(
-                block_weights, size
-            )
-        elif isinstance(block_weights, np.ndarray):
-            block_weights_arr = self._handle_array_block_weights(
-                block_weights, size
-            )
-        elif block_weights is None:
-            block_weights_arr = np.full(size, 1 / size)
-        else:
-            raise TypeError(
-                "'block_weights' must be a numpy array or a callable function or None."
-            )
-
-        # Validate the block_weights array
-        validate_weights(block_weights_arr)
-        # Normalize the block_weights array
-        block_weights_arr = self._normalize_array(block_weights_arr)
-
-        return block_weights_arr
-
     def _handle_callable_weights(
         self,
         weights_func: Callable,
-        size,
-    ) -> np.ndarray:
+        size: Union[Integral, List[Integral], np.ndarray],
+    ) -> Union[np.ndarray, List[np.ndarray]]:
         """
         Handle callable block_weights by executing the function and validating the output.
 
         Parameters
         ----------
-        block_weights : Callable
+        weights_func : Callable
             A callable function to generate block weights.
         size : int
             The size of the block_weights array.
 
         Returns
         -------
-        np.ndarray
-            An array of block_weights.
+        Union[np.ndarray, List[np.ndarray]]
+            An array or list of arrays of weights.
         """
         weights_arr = self._generate_weights_from_callable(weights_func, size)
 
         self._validate_callable_generated_weights(
             weights_arr, size, weights_func.__name__
         )
 
         return weights_arr
 
     def _generate_weights_from_callable(
         self,
         weights_func: Callable,
-        size,
-    ):
+        size: Union[Integral, List[Integral], np.ndarray],
+    ) -> Union[np.ndarray, List[np.ndarray]]:
         """
         Generate weights from a callable function.
 
         Parameters
         ----------
         weights_func : Callable
             A callable function to generate weights.
@@ -369,62 +327,150 @@
         Returns
         -------
         np.ndarray
             An array of weights.
         """
         if isinstance(size, Integral):
             return weights_func(size)
-        elif isinstance(size, (np.ndarray, list)):  # noqa: UP038
+        elif isinstance(size, (np.ndarray, list)):
             return [weights_func(size_iter) for size_iter in size]
         else:
             raise TypeError(
                 "size must be an integer or a list/array of integers"
             )
 
+    def _prepare_block_weights(
+        self, block_weights: Optional[Union[Callable, np.ndarray]] = None
+    ) -> np.ndarray:
+        """
+        Prepare the block_weights array by normalizing it or generating it based on the callable function provided.
+
+        Parameters
+        ----------
+        block_weights : Union[np.ndarray, Callable], optional
+            An array of weights or a callable function to generate weights. Defaults to None.
+
+        Returns
+        -------
+        np.ndarray
+            An array of normalized block_weights.
+        """
+        size = self.X.shape[0]
+
+        if callable(block_weights):
+            block_weights_arr = self._handle_callable_weights(
+                block_weights, size  # type: ignore
+            )
+        elif isinstance(block_weights, np.ndarray):
+            block_weights_arr = self._handle_array_block_weights(
+                block_weights, size
+            )
+        elif block_weights is None:
+            block_weights_arr = np.full(size, 1 / size)
+        else:
+            raise TypeError(
+                "'block_weights' must be a numpy array or a callable function or None."
+            )
+
+        # Validate the block_weights array
+        validate_weights(block_weights_arr)  # type: ignore
+        # Normalize the block_weights array
+        block_weights_arr = self._normalize_array(block_weights_arr)  # type: ignore
+
+        return block_weights_arr
+
+    @staticmethod
+    def _normalize_array(array: np.ndarray) -> np.ndarray:
+        """
+        Normalize the weights array.
+
+        Parameters
+        ----------
+        array : np.ndarray
+            n-dimensional array.
+
+        Returns
+        -------
+        np.ndarray
+            An array of normalized values, with the same shape as the input array.
+        """
+        sum_array = np.sum(array, axis=0, keepdims=True)
+        zero_mask = sum_array != 0
+        normalized_array = np.where(
+            zero_mask, array / sum_array, 1.0 / array.shape[0]
+        )
+        return normalized_array
+
     def _validate_callable_generated_weights(
         self,
-        weights_arr,
-        size,
+        weights_arr: Union[np.ndarray, List[np.ndarray]],
+        size: Union[Integral, List[Integral], np.ndarray],
         callable_name: str,
     ):
         """
         Validate the output of a callable function that generates either block_weights or tapered_weights.
 
         Parameters
         ----------
         weights_arr : Union[np.ndarray, List[np.ndarray]]
             An array or list of arrays of weights.
-        size : Union[Integral, List[Integral]]
+        size : Union[Integral, List[Integral], np.ndarray]
             The size of the weights array.
         callable_name : str
             The name of the callable function.
 
         Raises
         ------
         TypeError
             If the output of the callable function is not a numpy array.
         ValueError
             If the output of the callable function is not a 1d array of length 'size'.
+            If the size and the length of the weights array do not match.
 
         Returns
         -------
         None
         """
         if isinstance(weights_arr, list):
-            print("dealing with tapered_weights")
-            weights_arr = weights_arr[0]
-            size = size[0]
-        if not isinstance(weights_arr, np.ndarray):
+            logger.debug("dealing with tapered_weights")
+            if not isinstance(size, (list, np.ndarray)):
+                raise TypeError(
+                    "size must be a list or np.ndarray when weights_arr is a list."
+                )
+            if len(weights_arr) != len(size):
+                raise ValueError(
+                    f"When `weight_array` is a list of np.ndarrays, and `size` is either a list of ints or an array of ints, they must have the same length. Got {len(weights_arr)} and {len(size)} respectively."
+                )
+            for weights, size_iter in zip(weights_arr, size):
+                if not isinstance(weights, np.ndarray):
+                    raise TypeError(
+                        f"Output of '{callable_name}(size)' must be a numpy array."
+                    )
+                if len(weights) != size_iter or weights.ndim != 1:
+                    raise ValueError(
+                        f"Output of '{callable_name}(size)' must be a 1d array of length 'size'."
+                    )
+        elif isinstance(weights_arr, np.ndarray):
+            logger.debug("dealing with block_weights")
+            if isinstance(size, (list, np.ndarray)):
+                raise TypeError(
+                    "size must be an integer when weights_arr is a np.ndarray."
+                )
+            if not isinstance(size, Integral):
+                raise TypeError(
+                    "size must be an integer when weights_arr is a np.ndarray."
+                )
+            if len(weights_arr) != size or weights_arr.ndim != 1:
+                raise ValueError(
+                    f"Output of '{callable_name}(size)' must be a 1d array of length 'size'."
+                )
+        else:
             raise TypeError(
                 f"Output of '{callable_name}(size)' must be a numpy array."
             )
-        if len(weights_arr) != size or weights_arr.ndim != 1:
-            raise ValueError(
-                f"Output of '{callable_name}(size)' must be a 1d array of length 'size'."
-            )
 
     def _handle_array_block_weights(
         self, block_weights: np.ndarray, size: int
     ) -> np.ndarray:
         """
         Handle array block_weights by validating the array and returning it.
```

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/bootstrap.py` & `tsbootstrap-0.1.1/src/tsbootstrap/bootstrap.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,24 +8,38 @@
 from tsbootstrap.base_bootstrap import (
     BaseDistributionBootstrap,
     BaseMarkovBootstrap,
     BaseResidualBootstrap,
     BaseSieveBootstrap,
     BaseStatisticPreservingBootstrap,
 )
+from tsbootstrap.block_bootstrap import (
+    BlockBootstrap,
+    MovingBlockBootstrap,
+)
 from tsbootstrap.markov_sampler import MarkovSampler
 from tsbootstrap.time_series_simulator import TimeSeriesSimulator
 from tsbootstrap.utils.odds_and_ends import generate_random_indices
+from tsbootstrap.utils.types import (
+    BlockCompressorTypes,
+    ModelTypes,
+    ModelTypesWithoutArch,
+    OrderTypes,
+    RngTypes,
+)
 
 # TODO: add a check if generated block is only one unit long
 # TODO: ensure docstrings align with functionality
 # TODO: test -- check len(returned_indices) == X.shape[0]
 # TODO: ensure x is 2d only for var, otherwise 1d or 2d with 1 feature
 # TODO: block_weights=p with block_length=1 should be equivalent to the iid bootstrap
 # TODO: add test to fit_ar to ensure input lags, if list, are unique
+# TODO: for `StatisticPreservingBootstrap`, see if the statistic on the bootstrapped
+# sample is close to the statistic on the original sample
+# TODO: in `DistributionBootstrap`, allow mixture of distributions
 
 
 # Fit, then resample residuals.
 class WholeResidualBootstrap(BaseResidualBootstrap):
     """
     Whole Residual Bootstrap class for time series data.
 
@@ -38,42 +52,42 @@
     ----------
     n_bootstraps : Integral, default=10
         The number of bootstrap samples to create.
     model_type : str, default="ar"
         The model type to use. Must be one of "ar", "arima", "sarima", "var", or "arch".
     model_params : dict, default=None
         Additional keyword arguments to pass to the TSFit model.
-    order : Integral or list or tuple, default=None
+    order : OrderTypes, default=None
         The order of the model. If None, the best order is chosen via TSFitBestLag.
         If Integral, it is the lag order for AR, ARIMA, and SARIMA,
         and the lag order for ARCH. If list or tuple, the order is a
         tuple of (p, o, q) for ARIMA and (p, d, q, s) for SARIMAX.
         It is either a single Integral or a list of non-consecutive ints for AR,
         and an Integral for VAR and ARCH. If None, the best order is chosen via
         TSFitBestLag. Do note that TSFitBestLag only chooses the best lag,
         not the best order, so for the tuple values, it only chooses the best p,
         not the best (p, o, q) or (p, d, q, s). The rest of the values are set to 0.
     save_models : bool, default=False
         Whether to save the fitted models.
-    rng : Integral or np.random.Generator, default=np.random.default_rng()
+    rng : RngTypes, default=None
         The random number generator or seed used to generate the bootstrap samples.
 
     Methods
     -------
     __init__ : Initialize self.
     _generate_samples_single_bootstrap : Generate a single bootstrap sample.
     """
 
     def __init__(
         self,
         n_bootstraps: Integral = 10,  # type: ignore
-        rng=None,
-        model_type="ar",
-        model_params: Optional[dict] = None,  # noqa: UP007
-        order=None,
+        rng: RngTypes = None,  # type: ignore
+        model_type: ModelTypesWithoutArch = "ar",
+        model_params: Optional[dict] = None,
+        order: OrderTypes = None,  # type: ignore
         save_models: bool = False,
     ):
         self._model_type = model_type
 
         super().__init__(
             n_bootstraps=n_bootstraps,
             rng=rng,
@@ -103,61 +117,63 @@
 
     This class applies residual bootstrapping to blocks of the time series.
     The residuals are bootstrapped using the specified block structure and
     added to the fitted values to generate new samples.
 
     Parameters
     ----------
-    block_bootstrap : BaseBlockBootstrap
+    block_bootstrap : BlockBootstrap, default=MovingBlockBootstrap()
         The block bootstrap algorithm.
     n_bootstraps : Integral, default=10
         The number of bootstrap samples to create.
     model_type : str, default="ar"
         The model type to use. Must be one of "ar", "arima", "sarima", "var", or "arch".
     model_params : dict, default=None
         Additional keyword arguments to pass to the TSFit model.
-    order : Integral or list or tuple, default=None
+    order : OrderTypes, default=None
         The order of the model. If None, the best order is chosen via TSFitBestLag.
         If Integral, it is the lag order for AR, ARIMA, and SARIMA,
         and the lag order for ARCH. If list or tuple, the order is a
         tuple of (p, o, q) for ARIMA and (p, d, q, s) for SARIMAX.
         It is either a single Integral or a list of non-consecutive ints for AR,
         and an Integral for VAR and ARCH. If None, the best order is chosen via
         TSFitBestLag. Do note that TSFitBestLag only chooses the best lag,
         not the best order, so for the tuple values, it only chooses the best p,
         not the best (p, o, q) or (p, d, q, s). The rest of the values are set to 0.
     save_models : bool, default=False
         Whether to save the fitted models.
-    rng : Integral or np.random.Generator, default=np.random.default_rng()
+    rng : RngTypes, default=None
         The random number generator or seed used to generate the bootstrap samples.
 
     Methods
     -------
     __init__ : Initialize self.
     _generate_samples_single_bootstrap : Generate a single bootstrap sample.
     """
 
     def __init__(
         self,
-        block_bootstrap,
         n_bootstraps: Integral = 10,  # type: ignore
-        model_type="ar",
-        model_params=None,
-        order=None,
+        block_bootstrap: Optional[BlockBootstrap] = None,
+        model_type: ModelTypesWithoutArch = "ar",
+        model_params: Optional[dict] = None,
+        order: OrderTypes = None,  # type: ignore
         save_models: bool = False,
-        rng=None,
+        rng: RngTypes = None,  # type: ignore
     ) -> None:
         super().__init__(
             n_bootstraps=n_bootstraps,
             rng=rng,
             model_type=model_type,
             model_params=model_params,
             order=order,
             save_models=save_models,
         )
+        if block_bootstrap is None:
+            block_bootstrap = MovingBlockBootstrap()
         self.block_bootstrap = block_bootstrap
 
     def _generate_samples_single_bootstrap(self, X: np.ndarray, y=None):
         # Fit the model and store residuals, fitted values, etc.
         BaseResidualBootstrap._fit_model(self, X=X, y=y)
 
         # Generate blocks of residuals
@@ -186,54 +202,16 @@
 
     This class applies Markov bootstrapping to the entire time series,
     without any block structure. This is the most basic form of Markov
     bootstrapping. The residuals are fit to a Markov model, and then
     resampled using the Markov model. The resampled residuals are added to
     the fitted values to generate new samples.
 
-    Parameters
-    ----------
-    n_bootstraps : Integral, default=10
-        The number of bootstrap samples to create.
-    method : str, default="middle"
-        The method to use for compressing the blocks.
-        Must be one of "first", "middle", "last", "mean", "mode", "median",
-        "kmeans", "kmedians", "kmedoids".
-    apply_pca_flag : bool, default=False
-        Whether to apply PCA to the residuals before fitting the HMM.
-    pca : PCA, default=None
-        The PCA object to use for applying PCA to the residuals.
-    n_iter_hmm : Integral, default=10
-        Number of iterations for fitting the HMM.
-    n_fits_hmm : Integral, default=1
-        Number of times to fit the HMM.
-    blocks_as_hidden_states_flag : bool, default=False
-        Whether to use blocks as hidden states.
-    n_states : Integral, default=2
-        Number of states for the HMM.
-    model_type : str, default="ar"
-        The model type to use. Must be one of "ar", "arima", "sarima", "var", or "arch".
-    model_params : dict, default=None
-        Additional keyword arguments to pass to the TSFit model.
-    order : Integral or list or tuple, default=None
-        The order of the model. If None, the best order is chosen via TSFitBestLag.
-        If Integral, it is the lag order for AR, ARIMA, and SARIMA, and the lag order
-        for ARCH. If list or tuple, the order is a tuple of (p, o, q) for ARIMA
-        and (p, d, q, s) for SARIMAX. It is either a single Integral or a
-        list of non-consecutive ints for AR, and an Integral for VAR and ARCH.
-        If None, the best order is chosen via TSFitBestLag. Do note that TSFitBestLag
-        only chooses the best lag, not the best order, so for the tuple values,
-        it only chooses the best p, not the best (p, o, q) or (p, d, q, s).
-        The rest of the values are set to 0.
-    rng : Integral or np.random.Generator, default=np.random.default_rng()
-        The random number generator or seed used to generate the bootstrap samples.
-
     Methods
     -------
-    __init__ : Initialize self.
     _generate_samples_single_bootstrap : Generate a single bootstrap sample.
 
     Notes
     -----
     Fitting Markov models is expensive, hence we do not allow re-fititng. We instead fit once to the residuals and generate new samples by changing the random_seed.
     """
 
@@ -278,15 +256,15 @@
     residuals are fit to a Markov model, then resampled using the specified
     block structure. The resampled residuals are added to the fitted values
     to generate new samples. This class is a combination of the
     `BlockResidualBootstrap` and `WholeMarkovBootstrap` classes.
 
     Parameters
     ----------
-    block_bootstrap : BaseBlockBootstrap
+    block_bootstrap : BlockBootstrap, default=MovingBlockBootstrap()
         The block bootstrap algorithm.
     n_bootstraps : Integral, default=10
         The number of bootstrap samples to create.
     method : str, default="middle"
         The method to use for compressing the blocks.
         Must be one of "first", "middle", "last", "mean", "mode", "median",
         "kmeans", "kmedians", "kmedoids".
@@ -329,28 +307,28 @@
     Notes
     -----
     Fitting Markov models is expensive, hence we do not allow re-fititng. We instead fit once to the residuals, resample using blocks once, and generate new samples by changing the random_seed.
     """
 
     def __init__(
         self,
-        block_bootstrap,
         n_bootstraps: Integral = 10,  # type: ignore
-        method="middle",
+        block_bootstrap: Optional[BlockBootstrap] = None,
+        method: BlockCompressorTypes = "middle",
         apply_pca_flag: bool = False,
         pca=None,
         n_iter_hmm: Integral = 10,  # type: ignore
         n_fits_hmm: Integral = 1,  # type: ignore
         blocks_as_hidden_states_flag: bool = False,
         n_states: Integral = 2,  # type: ignore
-        model_type="ar",
-        model_params=None,
+        model_type: ModelTypesWithoutArch = "ar",
+        model_params: Optional[dict] = None,
         order=None,
         save_models: bool = False,
-        rng=None,
+        rng: RngTypes = None,  # type: ignore
     ) -> None:
         super().__init__(
             n_bootstraps=n_bootstraps,
             method=method,
             apply_pca_flag=apply_pca_flag,
             pca=pca,
             n_iter_hmm=n_iter_hmm,
@@ -359,14 +337,16 @@
             n_states=n_states,
             model_type=model_type,
             model_params=model_params,
             order=order,
             save_models=save_models,
             rng=rng,
         )
+        if block_bootstrap is None:
+            block_bootstrap = MovingBlockBootstrap()
         self.block_bootstrap = block_bootstrap
 
     def _generate_samples_single_bootstrap(self, X: np.ndarray, y=None):
         # Fit the model and store residuals, fitted values, etc.
         super()._fit_model(X=X, y=y)
 
         # Generate blocks of residuals
@@ -410,61 +390,55 @@
 
         bs = MovingBlockBootstrap()
         return {"block_bootstrap": bs}
 
 
 class WholeStatisticPreservingBootstrap(BaseStatisticPreservingBootstrap):
     """
-    Whole Bias Corrected Bootstrap class for time series data.
+    Whole Statistic Preserving Bootstrap class for time series data.
 
-    This class applies bias corrected bootstrapping to the entire time series,
-    without any block structure. This is the most basic form of bias corrected
+    This class applies statistic-preserving bootstrapping to the entire time series,
+    without any block structure. This is the most basic form of statistic-preserving
     bootstrapping. The residuals are resampled with replacement and added to
     the fitted values to generate new samples.
 
-    Attributes
-    ----------
-    statistic_X : np.ndarray, default=None
-        The statistic calculated from the original data. This is used as a parameter for generating the bootstrapped samples.
-
     Methods
     -------
-    __init__ : Initialize self.
     _generate_samples_single_bootstrap : Generate a single bootstrap sample.
     """
 
     def _generate_samples_single_bootstrap(self, X: np.ndarray, y=None):
         if self.statistic_X is None:
             self.statistic_X = self._calculate_statistic(X=X)
 
         # Resample residuals
         resampled_indices = generate_random_indices(
-            X.shape[0], self.config.rng
+            X.shape[0], self.config.rng  # type: ignore
         )
         bootstrapped_sample = X[resampled_indices]
         # Calculate the bootstrapped statistic
         statistic_bootstrapped = self._calculate_statistic(bootstrapped_sample)
         # Calculate the bias
         bias = self.statistic_X - statistic_bootstrapped
         # Add the bias to the bootstrapped sample
         bootstrap_sample_bias_corrected = bootstrapped_sample + bias
         return [resampled_indices], [bootstrap_sample_bias_corrected]
 
 
 class BlockStatisticPreservingBootstrap(BaseStatisticPreservingBootstrap):
     """
-    Block Bias Corrected Bootstrap class for time series data.
+    Block Statistic Preserving Bootstrap class for time series data.
 
-    This class applies bias corrected bootstrapping to blocks of the time series.
+    This class applies statistic-preserving bootstrapping to blocks of the time series.
     The residuals are resampled using the specified block structure and added to
     the fitted values to generate new samples.
 
     Parameters
     ----------
-    block_bootstrap : BaseBlockBootstrap
+    block_bootstrap : BlockBootstrap, default=MovingBlockBootstrap()
         The block bootstrap algorithm.
     n_bootstraps : Integral, default=10
         The number of bootstrap samples to create.
     statistic : Callable, default=np.mean
         A callable function to compute the statistic that should be preserved.
     statistic_axis : Integral, default=0
         The axis along which the statistic should be computed.
@@ -482,20 +456,20 @@
     -------
     __init__ : Initialize self.
     _generate_samples_single_bootstrap : Generate a single bootstrap sample.
     """
 
     def __init__(
         self,
-        block_bootstrap,
         n_bootstraps: Integral = 10,  # type: ignore
+        block_bootstrap: Optional[BlockBootstrap] = None,
         statistic=None,
         statistic_axis: Integral = 0,  # type: ignore
         statistic_keepdims: bool = False,
-        rng=None,
+        rng: RngTypes = None,  # type: ignore
     ) -> None:
         """
         Initialize self.
 
         Parameters
         ----------
         statistic_config : BaseStatisticPreservingBootstrapConfig
@@ -506,14 +480,16 @@
         super().__init__(
             n_bootstraps=n_bootstraps,
             statistic=statistic,
             statistic_axis=statistic_axis,
             statistic_keepdims=statistic_keepdims,
             rng=rng,
         )
+        if block_bootstrap is None:
+            block_bootstrap = MovingBlockBootstrap()
         self.block_bootstrap = block_bootstrap
 
     def _generate_samples_single_bootstrap(self, X: np.ndarray, y=None):
         if self.statistic_X is None:
             self.statistic_X = super()._calculate_statistic(X=X)
         (
             block_indices,
@@ -585,15 +561,15 @@
             # Add new residuals to the fitted values to create the bootstrap time series
             bootstrap_samples = self.X_fitted + bootstrap_residuals
             return [np.arange(0, X.shape[0])], [bootstrap_samples]
 
         else:
             # Resample residuals
             resampled_indices = generate_random_indices(
-                self.resids.shape[0], self.config.rng
+                self.resids.shape[0], self.config.rng  # type: ignore
             )
             resampled_residuals = self.resids[resampled_indices]
             resids_dist, resids_dist_params = super()._fit_distribution(
                 resampled_residuals
             )
             # Generate new residuals from the fitted distribution
             bootstrap_residuals = resids_dist.rvs(
@@ -614,15 +590,15 @@
     This class applies distribution bootstrapping to blocks of the time series.
     The residuals are fit to a distribution, then resampled using the specified
     block structure. Then new residuals are generated from the fitted
     distribution and added to the fitted values to generate new samples.
 
     Parameters
     ----------
-    block_bootstrap : BaseBlockBootstrap
+    block_bootstrap : BlockBootstrap, default=MovingBlockBootstrap()
         The block bootstrap algorithm.
     n_bootstraps : Integral, default=10
         The number of bootstrap samples to create.
     distribution: str, default='normal'
         The distribution to use for generating the bootstrapped samples.
         Must be one of 'poisson', 'exponential', 'normal', 'gamma', 'beta',
         'lognormal', 'weibull', 'pareto', 'geometric', or 'uniform'.
@@ -664,23 +640,23 @@
     Notes
     -----
     We either fit the distribution to the residuals once and generate new samples from the fitted distribution with a new random seed, or resample the residuals once and fit the distribution to the resampled residuals, then generate new samples from the fitted distribution with the same random seed n_bootstrap times.
     """
 
     def __init__(
         self,
-        block_bootstrap,
         n_bootstraps: Integral = 10,  # type: ignore
+        block_bootstrap: Optional[BlockBootstrap] = None,
         distribution: str = "normal",
         refit: bool = False,
-        model_type="ar",
-        model_params=None,
+        model_type: ModelTypesWithoutArch = "ar",
+        model_params: Optional[dict] = None,
         order=None,
         save_models: bool = False,
-        rng=None,
+        rng: RngTypes = None,  # type: ignore
     ) -> None:
         """
         Initialize self.
 
         Parameters
         ----------
         distribution_config : BaseDistributionBootstrapConfig
@@ -694,14 +670,16 @@
             refit=refit,
             save_models=save_models,
             order=order,
             model_type=model_type,
             model_params=model_params,
             rng=rng,
         )
+        if block_bootstrap is None:
+            block_bootstrap = MovingBlockBootstrap()
         self.block_bootstrap = block_bootstrap
 
     def _generate_samples_single_bootstrap(self, X: np.ndarray, y=None):
         # Fit the model and residuals
         super()._fit_model(X=X, y=y)
         (
             block_indices,
@@ -801,15 +779,15 @@
         ts_simulator = TimeSeriesSimulator(
             X_fitted=self.X_fitted,
             rng=self.config.rng,
             fitted_model=self.resids_fit_model,
         )
 
         simulated_samples = ts_simulator.generate_samples_sieve(
-            model_type=self.config.resids_model_type,
+            model_type=self.config.resids_model_type,  # type: ignore
             resids_lags=self.resids_order,
             resids_coefs=self.resids_coefs,
             resids=self.resids,
         )
 
         return [np.arange(X.shape[0])], [simulated_samples]
 
@@ -821,15 +799,15 @@
     This class applies Sieve bootstrapping to blocks of the time series.
     The residuals are fit to a second model, then resampled using the
     specified block structure. The new residuals are then added to the
     fitted values to generate new samples.
 
     Parameters
     ----------
-    block_bootstrap : BaseBlockBootstrap
+    block_bootstrap : BlockBootstrap, default=MovingBlockBootstrap()
         The block bootstrap algorithm.
     resids_model_type : str, default="ar"
         The model type to use for fitting the residuals. Must be one of "ar", "arima", "sarima", "var", or "arch".
     resids_order : Integral or list or tuple, default=None
         The order of the model to use for fitting the residuals. If None, the order is automatically determined.
     save_resids_models : bool, default=False
         Whether to save the fitted models for the residuals.
@@ -856,25 +834,25 @@
     -------
     _init_ : Initialize self.
     _generate_samples_single_bootstrap : Generate a single bootstrapped sample.
     """
 
     def __init__(
         self,
-        block_bootstrap,
         n_bootstraps: Integral = 10,  # type: ignore
-        resids_model_type="ar",
+        block_bootstrap: Optional[BlockBootstrap] = None,
+        resids_model_type: ModelTypes = "ar",
         resids_order=None,
         save_resids_models: bool = False,
         kwargs_base_sieve=None,
-        model_type="ar",
-        model_params=None,
+        model_type: ModelTypesWithoutArch = "ar",
+        model_params: Optional[dict] = None,
         order=None,
         save_models: bool = False,
-        rng=None,
+        rng: RngTypes = None,  # type: ignore
     ) -> None:
         """
         Initialize self.
 
         Parameters
         ----------
         sieve_config : BaseSieveBootstrapConfig
@@ -890,29 +868,31 @@
             kwargs_base_sieve=kwargs_base_sieve,
             model_type=model_type,
             model_params=model_params,
             order=order,
             save_models=save_models,
             rng=rng,
         )
+        if block_bootstrap is None:
+            block_bootstrap = MovingBlockBootstrap()
         self.block_bootstrap = block_bootstrap
 
     def _generate_samples_single_bootstrap(self, X: np.ndarray, y=None):
         # Fit the model and residuals
         super()._fit_model(X=X, y=y)
         super()._fit_resids_model(X=self.resids)
 
         ts_simulator = TimeSeriesSimulator(
             X_fitted=self.X_fitted,
             rng=self.config.rng,
             fitted_model=self.resids_fit_model,
         )
 
         simulated_samples = ts_simulator.generate_samples_sieve(
-            model_type=self.config.resids_model_type,
+            model_type=self.config.resids_model_type,  # type: ignore
             resids_lags=self.resids_order,
             resids_coefs=self.resids_coefs,
             resids=self.resids,
         )
 
         resids_resids = self.X_fitted - simulated_samples
         (
```

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/markov_sampler.py` & `tsbootstrap-0.1.1/src/tsbootstrap/markov_sampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import logging
 import warnings
 from numbers import Integral
+from typing import Optional
 
 import numpy as np
 import scipy.stats
 from sklearn.cluster import KMeans
 from sklearn.decomposition import PCA
 from sklearn.exceptions import NotFittedError
 from sklearn.utils.validation import check_is_fitted
@@ -11,14 +13,16 @@
 from tsbootstrap.utils.types import BlockCompressorTypes
 from tsbootstrap.utils.validate import (
     validate_blocks,
     validate_integers,
     validate_literal_type,
 )
 
+logger = logging.getLogger("tsbootstrap")
+
 try:
     from dtaidistance import dtw_ndim  # type: ignore
 
     # dtaidistance does not compile for Python 3.10 and 3.11
 
     dtaidistance_installed = True
 except ImportError:
@@ -41,16 +45,16 @@
         Summarize each block in the input list of blocks using the specified method.
     """
 
     def __init__(
         self,
         method: BlockCompressorTypes = "middle",
         apply_pca_flag: bool = False,
-        pca: PCA = None,
-        random_seed: Integral = None,
+        pca: Optional[PCA] = None,
+        random_seed: Optional[Integral] = None,
     ):
         """
         Initialize the BlockCompressor with the selected method, PCA flag, PCA instance, and random seed.
 
         Parameters
         ----------
         method : BlockCompressorTypes, optional
@@ -141,42 +145,42 @@
 
     @property
     def pca(self) -> PCA:
         """Getter for pca."""
         return self._pca
 
     @pca.setter
-    def pca(self, value: PCA) -> None:
+    def pca(self, value: Optional[PCA]) -> None:
         """
         Setter for pca. Performs validation on assignment.
 
         Parameters
         ----------
         value : Optional[PCA]
             The PCA instance to use.
         """
         if value is not None:
             if not isinstance(value, PCA):
                 raise TypeError(
                     "pca must be a sklearn.decomposition.PCA instance"
                 )
-            elif value.n_components != 1:
+            elif value.n_components != 1:  # type: ignore
                 raise ValueError(
                     "The provided PCA object must have n_components set to 1 for compression."
                 )
             self._pca = value
         else:
             self._pca = PCA(n_components=1)
 
     @property
     def random_seed(self):
         return self._random_seed
 
     @random_seed.setter
-    def random_seed(self, value: Integral) -> None:
+    def random_seed(self, value: Optional[Integral]) -> None:
         """
         Setter for rng. Performs validation on assignment.
 
         Parameters
         ----------
         value : Generator
             The random number generator to use.
@@ -290,15 +294,15 @@
             A 1D numpy array representing the compressed block.
 
         Notes
         -----
         This method uses the scikit-learn implementation of k-means clustering.
         """
         return (
-            KMeans(n_clusters=1, random_state=self.random_seed, n_init="auto")
+            KMeans(n_clusters=1, random_state=self.random_seed, n_init="auto")  # type: ignore
             .fit(block)
             .cluster_centers_[0]
         )
 
     def _kmedians_compression(self, block: np.ndarray) -> np.ndarray:
         """
         Helper method to compress a block using k-medians clustering.
@@ -315,19 +319,19 @@
 
         Notes
         -----
         This method uses the scipy implementation of k-medians clustering.
         """
         from pyclustering.cluster.kmedians import kmedians  # type: ignore
 
-        rng = np.random.default_rng(self.random_seed)
+        rng = np.random.default_rng(self.random_seed)  # type: ignore
         initial_centers = rng.choice(block.flatten(), size=(1, block.shape[1]))
         kmedians_instance = kmedians(block, initial_centers)
         kmedians_instance.process()
-        return kmedians_instance.get_medians()[0]
+        return kmedians_instance.get_medians()[0]  # type: ignore
 
     def _kmedoids_compression(self, block: np.ndarray) -> np.ndarray:
         """
         Helper method to compress a block using k-medoids clustering.
 
         Parameters
         ----------
@@ -339,18 +343,18 @@
         np.ndarray
             A 1D numpy array representing the compressed block.
 
         Notes
         -----
         This method uses the scikit-learn-extra implementation of k-medoids clustering.
         """
-        from sklearn_extra.cluster import KMedoids  # type: ignore
+        from sklearn_extra.cluster import KMedoids
 
         return (
-            KMedoids(n_clusters=1, random_state=self.random_seed)
+            KMedoids(n_clusters=1, random_state=self.random_seed)  # type: ignore
             .fit(block)
             .cluster_centers_[0]
         )
 
     def summarize_blocks(self, blocks) -> np.ndarray:
         """
         Summarize each block in the input list of blocks using the specified method.
@@ -484,15 +488,15 @@
 
         num_blocks = len(blocks)
 
         # Compute pairwise DTW distances between all pairs of blocks
         distances = np.zeros((num_blocks, num_blocks))
         for i in range(num_blocks):
             for j in range(i, num_blocks):
-                dist = dtw_ndim.distance(blocks[i], blocks[j]) + eps
+                dist = dtw_ndim.distance(blocks[i], blocks[j]) + eps  # type: ignore
                 distances[i, j] = dist
                 distances[j, i] = dist
 
         # Add a small constant to the diagonal to allow remaining in the same state
         np.fill_diagonal(distances, eps)
 
         return distances
@@ -575,19 +579,19 @@
     >>> start_probs, trans_probs, centers, covariances, assignments = sampler.sample(blocks, n_states=5, blocks_as_hidden_states_flag=True)
     """
 
     def __init__(
         self,
         method: BlockCompressorTypes = "middle",
         apply_pca_flag: bool = False,
-        pca: PCA = None,
-        n_iter_hmm: Integral = 100,
-        n_fits_hmm: Integral = 10,
+        pca: Optional[PCA] = None,
+        n_iter_hmm: Integral = 100,  # type: ignore
+        n_fits_hmm: Integral = 10,  # type: ignore
         blocks_as_hidden_states_flag: bool = False,
-        random_seed: Integral = None,
+        random_seed: Optional[Integral] = None,
     ):
         """
         Initialize the MarkovSampler instance.
 
         Parameters
         ----------
         method : str, optional
@@ -648,15 +652,15 @@
         Setter for n_iter_hmm. Performs validation on assignment.
 
         Parameters
         ----------
         value : Integral
             The number of iterations to run the HMM for.
         """
-        validate_integers(value, min_value=1)
+        validate_integers(value, min_value=1)  # type: ignore
         self._n_iter_hmm = value
 
     @property
     def n_fits_hmm(self) -> Integral:
         """Getter for n_fits_hmm."""
         return self._n_fits_hmm
 
@@ -666,15 +670,15 @@
         Setter for n_fits_hmm. Performs validation on assignment.
 
         Parameters
         ----------
         value : Integral
             The number of times to fit the HMM.
         """
-        validate_integers(value, min_value=1)
+        validate_integers(value, min_value=1)  # type: ignore
         self._n_fits_hmm = value
 
     @property
     def blocks_as_hidden_states_flag(self) -> bool:
         """Getter for blocks_as_hidden_states_flag."""
         return self._blocks_as_hidden_states_flag
 
@@ -694,15 +698,15 @@
 
     @property
     def random_seed(self):
         """Getter for random_seed."""
         return self._random_seed
 
     @random_seed.setter
-    def random_seed(self, value: Integral) -> None:
+    def random_seed(self, value: Optional[Integral]) -> None:
         """
         Setter for rng. Performs validation on assignment.
 
         Parameters
         ----------
         value : Generator
             The random number generator to use.
@@ -721,18 +725,18 @@
                     self._random_seed = value
         else:
             self._random_seed = None
 
     def fit_hidden_markov_model(
         self,
         X: np.ndarray,
-        n_states: Integral = 5,
-        transmat_init=None,
-        means_init=None,
-        lengths=None,
+        n_states: Integral = 5,  # type: ignore
+        transmat_init: Optional[np.ndarray] = None,
+        means_init: Optional[np.ndarray] = None,
+        lengths: Optional[np.ndarray] = None,
     ):
         """
         Fit a Gaussian Hidden Markov Model on the input data.
 
         Parameters
         ----------
         X : np.ndarray
@@ -749,15 +753,15 @@
             X, n_states, transmat_init, means_init
         )
 
         best_score = -np.inf
         best_hmm_model = None
         for idx in range(self.n_fits_hmm):
             hmm_model = self._initialize_hmm_model(
-                n_states, transmat_init, means_init, idx
+                n_states, transmat_init, means_init, idx  # type: ignore
             )
 
             try:
                 hmm_model.fit(X, lengths=lengths)
             except ValueError:
                 continue
 
@@ -773,16 +777,16 @@
 
         return best_hmm_model
 
     def _validate_fit_hidden_markov_model_inputs(
         self,
         X: np.ndarray,
         n_states: Integral,
-        transmat_init: np.ndarray,
-        means_init: np.ndarray,
+        transmat_init: Optional[np.ndarray],
+        means_init: Optional[np.ndarray],
     ) -> None:
         """
         Validate the inputs to fit_hidden_markov_model.
 
         Parameters
         ----------
         X : np.ndarray
@@ -828,16 +832,16 @@
                 raise TypeError("Input 'means_init' must be a NumPy array.")
             if means_init.shape != (n_states, X.shape[1]):
                 raise ValueError("Invalid shape for initial means")
 
     def _initialize_hmm_model(
         self,
         n_states: Integral,
-        transmat_init: np.ndarray,
-        means_init: np.ndarray,
+        transmat_init: Optional[np.ndarray],
+        means_init: Optional[np.ndarray],
         idx: Integral,
     ):
         """
         Initialize a Gaussian Hidden Markov Model.
 
         Parameters
         ----------
@@ -858,17 +862,17 @@
         Notes
         -----
         This method is called by fit_hidden_markov_model. It is not intended to be called directly.
         """
         from hmmlearn import hmm
 
         hmm_model = hmm.GaussianHMM(
-            n_components=n_states,
+            n_components=n_states,  # type: ignore
             covariance_type="full",
-            n_iter=self.n_iter_hmm,
+            n_iter=self.n_iter_hmm,  # type: ignore
             init_params="stmc",
             params="stmc",
             random_state=(
                 self.random_seed + idx if self.random_seed is not None else idx
             ),
         )
         if transmat_init is not None:
@@ -877,15 +881,15 @@
             hmm_model.means_ = means_init
 
         return hmm_model
 
     def fit(
         self,
         blocks,
-        n_states: Integral = 5,
+        n_states: Integral = 5,  # type: ignore
     ) -> "MarkovSampler":
         """
         Sample from a Markov chain with given transition probabilities.
 
         Parameters
         ----------
         blocks : List[np.ndarray] or np.ndarray
@@ -969,27 +973,27 @@
 
             if self.blocks_as_hidden_states_flag:
                 n_states = len(blocks)
                 if min(lengths) < 10:
                     raise ValueError(
                         f"Input 'X' must have at least {n_states * 10} points to fit a {n_states}-state HMM."
                     )
-                print(
+                logger.debug(
                     f"Using {len(blocks)} blocks as 'n_states', since 'blocks_as_hidden_states_flag' is True. Ignoring user-provided 'n_states' parameter."
                 )
                 lengths = None
         else:
             self._validate_single_block_input(blocks)
             X = blocks
             lengths = None
 
         if not isinstance(n_states, Integral) or n_states < 1:
             raise ValueError("Input 'n_states' must be an integer >= 1.")
 
-        if n_states > X.shape[0]:
+        if n_states > X.shape[0]:  # type: ignore
             raise ValueError(
                 f"Input 'X' must have at least {n_states} points to fit a {n_states}-state HMM."
             )
 
         return X, lengths, n_states
 
     def _validate_single_block_input(self, blocks: np.ndarray):
@@ -1022,16 +1026,16 @@
         if blocks.ndim != 2 or blocks.shape[0] == 0 or blocks.shape[1] == 0:
             raise ValueError(
                 "Input 'blocks' must be a non-empty two-dimensional array."
             )
 
     def sample(
         self,
-        X=None,
-        random_seed: Integral = None,
+        X: Optional[np.ndarray] = None,
+        random_seed: Optional[Integral] = None,
     ):
         """
         Sample from a Markov chain with given transition probabilities.
 
         Parameters
         ----------
         X : Optional[np.ndarray]
@@ -1041,20 +1045,20 @@
 
         Returns
         -------
         Tuple[np.ndarray, np.ndarray]
             A tuple containing the start probabilities and transition probabilities of the Markov chain.
         """
         # Check if the model is already fitted
-        check_is_fitted(self, ["model"])
+        check_is_fitted(self, ["model"])  # type: ignore
         if X is None:
             X = self.X
         if random_seed is None:
             random_seed = self.random_seed
-        return self.model.sample(X.shape[0], random_state=random_seed)
+        return self.model.sample(X.shape[0], random_state=random_seed)  # type: ignore
 
     def __repr__(self) -> str:
         return f"BlockCompressor(method='{self.method}', apply_pca_flag={self.apply_pca_flag}, pca={self.pca}, random_seed={self.random_seed})"
 
     def __str__(self) -> str:
         return f"BlockCompressor using method '{self.method}' with PCA flag {self.apply_pca_flag} and random seed {self.random_seed}"
```

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/ranklags.py` & `tsbootstrap-0.1.1/src/tsbootstrap/ranklags.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from __future__ import annotations
 
+import logging
 from numbers import Integral
 
 import numpy as np
 
 from tsbootstrap.utils.types import ModelTypes
 from tsbootstrap.utils.validate import validate_integers, validate_literal_type
 
+logger = logging.getLogger("tsbootstrap")
+
 
 class RankLags:
     """
     A class that uses several metrics to rank lags for time series models.
 
     Methods
     -------
@@ -188,15 +191,18 @@
         bic_values = []
         for lag in range(1, self.max_lag + 1):
             try:
                 fit_obj = TSFit(order=lag, model_type=self.model_type)
                 model = fit_obj.fit(X=self.X, y=self.y).model
             except Exception as e:
                 # raise RuntimeError(f"An error occurred during fitting: {e}")
-                print(f"{e}")
+                logger.warning(
+                    f"An error occurred during fitting for lag {lag}. Skipping remaining lags."
+                )
+                logger.debug(f"{e}")
                 break
             if self.save_models:
                 self.models.append(model)
             aic_values.append(model.aic)
             bic_values.append(model.bic)
 
         aic_ranked_lags = np.argsort(aic_values) + 1
```

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/registry/_lookup.py` & `tsbootstrap-0.1.1/src/tsbootstrap/registry/_lookup.py`

 * *Files identical despite different names*

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/registry/_tags.py` & `tsbootstrap-0.1.1/src/tsbootstrap/registry/_tags.py`

 * *Files identical despite different names*

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/tests/scenarios/scenarios.py` & `tsbootstrap-0.1.1/src/tsbootstrap/tests/scenarios/scenarios.py`

 * *Files identical despite different names*

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/tests/scenarios/scenarios_bootstrap.py` & `tsbootstrap-0.1.1/src/tsbootstrap/tests/scenarios/scenarios_bootstrap.py`

 * *Files identical despite different names*

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/tests/scenarios/scenarios_getter.py` & `tsbootstrap-0.1.1/src/tsbootstrap/tests/scenarios/scenarios_getter.py`

 * *Files identical despite different names*

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/tests/test_all_bootstraps.py` & `tsbootstrap-0.1.1/src/tsbootstrap/tests/test_all_bootstraps.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Automated tests based on the skbase test suite template."""
 
+import inspect
+
 import numpy as np
 import pytest
 from skbase.testing import QuickTester
 
 from tsbootstrap.tests.test_all_estimators import (
     BaseFixtureGenerator,
     PackageConfig,
@@ -15,14 +17,49 @@
 
     # class variables which can be overridden by descendants
     # ------------------------------------------------------
 
     # which object types are generated; None=all, or class (passed to all_objects)
     object_type_filter = "bootstrap"
 
+    def test_class_signature(self, object_class):
+        """Check constraints on class init signature.
+
+        Tests that:
+
+        * the first parameter is n_bootstraps, with default 10
+        * all parameters have defaults
+        """
+        init_signature = inspect.signature(object_class.__init__)
+
+        # Consider the constructor parameters excluding 'self'
+        param_names_in_order = [
+            p.name
+            for p in init_signature.parameters.values()
+            if p.name != "self" and p.kind != p.VAR_KEYWORD
+        ]
+
+        param_defaults = object_class.get_param_defaults()
+
+        # test that all parameters have defaults
+        params_without_default = [
+            param
+            for param in param_names_in_order
+            if param not in param_defaults
+        ]
+
+        assert len(params_without_default) == 0, (
+            f"All parameters of bootstraps must have default values. "
+            f"Init parameters without default values: {params_without_default}. "
+        )
+
+        # test that first parameter is n_bootstraps, with default 10
+        assert param_names_in_order[0] == "n_bootstraps"
+        assert param_defaults["n_bootstraps"] == 10
+
     def test_n_bootstraps(self, object_instance):
         """Tests handling of n_bootstraps parameter."""
         cls_name = object_instance.__class__.__name__
 
         params = object_instance.get_params()
 
         if "n_bootstraps" not in params:
```

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/tests/test_all_estimators.py` & `tsbootstrap-0.1.1/src/tsbootstrap/tests/test_all_estimators.py`

 * *Files identical despite different names*

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/tests/test_class_register.py` & `tsbootstrap-0.1.1/src/tsbootstrap/tests/test_class_register.py`

 * *Files identical despite different names*

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/tests/test_switch.py` & `tsbootstrap-0.1.1/src/tsbootstrap/tests/test_switch.py`

 * *Files identical despite different names*

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/time_series_model.py` & `tsbootstrap-0.1.1/src/tsbootstrap/time_series_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections.abc import Callable
 from numbers import Integral
-from typing import Any, Literal
+from typing import Any, Literal, Optional
 
 import numpy as np
 
 from tsbootstrap.utils.odds_and_ends import suppress_output
 from tsbootstrap.utils.types import ModelTypes, OrderTypes
 from tsbootstrap.utils.validate import (
     validate_integers,
@@ -17,15 +17,15 @@
     """A class for fitting time series models to data."""
 
     _tags = {"python_dependencies": ["arch", "statsmodels"]}
 
     def __init__(
         self,
         X: np.ndarray,
-        y=None,
+        y: Optional[np.ndarray] = None,
         model_type: ModelTypes = "ar",
         verbose: bool = True,
     ):
         """Initializes a TimeSeriesModel object.
 
         Parameters
         ----------
@@ -47,21 +47,21 @@
         self.X = X
         self.y = y
         self.verbose = verbose
 
     @property
     def model_type(self) -> ModelTypes:
         """The type of model to fit."""
-        return self._model_type
+        return self._model_type  # type: ignore
 
     @model_type.setter
     def model_type(self, value: ModelTypes) -> None:
         """Sets the type of model to fit."""
         validate_literal_type(value, ModelTypes)
-        value = value.lower()
+        value = value.lower()  # type: ignore
         self._model_type = value
 
     @property
     def X(self) -> np.ndarray:
         """The input data."""
         return self._X
 
@@ -72,20 +72,20 @@
             value,
             None,
             model_is_var=self.model_type == "var",
             model_is_arch=self.model_type == "arch",
         )
 
     @property
-    def y(self) -> np.ndarray:
+    def y(self) -> Optional[np.ndarray]:
         """Optional array of exogenous variables."""
         return self._y
 
     @y.setter
-    def y(self, value: np.ndarray) -> None:
+    def y(self, value: Optional[np.ndarray]) -> None:
         """Sets the optional array of exogenous variables."""
         _, self._y = validate_X_and_y(
             self.X,
             value,
             model_is_var=self.model_type == "var",
             model_is_arch=self.model_type == "arch",
         )
@@ -157,15 +157,17 @@
         Raises
         ------
         ValueError
             If the specified order value exceeds the allowed range.
         """
         k = self.y.shape[1] if self.y is not None else 0
         seasonal_terms, trend_parameters = self._calculate_terms(kwargs)
-        max_lag = (N - k - seasonal_terms - trend_parameters) // 2
+        max_lag = (
+            N - k - seasonal_terms - trend_parameters  # type: ignore
+        ) // 2  # - 1
 
         if order is not None:
             if isinstance(order, list):
                 if max(order) > max_lag:
                     raise ValueError(
                         f"Maximum allowed lag value exceeded. The allowed maximum is {max_lag}."
                     )
@@ -209,17 +211,15 @@
             else:
                 raise TypeError("The seasonal period must be an integer.")
 
         seasonal_terms = (period - 1) if seasonal and period is not None else 0
         trend_parameters = (
             1
             if kwargs.get("trend", "c") == "c"
-            else 2
-            if kwargs.get("trend") == "ct"
-            else 0
+            else 2 if kwargs.get("trend") == "ct" else 0
         )
 
         return seasonal_terms, trend_parameters
 
     def fit_ar(self, order=None, **kwargs):
         """
         Fits an AR model to the input data.
@@ -349,16 +349,16 @@
                 arima_order = (order[0], order[1], 0)
             else:
                 arima_order = order[:3]
 
         if len(arima_order) != 3:
             raise ValueError("The order must be a 3-tuple")
 
-        validate_integers(*order, min_value=0)
-        validate_integers(*arima_order, min_value=0)
+        validate_integers(*order, min_value=0)  # type: ignore
+        validate_integers(*arima_order, min_value=0)  # type: ignore
 
         # Check to ensure that the AR terms (p and P) don't duplicate order
         if arima_order[0] >= order[-1] and order[0] != 0:
             raise ValueError(
                 f"The autoregressive term 'p' ({arima_order[0]}) is greater than or equal to the seasonal period 's' ({order[-1]}) while the seasonal autoregressive term 'P' is not zero ({order[0]}). This could lead to duplication of order."
             )
 
@@ -380,15 +380,15 @@
                 **kwargs,
             )
             model_fit = model.fit(disp=-1)
             return model_fit
 
         return self._fit_with_verbose_handling(fit_logic)
 
-    def fit_var(self, order: int = None, **kwargs):
+    def fit_var(self, order: Optional[int] = None, **kwargs):
         """Fits a Vector Autoregression (VAR) model to the input data.
 
         Parameters
         ----------
         order : int, optional
             The number of order to include in the VAR model.
         **kwargs
@@ -419,15 +419,15 @@
             model_fit = model.fit(**kwargs)
             return model_fit
 
         return self._fit_with_verbose_handling(fit_logic)
 
     def fit_arch(
         self,
-        order: int = None,
+        order: Optional[int] = None,
         p: int = 1,
         q: int = 1,
         arch_model_type: Literal[
             "GARCH", "EGARCH", "TARCH", "AGARCH"
         ] = "GARCH",
         mean_type: Literal["zero", "AR"] = "zero",
         **kwargs,
@@ -461,26 +461,26 @@
         """
         from arch import arch_model
 
         if order is None:
             order = 1
 
         # Assuming a validate_X_and_y function exists for data validation
-        validate_integers(p, q, order, min_value=1)
+        validate_integers(p, q, order, min_value=1)  # type: ignore
 
         if mean_type not in ["zero", "AR"]:
             raise ValueError("mean_type must be one of 'zero' or 'AR'")
 
         if arch_model_type in ["GARCH", "EGARCH"]:
             model = arch_model(
                 y=self.X,
                 x=self.y,
                 mean=mean_type,
                 lags=order,
-                vol=arch_model_type,
+                vol=arch_model_type,  # type: ignore
                 p=p,
                 q=q,
                 **kwargs,
             )
         elif arch_model_type == "TARCH":
             model = arch_model(
                 y=self.X,
@@ -516,15 +516,15 @@
         def fit_logic(model=model, options=options):
             """Logic for fitting ARIMA model."""
             model_fit = model.fit(disp="off", options=options)
             return model_fit
 
         return self._fit_with_verbose_handling(fit_logic)
 
-    def fit(self, order: OrderTypes = None, **kwargs):
+    def fit(self, order: OrderTypes = None, **kwargs):  # type: ignore
         """Fits a time series model to the input data.
 
         Parameters
         ----------
         order : OrderTypes, optional
             The order of the model. If not specified, the default order for the selected model type is used.
         **kwargs
```

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/time_series_simulator.py` & `tsbootstrap-0.1.1/src/tsbootstrap/time_series_simulator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from numbers import Integral
-from typing import Any
+from typing import Any, List, Optional, Union
 
 import numpy as np
 from numpy.random import Generator
 
 from tsbootstrap.tsfit import TSFit
 from tsbootstrap.utils.types import ModelTypes
 from tsbootstrap.utils.validate import (
@@ -165,15 +165,15 @@
             If `init` is not the same length as `max_lag`.
 
         TypeError
             If `lags` is not an integer or a list of integers.
         """
         random_errors = self.rng.normal(size=self.n_samples)
 
-        if len(init) < max_lag:
+        if len(init) < max_lag:  # type: ignore
             raise ValueError(
                 "Length of 'init' must be at least as long as the maximum lag in 'lags'"
             )
 
         # In case init is 2d with shape (X, 1), convert it to 1d
         init = init.ravel()
         series = np.zeros(self.n_samples, dtype=init.dtype)
@@ -203,15 +203,15 @@
 
             series[t] = ar_term + trend_term + random_errors[t]
 
         return series
 
     def simulate_ar_process(
         self,
-        resids_lags,
+        resids_lags: Union[Integral, List[Integral]],
         resids_coefs: np.ndarray,
         resids: np.ndarray,
     ) -> np.ndarray:
         """
         Simulate AR process from the fitted model.
 
         Parameters
@@ -238,15 +238,15 @@
 
         TypeError
             If `fitted_model` is not an instance of `AutoRegResultsWrapper`.
             If `resids_lags` is not an integer or a list of integers.
         """
         from statsmodels.tsa.ar_model import AutoRegResultsWrapper
 
-        validate_integers(resids_lags, min_value=1)
+        validate_integers(resids_lags, min_value=1)  # type: ignore
 
         if not isinstance(self.fitted_model, AutoRegResultsWrapper):
             # logger.error("fitted_model must be an instance of AutoRegResultsWrapper.")
             raise TypeError(
                 f"fitted_model must be an instance of AutoRegResultsWrapper. Got {type(self.fitted_model)}."
             )
 
@@ -268,38 +268,38 @@
         # Convert resids_lags to a NumPy array if it is not already. When called from `generate_samples_sieve`, it will be sorted.
         resids_lags = (
             np.arange(1, resids_lags + 1)
             if isinstance(resids_lags, Integral)
             else np.array(sorted(resids_lags))
         )  # type: ignore
         # resids_lags.shape: (n_lags,)
-        max_lag = np.max(resids_lags)
+        max_lag = np.max(resids_lags)  # type: ignore
         if resids_coefs.shape[0] != 1:
             raise ValueError(
                 "AR coefficients must be a 1D NumPy array of shape (1, X)"
             )
         if resids_coefs.shape[1] != len(resids_lags):  # type: ignore
             raise ValueError(
                 "Length of 'resids_coefs' must be the same as the length of 'lags'"
             )
 
         # Simulate residuals using the AR model
         simulated_residuals = self._simulate_ar_residuals(
-            lags=resids_lags,
+            lags=resids_lags,  # type: ignore
             coefs=resids_coefs,
             init=resids[:max_lag],
             max_lag=max_lag,
         )
         # simulated_residuals.shape: (n_samples,)
 
         bootstrap_series[:max_lag] = X_fitted[:max_lag]
 
         # Loop through the series, calculating each value based on the lagged values, coefficients, and random error
         for t in range(max_lag, self.n_samples):
-            lagged_values = bootstrap_series[t - resids_lags]
+            lagged_values = bootstrap_series[t - resids_lags]  # type: ignore
             # lagged_values.shape: (n_lags,)
             lagged_values = lagged_values.reshape(-1, 1)
             # lagged_values.shape: (n_lags, 1)
             bootstrap_series[t] = (
                 resids_coefs @ lagged_values + simulated_residuals[t]
             )
 
@@ -333,15 +333,15 @@
                 random_state=self.rng,
             )
         elif isinstance(self.fitted_model, VARResultsWrapper):
             return self.fitted_model.simulate_var(
                 steps=self.n_samples + self.burnin, seed=rng_seed
             )
         elif isinstance(self.fitted_model, ARCHModelResult):
-            return self.fitted_model.model.simulate(
+            return self.fitted_model.model.simulate(  # type: ignore
                 params=self.fitted_model.params,
                 nobs=self.n_samples,
                 burn=self.burnin,
             )["data"].values
         raise ValueError(f"Unsupported fitted model type {self.fitted_model}.")
 
     def simulate_non_ar_process(self) -> np.ndarray:
@@ -367,17 +367,17 @@
         ):
             simulated_residuals = simulated_residuals[self.burnin :]
         return self.X_fitted + simulated_residuals
 
     def generate_samples_sieve(
         self,
         model_type: ModelTypes,
-        resids_lags=None,
-        resids_coefs: np.ndarray = None,
-        resids: np.ndarray = None,
+        resids_lags: Optional[Union[Integral, List[Integral]]] = None,
+        resids_coefs: Optional[np.ndarray] = None,
+        resids: Optional[np.ndarray] = None,
     ) -> np.ndarray:
         """
         Generate a bootstrap sample using the sieve bootstrap.
 
         Parameters
         ----------
         model_type: ModelTypes
@@ -404,15 +404,15 @@
             self._validate_ar_simulation_params(
                 {
                     "resids_lags": resids_lags,
                     "resids_coefs": resids_coefs,
                     "resids": resids,
                 }
             )
-            return self.simulate_ar_process(resids_lags, resids_coefs, resids)
+            return self.simulate_ar_process(resids_lags, resids_coefs, resids)  # type: ignore
         else:
             return self.simulate_non_ar_process()
 
     def __repr__(self) -> str:
         return f"TimeSeriesSimulator(fitted_model={self.fitted_model}, n_samples={self.n_samples}, n_features={self.n_features})"
 
     def __str__(self) -> str:
```

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/tsfit.py` & `tsbootstrap-0.1.1/src/tsbootstrap/tsfit.py`

 * *Files identical despite different names*

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/utils/dependencies.py` & `tsbootstrap-0.1.1/src/tsbootstrap/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/utils/estimator_checks.py` & `tsbootstrap-0.1.1/src/tsbootstrap/utils/estimator_checks.py`

 * *Files identical despite different names*

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/utils/odds_and_ends.py` & `tsbootstrap-0.1.1/src/tsbootstrap/utils/odds_and_ends.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import os
 from contextlib import contextmanager
 from numbers import Integral
+from typing import Union
 
 import numpy as np
 from numpy.random import Generator
 
+from tsbootstrap.utils.types import RngTypes
+
 
 def time_series_split(X: np.ndarray, test_ratio: float):
     """
     Splits a given time series into training and test sets.
 
     Parameters
     ----------
@@ -28,15 +31,15 @@
             f"Test ratio must be between 0 and 1. Got {test_ratio}"
         )
 
     split_index = int(len(X) * (1 - test_ratio))
     return X[:split_index], X[split_index:]
 
 
-def check_generator(seed_or_rng, seed_allowed: bool = True) -> Generator:
+def check_generator(seed_or_rng: RngTypes, seed_allowed: bool = True) -> Generator:  # type: ignore
     """Turn seed into a np.random.Generator instance.
 
     Parameters
     ----------
     seed_or_rng : int, Generator, or None
         If seed_or_rng is None, return the Generator singleton used by np.random.
         If seed_or_rng is an int, return a new Generator instance seeded with seed_or_rng.
@@ -72,15 +75,15 @@
 
     raise ValueError(
         f"{seed_or_rng} cannot be used to seed a numpy.random.Generator instance"
     )
 
 
 def generate_random_indices(
-    num_samples: Integral, rng: Generator = None
+    num_samples: Integral, rng: RngTypes = None  # type: ignore
 ) -> np.ndarray:
     """
     Generate random indices with replacement.
 
     This function generates random indices from 0 to `num_samples-1` with replacement.
     The generated indices can be used for bootstrap sampling, etc.
 
@@ -111,15 +114,15 @@
     >>> generate_random_indices(5)
     array([2, 1, 4, 2, 0])  # random
     """
     # Check types and values of num_samples and random_seed
     from tsbootstrap.utils.validate import validate_integers
 
     validate_integers(num_samples, min_value=1)  # type: ignore
-    rng = check_generator(rng, seed_allowed=False)
+    rng = check_generator(rng, seed_allowed=True)
 
     # Generate random indices with replacement
     in_bootstrap_indices = rng.choice(
         np.arange(num_samples), size=num_samples, replace=True  # type: ignore
     )
 
     return in_bootstrap_indices
```

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/utils/types.py` & `tsbootstrap-0.1.1/src/tsbootstrap/utils/types.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+# Use future annotations for better handling of forward references.
+from __future__ import annotations
+
 import sys
 from numbers import Integral
-from typing import Any, Literal, Optional, Union
+from typing import Any, List, Literal, Optional, Union
 
 from numpy.random import Generator
 from packaging.specifiers import SpecifierSet
 
+# Define model and block compressor types using Literal for clearer enum-style typing.
 ModelTypesWithoutArch = Literal["ar", "arima", "sarima", "var"]
 
 ModelTypes = Literal["ar", "arima", "sarima", "var", "arch"]
 
 BlockCompressorTypes = Literal[
     "first",
     "middle",
@@ -17,19 +21,27 @@
     "mode",
     "median",
     "kmeans",
     "kmedians",
     "kmedoids",
 ]
 
+# Check Python version for compatibility issues.
 sys_version = sys.version.split(" ")[0]
 new_typing_available = sys_version in SpecifierSet(">=3.10")
 
 
-def FittedModelTypes():
+def FittedModelTypes() -> tuple:
+    """
+    Return a tuple of fitted model types for use in isinstance checks.
+
+    Returns
+    -------
+        tuple: A tuple containing the result wrapper types for fitted models.
+    """
     from arch.univariate.base import ARCHModelResult
     from statsmodels.tsa.ar_model import AutoRegResultsWrapper
     from statsmodels.tsa.arima.model import ARIMAResultsWrapper
     from statsmodels.tsa.statespace.sarimax import SARIMAXResultsWrapper
     from statsmodels.tsa.vector_ar.var_model import VARResultsWrapper
 
     fmt = (
@@ -38,22 +50,23 @@
         SARIMAXResultsWrapper,
         VARResultsWrapper,
         ARCHModelResult,
     )
     return fmt
 
 
+# Define complex type conditions using the Python 3.10 union operator if available.
 if new_typing_available:
-    OrderTypesWithoutNone = Union[  # noqa: UP007
+    OrderTypesWithoutNone = Union[
         Integral,
-        list[Integral],
+        List[Integral],
         tuple[Integral, Integral, Integral],
         tuple[Integral, Integral, Integral, Integral],
     ]
-    OrderTypes = Optional[OrderTypesWithoutNone]  # noqa: UP007
+    OrderTypes = Optional[OrderTypesWithoutNone]
 
-    RngTypes = Optional[Union[Generator, Integral]]  # noqa: UP007
+    RngTypes = Optional[Union[Generator, Integral]]
 
 else:
     OrderTypesWithoutNone = Any
     OrderTypes = Any
     RngTypes = Any
```

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap/utils/validate.py` & `tsbootstrap-0.1.1/src/tsbootstrap/utils/validate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections.abc import Mapping
 from numbers import Integral
-from typing import Any, get_args
+from typing import Any, List, Optional, get_args
 
 import numpy as np
 from numpy.random import Generator
 from sklearn.utils import check_array
 
 from tsbootstrap.utils.odds_and_ends import check_generator
 from tsbootstrap.utils.types import FittedModelTypes, RngTypes
@@ -280,30 +280,30 @@
     if X.ndim == 1:  # and not model_is_var:
         X = X[:, np.newaxis]
     return X
 
 
 def validate_single_integer(
     value: Integral,
-    min_value: Integral = None,
-    max_value: Integral = None,
+    min_value: Optional[Integral] = None,
+    max_value: Optional[Integral] = None,
 ) -> None:
     """Validate a single integer value against an optional minimum value."""
     if not isinstance(value, Integral):
         raise TypeError(f"Input must be an integer. Got {value}.")
     if min_value is not None and value < min_value:
         raise ValueError(f"Integer must be at least {min_value}. Got {value}.")
     if max_value is not None and value > max_value:
         raise ValueError(f"Integer must be at most {max_value}. Got {value}.")
 
 
 def validate_list_of_integers(
     value,
-    min_value: Integral = None,
-    max_value: Integral = None,
+    min_value: Optional[Integral] = None,
+    max_value: Optional[Integral] = None,
 ) -> None:
     """Validate a list of integer values against an optional minimum value."""
     if not value:
         raise TypeError(f"List must not be empty. Got {value}.")
 
     if not all(isinstance(x, Integral) for x in value):
         raise TypeError(
@@ -319,16 +319,16 @@
         raise ValueError(
             f"All integers in the list must be at most {max_value}. Got {value}."
         )
 
 
 def validate_integer_array(
     value: np.ndarray,
-    min_value: Integral = None,
-    max_value: Integral = None,
+    min_value: Optional[Integral] = None,
+    max_value: Optional[Integral] = None,
 ) -> None:
     """Validate a 1D numpy array of integers against an optional minimum value."""
     if value.size == 0:
         raise TypeError(f"Array must not be empty. Got {value}.")
 
     if value.ndim != 1 or value.dtype.kind not in "iu":
         raise TypeError(
@@ -344,16 +344,16 @@
         raise ValueError(
             f"All integers in the array must be at most {max_value}. Got {value}."
         )
 
 
 def validate_integers(
     *values,
-    min_value: Integral = None,
-    max_value: Integral = None,
+    min_value: Optional[Integral] = None,
+    max_value: Optional[Integral] = None,
 ) -> None:
     """
     Validates that all input values are integers and optionally, above a minimum value.
 
     Each value can be an integer, a list of integers, or a 1D numpy array of integers.
     If min_value is provided, all integers must be greater than or equal to min_value.
 
@@ -384,15 +384,15 @@
                 f"Input must be an integer, a list of integers, or a 1D array of integers. Got {value}."
             )
 
 
 def validate_X(
     X: np.ndarray,
     model_is_var: bool,
-    allow_multi_column: bool = None,
+    allow_multi_column: Optional[bool] = None,
 ) -> np.ndarray:
     """
     Validate the input array X based on the given model type.
 
     Parameters
     ----------
     X : np.ndarray
@@ -457,15 +457,15 @@
         If `exog` contains fewer than two elements.
     """
     return validate_X(exog, model_is_var=False, allow_multi_column=True)
 
 
 def validate_X_and_y(
     X: np.ndarray,
-    y: np.ndarray,
+    y: Optional[np.ndarray],
     model_is_var: bool = False,
     model_is_arch: bool = False,
 ):
     """
     Validate and reshape input data and exogenous variables.
 
     This function uses :func:`validate_X` and :func:`validate_exog` to perform detailed validation.
@@ -504,15 +504,17 @@
         X = np.ascontiguousarray(X)
         if y is not None:
             y = np.ascontiguousarray(y)
 
     return X, y
 
 
-def validate_block_indices(block_indices, input_length: Integral) -> None:
+def validate_block_indices(
+    block_indices: List[np.ndarray], input_length: Integral
+) -> None:
     """
     Validate the input block indices. Each block index must be a 1D NumPy array with at least one index and all indices must be within the range of X.
 
     Parameters
     ----------
     block_indices : List[np.ndarray]
         The input block indices.
@@ -536,15 +538,15 @@
         block_indices, "block_indices"
     )
     block_indices = check_indices_within_range(
         block_indices, input_length, "block_indices"
     )
 
 
-def validate_blocks(blocks) -> None:
+def validate_blocks(blocks: List[np.ndarray]) -> None:
     """
     Validate the input blocks. Each block must be a 2D NumPy array with at least one element.
 
     Parameters
     ----------
     blocks : List[np.ndarray]
         The input blocks.
@@ -620,17 +622,17 @@
     """
     Validate the type of `input_value` against a Literal type or dictionary keys.
 
     Parameters
     ----------
     input_value : str
         The value to validate.
-    literal_type : type, or listt
+    literal_type : type, or list
         if type: Literal type or dictionary against which to validate the `input_value`.
-        if list: List of valid values against which to validate the `input_value`.
+        if list: list of valid values against which to validate the `input_value`.
 
     Raises
     ------
     TypeError
         If `input_value` is not a string.
     ValueError
         If `input_value` is not among the valid types in `literal_type` or dictionary keys.
@@ -658,15 +660,15 @@
 
     if input_value.lower() not in valid_types:
         raise ValueError(
             f"Invalid input_value '{input_value}'. Expected one of {', '.join(valid_types)}."
         )
 
 
-def validate_rng(rng: RngTypes, allow_seed: bool = True) -> Generator:
+def validate_rng(rng: RngTypes, allow_seed: bool = True) -> Generator:  # type: ignore
     """Validate the input random number generator.
 
     This function validates if the input random number generator is an instance of
     the numpy.random.Generator class or an integer. If allow_seed is True, the input
     can also be an integer, which will be used to seed the default random number
     generator.
```

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap.egg-info/PKG-INFO` & `tsbootstrap-0.1.1/src/tsbootstrap.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsbootstrap
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package to generate bootstrapped time series
 Author-email: Sankalp Gilda <sankalp.gilda@gmail.com>
 Maintainer-email: Sankalp Gilda <sankalp.gilda@gmail.com>, Franz Kiraly <franz.kiraly@sktime.net>, Benedikt Heidrich <benedikt.heidrich@sktime.net>
 License: MIT License
         
         Copyright (c) 2023 Sankalp Gilda
         
@@ -49,36 +49,48 @@
 Requires-Dist: packaging
 Provides-Extra: all-extras
 Requires-Dist: arch<6.0.0,>=5.0.0; extra == "all-extras"
 Requires-Dist: hmmlearn<0.3.2,>=0.3.0; extra == "all-extras"
 Requires-Dist: pyclustering<0.11.0,>=0.10.0; extra == "all-extras"
 Requires-Dist: scikit_learn_extra<0.4.0,>=0.3.0; extra == "all-extras"
 Requires-Dist: statsmodels<0.15.0,>=0.12.1; extra == "all-extras"
+Requires-Dist: dtaidistance; python_version < "3.10" and extra == "all-extras"
 Provides-Extra: docs
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: jupyter; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: nbsphinx>=0.8.6; extra == "docs"
 Requires-Dist: numpydoc; extra == "docs"
 Requires-Dist: pydata-sphinx-theme; extra == "docs"
 Requires-Dist: Sphinx!=7.2.0,<8.0.0; extra == "docs"
 Requires-Dist: sphinx-rtd-theme>=1.3.0; extra == "docs"
-Requires-Dist: sphinx-copybutton; extra == "docs"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "docs"
 Requires-Dist: sphinx-design<0.6.0; extra == "docs"
 Requires-Dist: sphinx-gallery<0.15.0; extra == "docs"
 Requires-Dist: sphinx-issues<4.0.0; extra == "docs"
 Requires-Dist: sphinx-version-warning; extra == "docs"
-Requires-Dist: tabulate; extra == "docs"
+Requires-Dist: tabulate>=0.9.0; extra == "docs"
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
+Requires-Dist: black>=24.3.0; extra == "dev"
 Requires-Dist: blacken-docs; extra == "dev"
 Requires-Dist: hypothesis; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: github-actions; extra == "dev"
+Requires-Dist: importlib-metadata; extra == "dev"
+Requires-Dist: pip-tools; extra == "dev"
+Requires-Dist: pyright; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: autoflake; extra == "dev"
+Requires-Dist: typos; extra == "dev"
+Requires-Dist: tox; extra == "dev"
+Requires-Dist: tox-gh-actions; extra == "dev"
+Requires-Dist: pycobertura; extra == "dev"
+Requires-Dist: tomlkit; extra == "dev"
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/github/all-contributors/astrogilda/tsbootstrap?color=ee8449&style=flat-square)](#contributors)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 
 <div align="center">
@@ -103,127 +115,117 @@
     <a href="https://pepy.tech/project/tsbootstrap">
         <img src="https://static.pepy.tech/badge/tsbootstrap" alt="Downloads"/>
     </a>
     <img src="https://img.shields.io/github/license/eli64s/readme-ai?color=5D6D7E" alt="github-license" />
     </a>
     <img src="https://github.com/astrogilda/tsbootstrap/workflows/CI/badge.svg" alt="Build Status"/>
     <a href="https://codecov.io/gh/astrogilda/tsbootstrap"><img src="https://codecov.io/gh/astrogilda/tsbootstrap/branch/main/graph/badge.svg" alt="codecov"/></a>
-    <a href="https://doi.org/10.5281/zenodo.8226496"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.8226496.svg" alt="DOI"/></a>
+    <a href="https://doi.org/10.5281/zenodo.8226495"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.8226495.svg" alt="DOI"/></a>
     <a href="https://codeclimate.com/github/astrogilda/tsbootstrap/maintainability"><img src="https://api.codeclimate.com/v1/badges/d80a0615a8c00f31565c/maintainability" alt="Code Quality"/></a>
     <img src="https://img.shields.io/github/last-commit/astrogilda/tsbootstrap" alt="Last Commit"/>
     <img src="https://img.shields.io/github/issues/astrogilda/tsbootstrap" alt="Issues"/>
     <img src="https://img.shields.io/github/issues-pr/astrogilda/tsbootstrap" alt="Pull Requests"/>
     <img src="https://img.shields.io/github/v/tag/astrogilda/tsbootstrap" alt="Tag"/>
 </div>
 
 
 
 ## 📒 Table of Contents
-1. [📍 Time Series Bootstrapping](#time-series-bootstrapping)
-    - [Overview](#overview)
-    - [Bootstrapping Methodology](#bootstrapping-methodology)
-    - [Block Bootstrap](#block-bootstrap)
-        - [Moving Block Bootstrap](#moving-block-bootstrap)
-        - [Circular Block Bootstrap](#circular-block-bootstrap)
-        - [Stationary Block Bootstrap](#stationary-block-bootstrap)
-        - [NonOverlapping Block Bootstrap](#nonoverlapping-block-bootstrap)
-        - [Bartletts Bootstrap](#bartletts-bootstrap)
-        - [Blackman Bootstrap](#blackman-bootstrap)
-        - [Hamming Bootstrap](#hamming-bootstrap)
-        - [Hanning Bootstrap](#hanning-bootstrap)
-        - [Tukey Bootstrap](#tukey-bootstrap)
-    - [Residual Bootstrap](#residual-bootstrap)
-    - [Bias Corrected Bootstrap](#bias-corrected-bootstrap)
-    - [Distribution Bootstrap](#distribution-bootstrap)
-    - [Markov Bootstrap](#markov-bootstrap)
-    - [Sieve Bootstrap](#sieve-bootstrap)
-3. [🧩 Modules](#-modules)
-4. [🚀 Getting Started](#-getting-started)
-5. [🗺 Roadmap](#-roadmap)
-6. [🤝 Contributing](#-contributing)
-7. [📄 License](#-license)
-8. [👏 Acknowledgments](#-acknowledgments)
 
+1. [🚀 Getting Started](#-getting-started)
+2. [🧩 Modules](#-modules)
+3. [🗺 Roadmap](#-roadmap)
+4. [🤝 Contributing](#-contributing)
+5. [📄 License](#-license)
+6. [📍 Time Series Bootstrapping Methods intro](#time-series-bootstrapping)
+7. [👏 Contributors](#-contributors)
 
----
 
 
-## 📍 Time Series Bootstrapping
-`tsbootstrap` is a comprehensive project designed to implement an array of bootstrapping techniques specifically tailored for time series data. This project is targeted towards data scientists, statisticians, economists, and other professionals or researchers who regularly work with time series data and require robust methods for generating bootstrapped copies of univariate and multivariate time series data.
+---
 
-### Overview
-Time series bootstrapping is a nuanced resampling method that is applied to time-dependent data. Traditional bootstrapping methods often assume independence between data points, which is an assumption that does not hold true for time series data where a data point is often dependent on previous data points. Time series bootstrapping techniques respect the chronological order and correlations of the data, providing more accurate estimates of uncertainty or variability.
+## 🚀 Getting Started
 
-### Bootstrapping Methodology
-The `tsbootstrap` project offers a diverse set of bootstrapping techniques that can be applied to either the entire input time series (classes prefixed with `Whole`), or after partitioning the data into blocks (classes prefixed with `Block`). These methodologies can be applied directly to the raw input data or to the residuals obtained after fitting one of the five statistical models defined in `time_series_model.py` (classes with `Residual` in their names).
 
-### Block Bootstrap
-Block Bootstrap is a prevalent approach in time series bootstrapping. It involves resampling blocks of consecutive data points, thus respecting the internal structures of the data. There are several techniques under Block Bootstrap, each with its unique approach. `tsbootstrap` provides highly flexible block bootstrapping, allowing the user to specify the block length sampling, block generation, and block resampling strategies. For additional details, refer to `block_length_sampler.py`, `block_generator.py`, and `block_resampler.py`.
+### 🎮 Using tsbootstrap
 
-The Moving Block Bootstrap, Circular Block Bootstrap, Stationary Block Bootstrap, and NonOverlapping Block Bootstrap methods are all variations of the Block Bootstrap that use different methods to sample the data, maintaining various types of dependencies.
+`tsbootstrap` provides a unified, `sklearn`-like interface to all bootstrap methods.
 
-Bartlett's, Blackman's, Hamming's, Hanning's, and Tukey's Bootstrap methods are specific implementations of the Block Bootstrap that use different window shapes to taper the data, reducing the influence of data points far from the center. In `tsbootstrap`, these methods inherit from `MovingBlockBootstrap`, but can easily be modified to inherit from any of the other three base block bootstrapping classes.
+Example using a `MovingBlockBootstrap` - all bootstrap algorithms follow
+the same interface!
 
-Each method comes with its distinct strengths and weaknesses. The choice of method should be based on the characteristics of the data and the specific requirements of the analysis.
+```python
+from tsbootstrap import MovingBlockBootstrap
+import numpy as np
 
-#### (i) Moving Block Bootstrap
-This method is implemented in `MovingBlockBootstrap` and is used for time series data where blocks of data are resampled to maintain the dependency structure within the blocks. It's useful when the data has dependencies that need to be preserved. It's not recommended when the data does not have any significant dependencies.
+# Create custom time series data. While below is for univariate time series, the bootstraps can handle multivariate time series as well.
+n_samples = 10
+X = np.arange(n_samples)
 
-#### (ii) Circular Block Bootstrap
-This method is implemented in `CircularBlockBootstrap` and treats the data as if it is circular (the end of the data is next to the beginning of the data). It's useful when the data is cyclical or seasonal in nature. It's not recommended when the data does not have a cyclical or seasonal component.
+# Instantiate the bootstrap object
+n_bootstraps = 3
+block_length = 3
+rng = 42
+mbb = MovingBlockBootstrap(n_bootstraps=n_bootstraps, rng=rng, block_length=block_length)
+
+# Generate bootstrapped samples
+return_indices = False
+bootstrapped_samples = mbb.bootstrap(
+    X, return_indices=return_indices)
+
+# Collect bootstrap samples
+X_bootstrapped = []
+for data in bootstrapped_samples:
+    X_bootstrapped.append(data)
 
-#### (iii) Stationary Block Bootstrap
-This method is implemented in `StationaryBlockBootstrap` and randomly resamples blocks of data with block lengths that follow a geometric distribution. It's useful for time series data where the degree of dependency needs to be preserved, and it doesn't require strict stationarity of the underlying process. It's not recommended when the data has strong seasonality or trend components which violate the weak dependence assumption.
+X_bootstrapped = np.array(X_bootstrapped)
+```
 
-#### (iv) NonOverlapping Block Bootstrap
- This method is implemented in `NonOverlappingBlockBootstrap` and resamples blocks of data without overlap. It's useful when the data has dependencies that need to be preserved and when overfitting is a concern. It's not recommended when the data does not have any significant dependencies or when the introduction of bias due to non-overlapping selection is a concern.
+### 📦 Installation and Setup
 
-#### (v) Bartlett's Bootstrap
- Bartlett's method is a time series bootstrap method that uses a window or filter that tapers off as you move away from the center of the window. It's useful when you have a large amount of data and you want to reduce the influence of the data points far away from the center. This method is not advised when the tapering of data points is not desired or when the dataset is small as the tapered data points might contain valuable information. It is implemented in `BartlettsBootstrap`.
+``tsbootstrap`` is installed via ``pip``, either from PyPI or locally.
 
-#### (vi) Blackman Bootstrap
-Similar to Bartlett's method, Blackman's method uses a window that tapers off as you move away from the center of the window. The key difference is the shape of the window (Blackman window has a different shape than Bartlett). It's useful when you want to reduce the influence of the data points far from the center with a different window shape. It's not recommended when the dataset is small or tapering of data points is not desired. It is implemented in `BlackmanBootstrap`.
+#### ✔️ Prerequisites
 
-#### (vii) Hamming Bootstrap
- Similar to the Bartlett and Blackman methods, the Hamming method uses a specific type of window function. It's useful when you want to reduce the influence of the data points far from the center with the Hamming window shape. It's not recommended for small datasets or when tapering of data points is not desired. It is implemented in `HammingBootstrap`.
+- Python (3.8 or higher)
+- `pip` (latest version recommended), plus suitable environment manager (`venv`, `conda`)
 
-#### (viii) Hanning Bootstrap
-This method also uses a specific type of window function. It's useful when you want to reduce the influence of the data points far from the center with the Hanning window shape. It's not recommended for small datasets or when tapering of data points is not desired. It is implemented in `HanningBootstrap`.
+You can also consider using ``uv`` to speed up environment setu.
 
-#### (ix) Tukey Bootstrap
-Similar to the Bartlett, Blackman, Hamming, and Hanning methods, the Tukey method uses a specific type of window function. It's useful when you want to reduce the influence of the data points far from the center with the Tukey window shape. It's not recommended for small datasets or when tapering of data points is not desired. It is implemented in `TukeyBootstrap`.
+#### Installing from PyPI
 
-### Residual Bootstrap
-Residual Bootstrap is a method designed for time series data where a model is fit to the data, and the residuals (the difference between the observed and predicted data) are bootstrapped. It's particularly useful when a good model fit is available for the data. However, it's not recommended when a model fit is not available or is poor. `tsbootstrap` provides four time series models to fit to the input data -- `AutoReg`, `ARIMA`, `SARIMA`, and `VAR` (for multivariate input time series data). For more details, refer to `time_series_model.py` and `tsfit.py`.
+To install the latest release of `tsbootstrap` directly from PyPI, run:
 
-### Statistic-Preserving Bootstrap
-Statistic-Preserving Bootstrap is a unique method designed to generate bootstrapped time series data while preserving a specific statistic of the original data. This method can be beneficial in scenarios where it's important to maintain the original data's characteristics in the bootstrapped samples. It is implemented in `StatisticPreservingBootstrap`.
+```sh
+pip install tsbootstrap
+```
 
-### Distribution Bootstrap
-Distribution Bootstrap generates bootstrapped samples by fitting a distribution to the residuals and then generating new residuals from the fitted distribution. The new residuals are then added to the fitted values to create the bootstrapped samples. This method is based on the assumption that the residuals follow a specific distribution (like Gaussian, Poisson, etc). It's not recommended when the distribution of residuals is unknown or hard to determine. It is implemented in `DistributionBootstrap`.
+To install with all optional dependencies:
 
-### Markov Bootstrap
-Markov Bootstrap is used for bootstrapping time series data where the residuals of the data are presumed to follow a Markov process. This method is especially useful in scenarios where the current residual primarily depends on the previous one, with little to no dependency on residuals from further in the past. Markov Bootstrap technique is designed to preserve this dependency structure in the bootstrapped samples, making it particularly valuable for time series data that exhibits Markov properties. However, it's not advisable when the residuals of the time series data exhibit long-range dependencies, as the Markov assumption of limited dependency may not hold true. It is implemented in `MarkovBootstrap`. See `markov_sampler.py` for implementation details.
+```
+pip install "tsbootstrap[all_extras]"
+```
+---
 
-### Sieve Bootstrap
-Sieve Bootstrap is designed for handling dependent data, where the residuals of the time series data follow an autoregressive process. This method aims to preserve and simulate the dependencies inherent in the original data within the bootstrapped samples. It operates by approximating the autoregressive process ofthe residuals using a finite order autoregressive model. The order of the model is determined based on the data, and the residuals are then bootstrapped. The Sieve Bootstrap technique is particularly valuable for time series data that exhibits autoregressive properties. However, it's not advisable when the residuals of the time series data do not follow an autoregressive process. It is implemented in `SieveBootstrap`. See `time_series_simulator.py` for implementations details.
+Bootstrap algorithms manage their own dependencies - if an extra is needed but not
+present, the object will raise this at construction.
 
 ## 🧩 Modules
 The `tsbootstrap` package contains various modules that handle tasks such as bootstrapping, time series simulation, and utility functions. This modular approach ensures flexibility, extensibility, and ease of maintenance.
 
 
 <details closed><summary>root</summary>
 
 | File                                                                                       | Summary                   |
 | ---                                                                                        | ---                       |
 | [setup.sh](https://github.com/astrogilda/tsbootstrap/blob/main/setup.sh)                         | Shell script for initial setup and environment configuration. |
 | [commitlint.config.js](https://github.com/astrogilda/tsbootstrap/blob/main/commitlint.config.js) | Configuration for enforcing conventional commit messages. |
 | [CITATION.cff](https://github.com/astrogilda/tsbootstrap/blob/main/CITATION.cff)                 | Citation metadata for the project. |
 | [CODE_OF_CONDUCT.md](https://github.com/astrogilda/tsbootstrap/blob/main/CODE_OF_CONDUCT.md)                 | Guidelines for community conduct and interactions. |
-| [CONTRIBUTING.md](https://github.com/astrogilda/tsbootstrap/blob/main/CITATION.md)                 | Instructions for contributing to the project. |
+| [CONTRIBUTING.md](https://github.com/astrogilda/tsbootstrap/blob/main/CONTRIBUTING.md)                 | Instructions for contributing to the project. |
 | [.codeclimate.yml](https://github.com/astrogilda/tsbootstrap/blob/main/.codeclimate.yml)                 | Configuration for Code Climate quality checks. |
 | [.gitignore](https://github.com/astrogilda/tsbootstrap/blob/main/.gitignore)                 | Specifies files and folders to be ignored by Git. |
 | [.pre-commit-config.yaml](https://github.com/astrogilda/tsbootstrap/blob/main/.pre-commit-config.yaml)                 | Configuration for pre-commit hooks. |
 | [poetry.toml](https://github.com/astrogilda/tsbootstrap/blob/main/poetry.toml)                 | Configuration file for Poetry package management. |
 | [tsbootstrap_logo.png](https://github.com/astrogilda/tsbootstrap/blob/main/tsbootstrap_logo.png)                 | Project logo image. |
 
 </details>
@@ -257,116 +259,76 @@
 | ---                                                                                                | ---                       |
 | [types.py](https://github.com/astrogilda/tsbootstrap/blob/main/src/tsbootstrap/utils/types.py)                 | Defines custom types used across the project. |
 | [validate.py](https://github.com/astrogilda/tsbootstrap/blob/main/src/tsbootstrap/utils/validate.py)           | Contains validation utilities. |
 | [odds_and_ends.py](https://github.com/astrogilda/tsbootstrap/blob/main/src/tsbootstrap/utils/odds_and_ends.py) | Contains miscellaneous utility functions. |
 
 </details>
 
----
 
-## 🚀 Getting Started
+## 🗺 Roadmap
 
-### ✔️ Prerequisites
+This is an abridged version; for the complete and evolving list of plans and improvements, see [Issue #144](https://github.com/astrogilda/tsbootstrap/issues/144).
 
-Before you begin, ensure that you have the following prerequisites installed:
-> - `ℹ️ Requirement 1`
-> - `ℹ️ Requirement 2`
-> - `ℹ️ ...`
+### Performance and Scaling
+ -handling large datasets, distributed backend integration (`Dask`, `Spark`, `Ray`), profiling/optimization
+### Tuning and AutoML
+ -adaptive block length, adaptive resampling, evaluation based parameter selection
+### Real-time and Stream Data
+ -stream bootstraps, data update interface
+### Stage 2 `sktime` Integration
+ -evaluation module, datasets, benchmarks, sktime forecasters in bootstraps
+### API and Capability Extension
+ -panel/hierarchical data, exogenous data, update/stream, model state management
+### Scope Extension (TBD)
+ -time series augmentation, fully probabilistic models
 
-### 📦 Installation and Setup
+## 🤝 Contributing
 
-This project comes with a `setup.sh` script to ease the setup process. The script will create a new Python virtual environment, install the necessary dependencies, and handle some version-specific installations.
+Contributions are always welcome!
 
-Here are the steps to follow:
+See our [good first issues ](https://github.com/astrogilda/tsbootstrap/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
+for getting started.
 
-1. Ensure that you have Python, Poetry, and Bash installed on your system. If not, you can install them using the links below:
-    - [Python](https://www.python.org/downloads/)
-    - [Poetry](https://python-poetry.org/docs/#installation)
-    - [Bash](https://www.gnu.org/software/bash/)
+Below is a quick start guide to contributing.
 
-2. Clone the tsbootstrap repository:
-```sh
-git clone https://github.com/astrogilda/tsbootstrap
-```
+### Developer setup
 
-3. Change to the project directory:
-```sh
-cd tsbootstrap
-```
+1. Fork the tsbootstrap repository
 
-4. Make the `setup.sh` script executable:
+2. Clone the fork to local:
 ```sh
-chmod +x setup.sh
+git clone https://github.com/astrogilda/tsbootstrap
 ```
 
-5. Run the `setup.sh` script:
-```sh
-./setup.sh
-```
+3. In the local repository root, set up a python environment, e.g., `venv` or `conda`.
 
-The `setup.sh` script sets up a Python environment using Poetry, locks and installs the necessary dependencies, and installs `dtaidistance` if the Python version is 3.9 or lower.
 
-6. Activate the python shell:
-```sh
-poetry shell
+4. Editable install via `pip`, including developer dependencies:
+```
+pip install -e .[dev]
 ```
 
-That's it! You are now set up and ready to go.
-
-### 🎮 Using tsbootstrap
-
-Here's a basic example using the Moving Block Bootstrap method:
-
-```python
-from tsbootstrap import MovingBlockBootstrap, MovingBlockBootstrapConfig
-import numpy as np
-
-np.random.seed(0)
-
-# Create custom time series data
-
-n_samples = 1000
-
-y = np.random.normal(0, 1, n_samples).cumsum()
-
-x1 = np.arange(1, n_samples + 1).reshape(-1, 1)
-x2 = np.random.normal(0, 1, (n_samples, 1))
-exog = np.concatenate([x1, x2], axis=1)
+The editable install ensures that changes to the package are reflected in
+your environment.
 
-# Instantiate the bootstrap object
-mbb_config = MovingBlockBootstrapConfig(
-    n_bootstraps=1000, rng=42, block_length=10
-)
-mbb = MovingBlockBootstrap(config=mbb_config)
+### Verifying the Installation
 
-# Generate the generator for 1000 bootstrapped samples
-bootstrapped_samples = bootstrap.bootstrap(n=1000)
+After installation, you can verify that tsbootstrap has been installed correctly by checking its version or by trying to import it in Python:
 ```
-
-### 🧪 Running Tests
-```sh
-pytest tests/
+python -c "import tsbootstrap; print(tsbootstrap.__version__)"
 ```
 
----
-
-
-## 🗺 Roadmap
-
-> - [ ] `ℹ️  Task 1: in distributionbootstrap, allow mixture of distributions`
-> - [ ] `ℹ️  Task 2: allow fractional block_length`
-> - [ ] `ℹ️  Task 3: enable multi-processing`
-> - [ ] `ℹ️  Task 4: test -- for biascorrectblockbootstrap, see if the statistic on the bootstrapped sample is close to the statistic on the original sample`
+This command should output the version number of tsbootstrap without any errors, indicating that the installation was successful.
 
+That's it! You are now set up and ready to go. You can start using tsbootstrap for your time series bootstrapping needs.
 
-## 🤝 Contributing
+### Contribution workflow
 
 Contributions are always welcome! Please follow these steps:
-1. Fork the project repository. This creates a copy of the project on your account that you can modify without affecting the original project.
-2. Clone the forked repository to your local machine using a Git client like Git or GitHub Desktop.
+
 3. Create a new branch with a descriptive name (e.g., `new-feature-branch` or `bugfix-issue-123`).
 ```sh
 git checkout -b new-feature-branch
 ```
 4. Make changes to the project's codebase.
 5. Commit your changes to your local branch with a clear commit message that explains the changes you've made.
 ```sh
@@ -375,14 +337,33 @@
 6. Push your changes to your forked repository on GitHub using the following command
 ```sh
 git push origin new-feature-branch
 ```
 7. Create a new pull request to the original project repository. In the pull request, describe the changes you've made and why they're necessary.
 The project maintainers will review your changes and provide feedback or merge them into the main branch.
 
+### 🧪 Running Tests
+
+To run all tests, in your developer environment, run:
+
+```sh
+pytest tests/
+```
+
+Individual bootstrap algorithms can be tested as follows:
+
+```python
+from tsbootstrap.utils import check_estimator
+
+check_estimator(my_bootstrap_algo)
+```
+
+### Contribution guide
+
+For more detailed information on how to contribute, please refer to our [CONTRIBUTING.md](https://github.com/astrogilda/tsbootstrap/blob/main/CONTRIBUTING.md)  guide.
 ---
 
 ## 📄 License
 
 This project is licensed under the `ℹ️  MIT` License. See the [LICENSE](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository) file for additional info.
 
 ---
@@ -396,7 +377,71 @@
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+
+
+---
+
+
+## 📍 Time Series Bootstrapping
+`tsbootstrap` is a comprehensive project designed to implement an array of bootstrapping techniques specifically tailored for time series data. This project is targeted towards data scientists, statisticians, economists, and other professionals or researchers who regularly work with time series data and require robust methods for generating bootstrapped copies of univariate and multivariate time series data.
+
+### Overview
+Time series bootstrapping is a nuanced resampling method that is applied to time-dependent data. Traditional bootstrapping methods often assume independence between data points, which is an assumption that does not hold true for time series data where a data point is often dependent on previous data points. Time series bootstrapping techniques respect the chronological order and correlations of the data, providing more accurate estimates of uncertainty or variability.
+
+### Bootstrapping Methodology
+The `tsbootstrap` project offers a diverse set of bootstrapping techniques that can be applied to either the entire input time series (classes prefixed with `Whole`), or after partitioning the data into blocks (classes prefixed with `Block`). These methodologies can be applied directly to the raw input data or to the residuals obtained after fitting one of the five statistical models defined in `time_series_model.py` (classes with `Residual` in their names).
+
+### Block Bootstrap
+Block Bootstrap is a prevalent approach in time series bootstrapping. It involves resampling blocks of consecutive data points, thus respecting the internal structures of the data. There are several techniques under Block Bootstrap, each with its unique approach. `tsbootstrap` provides highly flexible block bootstrapping, allowing the user to specify the block length sampling, block generation, and block resampling strategies. For additional details, refer to `block_length_sampler.py`, `block_generator.py`, and `block_resampler.py`.
+
+The Moving Block Bootstrap, Circular Block Bootstrap, Stationary Block Bootstrap, and NonOverlapping Block Bootstrap methods are all variations of the Block Bootstrap that use different methods to sample the data, maintaining various types of dependencies.
+
+Bartlett's, Blackman's, Hamming's, Hanning's, and Tukey's Bootstrap methods are specific implementations of the Block Bootstrap that use different window shapes to taper the data, reducing the influence of data points far from the center. In `tsbootstrap`, these methods inherit from `MovingBlockBootstrap`, but can easily be modified to inherit from any of the other three base block bootstrapping classes.
+
+Each method comes with its distinct strengths and weaknesses. The choice of method should be based on the characteristics of the data and the specific requirements of the analysis.
+
+#### (i) Moving Block Bootstrap
+This method is implemented in `MovingBlockBootstrap` and is used for time series data where blocks of data are resampled to maintain the dependency structure within the blocks. It's useful when the data has dependencies that need to be preserved. It's not recommended when the data does not have any significant dependencies.
+
+#### (ii) Circular Block Bootstrap
+This method is implemented in `CircularBlockBootstrap` and treats the data as if it is circular (the end of the data is next to the beginning of the data). It's useful when the data is cyclical or seasonal in nature. It's not recommended when the data does not have a cyclical or seasonal component.
+
+#### (iii) Stationary Block Bootstrap
+This method is implemented in `StationaryBlockBootstrap` and randomly resamples blocks of data with block lengths that follow a geometric distribution. It's useful for time series data where the degree of dependency needs to be preserved, and it doesn't require strict stationarity of the underlying process. It's not recommended when the data has strong seasonality or trend components which violate the weak dependence assumption.
+
+#### (iv) NonOverlapping Block Bootstrap
+ This method is implemented in `NonOverlappingBlockBootstrap` and resamples blocks of data without overlap. It's useful when the data has dependencies that need to be preserved and when overfitting is a concern. It's not recommended when the data does not have any significant dependencies or when the introduction of bias due to non-overlapping selection is a concern.
+
+#### (v) Bartlett's Bootstrap
+ Bartlett's method is a time series bootstrap method that uses a window or filter that tapers off as you move away from the center of the window. It's useful when you have a large amount of data and you want to reduce the influence of the data points far away from the center. This method is not advised when the tapering of data points is not desired or when the dataset is small as the tapered data points might contain valuable information. It is implemented in `BartlettsBootstrap`.
+
+#### (vi) Blackman Bootstrap
+Similar to Bartlett's method, Blackman's method uses a window that tapers off as you move away from the center of the window. The key difference is the shape of the window (Blackman window has a different shape than Bartlett). It's useful when you want to reduce the influence of the data points far from the center with a different window shape. It's not recommended when the dataset is small or tapering of data points is not desired. It is implemented in `BlackmanBootstrap`.
+
+#### (vii) Hamming Bootstrap
+ Similar to the Bartlett and Blackman methods, the Hamming method uses a specific type of window function. It's useful when you want to reduce the influence of the data points far from the center with the Hamming window shape. It's not recommended for small datasets or when tapering of data points is not desired. It is implemented in `HammingBootstrap`.
+
+#### (viii) Hanning Bootstrap
+This method also uses a specific type of window function. It's useful when you want to reduce the influence of the data points far from the center with the Hanning window shape. It's not recommended for small datasets or when tapering of data points is not desired. It is implemented in `HanningBootstrap`.
+
+#### (ix) Tukey Bootstrap
+Similar to the Bartlett, Blackman, Hamming, and Hanning methods, the Tukey method uses a specific type of window function. It's useful when you want to reduce the influence of the data points far from the center with the Tukey window shape. It's not recommended for small datasets or when tapering of data points is not desired. It is implemented in `TukeyBootstrap`.
+
+### Residual Bootstrap
+Residual Bootstrap is a method designed for time series data where a model is fit to the data, and the residuals (the difference between the observed and predicted data) are bootstrapped. It's particularly useful when a good model fit is available for the data. However, it's not recommended when a model fit is not available or is poor. `tsbootstrap` provides four time series models to fit to the input data -- `AutoReg`, `ARIMA`, `SARIMA`, and `VAR` (for multivariate input time series data). For more details, refer to `time_series_model.py` and `tsfit.py`.
+
+### Statistic-Preserving Bootstrap
+Statistic-Preserving Bootstrap is a unique method designed to generate bootstrapped time series data while preserving a specific statistic of the original data. This method can be beneficial in scenarios where it's important to maintain the original data's characteristics in the bootstrapped samples. It is implemented in `StatisticPreservingBootstrap`.
+
+### Distribution Bootstrap
+Distribution Bootstrap generates bootstrapped samples by fitting a distribution to the residuals and then generating new residuals from the fitted distribution. The new residuals are then added to the fitted values to create the bootstrapped samples. This method is based on the assumption that the residuals follow a specific distribution (like Gaussian, Poisson, etc). It's not recommended when the distribution of residuals is unknown or hard to determine. It is implemented in `DistributionBootstrap`.
+
+### Markov Bootstrap
+Markov Bootstrap is used for bootstrapping time series data where the residuals of the data are presumed to follow a Markov process. This method is especially useful in scenarios where the current residual primarily depends on the previous one, with little to no dependency on residuals from further in the past. Markov Bootstrap technique is designed to preserve this dependency structure in the bootstrapped samples, making it particularly valuable for time series data that exhibits Markov properties. However, it's not advisable when the residuals of the time series data exhibit long-range dependencies, as the Markov assumption of limited dependency may not hold true. It is implemented in `MarkovBootstrap`. See `markov_sampler.py` for implementation details.
+
+### Sieve Bootstrap
+Sieve Bootstrap is designed for handling dependent data, where the residuals of the time series data follow an autoregressive process. This method aims to preserve and simulate the dependencies inherent in the original data within the bootstrapped samples. It operates by approximating the autoregressive process ofthe residuals using a finite order autoregressive model. The order of the model is determined based on the data, and the residuals are then bootstrapped. The Sieve Bootstrap technique is particularly valuable for time series data that exhibits autoregressive properties. However, it's not advisable when the residuals of the time series data do not follow an autoregressive process. It is implemented in `SieveBootstrap`. See `time_series_simulator.py` for implementations details.
```

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap.egg-info/SOURCES.txt` & `tsbootstrap-0.1.1/src/tsbootstrap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tsbootstrap-0.1.0/src/tsbootstrap.egg-info/requires.txt` & `tsbootstrap-0.1.1/src/tsbootstrap.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,50 @@
 numpy<1.27,>=1.21
 scikit-base<0.8.0,>=0.6.1
 scikit-learn<1.5.0,>=0.24
 scipy<2.0.0,>=1.2
 packaging
 
-[all_extras]
+[all-extras]
 arch<6.0.0,>=5.0.0
 hmmlearn<0.3.2,>=0.3.0
 pyclustering<0.11.0,>=0.10.0
 scikit_learn_extra<0.4.0,>=0.3.0
 statsmodels<0.15.0,>=0.12.1
 
+[all-extras:python_version < "3.10"]
+dtaidistance
+
 [dev]
-black
+black>=24.3.0
 blacken-docs
 hypothesis
 pre-commit
 pytest
 pytest-cov
+github-actions
+importlib-metadata
+pip-tools
+pyright
+ruff
+autoflake
+typos
+tox
+tox-gh-actions
+pycobertura
+tomlkit
 
 [docs]
 furo
 jupyter
 myst-parser
 nbsphinx>=0.8.6
 numpydoc
 pydata-sphinx-theme
 Sphinx!=7.2.0,<8.0.0
 sphinx-rtd-theme>=1.3.0
-sphinx-copybutton
+sphinx-copybutton>=0.5.2
 sphinx-design<0.6.0
 sphinx-gallery<0.15.0
 sphinx-issues<4.0.0
 sphinx-version-warning
-tabulate
+tabulate>=0.9.0
```

### Comparing `tsbootstrap-0.1.0/tests/test_base_bootstrap_configs.py` & `tsbootstrap-0.1.1/tests/test_base_bootstrap_configs.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,14 @@
                 _ = BaseResidualBootstrapConfig(model_type=model_type)
 
         @given(order=one_of(text(), lists(text(), min_size=1), floats()))
         def test_invalid_order_type(self, order) -> None:
             """
             Test if the BaseResidualBootstrapConfig raises a TypeError when order is not an integer, list of integers, or None.
             """
-            print(order)
             with pytest.raises(TypeError):
                 _ = BaseResidualBootstrapConfig(order=order)
 
         @given(order=integers(max_value=0))
         def test_invalid_order_value(self, order) -> None:
             """
             Test if the BaseResidualBootstrapConfig raises a ValueError when order is less than or equal to 0.
```

### Comparing `tsbootstrap-0.1.0/tests/test_block_bootstrap.py` & `tsbootstrap-0.1.1/tests/test_block_bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,16 +177,15 @@
                 rng=rng,
             )
 
             assert isinstance(
                 bootstrap.bootstrap_instance,
                 BLOCK_BOOTSTRAP_TYPES_DICT[bootstrap_type],
             )
-            print(f"bootstrap_type from test: {bootstrap_type}\n")
-            print(f"block_length from test: {block_length}\n")
+
             # Check that bootstrap method runs without errors
             _ = list(bootstrap.bootstrap(np.array(X)))
 
             # Check that _generate_samples_single_bootstrap method runs without errors
             _ = bootstrap._generate_samples_single_bootstrap(X=np.array(X))
 
     class TestFailingCases:
```

### Comparing `tsbootstrap-0.1.0/tests/test_block_bootstrap_configs.py` & `tsbootstrap-0.1.1/tests/test_block_bootstrap_configs.py`

 * *Files identical despite different names*

### Comparing `tsbootstrap-0.1.0/tests/test_block_generator.py` & `tsbootstrap-0.1.1/tests/test_block_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
         ):
             """
             Test BlockGenerator initialization with valid arguments.
             """
             block_length_sampler = BlockLengthSampler(
                 avg_block_length=avg_block_length
             )
-            print(f"block_length_sampler.type: {type(block_length_sampler)}")
             rng = default_rng()
 
             block_generator = BlockGenerator(
                 block_length_sampler,
                 input_length,
                 wrap_around_flag,
                 rng,
@@ -51,15 +50,17 @@
                 min_block_length=min_block_length,
             )
 
             assert block_generator.block_length_sampler == block_length_sampler
             assert block_generator.input_length == input_length
             assert block_generator.wrap_around_flag == wrap_around_flag
             assert block_generator.rng == rng
-            assert block_generator.overlap_length == overlap_length
+            assert block_generator.overlap_length == min(
+                overlap_length, input_length - 1
+            )
             assert block_generator.min_block_length == min(
                 min_block_length, avg_block_length
             )
 
     class TestFailingCases:
         """
         Test class for failing tests of BlockGenerator __init__ method.
@@ -416,15 +417,14 @@
                 input_length=input_length,
                 wrap_around_flag=wrap_around_flag,
                 overlap_length=overlap_length,
                 min_block_length=min_block_length,
             )
             generated_blocks = block_generator.generate_overlapping_blocks()
 
-            print(f"generated_blocks: {generated_blocks}")
             assert len(generated_blocks) == len(expected_output)
 
             if not wrap_around_flag:
                 for gb, eo in zip(generated_blocks, expected_output):
                     assert np.array_equal(gb, eo)
 
             assert_unique_arrays(generated_blocks)
```

### Comparing `tsbootstrap-0.1.0/tests/test_block_length_sampler.py` & `tsbootstrap-0.1.1/tests/test_block_length_sampler.py`

 * *Files identical despite different names*

### Comparing `tsbootstrap-0.1.0/tests/test_block_resampler.py` & `tsbootstrap-0.1.1/tests/test_block_resampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     overlap_length=st.integers(min_value=1, max_value=2),
     min_block_length=st.integers(min_value=2, max_value=2),
     avg_block_length=st.integers(min_value=3, max_value=10),
     overlap_flag=st.booleans(),
 )
 
 
-def weights_func(size: int):
+def weights_func(size: int) -> np.ndarray:
     return np.random.uniform(low=0, high=1e6, size=size)
 
 
 class TestInit:
     """Test the __init__ method."""
 
     class TestPassingCases:
@@ -90,16 +90,14 @@
             assert len(br.block_weights) == len(X)
 
             assert isinstance(br.tapered_weights, list)
             assert all(
                 isinstance(br.tapered_weights[i], np.ndarray)
                 for i in range(len(blocks))
             )
-            pprint(f"br.tapered_weights:{br.tapered_weights}")
-            print("\n")
             if tapered_weights is None:
                 assert all(
                     np.isclose(
                         br.tapered_weights[i].sum(), len(br.tapered_weights[i])
                     )
                     for i in range(len(blocks))
                 )
@@ -359,32 +357,22 @@
             # Check that the length of new_blocks and new_tapered_weights are equal.
             assert len(new_blocks) == len(new_tapered_weights)
 
             # We set the len(blocks) to be 5, so we can minimize the chances that resampling blocks a second time, or with a different random seed, gives the same results.
             if len(blocks) > 1:
                 # Check that resampling with the same random seed, a second time, gives different results.
                 new_blocks_2, new_tapered_weights_2 = br.resample_blocks()
-                print(f"X.shape: {X.shape}")
-                print(f"blocks: {blocks}")
-                print(f"new_blocks: {new_blocks}")
-                print(f"new_blocks_2: {new_blocks_2}")
-                print("\n")
                 check_list_of_arrays_equality(
                     new_blocks, new_blocks_2, equal=False
                 )
 
                 # Check that resampling with a new random seed gives different results.
                 rng2 = np.random.default_rng((random_seed + 1) * 2)
                 br = BlockResampler(blocks, X, rng=rng2)
                 new_blocks_3, new_tapered_weights_3 = br.resample_blocks()
-                print(f"X.shape: {X.shape}")
-                print(f"blocks: {blocks}")
-                print(f"new_blocks: {new_blocks}")
-                print(f"new_blocks_2: {new_blocks_2}")
-                print("\n")
                 check_list_of_arrays_equality(
                     new_blocks, new_blocks_3, equal=False
                 )
 
                 # Check that resampling with the same random seed gives the same results.
                 rng = np.random.default_rng(random_seed)
                 br = BlockResampler(blocks, X, rng=rng)
@@ -440,39 +428,36 @@
             # We set the len(blocks) to be 5, so we can minimize the chances that resampling blocks a second time, or with a different random seed, gives the same results.
             if len(blocks) > 1:
                 # Check that resampling with the same random seed, a second time, gives different results.
                 (
                     new_blocks_2,
                     block_data_2,
                 ) = br.resample_block_indices_and_data()
-                print(f"blocks: {blocks}")
                 check_list_of_arrays_equality(
                     new_blocks, new_blocks_2, equal=False
                 )
 
                 # Check that resampling with a new random seed gives different results.
                 rng2 = np.random.default_rng((random_seed + 1) * 2)
                 br = BlockResampler(blocks, X, rng=rng2)
                 (
                     new_blocks_3,
                     block_data_3,
                 ) = br.resample_block_indices_and_data()
-                print(f"blocks: {blocks}")
                 check_list_of_arrays_equality(
                     new_blocks, new_blocks_3, equal=False
                 )
 
                 # Check that resampling with the same random seed gives the same results.
                 rng = np.random.default_rng(random_seed)
                 br = BlockResampler(blocks, X, rng=rng)
                 (
                     new_blocks_4,
                     block_data_4,
                 ) = br.resample_block_indices_and_data()
-                print(f"blocks: {blocks}")
                 check_list_of_arrays_equality(new_blocks, new_blocks_4)
 
     class TestFailingCases:
         """Test cases where resample_block_indices_and_data should raise exceptions."""
 
         pass
```

### Comparing `tsbootstrap-0.1.0/tests/test_bootstrap.py` & `tsbootstrap-0.1.1/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `tsbootstrap-0.1.0/tests/test_markov_sampler.py` & `tsbootstrap-0.1.1/tests/test_markov_sampler.py`

 * *Files identical despite different names*

### Comparing `tsbootstrap-0.1.0/tests/test_odds_and_ends.py` & `tsbootstrap-0.1.1/tests/test_odds_and_ends.py`

 * *Files identical despite different names*

### Comparing `tsbootstrap-0.1.0/tests/test_ranklags.py` & `tsbootstrap-0.1.1/tests/test_ranklags.py`

 * *Files identical despite different names*

### Comparing `tsbootstrap-0.1.0/tests/test_time_series_model.py` & `tsbootstrap-0.1.1/tests/test_time_series_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     "order", [1, 2, 10, 50, 99, [1, 3], [2, 5, 10], [1, 10, 50]]
 )
 def test_fit_ar(input_1d, exog_1d, order):
     # Test with no exog, seasonal order, and set trend to 'c' (constant, default)
     from statsmodels.tsa.ar_model import AutoRegResultsWrapper
 
     max_lag = (input_1d.shape[0] - 1) // 2
-    print(f"max_lag: {max_lag}")
     tsm = TimeSeriesModel(X=input_1d, y=None, model_type="ar")
     tsm_exog = TimeSeriesModel(X=input_1d, y=exog_1d, model_type="ar")
     if np.max(order) <= max_lag:
         model_fit = tsm.fit(order=order)
         assert isinstance(model_fit, AutoRegResultsWrapper)
 
         # Test with exog
```

### Comparing `tsbootstrap-0.1.0/tests/test_time_series_simulator.py` & `tsbootstrap-0.1.1/tests/test_time_series_simulator.py`

 * *Files 7% similar despite different names*

```diff
@@ -354,14 +354,19 @@
             | st.just(default_rng()),
         )
         def test_rng_valid(self, fitted_model, X_fitted, rng):
             """Test that ARIMA model rng property getter and setter work correctly."""
             simulator = TimeSeriesSimulator(fitted_model, X_fitted, rng)
             assert isinstance(simulator.rng, Generator)
 
+        @settings(
+            suppress_health_check=(HealthCheck.too_slow,),
+            max_examples=10,
+            deadline=None,
+        )
         @given(
             fitted_model=arima_model_strategy(),
             X_fitted=float_array,
             rng=st.none()
             | st.integers(min_value=MIN_INT, max_value=MAX_INT)
             | st.just(default_rng()),
         )
@@ -423,61 +428,70 @@
 
 @pytest.mark.skipif(
     not _check_soft_dependencies("statsmodels", severity="none"),
     reason="skip test if required soft dependency not available",
 )
 class TestSARIMAModel:
     class TestPassingCases:
+        @settings(suppress_health_check=(HealthCheck.too_slow,))
         @given(
             fitted_model=sarima_model_strategy(),
             X_fitted=float_array,
             rng=st.none()
             | st.integers(min_value=MIN_INT, max_value=MAX_INT)
             | st.just(default_rng()),
         )
         def test_init_valid(self, fitted_model, X_fitted, rng):
             """Test that SARIMA model initialization works with valid inputs."""
             TimeSeriesSimulator(fitted_model, X_fitted, rng)
 
+        @settings(suppress_health_check=(HealthCheck.too_slow,))
         @given(
             fitted_model=sarima_model_strategy(),
             X_fitted=float_array,
             rng=st.none()
             | st.integers(min_value=MIN_INT, max_value=MAX_INT)
             | st.just(default_rng()),
         )
         def test_fitted_model_valid(self, fitted_model, X_fitted, rng):
             """Test that SARIMA model fitted_model property getter and setter work correctly."""
             simulator = TimeSeriesSimulator(fitted_model, X_fitted, rng)
             assert simulator.fitted_model == fitted_model
 
+        @settings(suppress_health_check=(HealthCheck.too_slow,))
         @given(
             fitted_model=sarima_model_strategy(),
             X_fitted=float_array,
             rng=st.none()
             | st.integers(min_value=MIN_INT, max_value=MAX_INT)
             | st.just(default_rng()),
         )
         def test_X_fitted_valid(self, fitted_model, X_fitted, rng):
             """Test that SARIMA model X_fitted property getter and setter work correctly."""
             simulator = TimeSeriesSimulator(fitted_model, X_fitted, rng)
             assert np.allclose(simulator.X_fitted, X_fitted)
 
+        @settings(suppress_health_check=(HealthCheck.too_slow,))
         @given(
             fitted_model=sarima_model_strategy(),
             X_fitted=float_array,
             rng=st.none()
             | st.integers(min_value=MIN_INT, max_value=MAX_INT)
             | st.just(default_rng()),
         )
         def test_rng_valid(self, fitted_model, X_fitted, rng):
             """Test that SARIMA model rng property getter and setter work correctly."""
             simulator = TimeSeriesSimulator(fitted_model, X_fitted, rng)
             assert isinstance(simulator.rng, Generator)
 
+        @settings(
+            suppress_health_check=(HealthCheck.too_slow,),
+            max_examples=10,
+            deadline=None,
+        )
         @given(
             fitted_model=sarima_model_strategy(),
             X_fitted=float_array,
             rng=st.none()
             | st.integers(min_value=MIN_INT, max_value=MAX_INT)
             | st.just(default_rng()),
         )
@@ -573,29 +587,31 @@
             | st.just(default_rng()),
         )
         def test_rng_valid(self, fitted_model, X_fitted, rng):
             """Test that VAR model rng property getter and setter work correctly."""
             simulator = TimeSeriesSimulator(fitted_model, X_fitted, rng)
             assert isinstance(simulator.rng, Generator)
 
+        @settings(
+            suppress_health_check=(HealthCheck.too_slow,),
+            max_examples=10,
+            deadline=None,
+        )
         @given(
             fitted_model=var_model_strategy(),
             X_fitted=float_array.map(lambda x: np.column_stack([x, x])),
             rng=st.none()
             | st.integers(min_value=MIN_INT, max_value=MAX_INT)
             | st.just(default_rng()),
         )
         def test_simulate_non_ar_process_valid(
             self, fitted_model, X_fitted, rng
         ):
             """Test that VAR model simulation works with valid inputs."""
-            print(f"X_fitted.shape = {X_fitted.shape}")
             simulator = TimeSeriesSimulator(fitted_model, X_fitted, rng)
-            print(f"simulator.X_fitted.shape = {simulator.X_fitted.shape}")
-            print(f"simulator.burnin = {simulator.burnin}")
             simulator.simulate_non_ar_process()
 
         @given(
             fitted_model=var_model_strategy(),
             X_fitted=float_array.map(lambda x: np.column_stack([x, x])),
         )
         def test_simulate_non_ar_same_rng(self, fitted_model, X_fitted):
@@ -606,17 +622,14 @@
             simulator1 = TimeSeriesSimulator(fitted_model, X_fitted, rng1)
             simulated_series1 = simulator1.simulate_non_ar_process()
 
             rng2 = np.random.default_rng(rng_seed)
             simulator2 = TimeSeriesSimulator(fitted_model, X_fitted, rng2)
             simulated_series2 = simulator2.simulate_non_ar_process()
 
-            print(f"simulated_series1 = {simulated_series1}")
-            print(f"simulated_series2 = {simulated_series2}")
-            print("\n")
             assert_arrays_compare(simulated_series1, simulated_series2)
 
         @given(
             fitted_model=var_model_strategy(),
             X_fitted=float_array.map(lambda x: np.column_stack([x, x])),
         )
         def test_simulate_non_ar_different_rng(self, fitted_model, X_fitted):
@@ -654,61 +667,70 @@
 
 @pytest.mark.skipif(
     not _check_soft_dependencies("arch", severity="none"),
     reason="skip test if required soft dependency not available",
 )
 class TestARCHModel:
     class TestPassingCases:
+        @settings(suppress_health_check=(HealthCheck.too_slow,))
         @given(
             fitted_model=arch_model_strategy(),
             X_fitted=float_array,
             rng=st.none()
             | st.integers(min_value=MIN_INT, max_value=MAX_INT)
             | st.just(default_rng()),
         )
         def test_init_valid(self, fitted_model, X_fitted, rng):
             """Test that ARCH model initialization works with valid inputs."""
             TimeSeriesSimulator(fitted_model, X_fitted, rng)
 
+        @settings(suppress_health_check=(HealthCheck.too_slow,))
         @given(
             fitted_model=arch_model_strategy(),
             X_fitted=float_array,
             rng=st.none()
             | st.integers(min_value=MIN_INT, max_value=MAX_INT)
             | st.just(default_rng()),
         )
         def test_fitted_model_valid(self, fitted_model, X_fitted, rng):
             """Test that ARCH model fitted_model property getter and setter work correctly."""
             simulator = TimeSeriesSimulator(fitted_model, X_fitted, rng)
             assert simulator.fitted_model == fitted_model
 
+        @settings(suppress_health_check=(HealthCheck.too_slow,))
         @given(
             fitted_model=arch_model_strategy(),
             X_fitted=float_array,
             rng=st.none()
             | st.integers(min_value=MIN_INT, max_value=MAX_INT)
             | st.just(default_rng()),
         )
         def test_X_fitted_valid(self, fitted_model, X_fitted, rng):
             """Test that ARCH model X_fitted property getter and setter work correctly."""
             simulator = TimeSeriesSimulator(fitted_model, X_fitted, rng)
             assert np.allclose(simulator.X_fitted, X_fitted)
 
+        @settings(suppress_health_check=(HealthCheck.too_slow,))
         @given(
             fitted_model=arch_model_strategy(),
             X_fitted=float_array,
             rng=st.none()
             | st.integers(min_value=MIN_INT, max_value=MAX_INT)
             | st.just(default_rng()),
         )
         def test_rng_valid(self, fitted_model, X_fitted, rng):
             """Test that ARCH model rng property getter and setter work correctly."""
             simulator = TimeSeriesSimulator(fitted_model, X_fitted, rng)
             assert isinstance(simulator.rng, Generator)
 
+        @settings(
+            suppress_health_check=(HealthCheck.too_slow,),
+            max_examples=10,
+            deadline=None,
+        )
         @given(
             fitted_model=arch_model_strategy(),
             X_fitted=float_array,
             rng=st.none()
             | st.integers(min_value=MIN_INT, max_value=MAX_INT)
             | st.just(default_rng()),
         )
@@ -738,14 +760,15 @@
             print(f"simulated_series2 = {simulated_series2}")
             print("\n")
             assert_arrays_compare(
                 simulated_series1, simulated_series2)
         '''
 
     class TestFailingCases:
+        @settings(suppress_health_check=(HealthCheck.too_slow,))
         @given(
             fitted_model=st.none() | st.integers() | st.floats() | st.text(),
             X_fitted=float_array,
             rng=st.none()
             | st.integers(min_value=MIN_INT, max_value=MAX_INT)
             | st.just(default_rng()),
         )
@@ -768,14 +791,15 @@
             suppress_health_check=[HealthCheck.too_slow],
         )
         def test_init_invalid_X_fitted(self, fitted_model, X_fitted, rng):
             """Test that ARCH model initialization fails with invalid X_fitted."""
             with pytest.raises(TypeError):
                 TimeSeriesSimulator(fitted_model, X_fitted, rng)
 
+        @settings(suppress_health_check=(HealthCheck.too_slow,))
         @given(
             fitted_model=arch_model_strategy(),
             X_fitted=float_array,
             rng=st.floats() | st.text(),
         )
         def test_init_invalid_rng(self, fitted_model, X_fitted, rng):
             """Test that ARCH model initialization fails with invalid rng."""
```

### Comparing `tsbootstrap-0.1.0/tests/test_tsfit.py` & `tsbootstrap-0.1.1/tests/test_tsfit.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,16 +419,14 @@
                             pass
                         else:
                             raise
             else:
                 if not is_data_var_zero and not is_exog_var_zero:
                     fitted_model = tsfit.fit(data, y=exog)
                     predicted = fitted_model.predict(data, n_steps=5)
-                    print(f"predicted.type: {type(predicted)}")
-                    print(f"predicted: {predicted}")
                     assert isinstance(predicted, np.ndarray)
                     assert predicted.shape == (5,)
 
         @settings(deadline=None)
         @given(
             data=test_data,
             order=ar_order_strategy,
@@ -493,15 +491,14 @@
             model_type=sampled_from(["var", "arch"]),
             exog=exog_strategy,
         )
         def test_get_residuals_valid_var_arch(
             self, data, order, model_type, exog
         ):
             """Test TSFit get_residuals method with valid inputs and model_type = 'var' or 'arch'."""
-            print(f"input order: {order}")
             tsfit = TSFit(order, model_type)
             data = np.array(data).reshape(-1, 1)
             exog = np.array(exog)
             var = np.var(data)
             var_exog = np.var(exog, axis=0)
             is_data_var_zero = math.isclose(var, 0, abs_tol=0.01)
             is_exog_var_zero = any(
```

### Comparing `tsbootstrap-0.1.0/tests/test_validate.py` & `tsbootstrap-0.1.1/tests/test_validate.py`

 * *Files identical despite different names*

