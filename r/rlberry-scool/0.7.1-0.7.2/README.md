# Comparing `tmp/rlberry-scool-0.7.1.tar.gz` & `tmp/rlberry-scool-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlberry-scool-0.7.1.tar", last modified: Fri Mar  1 11:03:00 2024, max compression
+gzip compressed data, was "rlberry-scool-0.7.2.tar", last modified: Wed Mar  6 13:31:20 2024, max compression
```

## Comparing `rlberry-scool-0.7.1.tar` & `rlberry-scool-0.7.2.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2024-03-01 11:03:00.597687 rlberry-scool-0.7.1/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1067 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/LICENSE
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1397 2024-03-01 11:03:00.597687 rlberry-scool-0.7.1/PKG-INFO
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      715 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/README.md
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2024-03-01 11:03:00.597687 rlberry-scool-0.7.1/rlberry_scool/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       38 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       23 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/_version.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2024-03-01 11:03:00.597687 rlberry-scool-0.7.1/rlberry_scool/agents/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      161 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/agents/__init__.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2024-03-01 11:03:00.597687 rlberry-scool-0.7.1/rlberry_scool/agents/dynprog/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       49 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/agents/dynprog/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     8882 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/agents/dynprog/utils.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2806 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/agents/dynprog/value_iteration.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2024-03-01 11:03:00.597687 rlberry-scool-0.7.1/rlberry_scool/agents/features/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       36 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/agents/features/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      580 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/agents/features/feature_map.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2024-03-01 11:03:00.597687 rlberry-scool-0.7.1/rlberry_scool/agents/linear/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       35 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/agents/linear/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    11599 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/agents/linear/lsvi_ucb.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2024-03-01 11:03:00.597687 rlberry-scool-0.7.1/rlberry_scool/agents/mbqvi/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       30 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/agents/mbqvi/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5220 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/agents/mbqvi/mbqvi.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2024-03-01 11:03:00.597687 rlberry-scool-0.7.1/rlberry_scool/agents/tabular_rl/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       61 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/agents/tabular_rl/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4383 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/agents/tabular_rl/qlearning.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4417 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/agents/tabular_rl/sarsa.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2024-03-01 11:03:00.597687 rlberry-scool-0.7.1/rlberry_scool/agents/tests/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/agents/tests/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4948 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/agents/tests/test_dynprog.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     6192 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/agents/tests/test_lsvi_ucb.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      818 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/agents/tests/test_mbqvi.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2024-03-01 11:03:00.597687 rlberry-scool-0.7.1/rlberry_scool/colab_utils/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/colab_utils/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1053 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/colab_utils/display_setup.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2024-03-01 11:03:00.597687 rlberry-scool-0.7.1/rlberry_scool/envs/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       56 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/envs/__init__.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2024-03-01 11:03:00.597687 rlberry-scool-0.7.1/rlberry_scool/envs/finite/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      232 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/envs/finite/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4016 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/envs/finite/chain.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    16244 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/envs/finite/gridworld.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2011 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/envs/finite/gridworld_utils.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2024-03-01 11:03:00.597687 rlberry-scool-0.7.1/rlberry_scool/envs/tests/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/envs/tests/__init__.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2128 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/envs/tests/test_env_seeding.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3110 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/envs/tests/test_instantiation.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1498 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/envs/tests/test_rendering.py
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      564 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/rlberry_scool/random_agent.py
-drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2024-03-01 11:03:00.597687 rlberry-scool-0.7.1/rlberry_scool.egg-info/
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1397 2024-03-01 11:03:00.000000 rlberry-scool-0.7.1/rlberry_scool.egg-info/PKG-INFO
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1468 2024-03-01 11:03:00.000000 rlberry-scool-0.7.1/rlberry_scool.egg-info/SOURCES.txt
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        1 2024-03-01 11:03:00.000000 rlberry-scool-0.7.1/rlberry_scool.egg-info/dependency_links.txt
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        1 2024-03-01 11:03:00.000000 rlberry-scool-0.7.1/rlberry_scool.egg-info/not-zip-safe
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        8 2024-03-01 11:03:00.000000 rlberry-scool-0.7.1/rlberry_scool.egg-info/requires.txt
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       14 2024-03-01 11:03:00.000000 rlberry-scool-0.7.1/rlberry_scool.egg-info/top_level.txt
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       38 2024-03-01 11:03:00.597687 rlberry-scool-0.7.1/setup.cfg
--rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1156 2024-03-01 11:02:01.000000 rlberry-scool-0.7.1/setup.py
+drwxr-xr-x   0 dr.t      (1000) users      (998)        0 2024-03-06 13:31:20.393101 rlberry-scool-0.7.2/
+-rw-r--r--   0 dr.t      (1000) users      (998)     1067 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/LICENSE
+-rw-r--r--   0 dr.t      (1000) users      (998)     1400 2024-03-06 13:31:20.393101 rlberry-scool-0.7.2/PKG-INFO
+-rw-r--r--   0 dr.t      (1000) users      (998)      715 2024-03-06 13:25:27.000000 rlberry-scool-0.7.2/README.md
+drwxr-xr-x   0 dr.t      (1000) users      (998)        0 2024-03-06 13:31:20.389101 rlberry-scool-0.7.2/rlberry_scool/
+-rw-r--r--   0 dr.t      (1000) users      (998)      112 2024-03-06 13:25:27.000000 rlberry-scool-0.7.2/rlberry_scool/__init__.py
+-rw-r--r--   0 dr.t      (1000) users      (998)       23 2024-03-06 13:29:18.000000 rlberry-scool-0.7.2/rlberry_scool/_version.py
+drwxr-xr-x   0 dr.t      (1000) users      (998)        0 2024-03-06 13:31:20.389101 rlberry-scool-0.7.2/rlberry_scool/agents/
+-rw-r--r--   0 dr.t      (1000) users      (998)      161 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/agents/__init__.py
+drwxr-xr-x   0 dr.t      (1000) users      (998)        0 2024-03-06 13:31:20.389101 rlberry-scool-0.7.2/rlberry_scool/agents/dynprog/
+-rw-r--r--   0 dr.t      (1000) users      (998)       49 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/agents/dynprog/__init__.py
+-rw-r--r--   0 dr.t      (1000) users      (998)     8882 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/agents/dynprog/utils.py
+-rw-r--r--   0 dr.t      (1000) users      (998)     2803 2024-03-06 13:27:12.000000 rlberry-scool-0.7.2/rlberry_scool/agents/dynprog/value_iteration.py
+drwxr-xr-x   0 dr.t      (1000) users      (998)        0 2024-03-06 13:31:20.389101 rlberry-scool-0.7.2/rlberry_scool/agents/features/
+-rw-r--r--   0 dr.t      (1000) users      (998)       36 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/agents/features/__init__.py
+-rw-r--r--   0 dr.t      (1000) users      (998)      580 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/agents/features/feature_map.py
+drwxr-xr-x   0 dr.t      (1000) users      (998)        0 2024-03-06 13:31:20.389101 rlberry-scool-0.7.2/rlberry_scool/agents/linear/
+-rw-r--r--   0 dr.t      (1000) users      (998)       35 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/agents/linear/__init__.py
+-rw-r--r--   0 dr.t      (1000) users      (998)    11599 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/agents/linear/lsvi_ucb.py
+drwxr-xr-x   0 dr.t      (1000) users      (998)        0 2024-03-06 13:31:20.389101 rlberry-scool-0.7.2/rlberry_scool/agents/mbqvi/
+-rw-r--r--   0 dr.t      (1000) users      (998)       30 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/agents/mbqvi/__init__.py
+-rw-r--r--   0 dr.t      (1000) users      (998)     5220 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/agents/mbqvi/mbqvi.py
+drwxr-xr-x   0 dr.t      (1000) users      (998)        0 2024-03-06 13:31:20.389101 rlberry-scool-0.7.2/rlberry_scool/agents/tabular_rl/
+-rw-r--r--   0 dr.t      (1000) users      (998)       61 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/agents/tabular_rl/__init__.py
+-rw-r--r--   0 dr.t      (1000) users      (998)     4383 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/agents/tabular_rl/qlearning.py
+-rw-r--r--   0 dr.t      (1000) users      (998)     4417 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/agents/tabular_rl/sarsa.py
+drwxr-xr-x   0 dr.t      (1000) users      (998)        0 2024-03-06 13:31:20.389101 rlberry-scool-0.7.2/rlberry_scool/agents/tests/
+-rw-r--r--   0 dr.t      (1000) users      (998)        0 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/agents/tests/__init__.py
+-rw-r--r--   0 dr.t      (1000) users      (998)     4948 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/agents/tests/test_dynprog.py
+-rw-r--r--   0 dr.t      (1000) users      (998)     6192 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/agents/tests/test_lsvi_ucb.py
+-rw-r--r--   0 dr.t      (1000) users      (998)      818 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/agents/tests/test_mbqvi.py
+drwxr-xr-x   0 dr.t      (1000) users      (998)        0 2024-03-06 13:31:20.389101 rlberry-scool-0.7.2/rlberry_scool/colab_utils/
+-rw-r--r--   0 dr.t      (1000) users      (998)        0 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/colab_utils/__init__.py
+-rw-r--r--   0 dr.t      (1000) users      (998)     1053 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/colab_utils/display_setup.py
+drwxr-xr-x   0 dr.t      (1000) users      (998)        0 2024-03-06 13:31:20.389101 rlberry-scool-0.7.2/rlberry_scool/envs/
+-rw-r--r--   0 dr.t      (1000) users      (998)       56 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/envs/__init__.py
+drwxr-xr-x   0 dr.t      (1000) users      (998)        0 2024-03-06 13:31:20.393101 rlberry-scool-0.7.2/rlberry_scool/envs/finite/
+-rw-r--r--   0 dr.t      (1000) users      (998)      295 2024-03-06 13:26:15.000000 rlberry-scool-0.7.2/rlberry_scool/envs/finite/__init__.py
+-rw-r--r--   0 dr.t      (1000) users      (998)     4016 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/envs/finite/chain.py
+-rw-r--r--   0 dr.t      (1000) users      (998)     4501 2024-03-06 13:25:27.000000 rlberry-scool-0.7.2/rlberry_scool/envs/finite/discrete_mountain_car.py
+-rw-r--r--   0 dr.t      (1000) users      (998)    16244 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/envs/finite/gridworld.py
+-rw-r--r--   0 dr.t      (1000) users      (998)     2011 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/envs/finite/gridworld_utils.py
+drwxr-xr-x   0 dr.t      (1000) users      (998)        0 2024-03-06 13:31:20.393101 rlberry-scool-0.7.2/rlberry_scool/envs/tests/
+-rw-r--r--   0 dr.t      (1000) users      (998)        0 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/envs/tests/__init__.py
+-rw-r--r--   0 dr.t      (1000) users      (998)     2128 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/envs/tests/test_env_seeding.py
+-rw-r--r--   0 dr.t      (1000) users      (998)     3408 2024-03-06 13:26:20.000000 rlberry-scool-0.7.2/rlberry_scool/envs/tests/test_instantiation.py
+-rw-r--r--   0 dr.t      (1000) users      (998)     1498 2024-03-06 13:26:24.000000 rlberry-scool-0.7.2/rlberry_scool/envs/tests/test_rendering.py
+-rw-r--r--   0 dr.t      (1000) users      (998)      564 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/rlberry_scool/random_agent.py
+drwxr-xr-x   0 dr.t      (1000) users      (998)        0 2024-03-06 13:31:20.393101 rlberry-scool-0.7.2/rlberry_scool.egg-info/
+-rw-r--r--   0 dr.t      (1000) users      (998)     1400 2024-03-06 13:31:20.000000 rlberry-scool-0.7.2/rlberry_scool.egg-info/PKG-INFO
+-rw-r--r--   0 dr.t      (1000) users      (998)     1519 2024-03-06 13:31:20.000000 rlberry-scool-0.7.2/rlberry_scool.egg-info/SOURCES.txt
+-rw-r--r--   0 dr.t      (1000) users      (998)        1 2024-03-06 13:31:20.000000 rlberry-scool-0.7.2/rlberry_scool.egg-info/dependency_links.txt
+-rw-r--r--   0 dr.t      (1000) users      (998)        1 2024-03-06 13:31:20.000000 rlberry-scool-0.7.2/rlberry_scool.egg-info/not-zip-safe
+-rw-r--r--   0 dr.t      (1000) users      (998)        8 2024-03-06 13:31:20.000000 rlberry-scool-0.7.2/rlberry_scool.egg-info/requires.txt
+-rw-r--r--   0 dr.t      (1000) users      (998)       14 2024-03-06 13:31:20.000000 rlberry-scool-0.7.2/rlberry_scool.egg-info/top_level.txt
+-rw-r--r--   0 dr.t      (1000) users      (998)       38 2024-03-06 13:31:20.393101 rlberry-scool-0.7.2/setup.cfg
+-rw-r--r--   0 dr.t      (1000) users      (998)     1156 2024-03-06 13:24:34.000000 rlberry-scool-0.7.2/setup.py
```

### Comparing `rlberry-scool-0.7.1/LICENSE` & `rlberry-scool-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rlberry-scool-0.7.1/PKG-INFO` & `rlberry-scool-0.7.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: rlberry-scool
-Version: 0.7.1
+Version: 0.7.2
 Summary: Teaching Reinforcement Learning made easy
 Home-page: https://github.com/rlberry-py
 Author: Inria Scool team
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: rlberry
 
 
 <!-- The badges --> 
 <!--  TODO!!!
 <p align="center">
 #   <a href="https://pypi.org/project/rlberry/">
 #      <img alt="Python Version" src="https://img.shields.io/badge/python-3.11-blue">
@@ -33,9 +33,7 @@
 #</p>
 #![](https://img.shields.io/codecov/c/github/rlberry-py/rlberry-scool)
 -->  
 
 
 # rlberry-scool
 Teaching Reinforcement Learning made easy.
-
-
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: rlberry-scool Version: 0.7.1 Summary: Teaching
+Metadata-Version: 2.1 Name: rlberry-scool Version: 0.7.2 Summary: Teaching
 Reinforcement Learning made easy Home-page: https://github.com/rlberry-py
-Author: Inria Scool team License: MIT Platform: UNKNOWN Classifier: Development
-Status :: 4 - Beta Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Education Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Description-Content-Type: text/markdown License-File: LICENSE
-# rlberry-scool Teaching Reinforcement Learning made easy.
+Author: Inria Scool team License: MIT Classifier: Development Status :: 4 -
+Beta Classifier: Intended Audience :: Science/Research Classifier: Intended
+Audience :: Education Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: License :: OSI Approved
+:: MIT License Classifier: Operating System :: OS Independent Description-
+Content-Type: text/markdown License-File: LICENSE Requires-Dist: rlberry #
+rlberry-scool Teaching Reinforcement Learning made easy.
```

### Comparing `rlberry-scool-0.7.1/README.md` & `rlberry-scool-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `rlberry-scool-0.7.1/rlberry_scool/agents/dynprog/utils.py` & `rlberry-scool-0.7.2/rlberry_scool/agents/dynprog/utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-scool-0.7.1/rlberry_scool/agents/dynprog/value_iteration.py` & `rlberry-scool-0.7.2/rlberry_scool/agents/dynprog/value_iteration.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         problem is solved
         default = None
     epsilon : double
         Precision of value iteration, only used in discounted problems
         (when horizon is None).
     **kwargs : Keyword Arguments
          Arguments to be passed to `AgentWithSimplePolicy.__init__(self, env, **kwargs)` (:class:`~rlberry.agents.AgentWithSimplePolicy`).
-   
+
 
     """
 
     name = "ValueIteration"
 
     def __init__(self, env, gamma=0.95, horizon=None, epsilon=1e-6, **kwargs):
         AgentWithSimplePolicy.__init__(self, env, **kwargs)
```

### Comparing `rlberry-scool-0.7.1/rlberry_scool/agents/features/feature_map.py` & `rlberry-scool-0.7.2/rlberry_scool/agents/features/feature_map.py`

 * *Files identical despite different names*

### Comparing `rlberry-scool-0.7.1/rlberry_scool/agents/linear/lsvi_ucb.py` & `rlberry-scool-0.7.2/rlberry_scool/agents/linear/lsvi_ucb.py`

 * *Files identical despite different names*

### Comparing `rlberry-scool-0.7.1/rlberry_scool/agents/mbqvi/mbqvi.py` & `rlberry-scool-0.7.2/rlberry_scool/agents/mbqvi/mbqvi.py`

 * *Files identical despite different names*

### Comparing `rlberry-scool-0.7.1/rlberry_scool/agents/tabular_rl/qlearning.py` & `rlberry-scool-0.7.2/rlberry_scool/agents/tabular_rl/qlearning.py`

 * *Files identical despite different names*

### Comparing `rlberry-scool-0.7.1/rlberry_scool/agents/tabular_rl/sarsa.py` & `rlberry-scool-0.7.2/rlberry_scool/agents/tabular_rl/sarsa.py`

 * *Files identical despite different names*

### Comparing `rlberry-scool-0.7.1/rlberry_scool/agents/tests/test_dynprog.py` & `rlberry-scool-0.7.2/rlberry_scool/agents/tests/test_dynprog.py`

 * *Files identical despite different names*

### Comparing `rlberry-scool-0.7.1/rlberry_scool/agents/tests/test_lsvi_ucb.py` & `rlberry-scool-0.7.2/rlberry_scool/agents/tests/test_lsvi_ucb.py`

 * *Files identical despite different names*

### Comparing `rlberry-scool-0.7.1/rlberry_scool/agents/tests/test_mbqvi.py` & `rlberry-scool-0.7.2/rlberry_scool/agents/tests/test_mbqvi.py`

 * *Files identical despite different names*

### Comparing `rlberry-scool-0.7.1/rlberry_scool/colab_utils/display_setup.py` & `rlberry-scool-0.7.2/rlberry_scool/colab_utils/display_setup.py`

 * *Files identical despite different names*

### Comparing `rlberry-scool-0.7.1/rlberry_scool/envs/finite/chain.py` & `rlberry-scool-0.7.2/rlberry_scool/envs/finite/chain.py`

 * *Files identical despite different names*

### Comparing `rlberry-scool-0.7.1/rlberry_scool/envs/finite/gridworld.py` & `rlberry-scool-0.7.2/rlberry_scool/envs/finite/gridworld.py`

 * *Files identical despite different names*

### Comparing `rlberry-scool-0.7.1/rlberry_scool/envs/finite/gridworld_utils.py` & `rlberry-scool-0.7.2/rlberry_scool/envs/finite/gridworld_utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-scool-0.7.1/rlberry_scool/envs/tests/test_env_seeding.py` & `rlberry-scool-0.7.2/rlberry_scool/envs/tests/test_env_seeding.py`

 * *Files identical despite different names*

### Comparing `rlberry-scool-0.7.1/rlberry_scool/envs/tests/test_instantiation.py` & `rlberry-scool-0.7.2/rlberry_scool/envs/tests/test_instantiation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 import pytest
 
 from rlberry.envs import gym_make, PipelineEnv
 from rlberry_scool.envs.finite import Chain
 from rlberry_scool.envs.finite import GridWorld
+from rlberry_scool.envs.finite import get_discrete_mountain_car_env
 from rlberry.rendering.render_interface import RenderInterface2D
 
 classes = [
     GridWorld,
     Chain,
 ]
 
@@ -67,15 +68,14 @@
     OOOOO O OOOOO  # OOTOO
     OOOOO # OOOOO  # OOOOO
     IOOOO # OOOOO  # OOOOr"""
     env = GridWorld.from_layout(layout)
     env.reset()
 
 
-
 def test_pipeline():
     from rlberry.wrappers import RescaleRewardWrapper
     from rlberry.wrappers.discretize_state import DiscretizeStateWrapper
 
     env_ctor, env_kwargs = PipelineEnv, {
         "env_ctor": gym_make,
         "env_kwargs": {"id": "Acrobot-v1"},
@@ -95,7 +95,17 @@
     }
     env = env_ctor(**env_kwargs)
     # check that wrapped in the right order
     assert isinstance(
         env.env, RescaleRewardWrapper
     ), "the environments in Pipeline env may not be wrapped in order"
     assert isinstance(env.env.env, DiscretizeStateWrapper)
+
+
+def test_discrete_mc():
+    env = get_discrete_mountain_car_env()
+    env.reset()
+    done = False
+    while not done:
+        a = env.action_space.sample()
+        _, _, term, trunc, _ = env.step(a)
+        done = term or trunc
```

### Comparing `rlberry-scool-0.7.1/rlberry_scool/envs/tests/test_rendering.py` & `rlberry-scool-0.7.2/rlberry_scool/envs/tests/test_rendering.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from rlberry_scool.envs.finite import Chain,GridWorld
+from rlberry_scool.envs.finite import Chain, GridWorld
 from rlberry_scool.agents.dynprog import ValueIterationAgent
 import tempfile
 import os
 
 
 def test_chain_rendering():
     env = Chain(10, 0.3)
@@ -33,15 +33,14 @@
         observation, reward, terminated, truncated, info = env.step(action)
         done = terminated or truncated
         if done:
             # Warning: this will never happen in the present case because there is no terminal state.
             # See the doc of GridWorld for more informations on the default parameters of GridWorld.
             break
 
-
     with tempfile.TemporaryDirectory() as tmpdirname:
         saving_path = tmpdirname + "/test_gif.gif"
         env.save_gif(saving_path)
         assert os.path.isfile(saving_path)
         try:
             os.remove(saving_path)
         except Exception:
```

### Comparing `rlberry-scool-0.7.1/rlberry_scool/random_agent.py` & `rlberry-scool-0.7.2/rlberry_scool/random_agent.py`

 * *Files identical despite different names*

### Comparing `rlberry-scool-0.7.1/rlberry_scool.egg-info/PKG-INFO` & `rlberry-scool-0.7.2/rlberry_scool.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: rlberry-scool
-Version: 0.7.1
+Version: 0.7.2
 Summary: Teaching Reinforcement Learning made easy
 Home-page: https://github.com/rlberry-py
 Author: Inria Scool team
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: rlberry
 
 
 <!-- The badges --> 
 <!--  TODO!!!
 <p align="center">
 #   <a href="https://pypi.org/project/rlberry/">
 #      <img alt="Python Version" src="https://img.shields.io/badge/python-3.11-blue">
@@ -33,9 +33,7 @@
 #</p>
 #![](https://img.shields.io/codecov/c/github/rlberry-py/rlberry-scool)
 -->  
 
 
 # rlberry-scool
 Teaching Reinforcement Learning made easy.
-
-
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: rlberry-scool Version: 0.7.1 Summary: Teaching
+Metadata-Version: 2.1 Name: rlberry-scool Version: 0.7.2 Summary: Teaching
 Reinforcement Learning made easy Home-page: https://github.com/rlberry-py
-Author: Inria Scool team License: MIT Platform: UNKNOWN Classifier: Development
-Status :: 4 - Beta Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Education Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Description-Content-Type: text/markdown License-File: LICENSE
-# rlberry-scool Teaching Reinforcement Learning made easy.
+Author: Inria Scool team License: MIT Classifier: Development Status :: 4 -
+Beta Classifier: Intended Audience :: Science/Research Classifier: Intended
+Audience :: Education Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: License :: OSI Approved
+:: MIT License Classifier: Operating System :: OS Independent Description-
+Content-Type: text/markdown License-File: LICENSE Requires-Dist: rlberry #
+rlberry-scool Teaching Reinforcement Learning made easy.
```

### Comparing `rlberry-scool-0.7.1/rlberry_scool.egg-info/SOURCES.txt` & `rlberry-scool-0.7.2/rlberry_scool.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -28,13 +28,14 @@
 rlberry_scool/agents/tests/test_lsvi_ucb.py
 rlberry_scool/agents/tests/test_mbqvi.py
 rlberry_scool/colab_utils/__init__.py
 rlberry_scool/colab_utils/display_setup.py
 rlberry_scool/envs/__init__.py
 rlberry_scool/envs/finite/__init__.py
 rlberry_scool/envs/finite/chain.py
+rlberry_scool/envs/finite/discrete_mountain_car.py
 rlberry_scool/envs/finite/gridworld.py
 rlberry_scool/envs/finite/gridworld_utils.py
 rlberry_scool/envs/tests/__init__.py
 rlberry_scool/envs/tests/test_env_seeding.py
 rlberry_scool/envs/tests/test_instantiation.py
 rlberry_scool/envs/tests/test_rendering.py
```

### Comparing `rlberry-scool-0.7.1/setup.py` & `rlberry-scool-0.7.2/setup.py`

 * *Files identical despite different names*

