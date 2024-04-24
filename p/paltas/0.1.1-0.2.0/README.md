# Comparing `tmp/paltas-0.1.1.tar.gz` & `tmp/paltas-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/paltas-0.1.1.tar", last modified: Wed Apr 20 21:59:34 2022, max compression
+gzip compressed data, was "paltas-0.2.0.tar", last modified: Wed Apr 24 13:59:35 2024, max compression
```

## Comparing `paltas-0.1.1.tar` & `paltas-0.2.0.tar`

### file list

```diff
@@ -1,88 +1,90 @@
-drwxr-xr-x   0 sebwagner   (501) staff       (20)        0 2022-04-20 21:59:34.000000 paltas-0.1.1/
--rw-r--r--   0 sebwagner   (501) staff       (20)     5053 2022-04-20 21:59:34.000000 paltas-0.1.1/PKG-INFO
--rw-r--r--   0 sebwagner   (501) staff       (20)     4170 2022-04-15 18:34:17.000000 paltas-0.1.1/README.rst
-drwxr-xr-x   0 sebwagner   (501) staff       (20)        0 2022-04-20 21:59:34.000000 paltas-0.1.1/paltas/
-drwxr-xr-x   0 sebwagner   (501) staff       (20)        0 2022-04-20 21:59:34.000000 paltas-0.1.1/paltas/Analysis/
--rw-r--r--   0 sebwagner   (501) staff       (20)      305 2022-04-15 18:35:34.000000 paltas-0.1.1/paltas/Analysis/__init__.py
--rw-r--r--   0 sebwagner   (501) staff       (20)     7671 2022-04-15 18:35:34.000000 paltas-0.1.1/paltas/Analysis/conv_models.py
--rw-r--r--   0 sebwagner   (501) staff       (20)    19500 2022-04-15 18:35:34.000000 paltas-0.1.1/paltas/Analysis/dataset_generation.py
--rw-r--r--   0 sebwagner   (501) staff       (20)    17720 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Analysis/hierarchical_inference.py
--rw-r--r--   0 sebwagner   (501) staff       (20)    14766 2022-03-02 04:28:11.000000 paltas-0.1.1/paltas/Analysis/loss_functions.py
--rw-r--r--   0 sebwagner   (501) staff       (20)     3885 2022-03-02 04:28:11.000000 paltas-0.1.1/paltas/Analysis/pdf_functions.py
--rw-r--r--   0 sebwagner   (501) staff       (20)     8078 2022-03-02 04:28:11.000000 paltas-0.1.1/paltas/Analysis/posterior_functions.py
--rw-r--r--   0 sebwagner   (501) staff       (20)     4594 2022-01-29 23:21:51.000000 paltas-0.1.1/paltas/Analysis/run_hierarchical.py
--rw-r--r--   0 sebwagner   (501) staff       (20)     9161 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Analysis/train_model.py
-drwxr-xr-x   0 sebwagner   (501) staff       (20)        0 2022-04-20 21:59:34.000000 paltas-0.1.1/paltas/Configs/
-drwxr-xr-x   0 sebwagner   (501) staff       (20)        0 2022-04-20 21:59:34.000000 paltas-0.1.1/paltas/Configs/2203_00690/
--rw-r--r--   0 sebwagner   (501) staff       (20)      893 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_1.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      891 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_10.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      892 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_11.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      892 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_12.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      892 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_13.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      891 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_14.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      890 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_15.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      891 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_16.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      892 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_17.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      890 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_18.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      893 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_19.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      893 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_2.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      892 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_20.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      893 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_3.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      891 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_4.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      892 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_5.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      891 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_6.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      892 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_7.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      891 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_8.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      892 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_9.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      151 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_high_m_min.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      105 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_large_cone_angle.py
--rw-r--r--   0 sebwagner   (501) staff       (20)       97 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_large_los_dz.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      151 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_low_m_min.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      113 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_test_source_smoothing.py
--rw-r--r--   0 sebwagner   (501) staff       (20)     4884 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_train.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      484 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Configs/2203_00690/config_val.py
--rw-r--r--   0 sebwagner   (501) staff       (20)       28 2022-04-15 18:34:17.000000 paltas-0.1.1/paltas/Configs/__init__.py
--rw-r--r--   0 sebwagner   (501) staff       (20)    25320 2022-04-20 21:56:17.000000 paltas-0.1.1/paltas/Configs/config_handler.py
-drwxr-xr-x   0 sebwagner   (501) staff       (20)        0 2022-04-20 21:59:34.000000 paltas-0.1.1/paltas/MainDeflector/
--rw-r--r--   0 sebwagner   (501) staff       (20)       65 2022-03-02 04:28:11.000000 paltas-0.1.1/paltas/MainDeflector/__init__.py
--rw-r--r--   0 sebwagner   (501) staff       (20)     3247 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/MainDeflector/main_deflector_base.py
--rw-r--r--   0 sebwagner   (501) staff       (20)     9081 2022-04-20 21:56:17.000000 paltas-0.1.1/paltas/MainDeflector/simple_deflectors.py
-drwxr-xr-x   0 sebwagner   (501) staff       (20)        0 2022-04-20 21:59:34.000000 paltas-0.1.1/paltas/PointSource/
--rw-r--r--   0 sebwagner   (501) staff       (20)       66 2022-03-02 04:28:11.000000 paltas-0.1.1/paltas/PointSource/__init__.py
--rw-r--r--   0 sebwagner   (501) staff       (20)     1844 2022-03-02 04:28:11.000000 paltas-0.1.1/paltas/PointSource/point_source_base.py
--rw-r--r--   0 sebwagner   (501) staff       (20)     2145 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/PointSource/single_point_source.py
-drwxr-xr-x   0 sebwagner   (501) staff       (20)        0 2022-04-20 21:59:34.000000 paltas-0.1.1/paltas/Sampling/
--rw-r--r--   0 sebwagner   (501) staff       (20)       49 2022-03-02 04:28:11.000000 paltas-0.1.1/paltas/Sampling/__init__.py
--rw-r--r--   0 sebwagner   (501) staff       (20)     9636 2022-04-15 18:34:17.000000 paltas-0.1.1/paltas/Sampling/distributions.py
--rw-r--r--   0 sebwagner   (501) staff       (20)     3943 2022-03-02 04:28:11.000000 paltas-0.1.1/paltas/Sampling/sampler.py
-drwxr-xr-x   0 sebwagner   (501) staff       (20)        0 2022-04-20 21:59:34.000000 paltas-0.1.1/paltas/Sources/
--rw-r--r--   0 sebwagner   (501) staff       (20)      125 2022-04-15 18:34:17.000000 paltas-0.1.1/paltas/Sources/__init__.py
--rw-r--r--   0 sebwagner   (501) staff       (20)    16661 2022-04-20 21:56:17.000000 paltas-0.1.1/paltas/Sources/cosmos.py
--rw-r--r--   0 sebwagner   (501) staff       (20)     3892 2022-04-20 21:56:17.000000 paltas-0.1.1/paltas/Sources/cosmos_sersic.py
--rw-r--r--   0 sebwagner   (501) staff       (20)     6421 2022-04-20 21:56:17.000000 paltas-0.1.1/paltas/Sources/galaxy_catalog.py
--rw-r--r--   0 sebwagner   (501) staff       (20)     2892 2022-04-20 21:56:17.000000 paltas-0.1.1/paltas/Sources/sersic.py
--rw-r--r--   0 sebwagner   (501) staff       (20)     2583 2022-04-20 21:56:17.000000 paltas-0.1.1/paltas/Sources/source_base.py
-drwxr-xr-x   0 sebwagner   (501) staff       (20)        0 2022-04-20 21:59:34.000000 paltas-0.1.1/paltas/Substructure/
--rw-r--r--   0 sebwagner   (501) staff       (20)      129 2022-04-20 21:56:17.000000 paltas-0.1.1/paltas/Substructure/__init__.py
--rw-r--r--   0 sebwagner   (501) staff       (20)     4214 2022-04-15 18:35:34.000000 paltas-0.1.1/paltas/Substructure/los_base.py
--rw-r--r--   0 sebwagner   (501) staff       (20)    21663 2022-04-20 21:56:17.000000 paltas-0.1.1/paltas/Substructure/los_dg19.py
--rw-r--r--   0 sebwagner   (501) staff       (20)    15827 2022-03-02 04:28:11.000000 paltas-0.1.1/paltas/Substructure/nfw_functions.py
--rw-r--r--   0 sebwagner   (501) staff       (20)     3872 2022-04-15 18:35:34.000000 paltas-0.1.1/paltas/Substructure/subhalos_base.py
--rw-r--r--   0 sebwagner   (501) staff       (20)    14738 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Substructure/subhalos_dg19.py
-drwxr-xr-x   0 sebwagner   (501) staff       (20)        0 2022-04-20 21:59:34.000000 paltas-0.1.1/paltas/Utils/
--rw-r--r--   0 sebwagner   (501) staff       (20)      113 2022-04-15 18:34:17.000000 paltas-0.1.1/paltas/Utils/__init__.py
--rw-r--r--   0 sebwagner   (501) staff       (20)     2593 2022-03-17 20:41:53.000000 paltas-0.1.1/paltas/Utils/cosmology_utils.py
--rw-r--r--   0 sebwagner   (501) staff       (20)    12271 2022-03-02 04:28:11.000000 paltas-0.1.1/paltas/Utils/hubble_utils.py
--rw-r--r--   0 sebwagner   (501) staff       (20)     1950 2022-03-02 04:28:11.000000 paltas-0.1.1/paltas/Utils/lenstronomy_utils.py
--rw-r--r--   0 sebwagner   (501) staff       (20)     1417 2022-03-02 04:28:11.000000 paltas-0.1.1/paltas/Utils/power_law.py
--rw-r--r--   0 sebwagner   (501) staff       (20)      336 2022-04-20 21:56:32.000000 paltas-0.1.1/paltas/__init__.py
--rw-r--r--   0 sebwagner   (501) staff       (20)     4310 2022-04-15 18:34:17.000000 paltas-0.1.1/paltas/generate.py
-drwxr-xr-x   0 sebwagner   (501) staff       (20)        0 2022-04-20 21:59:34.000000 paltas-0.1.1/paltas.egg-info/
--rw-r--r--   0 sebwagner   (501) staff       (20)     5053 2022-04-20 21:59:33.000000 paltas-0.1.1/paltas.egg-info/PKG-INFO
--rw-r--r--   0 sebwagner   (501) staff       (20)     2688 2022-04-20 21:59:33.000000 paltas-0.1.1/paltas.egg-info/SOURCES.txt
--rw-r--r--   0 sebwagner   (501) staff       (20)        1 2022-04-20 21:59:33.000000 paltas-0.1.1/paltas.egg-info/dependency_links.txt
--rw-r--r--   0 sebwagner   (501) staff       (20)        1 2022-03-02 02:38:05.000000 paltas-0.1.1/paltas.egg-info/not-zip-safe
--rw-r--r--   0 sebwagner   (501) staff       (20)      137 2022-04-20 21:59:33.000000 paltas-0.1.1/paltas.egg-info/requires.txt
--rw-r--r--   0 sebwagner   (501) staff       (20)        7 2022-04-20 21:59:33.000000 paltas-0.1.1/paltas.egg-info/top_level.txt
--rw-r--r--   0 sebwagner   (501) staff       (20)       80 2022-04-20 21:59:34.000000 paltas-0.1.1/setup.cfg
--rw-r--r--   0 sebwagner   (501) staff       (20)      743 2022-04-20 21:56:48.000000 paltas-0.1.1/setup.py
+drwxr-xr-x   0 swagnercarena   (503) staff       (20)        0 2024-04-24 13:59:35.980827 paltas-0.2.0/
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     1070 2023-10-27 18:45:17.000000 paltas-0.2.0/LICENSE
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     6955 2024-04-24 13:59:35.980748 paltas-0.2.0/PKG-INFO
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     6364 2024-04-24 13:57:34.000000 paltas-0.2.0/README.rst
+drwxr-xr-x   0 swagnercarena   (503) staff       (20)        0 2024-04-24 13:59:35.967544 paltas-0.2.0/paltas/
+drwxr-xr-x   0 swagnercarena   (503) staff       (20)        0 2024-04-24 13:59:35.970541 paltas-0.2.0/paltas/Analysis/
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      338 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Analysis/__init__.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)    11169 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Analysis/conv_models.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)    22427 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Analysis/dataset_generation.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)    18482 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Analysis/hierarchical_inference.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)    14766 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Analysis/loss_functions.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     3885 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Analysis/pdf_functions.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     8078 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Analysis/posterior_functions.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     9946 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Analysis/train_model.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     7788 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Analysis/transformer_models.py
+drwxr-xr-x   0 swagnercarena   (503) staff       (20)        0 2024-04-24 13:59:35.970913 paltas-0.2.0/paltas/Configs/
+-rw-r--r--   0 swagnercarena   (503) staff       (20)       28 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/__init__.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)    28119 2024-04-24 13:57:34.000000 paltas-0.2.0/paltas/Configs/config_handler.py
+drwxr-xr-x   0 swagnercarena   (503) staff       (20)        0 2024-04-24 13:59:35.975550 paltas-0.2.0/paltas/Configs/paper_2203_00690/
+-rw-------   0 swagnercarena   (503) staff       (20)        0 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/__init__.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      941 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_01.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      941 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_02.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      941 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_03.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      939 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_04.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      940 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_05.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      939 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_06.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      940 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_07.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      939 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_08.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      940 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_09.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      939 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_10.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      940 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_11.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      940 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_12.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      940 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_13.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      939 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_14.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      938 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_15.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      939 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_16.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      940 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_17.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      938 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_18.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      941 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_19.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      940 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_20.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      158 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_high_m_min.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      112 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_large_cone_angle.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      104 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_large_los_dz.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      158 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_low_m_min.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      120 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_source_smoothing.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     4642 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_train.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      519 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Configs/paper_2203_00690/config_val.py
+drwxr-xr-x   0 swagnercarena   (503) staff       (20)        0 2024-04-24 13:59:35.976064 paltas-0.2.0/paltas/MainDeflector/
+-rw-r--r--   0 swagnercarena   (503) staff       (20)       65 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/MainDeflector/__init__.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     3247 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/MainDeflector/main_deflector_base.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     9038 2024-04-24 13:57:34.000000 paltas-0.2.0/paltas/MainDeflector/simple_deflectors.py
+drwxr-xr-x   0 swagnercarena   (503) staff       (20)        0 2024-04-24 13:59:35.976628 paltas-0.2.0/paltas/PointSource/
+-rw-r--r--   0 swagnercarena   (503) staff       (20)       66 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/PointSource/__init__.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     1844 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/PointSource/point_source_base.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     2145 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/PointSource/single_point_source.py
+drwxr-xr-x   0 swagnercarena   (503) staff       (20)        0 2024-04-24 13:59:35.977152 paltas-0.2.0/paltas/Sampling/
+-rw-r--r--   0 swagnercarena   (503) staff       (20)       49 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Sampling/__init__.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)    11093 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Sampling/distributions.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     4053 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Sampling/sampler.py
+drwxr-xr-x   0 swagnercarena   (503) staff       (20)        0 2024-04-24 13:59:35.978396 paltas-0.2.0/paltas/Sources/
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      125 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Sources/__init__.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)    17359 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Sources/cosmos.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     4274 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Sources/cosmos_sersic.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     8934 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Sources/galaxy_catalog.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)    11845 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Sources/sersic.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     2583 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Sources/source_base.py
+drwxr-xr-x   0 swagnercarena   (503) staff       (20)        0 2024-04-24 13:59:35.979449 paltas-0.2.0/paltas/Substructure/
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      129 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Substructure/__init__.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     4307 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Substructure/los_base.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)    21538 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Substructure/los_dg19.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)    15827 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Substructure/nfw_functions.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     3876 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Substructure/subhalos_base.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)    14738 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Substructure/subhalos_dg19.py
+drwxr-xr-x   0 swagnercarena   (503) staff       (20)        0 2024-04-24 13:59:35.980312 paltas-0.2.0/paltas/Utils/
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      113 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Utils/__init__.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     3934 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Utils/cosmology_utils.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)    12271 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Utils/hubble_utils.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     1950 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Utils/lenstronomy_utils.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     1417 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/Utils/power_law.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      498 2024-01-25 01:41:39.000000 paltas-0.2.0/paltas/__init__.py
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     5276 2023-10-27 18:45:17.000000 paltas-0.2.0/paltas/generate.py
+drwxr-xr-x   0 swagnercarena   (503) staff       (20)        0 2024-04-24 13:59:35.980486 paltas-0.2.0/paltas.egg-info/
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     6955 2024-04-24 13:59:35.000000 paltas-0.2.0/paltas.egg-info/PKG-INFO
+-rw-r--r--   0 swagnercarena   (503) staff       (20)     2913 2024-04-24 13:59:35.000000 paltas-0.2.0/paltas.egg-info/SOURCES.txt
+-rw-r--r--   0 swagnercarena   (503) staff       (20)        1 2024-04-24 13:59:35.000000 paltas-0.2.0/paltas.egg-info/dependency_links.txt
+-rw-r--r--   0 swagnercarena   (503) staff       (20)        1 2023-10-27 18:46:35.000000 paltas-0.2.0/paltas.egg-info/not-zip-safe
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      161 2024-04-24 13:59:35.000000 paltas-0.2.0/paltas.egg-info/requires.txt
+-rw-r--r--   0 swagnercarena   (503) staff       (20)        7 2024-04-24 13:59:35.000000 paltas-0.2.0/paltas.egg-info/top_level.txt
+-rw-r--r--   0 swagnercarena   (503) staff       (20)       80 2024-04-24 13:59:35.981015 paltas-0.2.0/setup.cfg
+-rw-r--r--   0 swagnercarena   (503) staff       (20)      743 2023-10-27 19:14:59.000000 paltas-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `paltas-0.1.1/paltas/Analysis/conv_models.py` & `paltas-0.2.0/paltas/Analysis/conv_models.py`

 * *Files 27% similar despite different names*

```diff
@@ -102,46 +102,41 @@
 	for i in range(2,blocks+1):
 		x = _xresnet_block(x,filters,kernel_size,1,conv_shortcut=False,
 			name=name+'_block%d'%(i),trainable=trainable)
 
 	return x
 
 
-def build_xresnet34(img_size,num_outputs,custom_head=False,
-	train_only_head=False):
-	""" Build the xresnet34 model described in
+def _xresnet34(conv_inputs,num_outputs,custom_head=False,trainable=True,
+	output_trainable=True):
+	"""Run a convolutional input through the xresnet34 model described in
 	https://arxiv.org/pdf/1812.01187.pdf
 
 	Args:
-		img_size ((int,int,int)): A tuple with shape (pix,pix,freq) that
-			describes the size of the input images.
+		conv_inputs (KerasTensor): A KerasTensor with dimension (batch_size,
+			image_size,image_size,n_channels) that will be used as the input to
+			the xresent_34 model.
 		num_outputs (int): The number of outputs to predict
 		custom_head (bool): If true, then add a custom head at the end of
 			xresnet34 in line with what' used in the fastai code.
-		train_only_head (bool): If true, only train the head of the network.
+		trainable (bool): If False, do not train the convolutional weights.
+		output_trainable (bool): If False do not train the last dense layer.
 
 	Returns:
-		(keras.Model): An instance of the xresnet34 model implemented in
-		Keras.
+		(KerasTensor): The outputs of the xresnet34 with dimension (batch_size,
+		num_outputs).
 	"""
 
-	# If we train only the head, then none of the previous weights should be
-	# trainable
-	trainable = not train_only_head
-
 	# Assume the first dimension is the batch size
 	bn_axis = -1
 
-	# Initialize the inputs
-	inputs = layers.Input(shape=img_size)
-
 	# Build the stem of the resnet
 	# Conv 1 of stem
 	x = layers.ZeroPadding2D(padding=((1,1),(1,1)),name='stem_pad1',
-		trainable=trainable)(inputs)
+		trainable=trainable)(conv_inputs)
 	x = layers.Conv2D(32,3,strides=2,use_bias=False,name='stem_conv1',
 		trainable=trainable)(x)
 	x = layers.BatchNormalization(axis=bn_axis,epsilon=1e-5,momentum=0.1,
 		name='stem_bn1',trainable=trainable)(x)
 	x = layers.Activation('relu',name='stem_relu1',trainable=trainable)(x)
 
 	# Conv 2 of stem
@@ -178,21 +173,118 @@
 	x = _xresnet_stack(x,filters=512,kernel_size=3,strides=2,
 		conv_shortcut=True,name='stack4',blocks=3,trainable=trainable)
 
 	# Conduct the pooling and a dense transform to the final prediction
 	x = layers.GlobalAveragePooling2D(name='avg_pool')(x)
 	if custom_head:
 		x = layers.BatchNormalization(axis=bn_axis,epsilon=1e-5,momentum=0.1,
-			name='head_bn1')(x)
-		x = layers.Dense(512,use_bias=False,name='head_dense1')(x)
+			name='head_bn1',trainable=output_trainable)(x)
+		x = layers.Dense(512,use_bias=False,name='head_dense1',
+			trainable=output_trainable)(x)
 		x = layers.Activation('relu',name='head_relu1')(x)
 		x = layers.BatchNormalization(axis=bn_axis,epsilon=1e-5,momentum=0.1,
-			name='head_bn2')(x)
-		x = layers.Dense(num_outputs,use_bias=False,name='head_dense2')(x)
+			name='head_bn2',trainable=output_trainable)(x)
+		x = layers.Dense(num_outputs,use_bias=False,name='head_dense2',
+			trainable=output_trainable)(x)
 		outputs = layers.BatchNormalization(axis=bn_axis,epsilon=1e-5,
-			momentum=0.1,name='head_bn3')(x)
+			momentum=0.1,name='head_bn3',trainable=output_trainable)(x)
 	else:
-		outputs = layers.Dense(num_outputs,name='output_dense')(x)
+		outputs = layers.Dense(num_outputs,name='output_dense',
+			trainable=output_trainable)(x)
+
+	return outputs
+
+
+def build_xresnet34(img_size,num_outputs,custom_head=False,
+	train_only_head=False):
+	""" Build the xresnet34 model described in
+	https://arxiv.org/pdf/1812.01187.pdf
+
+	Args:
+		img_size ((int,int,int)): A tuple with shape (pix,pix,freq) that
+			describes the size of the input images.
+		num_outputs (int): The number of outputs to predict
+		custom_head (bool): If true, then add a custom head at the end of
+			xresnet34 in line with what' used in the fastai code.
+		train_only_head (bool): If true, only train the head of the network.
+
+	Returns:
+		(keras.Model): An instance of the xresnet34 model implemented in
+		Keras.
+	"""
+
+	# If we train only the head, then none of the previous weights should be
+	# trainable
+	trainable = not train_only_head
+
+	# Initialize the inputs
+	inputs = layers.Input(shape=img_size)
+
+	# Pass the inputs through out xresnet 34 model.
+	outputs = _xresnet34(inputs,num_outputs,custom_head=custom_head,
+		trainable=trainable,output_trainable=True)
 
 	model = Model(inputs=inputs,outputs=outputs)
 
 	return model
+
+
+def build_xresnet34_fc_inputs(img_size,num_outputs,num_fc_inputs,
+	train_only_head=False):
+	""" Build the xresnet34 model described in
+	https://arxiv.org/pdf/1812.01187.pdf but include a few more
+	fully connected layers and introduce additional inputs (i.e.
+	float values associated with the images) into the fully
+	connected layers.
+
+	Args:
+		img_size ((int,int,int)): A tuple with shape (pix,pix,freq) that
+			describes the size of the input images.
+		num_outputs (int): The number of outputs to predict
+		num_fc_inputs (int): The number of input floats associated to each
+			image.
+		train_only_head (bool): If true, only train the head of the network.
+
+	Returns:
+		(keras.Model): An instance of the xresnet34 model implemented in
+		Keras.
+	"""
+
+	# If we train only the head, then none of the previous weights should be
+	# trainable
+	trainable = not train_only_head
+
+	# Initialize the image inputs
+	inputs_image = layers.Input(shape=img_size)
+
+	# Initialize the inputs to the fully connected layer.
+	inputs_fc = layers.Input(shape=(num_fc_inputs,))
+
+	# The output of our xresnet is not the input to our fc stack
+	xresnet_output = 512
+
+	# Pass the inputs through out xresnet 34 model.
+	xr_outputs = _xresnet34(inputs_image,xresnet_output,custom_head=False,
+		trainable=trainable,output_trainable=trainable)
+	xr_outputs = layers.Activation('relu',name='fc_relu1')(xr_outputs)
+
+	# Assume the first dimension is the batch size
+	bn_axis = -1
+
+	# Concatenate the redshifts to the xresnet output.
+	x = layers.Concatenate(axis=1,name='fc_concat')([xr_outputs,inputs_fc])
+	x = layers.Activation('relu',name='fc_relu2')(x)
+	x = layers.BatchNormalization(axis=bn_axis,epsilon=1e-5,momentum=0.1,
+		name='fc_bn1',trainable=True)(x)
+	x = layers.Dense(256,use_bias=True,name='fc_dense1',trainable=True)(x)
+	x = layers.Activation('relu',name='fc_relu3')(x)
+	x = layers.BatchNormalization(axis=bn_axis,epsilon=1e-5,momentum=0.1,
+		name='fc_bn2',trainable=True)(x)
+	x = layers.Dense(128,use_bias=True,name='fc_dense2',trainable=True)(x)
+	x = layers.Activation('relu',name='fc_relu4')(x)
+	x = layers.BatchNormalization(axis=bn_axis,epsilon=1e-5,momentum=0.1,
+		name='fc_bn3',trainable=True)(x)
+	outputs = layers.Dense(num_outputs,use_bias=True,name='fc_dense3')(x)
+
+	model = Model(inputs=[inputs_image,inputs_fc],outputs=outputs)
+
+	return model
```

### Comparing `paltas-0.1.1/paltas/Analysis/dataset_generation.py` & `paltas-0.2.0/paltas/Analysis/dataset_generation.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 import tensorflow as tf
 import pandas as pd
 import glob, os
 from tqdm import tqdm
 from lenstronomy.SimulationAPI.observation_api import SingleBand
 import warnings
 from scipy.ndimage import rotate
-
+import h5py
 # Global filters on the python warnings. Using this since filter
 # behaviour is a bit weird.
 DEFAULTVALUEWARNING = True
 
 
 def normalize_outputs(metadata,learning_params,input_norm_path,
 	log_learning_params=None):
-	""" Normalize the outputs of the network
+	"""Normalize the outputs of the network
 
 	Args:
 		metadata(pd.DataFrame): A pandas object containing the metadata
 		learning_params ([str,...]): A list of strings containing the
 			parameters that the network is expected to learn.
 		input_norm_path (str): The path to a csv that contains the
 			normalization to be applied to the output parameters. If the
@@ -66,26 +66,26 @@
 		if log_learning_params is not None:
 			log_norm_dict = pd.DataFrame(columns=['parameter','mean','std'])
 			log_norm_dict['parameter'] = log_learning_params
 			# Calculate the normalization for each parameter
 			log_data = metadata[log_learning_params].to_numpy()
 			log_norm_dict['mean'] = np.mean(np.log(log_data),axis=0)
 			log_norm_dict['std'] = np.std(np.log(log_data),axis=0)
-			norm_dict = norm_dict.append(log_norm_dict)
+			norm_dict = pd.concat([norm_dict, log_norm_dict], ignore_index=True)
 
 		# Set parameter to the index
 		norm_dict = norm_dict.set_index('parameter')
 		norm_dict.to_csv(input_norm_path)
 
 	return norm_dict
 
 
 def unnormalize_outputs(input_norm_path,learning_params,mean,standard_dev=None,
 	cov_mat=None):
-	""" Given NN outputs, undo the normalization step and return the parameters
+	"""Given NN outputs, undo the normalization step and return the parameters
 	in the original space
 
 	Args:
 		input_norm_path (str): The path to a csv that contains the
 			normalization to be undone.
 		learning_params ([str,...]): A list of strings containing the
 			parameters that the network is expected to learn. Length n_params.
@@ -119,15 +119,15 @@
 		# If provided we want to correct the covariance matrix
 		if cov_mat is not None:
 			cov_mat[:,lpi,:] *= param_std
 			cov_mat[:,:,lpi] *= param_std
 
 
 def kwargs_detector_to_tf_noise(image,kwargs_detector):
-	""" Add noise to the tf tensor provided in agreement with kwargs_detector
+	"""Add noise to the tf tensor provided in agreement with kwargs_detector
 
 	Args:
 		image (tf.Tensor): A tensorflow tensor containing the image
 		kwargs_detector (dict): A dictionary containing the detector kwargs
 			used to generate the noise on the fly.
 
 	Returns:
@@ -147,49 +147,69 @@
 		variance /= single_band.ccd_gain
 	noise += tf.random.normal(tf.shape(image)) * variance
 
 	return noise
 
 
 def generate_tf_record(npy_folder,learning_params,metadata_path,
-	tf_record_path):
-	""" Generate a TFRecord file from a directory of numpy files.
+	tf_record_path,h5=False):
+	"""Generate a TFRecord file from a directory of numpy or h5py files.
 
 	Args:
 		root_path (str): The path to the folder containing the numpy files.
 		learning_params ([str,...]): A list of strings containing the
 			parameters that the network is expected to learn.
 		metadata_path (str):  The path to the csv file containing the
 			image metadata.
 		tf_record_path (str): The path to which the TFRecord will be saved
+		h5 (bool): Boolean for whether the images were generated as h5 files (True) or numpy (False).
 	"""
-	# Pull the list of numpy filepaths from the directory
+	# Pull the list of numpy and/or h5 filepaths from the directory. Assumes there is only one h5 file in the folder.
 	npy_file_list = glob.glob(os.path.join(npy_folder,'image_*.npy'))
+	npy_file_list = list(sorted(npy_file_list))
+	h5_file = os.path.join(npy_folder,'image_data.h5')
+
 	# Open label csv
 	metadata = pd.read_csv(metadata_path, index_col=None)
 
 	# Warn the user a default value of 0 will be used for parameters not
 	# present in the metadata file.
 	global DEFAULTVALUEWARNING
 	for param in learning_params:
 		if param not in metadata and DEFAULTVALUEWARNING:
 			warnings.warn('One or more parameters in learning_params is not '+
 				' present in the metadata. A default value of 0 will be used.',
 				category=RuntimeWarning)
 			DEFAULTVALUEWARNING = False
-
-	# Initialize the writer object and write the lens data
+	# If h5 is used, the number of images is the length of the first dimension in the h5 file, rather than the number of h5 files:
+	if h5: 
+		with h5py.File(h5_file,'r') as f0:
+			number_of_files = f0['data'].shape[0]
+	else: 
+		number_of_files = len(npy_file_list)
+   	# Initialize the writer object and write the lens data
+	print('Saving '+str(number_of_files)+' files into the tf record')
 	with tf.io.TFRecordWriter(tf_record_path) as writer:
-		for npy_file in tqdm(npy_file_list):
-			# Pull the index from the filename
-			index = int(npy_file[-11:-4])
-			image_shape = np.load(npy_file).shape
+		if h5:
+			f = h5py.File(h5_file, "r")
+		# Iteratively retrieves images from list of npy files, or images within the h5 file:  
+		for file_number in tqdm(range(number_of_files)):
+			if h5:
+				index = int(file_number)
+				image = f['data'][()][index]
+				image_shape = image.shape
+			else:
+				npy_file = npy_file_list[file_number]
+				# Pull the index from the filename
+				index = int(npy_file[-11:-4])
+				image = np.load(npy_file)
+				image_shape = image.shape
 			# The image must be converted to a tf string feature
 			image_feature = tf.train.Feature(bytes_list=tf.train.BytesList(
-				value=[np.load(npy_file).astype(np.float32).tostring()]))
+				value=[image.astype(np.float32).tostring()]))
 			# Initialize a feature dictionary with the image, the height,
 			# and the width
 			feature = {
 				'image': image_feature,
 				'height': tf.train.Feature(
 					int64_list=tf.train.Int64List(value=[image_shape[0]])),
 				'width': tf.train.Feature(
@@ -207,20 +227,21 @@
 				feature[param] = tf.train.Feature(
 					float_list=tf.train.FloatList(value=[value]))
 			# Create the tf example object
 			example = tf.train.Example(features=tf.train.Features(
 				feature=feature))
 			# Write out the example to the TFRecord file
 			writer.write(example.SerializeToString())
-
+		if h5: 
+			f.close()
 
 def generate_tf_dataset(tf_record_path,learning_params,batch_size,
 	n_epochs,norm_images=False,input_norm_path=None,kwargs_detector=None,
-	log_learning_params=None):
-	"""	Generate a TFDataset that a model can be trained with.
+	log_learning_params=None,shuffle=True):
+	"""Generate a TFDataset that a model can be trained with.
 
 	Args:
 		tf_record_paths (str, or [str,...]) A string specifying the paths to
 			the TFRecords that will be used in the dataset. Can also be a list
 			of strings for specifying multiple tf_record_paths.
 		learning_params ([str,...]): A list of strings containing the
 			parameters that the network is expected to learn.
@@ -233,14 +254,15 @@
 			no normalization will be applied.
 		kwargs_detector (dict): A dictionary containing the detector kwargs
 			used to generate the noise on the fly. If None no additional
 			noise will be added.
 		log_learning_params ([str,...]): A list of strings containing the
 			parameters that the network is expected to learn the log of. Can
 			be None.
+		shuffle (bool): if True (default is True), randomly shuffles dataset.
 
 	Returns:
 		(tf.Dataset): A tf.Dataset object that returns the input image and the
 		output labels.
 
 	Notes:
 		Do not use kwargs_detector if noise was already added during dataset
@@ -309,21 +331,23 @@
 	buffer_size = int(batch_size*1.2)
 
 	# Set the feature decoder as the mapping function. Drop the remainder
 	# in the case that batch_size does not divide the number of training
 	# points exactly
 	dataset = raw_dataset.map(parse_image_features,
 		num_parallel_calls=tf.data.experimental.AUTOTUNE).repeat(
-		n_epochs).shuffle(buffer_size=buffer_size).batch(batch_size).prefetch(
-		tf.data.experimental.AUTOTUNE)
+		n_epochs)
+	if shuffle:
+		dataset = dataset.shuffle(buffer_size=buffer_size)
+	dataset = dataset.batch(batch_size).prefetch(tf.data.experimental.AUTOTUNE)
 	return dataset
 
 
 def rotate_params_batch(learning_params,output,rot_angle):
-	""" Rotate a batch of lensing parameters according to a specified rotation
+	"""Rotate a batch of lensing parameters according to a specified rotation
 	angle.
 
 	Args:
 		learning_params ([str,...]): A list of strings containing the
 			parameters that the network is expected to learn.
 		output (np.array): A numpy array of dimension (batch_size,n_outputs)
 			containing the true parameter values for each image in the batch.
@@ -356,15 +380,15 @@
 		yi = learning_params.index('main_deflector_parameters_gamma2')
 		x,y = rotate_param(output[:,xi],output[:,yi],2*rot_angle)
 		output[:,xi] = x
 		output[:,yi] = y
 
 
 def rotate_covariance_batch(learning_params,coavriance_batch,rot_angle):
-	""" Rotate a batch of lensing parameters according to a specified rotation
+	"""Rotate a batch of covariance matrices according to a specified rotation
 	angle.
 
 	Args:
 		learning_params ([str,...]): A list of strings containing the
 			parameters that the network is expected to learn.
 		coavriance_batch (np.array): A numpy array of dimension
 			(batch_size,n_outputs,n_outputs) containing the covariance values
@@ -408,15 +432,15 @@
 		yi+=1
 		rot_mat = rotation_matrix(2*rot_angle)
 		coavriance_batch[:,xi:yi,xi:yi] = np.dot(rot_mat,
 			np.dot(coavriance_batch[:,xi:yi,xi:yi],rot_mat.T).T).T
 
 
 def rotate_image_batch(image_batch,learning_params,output,rot_angle):
-	""" Rotate a batch of strong lensing images and the corresponding lensing
+	"""Rotate a batch of strong lensing images and the corresponding lensing
 	parameters
 
 	Args:
 		image_batch (np.array): A numpy image array of shape (batch_size,
 			height,width,n_channels) that will be rotated.
 		learning_params ([str,...]): A list of strings containing the
 			parameters that the network is expected to learn.
@@ -439,16 +463,16 @@
 	rotate_params_batch(learning_params,output,rot_angle)
 
 	return image_batch
 
 
 def generate_rotations_dataset(tf_record_path,learning_params,batch_size,
 	n_epochs,norm_images=False,input_norm_path=None,kwargs_detector=None,
-	log_learning_params=None):
-	"""	Returns a generator that builds off of a TFDataset by adding random
+	log_learning_params=None,shuffle=True):
+	"""Returns a generator that builds off of a TFDataset by adding random
 	rotations to the images and parameters.
 
 	Args:
 		tf_record_paths (str, or [str,...]) A string specifying the paths to
 			the TFRecords that will be used in the dataset. Can also be a list
 			of strings for specifying multiple tf_record_paths.
 		learning_params ([str,...]): A list of strings containing the
@@ -462,23 +486,25 @@
 			no normalization will be applied.
 		kwargs_detector (dict): A dictionary containing the detector kwargs
 			used to generate the noise on the fly. If None no additional
 			noise will be added.
 		log_learning_params ([str,...]): A list of strings containing the
 			parameters that the network is expected to learn the log of. Can
 			be None.
+		shuffle (bool): if True (default is True), randomly shuffles dataset.
 
 	Returns:
 		(generator): A generator that returns a tuple with the rotated image
 		and the parameter values.
 	"""
 	# Create our base tf dataset without normalization
 	base_dataset = generate_tf_dataset(tf_record_path,learning_params,
 		batch_size,n_epochs,norm_images=norm_images,
-		kwargs_detector=kwargs_detector,log_learning_params=log_learning_params)
+		kwargs_detector=kwargs_detector,log_learning_params=log_learning_params,
+		shuffle=shuffle)
 
 	# If normalization file is provided use it
 	if input_norm_path is not None:
 		norm_dict = pd.read_csv(input_norm_path,index_col='parameter')
 	else:
 		norm_dict = None
 
@@ -501,7 +527,53 @@
 					lens_param_batch[:,lpi] -= norm_dict['mean'][param]
 					lens_param_batch[:,lpi] /= norm_dict['std'][param]
 			# Yield the rotated image and parameters
 			yield image_batch, lens_param_batch
 
 	# Return a rotation generator on our base dataset.
 	return rotation_generator(base_dataset)
+
+
+def generate_params_as_input_dataset(base_dataset,params_as_inputs,
+	all_params):
+	"""Generate a dataset where some of the lens parameters are treated as
+	inputs to the model.
+
+	Args:
+		base_dataset (generator): A generator that yields a tuple containing
+			the images and the parameters values.
+		params_as_inputs ([str,...]): A list of strings containing the
+			parameters that will be turned into inputs for the model.
+		all_params ([str,...]): A list of strings containing the parameters
+			that will be outputted by the generator.
+
+	Returns:
+		(generator): A generator that returns a tuple with the inputs (which
+		are the image and the scalar input values), and the outputs parameter
+		values.
+	"""
+
+	# Set a boolean mask for the parameters we want to use as inputs and the
+	# parameters we want to use as outputs.
+	param_is_input = np.array([param in params_as_inputs for param in all_params])
+	param_is_output = ~param_is_input
+
+	def param_extractor(dataset):
+		# Iterate through the images and parameters in the dataset and
+		# reorganize the parameters as needed.
+		for image_batch,all_param_batch in dataset:
+			# If the images or parameters are tensors, do the
+			# appropriate conversion.
+			if isinstance(image_batch,tf.Tensor):
+				image_batch = image_batch.numpy()
+			if isinstance(all_param_batch,tf.Tensor):
+				all_param_batch = all_param_batch.numpy()
+
+			scalar_inputs = all_param_batch[:,param_is_input]
+			outputs_batch = all_param_batch[:,param_is_output]
+
+			# Yield the inputs, which are the image and the scalar inputs, along
+			# with the parameters we want to learn.
+			yield [image_batch, scalar_inputs], outputs_batch
+
+	# Return the generator on the base dataset
+	return param_extractor(base_dataset)
```

### Comparing `paltas-0.1.1/paltas/Analysis/hierarchical_inference.py` & `paltas-0.2.0/paltas/Analysis/hierarchical_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # -*- coding: utf-8 -*-
 """
 Conduct hierarchical inference on a population of lenses.
 
 This module contains the tools to conduct hierarchical inference on our
 network posteriors.
 """
+import warnings
 import numpy as np
 from scipy import special
 import numba
 
+# Global error filters for python warnings.
+LINALGWARNING = True
 
 # The predicted samples need to be et as a global variable for the pooling to
 # be efficient when done by emcee. This will have shape (num_params,num_samps,
 # batch_size).
 predict_samps_hier = None
 
 # As with the predicted samples, the predicted mu and cov for the analytical
@@ -104,19 +107,25 @@
 	"""
 	# This implements the final formula derived in the appendix of
 	# Wagner-Carena et al. 2021.
 
 	# Calculate the values of eta and the combined precision matrix
 	prec_comb = prec_pred+prec_omega-prec_omega_i
 
-	# This is not guaranteed to return a valid precision matrix. When it
-	# doesn't the analytical equation used here is wrong. In those cases
-	# return -np.inf
-	eigvals = np.linalg.eigvals(prec_comb.astype(np.complex128))
-	if (np.any(np.real(eigvals)<=0) or np.any(np.imag(eigvals)!=0)):
+	# prec_comb is not guaranteed to be a valid precision matrix.
+	# When it isn't, the analytical equation used here is wrong.
+	# In those cases, return -np.inf.
+	# To check the matrix is positive definite, we check that is symmetric
+	# and that its Cholesky decomposition exists
+	# (see https://stackoverflow.com/questions/16266720)
+	if not np.array_equal(prec_comb, prec_comb.T):
+		return -np.inf
+	try:
+		np.linalg.cholesky(prec_comb)
+	except Exception:  # LinAlgError, but numba can't match exceptions
 		return -np.inf
 
 	cov_comb = np.linalg.inv(prec_comb)
 	eta_pred = np.dot(prec_pred,mu_pred)
 	eta_omega_i = np.dot(prec_omega_i,mu_omega_i)
 	eta_omega = np.dot(prec_omega,mu_omega)
 	eta_comb = eta_pred + eta_omega - eta_omega_i
@@ -341,29 +350,46 @@
 
 		if self.predictions_init is False:
 			raise RuntimeError('Must set predictions or behaviour is '
 				+'ill-defined.')
 
 		global mu_pred_array
 		global prec_pred_array
+		global LINALGWARNING
 
 		# Start with the prior on omega
 		lprior = log_p_omega(hyperparameters,self.eval_func_omega)
 
 		# No need to evaluate the samples if the proposal is outside the prior.
 		if lprior == -np.inf:
 			return lprior
 
 		# Extract mu_omega and prec_omega from the provided hyperparameters
 		mu_omega = hyperparameters[:len(hyperparameters)//2]
 		cov_omega = np.diag(np.exp(hyperparameters[len(hyperparameters)//2:]*2))
-		prec_omega = np.linalg.inv(cov_omega)
-
-		like_ratio = self.log_integral_product(mu_pred_array,prec_pred_array,
-			self.mu_omega_i,self.prec_omega_i,mu_omega,prec_omega)
+		try:
+			prec_omega = np.linalg.inv(cov_omega)
+		except np.linalg.LinAlgError:
+			# Singular covariance matrix
+			if LINALGWARNING:
+				warnings.warn('Singular covariance matrix',
+					category=RuntimeWarning)
+				LINALGWARNING = False
+			return -np.inf
+
+		try:
+			like_ratio = self.log_integral_product(mu_pred_array,prec_pred_array,
+				self.mu_omega_i,self.prec_omega_i,mu_omega,prec_omega)
+		except np.linalg.LinAlgError:
+			# Something else was singular, too bad
+			if LINALGWARNING:
+				warnings.warn('Singular covariance matrix',
+					category=RuntimeWarning)
+				LINALGWARNING = False
+			return -np.inf
 
 		# Return the likelihood and the prior combined
 		return lprior + like_ratio
 
 
 class ProbabilityClassEnsemble(ProbabilityClassAnalytical):
 	""" An extension of the class ProbabilityClassAnalytical that allows for
```

### Comparing `paltas-0.1.1/paltas/Analysis/loss_functions.py` & `paltas-0.2.0/paltas/Analysis/loss_functions.py`

 * *Files identical despite different names*

### Comparing `paltas-0.1.1/paltas/Analysis/pdf_functions.py` & `paltas-0.2.0/paltas/Analysis/pdf_functions.py`

 * *Files identical despite different names*

### Comparing `paltas-0.1.1/paltas/Analysis/posterior_functions.py` & `paltas-0.2.0/paltas/Analysis/posterior_functions.py`

 * *Files identical despite different names*

### Comparing `paltas-0.1.1/paltas/Analysis/train_model.py` & `paltas-0.2.0/paltas/Analysis/train_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 """
 Initialize and train a neural posterior estimator on a strong lensing image
 dataset generated by paltas.
 """
 import argparse, os, sys, glob, math
 from importlib import import_module
 import tensorflow as tf
-from . import dataset_generation, loss_functions, conv_models
+from paltas.Analysis import dataset_generation, loss_functions, conv_models
 from tensorflow.keras.callbacks import TensorBoard, ModelCheckpoint
 from tensorflow.keras import optimizers
 import pandas as pd
-
+import h5py
 
 def parse_args():
 	"""Parse the input arguments by the user
 
 	Returns:
 		(argparse.Namespace): An instance of the Namespace object with the
 		users provided values.
@@ -23,14 +23,16 @@
 	# Initialize the parser and the possible inputs
 	parser = argparse.ArgumentParser()
 	parser.add_argument('training_config', help='Path to configuration for '
 		+'training the model.')
 	parser.add_argument('--tensorboard_dir', default=None, type=str,
 		dest='tensorboard_dir', help='Optional path to save a tensorboard ' +
 		'output to')
+	parser.add_argument('--h5', action='store_true',
+		help='Load images from .h5 files rather than .npy')
 	args = parser.parse_args()
 	return args
 
 
 def main():
 	"""The main script to run from the command line.
 	"""
@@ -54,47 +56,44 @@
 	# A list of the paths to the TFRecords for the training images
 	tfr_train_paths = config_module.tfr_train_paths
 	# The path to the TFRecord for the validation images
 	tfr_val_path = config_module.tfr_val_path
 	# The list of learning parameters to use
 	learning_params = config_module.learning_params
 	# Which parameters to put in log space
-	if hasattr(config_module,'log_learning_params'):
-		log_learning_params = config_module.log_learning_params
-	else:
-		log_learning_params = []
+	log_learning_params = getattr(config_module,'log_learning_params',[])
 	num_params = len(learning_params+log_learning_params)
 	# Which parameters to consider flipping
-	if hasattr(config_module,'flip_pairs'):
-		flip_pairs = config_module.flip_pairs
-	else:
-		flip_pairs = None
+	flip_pairs = getattr(config_module,'flip_pairs',None)
 	# Which parameters to weight
-	if hasattr(config_module,'weight_terms'):
-		weight_terms = config_module.weight_terms
-	else:
-		weight_terms = None
+	weight_terms = getattr(config_module,'weight_terms',None)
 	# Whether to train the full model or only the head
-	if hasattr(config_module,'train_only_head'):
-		train_only_head = config_module.train_only_head
-	else:
-		train_only_head = False
+	train_only_head = getattr(config_module,'train_only_head',False)
 	# A list to the paths of the fodlers containing the npy images
 	# for training
 	npy_folders_train = config_module.npy_folders_train
 	# Number of steps per epoch is number of examples over the batch size
-	n_npy_files = 0
+	n_images = 0
 	for npy_folder in npy_folders_train:
-		n_npy_files += len(glob.glob(os.path.join(npy_folder,'image_*.npy')))
-	steps_per_epoch = n_npy_files//batch_size
+		if not args.h5:
+			n_images += len(glob.glob(os.path.join(npy_folder,'image_*.npy')))
+		# Assumes there is only 1 h5 file per folder
+		else: 
+			with h5py.File(os.path.join(npy_folder,'image_data.h5'),'r') as f0:
+				n_images += f0['data'].shape[0]
+	steps_per_epoch = n_images//batch_size
 	# The path to the fodler containing the npy images
 	# for validation
 	npy_folder_val = config_module.npy_folder_val
 	# Get the number of validation files as well
-	n_val_npy = len(glob.glob(os.path.join(npy_folder_val,'image_*.npy')))
+	if not args.h5:
+		n_val_npy = len(glob.glob(os.path.join(npy_folder_val,'image_*.npy')))
+	else: 
+		with h5py.File(os.path.join(npy_folder_val,'image_data.h5'),'r') as f0:
+			n_val_npy = f0['data'].shape[0]
 	# A list of the paths to the training metadata
 	metadata_paths_train = config_module.metadata_paths_train
 	# The path to the validation metadata
 	metadata_path_val = config_module.metadata_path_val
 	# The path to the csv file to read from / write to for normalization
 	# of learning parameters.
 	input_norm_path = config_module.input_norm_path
@@ -112,70 +111,77 @@
 	model_weights_init = config_module.model_weights_init
 	model_weights = config_module.model_weights
 	# The learning rate for the model
 	learning_rate = config_module.learning_rate
 	# Whether or not to apply a random rotation to the input image
 	random_rotation = config_module.random_rotation
 
-	# Set the random seed for our network
-	# tf.random.set_seed(random_seed)
+	params_as_inputs = getattr(config_module,'params_as_inputs',[])
+	all_params = params_as_inputs + learning_params
 
 	# Check for tf records for train and validation and prepare them
 	# if needed
 	print('Checking for training data.')
 	for i, tf_path in enumerate(tfr_train_paths):
 		if not os.path.exists(tf_path):
 			print('Generating new TFRecord at %s'%(tf_path))
 			dataset_generation.generate_tf_record(npy_folders_train[i],
-				learning_params+log_learning_params,metadata_paths_train[i],
-				tf_path)
+				all_params+log_learning_params,metadata_paths_train[i],
+				tf_path,h5=args.h5)
 		else:
 			print('TFRecord found at %s'%(tf_path))
 
 	print('Checking for validation data.')
 	if not os.path.exists(tfr_val_path):
 		print('Generating new TFRecord at %s'%(tfr_val_path))
 		dataset_generation.generate_tf_record(npy_folder_val,
-			learning_params+log_learning_params,metadata_path_val,tfr_val_path)
+			all_params+log_learning_params,metadata_path_val,tfr_val_path,h5=args.h5)
 	else:
 		print('TFRecord found at %s'%(tfr_val_path))
 
 	# Normalize outputs if requested
 	if input_norm_path is not None:
 		print('Checking for normalization csv')
 		metadata = pd.read_csv(metadata_paths_train[0])
-		dataset_generation.normalize_outputs(metadata,learning_params,
+		dataset_generation.normalize_outputs(metadata,all_params,
 			input_norm_path,log_learning_params=log_learning_params)
 
 	# If no random rotations are required, the best tool is a tf dataset.
 	# Otherwise, it's better to take the output of the tf dataset and then
 	# run it through a generator that will do the rotations on the batches
 	# for us.
 	if random_rotation:
 		# Get a generator object that returns rotated images and parameters.
 		tf_dataset_t = dataset_generation.generate_rotations_dataset(
-			tfr_train_paths,learning_params,batch_size,n_epochs,
+			tfr_train_paths,all_params,batch_size,n_epochs,
 			norm_images=norm_images,input_norm_path=input_norm_path,
 			kwargs_detector=kwargs_detector,
 			log_learning_params=log_learning_params)
 	else:
 		# Turn our tf records into tf datasets for training and validation
 		tf_dataset_t = dataset_generation.generate_tf_dataset(tfr_train_paths,
-			learning_params,batch_size,n_epochs,norm_images=norm_images,
+			all_params,batch_size,n_epochs,norm_images=norm_images,
 			input_norm_path=input_norm_path,kwargs_detector=kwargs_detector,
 			log_learning_params=log_learning_params)
 	# We shouldn't be adding random noise to validation images. They should
 	# be generated with noise
 	if kwargs_detector is not None:
 		print('Make sure your validation images already have noise! Noise ' +
 			'will not be added on the fly for validation.')
 	tf_dataset_v = dataset_generation.generate_tf_dataset(tfr_val_path,
-		learning_params,min(batch_size,n_val_npy),1,norm_images=norm_images,
-		input_norm_path=input_norm_path,kwargs_detector=None,
-		log_learning_params=log_learning_params)
+		all_params,min(batch_size,n_val_npy),1,
+		norm_images=norm_images,input_norm_path=input_norm_path,
+		kwargs_detector=None,log_learning_params=log_learning_params)
+
+	# If some of the parameters need to be extracted as inputs, do that.
+	if params_as_inputs:
+		tf_dataset_t = dataset_generation.generate_params_as_input_dataset(
+			tf_dataset_t,params_as_inputs,all_params+log_learning_params)
+		tf_dataset_v = dataset_generation.generate_params_as_input_dataset(
+			tf_dataset_v,params_as_inputs,all_params+log_learning_params)
 
 	print('Initializing the model')
 
 	# Load the loss function
 	if loss_function == 'mse':
 		num_outputs = num_params
 		loss = loss_functions.MSELoss(num_params,flip_pairs,weight_terms).loss
@@ -188,17 +194,20 @@
 		loss = loss_functions.FullCovarianceLoss(num_params,flip_pairs,
 			weight_terms).loss
 	else:
 		raise ValueError('%s loss not in the list of supported losses'%(
 			loss_function))
 
 	# Load the model
-	if model_type == 'xresnet34':
+	if model_type == 'xresnet34' and not params_as_inputs:
 		model = conv_models.build_xresnet34(img_size,num_outputs,
 			train_only_head=train_only_head)
+	elif model_type == 'xresnet34' and params_as_inputs:
+		model = conv_models.build_xresnet34_fc_inputs(img_size,num_outputs,
+			len(params_as_inputs),train_only_head=False)
 	else:
 		raise ValueError('%s model not in the list of supported models'%(
 			model_type))
 
 	# Use learning rate decay for optimal learning
 	lr_schedule = tf.keras.optimizers.schedules.ExponentialDecay(
 		learning_rate,decay_steps=steps_per_epoch,decay_rate=0.98,
```

### Comparing `paltas-0.1.1/paltas/Configs/2203_00690/config_test_1.py` & `paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_01.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from paltas.Configs.xxxx_yyyy.config_val import *
+from paltas.Configs.paper_2203_00690.config_val import *
+config_dict = copy.deepcopy(config_dict)
 
 config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=2.0e-4,
 	scale=1.5e-4).rvs
 config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-201.8,
 	np.inf,loc=2.018,scale=0.01).rvs
 config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-71.7,
 	np.inf,loc=1.076,scale=0.015).rvs
```

### Comparing `paltas-0.1.1/paltas/Configs/2203_00690/config_test_10.py` & `paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_10.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from paltas.Configs.xxxx_yyyy.config_val import *
+from paltas.Configs.paper_2203_00690.config_val import *
+config_dict = copy.deepcopy(config_dict)
 
 config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=2.0e-3,
 	scale=1.5e-4).rvs
 config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-198.8,
 	np.inf,loc=1.988,scale=0.01).rvs
 config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-75.2,
 	np.inf,loc=1.128,scale=0.015).rvs
```

### Comparing `paltas-0.1.1/paltas/Configs/2203_00690/config_test_11.py` & `paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_11.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from paltas.Configs.xxxx_yyyy.config_val import *
+from paltas.Configs.paper_2203_00690.config_val import *
+config_dict = copy.deepcopy(config_dict)
 
 config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=2.2e-3,
 	scale=1.5e-4).rvs
 config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-196.7,
 	np.inf,loc=1.967,scale=0.01).rvs
 config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-76.4,
 	np.inf,loc=1.146,scale=0.015).rvs
```

### Comparing `paltas-0.1.1/paltas/Configs/2203_00690/config_test_12.py` & `paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_12.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from paltas.Configs.xxxx_yyyy.config_val import *
+from paltas.Configs.paper_2203_00690.config_val import *
+config_dict = copy.deepcopy(config_dict)
 
 config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=2.4e-3,
 	scale=1.5e-4).rvs
 config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-197.2,
 	np.inf,loc=1.972,scale=0.01).rvs
 config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-70.9,
 	np.inf,loc=1.063,scale=0.015).rvs
```

### Comparing `paltas-0.1.1/paltas/Configs/2203_00690/config_test_13.py` & `paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_13.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from paltas.Configs.xxxx_yyyy.config_val import *
+from paltas.Configs.paper_2203_00690.config_val import *
+config_dict = copy.deepcopy(config_dict)
 
 config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=2.6e-3,
 	scale=1.5e-4).rvs
 config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-200.4,
 	np.inf,loc=2.004,scale=0.01).rvs
 config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-76.2,
 	np.inf,loc=1.143,scale=0.015).rvs
```

### Comparing `paltas-0.1.1/paltas/Configs/2203_00690/config_test_14.py` & `paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_14.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from paltas.Configs.xxxx_yyyy.config_val import *
+from paltas.Configs.paper_2203_00690.config_val import *
+config_dict = copy.deepcopy(config_dict)
 
 config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=2.8e-3,
 	scale=1.5e-4).rvs
 config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-202.7,
 	np.inf,loc=2.027,scale=0.01).rvs
 config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-70.8,
 	np.inf,loc=1.061,scale=0.015).rvs
```

### Comparing `paltas-0.1.1/paltas/Configs/2203_00690/config_test_15.py` & `paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_17.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from paltas.Configs.xxxx_yyyy.config_val import *
+from paltas.Configs.paper_2203_00690.config_val import *
+config_dict = copy.deepcopy(config_dict)
 
-config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=3.0e-3,
+config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=3.4e-3,
 	scale=1.5e-4).rvs
-config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-202.5,
-	np.inf,loc=2.025,scale=0.01).rvs
-config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-75.0,
-	np.inf,loc=1.125,scale=0.015).rvs
-config_dict['main_deflector']['parameters']['e1'] = norm(loc=-0.014,
+config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-202.0,
+	np.inf,loc=2.020,scale=0.01).rvs
+config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-72.8,
+	np.inf,loc=1.091,scale=0.015).rvs
+config_dict['main_deflector']['parameters']['e1'] = norm(loc=-0.001,
 	scale=0.01).rvs
-config_dict['main_deflector']['parameters']['e2'] = norm(loc=0.017,
+config_dict['main_deflector']['parameters']['e2'] = norm(loc=0.039,
 	scale=0.01).rvs
-config_dict['main_deflector']['parameters']['center_x'] = norm(loc=0.019,
+config_dict['main_deflector']['parameters']['center_x'] = norm(loc=-0.076,
 	scale=0.016).rvs
-config_dict['main_deflector']['parameters']['center_y'] = norm(loc=0.048,
+config_dict['main_deflector']['parameters']['center_y'] = norm(loc=-0.025,
 	scale=0.016).rvs
-config_dict['main_deflector']['parameters']['gamma1'] = norm(loc=0.006,
+config_dict['main_deflector']['parameters']['gamma1'] = norm(loc=0.012,
 	scale=0.005).rvs
-config_dict['main_deflector']['parameters']['gamma2'] = norm(loc=0.014,
+config_dict['main_deflector']['parameters']['gamma2'] = norm(loc=0.008,
 	scale=0.005).rvs
```

### Comparing `paltas-0.1.1/paltas/Configs/2203_00690/config_test_16.py` & `paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_05.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from paltas.Configs.xxxx_yyyy.config_val import *
+from paltas.Configs.paper_2203_00690.config_val import *
+config_dict = copy.deepcopy(config_dict)
 
-config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=3.2e-3,
+config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=1.0e-3,
 	scale=1.5e-4).rvs
-config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-203.1,
-	np.inf,loc=2.031,scale=0.01).rvs
-config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-71.2,
-	np.inf,loc=1.068,scale=0.015).rvs
-config_dict['main_deflector']['parameters']['e1'] = norm(loc=0.027,
+config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-202.7,
+	np.inf,loc=2.027,scale=0.01).rvs
+config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-69.2,
+	np.inf,loc=1.038,scale=0.015).rvs
+config_dict['main_deflector']['parameters']['e1'] = norm(loc=0.033,
 	scale=0.01).rvs
-config_dict['main_deflector']['parameters']['e2'] = norm(loc=-0.040,
+config_dict['main_deflector']['parameters']['e2'] = norm(loc=0.017,
 	scale=0.01).rvs
-config_dict['main_deflector']['parameters']['center_x'] = norm(loc=0.065,
+config_dict['main_deflector']['parameters']['center_x'] = norm(loc=-0.062,
 	scale=0.016).rvs
-config_dict['main_deflector']['parameters']['center_y'] = norm(loc=0.068,
+config_dict['main_deflector']['parameters']['center_y'] = norm(loc=-0.051,
 	scale=0.016).rvs
-config_dict['main_deflector']['parameters']['gamma1'] = norm(loc=-0.011,
+config_dict['main_deflector']['parameters']['gamma1'] = norm(loc=0.000,
 	scale=0.005).rvs
-config_dict['main_deflector']['parameters']['gamma2'] = norm(loc=0.021,
+config_dict['main_deflector']['parameters']['gamma2'] = norm(loc=-0.000,
 	scale=0.005).rvs
```

### Comparing `paltas-0.1.1/paltas/Configs/2203_00690/config_test_17.py` & `paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_03.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from paltas.Configs.xxxx_yyyy.config_val import *
+from paltas.Configs.paper_2203_00690.config_val import *
+config_dict = copy.deepcopy(config_dict)
 
-config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=3.4e-3,
+config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=6.0e-4,
 	scale=1.5e-4).rvs
-config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-202.0,
-	np.inf,loc=2.020,scale=0.01).rvs
-config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-72.8,
-	np.inf,loc=1.091,scale=0.015).rvs
-config_dict['main_deflector']['parameters']['e1'] = norm(loc=-0.001,
+config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-201.5,
+	np.inf,loc=2.015,scale=0.01).rvs
+config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-71.7,
+	np.inf,loc=1.076,scale=0.015).rvs
+config_dict['main_deflector']['parameters']['e1'] = norm(loc=-0.032,
 	scale=0.01).rvs
-config_dict['main_deflector']['parameters']['e2'] = norm(loc=0.039,
+config_dict['main_deflector']['parameters']['e2'] = norm(loc=-0.025,
 	scale=0.01).rvs
-config_dict['main_deflector']['parameters']['center_x'] = norm(loc=-0.076,
+config_dict['main_deflector']['parameters']['center_x'] = norm(loc=0.070,
 	scale=0.016).rvs
-config_dict['main_deflector']['parameters']['center_y'] = norm(loc=-0.025,
+config_dict['main_deflector']['parameters']['center_y'] = norm(loc=0.048,
 	scale=0.016).rvs
-config_dict['main_deflector']['parameters']['gamma1'] = norm(loc=0.012,
+config_dict['main_deflector']['parameters']['gamma1'] = norm(loc=-0.012,
 	scale=0.005).rvs
-config_dict['main_deflector']['parameters']['gamma2'] = norm(loc=0.008,
+config_dict['main_deflector']['parameters']['gamma2'] = norm(loc=-0.007,
 	scale=0.005).rvs
```

### Comparing `paltas-0.1.1/paltas/Configs/2203_00690/config_test_18.py` & `paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_18.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from paltas.Configs.xxxx_yyyy.config_val import *
+from paltas.Configs.paper_2203_00690.config_val import *
+config_dict = copy.deepcopy(config_dict)
 
 config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=3.6e-3,
 	scale=1.5e-4).rvs
 config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-196.1,
 	np.inf,loc=1.961,scale=0.01).rvs
 config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-73.4,
 	np.inf,loc=1.101,scale=0.015).rvs
```

### Comparing `paltas-0.1.1/paltas/Configs/2203_00690/config_test_19.py` & `paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_19.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from paltas.Configs.xxxx_yyyy.config_val import *
+from paltas.Configs.paper_2203_00690.config_val import *
+config_dict = copy.deepcopy(config_dict)
 
 config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=3.8e-3,
 	scale=1.5e-4).rvs
 config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-195.8,
 	np.inf,loc=1.958,scale=0.01).rvs
 config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-73.8,
 	np.inf,loc=1.108,scale=0.015).rvs
```

### Comparing `paltas-0.1.1/paltas/Configs/2203_00690/config_test_2.py` & `paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_02.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from paltas.Configs.xxxx_yyyy.config_val import *
+from paltas.Configs.paper_2203_00690.config_val import *
+config_dict = copy.deepcopy(config_dict)
 
 config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=4.0e-4,
 	scale=1.5e-4).rvs
 config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-200.1,
 	np.inf,loc=2.001,scale=0.01).rvs
 config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-76.8,
 	np.inf,loc=1.153,scale=0.015).rvs
```

### Comparing `paltas-0.1.1/paltas/Configs/2203_00690/config_test_20.py` & `paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_20.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from paltas.Configs.xxxx_yyyy.config_val import *
+from paltas.Configs.paper_2203_00690.config_val import *
+config_dict = copy.deepcopy(config_dict)
 
 config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=4.0e-3,
 	scale=1.5e-4).rvs
 config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-197.6,
 	np.inf,loc=1.976,scale=0.01).rvs
 config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-73.1,
 	np.inf,loc=1.097,scale=0.015).rvs
```

### Comparing `paltas-0.1.1/paltas/Configs/2203_00690/config_test_3.py` & `paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_09.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from paltas.Configs.xxxx_yyyy.config_val import *
+from paltas.Configs.paper_2203_00690.config_val import *
+config_dict = copy.deepcopy(config_dict)
 
-config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=6.0e-4,
+config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=1.8e-3,
 	scale=1.5e-4).rvs
-config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-201.5,
-	np.inf,loc=2.015,scale=0.01).rvs
-config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-71.7,
-	np.inf,loc=1.076,scale=0.015).rvs
-config_dict['main_deflector']['parameters']['e1'] = norm(loc=-0.032,
+config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-199.5,np.inf,
+	loc=1.995,scale=0.01).rvs
+config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-74.9,np.inf,
+	loc=1.123,scale=0.015).rvs
+config_dict['main_deflector']['parameters']['e1'] = norm(loc=0.031,
 	scale=0.01).rvs
-config_dict['main_deflector']['parameters']['e2'] = norm(loc=-0.025,
+config_dict['main_deflector']['parameters']['e2'] = norm(loc=-0.003,
 	scale=0.01).rvs
-config_dict['main_deflector']['parameters']['center_x'] = norm(loc=0.070,
+config_dict['main_deflector']['parameters']['center_x'] = norm(loc=0.071,
 	scale=0.016).rvs
-config_dict['main_deflector']['parameters']['center_y'] = norm(loc=0.048,
+config_dict['main_deflector']['parameters']['center_y'] = norm(loc=-0.006,
 	scale=0.016).rvs
-config_dict['main_deflector']['parameters']['gamma1'] = norm(loc=-0.012,
+config_dict['main_deflector']['parameters']['gamma1'] = norm(loc=-0.001,
 	scale=0.005).rvs
-config_dict['main_deflector']['parameters']['gamma2'] = norm(loc=-0.007,
+config_dict['main_deflector']['parameters']['gamma2'] = norm(loc=0.010,
 	scale=0.005).rvs
```

### Comparing `paltas-0.1.1/paltas/Configs/2203_00690/config_test_4.py` & `paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_04.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from paltas.Configs.xxxx_yyyy.config_val import *
+from paltas.Configs.paper_2203_00690.config_val import *
+config_dict = copy.deepcopy(config_dict)
 
 config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=8.0e-4,
 	scale=1.5e-4).rvs
 config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-197.4,
 	np.inf,loc=1.974,scale=0.01).rvs
 config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-69.1,
 	np.inf,loc=1.037,scale=0.015).rvs
```

### Comparing `paltas-0.1.1/paltas/Configs/2203_00690/config_test_5.py` & `paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_07.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from paltas.Configs.xxxx_yyyy.config_val import *
+from paltas.Configs.paper_2203_00690.config_val import *
+config_dict = copy.deepcopy(config_dict)
 
-config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=1.0e-3,
+config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=1.4e-3,
 	scale=1.5e-4).rvs
-config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-202.7,
-	np.inf,loc=2.027,scale=0.01).rvs
-config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-69.2,
-	np.inf,loc=1.038,scale=0.015).rvs
-config_dict['main_deflector']['parameters']['e1'] = norm(loc=0.033,
+config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-203.8,
+	np.inf,loc=2.038,scale=0.01).rvs
+config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-70.6,
+	np.inf,loc=1.059,scale=0.015).rvs
+config_dict['main_deflector']['parameters']['e1'] = norm(loc=0.044,
 	scale=0.01).rvs
-config_dict['main_deflector']['parameters']['e2'] = norm(loc=0.017,
+config_dict['main_deflector']['parameters']['e2'] = norm(loc=-0.028,
 	scale=0.01).rvs
-config_dict['main_deflector']['parameters']['center_x'] = norm(loc=-0.062,
+config_dict['main_deflector']['parameters']['center_x'] = norm(loc=0.009,
 	scale=0.016).rvs
-config_dict['main_deflector']['parameters']['center_y'] = norm(loc=-0.051,
+config_dict['main_deflector']['parameters']['center_y'] = norm(loc=-0.013,
 	scale=0.016).rvs
-config_dict['main_deflector']['parameters']['gamma1'] = norm(loc=0.000,
+config_dict['main_deflector']['parameters']['gamma1'] = norm(loc=-0.022,
 	scale=0.005).rvs
-config_dict['main_deflector']['parameters']['gamma2'] = norm(loc=-0.000,
+config_dict['main_deflector']['parameters']['gamma2'] = norm(loc=0.023,
 	scale=0.005).rvs
```

### Comparing `paltas-0.1.1/paltas/Configs/2203_00690/config_test_6.py` & `paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_06.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from paltas.Configs.xxxx_yyyy.config_val import *
+from paltas.Configs.paper_2203_00690.config_val import *
+config_dict = copy.deepcopy(config_dict)
 
 config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=1.2e-3,
 	scale=1.5e-4).rvs
 config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-196.2,
 	np.inf,loc=1.962,scale=0.01).rvs
 config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-71.0,
 	np.inf,loc=1.065,scale=0.015).rvs
```

### Comparing `paltas-0.1.1/paltas/Configs/2203_00690/config_test_7.py` & `paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_16.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from paltas.Configs.xxxx_yyyy.config_val import *
+from paltas.Configs.paper_2203_00690.config_val import *
+config_dict = copy.deepcopy(config_dict)
 
-config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=1.4e-3,
+config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=3.2e-3,
 	scale=1.5e-4).rvs
-config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-203.8,
-	np.inf,loc=2.038,scale=0.01).rvs
-config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-70.6,
-	np.inf,loc=1.059,scale=0.015).rvs
-config_dict['main_deflector']['parameters']['e1'] = norm(loc=0.044,
+config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-203.1,
+	np.inf,loc=2.031,scale=0.01).rvs
+config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-71.2,
+	np.inf,loc=1.068,scale=0.015).rvs
+config_dict['main_deflector']['parameters']['e1'] = norm(loc=0.027,
 	scale=0.01).rvs
-config_dict['main_deflector']['parameters']['e2'] = norm(loc=-0.028,
+config_dict['main_deflector']['parameters']['e2'] = norm(loc=-0.040,
 	scale=0.01).rvs
-config_dict['main_deflector']['parameters']['center_x'] = norm(loc=0.009,
+config_dict['main_deflector']['parameters']['center_x'] = norm(loc=0.065,
 	scale=0.016).rvs
-config_dict['main_deflector']['parameters']['center_y'] = norm(loc=-0.013,
+config_dict['main_deflector']['parameters']['center_y'] = norm(loc=0.068,
 	scale=0.016).rvs
-config_dict['main_deflector']['parameters']['gamma1'] = norm(loc=-0.022,
+config_dict['main_deflector']['parameters']['gamma1'] = norm(loc=-0.011,
 	scale=0.005).rvs
-config_dict['main_deflector']['parameters']['gamma2'] = norm(loc=0.023,
+config_dict['main_deflector']['parameters']['gamma2'] = norm(loc=0.021,
 	scale=0.005).rvs
```

### Comparing `paltas-0.1.1/paltas/Configs/2203_00690/config_test_8.py` & `paltas-0.2.0/paltas/Configs/paper_2203_00690/config_test_08.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from paltas.Configs.xxxx_yyyy.config_val import *
+from paltas.Configs.paper_2203_00690.config_val import *
+config_dict = copy.deepcopy(config_dict)
 
 config_dict['subhalo']['parameters']['sigma_sub'] = norm(loc=1.6e-3,
 	scale=1.5e-4).rvs
 config_dict['main_deflector']['parameters']['gamma'] = truncnorm(-195.3,
 	np.inf,loc=1.953,scale=0.01).rvs
 config_dict['main_deflector']['parameters']['theta_E'] = truncnorm(-76.7,
 	np.inf,loc=1.150,scale=0.015).rvs
```

### Comparing `paltas-0.1.1/paltas/Configs/2203_00690/config_train.py` & `paltas-0.2.0/paltas/Configs/paper_2203_00690/config_train.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,33 +46,27 @@
 config_dict = {
 	'subhalo':{
 		'class': SubhalosDG19,
 		'parameters':{
 			'sigma_sub':norm(loc=2e-3,scale=1.1e-3).rvs,
 			'shmf_plaw_index':uniform(loc=-1.92,scale=0.1).rvs,
 			'm_pivot': 1e10,'m_min': 1e7,'m_max': 1e10,
-			'c_0':uniform(loc=16,scale=2).rvs,
-			'conc_zeta':uniform(loc=-0.3,scale=0.1).rvs,
-			'conc_beta':uniform(loc=0.55,scale=0.3).rvs,
+			# See cross_dict for mass-concentration parameters (c_0 etc)
 			'conc_m_ref': 1e8,
-			'dex_scatter': uniform(loc=0.1,scale=0.06).rvs,
 			'k1':0.0, 'k2':0.0
 		}
 	},
 	'los':{
 		'class': LOSDG19,
 		'parameters':{
 			'delta_los':norm(loc=1,scale=0.6).rvs,
 			'm_min':1e7,'m_max':1e10,'z_min':0.01,
 			'dz':0.01,'cone_angle':8.0,'r_min':0.5,'r_max':10.0,
-			'c_0':uniform(loc=16,scale=2).rvs,
-			'conc_zeta':uniform(loc=-0.3,scale=0.1).rvs,
-			'conc_beta':uniform(loc=0.55,scale=0.3).rvs,
+			# See cross_dict for mass-concentration parameters (c_0 etc)
 			'conc_m_ref': 1e8,
-			'dex_scatter': uniform(loc=0.1,scale=0.06).rvs,
 			'alpha_dz_factor':5.0
 		}
 	},
 	'main_deflector':{
 		'class': PEMDShear,
 		'parameters':{
 			'M200': 1e13,
```

### Comparing `paltas-0.1.1/paltas/Configs/config_handler.py` & `paltas-0.2.0/paltas/Configs/config_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """
 Interact with the paltas configuration files
 
 Classes used to draw relevant parameters from paltas configuration files.
 """
 import os, sys, warnings, copy
 from importlib import import_module
+import numba
 import numpy as np
 from ..Sampling.sampler import Sampler
 from ..Sources.galaxy_catalog import GalaxyCatalog
 from ..Utils.cosmology_utils import get_cosmology, ddt
 from ..Utils.hubble_utils import hubblify
 from ..Utils.lenstronomy_utils import PSFHelper
 from lenstronomy.Data.psf import PSF
@@ -20,37 +21,65 @@
 from lenstronomy.PointSource.point_source import PointSource
 from lenstronomy.ImSim.image_model import ImageModel
 import lenstronomy.Util.util as util
 
 # Global filters on the python warnings. Using this since filter
 # behaviour is a bit weird.
 SERIALIZATIONWARNING = True
-KWARGSNUMERICWARNING1 = True
-KWARGSNUMERICWARNING2 = True
+KWARGSNUMERICWARNING1 = False
+KWARGSNUMERICWARNING2 = False
+
+# Exclude these parameters from the image metadata. These are rarely sampled
+# and would bloat the metadata or make it hard to serialize.
+EXCLUDE_FROM_METADATA = (
+	# Long list of sources that were included
+	('source_parameters', 'source_inclusion_list'),
+	# Tiny list denoting drizzle pattern
+	# (allowing this would complicate check against lists entering metadata)
+	('drizzle_parameters', 'offset_pattern'),
+	# Path to the COSMOS images. Pointless repeating setup-specific string.
+	('source_parameters', 'cosmos_folder'),
+)
+
+
+class MagnificationError(Exception):
+	def __init__(self,mag_cut):
+		# Pass a useful message to base class constructor
+		message = 'Magnification cut of %.2f not met. '%(mag_cut)
+		message += 'If this is inteneded (i.e. in a loop) use try/except.'
+		super().__init__(message)
 
 
 class ConfigHandler():
 	"""Class that parses the configuration files to extract images and lenstronomy
 	configurations.
 
 	Args:
 		config_path (str): A path to the config file to parse.
 	"""
 
-	def __init__(self,config_path):
+	def __init__(self,config_path,):
 		# Get the dictionary from the provided .py file
 		config_dir, config_file = os.path.split(os.path.abspath(config_path))
 		sys.path.insert(0, config_dir)
 		config_name, _ = os.path.splitext(config_file)
 		self.config_module = import_module(config_name)
 		self.config_dict = self.config_module.config_dict
 
-		# Initialize the random seed provided with the config module
-		if hasattr(self.config_module,'seed'):
-			np.random.seed(self.config_module.seed)
+		# Get the random seed to use, or draw a random not-too-large one
+		# (so it is easy to copy-paste from metadata into config files)
+		# Max is 2**32 - 1, see _legacy_seeding in numpy/random/_mt19937.pyx
+		self.base_seed = getattr(
+			self.config_module,
+			'seed',
+			(np.random.randint(np.iinfo(np.uint32).max, dtype=np.int64)))
+		# Make sure base_seed is a sequence, not a number
+		if isinstance(self.base_seed, (int, float)):
+			self.base_seed = (self.base_seed,)
+		self.reseed_counter = 0
 
 		# Set up our sampler and draw a sample for initialization
 		self.sampler = Sampler(self.config_dict)
 		self.sample = None
 		self.draw_new_sample()
 		sample = self.get_current_sample()
 
@@ -90,15 +119,15 @@
 			self.point_source_class = self.config_dict['point_source']['class'](
 				sample['point_source_parameters'])
 
 		# We always need a source class
 		self.source_class = self.config_dict['source']['class'](
 			sample['cosmology_parameters'],sample['source_parameters'])
 
-		# See if a magnitude cut was specified
+		# See if a magnification cut was specified
 		if hasattr(self.config_module, 'mag_cut'):
 			self.mag_cut = self.config_module.mag_cut
 		else:
 			self.mag_cut = None
 
 		# See if ignoring noise was specified
 		if hasattr(self.config_module,'no_noise'):
@@ -277,23 +306,26 @@
 
 		for component in sample:
 			for key in sample[component]:
 				comp_value = sample[component][key]
 				# Make sure that lists and other objects that cannot be
 				# serialized well are not written out. Warn about this only
 				# once.
+				if (component, key) in EXCLUDE_FROM_METADATA:
+					continue
 				if isinstance(comp_value,bool):
 					metadata[component+'_'+key] = int(comp_value)
-				elif (isinstance(comp_value,str) or isinstance(comp_value,int) or
-					isinstance(comp_value,float)):
+				elif isinstance(comp_value, (str, int, float)) or comp_value is None:
 					metadata[component+'_'+key] = comp_value
 				elif SERIALIZATIONWARNING:
-					warnings.warn('One or more parameters in config_dict '
-						'cannot be serialized and will not be written to '
-						'metadata.csv',category=RuntimeWarning)
+					warnings.warn(
+						f'Parameter ({component}, {key}) in config_dict, '
+						'and possibly others, will not be written to '
+						'metadata.csv',
+						category=RuntimeWarning)
 					SERIALIZATIONWARNING = False
 
 		return metadata
 
 	def get_sample_cosmology(self,as_astropy=False):
 		"""Return the cosmology object for the current sample.
 
@@ -403,15 +435,15 @@
 			apply_psf (bool): If False, the psf will not be applied. Defaults
 				to True.
 		Returns:
 			(np.array,dict): A tuple containing a numpy array of the generated
 			image and a metavalue dictionary with the corresponding sampled
 			values.
 		Notes:
-			Will return None,None if the produced image does not meet a cut.
+			Will raise an error if the produced image does not meet a cut.
 		"""
 		# Get the lenstronomy parameters and the sample
 		sample = self.get_current_sample()
 		kwargs_model, kwargs_params = self.get_lenstronomy_models_kwargs(
 			new_sample=False)
 
 		# Get the psf and detector parameters from the sample
@@ -442,15 +474,15 @@
 		lens_light_model = LightModel(kwargs_model['lens_light_model_list'])
 
 		# Point source may need lens eqn solver kwargs
 		lens_equation_params = None
 		if 'lens_equation_solver_parameters' in sample.keys():
 			lens_equation_params = sample['lens_equation_solver_parameters']
 		point_source_model = PointSource(
-			kwargs_model['point_source_model_list'],lensModel=lens_model,
+			kwargs_model['point_source_model_list'],lens_model=lens_model,
 			save_cache=True,kwargs_lens_eqn_solver=lens_equation_params)
 
 		# Put it together into an image model
 		image_model = ImageModel(data_api.data_class,psf_model,
 			lens_model,source_light_model,lens_light_model,
 			point_source_model,kwargs_numerics=self.kwargs_numerics)
 
@@ -458,18 +490,25 @@
 		image = image_model.image(kwargs_params['kwargs_lens'],
 			kwargs_params['kwargs_source'],
 			kwargs_params['kwargs_lens_light'],
 			kwargs_params['kwargs_ps'])
 
 		# Check for the magnification cut and apply it.
 		if self.mag_cut is not None:
-			mag = np.sum(image)/np.sum(source_light_model.total_flux(
+			# Evaluate the light that would have been in the image using
+			# the image model
+			lens_light_total = np.sum(image_model.lens_surface_brightness(
+				kwargs_params['kwargs_lens_light']))
+			source_light_total = np.sum(source_light_model.total_flux(
 				kwargs_params['kwargs_source']))
+
+			mag = np.sum(image)-lens_light_total
+			mag /= source_light_total
 			if mag < self.mag_cut:
-				return None,None
+				raise MagnificationError(self.mag_cut)
 
 		# If noise is specified, add it.
 		if add_noise:
 			image += single_band.noise_for_model(image)
 
 		# Extract the metadata from the sample
 		metadata = self.get_metadata()
@@ -482,23 +521,20 @@
 
 		return image, metadata
 
 	def _draw_image_drizzle(self):
 		"""Uses the current config sample to generate a drizzled image and the
 		associated metadata.
 
-		Args:
-			apply_psf (bool): If False, the psf will not be applied. Defaults
-				to true.
 		Returns:
 			(np.array,dict): A tuple containing a numpy array of the generated
 			image and a metavalue dictionary with the corresponding sampled
 			values.
 		Notes:
-			Will return None,None if the produced image does not meet a cut.
+			Will return an error if the produced image does not meet a cut.
 			This function will fail if the drizzle parameters are not
 			present.
 		"""
 		# Grab our warning flags
 		global KWARGSNUMERICWARNING1
 		global KWARGSNUMERICWARNING2
 
@@ -537,23 +573,27 @@
 				KWARGSNUMERICWARNING2 = False
 			self.kwargs_numerics['point_source_supersampling_factor'] = max(1,
 				int(self.kwargs_numerics['point_source_supersampling_factor']/
 					ss_scaling))
 
 		# Use the normal generation class to make our highres image without
 		# noise.
-		image_ss, metadata = self._draw_image_standard(add_noise=False,
-			apply_psf=False)
+		try:
+			image_ss, metadata = self._draw_image_standard(add_noise=False,
+				apply_psf=False)
+		except MagnificationError:
+			# Reset the class properties that were modified, then reraise
+			self.sample = sample_copy
+			self.kwargs_numerics = kwargs_numerics_copy
+			self.numpix = numpix_copy
+			raise
+
 		self.sample['detector_parameters']['pixel_scale'] = detector_pixel_scale
 		self.numpix = numpix_copy
 
-		# Deal with an image that does not pass a cut.
-		if image_ss is None:
-			return image_ss, metadata
-
 		# Grab the PSF supersampling factor if present.
 		if 'psf_supersample_factor' in self.sample['drizzle_parameters']:
 			psf_supersample_factor = (
 				self.sample['drizzle_parameters']['psf_supersample_factor'])
 		else:
 			warnings.warn('No psf_supersample_factor provided so 1 will be ' +
 				'assumed.')
@@ -633,28 +673,72 @@
 		Notes:
 			Even if new_sample is False, this function is not guaranteed to be
 			deterministic. For example, most of the substructure classes draw
 			from populations specified by the input parameters, and therefore
 			calling the function repeatedly will return images of different
 			realizations of that population.
 		"""
+		# Generate a new random seed for each call to draw_image in order
+		# to ensure deterministic behavior
+		seed = self.reseed()
+
 		# Draw a new sample if requested
 		if new_sample:
 			self.draw_new_sample()
 
 		# Use the appropraite generation function
-		if self.do_drizzle:
-			image,metadata = self._draw_image_drizzle()
-		else:
-			# _draw_image_standard has a seperate add_noise parameter so
-			# it can be used by _draw_image_drizzle.
-			image,metadata = self._draw_image_standard(add_noise=self.add_noise)
+		try:
+			if self.do_drizzle:
+				image,metadata = self._draw_image_drizzle()
+			else:
+				# _draw_image_standard has a seperate add_noise parameter so
+				# it can be used by _draw_image_drizzle.
+				image,metadata = self._draw_image_standard(
+					add_noise=self.add_noise)
+		except MagnificationError:
+			# Magnification cut was not met, return None,None
+			return None, None
 
 		# Mask out an interior region of the image if requested
-		if hasattr(self.config_module,'mask_radius') and image is not None:
+		if hasattr(self.config_module,'mask_radius'):
 			kwargs_detector = self.get_current_sample()['detector_parameters']
 			x_grid, y_grid = util.make_grid(numPix=image.shape[0],
 				deltapix=kwargs_detector['pixel_scale'])
 			r = util.array2image(np.sqrt(x_grid**2+y_grid**2))
 			image[r<=self.config_module.mask_radius] = 0
 
+		# Save the seed
+		metadata['seed'] = seed
+
 		return image,metadata
+
+	def reseed(self):
+		"""Generates, sets, and returns a new random seed.
+
+		Returns:
+			(tuple): The tuple used to seed numpy.
+		"""
+		if self.reseed_counter == 0:
+			# Use the base seed; perhaps to reproduce one particular image
+			seed = self.base_seed
+		else:
+			# Append the counter to the base_seed tuple to form a new seed
+			seed = self.base_seed + (self.reseed_counter,)
+		# Seed numpy's random generator. Note this accepts tuples.
+		np.random.seed(seed)
+		self.reseed_counter += 1
+		# Seed numba's separate random generator
+		# Unfortunately it only accepts an integer argument
+		_set_numba_seed(np.random.randint(np.iinfo(np.uint32).max))
+		return seed
+
+
+# Must be compiled in regular (non-object) mode, see note under
+# https://numba.pydata.org/numba-doc/0.22.1/reference/numpysupported.html#random
+@numba.njit
+def _set_numba_seed(seed):
+	"""Reseeds numba's random number generator
+
+	Args:
+		seed (int): The integer random seed to use for seeding numba.
+	"""
+	np.random.seed(seed)
```

### Comparing `paltas-0.1.1/paltas/MainDeflector/main_deflector_base.py` & `paltas-0.2.0/paltas/MainDeflector/main_deflector_base.py`

 * *Files identical despite different names*

### Comparing `paltas-0.1.1/paltas/MainDeflector/simple_deflectors.py` & `paltas-0.2.0/paltas/MainDeflector/simple_deflectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Provide the implementation of a few main deflector profiles that consist
 of two or fewer components.
 
 This module contains the classes to render main deflectors consisting of simple
 combinations of lenstronomy profiles.
 """
 from .main_deflector_base import MainDeflectorBase
-from lenstronomy.LensModel.profile_list_base import ProfileListBase
+from lenstronomy.LensModel.profile_list_base import lens_class
 
 
 class PEMD(MainDeflectorBase):
 	"""Class for rendering a main deflector the includes a PEMD profile.
 
 	Args:
 		main_deflector_parameters (dict): A dictionary containing the type of
@@ -59,15 +59,17 @@
 		md_kwargs_list = []
 		md_z_list = [self.main_deflector_parameters['z_lens']] * len(
 			md_model_list)
 
 		# Use lenstronomy to sort the parameters
 		for model in md_model_list:
 			# The list of parameters linked to that lenstronomy model
-			p_names = ProfileListBase._import_class(model,None,None).param_names
+			p_names = (
+				lens_class(model).param_names
+			)
 			model_kwargs = {}
 			for param in p_names:
 				model_kwargs[param] = (self.main_deflector_parameters[param])
 			md_kwargs_list += [model_kwargs]
 
 		return md_model_list, md_kwargs_list, md_z_list
 
@@ -126,66 +128,65 @@
 		md_kwargs_list = []
 		md_z_list = [self.main_deflector_parameters['z_lens']] * len(
 			md_model_list)
 
 		# Use lenstronomy to sort the parameters
 		for model in md_model_list:
 			# The list of parameters linked to that lenstronomy model
-			p_names = ProfileListBase._import_class(model,None,None).param_names
+			p_names = (
+				lens_class(model).param_names
+			)
 			model_kwargs = {}
 			for param in p_names:
 				model_kwargs[param] = (self.main_deflector_parameters[param])
 			md_kwargs_list += [model_kwargs]
 
 		return md_model_list, md_kwargs_list, md_z_list
 
 
 class PEMDShearFourMultipole(PEMDShear):
 	"""Class for rendering a main deflector the includes a PEMD profile,
 	external shear, and order 2, 3, and 4 multipole.
+
 	Args:
 		main_deflector_parameters (dict): A dictionary containing the type of
 			main deflector and the value for each of its parameters.
 		cosmology_parameters (str,dict, or colossus.cosmology.Cosmology):
 			Either a name of colossus cosmology, a dict with 'cosmology name':
 			name of colossus cosmology, an instance of colussus cosmology, or a
 			dict with H0 and Om0 ( other parameters will be set to defaults).
 	Notes:
 		Uses the lenstronomy EPL class, which is equivalent to PEMD but is pure
 		python.
+
 	Required Parameters
+
 	- gamma - power law slope
 	- theta_E - Einstein radius of the profile in units of arcseconds
 	- e1 - x-direction ellipticity eccentricity
 	- e2 - xy-direction ellipticity eccentricity
 	- center_x - x-coordinate lens center in units of arcseconds
 	- center_y - y-coordinate lens center in units of arcseconds
 	- gamma1 - x-direction shear
 	- gamma2 - xy-direction shear
 	- ra_0 - ra origin of shear in units of arcseconds
 	- dec_0 - dec origin of shear in units of arcseconds
 	- z_lens - main deflector redshift
 	- mult2_a - multipole strength for order 2 multpole
 	- mult2_phi - multipole order 2 orientation in radians
-	- mult2_center_x - x-coordinate multipole order 2 center in units of
-	arcseconds
-	- mult2_center_y - y-coordinate multipole order 2 center in units of
-	arcseconds
+	- mult2_center_x - x-coordinate multipole order 2 center in units of arcseconds
+	- mult2_center_y - y-coordinate multipole order 2 center in units of arcseconds
 	- mult3_a - multipole strength for order 2 multpole
 	- mult3_phi - multipole order 2 orientation in radians
-	- mult3_center_x - x-coordinate multipole order 2 center in units of
-	arcseconds
-	- mult3_center_y - y-coordinate multipole order 2 center in units of
-	arcseconds
+	- mult3_center_x - x-coordinate multipole order 2 center in units of arcseconds
+	- mult3_center_y - y-coordinate multipole order 2 center in units of arcseconds
 	- mult4_a - multipole strength for order 2 multpole
 	- mult4_phi - multipole order 2 orientation in radians
-	- mult4_center_x - x-coordinate multipole order 2 center in units of
-	arcseconds
-	- mult4_center_y - y-coordinate multipole order 2 center in units of
-	arcseconds
+	- mult4_center_x - x-coordinate multipole order 2 center in units of arcseconds
+	- mult4_center_y - y-coordinate multipole order 2 center in units of arcseconds
 	"""
 	# Define the parameters we expect to find for the DG_19 model
 	required_parameters = PEMDShear.required_parameters + ('mult2_a',
 		'mult2_phi','mult2_center_x','mult2_center_y','mult3_a','mult3_phi',
 		'mult3_center_x','mult3_center_y','mult4_a','mult4_phi',
 		'mult4_center_x','mult4_center_y')
 
@@ -193,14 +194,15 @@
 
 		# Initialize the super class
 		super().__init__(main_deflector_parameters,cosmology_parameters)
 
 	def draw_main_deflector(self):
 		"""Draws the lenstronomy profile names and kwargs for the components
 		of the main deflector.
+
 		Returns:
 			(tuple): A tuple of three lists: the first is the profile type for
 			each component of the main deflector, the second is the
 			lenstronomy kwargs for each component, and the third is the
 			redshift for each component.
 		"""
 		# Get the first set of lists directly from the inherited class
```

### Comparing `paltas-0.1.1/paltas/PointSource/point_source_base.py` & `paltas-0.2.0/paltas/PointSource/point_source_base.py`

 * *Files identical despite different names*

### Comparing `paltas-0.1.1/paltas/PointSource/single_point_source.py` & `paltas-0.2.0/paltas/PointSource/single_point_source.py`

 * *Files identical despite different names*

### Comparing `paltas-0.1.1/paltas/Sampling/distributions.py` & `paltas-0.2.0/paltas/Sampling/distributions.py`

 * *Files 11% similar despite different names*

```diff
@@ -97,143 +97,143 @@
 		n_samp = n
 		keep_draws = np.zeros((n,self.mean.shape[1]))
 		rand_draw = np.random.randn(self.mean.shape[1]*n_samp).reshape(
 			(self.mean.shape[1],n_samp))
 		draws = (self.mean.T+np.dot(self.L,rand_draw)).T
 
 		# Check which draws are within our bounds
-		keep_ind = np.prod(draws > self.min_values,axis=-1,dtype=np.bool)
-		keep_ind *= np.prod(draws < self.max_values,axis=-1,dtype=np.bool)
+		keep_ind = np.prod(draws > self.min_values,axis=-1,dtype=bool)
+		keep_ind *= np.prod(draws < self.max_values,axis=-1,dtype=bool)
 		keep_draws[n_accepted:n_accepted+np.sum(keep_ind)] = draws[keep_ind]
 		n_accepted += np.sum(keep_ind)
 
 		# Keep drawing until we have enough samples.
 		while n_accepted<n:
 			# Draw
 			rand_draw = np.random.randn(self.mean.shape[1]*n_samp).reshape(
 				(self.mean.shape[1],n_samp))
 			draws = (self.mean.T+np.dot(self.L,rand_draw)).T
 			# Check for the values in bounds
-			keep_ind = np.prod(draws > self.min_values,axis=-1,dtype=np.bool)
-			keep_ind *= np.prod(draws < self.max_values,axis=-1,dtype=np.bool)
+			keep_ind = np.prod(draws > self.min_values,axis=-1,dtype=bool)
+			keep_ind *= np.prod(draws < self.max_values,axis=-1,dtype=bool)
 			# Only use the ones we need
 			use_keep = np.minimum(n-n_accepted,np.sum(keep_ind))
 			keep_draws[n_accepted:n_accepted+use_keep] = (
 				draws[keep_ind][:use_keep])
 			n_accepted += use_keep
 
 		# Remove first dimension for the n=1 case
 		if n==1:
 			keep_draws = np.squeeze(keep_draws)
 
 		return keep_draws
 
 
 class EllipticitiesTranslation():
-	"""Class that takes in distributions for q_lens and phi_lens, returns 
+	"""Class that takes in distributions for q_lens and phi_lens, returns
 	samples of e1 and e2 correspondingly
-	
-	Args: 
-		q_dist (scipy.stats.rv_continuous.rvs or float): distribution for 
+
+	Args:
+		q_dist (scipy.stats.rv_continuous.rvs or float): distribution for
 			axis ratio (can be callable or constant)
-		phi_dist (scipy.stats.rv_continuous.rvs or float): distribution for 
+		phi_dist (scipy.stats.rv_continuous.rvs or float): distribution for
 			orientation angle in radians (can be callable or constant)
 
-	Notes: 
+	Notes:
 
 	"""
 	def __init__(self,q_dist,phi_dist):
 		self.q_dist = q_dist
 		self.phi_dist = phi_dist
 
 	def __call__(self):
-		"""Returns a sample of e1,e2 
+		"""Returns a sample of e1,e2
 
 		Returns:
-			(float,float): samples of x-direction ellipticity 
+			(float,float): samples of x-direction ellipticity
 				eccentricity, xy-direction ellipticity eccentricity
 		"""
 
 		if callable(self.q_dist):
 			q = self.q_dist()
 		else:
 			q = self.q_dist
 		if callable(self.phi_dist):
 			phi = self.phi_dist()
 		else:
 			phi = self.phi_dist
-		
+
 		e1 = (1 - q)/(1+q) * np.cos(2*phi)
 		e2 = (1 - q)/(1+q) * np.sin(2*phi)
 
 		return e1,e2
 
 
 class ExternalShearTranslation():
-	"""Class that maps samples of gamma_ext, phi_ext distributions to 
+	"""Class that maps samples of gamma_ext, phi_ext distributions to
 		gamma1, gamma2
-	
-	Args: 
-		gamma_dist (scipy.stats.rv_continuous.rvs or float): distribution for 
-			external shear modulus (callable or constant) 
-		phi_dist (scipy.stats.rv_continuous.rvs or float): distribution for 
+
+	Args:
+		gamma_dist (scipy.stats.rv_continuous.rvs or float): distribution for
+			external shear modulus (callable or constant)
+		phi_dist (scipy.stats.rv_continuous.rvs or float): distribution for
 			orientation angle in radians (callable or constant)
-	
+
 	Notes:
 	"""
 
 	def __init__(self, gamma_dist,phi_dist):
 		self.gamma_dist = gamma_dist
 		self.phi_dist = phi_dist
-	
+
 	def __call__(self):
 		"""Returns gamma1, gamma2 samples
 
 		Returns:
-			(float,float): samples of external shear coordinate values 
+			(float,float): samples of external shear coordinate values
 		"""
 		if callable(self.gamma_dist):
 			gamma = self.gamma_dist()
 		else:
 			gamma = self.gamma_dist
 		if callable(self.phi_dist):
 			phi = self.phi_dist()
 		else:
 			phi = self.phi_dist
-		
+
 		gamma1 = gamma * np.cos(2*phi)
 		gamma2 = gamma * np.sin(2*phi)
-		
+
 		return gamma1,gamma2
 
 
 class KappaTransformDistribution():
-	"""Class that samples Kext given 1 / (1-Kext) ~ n. n is sampled from a 
+	"""Class that samples Kext given 1 / (1-Kext) ~ n. n is sampled from a
 	distribution given by n_dist, then Kext is computed given the
 	transformation
-	
-	Args: 
-		n_dist (scipy.stats.rv_continuous.rvs or float): distribution for 
+
+	Args:
+		n_dist (scipy.stats.rv_continuous.rvs or float): distribution for
 			1 / (1-Kext) (can be callable or constant)
 	"""
 
 	def __init__(self,n_dist):
 		self.n_dist = n_dist
 
 	def __call__(self):
 		"""Samples 1/(1-Kext), then maps that sample to Kext value
 
-		Returns: 
+		Returns:
 			(float): Kext sample
 		"""
 		if callable(self.n_dist):
 			n = self.n_dist()
 		else:
 			n = self.n_dist
-		
+
 		return 1 - (1/n)
 
 
 class Duplicate():
 	"""Class that returns two copies of the same random draw.
 
 	Args:
@@ -255,29 +255,56 @@
 			samp = self.dist()
 		else:
 			samp = self.dist
 
 		return samp,samp
 
 
+class DuplicateScatter(Duplicate):
+	"""Class that returns two copies of the same random draw with some
+	additional scatter on the second value.
+
+	Args:
+		dist (scipy.stats.rv_continuous.rvs or float): The distribution to
+			draw the sample from.
+		scatter (float): The additional scatter to add to the second draw
+			of the variable.
+	"""
+
+	def __init__(self,dist,scatter):
+		self.dist = dist
+		self.scatter = scatter
+
+	def __call__(self):
+		"""Returns two copies of the same sample with additional
+		scatter on the second sample.
+
+		Returns
+			(float,float): The two samples.
+		"""
+		# Get the samples from the super function and add the scatter.
+		samp,samp = super().__call__()
+		return samp,samp+np.random.randn()*self.scatter
+
+
 class DuplicateXY():
-	"""Class that returns two copies of x, y coordinates drawn from 
+	"""Class that returns two copies of x, y coordinates drawn from
 		distributions
 
-	Args: 
-		x_dist (scipy.stats.rv_continuous.rvs or float): distribution for x 
+	Args:
+		x_dist (scipy.stats.rv_continuous.rvs or float): distribution for x
 			(can be callable or constant)
-		y_dist (scipy.stats.rv_continuous.rvs or float): distribution for y 
+		y_dist (scipy.stats.rv_continuous.rvs or float): distribution for y
 			(can be callable or constant)
 	"""
 
 	def __init__(self,x_dist,y_dist):
 		self.x_dist = x_dist
 		self.y_dist = y_dist
-	
+
 	def __call__(self):
 		"""Returns two copies of x,y sample
 
 		Returns
 			(float,float,float,float): Two copies of x,y sampled from x_dist
 				and y_dist
 		"""
@@ -286,73 +313,98 @@
 			x = self.x_dist()
 		else:
 			x = self.x_dist
 		if callable(self.y_dist):
 			y = self.y_dist()
 		else:
 			y = self.y_dist
-		
+
 		return x,y,x,y
 
 
 class RedshiftsTruncNorm():
-	"""Class that samples z_lens and z_source from truncated normal 
+	"""Class that samples z_lens and z_source from truncated normal
 		distributions, forcing z_source > z_lens to be true
 
-	Args: 
+	Args:
 		z_lens_min (float): minimum allowed lens redshift
 		z_lens_mean (float): lens redshift mean
 		z_lens_std (float): lens redshift standard deviation
 		z_source_min (float): minimum allowed source redshift
 		z_source_mean (float): source redshift mean
 		z_source_std (float): source redshift standard deviation
 	"""
 
 	def __init__(self, z_lens_min,z_lens_mean,z_lens_std,z_source_min,
 		z_source_mean,z_source_std):
 		# transform z_lens_min, z_source_min to be in units of std. deviations
-		self.z_lens_min = (z_lens_min - z_lens_mean) / z_lens_std 
+		self.z_lens_min = (z_lens_min - z_lens_mean) / z_lens_std
 		self.z_source_min = (z_source_min - z_source_mean) / z_source_std
 		# define truncnorm dist for lens redshift
 		self.z_lens_dist = truncnorm(self.z_lens_min,np.inf,loc=z_lens_mean,
 			scale=z_lens_std).rvs
 		# save z_source info
 		self.z_source_mean = z_source_mean
 		self.z_source_std = z_source_std
-	
+
 	def __call__(self):
 		"""Returns samples of redshifts, ensuring z_source > z_lens
 
-		Returns: 
-			(float,float): z_lens,z_source 
+		Returns:
+			(float,float): z_lens,z_source
 		"""
 		z_lens = self.z_lens_dist()
 		clip = (z_lens - self.z_source_mean) / self.z_source_std
 		# number of std. devs away to stop (negative)
 		if(clip > self.z_source_min):
 			self.z_source_min = clip
 		# define truncnorm dist for source redshift
 		z_source = truncnorm(self.z_source_min,np.inf,self.z_source_mean,
 			self.z_source_std).rvs()
 
 		return z_lens,z_source
 
 
+class RedshiftsLensLight(RedshiftsTruncNorm):
+	"""Class that samples z_lens, z_lens_light, and z_source from truncated
+		normal distributions, forcing z_source > z_lens to be true and
+		z_lens_light = z_lens.
+
+	Args:
+		z_lens_min (float): minimum allowed lens redshift
+		z_lens_mean (float): lens redshift mean
+		z_lens_std (float): lens redshift standard deviation
+		z_source_min (float): minimum allowed source redshift
+		z_source_mean (float): source redshift mean
+		z_source_std (float): source redshift standard deviation
+	"""
+
+	def __call__(self):
+		"""Returns samples of redshifts, ensuring z_source > z_lens and
+		z_lens_light = z_lens.
+
+		Returns:
+			(float,float): z_lens,z_lens_light,z_source
+		"""
+		z_lens,z_source = super().__call__()
+		return z_lens,z_lens,z_source
+
+
 class MultipleValues():
 	"""Class to call dist.rvs(size=num)
 
 	Args:
 		dist (scipy.stats.rv_continuous.rvs): callable distribution
 		num (int): number of samples to return in one call
 	"""
 
 	def __init__(self, dist, num):
 		self.dist = dist
 		self.num = num
-	
+
 	def __call__(self):
 		"""Returns specified # of samples from dist
-		
-		Returns: 
+
+		Returns:
 			list(float): |num| samples from dist
 		"""
 		return self.dist(size=self.num)
```

### Comparing `paltas-0.1.1/paltas/Sampling/sampler.py` & `paltas-0.2.0/paltas/Sampling/sampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,15 +103,17 @@
 			cross_dict = self.draw_from_dict(draw_dict)
 			# Go through the params and update the full dict
 			for cross_param in cross_dict:
 				component, param = cross_param.split(':')
 				param_dict = full_param_dict[component+'_parameters']
 				# Warn the user the first time an overwrite happens
 				if param in param_dict and CROSSOBJECTWARNING:
-					warnings.warn('Parameter in cross dict specified elsewhere!'
-						+ ' Will be overwritten')
+					warnings.warn('Parameter %s in cross dict specified '%(param)
+						+ 'elsewhere! Will be overwritten. This warning only ' +
+						'flags once, but other parameters may also be ' +
+						'overwritten.')
 					CROSSOBJECTWARNING = False
 				full_param_dict[component+'_parameters'][param] = (
 					cross_dict[cross_param])
 
 		# Populate the cross objects
 		return full_param_dict
```

### Comparing `paltas-0.1.1/paltas/Sources/cosmos.py` & `paltas-0.2.0/paltas/Sources/cosmos.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,18 +48,25 @@
 	- 	min_flux_radius - minimum half-light radius for COSMOS source in pixels
 	- 	center_x - x-coordinate lens center for COSMOS source in units of
 		arcseconds
 	- 	center_y- y-coordinate lens center for COSMOS source in units of
 		arcseconds
 	- 	output_ab_zeropoint - AB magnitude zeropoint of the detector
 	- 	z_source - source redshift
+
+	Optional Parameters
+
+	-	source_absolute_magnitude - AB absolute magnitude of the source. The
+		light from the catalog galaxy will be rescaled to match this
+		magnitude.
 	"""
 	required_parameters = ('minimum_size_in_pixels','faintest_apparent_mag',
 		'max_z','smoothing_sigma','cosmos_folder','random_rotation',
-		'min_flux_radius','output_ab_zeropoint','z_source','center_x','center_y')
+		'min_flux_radius','output_ab_zeropoint','z_source','center_x',
+		'center_y')
 	# Average AB magnitude zeropoint for the COSMOS run.
 	ab_zeropoint = 25.95
 
 	def __init__(self, cosmology_parameters, source_parameters):
 		super().__init__(cosmology_parameters,source_parameters)
 
 		# Store the path as a Path object.
@@ -76,29 +83,29 @@
 		self.catalog_path = self.folder/'paltas_catalog.npy'
 		self.npy_files_path = self.folder/'npy_files'
 		if self.catalog_path.exists() and self.npy_files_path.exists():
 			self.catalog = np.load(str(self.catalog_path))
 
 		else:
 			# Make the directory where I'm going to save the npy files
-			self.npy_files_path.mkdir()
+			self.npy_files_path.mkdir(exist_ok=True)
 			# Combine all partial catalog files
 			catalogs = [unfits(str(self.folder / fn)) for fn in [
 				'real_galaxy_catalog_23.5.fits',
 				'real_galaxy_catalog_23.5_fits.fits'
 			]]
 
 			# Duplicate IDENT field crashes numpy's silly merge function.
 			catalogs[1] = numpy.lib.recfunctions.drop_fields(catalogs[1],
 				'IDENT')
 
 			# Custom fields
 			catalogs += [
 				np.zeros(len(catalogs[0]),
-					dtype=[('size_x', np.int),('size_y', np.int),('z', float),
+					dtype=[('size_x', int),('size_y', int),('z', float),
 					('pixel_width', float)])]
 
 			self.catalog = numpy.lib.recfunctions.merge_arrays(
 				catalogs, flatten=True)
 
 			self.catalog['pixel_width'] = HUBBLE_ACS_PIXEL_WIDTH
 			self.catalog['z'] = self.catalog['zphot']
@@ -106,15 +113,15 @@
 			# Loop over the images to find their sizes.
 			catalog_i = 0
 			for img, meta in self.iter_image_and_metadata_bulk(
 				message='One-time COSMOS startup'):
 				# Grab the shape of each image.
 				meta['size_x'], meta['size_y'] = img.shape
 				# Save the image as its own image.
-				img = img.astype(np.float)
+				img = img.astype(np.float64)
 				np.save(str(self.npy_files_path/('img_%d.npy'%(catalog_i))),img)
 				catalog_i += 1
 
 			np.save(self.catalog_path,self.catalog)
 
 	def __len__(self):
 		return len(self.catalog)
@@ -249,20 +256,26 @@
 	- 	min_flux_radius - minimum half-light radius for COSMOS source in pixels
 	- 	center_x - x-coordinate lens center for COSMOS source in units of
 		arcseconds
 	- 	center_y- y-coordinate lens center for COSMOS source in units of
 		arcseconds
 	- 	output_ab_zeropoint - AB magnitude zeropoint of the detector
 	- 	z_source - source redshift
+
+	Optional Parameters
+
+	-	source_absolute_magnitude - AB absolute magnitude of the source. The
+		light from the catalog galaxy will be rescaled to match this
+		magnitude.
 	"""
 
 	def __init__(self, *args, **kwargs):
 		super().__init__(*args, **kwargs)
 
-		_fit_results = self.catalog['sersicfit'].astype(np.float)
+		_fit_results = self.catalog['sersicfit'].astype(np.float64)
 		self.sercic_info = {
 			p: _fit_results[:, i]
 			for i, p in enumerate(
 				'intensity r_half n q boxiness x0 y0 phi'.split())}
 		# Convert half-light radius from pixels to arcseconds
 		self.sercic_info['r_half'] *= HUBBLE_ACS_PIXEL_WIDTH
 
@@ -380,14 +393,20 @@
 		arcseconds
 	- 	center_y- y-coordinate lens center for COSMOS source in units of
 		arcseconds
 	- 	output_ab_zeropoint - AB magnitude zeropoint of the detector
 	- 	z_source - source redshift
 	-	source_exclusion_list - A list of COSMOS source indices to exclude,
 		even if they pass the other cuts.
+
+	Optional Parameters
+
+	-	source_absolute_magnitude - AB absolute magnitude of the source. The
+		light from the catalog galaxy will be rescaled to match this
+		magnitude.
 	"""
 
 	required_parameters = ('minimum_size_in_pixels','faintest_apparent_mag',
 		'max_z','smoothing_sigma','cosmos_folder','random_rotation',
 		'min_flux_radius','source_exclusion_list','output_ab_zeropoint',
 		'center_x','center_y','z_source')
 
@@ -439,14 +458,20 @@
 		arcseconds
 	- 	center_y- y-coordinate lens center for COSMOS source in units of
 		arcseconds
 	- 	output_ab_zeropoint - AB magnitude zeropoint of the detector
 	- 	z_source - source redshift
 	-	source_inclusion_list - A list of COSMOS source indices to include,
 		cutting any source not in this list.
+
+	Optional Parameters
+
+	-	source_absolute_magnitude - AB absolute magnitude of the source. The
+		light from the catalog galaxy will be rescaled to match this
+		magnitude.
 	"""
 
 	required_parameters = ('minimum_size_in_pixels','faintest_apparent_mag',
 		'max_z','smoothing_sigma','cosmos_folder','random_rotation',
 		'min_flux_radius','source_inclusion_list','output_ab_zeropoint',
 		'center_x','center_y','z_source')
```

### Comparing `paltas-0.1.1/paltas/Sources/cosmos_sersic.py` & `paltas-0.2.0/paltas/Sources/cosmos_sersic.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Generate Lenstronomy inputs for a COSMOS galaxy + a Sersic Ellipse
 
 This module contains a class that combines a COSMOS galaxy and a Sersic light 
 distribution as the two sources for paltas.
 """
 from .cosmos import COSMOSCatalog
 from .sersic import SingleSersicSource
+from ..Utils.cosmology_utils import absolute_to_apparent
 
 
 class COSMOSSersic(COSMOSCatalog):
 	"""Class to Combine COSMOS galaxy with Sersic light source
 
 	Args:
 		cosmology_parameters (str,dict, or colossus.cosmology.Cosmology): 
@@ -43,21 +44,28 @@
 	- 	e1_sersic - x-direction ellipticity eccentricity for sersic
 	- 	e2_sersic - xy-direction ellipticity eccentricity for sersic
 	- 	center_x_sersic - x-coordinate lens center for sersic in units of
 		arcseconds
 	- 	center_y_sersic - y-coordinate lens center for sersic in units of
 		arcseconds
 	- 	z_source - source redshift
+
+	Optional Parameters
+
+	-	source_absolute_magnitude - AB absolute magnitude of the source. The
+		light from the catalog galaxy will be rescaled to match this
+		magnitude.
 	"""
 
 	required_parameters = ('minimum_size_in_pixels','faintest_apparent_mag',
 		'max_z','smoothing_sigma','cosmos_folder','random_rotation',
 		'min_flux_radius','output_ab_zeropoint','z_source', 'mag_sersic',
 		'center_x','center_y','R_sersic', 'n_sersic','e1_sersic', 'e2_sersic',
 		'center_x_sersic','center_y_sersic')
+	optional_parameters = ('source_absolute_magnitude')
 
 	def draw_source(self, catalog_i=None, phi=None):
 		"""Creates lenstronomy kwargs for a COSMOS catalog image and a 
 		Sersic source
 
 		Args:
 			catalog_i (int): Index of image in catalog
@@ -90,14 +98,16 @@
 						self.source_parameters[param_name])
 				else:
 					sersic_kwargs_dict[param_name[:-7]] = (
 						self.source_parameters[param_name])
 
 		# mag to amp conversion
 		sersic_kwargs_dict.pop('mag')
+		mag_apparent = absolute_to_apparent(self.source_parameters['mag_sersic'],
+			self.source_parameters['z_source'],self.cosmo)
 		sersic_kwargs_dict['amp'] = SingleSersicSource.mag_to_amplitude(
-			self.source_parameters['mag_sersic'],
-			self.source_parameters['output_ab_zeropoint'], sersic_kwargs_dict)
+			mag_apparent,self.source_parameters['output_ab_zeropoint'],
+			sersic_kwargs_dict)
 
 		kwargs_list.append(sersic_kwargs_dict)
 
 		return model_list, kwargs_list, [self.source_parameters['z_source']]*2
```

### Comparing `paltas-0.1.1/paltas/Sources/galaxy_catalog.py` & `paltas-0.2.0/paltas/Sources/galaxy_catalog.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,29 +3,51 @@
 Turn real galaxies into Lenstronomy inputs.
 
 This module contains the default class for transforming the objects of a
 source catalog into sources to be passed to lenstronomy.
 """
 import numpy as np
 from .source_base import SourceBase
+from ..Utils.cosmology_utils import absolute_to_apparent, get_k_correction
+from lenstronomy.Util.data_util import magnitude2cps
 
 
 class GalaxyCatalog(SourceBase):
 	"""Base class for turning real galaxy images into Lenstronomy inputs.
 
 	Args:
 		cosmology_parameters (str,dict, or colossus.cosmology.Cosmology):
 			Either a name of colossus cosmology, a dict with 'cosmology name':
 			name of colossus cosmology, an instance of colussus cosmology, or a
 			dict with H0 and Om0 ( other parameters will be set to defaults).
 		source_parameters (dict): A dictionary containing all the parameters
 			needed to draw sources (in this case random_rotation).
+
+	Notes:
+
+	Required Parameters
+
+	- 	random_rotation - boolean dictating if COSMOS sources will be rotated
+		randomly when drawn
+	- 	output_ab_zeropoint - AB magnitude zeropoint of the detector
+	- 	z_source - source redshift
+	- 	center_x - x-coordinate lens center for COSMOS source in units of
+		arcseconds
+	- 	center_y- y-coordinate lens center for COSMOS source in units of
+		arcseconds
+
+	Optional Parameters
+
+	-	source_absolute_magnitude - AB absolute magnitude of the source. The
+		light from the catalog galaxy will be rescaled to match this
+		magnitude.
 	"""
 	required_parameters = ('random_rotation','output_ab_zeropoint',
 		'z_source','center_x','center_y')
+	optional_parameters = ('source_absolute_magnitude')
 	# This parameter must be set by class inheriting GalaxyCatalog
 	ab_zeropoint = None
 
 	def __len__(self):
 		"""Returns the length of the catalog"""
 		raise NotImplementedError
 
@@ -158,26 +180,78 @@
 		# of the input survey and the output survey. Note this doesn't
 		# take into account the color of the object!
 		img *= 10**((self.source_parameters['output_ab_zeropoint']-
 			self.__class__.ab_zeropoint)/2.5)
 
 		pixel_width *= self.z_scale_factor(metadata['z'], z_new)
 
+		# Apply the k correction to the image from the redshifting
+		self.k_correct_image(img,metadata['z'],z_new)
+
+		# If a desired absolute magnitude was specified, scale the image
+		# accordingly
+		if 'source_absolute_magnitude' in self.source_parameters:
+			mag_apparent = absolute_to_apparent(
+				self.source_parameters['source_absolute_magnitude'],
+				self.source_parameters['z_source'],self.cosmo)
+			self.normalize_to_mag(img,mag_apparent,
+				self.source_parameters['output_ab_zeropoint'],pixel_width)
+
 		# Convert to kwargs for lenstronomy
 		return (
 			['INTERPOL'],
 			[dict(
 				image=img,
 				center_x=self.source_parameters['center_x'],
 				center_y=self.source_parameters['center_y'],
 				phi_G=phi,
 				scale=pixel_width)],
 			[z_new])
 
 	@staticmethod
+	def k_correct_image(image,z_original,z_new):
+		"""Apply the k-correction to the image at the pixel level.
+
+		Args:
+			image (np.array): The image that needs to be k-corrected
+			z_original (float): The original redshift of the object
+			z_new (float): The new redshift of the object
+
+		Notes:
+			image will be changed in place
+		"""
+		# Calculate the k-correction for the change in redshift
+		mag_k_correct = get_k_correction(z_new) - get_k_correction(z_original)
+
+		# Apply the correction
+		image *= 10**(-mag_k_correct/2.5)
+
+	@staticmethod
+	def normalize_to_mag(image,mag_apparent,mag_zero_point,pixel_width):
+		"""Renormalizes and image so that it has the specified apparent
+		magnitude.
+
+		Args:
+			image (np.array): Image to be renormalized
+			mag_apparent (float): TThe desired apparent magnitude
+			mag_zero_point (float): The magnitude zero-point of the detector
+			pixel_width (float): The width of a pixel in arcseconds
+		Notes:
+			Image changed in place.
+		"""
+		# Get the total flux of the image
+		flux_total = np.sum(image) * pixel_width**2
+
+		# Get the cps of an image of the desired magnitude
+		flux_true = magnitude2cps(mag_apparent, mag_zero_point)
+
+		# Rescale the image so that both values match
+		image *= flux_true/flux_total
+
+	@staticmethod
 	def draw_phi():
 		"""Draws a random rotation angle for the interpolation of the source.
 
 		Returns:
 			(float): The new angle to use in the interpolation class.
 		"""
 		return np.random.rand() * 2 * np.pi
```

### Comparing `paltas-0.1.1/paltas/Sources/source_base.py` & `paltas-0.2.0/paltas/Sources/source_base.py`

 * *Files identical despite different names*

### Comparing `paltas-0.1.1/paltas/Substructure/los_base.py` & `paltas-0.2.0/paltas/Substructure/los_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -94,17 +94,21 @@
 			each los halo returned, the second is the lenstronomy kwargs
 			for that halo, and the third is a list of redshift values for
 			each profile.
 		"""
 		raise NotImplementedError
 
 	def calculate_average_alpha(self,n_draws=100):
-		""" Calculates the average convergence from the los at each redshift
-		specified by the los parameters and returns corresponding lenstronomy
-		objects.
+		"""Calculates the average deflection maps from the los at each
+		redshift specified by the los parameters and returns corresponding
+		lenstronomy objects.
+
+		Args:
+			num_pix (int): The number of pixels to sample for our
+				interpolation maps.
 
 		Returns:
 			(tuple): A tuple of two lists: the first is the interpolation
 			profile type for each redshift slice and the second is the
 			lenstronomy kwargs for that profile.
 		"""
 		raise NotImplementedError
```

### Comparing `paltas-0.1.1/paltas/Substructure/los_dg19.py` & `paltas-0.2.0/paltas/Substructure/los_dg19.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 los halo distribution into masses, concentrations, and positions.
 """
 from .los_base import LOSBase
 import numba
 import numpy as np
 from colossus.lss import peaks, bias
 from ..Utils import power_law, cosmology_utils
-import functools
 from . import nfw_functions
 import lenstronomy.Util.util as util
 from lenstronomy.LensModel.Profiles.nfw import NFW
 from scipy.signal import fftconvolve
 
 
 class LOSDG19(LOSBase):
@@ -117,15 +116,14 @@
 		nfn_eval = self.nu_f_nu(nu)
 		d_ln_sigma_d_ln_r = self.cosmo.sigma(r,z,derivative=True)
 		# Density is returned in units of M_sun*h^2/kpc^3
 		rho_m = self.cosmo.rho_m(z)*h**2
 
 		return -1/3*nfn_eval*rho_m/m**2*d_ln_sigma_d_ln_r
 
-	@functools.lru_cache(maxsize=None)
 	def power_law_dn_dm(self,z,m_min,m_max,n_dm=100):
 		"""Returns the best fit power law parameters for the physical number
 		density at a given redshift and mass range.
 
 		Args:
 			z (float): The redshift at which to calculate the power law
 				parameters.
@@ -188,15 +186,14 @@
 
 		# Get the two halo term in the slice
 		xi_halo = self.cosmo.correlationFunction(r_cmv,z_lens)
 		xi_halo *= bias.haloBias(lens_m200*self.cosmo.h,z_lens,mdef='200c',
 			model='tinker10')
 		return 1+np.mean(xi_halo)
 
-	@functools.lru_cache(maxsize=1024)
 	def cone_angle_to_radius(self,z,z_lens,z_source,cone_angle,
 		angle_buffer=0.8):
 		"""Returns the radius in kpc at the given redshift for the given cone
 		angle.
 
 		Args:
 			z (float): The redshift at which to calculate the radius
@@ -224,15 +221,14 @@
 			scal_factor *= self.cosmo.comovingDistance(z_source)
 			scal_factor /= self.cosmo.comovingDistance(z_lens,z_source)
 			scal_factor *= self.cosmo.comovingDistance(z_lens,z)
 			scal_factor /= self.cosmo.comovingDistance(z)
 			r_los *= 1 - scal_factor
 		return r_los
 
-	@functools.lru_cache(maxsize=1024)
 	def volume_element(self,z,z_lens,z_source,dz,cone_angle,angle_buffer=0.8):
 		"""Returns the physical volume element at the given redshift
 
 		Args:
 			z (float): The redshift at which to calculate the volume element
 			z_lens (float): The redshift of the main deflector
 			z_source (float): The redshift of the source
```

### Comparing `paltas-0.1.1/paltas/Substructure/nfw_functions.py` & `paltas-0.2.0/paltas/Substructure/nfw_functions.py`

 * *Files identical despite different names*

### Comparing `paltas-0.1.1/paltas/Substructure/subhalos_base.py` & `paltas-0.2.0/paltas/Substructure/subhalos_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 	def update_parameters(self,subhalo_parameters=None,
 		main_deflector_parameters=None,source_parameters=None,
 		cosmology_parameters=None):
 		"""Updated the class parameters
 
 		Args:
-			los_parameters (dict): A dictionary containing the type of
+			subhalo_parameters (dict): A dictionary containing the type of
 				los distribution and the value for each of its parameters.
 			main_deflector_parameters (dict): A dictionary containing the type
 				of main deflector and the value for each of its parameters.
 			source_parameters (dict): A dictionary containing the type of the
 				source and the value for each of its parameters.
 			cosmology_parameters (str,dict, or colossus.cosmology.Cosmology):
 				Either a name of colossus cosmology, a dict with 'cosmology name':
```

### Comparing `paltas-0.1.1/paltas/Substructure/subhalos_dg19.py` & `paltas-0.2.0/paltas/Substructure/subhalos_dg19.py`

 * *Files identical despite different names*

### Comparing `paltas-0.1.1/paltas/Utils/hubble_utils.py` & `paltas-0.2.0/paltas/Utils/hubble_utils.py`

 * *Files identical despite different names*

### Comparing `paltas-0.1.1/paltas/Utils/lenstronomy_utils.py` & `paltas-0.2.0/paltas/Utils/lenstronomy_utils.py`

 * *Files identical despite different names*

### Comparing `paltas-0.1.1/paltas/Utils/power_law.py` & `paltas-0.2.0/paltas/Utils/power_law.py`

 * *Files identical despite different names*

### Comparing `paltas-0.1.1/paltas.egg-info/SOURCES.txt` & `paltas-0.2.0/paltas.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.rst
 setup.cfg
 setup.py
 paltas/__init__.py
 paltas/generate.py
 paltas.egg-info/PKG-INFO
 paltas.egg-info/SOURCES.txt
@@ -12,45 +13,46 @@
 paltas/Analysis/__init__.py
 paltas/Analysis/conv_models.py
 paltas/Analysis/dataset_generation.py
 paltas/Analysis/hierarchical_inference.py
 paltas/Analysis/loss_functions.py
 paltas/Analysis/pdf_functions.py
 paltas/Analysis/posterior_functions.py
-paltas/Analysis/run_hierarchical.py
 paltas/Analysis/train_model.py
+paltas/Analysis/transformer_models.py
 paltas/Configs/__init__.py
 paltas/Configs/config_handler.py
-paltas/Configs/2203_00690/config_test_1.py
-paltas/Configs/2203_00690/config_test_10.py
-paltas/Configs/2203_00690/config_test_11.py
-paltas/Configs/2203_00690/config_test_12.py
-paltas/Configs/2203_00690/config_test_13.py
-paltas/Configs/2203_00690/config_test_14.py
-paltas/Configs/2203_00690/config_test_15.py
-paltas/Configs/2203_00690/config_test_16.py
-paltas/Configs/2203_00690/config_test_17.py
-paltas/Configs/2203_00690/config_test_18.py
-paltas/Configs/2203_00690/config_test_19.py
-paltas/Configs/2203_00690/config_test_2.py
-paltas/Configs/2203_00690/config_test_20.py
-paltas/Configs/2203_00690/config_test_3.py
-paltas/Configs/2203_00690/config_test_4.py
-paltas/Configs/2203_00690/config_test_5.py
-paltas/Configs/2203_00690/config_test_6.py
-paltas/Configs/2203_00690/config_test_7.py
-paltas/Configs/2203_00690/config_test_8.py
-paltas/Configs/2203_00690/config_test_9.py
-paltas/Configs/2203_00690/config_test_high_m_min.py
-paltas/Configs/2203_00690/config_test_large_cone_angle.py
-paltas/Configs/2203_00690/config_test_large_los_dz.py
-paltas/Configs/2203_00690/config_test_low_m_min.py
-paltas/Configs/2203_00690/config_test_source_smoothing.py
-paltas/Configs/2203_00690/config_train.py
-paltas/Configs/2203_00690/config_val.py
+paltas/Configs/paper_2203_00690/__init__.py
+paltas/Configs/paper_2203_00690/config_test_01.py
+paltas/Configs/paper_2203_00690/config_test_02.py
+paltas/Configs/paper_2203_00690/config_test_03.py
+paltas/Configs/paper_2203_00690/config_test_04.py
+paltas/Configs/paper_2203_00690/config_test_05.py
+paltas/Configs/paper_2203_00690/config_test_06.py
+paltas/Configs/paper_2203_00690/config_test_07.py
+paltas/Configs/paper_2203_00690/config_test_08.py
+paltas/Configs/paper_2203_00690/config_test_09.py
+paltas/Configs/paper_2203_00690/config_test_10.py
+paltas/Configs/paper_2203_00690/config_test_11.py
+paltas/Configs/paper_2203_00690/config_test_12.py
+paltas/Configs/paper_2203_00690/config_test_13.py
+paltas/Configs/paper_2203_00690/config_test_14.py
+paltas/Configs/paper_2203_00690/config_test_15.py
+paltas/Configs/paper_2203_00690/config_test_16.py
+paltas/Configs/paper_2203_00690/config_test_17.py
+paltas/Configs/paper_2203_00690/config_test_18.py
+paltas/Configs/paper_2203_00690/config_test_19.py
+paltas/Configs/paper_2203_00690/config_test_20.py
+paltas/Configs/paper_2203_00690/config_test_high_m_min.py
+paltas/Configs/paper_2203_00690/config_test_large_cone_angle.py
+paltas/Configs/paper_2203_00690/config_test_large_los_dz.py
+paltas/Configs/paper_2203_00690/config_test_low_m_min.py
+paltas/Configs/paper_2203_00690/config_test_source_smoothing.py
+paltas/Configs/paper_2203_00690/config_train.py
+paltas/Configs/paper_2203_00690/config_val.py
 paltas/MainDeflector/__init__.py
 paltas/MainDeflector/main_deflector_base.py
 paltas/MainDeflector/simple_deflectors.py
 paltas/PointSource/__init__.py
 paltas/PointSource/point_source_base.py
 paltas/PointSource/single_point_source.py
 paltas/Sampling/__init__.py
```

### Comparing `paltas-0.1.1/setup.py` & `paltas-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 PACKAGE_PATH = os.path.abspath(os.path.join(__file__, os.pardir))
 
 required_packages = open('requirements.txt').read().splitlines()
 
 setup(
 	name='paltas',
-	version='0.1.1',
+	version='0.2.0',
 	description='Strong lens substructure package.',
 	long_description=readme,
 	author='Sebastian Wagner-Carena',
 	author_email='sebaswagner@outlook.com',
 	url='https://github.com/swagnercarena/paltas',
 	packages=find_packages(PACKAGE_PATH),
 	package_dir={'paltas': 'paltas'},
```

