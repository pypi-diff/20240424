# Comparing `tmp/PVNet-3.0.8.tar.gz` & `tmp/PVNet-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PVNet-3.0.8.tar", last modified: Thu Feb 29 11:24:59 2024, max compression
+gzip compressed data, was "PVNet-3.0.9.tar", last modified: Thu Feb 29 14:08:04 2024, max compression
```

## Comparing `PVNet-3.0.8.tar` & `PVNet-3.0.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:24:59.399462 PVNet-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-02-29 11:24:49.000000 PVNet-3.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-29 11:24:49.000000 PVNet-3.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-02-29 11:24:59.399462 PVNet-3.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:24:59.399462 PVNet-3.0.8/PVNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-02-29 11:24:59.000000 PVNet-3.0.8/PVNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-02-29 11:24:59.000000 PVNet-3.0.8/PVNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 11:24:59.000000 PVNet-3.0.8/PVNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-02-29 11:24:59.000000 PVNet-3.0.8/PVNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-29 11:24:59.000000 PVNet-3.0.8/PVNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-02-29 11:24:49.000000 PVNet-3.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:24:59.391462 PVNet-3.0.8/pvnet/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:24:59.391462 PVNet-3.0.8/pvnet/data/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/data/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/data/pv_site_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/data/wind_datamodule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:24:59.391462 PVNet-3.0.8/pvnet/models/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23211 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:24:59.395462 PVNet-3.0.8/pvnet/models/baseline/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/baseline/last_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/baseline/single_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:24:59.395462 PVNet-3.0.8/pvnet/models/multimodal/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/multimodal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/multimodal/basic_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/multimodal/deep_supervision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:24:59.395462 PVNet-3.0.8/pvnet/models/multimodal/encoders/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/multimodal/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/multimodal/encoders/basic_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    14420 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/multimodal/encoders/encoders2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    14595 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/multimodal/encoders/encoders3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/multimodal/encoders/encodersRNN.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:24:59.395462 PVNet-3.0.8/pvnet/models/multimodal/linear_networks/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/multimodal/linear_networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/multimodal/linear_networks/basic_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11118 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/multimodal/linear_networks/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)    17115 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/multimodal/multimodal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/multimodal/multimodal_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/multimodal/nwp_weighting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:24:59.395462 PVNet-3.0.8/pvnet/models/multimodal/site_encoders/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/multimodal/site_encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/multimodal/site_encoders/basic_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/multimodal/site_encoders/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    17612 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/multimodal/unimodal_teacher.py
--rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/multimodal/weather_residual.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6177 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/training.py
--rw-r--r--   0 runner    (1001) docker     (127)    11271 2024-02-29 11:24:49.000000 PVNet-3.0.8/pvnet/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-02-29 11:24:49.000000 PVNet-3.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-29 11:24:49.000000 PVNet-3.0.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-29 11:24:49.000000 PVNet-3.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 11:24:59.399462 PVNet-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-29 11:24:49.000000 PVNet-3.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:24:59.395462 PVNet-3.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 11:24:49.000000 PVNet-3.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-02-29 11:24:49.000000 PVNet-3.0.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-29 11:24:50.000000 PVNet-3.0.8/tests/test_end2end.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:08:04.297818 PVNet-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-02-29 14:07:56.000000 PVNet-3.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-29 14:07:56.000000 PVNet-3.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-02-29 14:08:04.297818 PVNet-3.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:08:04.293818 PVNet-3.0.9/PVNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-02-29 14:08:04.000000 PVNet-3.0.9/PVNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-02-29 14:08:04.000000 PVNet-3.0.9/PVNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 14:08:04.000000 PVNet-3.0.9/PVNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-02-29 14:08:04.000000 PVNet-3.0.9/PVNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-29 14:08:04.000000 PVNet-3.0.9/PVNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-02-29 14:07:56.000000 PVNet-3.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:08:04.289818 PVNet-3.0.9/pvnet/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:08:04.289818 PVNet-3.0.9/pvnet/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/data/pv_site_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/data/wind_datamodule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:08:04.289818 PVNet-3.0.9/pvnet/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23143 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:08:04.289818 PVNet-3.0.9/pvnet/models/baseline/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/baseline/last_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/baseline/single_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:08:04.293818 PVNet-3.0.9/pvnet/models/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/multimodal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/multimodal/basic_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/multimodal/deep_supervision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:08:04.293818 PVNet-3.0.9/pvnet/models/multimodal/encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/multimodal/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/multimodal/encoders/basic_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14420 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/multimodal/encoders/encoders2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14595 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/multimodal/encoders/encoders3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/multimodal/encoders/encodersRNN.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:08:04.293818 PVNet-3.0.9/pvnet/models/multimodal/linear_networks/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/multimodal/linear_networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/multimodal/linear_networks/basic_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11118 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/multimodal/linear_networks/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17115 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/multimodal/multimodal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/multimodal/multimodal_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/multimodal/nwp_weighting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:08:04.293818 PVNet-3.0.9/pvnet/models/multimodal/site_encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/multimodal/site_encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/multimodal/site_encoders/basic_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/multimodal/site_encoders/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17612 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/multimodal/unimodal_teacher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/multimodal/weather_residual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6177 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/training.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11271 2024-02-29 14:07:56.000000 PVNet-3.0.9/pvnet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-02-29 14:07:56.000000 PVNet-3.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-29 14:07:56.000000 PVNet-3.0.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-29 14:07:56.000000 PVNet-3.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 14:08:04.297818 PVNet-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-29 14:07:56.000000 PVNet-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:08:04.293818 PVNet-3.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 14:07:56.000000 PVNet-3.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-02-29 14:07:56.000000 PVNet-3.0.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-29 14:07:56.000000 PVNet-3.0.9/tests/test_end2end.py
```

### Comparing `PVNet-3.0.8/LICENSE` & `PVNet-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/PKG-INFO` & `PVNet-3.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PVNet
-Version: 3.0.8
+Version: 3.0.9
 Summary: PVNet
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ocf_datapipes>=3.1.5
```

### Comparing `PVNet-3.0.8/PVNet.egg-info/PKG-INFO` & `PVNet-3.0.9/PVNet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PVNet
-Version: 3.0.8
+Version: 3.0.9
 Summary: PVNet
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ocf_datapipes>=3.1.5
```

### Comparing `PVNet-3.0.8/PVNet.egg-info/SOURCES.txt` & `PVNet-3.0.9/PVNet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/README.md` & `PVNet-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/callbacks.py` & `PVNet-3.0.9/pvnet/callbacks.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/data/base.py` & `PVNet-3.0.9/pvnet/data/base.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/data/datamodule.py` & `PVNet-3.0.9/pvnet/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/data/pv_site_datamodule.py` & `PVNet-3.0.9/pvnet/data/pv_site_datamodule.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/data/utils.py` & `PVNet-3.0.9/pvnet/data/utils.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/data/wind_datamodule.py` & `PVNet-3.0.9/pvnet/data/wind_datamodule.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/models/base_model.py` & `PVNet-3.0.9/pvnet/models/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,27 +296,22 @@
 
         self.weighted_losses = WeightedLosses(forecast_length=self.forecast_len)
 
         self._accumulated_metrics = MetricAccumulator()
         self._accumulated_batches = BatchAccumulator(key_to_keep=self._target_key_name)
         self._accumulated_y_hat = PredAccumulator()
 
-    @property
-    def use_quantile_regression(self):
-        """Whether the model should use quantile regression or simply predict the mean"""
-        return self.output_quantiles is not None
-
-    @property
-    def num_output_features(self):
-        """Number of ouput features he model chould predict for"""
+        # Store whether the model should use quantile regression or simply predict the mean
+        self.use_quantile_regression = self.output_quantiles is not None
+
+        # Store the number of ouput features that the model should predict for
         if self.use_quantile_regression:
-            out_features = self.forecast_len * len(self.output_quantiles)
+            self.num_output_features = self.forecast_len * len(self.output_quantiles)
         else:
-            out_features = self.forecast_len
-        return out_features
+            self.num_output_features = self.forecast_len
 
     def _quantiles_to_prediction(self, y_quantiles):
         """
         Convert network prediction into a point prediction.
 
         Note:
             Implementation copied from:
```

### Comparing `PVNet-3.0.8/pvnet/models/baseline/last_value.py` & `PVNet-3.0.9/pvnet/models/baseline/last_value.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/models/baseline/single_value.py` & `PVNet-3.0.9/pvnet/models/baseline/single_value.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/models/ensemble.py` & `PVNet-3.0.9/pvnet/models/ensemble.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/models/multimodal/basic_blocks.py` & `PVNet-3.0.9/pvnet/models/multimodal/basic_blocks.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/models/multimodal/deep_supervision.py` & `PVNet-3.0.9/pvnet/models/multimodal/deep_supervision.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/models/multimodal/encoders/basic_blocks.py` & `PVNet-3.0.9/pvnet/models/multimodal/encoders/basic_blocks.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/models/multimodal/encoders/encoders2d.py` & `PVNet-3.0.9/pvnet/models/multimodal/encoders/encoders2d.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/models/multimodal/encoders/encoders3d.py` & `PVNet-3.0.9/pvnet/models/multimodal/encoders/encoders3d.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/models/multimodal/encoders/encodersRNN.py` & `PVNet-3.0.9/pvnet/models/multimodal/encoders/encodersRNN.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/models/multimodal/linear_networks/basic_blocks.py` & `PVNet-3.0.9/pvnet/models/multimodal/linear_networks/basic_blocks.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/models/multimodal/linear_networks/networks.py` & `PVNet-3.0.9/pvnet/models/multimodal/linear_networks/networks.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/models/multimodal/multimodal.py` & `PVNet-3.0.9/pvnet/models/multimodal/multimodal.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/models/multimodal/multimodal_base.py` & `PVNet-3.0.9/pvnet/models/multimodal/multimodal_base.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/models/multimodal/nwp_weighting.py` & `PVNet-3.0.9/pvnet/models/multimodal/nwp_weighting.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/models/multimodal/site_encoders/basic_blocks.py` & `PVNet-3.0.9/pvnet/models/multimodal/site_encoders/basic_blocks.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/models/multimodal/site_encoders/encoders.py` & `PVNet-3.0.9/pvnet/models/multimodal/site_encoders/encoders.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/models/multimodal/unimodal_teacher.py` & `PVNet-3.0.9/pvnet/models/multimodal/unimodal_teacher.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/models/multimodal/weather_residual.py` & `PVNet-3.0.9/pvnet/models/multimodal/weather_residual.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/models/utils.py` & `PVNet-3.0.9/pvnet/models/utils.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/optimizers.py` & `PVNet-3.0.9/pvnet/optimizers.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/training.py` & `PVNet-3.0.9/pvnet/training.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/pvnet/utils.py` & `PVNet-3.0.9/pvnet/utils.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/setup.py` & `PVNet-3.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `PVNet-3.0.8/tests/conftest.py` & `PVNet-3.0.9/tests/conftest.py`

 * *Files identical despite different names*

