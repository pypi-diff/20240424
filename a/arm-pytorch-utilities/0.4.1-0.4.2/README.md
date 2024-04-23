# Comparing `tmp/arm_pytorch_utilities-0.4.1.tar.gz` & `tmp/arm_pytorch_utilities-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arm_pytorch_utilities-0.4.1.tar", last modified: Mon Apr 22 19:21:51 2024, max compression
+gzip compressed data, was "arm_pytorch_utilities-0.4.2.tar", last modified: Tue Apr 23 23:57:05 2024, max compression
```

## Comparing `arm_pytorch_utilities-0.4.1.tar` & `arm_pytorch_utilities-0.4.2.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2024-04-22 19:21:51.933676 arm_pytorch_utilities-0.4.1/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1075 2023-02-10 02:18:25.000000 arm_pytorch_utilities-0.4.1/LICENSE.txt
--rw-r--r--   0 zhsh      (1001) zhsh      (1001)     2572 2024-04-22 19:21:51.933676 arm_pytorch_utilities-0.4.1/PKG-INFO
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      350 2023-02-10 03:51:44.000000 arm_pytorch_utilities-0.4.1/README.md
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     4183 2024-04-22 19:21:26.000000 arm_pytorch_utilities-0.4.1/pyproject.toml
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       38 2024-04-22 19:21:51.933676 arm_pytorch_utilities-0.4.1/setup.cfg
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2024-04-22 19:21:51.925676 arm_pytorch_utilities-0.4.1/src/
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2024-04-22 19:21:51.929676 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      592 2023-12-15 18:45:30.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/__init__.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     2555 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/array_utils.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1189 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/controller.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     7163 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/draw.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     7835 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/gmm.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1305 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/grad.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     7388 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/linalg.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     8889 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/load_data.py
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2024-04-22 19:21:51.929676 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/make_data/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)        0 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/make_data/__init__.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     5070 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/make_data/datasource.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1766 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/make_data/make.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      231 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/make_data/params.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1800 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/make_data/select.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     2871 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/math_utils.py
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2024-04-22 19:21:51.933676 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/model/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)        0 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/model/__init__.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     4483 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/model/common.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1805 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/model/make.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     3085 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/model/mdn.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     4688 2023-08-31 21:12:37.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/optim.py
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2024-04-22 19:21:51.933676 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/policy/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)        0 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/policy/__init__.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     3219 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/policy/lin_gauss.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    12030 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/preprocess.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       40 2023-02-15 18:20:51.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/rand.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1530 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/serialization.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     3964 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/simulation.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     2724 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/softknn.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       94 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/str_utils.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     4760 2024-01-24 00:48:52.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/tensor_utils.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     7325 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/trajectory.py
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2024-04-22 19:21:51.933676 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities.egg-info/
--rw-r--r--   0 zhsh      (1001) zhsh      (1001)     2572 2024-04-22 19:21:51.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities.egg-info/PKG-INFO
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1609 2024-04-22 19:21:51.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities.egg-info/SOURCES.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)        1 2024-04-22 19:21:51.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities.egg-info/dependency_links.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       57 2024-04-22 19:21:51.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities.egg-info/requires.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       22 2024-04-22 19:21:51.000000 arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities.egg-info/top_level.txt
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2024-04-22 19:21:51.933676 arm_pytorch_utilities-0.4.1/tests/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      709 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/tests/test_draw.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1521 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/tests/test_grad.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1486 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/tests/test_linalg.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1526 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/tests/test_math.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     4406 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/tests/test_preprocessor.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     6174 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.1/tests/test_softknn.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1296 2023-12-15 18:58:06.000000 arm_pytorch_utilities-0.4.1/tests/test_tensor_utils.py
+drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2024-04-23 23:57:05.930514 arm_pytorch_utilities-0.4.2/
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1075 2023-02-10 02:18:25.000000 arm_pytorch_utilities-0.4.2/LICENSE.txt
+-rw-r--r--   0 zhsh      (1001) zhsh      (1001)     2572 2024-04-23 23:57:05.930514 arm_pytorch_utilities-0.4.2/PKG-INFO
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      350 2023-02-10 03:51:44.000000 arm_pytorch_utilities-0.4.2/README.md
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     4183 2024-04-23 23:56:42.000000 arm_pytorch_utilities-0.4.2/pyproject.toml
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       38 2024-04-23 23:57:05.930514 arm_pytorch_utilities-0.4.2/setup.cfg
+drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2024-04-23 23:57:05.926514 arm_pytorch_utilities-0.4.2/src/
+drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2024-04-23 23:57:05.930514 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      592 2023-12-15 18:45:30.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/__init__.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     2555 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/array_utils.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      830 2024-04-23 23:02:27.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/cache.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1189 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/controller.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     7163 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/draw.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     7835 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/gmm.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1305 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/grad.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     7388 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/linalg.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     8889 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/load_data.py
+drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2024-04-23 23:57:05.930514 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/make_data/
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)        0 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/make_data/__init__.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     5070 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/make_data/datasource.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1766 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/make_data/make.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      231 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/make_data/params.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1800 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/make_data/select.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     2871 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/math_utils.py
+drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2024-04-23 23:57:05.930514 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/model/
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)        0 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/model/__init__.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     4483 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/model/common.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1805 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/model/make.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     3085 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/model/mdn.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     4688 2023-08-31 21:12:37.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/optim.py
+drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2024-04-23 23:57:05.930514 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/policy/
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)        0 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/policy/__init__.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     3219 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/policy/lin_gauss.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    12030 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/preprocess.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       40 2023-02-15 18:20:51.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/rand.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1530 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/serialization.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     3964 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/simulation.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     2724 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/softknn.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       94 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/str_utils.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     4760 2024-01-24 00:48:52.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/tensor_utils.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     7325 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/trajectory.py
+drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2024-04-23 23:57:05.930514 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities.egg-info/
+-rw-r--r--   0 zhsh      (1001) zhsh      (1001)     2572 2024-04-23 23:57:05.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities.egg-info/PKG-INFO
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1644 2024-04-23 23:57:05.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)        1 2024-04-23 23:57:05.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       57 2024-04-23 23:57:05.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities.egg-info/requires.txt
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       22 2024-04-23 23:57:05.000000 arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities.egg-info/top_level.txt
+drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2024-04-23 23:57:05.930514 arm_pytorch_utilities-0.4.2/tests/
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      709 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/tests/test_draw.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1521 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/tests/test_grad.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1486 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/tests/test_linalg.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1526 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/tests/test_math.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     4406 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/tests/test_preprocessor.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     6174 2022-07-12 20:10:40.000000 arm_pytorch_utilities-0.4.2/tests/test_softknn.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1296 2023-12-15 18:58:06.000000 arm_pytorch_utilities-0.4.2/tests/test_tensor_utils.py
```

### Comparing `arm_pytorch_utilities-0.4.1/LICENSE.txt` & `arm_pytorch_utilities-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/PKG-INFO` & `arm_pytorch_utilities-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arm_pytorch_utilities
-Version: 0.4.1
+Version: 0.4.2
 Summary: Utilities for working with pytorch
 Author-email: Sheng Zhong <zhsh@umich.edu>
 Maintainer-email: Sheng Zhong <zhsh@umich.edu>
 License: Copyright (c) 2023 University of Michigan ARM Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `arm_pytorch_utilities-0.4.1/pyproject.toml` & `arm_pytorch_utilities-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arm_pytorch_utilities"
-version = "0.4.1"
+version = "0.4.2"
 description = "Utilities for working with pytorch"
 readme = "README.md" # Optional
 
 # Specify which Python versions you support. In contrast to the
 # 'Programming Language' classifiers above, 'pip install' will check this
 # and refuse to install the project if the version does not match. See
 # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
```

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/__init__.py` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/array_utils.py` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/array_utils.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/controller.py` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/controller.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/draw.py` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/draw.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/gmm.py` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/gmm.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/grad.py` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/grad.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/linalg.py` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/linalg.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/load_data.py` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/load_data.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/make_data/datasource.py` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/make_data/datasource.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/make_data/make.py` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/make_data/make.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/make_data/select.py` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/make_data/select.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/math_utils.py` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/math_utils.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/model/common.py` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/model/common.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/model/make.py` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/model/make.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/model/mdn.py` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/model/mdn.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/optim.py` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/optim.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/policy/lin_gauss.py` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/policy/lin_gauss.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/preprocess.py` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/preprocess.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/serialization.py` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/serialization.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/simulation.py` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/simulation.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/softknn.py` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/softknn.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/tensor_utils.py` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities/trajectory.py` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities/trajectory.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities.egg-info/PKG-INFO` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arm_pytorch_utilities
-Version: 0.4.1
+Version: 0.4.2
 Summary: Utilities for working with pytorch
 Author-email: Sheng Zhong <zhsh@umich.edu>
 Maintainer-email: Sheng Zhong <zhsh@umich.edu>
 License: Copyright (c) 2023 University of Michigan ARM Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `arm_pytorch_utilities-0.4.1/src/arm_pytorch_utilities.egg-info/SOURCES.txt` & `arm_pytorch_utilities-0.4.2/src/arm_pytorch_utilities.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE.txt
 README.md
 pyproject.toml
 src/arm_pytorch_utilities/__init__.py
 src/arm_pytorch_utilities/array_utils.py
+src/arm_pytorch_utilities/cache.py
 src/arm_pytorch_utilities/controller.py
 src/arm_pytorch_utilities/draw.py
 src/arm_pytorch_utilities/gmm.py
 src/arm_pytorch_utilities/grad.py
 src/arm_pytorch_utilities/linalg.py
 src/arm_pytorch_utilities/load_data.py
 src/arm_pytorch_utilities/math_utils.py
```

### Comparing `arm_pytorch_utilities-0.4.1/tests/test_draw.py` & `arm_pytorch_utilities-0.4.2/tests/test_draw.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/tests/test_grad.py` & `arm_pytorch_utilities-0.4.2/tests/test_grad.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/tests/test_linalg.py` & `arm_pytorch_utilities-0.4.2/tests/test_linalg.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/tests/test_math.py` & `arm_pytorch_utilities-0.4.2/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/tests/test_preprocessor.py` & `arm_pytorch_utilities-0.4.2/tests/test_preprocessor.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/tests/test_softknn.py` & `arm_pytorch_utilities-0.4.2/tests/test_softknn.py`

 * *Files identical despite different names*

### Comparing `arm_pytorch_utilities-0.4.1/tests/test_tensor_utils.py` & `arm_pytorch_utilities-0.4.2/tests/test_tensor_utils.py`

 * *Files identical despite different names*

