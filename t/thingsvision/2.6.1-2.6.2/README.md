# Comparing `tmp/thingsvision-2.6.1.tar.gz` & `tmp/thingsvision-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thingsvision-2.6.1.tar", last modified: Mon Apr 22 11:27:18 2024, max compression
+gzip compressed data, was "thingsvision-2.6.2.tar", last modified: Wed Apr 24 14:58:24 2024, max compression
```

## Comparing `thingsvision-2.6.1.tar` & `thingsvision-2.6.2.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 11:27:18.822059 thingsvision-2.6.1/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1097 2021-01-22 09:49:59.000000 thingsvision-2.6.1/LICENSE
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16641 2024-04-22 11:27:18.821746 thingsvision-2.6.1/PKG-INFO
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16038 2024-04-22 11:26:42.000000 thingsvision-2.6.1/README.md
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       38 2024-04-22 11:27:18.822134 thingsvision-2.6.1/setup.cfg
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1698 2024-04-22 08:56:16.000000 thingsvision-2.6.1/setup.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 11:27:18.787534 thingsvision-2.6.1/tests/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-02-02 09:19:53.000000 thingsvision-2.6.1/tests/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 11:27:18.788530 thingsvision-2.6.1/tests/extractor/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.6.1/tests/extractor/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 11:27:18.791947 thingsvision-2.6.1/tests/extractor/extraction/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.6.1/tests/extractor/extraction/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2452 2024-04-06 10:03:37.000000 thingsvision-2.6.1/tests/extractor/extraction/test_custom_model.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3196 2024-04-01 11:22:39.000000 thingsvision-2.6.1/tests/extractor/extraction/test_model_extractor.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1954 2024-04-06 10:03:24.000000 thingsvision-2.6.1/tests/extractor/extraction/test_pretrained_model.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2977 2024-04-06 10:04:01.000000 thingsvision-2.6.1/tests/extractor/extraction/test_torch_vs_tensorflow.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4459 2024-04-01 11:29:46.000000 thingsvision-2.6.1/tests/extractor/test_load_extractor.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1487 2023-02-22 09:56:38.000000 thingsvision-2.6.1/tests/extractor/test_transformations.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    10967 2024-04-22 11:26:42.000000 thingsvision-2.6.1/tests/helper.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4447 2024-04-22 11:26:42.000000 thingsvision-2.6.1/tests/test_features.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4304 2024-04-22 11:26:42.000000 thingsvision-2.6.1/tests/test_rest.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 11:27:18.793258 thingsvision-2.6.1/thingsvision/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      103 2022-11-09 16:59:35.000000 thingsvision-2.6.1/thingsvision/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       22 2024-04-22 11:26:42.000000 thingsvision-2.6.1/thingsvision/_version.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 11:27:18.795757 thingsvision-2.6.1/thingsvision/core/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-23 10:25:59.000000 thingsvision-2.6.1/thingsvision/core/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 11:27:18.796923 thingsvision-2.6.1/thingsvision/core/cka/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       29 2024-04-22 08:56:16.000000 thingsvision-2.6.1/thingsvision/core/cka/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2269 2024-04-22 08:56:16.000000 thingsvision-2.6.1/thingsvision/core/cka/cka_base.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3567 2024-04-22 08:56:16.000000 thingsvision-2.6.1/thingsvision/core/cka/cka_numpy.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5957 2024-04-22 11:26:42.000000 thingsvision-2.6.1/thingsvision/core/cka/cka_torch.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      818 2024-04-22 08:56:16.000000 thingsvision-2.6.1/thingsvision/core/cka/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 11:27:18.801320 thingsvision-2.6.1/thingsvision/core/extraction/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      176 2024-04-01 11:36:55.000000 thingsvision-2.6.1/thingsvision/core/extraction/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    10749 2024-04-04 09:43:21.000000 thingsvision-2.6.1/thingsvision/core/extraction/base.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    17334 2024-04-08 11:02:58.000000 thingsvision-2.6.1/thingsvision/core/extraction/extractors.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8452 2024-04-04 09:43:21.000000 thingsvision-2.6.1/thingsvision/core/extraction/helpers.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3134 2024-04-04 09:43:21.000000 thingsvision-2.6.1/thingsvision/core/extraction/tensorflow.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8530 2024-04-19 11:52:36.000000 thingsvision-2.6.1/thingsvision/core/extraction/torch.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 11:27:18.802400 thingsvision-2.6.1/thingsvision/core/rsa/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       59 2022-08-22 09:49:44.000000 thingsvision-2.6.1/thingsvision/core/rsa/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-29 15:24:25.000000 thingsvision-2.6.1/thingsvision/core/rsa/base.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4651 2022-08-31 09:02:04.000000 thingsvision-2.6.1/thingsvision/core/rsa/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 11:27:18.808995 thingsvision-2.6.1/thingsvision/custom_models/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      286 2023-08-04 09:46:20.000000 thingsvision-2.6.1/thingsvision/custom_models/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      620 2023-07-11 09:50:14.000000 thingsvision-2.6.1/thingsvision/custom_models/alexnet_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      627 2023-07-11 09:50:14.000000 thingsvision-2.6.1/thingsvision/custom_models/alexnet_salobjsub.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 11:27:18.811174 thingsvision-2.6.1/thingsvision/custom_models/cornet/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1474 2022-08-22 09:49:44.000000 thingsvision-2.6.1/thingsvision/custom_models/cornet/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3588 2022-08-22 09:49:44.000000 thingsvision-2.6.1/thingsvision/custom_models/cornet/cornet_r.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3682 2022-08-22 09:49:44.000000 thingsvision-2.6.1/thingsvision/custom_models/cornet/cornet_rt.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4203 2022-08-22 09:49:44.000000 thingsvision-2.6.1/thingsvision/custom_models/cornet/cornet_s.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-08-22 09:49:44.000000 thingsvision-2.6.1/thingsvision/custom_models/cornet/cornet_z.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      287 2023-01-18 14:03:54.000000 thingsvision-2.6.1/thingsvision/custom_models/custom.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 11:27:18.812018 thingsvision-2.6.1/thingsvision/custom_models/dreamsim/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2023-08-04 09:46:20.000000 thingsvision-2.6.1/thingsvision/custom_models/dreamsim/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1999 2024-03-19 09:46:42.000000 thingsvision-2.6.1/thingsvision/custom_models/dreamsim/dreamsim.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 11:27:18.813298 thingsvision-2.6.1/thingsvision/custom_models/harmonization/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       41 2023-03-06 11:11:47.000000 thingsvision-2.6.1/thingsvision/custom_models/harmonization/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1366 2023-03-06 11:11:52.000000 thingsvision-2.6.1/thingsvision/custom_models/harmonization/harmonization.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      629 2023-08-04 09:17:34.000000 thingsvision-2.6.1/thingsvision/custom_models/inception_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      453 2023-07-26 10:09:51.000000 thingsvision-2.6.1/thingsvision/custom_models/official_clip.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1033 2023-07-11 09:50:14.000000 thingsvision-2.6.1/thingsvision/custom_models/openclip.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      623 2023-08-04 09:16:38.000000 thingsvision-2.6.1/thingsvision/custom_models/resnet50_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      614 2023-08-04 09:31:47.000000 thingsvision-2.6.1/thingsvision/custom_models/vgg16_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      621 2023-08-04 09:46:20.000000 thingsvision-2.6.1/thingsvision/custom_models/vgg16bn_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5992 2024-04-16 08:05:49.000000 thingsvision-2.6.1/thingsvision/thingsvision.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 11:27:18.813994 thingsvision-2.6.1/thingsvision/utils/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-26 11:38:32.000000 thingsvision-2.6.1/thingsvision/utils/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 11:27:18.814679 thingsvision-2.6.1/thingsvision/utils/alignment/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2024-03-28 13:19:33.000000 thingsvision-2.6.1/thingsvision/utils/alignment/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2633 2024-03-28 13:33:43.000000 thingsvision-2.6.1/thingsvision/utils/alignment/transforms.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 11:27:18.815192 thingsvision-2.6.1/thingsvision/utils/checkpointing/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      522 2023-07-26 10:09:51.000000 thingsvision-2.6.1/thingsvision/utils/checkpointing/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 11:27:18.817187 thingsvision-2.6.1/thingsvision/utils/data/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-11-15 12:25:36.000000 thingsvision-2.6.1/thingsvision/utils/data/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1778 2022-11-15 12:25:36.000000 thingsvision-2.6.1/thingsvision/utils/data/data_loader.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7808 2022-11-15 12:25:36.000000 thingsvision-2.6.1/thingsvision/utils/data/dataset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2969 2022-08-25 08:25:51.000000 thingsvision-2.6.1/thingsvision/utils/data/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 11:27:18.817895 thingsvision-2.6.1/thingsvision/utils/imagenet/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2355 2022-08-22 09:49:44.000000 thingsvision-2.6.1/thingsvision/utils/imagenet/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 11:27:18.818205 thingsvision-2.6.1/thingsvision/utils/models/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2023-08-09 09:09:13.000000 thingsvision-2.6.1/thingsvision/utils/models/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 11:27:18.819385 thingsvision-2.6.1/thingsvision/utils/models/dino/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       62 2024-04-05 17:27:52.000000 thingsvision-2.6.1/thingsvision/utils/models/dino/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2396 2023-08-08 13:01:35.000000 thingsvision-2.6.1/thingsvision/utils/models/dino/utils.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11168 2023-08-08 13:01:35.000000 thingsvision-2.6.1/thingsvision/utils/models/dino/vision_transformer.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 11:27:18.820828 thingsvision-2.6.1/thingsvision/utils/models/mae/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      116 2024-04-08 11:02:58.000000 thingsvision-2.6.1/thingsvision/utils/models/mae/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2157 2024-04-08 11:02:58.000000 thingsvision-2.6.1/thingsvision/utils/models/mae/utils.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2108 2024-04-08 11:02:58.000000 thingsvision-2.6.1/thingsvision/utils/models/mae/vit_mae.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 11:27:18.821425 thingsvision-2.6.1/thingsvision/utils/storing/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       67 2022-08-22 09:49:44.000000 thingsvision-2.6.1/thingsvision/utils/storing/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7325 2024-04-20 11:40:10.000000 thingsvision-2.6.1/thingsvision/utils/storing/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 11:27:18.795457 thingsvision-2.6.1/thingsvision.egg-info/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16641 2024-04-22 11:27:18.000000 thingsvision-2.6.1/thingsvision.egg-info/PKG-INFO
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2880 2024-04-22 11:27:18.000000 thingsvision-2.6.1/thingsvision.egg-info/SOURCES.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       39 2024-04-22 11:27:18.000000 thingsvision-2.6.1/thingsvision.egg-info/dependency_links.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       64 2024-04-22 11:27:18.000000 thingsvision-2.6.1/thingsvision.egg-info/entry_points.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      325 2024-04-22 11:27:18.000000 thingsvision-2.6.1/thingsvision.egg-info/requires.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       19 2024-04-22 11:27:18.000000 thingsvision-2.6.1/thingsvision.egg-info/top_level.txt
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-24 14:58:24.512333 thingsvision-2.6.2/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1097 2021-01-22 09:49:59.000000 thingsvision-2.6.2/LICENSE
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16819 2024-04-24 14:58:24.512028 thingsvision-2.6.2/PKG-INFO
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16216 2024-04-24 14:58:04.000000 thingsvision-2.6.2/README.md
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       38 2024-04-24 14:58:24.512412 thingsvision-2.6.2/setup.cfg
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1698 2024-04-22 08:56:16.000000 thingsvision-2.6.2/setup.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-24 14:58:24.481728 thingsvision-2.6.2/tests/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-02-02 09:19:53.000000 thingsvision-2.6.2/tests/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-24 14:58:24.482774 thingsvision-2.6.2/tests/extractor/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.6.2/tests/extractor/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-24 14:58:24.484978 thingsvision-2.6.2/tests/extractor/extraction/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.6.2/tests/extractor/extraction/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2452 2024-04-06 10:03:37.000000 thingsvision-2.6.2/tests/extractor/extraction/test_custom_model.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3196 2024-04-01 11:22:39.000000 thingsvision-2.6.2/tests/extractor/extraction/test_model_extractor.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1954 2024-04-22 12:22:02.000000 thingsvision-2.6.2/tests/extractor/extraction/test_pretrained_model.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2977 2024-04-06 10:04:01.000000 thingsvision-2.6.2/tests/extractor/extraction/test_torch_vs_tensorflow.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4459 2024-04-22 12:21:01.000000 thingsvision-2.6.2/tests/extractor/test_load_extractor.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1487 2023-02-22 09:56:38.000000 thingsvision-2.6.2/tests/extractor/test_transformations.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11260 2024-04-24 14:58:04.000000 thingsvision-2.6.2/tests/helper.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4447 2024-04-22 11:26:42.000000 thingsvision-2.6.2/tests/test_features.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4304 2024-04-22 11:26:42.000000 thingsvision-2.6.2/tests/test_rest.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-24 14:58:24.486231 thingsvision-2.6.2/thingsvision/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      103 2022-11-09 16:59:35.000000 thingsvision-2.6.2/thingsvision/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       22 2024-04-24 14:58:04.000000 thingsvision-2.6.2/thingsvision/_version.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-24 14:58:24.488181 thingsvision-2.6.2/thingsvision/core/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-23 10:25:59.000000 thingsvision-2.6.2/thingsvision/core/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-24 14:58:24.489987 thingsvision-2.6.2/thingsvision/core/cka/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       29 2024-04-22 08:56:16.000000 thingsvision-2.6.2/thingsvision/core/cka/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2269 2024-04-22 08:56:16.000000 thingsvision-2.6.2/thingsvision/core/cka/cka_base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3567 2024-04-22 08:56:16.000000 thingsvision-2.6.2/thingsvision/core/cka/cka_numpy.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5957 2024-04-22 11:26:42.000000 thingsvision-2.6.2/thingsvision/core/cka/cka_torch.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      818 2024-04-22 08:56:16.000000 thingsvision-2.6.2/thingsvision/core/cka/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-24 14:58:24.491638 thingsvision-2.6.2/thingsvision/core/extraction/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      176 2024-04-24 08:51:44.000000 thingsvision-2.6.2/thingsvision/core/extraction/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    10927 2024-04-24 14:58:04.000000 thingsvision-2.6.2/thingsvision/core/extraction/base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    17346 2024-04-24 14:58:04.000000 thingsvision-2.6.2/thingsvision/core/extraction/extractors.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8453 2024-04-24 14:58:04.000000 thingsvision-2.6.2/thingsvision/core/extraction/helpers.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3134 2024-04-04 09:43:21.000000 thingsvision-2.6.2/thingsvision/core/extraction/tensorflow.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    10948 2024-04-24 14:58:04.000000 thingsvision-2.6.2/thingsvision/core/extraction/torch.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-24 14:58:24.492491 thingsvision-2.6.2/thingsvision/core/rsa/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       59 2022-08-22 09:49:44.000000 thingsvision-2.6.2/thingsvision/core/rsa/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-29 15:24:25.000000 thingsvision-2.6.2/thingsvision/core/rsa/base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4651 2022-08-31 09:02:04.000000 thingsvision-2.6.2/thingsvision/core/rsa/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-24 14:58:24.498129 thingsvision-2.6.2/thingsvision/custom_models/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      286 2023-08-04 09:46:20.000000 thingsvision-2.6.2/thingsvision/custom_models/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      620 2023-07-11 09:50:14.000000 thingsvision-2.6.2/thingsvision/custom_models/alexnet_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      627 2023-07-11 09:50:14.000000 thingsvision-2.6.2/thingsvision/custom_models/alexnet_salobjsub.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-24 14:58:24.500151 thingsvision-2.6.2/thingsvision/custom_models/cornet/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1474 2022-08-22 09:49:44.000000 thingsvision-2.6.2/thingsvision/custom_models/cornet/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3588 2022-08-22 09:49:44.000000 thingsvision-2.6.2/thingsvision/custom_models/cornet/cornet_r.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3682 2022-08-22 09:49:44.000000 thingsvision-2.6.2/thingsvision/custom_models/cornet/cornet_rt.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4203 2022-08-22 09:49:44.000000 thingsvision-2.6.2/thingsvision/custom_models/cornet/cornet_s.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-08-22 09:49:44.000000 thingsvision-2.6.2/thingsvision/custom_models/cornet/cornet_z.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      287 2023-01-18 14:03:54.000000 thingsvision-2.6.2/thingsvision/custom_models/custom.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-24 14:58:24.500953 thingsvision-2.6.2/thingsvision/custom_models/dreamsim/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2023-08-04 09:46:20.000000 thingsvision-2.6.2/thingsvision/custom_models/dreamsim/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1999 2024-03-19 09:46:42.000000 thingsvision-2.6.2/thingsvision/custom_models/dreamsim/dreamsim.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-24 14:58:24.502197 thingsvision-2.6.2/thingsvision/custom_models/harmonization/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       41 2023-03-06 11:11:47.000000 thingsvision-2.6.2/thingsvision/custom_models/harmonization/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1366 2023-03-06 11:11:52.000000 thingsvision-2.6.2/thingsvision/custom_models/harmonization/harmonization.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      629 2023-08-04 09:17:34.000000 thingsvision-2.6.2/thingsvision/custom_models/inception_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      453 2023-07-26 10:09:51.000000 thingsvision-2.6.2/thingsvision/custom_models/official_clip.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1033 2023-07-11 09:50:14.000000 thingsvision-2.6.2/thingsvision/custom_models/openclip.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      623 2023-08-04 09:16:38.000000 thingsvision-2.6.2/thingsvision/custom_models/resnet50_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      614 2023-08-04 09:31:47.000000 thingsvision-2.6.2/thingsvision/custom_models/vgg16_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      621 2023-08-04 09:46:20.000000 thingsvision-2.6.2/thingsvision/custom_models/vgg16bn_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5992 2024-04-16 08:05:49.000000 thingsvision-2.6.2/thingsvision/thingsvision.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-24 14:58:24.502645 thingsvision-2.6.2/thingsvision/utils/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-26 11:38:32.000000 thingsvision-2.6.2/thingsvision/utils/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-24 14:58:24.503562 thingsvision-2.6.2/thingsvision/utils/alignment/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2024-03-28 13:19:33.000000 thingsvision-2.6.2/thingsvision/utils/alignment/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2633 2024-03-28 13:33:43.000000 thingsvision-2.6.2/thingsvision/utils/alignment/transforms.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-24 14:58:24.504565 thingsvision-2.6.2/thingsvision/utils/checkpointing/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      522 2023-07-26 10:09:51.000000 thingsvision-2.6.2/thingsvision/utils/checkpointing/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-24 14:58:24.506464 thingsvision-2.6.2/thingsvision/utils/data/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-11-15 12:25:36.000000 thingsvision-2.6.2/thingsvision/utils/data/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1778 2022-11-15 12:25:36.000000 thingsvision-2.6.2/thingsvision/utils/data/data_loader.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7808 2022-11-15 12:25:36.000000 thingsvision-2.6.2/thingsvision/utils/data/dataset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2969 2022-08-25 08:25:51.000000 thingsvision-2.6.2/thingsvision/utils/data/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-24 14:58:24.507305 thingsvision-2.6.2/thingsvision/utils/imagenet/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2355 2022-08-22 09:49:44.000000 thingsvision-2.6.2/thingsvision/utils/imagenet/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-24 14:58:24.507601 thingsvision-2.6.2/thingsvision/utils/models/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2023-08-09 09:09:13.000000 thingsvision-2.6.2/thingsvision/utils/models/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-24 14:58:24.508799 thingsvision-2.6.2/thingsvision/utils/models/dino/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       62 2024-04-05 17:27:52.000000 thingsvision-2.6.2/thingsvision/utils/models/dino/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2396 2023-08-08 13:01:35.000000 thingsvision-2.6.2/thingsvision/utils/models/dino/utils.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11168 2023-08-08 13:01:35.000000 thingsvision-2.6.2/thingsvision/utils/models/dino/vision_transformer.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-24 14:58:24.510422 thingsvision-2.6.2/thingsvision/utils/models/mae/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      116 2024-04-08 11:02:58.000000 thingsvision-2.6.2/thingsvision/utils/models/mae/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2157 2024-04-08 11:02:58.000000 thingsvision-2.6.2/thingsvision/utils/models/mae/utils.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2108 2024-04-08 11:02:58.000000 thingsvision-2.6.2/thingsvision/utils/models/mae/vit_mae.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-24 14:58:24.511252 thingsvision-2.6.2/thingsvision/utils/storing/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       67 2022-08-22 09:49:44.000000 thingsvision-2.6.2/thingsvision/utils/storing/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7325 2024-04-20 11:40:10.000000 thingsvision-2.6.2/thingsvision/utils/storing/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-24 14:58:24.487961 thingsvision-2.6.2/thingsvision.egg-info/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16819 2024-04-24 14:58:24.000000 thingsvision-2.6.2/thingsvision.egg-info/PKG-INFO
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2880 2024-04-24 14:58:24.000000 thingsvision-2.6.2/thingsvision.egg-info/SOURCES.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       39 2024-04-24 14:58:24.000000 thingsvision-2.6.2/thingsvision.egg-info/dependency_links.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       64 2024-04-24 14:58:24.000000 thingsvision-2.6.2/thingsvision.egg-info/entry_points.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      325 2024-04-24 14:58:24.000000 thingsvision-2.6.2/thingsvision.egg-info/requires.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       19 2024-04-24 14:58:24.000000 thingsvision-2.6.2/thingsvision.egg-info/top_level.txt
```

### Comparing `thingsvision-2.6.1/LICENSE` & `thingsvision-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/PKG-INFO` & `thingsvision-2.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thingsvision
-Version: 2.6.1
+Version: 2.6.2
 Summary: Extracting image features from state-of-the-art neural networks for Computer Vision made easy
 Home-page: https://github.com/ViCCo-Group/thingsvision
 Author: Lukas Muttenthaler
 Author-email: muttenthaler@cbs.mpg.de
 License: MIT License
 Keywords: feature extraction
 Classifier: Programming Language :: Python :: 3.8
@@ -72,16 +72,16 @@
 
 <!-- Functionality -->
 ### :mechanical_arm: Functionality
 With `thingsvision`, you can:
 - extract features for any imageset from many popular networks.
 - extract features for any imageset from your custom networks.
 - extract features for >26,000 images from the [THINGS image database](https://osf.io/jum2f/).
-- [align](https://vicco-group.github.io/thingsvision/Alignment.html) the extracted features with human object perception.
-- extract features from [HDF5 datasets](https://vicco-group.github.io/thingsvision/LoadingYourData.html#using-the-hdf5dataset-class) directly (e.g., NSD stimuli)
+- [align](https://vicco-group.github.io/thingsvision/Alignment.html) the extracted features with human object perception (e.g., using [gLocal](https://proceedings.neurips.cc/paper_files/paper/2023/hash/9febda1c8344cc5f2d51713964864e93-Abstract-Conference.html)).
+- extract features from [HDF5 datasets](https://vicco-group.github.io/thingsvision/LoadingYourData.html#using-the-hdf5dataset-class) directly (e.g., [NSD stimuli](https://naturalscenesdataset.org/))
 - conduct basic [Representational Similarity Analysis (RSA)](https://vicco-group.github.io/thingsvision/RSA.html#representational-similarity-analysis-rsa) after feature extraction.
 - perform efficient [Centered Kernel Alignment (CKA)](https://vicco-group.github.io/thingsvision/RSA.html#centered-kernel-alignment-cka) to compare image features across model-module combinations.
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- Model collection -->
 ### :file_cabinet: Model collection
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thingsvision Version: 2.6.1 Summary: Extracting
+Metadata-Version: 2.1 Name: thingsvision Version: 2.6.2 Summary: Extracting
 image features from state-of-the-art neural networks for Computer Vision made
 easy Home-page: https://github.com/ViCCo-Group/thingsvision Author: Lukas
 Muttenthaler Author-email: muttenthaler@cbs.mpg.de License: MIT License
 Keywords: feature extraction Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
@@ -30,22 +30,24 @@
 rotating_light:
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### :mechanical_arm: Functionality With `thingsvision`, you can: - extract
 features for any imageset from many popular networks. - extract features for
 any imageset from your custom networks. - extract features for >26,000 images
 from the [THINGS image database](https://osf.io/jum2f/). - [align](https://
 vicco-group.github.io/thingsvision/Alignment.html) the extracted features with
-human object perception. - extract features from [HDF5 datasets](https://vicco-
+human object perception (e.g., using [gLocal](https://proceedings.neurips.cc/
+paper_files/paper/2023/hash/9febda1c8344cc5f2d51713964864e93-Abstract-
+Conference.html)). - extract features from [HDF5 datasets](https://vicco-
 group.github.io/thingsvision/LoadingYourData.html#using-the-hdf5dataset-class)
-directly (e.g., NSD stimuli) - conduct basic [Representational Similarity
-Analysis (RSA)](https://vicco-group.github.io/thingsvision/
-RSA.html#representational-similarity-analysis-rsa) after feature extraction. -
-perform efficient [Centered Kernel Alignment (CKA)](https://vicco-
-group.github.io/thingsvision/RSA.html#centered-kernel-alignment-cka) to compare
-image features across model-module combinations.
+directly (e.g., [NSD stimuli](https://naturalscenesdataset.org/)) - conduct
+basic [Representational Similarity Analysis (RSA)](https://vicco-
+group.github.io/thingsvision/RSA.html#representational-similarity-analysis-rsa)
+after feature extraction. - perform efficient [Centered Kernel Alignment (CKA)]
+(https://vicco-group.github.io/thingsvision/RSA.html#centered-kernel-alignment-
+cka) to compare image features across model-module combinations.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### :file_cabinet: Model collection Neural networks come from different
 sources. With `thingsvision`, you can extract image representations of all
 models from: - [torchvision](https://pytorch.org/vision/0.8/models.html) -
 [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications) -
 [timm](https://github.com/rwightman/pytorch-image-models) - `ssl` (self-
 supervised learning models) - `simclr-rn50`, `mocov2-rn50`, `barlowtwins-rn50`,
```

### Comparing `thingsvision-2.6.1/README.md` & `thingsvision-2.6.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,16 @@
 
 <!-- Functionality -->
 ### :mechanical_arm: Functionality
 With `thingsvision`, you can:
 - extract features for any imageset from many popular networks.
 - extract features for any imageset from your custom networks.
 - extract features for >26,000 images from the [THINGS image database](https://osf.io/jum2f/).
-- [align](https://vicco-group.github.io/thingsvision/Alignment.html) the extracted features with human object perception.
-- extract features from [HDF5 datasets](https://vicco-group.github.io/thingsvision/LoadingYourData.html#using-the-hdf5dataset-class) directly (e.g., NSD stimuli)
+- [align](https://vicco-group.github.io/thingsvision/Alignment.html) the extracted features with human object perception (e.g., using [gLocal](https://proceedings.neurips.cc/paper_files/paper/2023/hash/9febda1c8344cc5f2d51713964864e93-Abstract-Conference.html)).
+- extract features from [HDF5 datasets](https://vicco-group.github.io/thingsvision/LoadingYourData.html#using-the-hdf5dataset-class) directly (e.g., [NSD stimuli](https://naturalscenesdataset.org/))
 - conduct basic [Representational Similarity Analysis (RSA)](https://vicco-group.github.io/thingsvision/RSA.html#representational-similarity-analysis-rsa) after feature extraction.
 - perform efficient [Centered Kernel Alignment (CKA)](https://vicco-group.github.io/thingsvision/RSA.html#centered-kernel-alignment-cka) to compare image features across model-module combinations.
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- Model collection -->
 ### :file_cabinet: Model collection
```

#### html2text {}

```diff
@@ -22,22 +22,24 @@
 rotating_light:
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### :mechanical_arm: Functionality With `thingsvision`, you can: - extract
 features for any imageset from many popular networks. - extract features for
 any imageset from your custom networks. - extract features for >26,000 images
 from the [THINGS image database](https://osf.io/jum2f/). - [align](https://
 vicco-group.github.io/thingsvision/Alignment.html) the extracted features with
-human object perception. - extract features from [HDF5 datasets](https://vicco-
+human object perception (e.g., using [gLocal](https://proceedings.neurips.cc/
+paper_files/paper/2023/hash/9febda1c8344cc5f2d51713964864e93-Abstract-
+Conference.html)). - extract features from [HDF5 datasets](https://vicco-
 group.github.io/thingsvision/LoadingYourData.html#using-the-hdf5dataset-class)
-directly (e.g., NSD stimuli) - conduct basic [Representational Similarity
-Analysis (RSA)](https://vicco-group.github.io/thingsvision/
-RSA.html#representational-similarity-analysis-rsa) after feature extraction. -
-perform efficient [Centered Kernel Alignment (CKA)](https://vicco-
-group.github.io/thingsvision/RSA.html#centered-kernel-alignment-cka) to compare
-image features across model-module combinations.
+directly (e.g., [NSD stimuli](https://naturalscenesdataset.org/)) - conduct
+basic [Representational Similarity Analysis (RSA)](https://vicco-
+group.github.io/thingsvision/RSA.html#representational-similarity-analysis-rsa)
+after feature extraction. - perform efficient [Centered Kernel Alignment (CKA)]
+(https://vicco-group.github.io/thingsvision/RSA.html#centered-kernel-alignment-
+cka) to compare image features across model-module combinations.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### :file_cabinet: Model collection Neural networks come from different
 sources. With `thingsvision`, you can extract image representations of all
 models from: - [torchvision](https://pytorch.org/vision/0.8/models.html) -
 [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications) -
 [timm](https://github.com/rwightman/pytorch-image-models) - `ssl` (self-
 supervised learning models) - `simclr-rn50`, `mocov2-rn50`, `barlowtwins-rn50`,
```

### Comparing `thingsvision-2.6.1/setup.py` & `thingsvision-2.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/tests/extractor/extraction/test_custom_model.py` & `thingsvision-2.6.2/tests/extractor/extraction/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/tests/extractor/extraction/test_model_extractor.py` & `thingsvision-2.6.2/tests/extractor/extraction/test_model_extractor.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/tests/extractor/extraction/test_pretrained_model.py` & `thingsvision-2.6.2/tests/extractor/extraction/test_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/tests/extractor/extraction/test_torch_vs_tensorflow.py` & `thingsvision-2.6.2/tests/extractor/extraction/test_torch_vs_tensorflow.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/tests/extractor/test_load_extractor.py` & `thingsvision-2.6.2/tests/extractor/test_load_extractor.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/tests/extractor/test_transformations.py` & `thingsvision-2.6.2/tests/extractor/test_transformations.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/tests/helper.py` & `thingsvision-2.6.2/tests/helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         "source": "torchvision",
     },
     "vit_b_16": {
         "model_name": "vit_b_16",
         "modules": ["encoder.ln"],
         "pretrained": True,
         "source": "torchvision",
-        "kwargs": {"extract_cls_token": True, "weights": "DEFAULT"},
+        "kwargs": {"token_extraction": "cls_token", "weights": "DEFAULT"},
     },
     # Hardcoded models
     "cornet_r": {
         "model_name": "cornet_r",
         "modules": ["decoder.flatten"],
         "pretrained": True,
         "source": "custom",
@@ -83,20 +83,27 @@
         "modules": ["visual"],
         "pretrained": True,
         "source": "custom",
         "clip": True,
         "kwargs": {"variant": "ViT-L-14", "dataset": "laion400m_e32"},
     },
     # Timm models
-    "mixnet_l": {
-        "model_name": "mixnet_l",
-        "modules": ["conv_head"],
-        "pretrained": True,
-        "source": "timm",
-    },
+    # "vit_base_patch16_224": {
+    #    "model_name": "vit_base_patch16_224",
+    #    "modules": ["encoder.ln"],
+    #    "pretrained": True,
+    #    "source": "timm",
+    #    "kwargs": {"token_extraction": "avg_pool"},
+    # },
+    # "mixnet_l": {
+    #    "model_name": "mixnet_l",
+    #    "modules": ["conv_head"],
+    #    "pretrained": True,
+    #    "source": "timm",
+    # },
     # Keras models
     "VGG16_keras": {
         "model_name": "VGG16",
         "modules": ["block1_conv1", "flatten"],
         "pretrained": True,
         "source": "keras",
     },
@@ -132,50 +139,50 @@
         "source": "ssl",
     },
     "dino-vit-tiny-p8": {
         "model_name": "dino-vit-small-p8",
         "modules": ["norm"],
         "pretrained": True,
         "source": "ssl",
-        "kwargs": {"extract_cls_token": True},
+        "kwargs": {"token_extraction": "cls_token+avg_pool"},
     },
     "dino-vit-small-p8": {
         "model_name": "dino-vit-small-p8",
         "modules": ["norm"],
         "pretrained": True,
         "source": "ssl",
-        "kwargs": {"extract_cls_token": True},
+        "kwargs": {"token_extraction": "avg_pool"},
     },
     "dino-vit-base-p8": {
         "model_name": "dino-vit-base-p8",
         "modules": ["norm"],
         "pretrained": True,
         "source": "ssl",
-        "kwargs": {"extract_cls_token": True},
+        "kwargs": {"token_extraction": "cls_token"},
     },
     "dinov2-vit-small-p14": {
         "model_name": "dinov2-vit-small-p14",
         "modules": ["norm"],
         "pretrained": True,
         "source": "ssl",
-        "kwargs": {"extract_cls_token": True},
+        "kwargs": {"token_extraction": "cls_token+avg_pool"},
     },
     "dinov2-vit-base-p14": {
         "model_name": "dinov2-vit-base-p14",
         "modules": ["norm"],
         "pretrained": True,
         "source": "ssl",
         "kwargs": {"extract_cls_token": True},
     },
     "mae-vit-base-p16": {
         "model_name": "mae-vit-base-p16",
         "modules": ["norm", "fc_norm"],
         "pretrained": True,
         "source": "ssl",
-        "kwargs": {"extract_cls_token": True},
+        "kwargs": {"token_extraction": "avg_pool"},
     },
     # Additional models
     "Harmonization_visual_ResNet50": {
         "model_name": "Harmonization",
         "modules": ["avg_pool"],
         "pretrained": True,
         "source": "custom",
```

### Comparing `thingsvision-2.6.1/tests/test_features.py` & `thingsvision-2.6.2/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/tests/test_rest.py` & `thingsvision-2.6.2/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/core/cka/cka_base.py` & `thingsvision-2.6.2/thingsvision/core/cka/cka_base.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/core/cka/cka_numpy.py` & `thingsvision-2.6.2/thingsvision/core/cka/cka_numpy.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/core/cka/cka_torch.py` & `thingsvision-2.6.2/thingsvision/core/cka/cka_torch.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/core/cka/helpers.py` & `thingsvision-2.6.2/thingsvision/core/cka/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/core/extraction/base.py` & `thingsvision-2.6.2/thingsvision/core/extraction/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import abc
 import os
 import re
 import warnings
 from typing import Callable, Iterator, List, Optional, Union
 
 import numpy as np
-import torch
 from torchtyping import TensorType
 from tqdm.auto import tqdm
 
+import torch
+
 Array = np.ndarray
 
 
 class BaseExtractor(metaclass=abc.ABCMeta):
     def __init__(self, device, preprocess) -> None:
         self.device = device
         self._check_device()
@@ -22,14 +23,15 @@
         warnings.warn(
             message="\nThe .show() method is deprecated and will be removed in future versions. Use .show_model() instead.\n",
             category=UserWarning,
         )
         self.show_model()
 
     def _check_device(self) -> None:
+        """Check whether the selected device is available on the current compute node."""
         if self.device.startswith("cuda"):
             gpu_index = re.search(r"cuda:(\d+)", self.device)
 
             if not torch.cuda.is_available():
                 warnings.warn(
                     "\nCUDA is not available on your system. Switching to device='cpu'.\n",
                     category=UserWarning,
@@ -40,15 +42,15 @@
                     f"\nGPU index {gpu_index.group(1)} is out of range. "
                     f"Available GPUs: {torch.cuda.device_count()}. "
                     f"Switching to device='cuda:0'.\n",
                     category=UserWarning,
                 )
                 self.device = "cuda:0"
 
-        print("Using device: ", self.device)
+        print(f"\nUsing device: {self.device}\n")
 
     @abc.abstractmethod
     def show_model(self) -> None:
         """Show architecture."""
         raise NotImplementedError
 
     @abc.abstractmethod
@@ -82,15 +84,15 @@
             TensorType["b", "num_maps", "h_prime", "w_prime"],
             TensorType["b", "t", "d"],
             TensorType["b", "p"],
             TensorType["b", "d"],
         ],
         Array,
     ]:
-        """Extract hidden unit activations (at specified layer) for every image in a mini-batch.
+        """Extract the activations of a selected module for every image in a mini-batch.
 
         Parameters
         ----------
         batch : np.ndarray or torch.Tensor
             mini-batch of three-dimensional image tensors.
         module_name : str
             Name of the module for which features should be extraced.
@@ -120,14 +122,15 @@
             TensorType["b", "d"],
         ],
         Array,
     ]:
         raise NotImplementedError
 
     def get_output_types(self) -> List[str]:
+        """Return the list of available output types (for the feature matrix)."""
         return ["ndarray", "tensor"]
 
     def _module_and_output_check(self, module_name: str, output_type: str) -> None:
         """Checks whether the provided module name and output type are valid."""
         valid_names = self.get_module_names()
         if not module_name in valid_names:
             raise ValueError(
@@ -137,15 +140,15 @@
             output_type in self.get_output_types()
         ), f"\nData type of output feature matrix must be set to one of the following available data types: {self.get_output_types()}\n"
 
     def extract_features(
         self,
         batches: Iterator[Union[TensorType["b", "c", "h", "w"], Array]],
         module_name: str,
-        flatten_acts: bool,
+        flatten_acts: bool = False,
         output_type: Optional[str] = "ndarray",
         output_dir: Optional[str] = None,
         step_size: Optional[int] = None,
     ) -> Union[
         Union[
             TensorType["n", "num_maps", "h_prime", "w_prime"],
             TensorType["n", "t", "d"],
```

### Comparing `thingsvision-2.6.1/thingsvision/core/extraction/extractors.py` & `thingsvision-2.6.2/thingsvision/core/extraction/extractors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import numpy as np
+import timm
+import torchvision
+
 import tensorflow as tf
 import tensorflow.keras.applications as tensorflow_models
-import timm
 import torch
-import torchvision
 
 try:
     from torch.hub import load_state_dict_from_url
 except ImportError:
     from torch.utils.model_zoo import load_url as load_state_dict_from_url
 
 from thingsvision.utils.checkpointing import get_torch_home
@@ -130,15 +131,15 @@
             preprocess=preprocess,
             device=device,
         )
 
     def load_model_from_source(self) -> None:
         """Load a (pretrained) neural network model from <timm>."""
         if self.model_name in timm.list_models():
-            self.model = timm.create_model(self.model_name, self.pretrained)
+            self.model = timm.create_model(self.model_name, pretrained=self.pretrained)
         else:
             raise ValueError(
                 f"\nCould not find {self.model_name} in timm library.\nChoose a different model.\n"
             )
 
 
 class KerasExtractor(TensorFlowExtractor):
```

### Comparing `thingsvision-2.6.1/thingsvision/core/extraction/helpers.py` & `thingsvision-2.6.2/thingsvision/core/extraction/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import warnings
 from typing import Any, Callable, Dict, Union
 
 import numpy as np
-import torch
 from torchtyping import TensorType
 
+import torch
+
 from .extractors import (
     KerasExtractor,
     SSLExtractor,
     TimmExtractor,
     TorchvisionExtractor,
 )
 from .tensorflow import TensorFlowExtractor
```

### Comparing `thingsvision-2.6.1/thingsvision/core/extraction/tensorflow.py` & `thingsvision-2.6.2/thingsvision/core/extraction/tensorflow.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/core/rsa/helpers.py` & `thingsvision-2.6.2/thingsvision/core/rsa/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/custom_models/alexnet_ecoset.py` & `thingsvision-2.6.2/thingsvision/custom_models/alexnet_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/custom_models/alexnet_salobjsub.py` & `thingsvision-2.6.2/thingsvision/custom_models/alexnet_salobjsub.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/custom_models/cornet/__init__.py` & `thingsvision-2.6.2/thingsvision/custom_models/cornet/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/custom_models/cornet/cornet_r.py` & `thingsvision-2.6.2/thingsvision/custom_models/cornet/cornet_r.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/custom_models/cornet/cornet_rt.py` & `thingsvision-2.6.2/thingsvision/custom_models/cornet/cornet_rt.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/custom_models/cornet/cornet_s.py` & `thingsvision-2.6.2/thingsvision/custom_models/cornet/cornet_s.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/custom_models/cornet/cornet_z.py` & `thingsvision-2.6.2/thingsvision/custom_models/cornet/cornet_z.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/custom_models/dreamsim/dreamsim.py` & `thingsvision-2.6.2/thingsvision/custom_models/dreamsim/dreamsim.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/custom_models/harmonization/harmonization.py` & `thingsvision-2.6.2/thingsvision/custom_models/harmonization/harmonization.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/custom_models/inception_ecoset.py` & `thingsvision-2.6.2/thingsvision/custom_models/inception_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/custom_models/openclip.py` & `thingsvision-2.6.2/thingsvision/custom_models/openclip.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/custom_models/resnet50_ecoset.py` & `thingsvision-2.6.2/thingsvision/custom_models/resnet50_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/custom_models/vgg16_ecoset.py` & `thingsvision-2.6.2/thingsvision/custom_models/vgg16_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/custom_models/vgg16bn_ecoset.py` & `thingsvision-2.6.2/thingsvision/custom_models/vgg16bn_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/thingsvision.py` & `thingsvision-2.6.2/thingsvision/thingsvision.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/utils/alignment/transforms.py` & `thingsvision-2.6.2/thingsvision/utils/alignment/transforms.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/utils/checkpointing/__init__.py` & `thingsvision-2.6.2/thingsvision/utils/checkpointing/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/utils/data/__init__.py` & `thingsvision-2.6.2/thingsvision/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/utils/data/data_loader.py` & `thingsvision-2.6.2/thingsvision/utils/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/utils/data/dataset.py` & `thingsvision-2.6.2/thingsvision/utils/data/dataset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/utils/data/helpers.py` & `thingsvision-2.6.2/thingsvision/utils/data/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/utils/imagenet/__init__.py` & `thingsvision-2.6.2/thingsvision/utils/imagenet/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/utils/models/dino/utils.py` & `thingsvision-2.6.2/thingsvision/utils/models/dino/utils.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/utils/models/dino/vision_transformer.py` & `thingsvision-2.6.2/thingsvision/utils/models/dino/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/utils/models/mae/utils.py` & `thingsvision-2.6.2/thingsvision/utils/models/mae/utils.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/utils/models/mae/vit_mae.py` & `thingsvision-2.6.2/thingsvision/utils/models/mae/vit_mae.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision/utils/storing/helpers.py` & `thingsvision-2.6.2/thingsvision/utils/storing/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.1/thingsvision.egg-info/PKG-INFO` & `thingsvision-2.6.2/thingsvision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thingsvision
-Version: 2.6.1
+Version: 2.6.2
 Summary: Extracting image features from state-of-the-art neural networks for Computer Vision made easy
 Home-page: https://github.com/ViCCo-Group/thingsvision
 Author: Lukas Muttenthaler
 Author-email: muttenthaler@cbs.mpg.de
 License: MIT License
 Keywords: feature extraction
 Classifier: Programming Language :: Python :: 3.8
@@ -72,16 +72,16 @@
 
 <!-- Functionality -->
 ### :mechanical_arm: Functionality
 With `thingsvision`, you can:
 - extract features for any imageset from many popular networks.
 - extract features for any imageset from your custom networks.
 - extract features for >26,000 images from the [THINGS image database](https://osf.io/jum2f/).
-- [align](https://vicco-group.github.io/thingsvision/Alignment.html) the extracted features with human object perception.
-- extract features from [HDF5 datasets](https://vicco-group.github.io/thingsvision/LoadingYourData.html#using-the-hdf5dataset-class) directly (e.g., NSD stimuli)
+- [align](https://vicco-group.github.io/thingsvision/Alignment.html) the extracted features with human object perception (e.g., using [gLocal](https://proceedings.neurips.cc/paper_files/paper/2023/hash/9febda1c8344cc5f2d51713964864e93-Abstract-Conference.html)).
+- extract features from [HDF5 datasets](https://vicco-group.github.io/thingsvision/LoadingYourData.html#using-the-hdf5dataset-class) directly (e.g., [NSD stimuli](https://naturalscenesdataset.org/))
 - conduct basic [Representational Similarity Analysis (RSA)](https://vicco-group.github.io/thingsvision/RSA.html#representational-similarity-analysis-rsa) after feature extraction.
 - perform efficient [Centered Kernel Alignment (CKA)](https://vicco-group.github.io/thingsvision/RSA.html#centered-kernel-alignment-cka) to compare image features across model-module combinations.
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- Model collection -->
 ### :file_cabinet: Model collection
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thingsvision Version: 2.6.1 Summary: Extracting
+Metadata-Version: 2.1 Name: thingsvision Version: 2.6.2 Summary: Extracting
 image features from state-of-the-art neural networks for Computer Vision made
 easy Home-page: https://github.com/ViCCo-Group/thingsvision Author: Lukas
 Muttenthaler Author-email: muttenthaler@cbs.mpg.de License: MIT License
 Keywords: feature extraction Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
@@ -30,22 +30,24 @@
 rotating_light:
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### :mechanical_arm: Functionality With `thingsvision`, you can: - extract
 features for any imageset from many popular networks. - extract features for
 any imageset from your custom networks. - extract features for >26,000 images
 from the [THINGS image database](https://osf.io/jum2f/). - [align](https://
 vicco-group.github.io/thingsvision/Alignment.html) the extracted features with
-human object perception. - extract features from [HDF5 datasets](https://vicco-
+human object perception (e.g., using [gLocal](https://proceedings.neurips.cc/
+paper_files/paper/2023/hash/9febda1c8344cc5f2d51713964864e93-Abstract-
+Conference.html)). - extract features from [HDF5 datasets](https://vicco-
 group.github.io/thingsvision/LoadingYourData.html#using-the-hdf5dataset-class)
-directly (e.g., NSD stimuli) - conduct basic [Representational Similarity
-Analysis (RSA)](https://vicco-group.github.io/thingsvision/
-RSA.html#representational-similarity-analysis-rsa) after feature extraction. -
-perform efficient [Centered Kernel Alignment (CKA)](https://vicco-
-group.github.io/thingsvision/RSA.html#centered-kernel-alignment-cka) to compare
-image features across model-module combinations.
+directly (e.g., [NSD stimuli](https://naturalscenesdataset.org/)) - conduct
+basic [Representational Similarity Analysis (RSA)](https://vicco-
+group.github.io/thingsvision/RSA.html#representational-similarity-analysis-rsa)
+after feature extraction. - perform efficient [Centered Kernel Alignment (CKA)]
+(https://vicco-group.github.io/thingsvision/RSA.html#centered-kernel-alignment-
+cka) to compare image features across model-module combinations.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### :file_cabinet: Model collection Neural networks come from different
 sources. With `thingsvision`, you can extract image representations of all
 models from: - [torchvision](https://pytorch.org/vision/0.8/models.html) -
 [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications) -
 [timm](https://github.com/rwightman/pytorch-image-models) - `ssl` (self-
 supervised learning models) - `simclr-rn50`, `mocov2-rn50`, `barlowtwins-rn50`,
```

### Comparing `thingsvision-2.6.1/thingsvision.egg-info/SOURCES.txt` & `thingsvision-2.6.2/thingsvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

