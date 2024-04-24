# Comparing `tmp/experiment_lab-1.1.5.tar.gz` & `tmp/experiment_lab-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experiment_lab-1.1.5.tar", last modified: Sun Apr 21 21:43:03 2024, max compression
+gzip compressed data, was "experiment_lab-1.1.6.tar", last modified: Wed Apr 24 04:03:06 2024, max compression
```

## Comparing `experiment_lab-1.1.5.tar` & `experiment_lab-1.1.6.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-21 21:43:03.885233 experiment_lab-1.1.5/
--rw-r--r--   0 rbhagat    (501) staff       (20)     1066 2024-03-01 07:08:11.000000 experiment_lab-1.1.5/LICENCE
--rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment_lab-1.1.5/MANIFEST.in
--rw-r--r--   0 rbhagat    (501) staff       (20)     3969 2024-04-21 21:43:03.885050 experiment_lab-1.1.5/PKG-INFO
--rw-r--r--   0 rbhagat    (501) staff       (20)     2763 2024-03-23 19:11:29.000000 experiment_lab-1.1.5/README.md
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-21 21:43:03.878631 experiment_lab-1.1.5/experiment_lab/
--rw-r--r--   0 rbhagat    (501) staff       (20)       75 2024-04-21 21:43:00.000000 experiment_lab-1.1.5/experiment_lab/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-21 21:43:03.879420 experiment_lab-1.1.5/experiment_lab/common/
--rw-r--r--   0 rbhagat    (501) staff       (20)        0 2024-03-23 19:11:29.000000 experiment_lab-1.1.5/experiment_lab/common/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-21 21:43:03.879851 experiment_lab-1.1.5/experiment_lab/common/networks/
--rw-r--r--   0 rbhagat    (501) staff       (20)      240 2024-03-12 21:19:35.000000 experiment_lab-1.1.5/experiment_lab/common/networks/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1773 2024-03-11 20:50:57.000000 experiment_lab-1.1.5/experiment_lab/common/networks/blocks.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1820 2024-03-12 21:19:35.000000 experiment_lab-1.1.5/experiment_lab/common/networks/mlp.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     6764 2024-04-15 14:50:08.000000 experiment_lab-1.1.5/experiment_lab/common/networks/network.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-21 21:43:03.880175 experiment_lab-1.1.5/experiment_lab/common/resolvers/
--rw-r--r--   0 rbhagat    (501) staff       (20)      728 2024-04-21 21:28:56.000000 experiment_lab-1.1.5/experiment_lab/common/resolvers/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1708 2024-03-12 21:19:35.000000 experiment_lab-1.1.5/experiment_lab/common/resolvers/list_resolvers.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment_lab-1.1.5/experiment_lab/common/resolvers/object_resolvers.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-21 21:43:03.880306 experiment_lab-1.1.5/experiment_lab/common/utils/
--rw-r--r--   0 rbhagat    (501) staff       (20)     1548 2024-03-11 19:31:56.000000 experiment_lab-1.1.5/experiment_lab/common/utils/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-21 21:43:03.880423 experiment_lab-1.1.5/experiment_lab/configs/
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-21 21:43:03.880513 experiment_lab-1.1.5/experiment_lab/configs/__pycache__/
--rw-r--r--   0 rbhagat    (501) staff       (20)      181 2024-03-02 18:58:05.000000 experiment_lab-1.1.5/experiment_lab/configs/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 rbhagat    (501) staff       (20)       40 2024-03-23 19:11:29.000000 experiment_lab-1.1.5/experiment_lab/configs/config.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-21 21:43:03.880742 experiment_lab-1.1.5/experiment_lab/configs/mc/
--rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-03-23 19:11:29.000000 experiment_lab-1.1.5/experiment_lab/configs/mc/config.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      750 2024-03-23 19:11:29.000000 experiment_lab-1.1.5/experiment_lab/configs/mc/estimate_pi.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-21 21:43:03.881314 experiment_lab-1.1.5/experiment_lab/configs/rl/
--rw-r--r--   0 rbhagat    (501) staff       (20)      423 2024-03-23 19:11:29.000000 experiment_lab-1.1.5/experiment_lab/configs/rl/atari.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      543 2024-04-21 21:17:21.000000 experiment_lab-1.1.5/experiment_lab/configs/rl/cartpole.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)       39 2024-03-23 19:11:29.000000 experiment_lab-1.1.5/experiment_lab/configs/rl/config.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      503 2024-03-23 19:11:29.000000 experiment_lab-1.1.5/experiment_lab/configs/rl/crossing.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      534 2024-03-23 19:11:29.000000 experiment_lab-1.1.5/experiment_lab/configs/rl/walker.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-21 21:43:03.881510 experiment_lab-1.1.5/experiment_lab/configs/supervised/
--rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment_lab-1.1.5/experiment_lab/configs/supervised/config.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)     2478 2024-03-23 19:11:29.000000 experiment_lab-1.1.5/experiment_lab/configs/supervised/fashion_mnist.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-21 21:43:03.882056 experiment_lab-1.1.5/experiment_lab/core/
--rw-r--r--   0 rbhagat    (501) staff       (20)      265 2024-04-15 14:50:08.000000 experiment_lab-1.1.5/experiment_lab/core/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     5398 2024-04-15 14:50:08.000000 experiment_lab-1.1.5/experiment_lab/core/base_analysis.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1429 2024-04-21 21:43:00.000000 experiment_lab-1.1.5/experiment_lab/core/base_config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     5813 2024-04-21 21:43:00.000000 experiment_lab-1.1.5/experiment_lab/core/base_experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     2299 2024-04-15 19:21:43.000000 experiment_lab-1.1.5/experiment_lab/core/runner.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-21 21:43:03.882159 experiment_lab-1.1.5/experiment_lab/experiments/
--rw-r--r--   0 rbhagat    (501) staff       (20)       44 2024-03-04 14:43:06.000000 experiment_lab-1.1.5/experiment_lab/experiments/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-21 21:43:03.882473 experiment_lab-1.1.5/experiment_lab/experiments/examples/
--rw-r--r--   0 rbhagat    (501) staff       (20)       36 2024-03-23 19:11:29.000000 experiment_lab-1.1.5/experiment_lab/experiments/examples/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1767 2024-03-11 14:00:07.000000 experiment_lab-1.1.5/experiment_lab/experiments/examples/mc_pi_estimate.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1371 2024-03-23 19:11:29.000000 experiment_lab-1.1.5/experiment_lab/experiments/examples/random_waits.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-21 21:43:03.882856 experiment_lab-1.1.5/experiment_lab/experiments/monte_carlo/
--rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment_lab-1.1.5/experiment_lab/experiments/monte_carlo/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-21 21:43:03.883354 experiment_lab-1.1.5/experiment_lab/experiments/monte_carlo/components/
--rw-r--r--   0 rbhagat    (501) staff       (20)      563 2024-03-11 14:00:07.000000 experiment_lab-1.1.5/experiment_lab/experiments/monte_carlo/components/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     2328 2024-03-11 14:00:07.000000 experiment_lab-1.1.5/experiment_lab/experiments/monte_carlo/components/aggregators.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1103 2024-03-11 14:00:07.000000 experiment_lab-1.1.5/experiment_lab/experiments/monte_carlo/components/post_processors.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1062 2024-03-11 14:00:07.000000 experiment_lab-1.1.5/experiment_lab/experiments/monte_carlo/components/sample_filters.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1902 2024-03-11 14:00:07.000000 experiment_lab-1.1.5/experiment_lab/experiments/monte_carlo/components/samplers.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1638 2024-04-03 18:52:52.000000 experiment_lab-1.1.5/experiment_lab/experiments/monte_carlo/config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     3212 2024-04-03 18:52:52.000000 experiment_lab-1.1.5/experiment_lab/experiments/monte_carlo/experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      575 2024-03-23 19:11:29.000000 experiment_lab-1.1.5/experiment_lab/experiments/monte_carlo/main.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-21 21:43:03.883938 experiment_lab-1.1.5/experiment_lab/experiments/rl/
--rw-r--r--   0 rbhagat    (501) staff       (20)      255 2024-03-11 14:00:07.000000 experiment_lab-1.1.5/experiment_lab/experiments/rl/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1421 2024-04-15 14:50:08.000000 experiment_lab-1.1.5/experiment_lab/experiments/rl/analysis.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1852 2024-03-13 20:27:53.000000 experiment_lab-1.1.5/experiment_lab/experiments/rl/config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)    10546 2024-04-15 14:50:08.000000 experiment_lab-1.1.5/experiment_lab/experiments/rl/environment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     6423 2024-04-21 21:17:21.000000 experiment_lab-1.1.5/experiment_lab/experiments/rl/experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      656 2024-04-15 14:50:08.000000 experiment_lab-1.1.5/experiment_lab/experiments/rl/main.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-21 21:43:03.884397 experiment_lab-1.1.5/experiment_lab/experiments/supervised/
--rw-r--r--   0 rbhagat    (501) staff       (20)       63 2024-03-12 21:19:35.000000 experiment_lab-1.1.5/experiment_lab/experiments/supervised/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     3436 2024-03-12 21:19:35.000000 experiment_lab-1.1.5/experiment_lab/experiments/supervised/config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     8526 2024-03-13 13:55:28.000000 experiment_lab-1.1.5/experiment_lab/experiments/supervised/experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      641 2024-03-23 19:11:29.000000 experiment_lab-1.1.5/experiment_lab/experiments/supervised/main.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-21 21:43:03.884539 experiment_lab-1.1.5/experiment_lab.egg-info/
--rw-r--r--   0 rbhagat    (501) staff       (20)     3969 2024-04-21 21:43:03.000000 experiment_lab-1.1.5/experiment_lab.egg-info/PKG-INFO
--rw-r--r--   0 rbhagat    (501) staff       (20)     2501 2024-04-21 21:43:03.000000 experiment_lab-1.1.5/experiment_lab.egg-info/SOURCES.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)        1 2024-04-21 21:43:03.000000 experiment_lab-1.1.5/experiment_lab.egg-info/dependency_links.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)      237 2024-04-21 21:43:03.000000 experiment_lab-1.1.5/experiment_lab.egg-info/entry_points.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)      228 2024-04-21 21:43:03.000000 experiment_lab-1.1.5/experiment_lab.egg-info/requires.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)       15 2024-04-21 21:43:03.000000 experiment_lab-1.1.5/experiment_lab.egg-info/top_level.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)     1212 2024-04-21 21:17:21.000000 experiment_lab-1.1.5/pyproject.toml
--rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-04-21 21:43:03.885267 experiment_lab-1.1.5/setup.cfg
--rw-r--r--   0 rbhagat    (501) staff       (20)     1030 2024-03-03 02:11:13.000000 experiment_lab-1.1.5/setup.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-24 04:03:06.156339 experiment_lab-1.1.6/
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1066 2024-03-01 07:08:11.000000 experiment_lab-1.1.6/LICENCE
+-rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment_lab-1.1.6/MANIFEST.in
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3969 2024-04-24 04:03:06.156175 experiment_lab-1.1.6/PKG-INFO
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2763 2024-03-23 19:11:29.000000 experiment_lab-1.1.6/README.md
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-24 04:03:06.149422 experiment_lab-1.1.6/experiment_lab/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       75 2024-04-24 04:02:15.000000 experiment_lab-1.1.6/experiment_lab/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-24 04:03:06.150273 experiment_lab-1.1.6/experiment_lab/common/
+-rw-r--r--   0 rbhagat    (501) staff       (20)        0 2024-03-23 19:11:29.000000 experiment_lab-1.1.6/experiment_lab/common/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-24 04:03:06.150802 experiment_lab-1.1.6/experiment_lab/common/networks/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      240 2024-03-12 21:19:35.000000 experiment_lab-1.1.6/experiment_lab/common/networks/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1773 2024-03-11 20:50:57.000000 experiment_lab-1.1.6/experiment_lab/common/networks/blocks.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1820 2024-03-12 21:19:35.000000 experiment_lab-1.1.6/experiment_lab/common/networks/mlp.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     6689 2024-04-24 04:01:57.000000 experiment_lab-1.1.6/experiment_lab/common/networks/network.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-24 04:03:06.151138 experiment_lab-1.1.6/experiment_lab/common/resolvers/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      728 2024-04-21 21:28:56.000000 experiment_lab-1.1.6/experiment_lab/common/resolvers/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1708 2024-03-12 21:19:35.000000 experiment_lab-1.1.6/experiment_lab/common/resolvers/list_resolvers.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment_lab-1.1.6/experiment_lab/common/resolvers/object_resolvers.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-24 04:03:06.151242 experiment_lab-1.1.6/experiment_lab/common/utils/
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1548 2024-03-11 19:31:56.000000 experiment_lab-1.1.6/experiment_lab/common/utils/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-24 04:03:06.151342 experiment_lab-1.1.6/experiment_lab/configs/
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-24 04:03:06.151455 experiment_lab-1.1.6/experiment_lab/configs/__pycache__/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      181 2024-03-02 18:58:05.000000 experiment_lab-1.1.6/experiment_lab/configs/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 rbhagat    (501) staff       (20)       40 2024-03-23 19:11:29.000000 experiment_lab-1.1.6/experiment_lab/configs/config.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-24 04:03:06.151702 experiment_lab-1.1.6/experiment_lab/configs/mc/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-03-23 19:11:29.000000 experiment_lab-1.1.6/experiment_lab/configs/mc/config.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      750 2024-03-23 19:11:29.000000 experiment_lab-1.1.6/experiment_lab/configs/mc/estimate_pi.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-24 04:03:06.152239 experiment_lab-1.1.6/experiment_lab/configs/rl/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      423 2024-03-23 19:11:29.000000 experiment_lab-1.1.6/experiment_lab/configs/rl/atari.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      543 2024-04-21 21:17:21.000000 experiment_lab-1.1.6/experiment_lab/configs/rl/cartpole.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)       39 2024-03-23 19:11:29.000000 experiment_lab-1.1.6/experiment_lab/configs/rl/config.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      503 2024-03-23 19:11:29.000000 experiment_lab-1.1.6/experiment_lab/configs/rl/crossing.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      534 2024-03-23 19:11:29.000000 experiment_lab-1.1.6/experiment_lab/configs/rl/walker.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-24 04:03:06.152456 experiment_lab-1.1.6/experiment_lab/configs/supervised/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment_lab-1.1.6/experiment_lab/configs/supervised/config.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2478 2024-03-23 19:11:29.000000 experiment_lab-1.1.6/experiment_lab/configs/supervised/fashion_mnist.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-24 04:03:06.152953 experiment_lab-1.1.6/experiment_lab/core/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      265 2024-04-15 14:50:08.000000 experiment_lab-1.1.6/experiment_lab/core/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     5398 2024-04-15 14:50:08.000000 experiment_lab-1.1.6/experiment_lab/core/base_analysis.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1429 2024-04-21 21:43:00.000000 experiment_lab-1.1.6/experiment_lab/core/base_config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     5813 2024-04-21 21:43:00.000000 experiment_lab-1.1.6/experiment_lab/core/base_experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2299 2024-04-15 19:21:43.000000 experiment_lab-1.1.6/experiment_lab/core/runner.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-24 04:03:06.153047 experiment_lab-1.1.6/experiment_lab/experiments/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       44 2024-03-04 14:43:06.000000 experiment_lab-1.1.6/experiment_lab/experiments/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-24 04:03:06.153341 experiment_lab-1.1.6/experiment_lab/experiments/examples/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       36 2024-03-23 19:11:29.000000 experiment_lab-1.1.6/experiment_lab/experiments/examples/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1767 2024-03-11 14:00:07.000000 experiment_lab-1.1.6/experiment_lab/experiments/examples/mc_pi_estimate.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1371 2024-03-23 19:11:29.000000 experiment_lab-1.1.6/experiment_lab/experiments/examples/random_waits.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-24 04:03:06.153731 experiment_lab-1.1.6/experiment_lab/experiments/monte_carlo/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment_lab-1.1.6/experiment_lab/experiments/monte_carlo/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-24 04:03:06.154285 experiment_lab-1.1.6/experiment_lab/experiments/monte_carlo/components/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      563 2024-03-11 14:00:07.000000 experiment_lab-1.1.6/experiment_lab/experiments/monte_carlo/components/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2328 2024-03-11 14:00:07.000000 experiment_lab-1.1.6/experiment_lab/experiments/monte_carlo/components/aggregators.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1103 2024-03-11 14:00:07.000000 experiment_lab-1.1.6/experiment_lab/experiments/monte_carlo/components/post_processors.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1062 2024-03-11 14:00:07.000000 experiment_lab-1.1.6/experiment_lab/experiments/monte_carlo/components/sample_filters.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1902 2024-03-11 14:00:07.000000 experiment_lab-1.1.6/experiment_lab/experiments/monte_carlo/components/samplers.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1638 2024-04-03 18:52:52.000000 experiment_lab-1.1.6/experiment_lab/experiments/monte_carlo/config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3212 2024-04-03 18:52:52.000000 experiment_lab-1.1.6/experiment_lab/experiments/monte_carlo/experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      575 2024-03-23 19:11:29.000000 experiment_lab-1.1.6/experiment_lab/experiments/monte_carlo/main.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-24 04:03:06.155030 experiment_lab-1.1.6/experiment_lab/experiments/rl/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      255 2024-03-11 14:00:07.000000 experiment_lab-1.1.6/experiment_lab/experiments/rl/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1421 2024-04-15 14:50:08.000000 experiment_lab-1.1.6/experiment_lab/experiments/rl/analysis.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1852 2024-03-13 20:27:53.000000 experiment_lab-1.1.6/experiment_lab/experiments/rl/config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)    10546 2024-04-15 14:50:08.000000 experiment_lab-1.1.6/experiment_lab/experiments/rl/environment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     6423 2024-04-21 21:17:21.000000 experiment_lab-1.1.6/experiment_lab/experiments/rl/experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      656 2024-04-15 14:50:08.000000 experiment_lab-1.1.6/experiment_lab/experiments/rl/main.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-24 04:03:06.155511 experiment_lab-1.1.6/experiment_lab/experiments/supervised/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       63 2024-03-12 21:19:35.000000 experiment_lab-1.1.6/experiment_lab/experiments/supervised/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3436 2024-03-12 21:19:35.000000 experiment_lab-1.1.6/experiment_lab/experiments/supervised/config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     8526 2024-03-13 13:55:28.000000 experiment_lab-1.1.6/experiment_lab/experiments/supervised/experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      641 2024-03-23 19:11:29.000000 experiment_lab-1.1.6/experiment_lab/experiments/supervised/main.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-24 04:03:06.155652 experiment_lab-1.1.6/experiment_lab.egg-info/
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3969 2024-04-24 04:03:06.000000 experiment_lab-1.1.6/experiment_lab.egg-info/PKG-INFO
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2501 2024-04-24 04:03:06.000000 experiment_lab-1.1.6/experiment_lab.egg-info/SOURCES.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)        1 2024-04-24 04:03:06.000000 experiment_lab-1.1.6/experiment_lab.egg-info/dependency_links.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)      237 2024-04-24 04:03:06.000000 experiment_lab-1.1.6/experiment_lab.egg-info/entry_points.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)      228 2024-04-24 04:03:06.000000 experiment_lab-1.1.6/experiment_lab.egg-info/requires.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)       15 2024-04-24 04:03:06.000000 experiment_lab-1.1.6/experiment_lab.egg-info/top_level.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1212 2024-04-21 21:17:21.000000 experiment_lab-1.1.6/pyproject.toml
+-rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-04-24 04:03:06.156373 experiment_lab-1.1.6/setup.cfg
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1030 2024-03-03 02:11:13.000000 experiment_lab-1.1.6/setup.py
```

### Comparing `experiment_lab-1.1.5/LICENCE` & `experiment_lab-1.1.6/LICENCE`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/PKG-INFO` & `experiment_lab-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experiment-lab
-Version: 1.1.5
+Version: 1.1.6
 Summary: A suite of flexible experiments of a variety of different tasks.
 Author-email: Rishav Bhagat <rishavbhagat.cs@gmail.com>
 Project-URL: Repository, https://github.com/rishavb123/ExperimentLab
 Keywords: experiment,suite,lab
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `experiment_lab-1.1.5/README.md` & `experiment_lab-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/common/networks/blocks.py` & `experiment_lab-1.1.6/experiment_lab/common/networks/blocks.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/common/networks/mlp.py` & `experiment_lab-1.1.6/experiment_lab/common/networks/mlp.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/common/networks/network.py` & `experiment_lab-1.1.6/experiment_lab/common/networks/network.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,22 +82,22 @@
 
 class AggregatedNetwork(nn.Module):
     """A class for aggregated multi input networks."""
 
     def __init__(
         self,
         module_lst: Sequence[nn.Module],
-        aggregator: Callable[[torch.Tensor, torch.Tensor], torch.Tensor],
+        aggregator: Callable[[Sequence[torch.Tensor]], torch.Tensor],
         output_module: nn.Module,
     ) -> None:
         """The constructor for the multi input network.
 
         Args:
             module_lst (Sequence[nn.Module]): The list of modules to apply before aggregation.
-            aggregator (Callable[[torch.Tensor, torch.Tensor], torch.Tensor]): The aggregator to use on the tensors.
+            aggregator (Callable[[Sequence[torch.Tensor]], torch.Tensor]): The aggregator to use on the tensors.
             output_module (nn.Module): The module to apply after aggregation.
         """
         super().__init__()
         self.module_lst = nn.ModuleList(module_lst)
         self.aggregator = aggregator
         self.output_module = output_module
 
@@ -107,17 +107,15 @@
         Args:
             xs (Sequence[torch.Tensor]): The inputs to the network.
 
         Returns:
             torch.Tensor: The output of the network.
         """
         zs: Sequence[torch.Tensor] = [m(x) for x, m in zip(xs, self.module_lst)]
-        agg_z = zs[0]
-        for z in zs[1:]:
-            agg_z = self.aggregator(agg_z, z)
+        agg_z = self.aggregator(zs)
         return self.output_module(agg_z)
 
 
 class MultiNetwork(nn.Module):
     """A class for a multi output network."""
 
     def __init__(
@@ -146,22 +144,22 @@
         """
         z = self.input_module(x)
         return [m(z) for m in self.module_lst]
 
 
 def create_aggregated_network(
     module_lst: Sequence[nn.Module],
-    aggregator: Callable[[torch.Tensor, torch.Tensor], torch.Tensor],
+    aggregator: Callable[[Sequence[torch.Tensor]], torch.Tensor],
     output_module: nn.Module,
 ) -> AggregatedNetwork:
     """Creates an instance of the complex multi input network.
 
         Args:
             module_lst (Sequence[nn.Module]): The list of modules to apply before aggregation.
-            aggregator (Callable[[torch.Tensor, torch.Tensor], torch.Tensor]): The aggregator to use on the tensors.
+            aggregator (Callable[Sequence[torch.Tensor], torch.Tensor]): The aggregator to use on the tensors.
             output_module (nn.Module): The module to apply after aggregation.
 
     Returns:
         AggregatedNetwork: The complex multi input network.
     """
     return AggregatedNetwork(module_lst, aggregator, output_module)
```

### Comparing `experiment_lab-1.1.5/experiment_lab/common/resolvers/__init__.py` & `experiment_lab-1.1.6/experiment_lab/common/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/common/resolvers/list_resolvers.py` & `experiment_lab-1.1.6/experiment_lab/common/resolvers/list_resolvers.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/common/utils/__init__.py` & `experiment_lab-1.1.6/experiment_lab/common/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/configs/mc/estimate_pi.yaml` & `experiment_lab-1.1.6/experiment_lab/configs/mc/estimate_pi.yaml`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/configs/rl/cartpole.yaml` & `experiment_lab-1.1.6/experiment_lab/configs/rl/cartpole.yaml`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/configs/rl/walker.yaml` & `experiment_lab-1.1.6/experiment_lab/configs/rl/walker.yaml`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/configs/supervised/fashion_mnist.yaml` & `experiment_lab-1.1.6/experiment_lab/configs/supervised/fashion_mnist.yaml`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/core/base_analysis.py` & `experiment_lab-1.1.6/experiment_lab/core/base_analysis.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/core/base_config.py` & `experiment_lab-1.1.6/experiment_lab/core/base_config.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/core/base_experiment.py` & `experiment_lab-1.1.6/experiment_lab/core/base_experiment.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/core/runner.py` & `experiment_lab-1.1.6/experiment_lab/core/runner.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/experiments/examples/mc_pi_estimate.py` & `experiment_lab-1.1.6/experiment_lab/experiments/examples/mc_pi_estimate.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/experiments/examples/random_waits.py` & `experiment_lab-1.1.6/experiment_lab/experiments/examples/random_waits.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/experiments/monte_carlo/components/__init__.py` & `experiment_lab-1.1.6/experiment_lab/experiments/monte_carlo/components/__init__.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/experiments/monte_carlo/components/aggregators.py` & `experiment_lab-1.1.6/experiment_lab/experiments/monte_carlo/components/aggregators.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/experiments/monte_carlo/components/post_processors.py` & `experiment_lab-1.1.6/experiment_lab/experiments/monte_carlo/components/post_processors.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/experiments/monte_carlo/components/sample_filters.py` & `experiment_lab-1.1.6/experiment_lab/experiments/monte_carlo/components/sample_filters.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/experiments/monte_carlo/components/samplers.py` & `experiment_lab-1.1.6/experiment_lab/experiments/monte_carlo/components/samplers.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/experiments/monte_carlo/config.py` & `experiment_lab-1.1.6/experiment_lab/experiments/monte_carlo/config.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/experiments/monte_carlo/experiment.py` & `experiment_lab-1.1.6/experiment_lab/experiments/monte_carlo/experiment.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/experiments/monte_carlo/main.py` & `experiment_lab-1.1.6/experiment_lab/experiments/monte_carlo/main.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/experiments/rl/analysis.py` & `experiment_lab-1.1.6/experiment_lab/experiments/rl/analysis.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/experiments/rl/config.py` & `experiment_lab-1.1.6/experiment_lab/experiments/rl/config.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/experiments/rl/environment.py` & `experiment_lab-1.1.6/experiment_lab/experiments/rl/environment.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/experiments/rl/experiment.py` & `experiment_lab-1.1.6/experiment_lab/experiments/rl/experiment.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/experiments/rl/main.py` & `experiment_lab-1.1.6/experiment_lab/experiments/rl/main.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/experiments/supervised/config.py` & `experiment_lab-1.1.6/experiment_lab/experiments/supervised/config.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/experiments/supervised/experiment.py` & `experiment_lab-1.1.6/experiment_lab/experiments/supervised/experiment.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab/experiments/supervised/main.py` & `experiment_lab-1.1.6/experiment_lab/experiments/supervised/main.py`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/experiment_lab.egg-info/PKG-INFO` & `experiment_lab-1.1.6/experiment_lab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experiment-lab
-Version: 1.1.5
+Version: 1.1.6
 Summary: A suite of flexible experiments of a variety of different tasks.
 Author-email: Rishav Bhagat <rishavbhagat.cs@gmail.com>
 Project-URL: Repository, https://github.com/rishavb123/ExperimentLab
 Keywords: experiment,suite,lab
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `experiment_lab-1.1.5/experiment_lab.egg-info/SOURCES.txt` & `experiment_lab-1.1.6/experiment_lab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/pyproject.toml` & `experiment_lab-1.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `experiment_lab-1.1.5/setup.py` & `experiment_lab-1.1.6/setup.py`

 * *Files identical despite different names*

