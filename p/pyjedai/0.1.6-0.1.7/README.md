# Comparing `tmp/pyjedai-0.1.6.tar.gz` & `tmp/pyjedai-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjedai-0.1.6.tar", last modified: Fri Mar 15 10:47:32 2024, max compression
+gzip compressed data, was "pyjedai-0.1.7.tar", last modified: Wed Apr 24 07:59:28 2024, max compression
```

## Comparing `pyjedai-0.1.6.tar` & `pyjedai-0.1.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 10:47:32.102020 pyjedai-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-03-15 10:47:21.000000 pyjedai-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10555 2024-03-15 10:47:32.102020 pyjedai-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-03-15 10:47:21.000000 pyjedai-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-03-15 10:47:21.000000 pyjedai-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 10:47:32.102020 pyjedai-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 10:47:32.094020 pyjedai-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 10:47:32.098020 pyjedai-0.1.6/src/pyjedai/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-15 10:47:21.000000 pyjedai-0.1.6/src/pyjedai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-15 10:47:21.000000 pyjedai-0.1.6/src/pyjedai/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    27254 2024-03-15 10:47:21.000000 pyjedai-0.1.6/src/pyjedai/block_building.py
--rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-03-15 10:47:21.000000 pyjedai-0.1.6/src/pyjedai/block_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)    68182 2024-03-15 10:47:21.000000 pyjedai-0.1.6/src/pyjedai/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)    50407 2024-03-15 10:47:21.000000 pyjedai-0.1.6/src/pyjedai/comparison_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)    19457 2024-03-15 10:47:21.000000 pyjedai-0.1.6/src/pyjedai/datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    19286 2024-03-15 10:47:21.000000 pyjedai-0.1.6/src/pyjedai/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    23514 2024-03-15 10:47:21.000000 pyjedai-0.1.6/src/pyjedai/joins.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-15 10:47:21.000000 pyjedai-0.1.6/src/pyjedai/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    26464 2024-03-15 10:47:21.000000 pyjedai-0.1.6/src/pyjedai/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)    68656 2024-03-15 10:47:21.000000 pyjedai-0.1.6/src/pyjedai/prioritization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 10:47:32.102020 pyjedai-0.1.6/src/pyjedai/schema/
--rw-r--r--   0 runner    (1001) docker     (127)    27821 2024-03-15 10:47:21.000000 pyjedai-0.1.6/src/pyjedai/schema/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-03-15 10:47:21.000000 pyjedai-0.1.6/src/pyjedai/schema/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 10:47:32.102020 pyjedai-0.1.6/src/pyjedai/spatial/
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-03-15 10:47:21.000000 pyjedai-0.1.6/src/pyjedai/spatial/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-03-15 10:47:21.000000 pyjedai-0.1.6/src/pyjedai/spatial/initialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    11247 2024-03-15 10:47:21.000000 pyjedai-0.1.6/src/pyjedai/spatial/verification.py
--rw-r--r--   0 runner    (1001) docker     (127)    52783 2024-03-15 10:47:21.000000 pyjedai-0.1.6/src/pyjedai/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    28949 2024-03-15 10:47:21.000000 pyjedai-0.1.6/src/pyjedai/vector_based_blocking.py
--rw-r--r--   0 runner    (1001) docker     (127)    31421 2024-03-15 10:47:21.000000 pyjedai-0.1.6/src/pyjedai/visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)    46747 2024-03-15 10:47:21.000000 pyjedai-0.1.6/src/pyjedai/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 10:47:32.102020 pyjedai-0.1.6/src/pyjedai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10555 2024-03-15 10:47:32.000000 pyjedai-0.1.6/src/pyjedai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-15 10:47:32.000000 pyjedai-0.1.6/src/pyjedai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 10:47:32.000000 pyjedai-0.1.6/src/pyjedai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-15 10:47:32.000000 pyjedai-0.1.6/src/pyjedai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-15 10:47:32.000000 pyjedai-0.1.6/src/pyjedai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 10:47:32.102020 pyjedai-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-03-15 10:47:21.000000 pyjedai-0.1.6/tests/test_block_building.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-03-15 10:47:21.000000 pyjedai-0.1.6/tests/test_block_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-03-15 10:47:21.000000 pyjedai-0.1.6/tests/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-03-15 10:47:21.000000 pyjedai-0.1.6/tests/test_comparison_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 10:47:21.000000 pyjedai-0.1.6/tests/test_joins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:59:28.929417 pyjedai-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-04-24 07:59:17.000000 pyjedai-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10547 2024-04-24 07:59:28.929417 pyjedai-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8343 2024-04-24 07:59:17.000000 pyjedai-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-24 07:59:17.000000 pyjedai-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 07:59:28.933418 pyjedai-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:59:28.921418 pyjedai-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:59:28.929417 pyjedai-0.1.7/src/pyjedai/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-24 07:59:17.000000 pyjedai-0.1.7/src/pyjedai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 07:59:17.000000 pyjedai-0.1.7/src/pyjedai/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27254 2024-04-24 07:59:17.000000 pyjedai-0.1.7/src/pyjedai/block_building.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8396 2024-04-24 07:59:17.000000 pyjedai-0.1.7/src/pyjedai/block_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69347 2024-04-24 07:59:17.000000 pyjedai-0.1.7/src/pyjedai/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50407 2024-04-24 07:59:17.000000 pyjedai-0.1.7/src/pyjedai/comparison_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19975 2024-04-24 07:59:17.000000 pyjedai-0.1.7/src/pyjedai/datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19285 2024-04-24 07:59:17.000000 pyjedai-0.1.7/src/pyjedai/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23514 2024-04-24 07:59:17.000000 pyjedai-0.1.7/src/pyjedai/joins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-24 07:59:17.000000 pyjedai-0.1.7/src/pyjedai/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26446 2024-04-24 07:59:17.000000 pyjedai-0.1.7/src/pyjedai/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68656 2024-04-24 07:59:17.000000 pyjedai-0.1.7/src/pyjedai/prioritization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:59:28.929417 pyjedai-0.1.7/src/pyjedai/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)    27821 2024-04-24 07:59:17.000000 pyjedai-0.1.7/src/pyjedai/schema/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-24 07:59:17.000000 pyjedai-0.1.7/src/pyjedai/schema/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:59:28.929417 pyjedai-0.1.7/src/pyjedai/spatial/
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-24 07:59:17.000000 pyjedai-0.1.7/src/pyjedai/spatial/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-24 07:59:17.000000 pyjedai-0.1.7/src/pyjedai/spatial/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11247 2024-04-24 07:59:17.000000 pyjedai-0.1.7/src/pyjedai/spatial/verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52783 2024-04-24 07:59:17.000000 pyjedai-0.1.7/src/pyjedai/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24151 2024-04-24 07:59:17.000000 pyjedai-0.1.7/src/pyjedai/vector_based_blocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31421 2024-04-24 07:59:17.000000 pyjedai-0.1.7/src/pyjedai/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42942 2024-04-24 07:59:17.000000 pyjedai-0.1.7/src/pyjedai/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:59:28.929417 pyjedai-0.1.7/src/pyjedai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10547 2024-04-24 07:59:28.000000 pyjedai-0.1.7/src/pyjedai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-24 07:59:28.000000 pyjedai-0.1.7/src/pyjedai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 07:59:28.000000 pyjedai-0.1.7/src/pyjedai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-24 07:59:28.000000 pyjedai-0.1.7/src/pyjedai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 07:59:28.000000 pyjedai-0.1.7/src/pyjedai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:59:28.929417 pyjedai-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-24 07:59:17.000000 pyjedai-0.1.7/tests/test_block_building.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-24 07:59:17.000000 pyjedai-0.1.7/tests/test_block_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-24 07:59:17.000000 pyjedai-0.1.7/tests/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-24 07:59:17.000000 pyjedai-0.1.7/tests/test_comparison_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:59:17.000000 pyjedai-0.1.7/tests/test_joins.py
```

### Comparing `pyjedai-0.1.6/LICENSE` & `pyjedai-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjedai-0.1.6/PKG-INFO` & `pyjedai-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 6a65  : 2.1.Name: pyje
 00000020: 6461 690a 5665 7273 696f 6e3a 2030 2e31  dai.Version: 0.1
-00000030: 2e36 0a53 756d 6d61 7279 3a20 416e 206f  .6.Summary: An o
+00000030: 2e37 0a53 756d 6d61 7279 3a20 416e 206f  .7.Summary: An o
 00000040: 7065 6e2d 736f 7572 6365 206c 6962 7261  pen-source libra
 00000050: 7279 2074 6861 7420 6275 696c 6473 2070  ry that builds p
 00000060: 6f77 6572 6675 6c20 656e 642d 746f 2d65  owerful end-to-e
 00000070: 6e64 2045 6e74 6974 7920 5265 736f 6c75  nd Entity Resolu
 00000080: 7469 6f6e 2077 6f72 6b66 6c6f 7773 2e0a  tion workflows..
 00000090: 4175 7468 6f72 2d65 6d61 696c 3a20 4b6f  Author-email: Ko
 000000a0: 6e73 7461 6e74 696e 6f73 204e 696b 6f6c  nstantinos Nikol
@@ -100,561 +100,561 @@
 00000630: 4d6f 6475 6c65 730a 5265 7175 6972 6573  Modules.Requires
 00000640: 2d50 7974 686f 6e3a 203e 3d33 2e38 0a44  -Python: >=3.8.D
 00000650: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
 00000660: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
 00000670: 726b 646f 776e 0a4c 6963 656e 7365 2d46  rkdown.License-F
 00000680: 696c 653a 204c 4943 454e 5345 0a52 6571  ile: LICENSE.Req
 00000690: 7569 7265 732d 4469 7374 3a20 6765 6e73  uires-Dist: gens
-000006a0: 696d 3e3d 342e 322e 300a 5265 7175 6972  im>=4.2.0.Requir
-000006b0: 6573 2d44 6973 743a 206d 6174 706c 6f74  es-Dist: matplot
-000006c0: 6c69 623e 3d33 2e31 2e33 0a52 6571 7569  lib>=3.1.3.Requi
-000006d0: 7265 732d 4469 7374 3a20 6d61 7470 6c6f  res-Dist: matplo
-000006e0: 746c 6962 2d69 6e6c 696e 653e 3d30 2e31  tlib-inline>=0.1
-000006f0: 2e33 0a52 6571 7569 7265 732d 4469 7374  .3.Requires-Dist
-00000700: 3a20 6e65 7477 6f72 6b78 3e3d 322e 330a  : networkx>=2.3.
-00000710: 5265 7175 6972 6573 2d44 6973 743a 206e  Requires-Dist: n
-00000720: 6c74 6b3e 3d33 2e37 0a52 6571 7569 7265  ltk>=3.7.Require
-00000730: 732d 4469 7374 3a20 6e75 6d70 793e 3d31  s-Dist: numpy>=1
-00000740: 2e32 310a 5265 7175 6972 6573 2d44 6973  .21.Requires-Dis
-00000750: 743a 2070 616e 6461 733e 3d30 2e32 352e  t: pandas>=0.25.
-00000760: 330a 5265 7175 6972 6573 2d44 6973 743a  3.Requires-Dist:
-00000770: 2070 616e 6461 732d 7072 6f66 696c 696e   pandas-profilin
-00000780: 673e 3d33 2e32 0a52 6571 7569 7265 732d  g>=3.2.Requires-
-00000790: 4469 7374 3a20 7061 6e64 6f63 6669 6c74  Dist: pandocfilt
-000007a0: 6572 733e 3d31 2e35 0a52 6571 7569 7265  ers>=1.5.Require
-000007b0: 732d 4469 7374 3a20 5079 5941 4d4c 3e3d  s-Dist: PyYAML>=
-000007c0: 362e 300a 5265 7175 6972 6573 2d44 6973  6.0.Requires-Dis
-000007d0: 743a 2072 6466 6c69 623e 3d36 2e31 2e31  t: rdflib>=6.1.1
-000007e0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000007f0: 7264 6670 616e 6461 733e 3d31 2e31 2e35  rdfpandas>=1.1.5
-00000800: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000810: 7265 6765 783e 3d32 3032 322e 362e 320a  regex>=2022.6.2.
-00000820: 5265 7175 6972 6573 2d44 6973 743a 2073  Requires-Dist: s
-00000830: 6369 7079 3e3d 312e 370a 5265 7175 6972  cipy>=1.7.Requir
-00000840: 6573 2d44 6973 743a 2073 6561 626f 726e  es-Dist: seaborn
-00000850: 3e3d 302e 3131 0a52 6571 7569 7265 732d  >=0.11.Requires-
-00000860: 4469 7374 3a20 7374 7273 696d 3e3d 302e  Dist: strsim>=0.
-00000870: 302e 330a 5265 7175 6972 6573 2d44 6973  0.3.Requires-Dis
-00000880: 743a 2073 7472 7369 6d70 793e 3d30 2e32  t: strsimpy>=0.2
-00000890: 2e31 0a52 6571 7569 7265 732d 4469 7374  .1.Requires-Dist
-000008a0: 3a20 7471 646d 3e3d 342e 3634 0a52 6571  : tqdm>=4.64.Req
-000008b0: 7569 7265 732d 4469 7374 3a20 7472 616e  uires-Dist: tran
-000008c0: 7366 6f72 6d65 7273 3e3d 342e 3231 0a52  sformers>=4.21.R
-000008d0: 6571 7569 7265 732d 4469 7374 3a20 7365  equires-Dist: se
-000008e0: 6e74 656e 6365 2d74 7261 6e73 666f 726d  ntence-transform
-000008f0: 6572 733e 3d32 2e32 0a52 6571 7569 7265  ers>=2.2.Require
-00000900: 732d 4469 7374 3a20 6661 6973 732d 6370  s-Dist: faiss-cp
-00000910: 753e 3d31 2e37 0a52 6571 7569 7265 732d  u>=1.7.Requires-
-00000920: 4469 7374 3a20 6f70 7475 6e61 3e3d 332e  Dist: optuna>=3.
-00000930: 300a 5265 7175 6972 6573 2d44 6973 743a  0.Requires-Dist:
-00000940: 2074 6f6d 6c69 3b20 7079 7468 6f6e 5f76   tomli; python_v
-00000950: 6572 7369 6f6e 203c 2022 332e 3131 220a  ersion < "3.11".
-00000960: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
-00000970: 792d 7374 7269 6e67 6d61 7463 6869 6e67  y-stringmatching
-00000980: 3e3d 302e 340a 5265 7175 6972 6573 2d44  >=0.4.Requires-D
-00000990: 6973 743a 2076 616c 656e 7469 6e65 3e3d  ist: valentine>=
-000009a0: 302e 313b 2070 7974 686f 6e5f 7665 7273  0.1; python_vers
-000009b0: 696f 6e20 3e20 2233 2e37 220a 5265 7175  ion > "3.7".Requ
-000009c0: 6972 6573 2d44 6973 743a 206f 7264 6572  ires-Dist: order
-000009d0: 6564 2d73 6574 3e3d 342e 300a 5265 7175  ed-set>=4.0.Requ
-000009e0: 6972 6573 2d44 6973 743a 2070 6c6f 746c  ires-Dist: plotl
-000009f0: 793e 3d35 2e31 362e 300a 5265 7175 6972  y>=5.16.0.Requir
-00000a00: 6573 2d44 6973 743a 2073 6861 7065 6c79  es-Dist: shapely
-00000a10: 3e3d 322e 300a 5265 7175 6972 6573 2d44  >=2.0.Requires-D
-00000a20: 6973 743a 2073 6361 6e6e 3b20 706c 6174  ist: scann; plat
-00000a30: 666f 726d 5f73 7973 7465 6d20 3d3d 2022  form_system == "
-00000a40: 4c69 6e75 7822 0a52 6571 7569 7265 732d  Linux".Requires-
-00000a50: 4469 7374 3a20 6661 6c63 6f6e 6e3b 2070  Dist: falconn; p
-00000a60: 6c61 7466 6f72 6d5f 7379 7374 656d 203d  latform_system =
-00000a70: 3d20 224c 696e 7578 220a 5072 6f76 6964  = "Linux".Provid
-00000a80: 6573 2d45 7874 7261 3a20 6465 760a 5265  es-Extra: dev.Re
-00000a90: 7175 6972 6573 2d44 6973 743a 2070 6970  quires-Dist: pip
-00000aa0: 2d74 6f6f 6c73 3b20 6578 7472 6120 3d3d  -tools; extra ==
-00000ab0: 2022 6465 7622 0a52 6571 7569 7265 732d   "dev".Requires-
-00000ac0: 4469 7374 3a20 7079 7465 7374 3b20 6578  Dist: pytest; ex
-00000ad0: 7472 6120 3d3d 2022 6465 7622 0a0a 3c64  tra == "dev"..<d
-00000ae0: 6976 2061 6c69 676e 3d22 6365 6e74 6572  iv align="center
-00000af0: 223e 0a20 2020 203c 6272 3e0a 2020 2020  ">.    <br>.    
-00000b00: 3c69 6d67 2061 6c69 676e 3d22 6365 6e74  <img align="cent
-00000b10: 6572 2220 7372 633d 2268 7474 7073 3a2f  er" src="https:/
-00000b20: 2f67 6974 6875 622e 636f 6d2f 4149 2d74  /github.com/AI-t
-00000b30: 6561 6d2d 556f 412f 7079 4a65 6441 492f  eam-UoA/pyJedAI/
-00000b40: 626c 6f62 2f6d 6169 6e2f 646f 6373 2f69  blob/main/docs/i
-00000b50: 6d67 2f70 796a 6564 6169 2e6c 6f67 6f2e  mg/pyjedai.logo.
-00000b60: 6472 6177 696f 2e70 6e67 3f72 6177 3d74  drawio.png?raw=t
-00000b70: 7275 6522 2061 6c74 3d22 7079 4a65 6441  rue" alt="pyJedA
-00000b80: 4922 2077 6964 7468 3d22 3430 3022 2f3e  I" width="400"/>
-00000b90: 0a3c 2f64 6976 3e0a 3c62 723e 0a3c 6272  .</div>.<br>.<br
-00000ba0: 3e0a 3c64 6976 2061 6c69 676e 3d22 6365  >.<div align="ce
-00000bb0: 6e74 6572 223e 0a41 6e20 6f70 656e 2d73  nter">.An open-s
-00000bc0: 6f75 7263 6520 6c69 6272 6172 7920 7468  ource library th
-00000bd0: 6174 206c 6576 6572 6167 6573 2050 7974  at leverages Pyt
-00000be0: 686f 6ee2 8099 7320 6461 7461 2073 6369  hon...s data sci
-00000bf0: 656e 6365 2065 636f 7379 7374 656d 2074  ence ecosystem t
-00000c00: 6f20 6275 696c 6420 3c62 723e 2070 6f77  o build <br> pow
-00000c10: 6572 6675 6c20 656e 642d 746f 2d65 6e64  erful end-to-end
-00000c20: 2045 6e74 6974 7920 5265 736f 6c75 7469   Entity Resoluti
-00000c30: 6f6e 2077 6f72 6b66 6c6f 7773 2e0a 3c2f  on workflows..</
-00000c40: 6469 763e 0a0a 0a2d 2d2d 0a0a 0a23 204f  div>...---...# O
-00000c50: 7665 7276 6965 770a 0a70 794a 6564 4149  verview..pyJedAI
-00000c60: 2069 7320 6120 7079 7468 6f6e 2066 7261   is a python fra
-00000c70: 6d65 776f 726b 2c20 6169 6d69 6e67 2074  mework, aiming t
-00000c80: 6f20 6f66 6665 7220 6578 7065 7274 7320  o offer experts 
-00000c90: 616e 6420 6e6f 7669 6365 2075 7365 7273  and novice users
-00000ca0: 2c20 726f 6275 7374 2061 6e64 2066 6173  , robust and fas
-00000cb0: 7420 736f 6c75 7469 6f6e 7320 666f 7220  t solutions for 
-00000cc0: 6d75 6c74 6970 6c65 2074 7970 6573 206f  multiple types o
-00000cd0: 6620 456e 7469 7479 2052 6573 6f6c 7574  f Entity Resolut
-00000ce0: 696f 6e20 7072 6f62 6c65 6d73 2e20 4974  ion problems. It
-00000cf0: 2069 7320 6275 696c 6465 6420 7573 696e   is builded usin
-00000d00: 6720 7374 6174 652d 6f66 2d74 6865 2d61  g state-of-the-a
-00000d10: 7274 2070 7974 686f 6e20 6672 616d 6577  rt python framew
-00000d20: 6f72 6b73 2e20 7079 4a65 6441 4920 636f  orks. pyJedAI co
-00000d30: 6e73 7469 7475 7465 7320 7468 6520 736f  nstitutes the so
-00000d40: 6c65 206f 7065 6e2d 736f 7572 6365 204c  le open-source L
-00000d50: 696e 6b20 4469 7363 6f76 6572 7920 746f  ink Discovery to
-00000d60: 6f6c 2074 6861 7420 6973 2063 6170 6162  ol that is capab
-00000d70: 6c65 206f 6620 6578 706c 6f69 7469 6e67  le of exploiting
-00000d80: 2074 6865 206c 6174 6573 7420 6272 6561   the latest brea
-00000d90: 6b74 6872 6f75 6768 7320 696e 2044 6565  kthroughs in Dee
-00000da0: 7020 4c65 6172 6e69 6e67 2061 6e64 204e  p Learning and N
-00000db0: 4c50 2074 6563 686e 6971 7565 732c 2077  LP techniques, w
-00000dc0: 6869 6368 2061 7265 2070 7562 6c69 636c  hich are publicl
-00000dd0: 7920 6176 6169 6c61 626c 6520 7468 726f  y available thro
-00000de0: 7567 6820 7468 6520 5079 7468 6f6e 2064  ugh the Python d
-00000df0: 6174 6120 7363 6965 6e63 6520 6563 6f73  ata science ecos
-00000e00: 7973 7465 6d2e 2054 6869 7320 6170 706c  ystem. This appl
-00000e10: 6965 7320 746f 2062 6f74 6820 626c 6f63  ies to both bloc
-00000e20: 6b69 6e67 2061 6e64 206d 6174 6368 696e  king and matchin
-00000e30: 672c 2074 6875 7320 656e 7375 7269 6e67  g, thus ensuring
-00000e40: 2068 6967 6820 7469 6d65 2065 6666 6963   high time effic
-00000e50: 6965 6e63 792c 2068 6967 6820 7363 616c  iency, high scal
-00000e60: 6162 696c 6974 7920 6173 2077 656c 6c20  ability as well 
-00000e70: 6173 2068 6967 6820 6566 6665 6374 6976  as high effectiv
-00000e80: 656e 6573 732c 2077 6974 686f 7574 2072  eness, without r
-00000e90: 6571 7569 7269 6e67 2061 6e79 206c 6162  equiring any lab
-00000ea0: 656c 6c65 6420 696e 7374 616e 6365 7320  elled instances 
-00000eb0: 6672 6f6d 2074 6865 2075 7365 722e 0a0a  from the user...
-00000ec0: 2323 2320 4b65 792d 4665 6174 7572 6573  ### Key-Features
-00000ed0: 0a0a 2d20 496e 7075 7420 6461 7461 2d74  ..- Input data-t
-00000ee0: 7970 6520 696e 6465 7065 6e64 656e 742e  ype independent.
-00000ef0: 2042 6f74 6820 7374 7275 6374 7572 6564   Both structured
-00000f00: 2061 6e64 2073 656d 692d 7374 7275 6374   and semi-struct
-00000f10: 7572 6564 2064 6174 6120 6361 6e20 6265  ured data can be
-00000f20: 2070 726f 6365 7373 6564 2e0a 2d20 5661   processed..- Va
-00000f30: 7269 6f75 7320 696d 706c 656d 656e 7465  rious implemente
-00000f40: 6420 616c 676f 7269 7468 6d73 2e0a 2d20  d algorithms..- 
-00000f50: 4561 7379 2d74 6f2d 7573 652e 0a2d 2055  Easy-to-use..- U
-00000f60: 7469 6c69 7a65 7320 736f 6d65 206f 6620  tilizes some of 
-00000f70: 7468 6520 6661 6d6f 7573 2061 6e64 2063  the famous and c
-00000f80: 7574 7469 6e67 2d65 6467 6520 6d61 6368  utting-edge mach
-00000f90: 696e 6520 6c65 6172 6e69 6e67 2070 6163  ine learning pac
-00000fa0: 6b61 6765 732e 0a2d 204f 6666 6572 7320  kages..- Offers 
-00000fb0: 7375 7065 7276 6973 6564 2061 6e64 2075  supervised and u
-00000fc0: 6e2d 7375 7065 7276 6973 6564 204d 4c20  n-supervised ML 
-00000fd0: 7465 6368 6e69 7175 6573 2e0a 0a5f 5f4f  techniques...__O
-00000fe0: 7065 6e20 6465 6d6f 7320 6172 6520 6176  pen demos are av
-00000ff0: 6169 6c61 626c 6520 696e 3a5f 5f0a 0a3c  ailable in:__..<
-00001000: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
-00001010: 7222 3e0a 2020 2020 3c61 2068 7265 663d  r">.    <a href=
-00001020: 2268 7474 7073 3a2f 2f6e 6276 6965 7765  "https://nbviewe
-00001030: 722e 6f72 672f 6769 7468 7562 2f41 492d  r.org/github/AI-
-00001040: 7465 616d 2d55 6f41 2f70 794a 6564 4149  team-UoA/pyJedAI
-00001050: 2f62 6c6f 622f 6d61 696e 2f64 6f63 732f  /blob/main/docs/
-00001060: 7475 746f 7269 616c 732f 4465 6d6f 2e69  tutorials/Demo.i
-00001070: 7079 6e62 223e 0a20 2020 2020 2020 203c  pynb">.        <
-00001080: 696d 6720 616c 6967 6e3d 2263 656e 7465  img align="cente
-00001090: 7222 2073 7263 3d22 6874 7470 733a 2f2f  r" src="https://
-000010a0: 6e62 7669 6577 6572 2e6f 7267 2f73 7461  nbviewer.org/sta
-000010b0: 7469 632f 696d 672f 6e61 765f 6c6f 676f  tic/img/nav_logo
-000010c0: 2e73 7667 2220 7769 6474 683d 3132 302f  .svg" width=120/
-000010d0: 3e20 0a20 2020 203c 2f61 3e20 2026 6e62  > .    </a>  &nb
-000010e0: 7370 3b26 6e62 7370 3b26 6e62 7370 3b26  sp;&nbsp;&nbsp;&
-000010f0: 6e62 7370 3b26 6e62 7370 3b26 6e62 7370  nbsp;&nbsp;&nbsp
-00001100: 3b26 6e62 7370 3b0a 2020 2020 3c61 2068  ;&nbsp;.    <a h
-00001110: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00001120: 6875 622e 636f 6d2f 4149 2d74 6561 6d2d  hub.com/AI-team-
-00001130: 556f 412f 7079 4a65 6441 492f 626c 6f62  UoA/pyJedAI/blob
-00001140: 2f6d 6169 6e2f 646f 6373 2f74 7574 6f72  /main/docs/tutor
-00001150: 6961 6c73 2f44 656d 6f2e 6970 796e 6222  ials/Demo.ipynb"
-00001160: 3e0a 2020 2020 2020 2020 3c69 6d67 2061  >.        <img a
-00001170: 6c69 676e 3d22 6365 6e74 6572 2220 7372  lign="center" sr
-00001180: 633d 2268 7474 7073 3a2f 2f6d 6972 6f2e  c="https://miro.
-00001190: 6d65 6469 756d 2e63 6f6d 2f6d 6178 2f31  medium.com/max/1
-000011a0: 3430 302f 312a 4564 6e5f 4c70 6253 704c  400/1*Edn_LpbSpL
-000011b0: 654e 4b66 576b 4564 4732 4a67 2e70 6e67  eNKfWkEdG2Jg.png
-000011c0: 2220 7769 6474 683d 3132 302f 3e20 0a20  " width=120/> . 
-000011d0: 2020 203c 2f61 3e0a 3c2f 6469 763e 0a0a     </a>.</div>..
-000011e0: 5f5f 476f 6f67 6c65 2043 6f6c 6162 2048  __Google Colab H
-000011f0: 616e 6473 2d6f 6e20 6465 6d6f 3a5f 5f20  ands-on demo:__ 
-00001200: 0a0a 3c64 6976 2061 6c69 676e 3d22 6365  ..<div align="ce
-00001210: 6e74 6572 223e 0a20 2020 203c 6120 6872  nter">.    <a hr
-00001220: 6566 3d22 6874 7470 733a 2f2f 636f 6c61  ef="https://cola
-00001230: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
-00001240: 652e 636f 6d2f 6472 6976 652f 3138 5667  e.com/drive/18Vg
-00001250: 454f 4b41 6332 4f62 4646 7844 4e62 3273  EOKAc2ObFFxDNb2s
-00001260: 6a68 424c 4b4b 734e 7666 4550 6f3f 7573  jhBLKKsNvfEPo?us
-00001270: 703d 7368 6172 696e 6722 3e0a 2020 2020  p=sharing">.    
-00001280: 2020 2020 3c69 6d67 2061 6c69 676e 3d22      <img align="
-00001290: 6365 6e74 6572 2220 7372 633d 2268 7474  center" src="htt
-000012a0: 7073 3a2f 2f33 2e62 702e 626c 6f67 7370  ps://3.bp.blogsp
-000012b0: 6f74 2e63 6f6d 2f2d 6170 6f42 6557 4679  ot.com/-apoBeWFy
-000012c0: 634b 512f 5868 4b42 3866 4570 7277 492f  cKQ/XhKB8fEprwI/
-000012d0: 4141 4141 4141 4141 434d 342f 536c 3736  AAAAAAAACM4/Sl76
-000012e0: 797a 4e53 4e59 776c 5368 4942 7268 6544  yzNSNYwlShIBrheD
-000012f0: 4175 6d38 4c39 7152 7457 4e64 6743 4c63  Aum8L9qRtWNdgCLc
-00001300: 4247 4173 5948 512f 7331 3630 302f 636f  BGAsYHQ/s1600/co
-00001310: 6c61 622e 706e 6722 2077 6964 7468 3d31  lab.png" width=1
-00001320: 3230 2f3e 200a 2020 2020 3c2f 613e 0a3c  20/> .    </a>.<
-00001330: 2f64 6976 3e0a 0a23 2049 6e73 7461 6c6c  /div>..# Install
-00001340: 0a0a 2323 2320 5079 5049 0a49 6e73 7461  ..### PyPI.Insta
-00001350: 6c6c 2074 6865 206c 6174 6573 7420 7665  ll the latest ve
-00001360: 7273 696f 6e20 6f66 2070 796a 6564 6169  rsion of pyjedai
-00001370: 205f 5f5b 7265 7175 6972 6573 2070 7974   __[requires pyt
-00001380: 686f 6e20 3e3d 2033 2e38 5d5f 5f3a 0a60  hon >= 3.8]__:.`
-00001390: 6060 0a70 6970 2069 6e73 7461 6c6c 2070  ``.pip install p
-000013a0: 796a 6564 6169 0a60 6060 0a4d 6f72 6520  yjedai.```.More 
-000013b0: 6f6e 205b 5079 5049 5d28 6874 7470 733a  on [PyPI](https:
-000013c0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-000013d0: 6374 2f70 796a 6564 6169 292e 0a0a 2323  ct/pyjedai)...##
-000013e0: 2320 4769 740a 0a53 6574 2075 7020 6c6f  # Git..Set up lo
-000013f0: 6361 6c6c 793a 0a60 6060 0a67 6974 2063  cally:.```.git c
-00001400: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
-00001410: 6875 622e 636f 6d2f 4149 2d74 6561 6d2d  hub.com/AI-team-
-00001420: 556f 412f 7079 4a65 6441 492e 6769 740a  UoA/pyJedAI.git.
-00001430: 6060 600a 676f 2074 6f20 7468 6520 726f  ```.go to the ro
-00001440: 6f74 2064 6972 6563 746f 7279 2077 6974  ot directory wit
-00001450: 6820 6063 6420 7079 4a65 6441 4960 2061  h `cd pyJedAI` a
-00001460: 6e64 2074 7970 653a 0a60 6060 0a70 6970  nd type:.```.pip
-00001470: 2069 6e73 7461 6c6c 202e 0a60 6060 0a0a   install ..```..
-00001480: 2323 2320 446f 636b 6572 0a0a 4176 6169  ### Docker..Avai
-00001490: 6c61 626c 6520 6174 205b 446f 636b 6572  lable at [Docker
-000014a0: 2048 7562 5d28 6874 7470 733a 2f2f 6875   Hub](https://hu
-000014b0: 622e 646f 636b 6572 2e63 6f6d 2f72 2f61  b.docker.com/r/a
-000014c0: 6974 6561 6d75 6f61 2f70 796a 6564 6169  iteamuoa/pyjedai
-000014d0: 292c 206f 7220 636c 6f6e 6520 7468 6973  ), or clone this
-000014e0: 2072 6570 6f20 616e 643a 0a60 6060 0a64   repo and:.```.d
-000014f0: 6f63 6b65 7220 6275 696c 6420 2d66 2044  ocker build -f D
-00001500: 6f63 6b65 7266 696c 650a 6060 600a 0a23  ockerfile.```..#
-00001510: 2044 6570 656e 6465 6e63 6965 730a 0a3c   Dependencies..<
-00001520: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
-00001530: 7222 3e0a 2020 2020 3c69 6d67 2061 6c69  r">.    <img ali
-00001540: 676e 3d22 6365 6e74 6572 2220 7372 633d  gn="center" src=
-00001550: 2268 7474 7073 3a2f 2f75 706c 6f61 642e  "https://upload.
-00001560: 7769 6b69 6d65 6469 612e 6f72 672f 7769  wikimedia.org/wi
-00001570: 6b69 7065 6469 612f 636f 6d6d 6f6e 732f  kipedia/commons/
-00001580: 7468 756d 622f 652f 6564 2f50 616e 6461  thumb/e/ed/Panda
-00001590: 735f 6c6f 676f 2e73 7667 2f32 3536 3070  s_logo.svg/2560p
-000015a0: 782d 5061 6e64 6173 5f6c 6f67 6f2e 7376  x-Pandas_logo.sv
-000015b0: 672e 706e 6722 2077 6964 7468 3d31 3230  g.png" width=120
-000015c0: 2f3e 2026 6e62 7370 3b26 6e62 7370 3b0a  /> &nbsp;&nbsp;.
-000015d0: 2020 2020 3c69 6d67 2061 6c69 676e 3d22      <img align="
-000015e0: 6365 6e74 6572 2220 7372 633d 2268 7474  center" src="htt
-000015f0: 7073 3a2f 2f75 706c 6f61 642e 7769 6b69  ps://upload.wiki
-00001600: 6d65 6469 612e 6f72 672f 7769 6b69 7065  media.org/wikipe
-00001610: 6469 612f 636f 6d6d 6f6e 732f 7468 756d  dia/commons/thum
-00001620: 622f 332f 3331 2f4e 756d 5079 5f6c 6f67  b/3/31/NumPy_log
-00001630: 6f5f 3230 3230 2e73 7667 2f31 3238 3070  o_2020.svg/1280p
-00001640: 782d 4e75 6d50 795f 6c6f 676f 5f32 3032  x-NumPy_logo_202
-00001650: 302e 7376 672e 706e 6722 2077 6964 7468  0.svg.png" width
-00001660: 3d31 3230 2f3e 2026 6e62 7370 3b26 6e62  =120/> &nbsp;&nb
-00001670: 7370 3b0a 2020 2020 3c69 6d67 2061 6c69  sp;.    <img ali
-00001680: 676e 3d22 6365 6e74 6572 2220 7372 633d  gn="center" src=
-00001690: 2268 7474 7073 3a2f 2f6c 6f67 6f65 7073  "https://logoeps
-000016a0: 2e63 6f6d 2f77 702d 636f 6e74 656e 742f  .com/wp-content/
-000016b0: 7570 6c6f 6164 732f 3230 3132 2f31 302f  uploads/2012/10/
-000016c0: 7079 7468 6f6e 2d6c 6f67 6f2d 7665 6374  python-logo-vect
-000016d0: 6f72 2e70 6e67 2220 7769 6474 683d 3132  or.png" width=12
-000016e0: 302f 3e20 266e 6273 703b 266e 6273 703b  0/> &nbsp;&nbsp;
-000016f0: 266e 6273 703b 0a20 2020 203c 696d 6720  &nbsp;.    <img 
-00001700: 616c 6967 6e3d 2263 656e 7465 7222 2073  align="center" s
-00001710: 7263 3d22 6874 7470 733a 2f2f 7570 6c6f  rc="https://uplo
-00001720: 6164 2e77 696b 696d 6564 6961 2e6f 7267  ad.wikimedia.org
-00001730: 2f77 696b 6970 6564 6961 2f63 6f6d 6d6f  /wikipedia/commo
-00001740: 6e73 2f74 6875 6d62 2f33 2f33 382f 4a75  ns/thumb/3/38/Ju
-00001750: 7079 7465 725f 6c6f 676f 2e73 7667 2f38  pyter_logo.svg/8
-00001760: 3833 7078 2d4a 7570 7974 6572 5f6c 6f67  83px-Jupyter_log
-00001770: 6f2e 7376 672e 706e 6722 2077 6964 7468  o.svg.png" width
-00001780: 3d37 302f 3e20 203c 6272 3e0a 2020 2020  =70/>  <br>.    
-00001790: 3c69 6d67 2061 6c69 676e 3d22 6365 6e74  <img align="cent
-000017a0: 6572 2220 7372 633d 2268 7474 7073 3a2f  er" src="https:/
-000017b0: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-000017c0: 6f6e 7465 6e74 2e63 6f6d 2f6f 7074 756e  ontent.com/optun
-000017d0: 612f 6f70 7475 6e61 2f6d 6173 7465 722f  a/optuna/master/
-000017e0: 646f 6373 2f69 6d61 6765 2f6f 7074 756e  docs/image/optun
-000017f0: 612d 6c6f 676f 2e70 6e67 2220 7769 6474  a-logo.png" widt
-00001800: 683d 3135 302f 3e0a 2020 2020 3c69 6d67  h=150/>.    <img
-00001810: 2061 6c69 676e 3d22 6365 6e74 6572 2220   align="center" 
-00001820: 7372 633d 2268 7474 7073 3a2f 2f75 706c  src="https://upl
-00001830: 6f61 642e 7769 6b69 6d65 6469 612e 6f72  oad.wikimedia.or
-00001840: 672f 7769 6b69 7065 6469 612f 636f 6d6d  g/wikipedia/comm
-00001850: 6f6e 732f 7468 756d 622f 382f 3861 2f50  ons/thumb/8/8a/P
-00001860: 6c6f 746c 795f 6c6f 676f 5f66 6f72 5f64  lotly_logo_for_d
-00001870: 6967 6974 616c 5f66 696e 616c 5f25 3238  igital_final_%28
-00001880: 3625 3239 2e70 6e67 2f31 3230 3070 782d  6%29.png/1200px-
-00001890: 506c 6f74 6c79 5f6c 6f67 6f5f 666f 725f  Plotly_logo_for_
-000018a0: 6469 6769 7461 6c5f 6669 6e61 6c5f 2532  digital_final_%2
-000018b0: 3836 2532 392e 706e 6722 2077 6964 7468  86%29.png" width
-000018c0: 3d31 3530 2f3e 0a20 2020 203c 696d 6720  =150/>.    <img 
-000018d0: 616c 6967 6e3d 2263 656e 7465 7222 2073  align="center" s
-000018e0: 7263 3d22 6874 7470 733a 2f2f 7079 746f  rc="https://pyto
-000018f0: 7263 682e 6f72 672f 7475 746f 7269 616c  rch.org/tutorial
-00001900: 732f 5f73 7461 7469 632f 696d 672f 7468  s/_static/img/th
-00001910: 756d 626e 6169 6c73 2f63 726f 7070 6564  umbnails/cropped
-00001920: 2f70 726f 6669 6c65 722e 706e 6722 2077  /profiler.png" w
-00001930: 6964 7468 3d31 3630 2f3e 200a 2020 2020  idth=160/> .    
-00001940: 3c69 6d67 2061 6c69 676e 3d22 6365 6e74  <img align="cent
-00001950: 6572 2220 7372 633d 2268 7474 7073 3a2f  er" src="https:/
-00001960: 2f77 7777 2e66 756c 6c73 7461 636b 7079  /www.fullstackpy
-00001970: 7468 6f6e 2e63 6f6d 2f69 6d67 2f6c 6f67  thon.com/img/log
-00001980: 6f73 2f73 6369 7079 2e70 6e67 2220 7769  os/scipy.png" wi
-00001990: 6474 683d 3135 302f 3e20 203c 6272 3e3c  dth=150/>  <br><
-000019a0: 6272 3e0a 2020 2020 3c69 6d67 2061 6c69  br>.    <img ali
-000019b0: 676e 3d22 6365 6e74 6572 2220 7372 633d  gn="center" src=
-000019c0: 2268 7474 7073 3a2f 2f77 7777 2e6b 6f72  "https://www.kor
-000019d0: 6e6f 736b 2e6d 652f 7265 736f 7572 6365  nosk.me/resource
-000019e0: 732f 6c61 6e67 7561 6765 2d6d 6f64 656c  s/language-model
-000019f0: 2f66 6561 7475 7265 642e 706e 6722 2077  /featured.png" w
-00001a00: 6964 7468 3d31 3530 2f3e 2026 6e62 7370  idth=150/> &nbsp
-00001a10: 3b26 6e62 7370 3b26 6e62 7370 3b0a 2020  ;&nbsp;&nbsp;.  
-00001a20: 2020 3c69 6d67 2061 6c69 676e 3d22 6365    <img align="ce
-00001a30: 6e74 6572 2220 7372 633d 2268 7474 7073  nter" src="https
-00001a40: 3a2f 2f72 6570 6f73 6974 6f72 792d 696d  ://repository-im
-00001a50: 6167 6573 2e67 6974 6875 6275 7365 7263  ages.githubuserc
-00001a60: 6f6e 7465 6e74 2e63 6f6d 2f31 3334 3937  ontent.com/13497
-00001a70: 3735 2f32 3032 6334 3638 302d 3866 3763  75/202c4680-8f7c
-00001a80: 2d31 3165 392d 3931 6336 2d37 3435 6664  -11e9-91c6-745fd
-00001a90: 6362 6566 6665 3822 2077 6964 7468 3d31  cbeffe8" width=1
-00001aa0: 3530 2f3e 2026 6e62 7370 3b26 6e62 7370  50/> &nbsp;&nbsp
-00001ab0: 3b26 6e62 7370 3b0a 2020 2020 3c69 6d67  ;&nbsp;.    <img
-00001ac0: 2061 6c69 676e 3d22 6365 6e74 6572 2220   align="center" 
-00001ad0: 7372 633d 2268 7474 7073 3a2f 2f6e 6574  src="https://net
-00001ae0: 776f 726b 782e 6f72 672f 5f73 7461 7469  workx.org/_stati
-00001af0: 632f 6e65 7477 6f72 6b78 5f6c 6f67 6f2e  c/networkx_logo.
-00001b00: 7376 6722 2077 6964 7468 3d31 3530 2f3e  svg" width=150/>
-00001b10: 2026 6e62 7370 3b26 6e62 7370 3b26 6e62   &nbsp;&nbsp;&nb
-00001b20: 7370 3b0a 2020 2020 3c69 6d67 2061 6c69  sp;.    <img ali
-00001b30: 676e 3d22 6365 6e74 6572 2220 7372 633d  gn="center" src=
-00001b40: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
-00001b50: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00001b60: 6f6d 2f52 4446 4c69 622f 4f57 4c2d 524c  om/RDFLib/OWL-RL
-00001b70: 2f6d 6173 7465 722f 4f57 4c2d 524c 2e70  /master/OWL-RL.p
-00001b80: 6e67 2220 7769 6474 683d 3730 2f3e 200a  ng" width=70/> .
-00001b90: 3c2f 6469 763e 0a3c 6272 3e0a 0a53 6565  </div>.<br>..See
-00001ba0: 2074 6865 2066 756c 6c20 6c69 7374 206f   the full list o
-00001bb0: 6620 6465 7065 6e64 656e 6369 6573 2061  f dependencies a
-00001bc0: 6e64 2061 6c6c 2076 6572 7369 6f6e 7320  nd all versions 
-00001bd0: 7573 6564 2c20 696e 2074 6869 7320 5b66  used, in this [f
-00001be0: 696c 655d 2868 7474 7073 3a2f 2f67 6974  ile](https://git
-00001bf0: 6875 622e 636f 6d2f 4149 2d74 6561 6d2d  hub.com/AI-team-
-00001c00: 556f 412f 7079 4a65 6441 492f 626c 6f62  UoA/pyJedAI/blob
-00001c10: 2f6d 6169 6e2f 7079 7072 6f6a 6563 742e  /main/pyproject.
-00001c20: 746f 6d6c 292e 0a0a 5f5f 5374 6174 7573  toml)...__Status
-00001c30: 5f5f 0a0a 5b21 5b54 6573 7473 5d28 6874  __..[![Tests](ht
-00001c40: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001c50: 2f41 492d 7465 616d 2d55 6f41 2f70 794a  /AI-team-UoA/pyJ
-00001c60: 6564 4149 2f61 6374 696f 6e73 2f77 6f72  edAI/actions/wor
-00001c70: 6b66 6c6f 7773 2f74 6573 7473 2e79 6d6c  kflows/tests.yml
-00001c80: 2f62 6164 6765 2e73 7667 3f62 7261 6e63  /badge.svg?branc
-00001c90: 683d 6d61 696e 295d 2868 7474 7073 3a2f  h=main)](https:/
-00001ca0: 2f67 6974 6875 622e 636f 6d2f 4149 2d74  /github.com/AI-t
-00001cb0: 6561 6d2d 556f 412f 7079 4a65 6441 492f  eam-UoA/pyJedAI/
-00001cc0: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-00001cd0: 732f 7465 7374 732e 796d 6c29 0a5b 215b  s/tests.yml).[![
-00001ce0: 5079 5069 5d28 6874 7470 733a 2f2f 6769  PyPi](https://gi
-00001cf0: 7468 7562 2e63 6f6d 2f41 492d 7465 616d  thub.com/AI-team
-00001d00: 2d55 6f41 2f70 794a 6564 4149 2f61 6374  -UoA/pyJedAI/act
-00001d10: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f70  ions/workflows/p
-00001d20: 7970 692d 7075 626c 6973 682e 796d 6c2f  ypi-publish.yml/
-00001d30: 6261 6467 652e 7376 6729 5d28 6874 7470  badge.svg)](http
-00001d40: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
-00001d50: 492d 7465 616d 2d55 6f41 2f70 794a 6564  I-team-UoA/pyJed
-00001d60: 4149 2f61 6374 696f 6e73 2f77 6f72 6b66  AI/actions/workf
-00001d70: 6c6f 7773 2f70 7970 692d 7075 626c 6973  lows/pypi-publis
-00001d80: 682e 796d 6c29 0a5b 215b 6d61 6465 2d77  h.yml).[![made-w
-00001d90: 6974 682d 7079 7468 6f6e 5d28 6874 7470  ith-python](http
-00001da0: 733a 2f2f 7265 6164 7468 6564 6f63 732e  s://readthedocs.
-00001db0: 6f72 672f 7072 6f6a 6563 7473 2f70 796a  org/projects/pyj
-00001dc0: 6564 6169 2f62 6164 6765 2f3f 7665 7273  edai/badge/?vers
-00001dd0: 696f 6e3d 6c61 7465 7374 295d 2868 7474  ion=latest)](htt
-00001de0: 7073 3a2f 2f70 796a 6564 6169 2e72 6561  ps://pyjedai.rea
-00001df0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00001e00: 6174 6573 742f 3f62 6164 6765 3d6c 6174  atest/?badge=lat
-00001e10: 6573 7429 0a5b 215b 636f 6465 636f 765d  est).[![codecov]
-00001e20: 2868 7474 7073 3a2f 2f63 6f64 6563 6f76  (https://codecov
-00001e30: 2e69 6f2f 6768 2f41 492d 7465 616d 2d55  .io/gh/AI-team-U
-00001e40: 6f41 2f70 796a 6564 6169 2f62 7261 6e63  oA/pyjedai/branc
-00001e50: 682f 6d61 7374 6572 2f67 7261 7068 2f62  h/master/graph/b
-00001e60: 6164 6765 2e73 7667 3f74 6f6b 656e 3d34  adge.svg?token=4
-00001e70: 5152 3058 3331 3543 4c29 5d28 6874 7470  QR0X315CL)](http
-00001e80: 733a 2f2f 636f 6465 636f 762e 696f 2f67  s://codecov.io/g
-00001e90: 682f 4149 2d74 6561 6d2d 556f 412f 7079  h/AI-team-UoA/py
-00001ea0: 6a65 6461 6929 0a0a 0a5f 5f53 7461 7469  jedai)...__Stati
-00001eb0: 7374 6963 7320 2620 496e 666f 5f5f 0a0a  stics & Info__..
-00001ec0: 215b 5079 5049 202d 2044 6f77 6e6c 6f61  ![PyPI - Downloa
-00001ed0: 6473 5d28 6874 7470 733a 2f2f 696d 672e  ds](https://img.
-00001ee0: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00001ef0: 646d 2f70 796a 6564 6169 290a 5b21 5b50  dm/pyjedai).[![P
-00001f00: 7950 4920 7665 7273 696f 6e5d 2868 7474  yPI version](htt
-00001f10: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00001f20: 2e69 6f2f 7079 7069 2f76 2f70 796a 6564  .io/pypi/v/pyjed
-00001f30: 6169 2e73 7667 3f6c 6f67 6f3d 7079 7069  ai.svg?logo=pypi
-00001f40: 266c 6f67 6f43 6f6c 6f72 3d46 4645 3837  &logoColor=FFE87
-00001f50: 3329 5d28 6874 7470 733a 2f2f 7079 7069  3)](https://pypi
-00001f60: 2e6f 7267 2f70 726f 6a65 6374 2f70 796a  .org/project/pyj
-00001f70: 6564 6169 2f29 0a0a 0a23 2042 7567 732c  edai/)...# Bugs,
-00001f80: 2044 6973 6375 7373 696f 6e73 2026 204e   Discussions & N
-00001f90: 6577 730a 0a5b 4769 7448 7562 2044 6973  ews..[GitHub Dis
-00001fa0: 6375 7373 696f 6e73 5d28 6874 7470 733a  cussions](https:
-00001fb0: 2f2f 6769 7468 7562 2e63 6f6d 2f41 492d  //github.com/AI-
-00001fc0: 7465 616d 2d55 6f41 2f70 794a 6564 4149  team-UoA/pyJedAI
-00001fd0: 2f64 6973 6375 7373 696f 6e73 2920 6973  /discussions) is
-00001fe0: 2074 6865 2064 6973 6375 7373 696f 6e20   the discussion 
-00001ff0: 666f 7275 6d20 666f 7220 6765 6e65 7261  forum for genera
-00002000: 6c20 7175 6573 7469 6f6e 7320 616e 6420  l questions and 
-00002010: 6469 7363 7573 7369 6f6e 7320 616e 6420  discussions and 
-00002020: 6f75 7220 7265 636f 6d6d 656e 6465 6420  our recommended 
-00002030: 7374 6172 7469 6e67 2070 6f69 6e74 2e20  starting point. 
-00002040: 506c 6561 7365 2072 6570 6f72 7420 616e  Please report an
-00002050: 7920 6275 6773 2074 6861 7420 796f 7520  y bugs that you 
-00002060: 6669 6e64 205b 6865 7265 5d28 6874 7470  find [here](http
-00002070: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
-00002080: 492d 7465 616d 2d55 6f41 2f70 794a 6564  I-team-UoA/pyJed
-00002090: 4149 2f69 7373 7565 7329 2e0a 0a23 204a  AI/issues)...# J
-000020a0: 6176 6120 2d20 5765 6220 4170 706c 6963  ava - Web Applic
-000020b0: 6174 696f 6e20 0a0a 3c69 6d67 2061 6c69  ation ..<img ali
-000020c0: 676e 3d22 6c65 6674 2220 7372 633d 2268  gn="left" src="h
-000020d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000020e0: 6d2f 7363 6966 792f 4a65 6441 4954 6f6f  m/scify/JedAIToo
-000020f0: 6c6b 6974 2f62 6c6f 622f 6d61 7374 6572  lkit/blob/master
-00002100: 2f64 6f63 756d 656e 7461 7469 6f6e 2f4a  /documentation/J
-00002110: 6564 4149 5f6c 6f67 6f2e 706e 673f 7261  edAI_logo.png?ra
-00002120: 773d 7472 7565 2220 616c 743d 2270 794a  w=true" alt="pyJ
-00002130: 6564 4149 2220 7769 6474 683d 2231 3330  edAI" width="130
-00002140: 222f 3e0a 0a46 6f72 204a 6176 6120 7573  "/>..For Java us
-00002150: 6572 7320 6368 6563 6b6f 7574 2074 6865  ers checkout the
-00002160: 2069 6e69 7469 616c 205b 4a65 6441 495d   initial [JedAI]
-00002170: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00002180: 636f 6d2f 7363 6966 792f 4a65 6441 4954  com/scify/JedAIT
-00002190: 6f6f 6c6b 6974 292e 2054 6865 7265 2079  oolkit). There y
-000021a0: 6f75 2063 616e 2066 696e 6420 4a61 7661  ou can find Java
-000021b0: 2062 6173 6564 2063 6f64 6520 616e 6420   based code and 
-000021c0: 6120 5765 6220 4170 706c 6963 6174 696f  a Web Applicatio
-000021d0: 6e20 666f 7220 696e 7465 7261 6374 6976  n for interactiv
-000021e0: 6520 6372 6561 7469 6f6e 206f 6620 4552  e creation of ER
-000021f0: 2077 6f72 6b66 6c6f 7773 2e20 3c62 723e   workflows. <br>
-00002200: 3c62 723e 204a 6564 4149 2063 6f6e 7374  <br> JedAI const
-00002210: 6974 7574 6573 2061 6e20 6f70 656e 2073  itutes an open s
-00002220: 6f75 7263 652c 2068 6967 6820 7363 616c  ource, high scal
-00002230: 6162 696c 6974 7920 746f 6f6c 6b69 7420  ability toolkit 
-00002240: 7468 6174 206f 6666 6572 7320 6f75 742d  that offers out-
-00002250: 6f66 2d74 6865 2d62 6f78 2073 6f6c 7574  of-the-box solut
-00002260: 696f 6e73 2066 6f72 2061 6e79 2064 6174  ions for any dat
-00002270: 6120 696e 7465 6772 6174 696f 6e20 7461  a integration ta
-00002280: 736b 2c20 652e 672e 2c20 5265 636f 7264  sk, e.g., Record
-00002290: 204c 696e 6b61 6765 2c20 456e 7469 7479   Linkage, Entity
-000022a0: 2052 6573 6f6c 7574 696f 6e20 616e 6420   Resolution and 
-000022b0: 4c69 6e6b 2044 6973 636f 7665 7279 2e20  Link Discovery. 
-000022c0: 4174 2069 7473 2063 6f72 6520 6c69 6573  At its core lies
-000022d0: 2061 2073 6574 206f 6620 646f 6d61 696e   a set of domain
-000022e0: 2d69 6e64 6570 656e 6465 6e74 2c20 7374  -independent, st
-000022f0: 6174 652d 6f66 2d74 6865 2d61 7274 2074  ate-of-the-art t
-00002300: 6563 686e 6971 7565 7320 7468 6174 2061  echniques that a
-00002310: 7070 6c79 2074 6f20 626f 7468 2052 4446  pply to both RDF
-00002320: 2061 6e64 2072 656c 6174 696f 6e61 6c20   and relational 
-00002330: 6461 7461 2e0a 0a3c 6272 3e0a 0a23 2054  data...<br>..# T
-00002340: 6561 6d20 2620 4175 7468 6f72 730a 0a3c  eam & Authors..<
-00002350: 696d 6720 616c 6967 6e3d 2272 6967 6874  img align="right
-00002360: 2220 7372 633d 2268 7474 7073 3a2f 2f67  " src="https://g
-00002370: 6974 6875 622e 636f 6d2f 4149 2d74 6561  ithub.com/AI-tea
-00002380: 6d2d 556f 412f 2e67 6974 6875 622f 626c  m-UoA/.github/bl
-00002390: 6f62 2f6d 6169 6e2f 4149 5f4c 4f47 4f2e  ob/main/AI_LOGO.
-000023a0: 706e 673f 7261 773d 7472 7565 2220 616c  png?raw=true" al
-000023b0: 743d 2270 794a 6564 4149 2220 7769 6474  t="pyJedAI" widt
-000023c0: 683d 2232 3030 222f 3e0a 0a2d 205b 4b6f  h="200"/>..- [Ko
-000023d0: 6e73 7461 6e74 696e 6f73 204e 696b 6f6c  nstantinos Nikol
-000023e0: 6574 6f73 5d28 6874 7470 733a 2f2f 6e69  etos](https://ni
-000023f0: 6b6f 6c65 746f 732d 6b2e 6769 7468 7562  koletos-k.github
-00002400: 2e69 6f29 0a2d 204a 616b 7562 204d 6163  .io).- Jakub Mac
-00002410: 6965 6a65 7773 6b69 0a2d 205b 4765 6f72  iejewski.- [Geor
-00002420: 6765 2050 6170 6164 616b 6973 5d28 6874  ge Papadakis](ht
-00002430: 7470 733a 2f2f 6770 6170 6164 6973 2e77  tps://gpapadis.w
-00002440: 6f72 6470 7265 7373 2e63 6f6d 290a 2d20  ordpress.com).- 
-00002450: 5b4d 616e 6f6c 6973 204b 6f75 6261 7261  [Manolis Koubara
-00002460: 6b69 735d 2868 7474 7073 3a2f 2f63 6769  kis](https://cgi
-00002470: 2e64 692e 756f 612e 6772 2f7e 6b6f 7562  .di.uoa.gr/~koub
-00002480: 6172 616b 2f29 0a0a 5265 7365 6172 6368  arak/)..Research
-00002490: 2061 6e64 2064 6576 656c 6f70 6d65 6e74   and development
-000024a0: 2069 7320 6d61 6465 2075 6e64 6572 2074   is made under t
-000024b0: 6865 2073 7570 6572 7669 7369 6f6e 206f  he supervision o
-000024c0: 6620 5072 2e20 4d61 6e6f 6c69 7320 4b6f  f Pr. Manolis Ko
-000024d0: 7562 6172 616b 6973 2e20 5468 6973 2069  ubarakis. This i
-000024e0: 7320 6120 7265 7365 6172 6368 2070 726f  s a research pro
-000024f0: 6a65 6374 2062 7920 7468 6520 5b41 492d  ject by the [AI-
-00002500: 5465 616d 5d28 6874 7470 733a 2f2f 6169  Team](https://ai
-00002510: 2e64 692e 756f 612e 6772 2920 6f66 2074  .di.uoa.gr) of t
-00002520: 6865 2044 6570 6172 746d 656e 7420 6f66  he Department of
-00002530: 2049 6e66 6f72 6d61 7469 6373 2061 6e64   Informatics and
-00002540: 2054 656c 6563 6f6d 6d75 6e69 6361 7469   Telecommunicati
-00002550: 6f6e 7320 6174 2074 6865 2055 6e69 7665  ons at the Unive
-00002560: 7273 6974 7920 6f66 2041 7468 656e 732e  rsity of Athens.
-00002570: 0a0a 2320 4c69 6365 6e73 650a 0a52 656c  ..# License..Rel
-00002580: 6561 7365 6420 756e 6465 7220 7468 6520  eased under the 
-00002590: 4170 6163 6865 2d32 2e30 206c 6963 656e  Apache-2.0 licen
-000025a0: 7365 2028 7365 6520 5b4c 4943 454e 5345  se (see [LICENSE
-000025b0: 2e74 7874 5d28 6874 7470 733a 2f2f 6769  .txt](https://gi
-000025c0: 7468 7562 2e63 6f6d 2f41 492d 7465 616d  thub.com/AI-team
-000025d0: 2d55 6f41 2f70 794a 6564 4149 2f62 6c6f  -UoA/pyJedAI/blo
-000025e0: 622f 6d61 696e 2f4c 4943 454e 5345 2929  b/main/LICENSE))
-000025f0: 2e0a 0a43 6f70 7972 6967 6874 20c2 a920  ...Copyright .. 
-00002600: 3230 3233 2041 492d 5465 616d 2c20 556e  2023 AI-Team, Un
-00002610: 6976 6572 7369 7479 206f 6620 4174 6865  iversity of Athe
-00002620: 6e73 0a0a 3c64 6976 2061 6c69 676e 3d22  ns..<div align="
-00002630: 6365 6e74 6572 223e 0a20 2020 203c 6872  center">.    <hr
-00002640: 3e0a 2020 2020 3c62 723e 0a20 2020 203c  >.    <br>.    <
-00002650: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00002660: 7374 656c 6172 2d70 726f 6a65 6374 2e65  stelar-project.e
-00002670: 7522 3e0a 2020 2020 2020 2020 3c69 6d67  u">.        <img
-00002680: 2061 6c69 676e 3d22 6365 6e74 6572 2220   align="center" 
-00002690: 7372 633d 2268 7474 7073 3a2f 2f73 7465  src="https://ste
-000026a0: 6c61 722d 7072 6f6a 6563 742e 6575 2f77  lar-project.eu/w
-000026b0: 702d 636f 6e74 656e 742f 7570 6c6f 6164  p-content/upload
-000026c0: 732f 3230 3232 2f30 382f 4c6f 676f 2d53  s/2022/08/Logo-S
-000026d0: 7465 6c61 722d 312d 662e 706e 6722 2077  telar-1-f.png" w
-000026e0: 6964 7468 3d31 3830 2f3e 0a20 2020 203c  idth=180/>.    <
-000026f0: 2f61 3e20 266e 6273 703b 266e 6273 703b  /a> &nbsp;&nbsp;
-00002700: 266e 6273 703b 266e 6273 703b 266e 6273  &nbsp;&nbsp;&nbs
-00002710: 703b 266e 6273 703b 266e 6273 703b 0a20  p;&nbsp;&nbsp;. 
-00002720: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
-00002730: 733a 2f2f 6563 2e65 7572 6f70 612e 6575  s://ec.europa.eu
-00002740: 2f69 6e66 6f2f 696e 6465 785f 656e 223e  /info/index_en">
-00002750: 0a20 2020 2020 2020 203c 696d 6720 616c  .        <img al
-00002760: 6967 6e3d 2263 656e 7465 7222 2073 7263  ign="center" src
-00002770: 3d22 6874 7470 733a 2f2f 7570 6c6f 6164  ="https://upload
-00002780: 2e77 696b 696d 6564 6961 2e6f 7267 2f77  .wikimedia.org/w
-00002790: 696b 6970 6564 6961 2f63 6f6d 6d6f 6e73  ikipedia/commons
-000027a0: 2f74 6875 6d62 2f62 2f62 372f 466c 6167  /thumb/b/b7/Flag
-000027b0: 5f6f 665f 4575 726f 7065 2e73 7667 2f31  _of_Europe.svg/1
-000027c0: 3230 3070 782d 466c 6167 5f6f 665f 4575  200px-Flag_of_Eu
-000027d0: 726f 7065 2e73 7667 2e70 6e67 2220 7769  rope.svg.png" wi
-000027e0: 6474 683d 3134 302f 3e0a 2020 2020 3c2f  dth=140/>.    </
-000027f0: 613e 0a20 2020 203c 6272 3e0a 2020 2020  a>.    <br>.    
-00002800: 3c62 723e 0a20 2020 2020 2020 203c 623e  <br>.        <b>
-00002810: 5468 6973 2070 726f 6a65 6374 2069 7320  This project is 
-00002820: 6265 696e 6720 6675 6e64 6564 2069 6e20  being funded in 
-00002830: 7468 6520 636f 6e74 6578 7420 6f66 203c  the context of <
-00002840: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00002850: 7374 656c 6172 2d70 726f 6a65 6374 2e65  stelar-project.e
-00002860: 7522 3e53 5445 4c41 523c 2f61 3e20 7468  u">STELAR</a> th
-00002870: 6174 2069 7320 616e 203c 6120 6872 6566  at is an <a href
-00002880: 3d22 6874 7470 733a 2f2f 7265 7365 6172  ="https://resear
-00002890: 6368 2d61 6e64 2d69 6e6e 6f76 6174 696f  ch-and-innovatio
-000028a0: 6e2e 6563 2e65 7572 6f70 612e 6575 2f66  n.ec.europa.eu/f
-000028b0: 756e 6469 6e67 2f66 756e 6469 6e67 2d6f  unding/funding-o
-000028c0: 7070 6f72 7475 6e69 7469 6573 2f66 756e  pportunities/fun
-000028d0: 6469 6e67 2d70 726f 6772 616d 6d65 732d  ding-programmes-
-000028e0: 616e 642d 6f70 656e 2d63 616c 6c73 2f68  and-open-calls/h
-000028f0: 6f72 697a 6f6e 2d65 7572 6f70 655f 656e  orizon-europe_en
-00002900: 223e 484f 5249 5a4f 4e2d 4575 726f 7065  ">HORIZON-Europe
-00002910: 3c2f 613e 2070 726f 6a65 6374 2e0a 2020  </a> project..  
-00002920: 2020 2020 2020 3c2f 623e 0a20 2020 203c        </b>.    <
-00002930: 6272 3e0a 3c2f 6469 763e 0a              br>.</div>.
+000006a0: 696d 0a52 6571 7569 7265 732d 4469 7374  im.Requires-Dist
+000006b0: 3a20 6d61 7470 6c6f 746c 6962 0a52 6571  : matplotlib.Req
+000006c0: 7569 7265 732d 4469 7374 3a20 6e65 7477  uires-Dist: netw
+000006d0: 6f72 6b78 0a52 6571 7569 7265 732d 4469  orkx.Requires-Di
+000006e0: 7374 3a20 6e6c 746b 0a52 6571 7569 7265  st: nltk.Require
+000006f0: 732d 4469 7374 3a20 6e75 6d70 790a 5265  s-Dist: numpy.Re
+00000700: 7175 6972 6573 2d44 6973 743a 2070 616e  quires-Dist: pan
+00000710: 6461 730a 5265 7175 6972 6573 2d44 6973  das.Requires-Dis
+00000720: 743a 2073 6369 7079 3d3d 312e 3132 0a52  t: scipy==1.12.R
+00000730: 6571 7569 7265 732d 4469 7374 3a20 7365  equires-Dist: se
+00000740: 6162 6f72 6e0a 5265 7175 6972 6573 2d44  aborn.Requires-D
+00000750: 6973 743a 2074 7164 6d0a 5265 7175 6972  ist: tqdm.Requir
+00000760: 6573 2d44 6973 743a 2074 7261 6e73 666f  es-Dist: transfo
+00000770: 726d 6572 730a 5265 7175 6972 6573 2d44  rmers.Requires-D
+00000780: 6973 743a 2073 656e 7465 6e63 652d 7472  ist: sentence-tr
+00000790: 616e 7366 6f72 6d65 7273 0a52 6571 7569  ansformers.Requi
+000007a0: 7265 732d 4469 7374 3a20 6661 6973 732d  res-Dist: faiss-
+000007b0: 6370 750a 5265 7175 6972 6573 2d44 6973  cpu.Requires-Dis
+000007c0: 743a 2070 792d 7374 7269 6e67 6d61 7463  t: py-stringmatc
+000007d0: 6869 6e67 0a52 6571 7569 7265 732d 4469  hing.Requires-Di
+000007e0: 7374 3a20 7661 6c65 6e74 696e 653b 2070  st: valentine; p
+000007f0: 7974 686f 6e5f 7665 7273 696f 6e20 3e20  ython_version > 
+00000800: 2233 2e37 220a 5265 7175 6972 6573 2d44  "3.7".Requires-D
+00000810: 6973 743a 206f 7264 6572 6564 2d73 6574  ist: ordered-set
+00000820: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000830: 7368 6170 656c 790a 5072 6f76 6964 6573  shapely.Provides
+00000840: 2d45 7874 7261 3a20 6465 760a 5265 7175  -Extra: dev.Requ
+00000850: 6972 6573 2d44 6973 743a 2070 6970 2d74  ires-Dist: pip-t
+00000860: 6f6f 6c73 3b20 6578 7472 6120 3d3d 2022  ools; extra == "
+00000870: 6465 7622 0a52 6571 7569 7265 732d 4469  dev".Requires-Di
+00000880: 7374 3a20 7079 7465 7374 3b20 6578 7472  st: pytest; extr
+00000890: 6120 3d3d 2022 6465 7622 0a0a 3c64 6976  a == "dev"..<div
+000008a0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+000008b0: 0a20 2020 203c 6272 3e0a 2020 2020 3c69  .    <br>.    <i
+000008c0: 6d67 2061 6c69 676e 3d22 6365 6e74 6572  mg align="center
+000008d0: 2220 7372 633d 2268 7474 7073 3a2f 2f67  " src="https://g
+000008e0: 6974 6875 622e 636f 6d2f 4149 2d74 6561  ithub.com/AI-tea
+000008f0: 6d2d 556f 412f 7079 4a65 6441 492f 626c  m-UoA/pyJedAI/bl
+00000900: 6f62 2f6d 6169 6e2f 646f 6373 2f69 6d67  ob/main/docs/img
+00000910: 2f70 796a 6564 6169 2e6c 6f67 6f2e 6472  /pyjedai.logo.dr
+00000920: 6177 696f 2e70 6e67 3f72 6177 3d74 7275  awio.png?raw=tru
+00000930: 6522 2061 6c74 3d22 7079 4a65 6441 4922  e" alt="pyJedAI"
+00000940: 2077 6964 7468 3d22 3430 3022 2f3e 0a3c   width="400"/>.<
+00000950: 2f64 6976 3e0a 3c62 723e 0a3c 6272 3e0a  /div>.<br>.<br>.
+00000960: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00000970: 6572 223e 0a41 6e20 6f70 656e 2d73 6f75  er">.An open-sou
+00000980: 7263 6520 6c69 6272 6172 7920 7468 6174  rce library that
+00000990: 206c 6576 6572 6167 6573 2050 7974 686f   leverages Pytho
+000009a0: 6ee2 8099 7320 6461 7461 2073 6369 656e  n...s data scien
+000009b0: 6365 2065 636f 7379 7374 656d 2074 6f20  ce ecosystem to 
+000009c0: 6275 696c 6420 3c62 723e 2070 6f77 6572  build <br> power
+000009d0: 6675 6c20 656e 642d 746f 2d65 6e64 2045  ful end-to-end E
+000009e0: 6e74 6974 7920 5265 736f 6c75 7469 6f6e  ntity Resolution
+000009f0: 2077 6f72 6b66 6c6f 7773 2e0a 3c2f 6469   workflows..</di
+00000a00: 763e 0a0a 0a2d 2d2d 0a0a 0a23 204f 7665  v>...---...# Ove
+00000a10: 7276 6965 770a 0a70 794a 6564 4149 2069  rview..pyJedAI i
+00000a20: 7320 6120 7079 7468 6f6e 2066 7261 6d65  s a python frame
+00000a30: 776f 726b 2c20 6169 6d69 6e67 2074 6f20  work, aiming to 
+00000a40: 6f66 6665 7220 6578 7065 7274 7320 616e  offer experts an
+00000a50: 6420 6e6f 7669 6365 2075 7365 7273 2c20  d novice users, 
+00000a60: 726f 6275 7374 2061 6e64 2066 6173 7420  robust and fast 
+00000a70: 736f 6c75 7469 6f6e 7320 666f 7220 6d75  solutions for mu
+00000a80: 6c74 6970 6c65 2074 7970 6573 206f 6620  ltiple types of 
+00000a90: 456e 7469 7479 2052 6573 6f6c 7574 696f  Entity Resolutio
+00000aa0: 6e20 7072 6f62 6c65 6d73 2e20 4974 2069  n problems. It i
+00000ab0: 7320 6275 696c 6465 6420 7573 696e 6720  s builded using 
+00000ac0: 7374 6174 652d 6f66 2d74 6865 2d61 7274  state-of-the-art
+00000ad0: 2070 7974 686f 6e20 6672 616d 6577 6f72   python framewor
+00000ae0: 6b73 2e20 7079 4a65 6441 4920 636f 6e73  ks. pyJedAI cons
+00000af0: 7469 7475 7465 7320 7468 6520 736f 6c65  titutes the sole
+00000b00: 206f 7065 6e2d 736f 7572 6365 204c 696e   open-source Lin
+00000b10: 6b20 4469 7363 6f76 6572 7920 746f 6f6c  k Discovery tool
+00000b20: 2074 6861 7420 6973 2063 6170 6162 6c65   that is capable
+00000b30: 206f 6620 6578 706c 6f69 7469 6e67 2074   of exploiting t
+00000b40: 6865 206c 6174 6573 7420 6272 6561 6b74  he latest breakt
+00000b50: 6872 6f75 6768 7320 696e 2044 6565 7020  hroughs in Deep 
+00000b60: 4c65 6172 6e69 6e67 2061 6e64 204e 4c50  Learning and NLP
+00000b70: 2074 6563 686e 6971 7565 732c 2077 6869   techniques, whi
+00000b80: 6368 2061 7265 2070 7562 6c69 636c 7920  ch are publicly 
+00000b90: 6176 6169 6c61 626c 6520 7468 726f 7567  available throug
+00000ba0: 6820 7468 6520 5079 7468 6f6e 2064 6174  h the Python dat
+00000bb0: 6120 7363 6965 6e63 6520 6563 6f73 7973  a science ecosys
+00000bc0: 7465 6d2e 2054 6869 7320 6170 706c 6965  tem. This applie
+00000bd0: 7320 746f 2062 6f74 6820 626c 6f63 6b69  s to both blocki
+00000be0: 6e67 2061 6e64 206d 6174 6368 696e 672c  ng and matching,
+00000bf0: 2074 6875 7320 656e 7375 7269 6e67 2068   thus ensuring h
+00000c00: 6967 6820 7469 6d65 2065 6666 6963 6965  igh time efficie
+00000c10: 6e63 792c 2068 6967 6820 7363 616c 6162  ncy, high scalab
+00000c20: 696c 6974 7920 6173 2077 656c 6c20 6173  ility as well as
+00000c30: 2068 6967 6820 6566 6665 6374 6976 656e   high effectiven
+00000c40: 6573 732c 2077 6974 686f 7574 2072 6571  ess, without req
+00000c50: 7569 7269 6e67 2061 6e79 206c 6162 656c  uiring any label
+00000c60: 6c65 6420 696e 7374 616e 6365 7320 6672  led instances fr
+00000c70: 6f6d 2074 6865 2075 7365 722e 0a0a 2323  om the user...##
+00000c80: 2320 4b65 792d 4665 6174 7572 6573 0a0a  # Key-Features..
+00000c90: 2d20 496e 7075 7420 6461 7461 2d74 7970  - Input data-typ
+00000ca0: 6520 696e 6465 7065 6e64 656e 742e 2042  e independent. B
+00000cb0: 6f74 6820 7374 7275 6374 7572 6564 2061  oth structured a
+00000cc0: 6e64 2073 656d 692d 7374 7275 6374 7572  nd semi-structur
+00000cd0: 6564 2064 6174 6120 6361 6e20 6265 2070  ed data can be p
+00000ce0: 726f 6365 7373 6564 2e0a 2d20 5661 7269  rocessed..- Vari
+00000cf0: 6f75 7320 696d 706c 656d 656e 7465 6420  ous implemented 
+00000d00: 616c 676f 7269 7468 6d73 2e0a 2d20 4561  algorithms..- Ea
+00000d10: 7379 2d74 6f2d 7573 652e 0a2d 2055 7469  sy-to-use..- Uti
+00000d20: 6c69 7a65 7320 736f 6d65 206f 6620 7468  lizes some of th
+00000d30: 6520 6661 6d6f 7573 2061 6e64 2063 7574  e famous and cut
+00000d40: 7469 6e67 2d65 6467 6520 6d61 6368 696e  ting-edge machin
+00000d50: 6520 6c65 6172 6e69 6e67 2070 6163 6b61  e learning packa
+00000d60: 6765 732e 0a2d 204f 6666 6572 7320 7375  ges..- Offers su
+00000d70: 7065 7276 6973 6564 2061 6e64 2075 6e2d  pervised and un-
+00000d80: 7375 7065 7276 6973 6564 204d 4c20 7465  supervised ML te
+00000d90: 6368 6e69 7175 6573 2e0a 0a5f 5f4f 7065  chniques...__Ope
+00000da0: 6e20 6465 6d6f 7320 6172 6520 6176 6169  n demos are avai
+00000db0: 6c61 626c 6520 696e 3a5f 5f0a 0a3c 6469  lable in:__..<di
+00000dc0: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
+00000dd0: 3e0a 2020 2020 3c61 2068 7265 663d 2268  >.    <a href="h
+00000de0: 7474 7073 3a2f 2f6e 6276 6965 7765 722e  ttps://nbviewer.
+00000df0: 6f72 672f 6769 7468 7562 2f41 492d 7465  org/github/AI-te
+00000e00: 616d 2d55 6f41 2f70 794a 6564 4149 2f62  am-UoA/pyJedAI/b
+00000e10: 6c6f 622f 6d61 696e 2f64 6f63 732f 7475  lob/main/docs/tu
+00000e20: 746f 7269 616c 732f 4465 6d6f 2e69 7079  torials/Demo.ipy
+00000e30: 6e62 223e 0a20 2020 2020 2020 203c 696d  nb">.        <im
+00000e40: 6720 616c 6967 6e3d 2263 656e 7465 7222  g align="center"
+00000e50: 2073 7263 3d22 6874 7470 733a 2f2f 6e62   src="https://nb
+00000e60: 7669 6577 6572 2e6f 7267 2f73 7461 7469  viewer.org/stati
+00000e70: 632f 696d 672f 6e61 765f 6c6f 676f 2e73  c/img/nav_logo.s
+00000e80: 7667 2220 7769 6474 683d 3132 302f 3e20  vg" width=120/> 
+00000e90: 0a20 2020 203c 2f61 3e20 2026 6e62 7370  .    </a>  &nbsp
+00000ea0: 3b26 6e62 7370 3b26 6e62 7370 3b26 6e62  ;&nbsp;&nbsp;&nb
+00000eb0: 7370 3b26 6e62 7370 3b26 6e62 7370 3b26  sp;&nbsp;&nbsp;&
+00000ec0: 6e62 7370 3b0a 2020 2020 3c61 2068 7265  nbsp;.    <a hre
+00000ed0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00000ee0: 622e 636f 6d2f 4149 2d74 6561 6d2d 556f  b.com/AI-team-Uo
+00000ef0: 412f 7079 4a65 6441 492f 626c 6f62 2f6d  A/pyJedAI/blob/m
+00000f00: 6169 6e2f 646f 6373 2f74 7574 6f72 6961  ain/docs/tutoria
+00000f10: 6c73 2f44 656d 6f2e 6970 796e 6222 3e0a  ls/Demo.ipynb">.
+00000f20: 2020 2020 2020 2020 3c69 6d67 2061 6c69          <img ali
+00000f30: 676e 3d22 6365 6e74 6572 2220 7372 633d  gn="center" src=
+00000f40: 2268 7474 7073 3a2f 2f6d 6972 6f2e 6d65  "https://miro.me
+00000f50: 6469 756d 2e63 6f6d 2f6d 6178 2f31 3430  dium.com/max/140
+00000f60: 302f 312a 4564 6e5f 4c70 6253 704c 654e  0/1*Edn_LpbSpLeN
+00000f70: 4b66 576b 4564 4732 4a67 2e70 6e67 2220  KfWkEdG2Jg.png" 
+00000f80: 7769 6474 683d 3132 302f 3e20 0a20 2020  width=120/> .   
+00000f90: 203c 2f61 3e0a 3c2f 6469 763e 0a0a 5f5f   </a>.</div>..__
+00000fa0: 476f 6f67 6c65 2043 6f6c 6162 2048 616e  Google Colab Han
+00000fb0: 6473 2d6f 6e20 6465 6d6f 3a5f 5f20 0a0a  ds-on demo:__ ..
+00000fc0: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00000fd0: 6572 223e 0a20 2020 203c 6120 6872 6566  er">.    <a href
+00000fe0: 3d22 6874 7470 733a 2f2f 636f 6c61 622e  ="https://colab.
+00000ff0: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
+00001000: 636f 6d2f 6472 6976 652f 3138 5667 454f  com/drive/18VgEO
+00001010: 4b41 6332 4f62 4646 7844 4e62 3273 6a68  KAc2ObFFxDNb2sjh
+00001020: 424c 4b4b 734e 7666 4550 6f3f 7573 703d  BLKKsNvfEPo?usp=
+00001030: 7368 6172 696e 6722 3e0a 2020 2020 2020  sharing">.      
+00001040: 2020 3c69 6d67 2061 6c69 676e 3d22 6365    <img align="ce
+00001050: 6e74 6572 2220 7372 633d 2268 7474 7073  nter" src="https
+00001060: 3a2f 2f33 2e62 702e 626c 6f67 7370 6f74  ://3.bp.blogspot
+00001070: 2e63 6f6d 2f2d 6170 6f42 6557 4679 634b  .com/-apoBeWFycK
+00001080: 512f 5868 4b42 3866 4570 7277 492f 4141  Q/XhKB8fEprwI/AA
+00001090: 4141 4141 4141 434d 342f 536c 3736 797a  AAAAAACM4/Sl76yz
+000010a0: 4e53 4e59 776c 5368 4942 7268 6544 4175  NSNYwlShIBrheDAu
+000010b0: 6d38 4c39 7152 7457 4e64 6743 4c63 4247  m8L9qRtWNdgCLcBG
+000010c0: 4173 5948 512f 7331 3630 302f 636f 6c61  AsYHQ/s1600/cola
+000010d0: 622e 706e 6722 2077 6964 7468 3d31 3230  b.png" width=120
+000010e0: 2f3e 200a 2020 2020 3c2f 613e 0a3c 2f64  /> .    </a>.</d
+000010f0: 6976 3e0a 0a23 2049 6e73 7461 6c6c 0a0a  iv>..# Install..
+00001100: 7079 4a65 6441 4920 6861 7320 6265 656e  pyJedAI has been
+00001110: 2074 6573 7465 6420 696e 2057 696e 646f   tested in Windo
+00001120: 7773 2061 6e64 204c 696e 7578 204f 532e  ws and Linux OS.
+00001130: 200a 0a5f 5f42 6173 6963 2072 6571 7569   ..__Basic requi
+00001140: 7265 6d65 6e74 733a 5f5f 0a0a 2d20 5079  rements:__..- Py
+00001150: 7468 6f6e 2076 6572 7369 6f6e 2067 7265  thon version gre
+00001160: 6174 6572 206f 7220 6571 7561 6c20 746f  ater or equal to
+00001170: 202a 2a33 2e38 2a2a 2e0a 2d20 466f 7220   **3.8**..- For 
+00001180: 5769 6e64 6f77 732c 204d 6963 726f 736f  Windows, Microso
+00001190: 6674 2056 6973 7561 6c20 432b 2b20 3134  ft Visual C++ 14
+000011a0: 2e30 2069 7320 7265 7175 6972 6564 2e20  .0 is required. 
+000011b0: 446f 776e 6c6f 6164 2069 7420 6672 6f6d  Download it from
+000011c0: 205b 4d69 6372 6f73 6f66 7420 4f66 6669   [Microsoft Offi
+000011d0: 6369 616c 2073 6974 655d 2868 7474 7073  cial site](https
+000011e0: 3a2f 2f76 6973 7561 6c73 7475 6469 6f2e  ://visualstudio.
+000011f0: 6d69 6372 6f73 6f66 742e 636f 6d2f 7669  microsoft.com/vi
+00001200: 7375 616c 2d63 7070 2d62 7569 6c64 2d74  sual-cpp-build-t
+00001210: 6f6f 6c73 2f29 2e0a 0a23 2323 2050 7950  ools/)...### PyP
+00001220: 490a 496e 7374 616c 6c20 7468 6520 6c61  I.Install the la
+00001230: 7465 7374 2076 6572 7369 6f6e 206f 6620  test version of 
+00001240: 7079 6a65 6461 693a 0a60 6060 0a70 6970  pyjedai:.```.pip
+00001250: 2069 6e73 7461 6c6c 2070 796a 6564 6169   install pyjedai
+00001260: 0a60 6060 0a4d 6f72 6520 6f6e 205b 5079  .```.More on [Py
+00001270: 5049 5d28 6874 7470 733a 2f2f 7079 7069  PI](https://pypi
+00001280: 2e6f 7267 2f70 726f 6a65 6374 2f70 796a  .org/project/pyj
+00001290: 6564 6169 292e 0a0a 2323 2320 4769 740a  edai)...### Git.
+000012a0: 0a53 6574 2075 7020 6c6f 6361 6c6c 793a  .Set up locally:
+000012b0: 0a60 6060 0a67 6974 2063 6c6f 6e65 2068  .```.git clone h
+000012c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000012d0: 6d2f 4149 2d74 6561 6d2d 556f 412f 7079  m/AI-team-UoA/py
+000012e0: 4a65 6441 492e 6769 740a 6060 600a 676f  JedAI.git.```.go
+000012f0: 2074 6f20 7468 6520 726f 6f74 2064 6972   to the root dir
+00001300: 6563 746f 7279 2077 6974 6820 6063 6420  ectory with `cd 
+00001310: 7079 4a65 6441 4960 2061 6e64 2074 7970  pyJedAI` and typ
+00001320: 653a 0a60 6060 0a70 6970 2069 6e73 7461  e:.```.pip insta
+00001330: 6c6c 202e 0a60 6060 0a0a 2323 2320 446f  ll ..```..### Do
+00001340: 636b 6572 0a0a 4176 6169 6c61 626c 6520  cker..Available 
+00001350: 6174 205b 446f 636b 6572 2048 7562 5d28  at [Docker Hub](
+00001360: 6874 7470 733a 2f2f 6875 622e 646f 636b  https://hub.dock
+00001370: 6572 2e63 6f6d 2f72 2f61 6974 6561 6d75  er.com/r/aiteamu
+00001380: 6f61 2f70 796a 6564 6169 292c 206f 7220  oa/pyjedai), or 
+00001390: 636c 6f6e 6520 7468 6973 2072 6570 6f20  clone this repo 
+000013a0: 616e 643a 0a60 6060 0a64 6f63 6b65 7220  and:.```.docker 
+000013b0: 6275 696c 6420 2d66 2044 6f63 6b65 7266  build -f Dockerf
+000013c0: 696c 650a 6060 600a 0a23 2044 6570 656e  ile.```..# Depen
+000013d0: 6465 6e63 6965 730a 0a3c 6469 7620 616c  dencies..<div al
+000013e0: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+000013f0: 2020 3c69 6d67 2061 6c69 676e 3d22 6365    <img align="ce
+00001400: 6e74 6572 2220 7372 633d 2268 7474 7073  nter" src="https
+00001410: 3a2f 2f75 706c 6f61 642e 7769 6b69 6d65  ://upload.wikime
+00001420: 6469 612e 6f72 672f 7769 6b69 7065 6469  dia.org/wikipedi
+00001430: 612f 636f 6d6d 6f6e 732f 7468 756d 622f  a/commons/thumb/
+00001440: 652f 6564 2f50 616e 6461 735f 6c6f 676f  e/ed/Pandas_logo
+00001450: 2e73 7667 2f32 3536 3070 782d 5061 6e64  .svg/2560px-Pand
+00001460: 6173 5f6c 6f67 6f2e 7376 672e 706e 6722  as_logo.svg.png"
+00001470: 2077 6964 7468 3d31 3230 2f3e 2026 6e62   width=120/> &nb
+00001480: 7370 3b26 6e62 7370 3b0a 2020 2020 3c69  sp;&nbsp;.    <i
+00001490: 6d67 2061 6c69 676e 3d22 6365 6e74 6572  mg align="center
+000014a0: 2220 7372 633d 2268 7474 7073 3a2f 2f75  " src="https://u
+000014b0: 706c 6f61 642e 7769 6b69 6d65 6469 612e  pload.wikimedia.
+000014c0: 6f72 672f 7769 6b69 7065 6469 612f 636f  org/wikipedia/co
+000014d0: 6d6d 6f6e 732f 7468 756d 622f 332f 3331  mmons/thumb/3/31
+000014e0: 2f4e 756d 5079 5f6c 6f67 6f5f 3230 3230  /NumPy_logo_2020
+000014f0: 2e73 7667 2f31 3238 3070 782d 4e75 6d50  .svg/1280px-NumP
+00001500: 795f 6c6f 676f 5f32 3032 302e 7376 672e  y_logo_2020.svg.
+00001510: 706e 6722 2077 6964 7468 3d31 3230 2f3e  png" width=120/>
+00001520: 2026 6e62 7370 3b26 6e62 7370 3b0a 2020   &nbsp;&nbsp;.  
+00001530: 2020 3c69 6d67 2061 6c69 676e 3d22 6365    <img align="ce
+00001540: 6e74 6572 2220 7372 633d 2268 7474 7073  nter" src="https
+00001550: 3a2f 2f6c 6f67 6f65 7073 2e63 6f6d 2f77  ://logoeps.com/w
+00001560: 702d 636f 6e74 656e 742f 7570 6c6f 6164  p-content/upload
+00001570: 732f 3230 3132 2f31 302f 7079 7468 6f6e  s/2012/10/python
+00001580: 2d6c 6f67 6f2d 7665 6374 6f72 2e70 6e67  -logo-vector.png
+00001590: 2220 7769 6474 683d 3132 302f 3e20 266e  " width=120/> &n
+000015a0: 6273 703b 266e 6273 703b 266e 6273 703b  bsp;&nbsp;&nbsp;
+000015b0: 0a20 2020 203c 696d 6720 616c 6967 6e3d  .    <img align=
+000015c0: 2263 656e 7465 7222 2073 7263 3d22 6874  "center" src="ht
+000015d0: 7470 733a 2f2f 7570 6c6f 6164 2e77 696b  tps://upload.wik
+000015e0: 696d 6564 6961 2e6f 7267 2f77 696b 6970  imedia.org/wikip
+000015f0: 6564 6961 2f63 6f6d 6d6f 6e73 2f74 6875  edia/commons/thu
+00001600: 6d62 2f33 2f33 382f 4a75 7079 7465 725f  mb/3/38/Jupyter_
+00001610: 6c6f 676f 2e73 7667 2f38 3833 7078 2d4a  logo.svg/883px-J
+00001620: 7570 7974 6572 5f6c 6f67 6f2e 7376 672e  upyter_logo.svg.
+00001630: 706e 6722 2077 6964 7468 3d37 302f 3e20  png" width=70/> 
+00001640: 203c 6272 3e0a 2020 2020 3c69 6d67 2061   <br>.    <img a
+00001650: 6c69 676e 3d22 6365 6e74 6572 2220 7372  lign="center" sr
+00001660: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00001670: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00001680: 2e63 6f6d 2f6f 7074 756e 612f 6f70 7475  .com/optuna/optu
+00001690: 6e61 2f6d 6173 7465 722f 646f 6373 2f69  na/master/docs/i
+000016a0: 6d61 6765 2f6f 7074 756e 612d 6c6f 676f  mage/optuna-logo
+000016b0: 2e70 6e67 2220 7769 6474 683d 3135 302f  .png" width=150/
+000016c0: 3e0a 2020 2020 3c69 6d67 2061 6c69 676e  >.    <img align
+000016d0: 3d22 6365 6e74 6572 2220 7372 633d 2268  ="center" src="h
+000016e0: 7474 7073 3a2f 2f75 706c 6f61 642e 7769  ttps://upload.wi
+000016f0: 6b69 6d65 6469 612e 6f72 672f 7769 6b69  kimedia.org/wiki
+00001700: 7065 6469 612f 636f 6d6d 6f6e 732f 7468  pedia/commons/th
+00001710: 756d 622f 382f 3861 2f50 6c6f 746c 795f  umb/8/8a/Plotly_
+00001720: 6c6f 676f 5f66 6f72 5f64 6967 6974 616c  logo_for_digital
+00001730: 5f66 696e 616c 5f25 3238 3625 3239 2e70  _final_%286%29.p
+00001740: 6e67 2f31 3230 3070 782d 506c 6f74 6c79  ng/1200px-Plotly
+00001750: 5f6c 6f67 6f5f 666f 725f 6469 6769 7461  _logo_for_digita
+00001760: 6c5f 6669 6e61 6c5f 2532 3836 2532 392e  l_final_%286%29.
+00001770: 706e 6722 2077 6964 7468 3d31 3530 2f3e  png" width=150/>
+00001780: 0a20 2020 203c 696d 6720 616c 6967 6e3d  .    <img align=
+00001790: 2263 656e 7465 7222 2073 7263 3d22 6874  "center" src="ht
+000017a0: 7470 733a 2f2f 7079 746f 7263 682e 6f72  tps://pytorch.or
+000017b0: 672f 7475 746f 7269 616c 732f 5f73 7461  g/tutorials/_sta
+000017c0: 7469 632f 696d 672f 7468 756d 626e 6169  tic/img/thumbnai
+000017d0: 6c73 2f63 726f 7070 6564 2f70 726f 6669  ls/cropped/profi
+000017e0: 6c65 722e 706e 6722 2077 6964 7468 3d31  ler.png" width=1
+000017f0: 3630 2f3e 200a 2020 2020 3c69 6d67 2061  60/> .    <img a
+00001800: 6c69 676e 3d22 6365 6e74 6572 2220 7372  lign="center" sr
+00001810: 633d 2268 7474 7073 3a2f 2f77 7777 2e66  c="https://www.f
+00001820: 756c 6c73 7461 636b 7079 7468 6f6e 2e63  ullstackpython.c
+00001830: 6f6d 2f69 6d67 2f6c 6f67 6f73 2f73 6369  om/img/logos/sci
+00001840: 7079 2e70 6e67 2220 7769 6474 683d 3135  py.png" width=15
+00001850: 302f 3e20 203c 6272 3e3c 6272 3e0a 2020  0/>  <br><br>.  
+00001860: 2020 3c69 6d67 2061 6c69 676e 3d22 6365    <img align="ce
+00001870: 6e74 6572 2220 7372 633d 2268 7474 7073  nter" src="https
+00001880: 3a2f 2f77 7777 2e6b 6f72 6e6f 736b 2e6d  ://www.kornosk.m
+00001890: 652f 7265 736f 7572 6365 732f 6c61 6e67  e/resources/lang
+000018a0: 7561 6765 2d6d 6f64 656c 2f66 6561 7475  uage-model/featu
+000018b0: 7265 642e 706e 6722 2077 6964 7468 3d31  red.png" width=1
+000018c0: 3530 2f3e 2026 6e62 7370 3b26 6e62 7370  50/> &nbsp;&nbsp
+000018d0: 3b26 6e62 7370 3b0a 2020 2020 3c69 6d67  ;&nbsp;.    <img
+000018e0: 2061 6c69 676e 3d22 6365 6e74 6572 2220   align="center" 
+000018f0: 7372 633d 2268 7474 7073 3a2f 2f72 6570  src="https://rep
+00001900: 6f73 6974 6f72 792d 696d 6167 6573 2e67  ository-images.g
+00001910: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00001920: 2e63 6f6d 2f31 3334 3937 3735 2f32 3032  .com/1349775/202
+00001930: 6334 3638 302d 3866 3763 2d31 3165 392d  c4680-8f7c-11e9-
+00001940: 3931 6336 2d37 3435 6664 6362 6566 6665  91c6-745fdcbeffe
+00001950: 3822 2077 6964 7468 3d31 3530 2f3e 2026  8" width=150/> &
+00001960: 6e62 7370 3b26 6e62 7370 3b26 6e62 7370  nbsp;&nbsp;&nbsp
+00001970: 3b0a 2020 2020 3c69 6d67 2061 6c69 676e  ;.    <img align
+00001980: 3d22 6365 6e74 6572 2220 7372 633d 2268  ="center" src="h
+00001990: 7474 7073 3a2f 2f6e 6574 776f 726b 782e  ttps://networkx.
+000019a0: 6f72 672f 5f73 7461 7469 632f 6e65 7477  org/_static/netw
+000019b0: 6f72 6b78 5f6c 6f67 6f2e 7376 6722 2077  orkx_logo.svg" w
+000019c0: 6964 7468 3d31 3530 2f3e 2026 6e62 7370  idth=150/> &nbsp
+000019d0: 3b26 6e62 7370 3b26 6e62 7370 3b0a 2020  ;&nbsp;&nbsp;.  
+000019e0: 2020 3c69 6d67 2061 6c69 676e 3d22 6365    <img align="ce
+000019f0: 6e74 6572 2220 7372 633d 2268 7474 7073  nter" src="https
+00001a00: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00001a10: 7263 6f6e 7465 6e74 2e63 6f6d 2f52 4446  rcontent.com/RDF
+00001a20: 4c69 622f 4f57 4c2d 524c 2f6d 6173 7465  Lib/OWL-RL/maste
+00001a30: 722f 4f57 4c2d 524c 2e70 6e67 2220 7769  r/OWL-RL.png" wi
+00001a40: 6474 683d 3730 2f3e 200a 3c2f 6469 763e  dth=70/> .</div>
+00001a50: 0a3c 6272 3e0a 0a53 6565 2074 6865 2066  .<br>..See the f
+00001a60: 756c 6c20 6c69 7374 206f 6620 6465 7065  ull list of depe
+00001a70: 6e64 656e 6369 6573 2061 6e64 2061 6c6c  ndencies and all
+00001a80: 2076 6572 7369 6f6e 7320 7573 6564 2c20   versions used, 
+00001a90: 696e 2074 6869 7320 5b66 696c 655d 2868  in this [file](h
+00001aa0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001ab0: 6d2f 4149 2d74 6561 6d2d 556f 412f 7079  m/AI-team-UoA/py
+00001ac0: 4a65 6441 492f 626c 6f62 2f6d 6169 6e2f  JedAI/blob/main/
+00001ad0: 7079 7072 6f6a 6563 742e 746f 6d6c 292e  pyproject.toml).
+00001ae0: 0a0a 5f5f 5374 6174 7573 5f5f 0a0a 5b21  ..__Status__..[!
+00001af0: 5b54 6573 7473 5d28 6874 7470 733a 2f2f  [Tests](https://
+00001b00: 6769 7468 7562 2e63 6f6d 2f41 492d 7465  github.com/AI-te
+00001b10: 616d 2d55 6f41 2f70 794a 6564 4149 2f61  am-UoA/pyJedAI/a
+00001b20: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+00001b30: 2f74 6573 7473 2e79 6d6c 2f62 6164 6765  /tests.yml/badge
+00001b40: 2e73 7667 3f62 7261 6e63 683d 6d61 696e  .svg?branch=main
+00001b50: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00001b60: 622e 636f 6d2f 4149 2d74 6561 6d2d 556f  b.com/AI-team-Uo
+00001b70: 412f 7079 4a65 6441 492f 6163 7469 6f6e  A/pyJedAI/action
+00001b80: 732f 776f 726b 666c 6f77 732f 7465 7374  s/workflows/test
+00001b90: 732e 796d 6c29 0a5b 215b 5079 5069 5d28  s.yml).[![PyPi](
+00001ba0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001bb0: 6f6d 2f41 492d 7465 616d 2d55 6f41 2f70  om/AI-team-UoA/p
+00001bc0: 794a 6564 4149 2f61 6374 696f 6e73 2f77  yJedAI/actions/w
+00001bd0: 6f72 6b66 6c6f 7773 2f70 7970 692d 7075  orkflows/pypi-pu
+00001be0: 626c 6973 682e 796d 6c2f 6261 6467 652e  blish.yml/badge.
+00001bf0: 7376 6729 5d28 6874 7470 733a 2f2f 6769  svg)](https://gi
+00001c00: 7468 7562 2e63 6f6d 2f41 492d 7465 616d  thub.com/AI-team
+00001c10: 2d55 6f41 2f70 794a 6564 4149 2f61 6374  -UoA/pyJedAI/act
+00001c20: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f70  ions/workflows/p
+00001c30: 7970 692d 7075 626c 6973 682e 796d 6c29  ypi-publish.yml)
+00001c40: 0a5b 215b 6d61 6465 2d77 6974 682d 7079  .[![made-with-py
+00001c50: 7468 6f6e 5d28 6874 7470 733a 2f2f 7265  thon](https://re
+00001c60: 6164 7468 6564 6f63 732e 6f72 672f 7072  adthedocs.org/pr
+00001c70: 6f6a 6563 7473 2f70 796a 6564 6169 2f62  ojects/pyjedai/b
+00001c80: 6164 6765 2f3f 7665 7273 696f 6e3d 6c61  adge/?version=la
+00001c90: 7465 7374 295d 2868 7474 7073 3a2f 2f70  test)](https://p
+00001ca0: 796a 6564 6169 2e72 6561 6474 6865 646f  yjedai.readthedo
+00001cb0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00001cc0: 3f62 6164 6765 3d6c 6174 6573 7429 0a5b  ?badge=latest).[
+00001cd0: 215b 636f 6465 636f 765d 2868 7474 7073  ![codecov](https
+00001ce0: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
+00001cf0: 2f41 492d 7465 616d 2d55 6f41 2f70 796a  /AI-team-UoA/pyj
+00001d00: 6564 6169 2f62 7261 6e63 682f 6d61 7374  edai/branch/mast
+00001d10: 6572 2f67 7261 7068 2f62 6164 6765 2e73  er/graph/badge.s
+00001d20: 7667 3f74 6f6b 656e 3d34 5152 3058 3331  vg?token=4QR0X31
+00001d30: 3543 4c29 5d28 6874 7470 733a 2f2f 636f  5CL)](https://co
+00001d40: 6465 636f 762e 696f 2f67 682f 4149 2d74  decov.io/gh/AI-t
+00001d50: 6561 6d2d 556f 412f 7079 6a65 6461 6929  eam-UoA/pyjedai)
+00001d60: 0a0a 0a5f 5f53 7461 7469 7374 6963 7320  ...__Statistics 
+00001d70: 2620 496e 666f 5f5f 0a0a 215b 5079 5049  & Info__..![PyPI
+00001d80: 202d 2044 6f77 6e6c 6f61 6473 5d28 6874   - Downloads](ht
+00001d90: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00001da0: 732e 696f 2f70 7970 692f 646d 2f70 796a  s.io/pypi/dm/pyj
+00001db0: 6564 6169 290a 5b21 5b50 7950 4920 7665  edai).[![PyPI ve
+00001dc0: 7273 696f 6e5d 2868 7474 7073 3a2f 2f69  rsion](https://i
+00001dd0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00001de0: 7069 2f76 2f70 796a 6564 6169 2e73 7667  pi/v/pyjedai.svg
+00001df0: 3f6c 6f67 6f3d 7079 7069 266c 6f67 6f43  ?logo=pypi&logoC
+00001e00: 6f6c 6f72 3d46 4645 3837 3329 5d28 6874  olor=FFE873)](ht
+00001e10: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00001e20: 726f 6a65 6374 2f70 796a 6564 6169 2f29  roject/pyjedai/)
+00001e30: 0a0a 0a23 2042 7567 732c 2044 6973 6375  ...# Bugs, Discu
+00001e40: 7373 696f 6e73 2026 204e 6577 730a 0a5b  ssions & News..[
+00001e50: 4769 7448 7562 2044 6973 6375 7373 696f  GitHub Discussio
+00001e60: 6e73 5d28 6874 7470 733a 2f2f 6769 7468  ns](https://gith
+00001e70: 7562 2e63 6f6d 2f41 492d 7465 616d 2d55  ub.com/AI-team-U
+00001e80: 6f41 2f70 794a 6564 4149 2f64 6973 6375  oA/pyJedAI/discu
+00001e90: 7373 696f 6e73 2920 6973 2074 6865 2064  ssions) is the d
+00001ea0: 6973 6375 7373 696f 6e20 666f 7275 6d20  iscussion forum 
+00001eb0: 666f 7220 6765 6e65 7261 6c20 7175 6573  for general ques
+00001ec0: 7469 6f6e 7320 616e 6420 6469 7363 7573  tions and discus
+00001ed0: 7369 6f6e 7320 616e 6420 6f75 7220 7265  sions and our re
+00001ee0: 636f 6d6d 656e 6465 6420 7374 6172 7469  commended starti
+00001ef0: 6e67 2070 6f69 6e74 2e20 506c 6561 7365  ng point. Please
+00001f00: 2072 6570 6f72 7420 616e 7920 6275 6773   report any bugs
+00001f10: 2074 6861 7420 796f 7520 6669 6e64 205b   that you find [
+00001f20: 6865 7265 5d28 6874 7470 733a 2f2f 6769  here](https://gi
+00001f30: 7468 7562 2e63 6f6d 2f41 492d 7465 616d  thub.com/AI-team
+00001f40: 2d55 6f41 2f70 794a 6564 4149 2f69 7373  -UoA/pyJedAI/iss
+00001f50: 7565 7329 2e0a 0a23 204a 6176 6120 2d20  ues)...# Java - 
+00001f60: 5765 6220 4170 706c 6963 6174 696f 6e20  Web Application 
+00001f70: 0a0a 3c69 6d67 2061 6c69 676e 3d22 6c65  ..<img align="le
+00001f80: 6674 2220 7372 633d 2268 7474 7073 3a2f  ft" src="https:/
+00001f90: 2f67 6974 6875 622e 636f 6d2f 7363 6966  /github.com/scif
+00001fa0: 792f 4a65 6441 4954 6f6f 6c6b 6974 2f62  y/JedAIToolkit/b
+00001fb0: 6c6f 622f 6d61 7374 6572 2f64 6f63 756d  lob/master/docum
+00001fc0: 656e 7461 7469 6f6e 2f4a 6564 4149 5f6c  entation/JedAI_l
+00001fd0: 6f67 6f2e 706e 673f 7261 773d 7472 7565  ogo.png?raw=true
+00001fe0: 2220 616c 743d 2270 794a 6564 4149 2220  " alt="pyJedAI" 
+00001ff0: 7769 6474 683d 2231 3330 222f 3e0a 0a46  width="130"/>..F
+00002000: 6f72 204a 6176 6120 7573 6572 7320 6368  or Java users ch
+00002010: 6563 6b6f 7574 2074 6865 2069 6e69 7469  eckout the initi
+00002020: 616c 205b 4a65 6441 495d 2868 7474 7073  al [JedAI](https
+00002030: 3a2f 2f67 6974 6875 622e 636f 6d2f 7363  ://github.com/sc
+00002040: 6966 792f 4a65 6441 4954 6f6f 6c6b 6974  ify/JedAIToolkit
+00002050: 292e 2054 6865 7265 2079 6f75 2063 616e  ). There you can
+00002060: 2066 696e 6420 4a61 7661 2062 6173 6564   find Java based
+00002070: 2063 6f64 6520 616e 6420 6120 5765 6220   code and a Web 
+00002080: 4170 706c 6963 6174 696f 6e20 666f 7220  Application for 
+00002090: 696e 7465 7261 6374 6976 6520 6372 6561  interactive crea
+000020a0: 7469 6f6e 206f 6620 4552 2077 6f72 6b66  tion of ER workf
+000020b0: 6c6f 7773 2e20 3c62 723e 3c62 723e 204a  lows. <br><br> J
+000020c0: 6564 4149 2063 6f6e 7374 6974 7574 6573  edAI constitutes
+000020d0: 2061 6e20 6f70 656e 2073 6f75 7263 652c   an open source,
+000020e0: 2068 6967 6820 7363 616c 6162 696c 6974   high scalabilit
+000020f0: 7920 746f 6f6c 6b69 7420 7468 6174 206f  y toolkit that o
+00002100: 6666 6572 7320 6f75 742d 6f66 2d74 6865  ffers out-of-the
+00002110: 2d62 6f78 2073 6f6c 7574 696f 6e73 2066  -box solutions f
+00002120: 6f72 2061 6e79 2064 6174 6120 696e 7465  or any data inte
+00002130: 6772 6174 696f 6e20 7461 736b 2c20 652e  gration task, e.
+00002140: 672e 2c20 5265 636f 7264 204c 696e 6b61  g., Record Linka
+00002150: 6765 2c20 456e 7469 7479 2052 6573 6f6c  ge, Entity Resol
+00002160: 7574 696f 6e20 616e 6420 4c69 6e6b 2044  ution and Link D
+00002170: 6973 636f 7665 7279 2e20 4174 2069 7473  iscovery. At its
+00002180: 2063 6f72 6520 6c69 6573 2061 2073 6574   core lies a set
+00002190: 206f 6620 646f 6d61 696e 2d69 6e64 6570   of domain-indep
+000021a0: 656e 6465 6e74 2c20 7374 6174 652d 6f66  endent, state-of
+000021b0: 2d74 6865 2d61 7274 2074 6563 686e 6971  -the-art techniq
+000021c0: 7565 7320 7468 6174 2061 7070 6c79 2074  ues that apply t
+000021d0: 6f20 626f 7468 2052 4446 2061 6e64 2072  o both RDF and r
+000021e0: 656c 6174 696f 6e61 6c20 6461 7461 2e0a  elational data..
+000021f0: 0a3c 6272 3e0a 0a23 2054 6561 6d20 2620  .<br>..# Team & 
+00002200: 4175 7468 6f72 730a 0a3c 696d 6720 616c  Authors..<img al
+00002210: 6967 6e3d 2272 6967 6874 2220 7372 633d  ign="right" src=
+00002220: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00002230: 636f 6d2f 4149 2d74 6561 6d2d 556f 412f  com/AI-team-UoA/
+00002240: 2e67 6974 6875 622f 626c 6f62 2f6d 6169  .github/blob/mai
+00002250: 6e2f 4149 5f4c 4f47 4f2e 706e 673f 7261  n/AI_LOGO.png?ra
+00002260: 773d 7472 7565 2220 616c 743d 2270 794a  w=true" alt="pyJ
+00002270: 6564 4149 2220 7769 6474 683d 2232 3030  edAI" width="200
+00002280: 222f 3e0a 0a2d 205b 4b6f 6e73 7461 6e74  "/>..- [Konstant
+00002290: 696e 6f73 204e 696b 6f6c 6574 6f73 5d28  inos Nikoletos](
+000022a0: 6874 7470 733a 2f2f 6e69 6b6f 6c65 746f  https://nikoleto
+000022b0: 732d 6b2e 6769 7468 7562 2e69 6f29 2c20  s-k.github.io), 
+000022c0: 5265 7365 6172 6368 2041 7373 6f63 6961  Research Associa
+000022d0: 7465 2061 7420 556e 6976 6572 7369 7479  te at University
+000022e0: 206f 6620 4174 6865 6e73 2c20 4772 6565   of Athens, Gree
+000022f0: 6365 0a2d 205b 4a61 6b75 6220 4d61 6369  ce.- [Jakub Maci
+00002300: 656a 6577 736b 695d 2868 7474 7073 3a2f  ejewski](https:/
+00002310: 2f77 7777 2e6c 696e 6b65 6469 6e2e 636f  /www.linkedin.co
+00002320: 6d2f 696e 2f6a 616b 7562 2d6d 6163 6965  m/in/jakub-macie
+00002330: 6a65 7773 6b69 2d30 3237 3032 3931 6237  jewski-0270291b7
+00002340: 2f29 2c20 5265 7365 6172 6368 2041 7373  /), Research Ass
+00002350: 6f63 6961 7465 2061 7420 556e 6976 6572  ociate at Univer
+00002360: 7369 7479 206f 6620 4174 6865 6e73 2c20  sity of Athens, 
+00002370: 4772 6565 6365 0a2d 205b 4765 6f72 6765  Greece.- [George
+00002380: 2050 6170 6164 616b 6973 5d28 6874 7470   Papadakis](http
+00002390: 733a 2f2f 6770 6170 6164 6973 2e77 6f72  s://gpapadis.wor
+000023a0: 6470 7265 7373 2e63 6f6d 292c 2053 656e  dpress.com), Sen
+000023b0: 696f 7220 5265 7365 6172 6368 6572 2061  ior Researcher a
+000023c0: 7420 556e 6976 6572 7369 7479 206f 6620  t University of 
+000023d0: 4174 6865 6e73 2c20 4772 6565 6365 0a2d  Athens, Greece.-
+000023e0: 205b 456b 6174 6572 696e 6920 496f 616e   [Ekaterini Ioan
+000023f0: 6e6f 755d 2868 7474 7073 3a2f 2f77 7777  nou](https://www
+00002400: 2e74 696c 6275 7267 756e 6976 6572 7369  .tilburguniversi
+00002410: 7479 2e65 6475 2f73 7461 6666 2f65 6b61  ty.edu/staff/eka
+00002420: 7465 7269 6e69 2d69 6f61 6e6e 6f75 292c  terini-ioannou),
+00002430: 2041 7373 6973 7461 6e74 2050 726f 6665   Assistant Profe
+00002440: 7373 6f72 2061 7420 5469 6c62 7572 6720  ssor at Tilburg 
+00002450: 556e 6976 6572 7369 7479 2c20 5468 6520  University, The 
+00002460: 4e65 7468 6572 6c61 6e64 7320 0a2d 205b  Netherlands .- [
+00002470: 4d61 6e6f 6c69 7320 4b6f 7562 6172 616b  Manolis Koubarak
+00002480: 6973 5d28 6874 7470 733a 2f2f 6367 692e  is](https://cgi.
+00002490: 6469 2e75 6f61 2e67 722f 7e6b 6f75 6261  di.uoa.gr/~kouba
+000024a0: 7261 6b2f 292c 2050 726f 6665 7373 6f72  rak/), Professor
+000024b0: 2061 7420 556e 6976 6572 7369 7479 206f   at University o
+000024c0: 6620 4174 6865 6e73 2c20 4772 6565 6365  f Athens, Greece
+000024d0: 0a0a 5468 6973 2069 7320 6120 7265 7365  ..This is a rese
+000024e0: 6172 6368 2070 726f 6a65 6374 2062 7920  arch project by 
+000024f0: 7468 6520 5b41 492d 5465 616d 5d28 6874  the [AI-Team](ht
+00002500: 7470 733a 2f2f 6169 2e64 692e 756f 612e  tps://ai.di.uoa.
+00002510: 6772 2920 6f66 2074 6865 2044 6570 6172  gr) of the Depar
+00002520: 746d 656e 7420 6f66 2049 6e66 6f72 6d61  tment of Informa
+00002530: 7469 6373 2061 6e64 2054 656c 6563 6f6d  tics and Telecom
+00002540: 6d75 6e69 6361 7469 6f6e 7320 6174 2074  munications at t
+00002550: 6865 2055 6e69 7665 7273 6974 7920 6f66  he University of
+00002560: 2041 7468 656e 732e 0a0a 2320 4c69 6365   Athens...# Lice
+00002570: 6e73 650a 0a52 656c 6561 7365 6420 756e  nse..Released un
+00002580: 6465 7220 7468 6520 4170 6163 6865 2d32  der the Apache-2
+00002590: 2e30 206c 6963 656e 7365 2028 7365 6520  .0 license (see 
+000025a0: 5b4c 4943 454e 5345 2e74 7874 5d28 6874  [LICENSE.txt](ht
+000025b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000025c0: 2f41 492d 7465 616d 2d55 6f41 2f70 794a  /AI-team-UoA/pyJ
+000025d0: 6564 4149 2f62 6c6f 622f 6d61 696e 2f4c  edAI/blob/main/L
+000025e0: 4943 454e 5345 2929 2e0a 0a43 6f70 7972  ICENSE))...Copyr
+000025f0: 6967 6874 20c2 a920 3230 3234 2041 492d  ight .. 2024 AI-
+00002600: 5465 616d 2c20 556e 6976 6572 7369 7479  Team, University
+00002610: 206f 6620 4174 6865 6e73 0a0a 3c64 6976   of Athens..<div
+00002620: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00002630: 0a20 2020 203c 6872 3e0a 2020 2020 3c62  .    <hr>.    <b
+00002640: 723e 0a20 2020 203c 6120 6872 6566 3d22  r>.    <a href="
+00002650: 6874 7470 733a 2f2f 7374 656c 6172 2d70  https://stelar-p
+00002660: 726f 6a65 6374 2e65 7522 3e0a 2020 2020  roject.eu">.    
+00002670: 2020 2020 3c69 6d67 2061 6c69 676e 3d22      <img align="
+00002680: 6365 6e74 6572 2220 7372 633d 2268 7474  center" src="htt
+00002690: 7073 3a2f 2f73 7465 6c61 722d 7072 6f6a  ps://stelar-proj
+000026a0: 6563 742e 6575 2f77 702d 636f 6e74 656e  ect.eu/wp-conten
+000026b0: 742f 7570 6c6f 6164 732f 3230 3232 2f30  t/uploads/2022/0
+000026c0: 382f 4c6f 676f 2d53 7465 6c61 722d 312d  8/Logo-Stelar-1-
+000026d0: 662e 706e 6722 2077 6964 7468 3d31 3830  f.png" width=180
+000026e0: 2f3e 0a20 2020 203c 2f61 3e20 266e 6273  />.    </a> &nbs
+000026f0: 703b 266e 6273 703b 266e 6273 703b 266e  p;&nbsp;&nbsp;&n
+00002700: 6273 703b 266e 6273 703b 266e 6273 703b  bsp;&nbsp;&nbsp;
+00002710: 266e 6273 703b 0a20 2020 203c 6120 6872  &nbsp;.    <a hr
+00002720: 6566 3d22 6874 7470 733a 2f2f 6563 2e65  ef="https://ec.e
+00002730: 7572 6f70 612e 6575 2f69 6e66 6f2f 696e  uropa.eu/info/in
+00002740: 6465 785f 656e 223e 0a20 2020 2020 2020  dex_en">.       
+00002750: 203c 696d 6720 616c 6967 6e3d 2263 656e   <img align="cen
+00002760: 7465 7222 2073 7263 3d22 6874 7470 733a  ter" src="https:
+00002770: 2f2f 7570 6c6f 6164 2e77 696b 696d 6564  //upload.wikimed
+00002780: 6961 2e6f 7267 2f77 696b 6970 6564 6961  ia.org/wikipedia
+00002790: 2f63 6f6d 6d6f 6e73 2f74 6875 6d62 2f62  /commons/thumb/b
+000027a0: 2f62 372f 466c 6167 5f6f 665f 4575 726f  /b7/Flag_of_Euro
+000027b0: 7065 2e73 7667 2f31 3230 3070 782d 466c  pe.svg/1200px-Fl
+000027c0: 6167 5f6f 665f 4575 726f 7065 2e73 7667  ag_of_Europe.svg
+000027d0: 2e70 6e67 2220 7769 6474 683d 3134 302f  .png" width=140/
+000027e0: 3e0a 2020 2020 3c2f 613e 0a20 2020 203c  >.    </a>.    <
+000027f0: 6272 3e0a 2020 2020 3c62 723e 0a20 2020  br>.    <br>.   
+00002800: 2020 2020 203c 623e 5468 6973 2070 726f       <b>This pro
+00002810: 6a65 6374 2069 7320 6265 696e 6720 6675  ject is being fu
+00002820: 6e64 6564 2069 6e20 7468 6520 636f 6e74  nded in the cont
+00002830: 6578 7420 6f66 203c 6120 6872 6566 3d22  ext of <a href="
+00002840: 6874 7470 733a 2f2f 7374 656c 6172 2d70  https://stelar-p
+00002850: 726f 6a65 6374 2e65 7522 3e53 5445 4c41  roject.eu">STELA
+00002860: 523c 2f61 3e20 7468 6174 2069 7320 616e  R</a> that is an
+00002870: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00002880: 2f2f 7265 7365 6172 6368 2d61 6e64 2d69  //research-and-i
+00002890: 6e6e 6f76 6174 696f 6e2e 6563 2e65 7572  nnovation.ec.eur
+000028a0: 6f70 612e 6575 2f66 756e 6469 6e67 2f66  opa.eu/funding/f
+000028b0: 756e 6469 6e67 2d6f 7070 6f72 7475 6e69  unding-opportuni
+000028c0: 7469 6573 2f66 756e 6469 6e67 2d70 726f  ties/funding-pro
+000028d0: 6772 616d 6d65 732d 616e 642d 6f70 656e  grammes-and-open
+000028e0: 2d63 616c 6c73 2f68 6f72 697a 6f6e 2d65  -calls/horizon-e
+000028f0: 7572 6f70 655f 656e 223e 484f 5249 5a4f  urope_en">HORIZO
+00002900: 4e2d 4575 726f 7065 3c2f 613e 2070 726f  N-Europe</a> pro
+00002910: 6a65 6374 2e0a 2020 2020 2020 2020 3c2f  ject..        </
+00002920: 623e 0a20 2020 203c 6272 3e0a 3c2f 6469  b>.    <br>.</di
+00002930: 763e 0a                                  v>.
```

### Comparing `pyjedai-0.1.6/README.md` & `pyjedai-0.1.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -41,16 +41,23 @@
     <a href="https://colab.research.google.com/drive/18VgEOKAc2ObFFxDNb2sjhBLKKsNvfEPo?usp=sharing">
         <img align="center" src="https://3.bp.blogspot.com/-apoBeWFycKQ/XhKB8fEprwI/AAAAAAAACM4/Sl76yzNSNYwlShIBrheDAum8L9qRtWNdgCLcBGAsYHQ/s1600/colab.png" width=120/> 
     </a>
 </div>
 
 # Install
 
+pyJedAI has been tested in Windows and Linux OS. 
+
+__Basic requirements:__
+
+- Python version greater or equal to **3.8**.
+- For Windows, Microsoft Visual C++ 14.0 is required. Download it from [Microsoft Official site](https://visualstudio.microsoft.com/visual-cpp-build-tools/).
+
 ### PyPI
-Install the latest version of pyjedai __[requires python >= 3.8]__:
+Install the latest version of pyjedai:
 ```
 pip install pyjedai
 ```
 More on [PyPI](https://pypi.org/project/pyjedai).
 
 ### Git
 
@@ -116,26 +123,27 @@
 
 <br>
 
 # Team & Authors
 
 <img align="right" src="https://github.com/AI-team-UoA/.github/blob/main/AI_LOGO.png?raw=true" alt="pyJedAI" width="200"/>
 
-- [Konstantinos Nikoletos](https://nikoletos-k.github.io)
-- Jakub Maciejewski
-- [George Papadakis](https://gpapadis.wordpress.com)
-- [Manolis Koubarakis](https://cgi.di.uoa.gr/~koubarak/)
+- [Konstantinos Nikoletos](https://nikoletos-k.github.io), Research Associate at University of Athens, Greece
+- [Jakub Maciejewski](https://www.linkedin.com/in/jakub-maciejewski-0270291b7/), Research Associate at University of Athens, Greece
+- [George Papadakis](https://gpapadis.wordpress.com), Senior Researcher at University of Athens, Greece
+- [Ekaterini Ioannou](https://www.tilburguniversity.edu/staff/ekaterini-ioannou), Assistant Professor at Tilburg University, The Netherlands 
+- [Manolis Koubarakis](https://cgi.di.uoa.gr/~koubarak/), Professor at University of Athens, Greece
 
-Research and development is made under the supervision of Pr. Manolis Koubarakis. This is a research project by the [AI-Team](https://ai.di.uoa.gr) of the Department of Informatics and Telecommunications at the University of Athens.
+This is a research project by the [AI-Team](https://ai.di.uoa.gr) of the Department of Informatics and Telecommunications at the University of Athens.
 
 # License
 
 Released under the Apache-2.0 license (see [LICENSE.txt](https://github.com/AI-team-UoA/pyJedAI/blob/main/LICENSE)).
 
-Copyright © 2023 AI-Team, University of Athens
+Copyright © 2024 AI-Team, University of Athens
 
 <div align="center">
     <hr>
     <br>
     <a href="https://stelar-project.eu">
         <img align="center" src="https://stelar-project.eu/wp-content/uploads/2022/08/Logo-Stelar-1-f.png" width=180/>
     </a> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
```

#### html2text {}

```diff
@@ -19,21 +19,24 @@
 machine learning packages. - Offers supervised and un-supervised ML techniques.
 __Open demos are available in:__
 _[_h_t_t_p_s_:_/_/_n_b_v_i_e_w_e_r_._o_r_g_/_s_t_a_t_i_c_/_i_m_g_/_n_a_v___l_o_g_o_._s_v_g_]       _[_h_t_t_p_s_:_/_/_m_i_r_o_._m_e_d_i_u_m_._c_o_m_/
                     _m_a_x_/_1_4_0_0_/_1_*_E_d_n___L_p_b_S_p_L_e_N_K_f_W_k_E_d_G_2_J_g_._p_n_g_]
 __Google Colab Hands-on demo:__
        _[_h_t_t_p_s_:_/_/_3_._b_p_._b_l_o_g_s_p_o_t_._c_o_m_/_-_a_p_o_B_e_W_F_y_c_K_Q_/_X_h_K_B_8_f_E_p_r_w_I_/_A_A_A_A_A_A_A_A_C_M_4_/
          _S_l_7_6_y_z_N_S_N_Y_w_l_S_h_I_B_r_h_e_D_A_u_m_8_L_9_q_R_t_W_N_d_g_C_L_c_B_G_A_s_Y_H_Q_/_s_1_6_0_0_/_c_o_l_a_b_._p_n_g_]
-# Install ### PyPI Install the latest version of pyjedai __[requires python >=
-3.8]__: ``` pip install pyjedai ``` More on [PyPI](https://pypi.org/project/
-pyjedai). ### Git Set up locally: ``` git clone https://github.com/AI-team-UoA/
-pyJedAI.git ``` go to the root directory with `cd pyJedAI` and type: ``` pip
-install . ``` ### Docker Available at [Docker Hub](https://hub.docker.com/r/
-aiteamuoa/pyjedai), or clone this repo and: ``` docker build -f Dockerfile ```
-# Dependencies
+# Install pyJedAI has been tested in Windows and Linux OS. __Basic
+requirements:__ - Python version greater or equal to **3.8**. - For Windows,
+Microsoft Visual C++ 14.0 is required. Download it from [Microsoft Official
+site](https://visualstudio.microsoft.com/visual-cpp-build-tools/). ### PyPI
+Install the latest version of pyjedai: ``` pip install pyjedai ``` More on
+[PyPI](https://pypi.org/project/pyjedai). ### Git Set up locally: ``` git clone
+https://github.com/AI-team-UoA/pyJedAI.git ``` go to the root directory with
+`cd pyJedAI` and type: ``` pip install . ``` ### Docker Available at [Docker
+Hub](https://hub.docker.com/r/aiteamuoa/pyjedai), or clone this repo and: ```
+docker build -f Dockerfile ``` # Dependencies
   [https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Pandas_logo.svg/
 2560px-Pandas_logo.svg.png]   [https://upload.wikimedia.org/wikipedia/commons/
   thumb/3/31/NumPy_logo_2020.svg/1280px-NumPy_logo_2020.svg.png]   [https://
   logoeps.com/wp-content/uploads/2012/10/python-logo-vector.png]    [https://
    upload.wikimedia.org/wikipedia/commons/thumb/3/38/Jupyter_logo.svg/883px-
                              Jupyter_logo.svg.png]
   [https://raw.githubusercontent.com/optuna/optuna/master/docs/image/optuna-
@@ -70,22 +73,26 @@
 based code and a Web Application for interactive creation of ER workflows.
 
 JedAI constitutes an open source, high scalability toolkit that offers out-of-
 the-box solutions for any data integration task, e.g., Record Linkage, Entity
 Resolution and Link Discovery. At its core lies a set of domain-independent,
 state-of-the-art techniques that apply to both RDF and relational data.
 # Team & Authors [pyJedAI]- [Konstantinos Nikoletos](https://nikoletos-
-k.github.io) - Jakub Maciejewski - [George Papadakis](https://
-gpapadis.wordpress.com) - [Manolis Koubarakis](https://cgi.di.uoa.gr/~koubarak/
-) Research and development is made under the supervision of Pr. Manolis
-Koubarakis. This is a research project by the [AI-Team](https://ai.di.uoa.gr)
-of the Department of Informatics and Telecommunications at the University of
-Athens. # License Released under the Apache-2.0 license (see [LICENSE.txt]
-(https://github.com/AI-team-UoA/pyJedAI/blob/main/LICENSE)). Copyright Â© 2023
-AI-Team, University of Athens
+k.github.io), Research Associate at University of Athens, Greece - [Jakub
+Maciejewski](https://www.linkedin.com/in/jakub-maciejewski-0270291b7/),
+Research Associate at University of Athens, Greece - [George Papadakis](https:/
+/gpapadis.wordpress.com), Senior Researcher at University of Athens, Greece -
+[Ekaterini Ioannou](https://www.tilburguniversity.edu/staff/ekaterini-ioannou),
+Assistant Professor at Tilburg University, The Netherlands - [Manolis
+Koubarakis](https://cgi.di.uoa.gr/~koubarak/), Professor at University of
+Athens, Greece This is a research project by the [AI-Team](https://
+ai.di.uoa.gr) of the Department of Informatics and Telecommunications at the
+University of Athens. # License Released under the Apache-2.0 license (see
+[LICENSE.txt](https://github.com/AI-team-UoA/pyJedAI/blob/main/LICENSE)).
+Copyright Â© 2024 AI-Team, University of Athens
 ===============================================================================
 
      _[_h_t_t_p_s_:_/_/_s_t_e_l_a_r_-_p_r_o_j_e_c_t_._e_u_/_w_p_-_c_o_n_t_e_n_t_/_u_p_l_o_a_d_s_/_2_0_2_2_/_0_8_/_L_o_g_o_-_S_t_e_l_a_r_-_1_-
    _f_._p_n_g_]        _[_h_t_t_p_s_:_/_/_u_p_l_o_a_d_._w_i_k_i_m_e_d_i_a_._o_r_g_/_w_i_k_i_p_e_d_i_a_/_c_o_m_m_o_n_s_/_t_h_u_m_b_/_b_/_b_7_/
                _F_l_a_g___o_f___E_u_r_o_p_e_._s_v_g_/_1_2_0_0_p_x_-_F_l_a_g___o_f___E_u_r_o_p_e_._s_v_g_._p_n_g_]
 
 TThhiiss pprroojjeecctt iiss bbeeiinngg ffuunnddeedd iinn tthhee ccoonntteexxtt ooff _SS_TT_EE_LL_AA_RR tthhaatt iiss aann _HH_OO_RR_II_ZZ_OO_NN_--_EE_uu_rr_oo_pp_ee
```

### Comparing `pyjedai-0.1.6/src/pyjedai/block_building.py` & `pyjedai-0.1.7/src/pyjedai/block_building.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.1.6/src/pyjedai/block_cleaning.py` & `pyjedai-0.1.7/src/pyjedai/block_cleaning.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,15 @@
         if not blocks:
             raise AttributeError("Empty dict of blocks was given as input!")
         else:
             new_blocks = blocks.copy()
         self._progress_bar = tqdm(total=2*len(new_blocks), desc=self._method_name, disable=self.tqdm_disable)            
         self._set_threshold(new_blocks)
         new_blocks = dict(filter(self._cardinality_threshold, blocks.items()))
+        self.num_of_blocks_dropped = len(blocks) - len(new_blocks)
         self._progress_bar.close()
         self.execution_time = time() - start_time
         self.blocks = new_blocks
 
         return new_blocks
 
     def _cardinality_threshold(self, id_block_tuple) -> bool:
```

### Comparing `pyjedai-0.1.6/src/pyjedai/clustering.py` & `pyjedai-0.1.7/src/pyjedai/clustering.py`

 * *Files 6% similar despite different names*

```diff
@@ -370,15 +370,15 @@
                                 with_classification_report,
                                 verbose)
     
     def stats(self) -> None:
         pass
 
     def _configuration(self) -> dict:
-        return {}
+        pass
 
     def export_to_df(self, prediction: list) -> pd.DataFrame:
         """creates a dataframe for the evaluation report
 
         Args:
             prediction (any): Predicted clusters
 
@@ -451,15 +451,17 @@
         resulting_clusters = list(filter(lambda x: len(x) == 2, clusters)) \
                                 if not data.is_dirty_er else clusters
         # print("Number of clusters after filtering: ", len(resulting_clusters))
         self.execution_time = time() - start_time
         return resulting_clusters
 
     def _configuration(self) -> dict:
-        return {}
+        return {
+            "Similarity Threshold": self.similarity_threshold
+        }
 
 class UniqueMappingClustering(AbstractClustering):
     """Prunes all edges with a weight lower than t, sorts the remaining ones in
         decreasing weight/similarity and iteratively forms a partition for
         the top-weighted pair as long as none of its entities has already
         been matched to some other.
     """
@@ -513,15 +515,17 @@
             matched_entities.add(entity_2)
 
         clusters = ConnectedComponentsClustering().process(new_graph, data, similarity_threshold=None)
         self.execution_time = time() - start_time
         return clusters
 
     def _configuration(self) -> dict:
-        return {}
+        return {
+            "Similarity Threshold": self.similarity_threshold
+        }
 
 class ExactClustering(AbstractClustering):
     """Implements an adapted, simplified version of the Exact THRESHOLD algorithm,
         introduced in "Similarity Flooding: A Versatile Graph Matching Algorithm and Its Application to Schema Matching",
         also referred in "BIGMAT: A Distributed Affinity-Preserving Random Walk Strategy for Instance Matching on Knowledge Graphs".
         In essence, it keeps the top-1 candidate per entity, as long as the candidate also considers this node as its top candidate.
     """
@@ -538,15 +542,17 @@
     def process(self, graph: Graph, data: Data, similarity_threshold: float = 0.1) -> list:
         """
         """
         self.similarity_threshold = similarity_threshold
         raise NotImplementedError("Exact Clustering is not implemented yet.")
 
     def _configuration(self) -> dict:
-        return {}
+        return {
+            "Similarity Threshold": self.similarity_threshold
+        }
 
 class CenterClustering(AbstractClustering):
     """Implements the Center Clustering algorithm. Input comparisons (graph edges) are sorted in descending order of similarity.
        Pairs of entities connected by these edges form the basis of the updated graph. Entities are evaluated to determine if they will serve
        as a center of a future cluster or as its member. This evaluation is based on a comparison of their cumulative edge weights in the graph,
        normalized by the number of edges in which they are involved. Finally, the algorithm identifies connected components within the graph,
        using the previously defined centers as the focal points for forming clusters.
@@ -609,15 +615,17 @@
                 new_graph.add_edge(v1, v2, weight=-similarity_score)
 
         clusters = list(connected_components(new_graph))
         self.execution_time = time() - start_time
         return clusters
 
     def _configuration(self) -> dict:
-        return {}
+        return {
+            "Similarity Threshold": self.similarity_threshold
+        }
 
 class BestMatchClustering(AbstractClustering):
     """Implements the Best Match Clustering algorithm. Based on supplied order, it either traverse the entities of the left (inorder)
        or right (reverse) dataset. For each entity, it retrieves all of its candidate pairs, stores them in descending similarity order.
        For each source entity, only the best candidate is kept (only highest similarity edge is kept in the new graph).
     """
 
@@ -692,15 +700,17 @@
                 break
 
         clusters = list(connected_components(new_graph))
         self.execution_time = time() - start_time
         return clusters
 
     def _configuration(self) -> dict:
-        return {}
+        return {
+            "Similarity Threshold": self.similarity_threshold
+        }
     
     def set_order(self, order : str) -> None:
         self.order : str = order
         
         
 class MergeCenterClustering(AbstractClustering):
     """Implements the Merge Center Clustering algorithm. It is a simplified version of the Center Clustering algorithm,
@@ -757,16 +767,17 @@
                 new_graph.add_edge(v1, v2, weight=-similarity_score)
 
         clusters = list(connected_components(new_graph))
         self.execution_time = time() - start_time
         return clusters
 
     def _configuration(self) -> dict:
-        return {}
-    
+        return {
+            "Similarity Threshold": self.similarity_threshold
+        }
     
 class CorrelationClustering(AbstractClustering):
     """Implements the Correlation Clustering algorithm. Candidate pairs are mapped into a graph, whose connected components
        act as our initial clusters. We iteratively choose one of the 3 possible moves (change, merge, break up cluster) and
        we apply them on randomly chosen entities. We decide whether we should conduct the move or not, based on an objective function,
        which quantifies the quality of our clusters (contain similar entities, seperate disimilar ones)   
     """
@@ -777,15 +788,14 @@
     _method_info: str = "Implements the Correlation Clustering algorithm," + \
         "In essence, it implements iterative clustering, " + \
         "reassigning clusters to randomly chosen entities based on the reassignment's effect on our objective function " + \
         "that evaluates the quality of the newly defined clusters." 
     
     def __init__(self) -> None:
         super().__init__()
-        self.similarity_threshold: float
         self.initial_threshold : float
         self.similarity_threshold : float
         self.non_similarity_threshold : float
         self.move_limit : int
         self.lsi_iterations: int
 
     def process(self,
@@ -879,15 +889,15 @@
     def choose_move(self) -> int:
         move = random.randint(0, self.move_limit - 1)
         while(move == 1 and len(self.clusters) == 1):
             move = random.randint(0, self.move_limit - 1)
         return move
             
     def move(self, move_index : int, previous_OF : int):
-        # print(f"Move[{move_index}] OF[{previous_OF}]")
+
         if(move_index == 0):
             random_entity = random.choice(self.valid_entities)
             random_cluster = random.randint(0, self.initial_clusters_num - 1)
             while(not self.clusters[random_cluster].has_entities()):
                 random_cluster = random.randint(0, self.initial_clusters_num - 1)
             return self.change_entity_cluster(previous_OF, random_entity, random_cluster)
         elif(move_index == 1):
@@ -904,23 +914,22 @@
         elif(move_index == 2):
             previous_cluster = random.randint(0, self.initial_clusters_num - 1)
             while(not self.clusters[previous_cluster].has_entities()):
                 previous_cluster = random.randint(0, self.initial_clusters_num - 1)
             return self.seperate_clusters(previous_OF, previous_cluster)
         else:
             raise ValueError(f"Invalid Move Index \"{move_index}\": Choose 0->2")
-            return float("inf")
         
         
     def change_entity_cluster(self, previous_OF : int, entity : int, new_cluster : int):
         previous_cluster = self.entity_cluster_index[entity]
         self.entity_cluster_index[entity] = new_cluster
         
         new_OF = self.calculate_OF()
-        # print(previous_OF, new_OF)
+
         if(new_OF > previous_OF):
             self.clusters[previous_cluster].remove_entity(entity)
             self.clusters[new_cluster].add_entity(entity)
             return new_OF
         else:
             self.entity_cluster_index[entity] = previous_cluster
             return previous_OF
@@ -932,15 +941,15 @@
         previous_cluster_entities = previous_cluster.get_entities()
     
         for entity in previous_cluster_entities:
             to_be_removed_entities.append(entity)
             self.entity_cluster_index[entity] = new_cluster_index
         
         new_OF : int = self.calculate_OF()
-        # print(previous_OF, new_OF)
+
         if(new_OF > previous_OF):
             previous_cluster.remove_entities(previous_cluster_entities)
             new_cluster.add_entities(previous_cluster_entities)
             return new_OF
 
         for to_be_removed_entity in to_be_removed_entities:
             self.entity_cluster_index[to_be_removed_entity] = previous_cluster_index
@@ -968,15 +977,21 @@
         
         for to_be_removed_entity in to_be_removed_entities:
             self.entity_cluster_index[to_be_removed_entity] = previous_cluster_index
               
         return previous_OF
 
     def _configuration(self) -> dict:
-        return {}
+        return {
+            "Initial Threshold" : self.initial_threshold,
+            "Similarity Threshold" : self.similarity_threshold,
+            "Non-Similarity Threshold" : self.non_similarity_threshold,
+            "Move limit" : self.move_limit,
+            "LSI Iterations" : self.lsi_iterations
+        }
     
 class CutClustering(AbstractClustering):
     """Implements the Cut Clustering algorithm. Retains the candidate pairs whose similarity is over the specified threshold.
        Those pairs are mapped into graph edges. Using the newly defined graph, we retrieve its Gomory Hu Tree representation
        using the Edmonds Karp flow function, while edges' capacity is considered to be infinite. We return the connected components
        of the resulting minimum s-t cuts for the pairs in the original, trimmed graph.    
     """
@@ -1014,15 +1029,17 @@
         clusters = list(connected_components(final_gomory_hu_tree))
         
         # print(len(clusters))
         self.execution_time = time() - start_time
         return clusters
 
     def _configuration(self) -> dict:
-        return {}
+        return {
+            "Similarity Threshold": self.similarity_threshold
+        }
     
 class MarkovClustering(AbstractClustering):
     """Implements the Markov Clustering algorithm. It simulates random walks on a (n x n) matrix as the adjacency matrix
        of a weighted, similarity graph. It alternates an expansion step and an inflation step until an equilibrium state is reached.
        Entries with similarity above threhold, are inserted into final graph, whose CCs we retain.    
     """
 
@@ -1127,15 +1144,20 @@
             
         return True  
     
     def get_existing_indices(self, matrix):
         return set([indices for indices in zip(*matrix.nonzero())])
     
     def _configuration(self) -> dict:
-        return {}
+        return {
+            "Similarity Threshold" : self.similarity_threshold,
+            "Cluster Threshold" : self.cluster_threshold,
+            "Matrix Similarity Threshold" : self.matrix_similarity_threshold,
+            "Similarity Checks Limit" : self.similarity_checks_limit
+        }
     
 class KiralyMSMApproximateClustering(AbstractClustering):
     """Implements the Kiraly MSM Approximate Clustering algorithm. Implements the so-called "New Algorithm"
        by Zoltan Kiraly 2013, which is a 3/2-approximation to the Maximum Stable Marriage (MSM) problem.
        The pairs resulting from the approximation of the stable relationships are translated into a graph,
        whose connected components we retain.    
     """
@@ -1295,59 +1317,64 @@
                 man_score = comparison.similarity
             elif(candidate == current_fiance):
                 current_fiance_score = comparison.similarity
         
         return (man_score > current_fiance_score)
     
     def _configuration(self) -> dict:
-        return {}
+        return {
+            "Similarity Threshold": self.similarity_threshold
+        }
     
 class RicochetSRClustering(AbstractClustering):
     """Implements the Ricochet SR Clustering algorithm. Implements the so-called "New Algorithm"
        by Zoltan Kiraly 2013, which is a 3/2-approximation to the Maximum Stable Marriage (MSM) problem.
        The pairs resulting from the approximation of the stable relationships are translated into a graph,
        whose connected components we retain.    
     """
 
     _method_name: str = "Ricochet SR Clustering"
     _method_short_name: str = "RSRC"
-    _method_info: str = "Ιmplements the Ricochet SR Clustering algorithm," + \
+    _method_info: str = "Implements the Ricochet SR Clustering algorithm," + \
         "In essence, it is a 3/2-approximation to the Maximum Stable Marriage (MSM) problem."
     def __init__(self) -> None:
         super().__init__()
         self.similarity_threshold : float
         
-    def process(self, 
+    def process(self,
                 graph: Graph,
                 data: Data, 
                 similarity_threshold: float = 0.5) -> list:
 
+        if self.data.is_dirty_er:
+            raise ValueError(f"RicochetSRClustering doesn't support Dirty ER.")
+
         start_time = time()
         self.similarity_threshold : float = similarity_threshold
         self.data = data
         clusters : list = []
         self.vertices : dict = {}
         self.sorted_vertices = PriorityQueue(maxsize = self.data.num_of_entities)
         
         for (v1, v2, data) in graph.edges(data=True):
             d1_id, d2_id = self.sorted_indicators(v1, v2)
-            similarity = data.get('weight', 0) 
-            if similarity > self.similarity_threshold:  
+            similarity = data.get('weight', 0)
+            if similarity > self.similarity_threshold:
                 if d1_id not in self.vertices: self.vertices[d1_id] = Vertex(identifier=d1_id)
                 if d2_id not in self.vertices: self.vertices[d2_id] = Vertex(identifier=d2_id)
                 self.vertices[d1_id].insert_edge(edge=(d2_id, similarity))
                 self.vertices[d2_id].insert_edge(edge=(d1_id, similarity))
         
         for _, vertex in self.vertices.items():
             if(vertex.has_edges()):
                 self.sorted_vertices.put(vertex)
 
-        if(self.sorted_vertices.empty()):            
+        if(self.sorted_vertices.empty()):
             return clusters
-        
+
         self.centers : set = set()
         self.members : set = set()
         self.center_of : dict = {}
         self.similarity_with_center : dict = defaultdict(float)
         self.current_clusters : dict = defaultdict(set)
         
         top_vertex : Vertex = self.sorted_vertices.get()
@@ -1439,27 +1466,29 @@
                                                             flattened_cluster=list(members)) 
             clusters.append(set(center_equivalence_cluster.flatten()))
         
         self.execution_time = time() - start_time
         return clusters
     
     def _configuration(self) -> dict:
-        return {}
+        return {
+            "Similarity Threshold" : self.similarity_threshold
+        }
     
     
 class RowColumnClustering(AbstractClustering):
-    """Ιmplements the Row Column Clustering algorithm. For each row and column find their equivalent
+    """Implements the Row Column Clustering algorithm. For each row and column find their equivalent
        column and row respectively corresponding to the smallest similarity. Subsequently, chooses
        either rows or columns dependent on which one has the highest out of the lowest similariities 
        on average.        
     """
 
     _method_name: str = "Row Column Clustering"
     _method_short_name: str = "RCC"
-    _method_info: str = "Ιmplements the Row Column Clustering algorithm," + \
+    _method_info: str = "Implements the Row Column Clustering algorithm," + \
         "In essence, it is a 3/2-approximation to the Maximum Stable Marriage (MSM) problem."
     def __init__(self) -> None:
         super().__init__()
         self.similarity_threshold : float
         
     def process(self, 
                 graph: Graph,
@@ -1581,8 +1610,10 @@
         self.selected_row = [0] * similarity_matrix.shape[1]
         self.row_covered = [False] * similarity_matrix.shape[0]
         self.column_covered = [False] * similarity_matrix.shape[1]
     
         self.columns_from_selected_row = [0] * similarity_matrix.shape[0]    
     
     def _configuration(self) -> dict:
-        return {}
+        return {
+            "Similarity Threshold" : self.similarity_threshold
+        }
```

### Comparing `pyjedai-0.1.6/src/pyjedai/comparison_cleaning.py` & `pyjedai-0.1.7/src/pyjedai/comparison_cleaning.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.1.6/src/pyjedai/datamodel.py` & `pyjedai-0.1.7/src/pyjedai/datamodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,16 +119,18 @@
         self.id_column_name_1 = id_column_name_1
         self.id_column_name_2 = id_column_name_2
         
         self.dataset_name_1 = dataset_name_1
         self.dataset_name_2 = dataset_name_2
         
         # Fill NaN values with empty string
+        self.dataset_1 = self.dataset_1.astype(str)
         self.dataset_1.fillna("", inplace=True)
         if not self.is_dirty_er:
+            self.dataset_2 = self.dataset_2.astype(str)
             self.dataset_2.fillna("", inplace=True)
 
         # Attributes
         if attributes_1 is None:
             if dataset_1.columns.values.tolist():
                 self.attributes_1 = dataset_1.columns.values.tolist()
                 if self.id_column_name_1 in self.attributes_1:
@@ -150,14 +152,15 @@
             else:
                 self.attributes_2: list = attributes_2
 
         # Ground truth data
         self.skip_ground_truth_processing = skip_ground_truth_processing
         if ground_truth is not None and not skip_ground_truth_processing:
             self.ground_truth = ground_truth.astype(str)
+            self.ground_truth.drop_duplicates(inplace=True)
             self._ids_mapping_1: dict
             self._gt_to_ids_reversed_1: dict
             self._ids_mapping_2: dict
             self._gt_to_ids_reversed_2: dict
         else:
             self.ground_truth = None
         
@@ -183,15 +186,15 @@
     
     def _store_pairs(self) -> None:
         """Creates a mapping:
             - pairs_of : ids of first dataset to ids of true matches from second dataset"""
         self.duplicate_of = defaultdict(set)
         
         for _, row in self.ground_truth.iterrows():
-            id1, id2 = (row[0], row[1])
+            id1, id2 = (row.iloc[0], row.iloc[1])
             if id1 in self.duplicate_of: self.duplicate_of[id1].add(id2)
             else: self.duplicate_of[id1] = {id2}
             
     def _are_true_positives(self, id1 : int, id2 : int):
         """Checks if given pair of identifiers represents a duplicate.
            Identifiers must be inorder, first one belonging to the first and the second to the second dataset
 
@@ -248,15 +251,14 @@
     
     def get_real_id_of(self, pyjedai_id: int) -> any:
         if pyjedai_id < self.dataset_limit:
             return self._gt_to_ids_reversed_1[pyjedai_id]
         else:
             return self._gt_to_ids_reversed_2[pyjedai_id]
         
-        
     def print_specs(self) -> None:
         """Dataset report.
         """
         def calculate_memory_usage_of_pandas(dataframe: pd.DataFrame) -> float:
             memory_usage = dataframe.memory_usage(deep=True).sum()
             if memory_usage > 1024**4:
                 memory_usage /= (1024**4)
@@ -271,34 +273,41 @@
                 memory_usage /= (1024)
                 unit = "KB"
             else:
                 unit = "B"
             
             return memory_usage, unit
 
-        print(25*"-", "Data", 25*"-")
+        print('*' * 123)
+        print(' ' * 50, 'Data Report')
+        print('*' * 123)
         print("Type of Entity Resolution: ", "Dirty" if self.is_dirty_er else "Clean-Clean" )
-        print("Dataset-1:")
+        name1 = self.dataset_name_1 if self.dataset_name_1 is not None else "D1"
+        print("Dataset 1 (" + name1 + "):")
         print("\tNumber of entities: ", self.num_of_entities_1)
         print("\tNumber of NaN values: ", self.dataset_1.isnull().sum().sum())
         memory_usage, unit = calculate_memory_usage_of_pandas(self.dataset_1)
         print("\tMemory usage [" + unit + "]: ", "{:.2f}".format(memory_usage))
-        print("\tAttributes: \n\t\t", self.attributes_1)
+        print("\tAttributes:")
+        for attr in self.attributes_1:
+            print("\t\t", attr)
         if not self.is_dirty_er:
-            print("Dataset-2:")
+            name2 = self.dataset_name_2 if self.dataset_name_2 is not None else "D2"
+            print("Dataset 2 (" + name2 + "):")
             print("\tNumber of entities: ", self.num_of_entities_2)
             print("\tNumber of NaN values: ", self.dataset_2.isnull().sum().sum())
             memory_usage, unit = calculate_memory_usage_of_pandas(self.dataset_2)
             print("\tMemory usage [" + unit + "]: ", "{:.2f}".format(memory_usage))
-            print("\tAttributes: \n\t\t", self.attributes_2)
+            print("\tAttributes:")
+            for attr in self.attributes_2:
+                print("\t\t", attr)
         print("\nTotal number of entities: ", self.num_of_entities)
         if self.ground_truth is not None:
             print("Number of matching pairs in ground-truth: ", len(self.ground_truth))
-        print(56*"-", "\n")
-
+        print(u'\u2500' * 123)
     
     # Functions that removes stopwords, punctuation, uni-codes, numbers from the dataset
     def clean_dataset(self, 
                       remove_stopwords: bool = True, 
                       remove_punctuation: bool = True, 
                       remove_numbers:bool = True,
                       remove_unicodes: bool = True) -> None:
```

### Comparing `pyjedai-0.1.6/src/pyjedai/evaluation.py` & `pyjedai-0.1.7/src/pyjedai/evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                 'True Negatives': self.true_negatives,
                 'False Negatives': self.false_negatives
             }
 
         if verbose:
             if configuration:
                 print('*' * 123)
-                print(' ' * 40, 'Μethod: ', configuration['name'])
+                print(' ' * 40, 'Method: ', configuration['name'])
                 print('*' * 123)
                 print(
                     "Method name: " + configuration['name'] +
                     "\nParameters: \n" + ''.join(['\t{0}: {1}\n'.format(k, v) for k, v in configuration['parameters'].items()]) +
                     "Runtime: {:2.4f} seconds".format(configuration['runtime'])
                 )
             else:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyjedai-0.1.6/src/pyjedai/joins.py` & `pyjedai-0.1.7/src/pyjedai/joins.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.1.6/src/pyjedai/logs.py` & `pyjedai-0.1.7/src/pyjedai/logs.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.1.6/src/pyjedai/matching.py` & `pyjedai-0.1.7/src/pyjedai/matching.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,15 +417,15 @@
             raise ValueError("Empty blocks structure")
         self.data = data
         self.pairs = Graph()
         all_blocks = list(blocks.values())
         self._progress_bar = tqdm(total=len(blocks),
                                   desc=self._method_name+" ("+self.metric+ ", " + str(self.tokenizer) + ")",
                                   disable=self.tqdm_disable)
-                
+
         if self.vectorizer is not None:
             self.initialize_vectorizer()
 
         if 'Block' in str(type(all_blocks[0])):
             self._predict_raw_blocks(blocks)
         elif isinstance(all_blocks[0], set):
             self._predict_candidate_pairs(blocks)
@@ -500,23 +500,23 @@
                 e1 = self.data.entities.iloc[entity_id1][attribute].lower()
                 e2 = self.data.entities.iloc[entity_id2][attribute].lower()
 
                 similarity += weight*metrics_mapping[self._metric].get_sim_score(
                     self._tokenizer.tokenize(e1) if self._metric in set_metrics else e1,
                     self._tokenizer.tokenize(e2) if self._metric in set_metrics else e2
                 )
-        if isinstance(self.attributes, list):
+        elif isinstance(self.attributes, list):
             for attribute in self.attributes:
                 e1 = self.data.entities.iloc[entity_id1][attribute].lower()
                 e2 = self.data.entities.iloc[entity_id2][attribute].lower()
                 similarity += metrics_mapping[self._metric].get_sim_score(
                     self._tokenizer.tokenize(e1) if self._metric in set_metrics else e1,
                     self._tokenizer.tokenize(e2) if self._metric in set_metrics else e2
                 )
-                similarity /= len(self.attributes)
+            similarity /= len(self.attributes)
         else:
             # concatenated row string
             e1 = self.data.entities.iloc[entity_id1].str.cat(sep=' ').lower()
             e2 = self.data.entities.iloc[entity_id2].str.cat(sep=' ').lower()
             te1 = self._tokenizer.tokenize(e1) if self._metric in set_metrics else e1
             te2 = self._tokenizer.tokenize(e2) if self._metric in set_metrics else e2
             similarity = metrics_mapping[self._metric].get_sim_score(te1, te2)
```

### Comparing `pyjedai-0.1.6/src/pyjedai/prioritization.py` & `pyjedai-0.1.7/src/pyjedai/prioritization.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.1.6/src/pyjedai/schema/clustering.py` & `pyjedai-0.1.7/src/pyjedai/schema/clustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,15 +271,14 @@
             pairs = self.transform_mapping_to_ids(new_clusters, new_data)            
             global_pairs_dict.update(pairs)
             
         self.execution_time = time.time() - _start_time
         
         return global_pairs_dict
 
-
 class RDFSchemaClustering(AbstractSchemaClustering):
     """Class to provide schema clustering methods
     """
     _method_name = "RDF Schema Clustering"
     _method_info = "Performs pyjedai dirty er workflow for the concatenation of objects per predicate. " + \
                         "For each rdf-triple containing the corresponding predicate, a new set is created. " + \
                             "For each set, a pyjedai dirty er workflow runs and finds the duplicate entities. " + \
@@ -487,15 +486,16 @@
         # free(all)
         print("New datasets: ", len(new_datasets))
         
         if return_clusters:
             return new_datasets
 
         print("Freeing memory")
-        del all_predicates_data, predicates_df, clusters, all_ids, redundant_entities, non_nan_indexes_d1, non_nan_indexes_d2
+        del all_predicates_data, predicates_df, clusters, all_ids, \
+            redundant_entities, non_nan_indexes_d1, non_nan_indexes_d2
 
         if pyjedai_workflow_for_er == None:
             pyjedai_workflow_for_er = self.pyjedai_workflow_for_er_on_subjects()
             # if data.is_dirty_er:
             #     pyjedai_workflow_for_er.best_blocking_workflow_der()
             # else:
             #     pyjedai_workflow_for_er.best_blocking_workflow_ccer()
@@ -513,15 +513,14 @@
 
             print("Dataset 2: ", d2.shape)
             # print(d2.head())
             
             if d1.shape[0] < 2 or (not data.is_dirty_er and d2.shape[0] < 2):
                 continue
 
-            
             subjects_d1 = dict()
             for _, row in tqdm(d1.iterrows(), desc="Creating subjects for dataset 1"):
                 if row['subject'] not in subjects_d1:
                     subjects_d1[row['subject']] = str()
                 subjects_d1[row['subject']] += ' ' + row['object']
             
             subjects_d2 = None
```

### Comparing `pyjedai-0.1.6/src/pyjedai/schema/matching.py` & `pyjedai-0.1.7/src/pyjedai/schema/matching.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.1.6/src/pyjedai/spatial/filtering.py` & `pyjedai-0.1.7/src/pyjedai/spatial/filtering.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.1.6/src/pyjedai/spatial/initialization.py` & `pyjedai-0.1.7/src/pyjedai/spatial/initialization.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.1.6/src/pyjedai/spatial/verification.py` & `pyjedai-0.1.7/src/pyjedai/spatial/verification.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.1.6/src/pyjedai/utils.py` & `pyjedai-0.1.7/src/pyjedai/utils.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.1.6/src/pyjedai/vector_based_blocking.py` & `pyjedai-0.1.7/src/pyjedai/vector_based_blocking.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 import pandas as pd
 from time import time
 from typing import List, Tuple
 from math import sqrt
 import faiss
 import platform
 RUNNING_OS = platform.system()
-if RUNNING_OS != "Windows":
-    import scann
-    import falconn
+
 import gensim.downloader as api
 import networkx as nx
 import numpy as np
 import torch
 import transformers
 from sentence_transformers import SentenceTransformer
 from tqdm.autonotebook import tqdm
@@ -64,15 +62,15 @@
         'sminilm' : 'all-MiniLM-L12-v2',
         'sent_glove' : 'average_word_embeddings_glove.6B.300d'
     }
 
     def __init__(
             self,
             vectorizer: str,
-            similarity_search: str
+            similarity_search: str = 'faiss'
     ) -> None:
         super().__init__()
         self.vectorizer, self.similarity_search = vectorizer, similarity_search
         self.embeddings: np.array
         self.vectors_1: np.array
         self.vectors_2: np.array = None
         self.vector_size: int
@@ -103,15 +101,16 @@
                      tqdm_disable: bool = False,
                      save_embeddings: bool = True,
                      load_embeddings_if_exist: bool = False,
                      load_path_d1: str = None,
                      load_path_d2: str = None,
                      with_entity_matching: bool = False,
                      input_cleaned_blocks: dict = None,
-                     similarity_distance: str = 'cosine'
+                     similarity_distance: str = 'cosine',
+                     verbose: bool = False
     ) -> any:
         """Main method of the vector based approach. Contains two steps. First an embedding method. \
             And afterwards a similarity search upon the vectors created in the previous step.
             Pre-trained schemes are used for the embedding process.
 
         Args:
             data (Data): dataset from datamodel
@@ -132,17 +131,21 @@
             AttributeError: Vectorizer check
             AttributeError: Similarity Search method check.
 
         Returns:
             dict: Entity ids to sets of top-K candidate ids. OR
             Tuple(np.array, np.array): vectors from d1 and vectors from d2
         """
+        if self.similarity_search != 'faiss':
+            raise AttributeError("Only FAISS is available for now.")
+        
         print('Building blocks via Embeddings-NN Block Building [' + self.vectorizer + ', ' + self.similarity_search + ']')
         _start_time = time()
         self.blocks = dict()
+        self.verbose = verbose
         self.with_entity_matching = with_entity_matching
         self.save_embeddings, self.load_embeddings_if_exist = save_embeddings, load_embeddings_if_exist
         self.max_word_embeddings_size = max_word_embeddings_size
         self.similarity_distance = similarity_distance
         self.data, self.attributes_1, self.attributes_2, self.vector_size, self.num_of_clusters, self.top_k, self.input_cleaned_blocks \
             = data, attributes_1, attributes_2, vector_size, num_of_clusters, top_k, input_cleaned_blocks
         self.load_path_d1, self.load_path_d2 = load_path_d1, load_path_d2
@@ -184,82 +187,85 @@
         
         if self.with_entity_matching:
             self.graph = nx.Graph()
         
         self._d1_loaded : bool = False
         self._d2_loaded : bool = False
         if load_embeddings_if_exist:
+            if verbose:
                 print("Loading embeddings from file...")
-                if(self.load_path_d1 is not None):
-                    p1 = self.load_path_d1
-                else:
-                    p1 = os.path.join(EMBEDDINGS_DIR, self.vectorizer + '_' + (self.data.dataset_name_1 \
-                                                        if self.data.dataset_name_1 is not None else "d1") +'.npy')
+            if(self.load_path_d1 is not None):
+                p1 = self.load_path_d1
+            else:
+                p1 = os.path.join(EMBEDDINGS_DIR, self.vectorizer + '_' + (self.data.dataset_name_1 \
+                                                    if self.data.dataset_name_1 is not None else "d1") +'.npy')
+            if verbose:
                 print("Attempting to load D1 embeddings...")
-                if os.path.exists(p1):
-                    self.vectors_1 = vectors_1 = np.load(p1)
-                    self.vectors_1 = vectors_1 = vectors_1[self._d1_valid_indices]
-                    self._progress_bar.update(data.num_of_entities_1)
-                    self._d1_loaded = True
+            if os.path.exists(p1):
+                self.vectors_1 = vectors_1 = np.load(p1)
+                self.vectors_1 = vectors_1 = vectors_1[self._d1_valid_indices]
+                self._progress_bar.update(data.num_of_entities_1)
+                self._d1_loaded = True
+                if verbose:
                     print(f"{p1} -> Loaded Successfully")
-                else:
-                    print("Embeddings not found. Creating new ones.")
-                
+            else:
+                if verbose:
+                    print("Embeddings not found for D1. Creating new ones.")
+            
+            if not data.is_dirty_er:
                 if(self.load_path_d2 is not None):
                     p2 = self.load_path_d2
                 else:
                     p2 = os.path.join(EMBEDDINGS_DIR, self.vectorizer + '_' + (self.data.dataset_name_2 \
                                                         if self.data.dataset_name_2 is not None else "d2") +'.npy')    
-                print("Attempting to load D2 embeddings...")
+                if verbose: print("Attempting to load D2 embeddings...")
                 if os.path.exists(p2):
                     self.vectors_2 = vectors_2 = np.load(p2)
                     self.vectors_2 = vectors_2 = vectors_2[self._d2_valid_indices]
                     self._progress_bar.update(data.num_of_entities_2)
                     self._d2_loaded = True
-                    print(f"{p2} -> Loaded Successfully")
+                    if verbose: print(f"{p2} -> Loaded Successfully")
                 else:
-                    print("Embeddings not found. Creating new ones.")
+                    if verbose: print("Embeddings not found for D2. Creating new ones.")
         if not self._d1_loaded or not self._d2_loaded:
             if self.vectorizer in ['word2vec', 'fasttext', 'doc2vec', 'glove']:
                 self.vectors_1, self.vectors_2 = self._create_gensim_embeddings()
             elif self.vectorizer in ['bert', 'distilbert', 'roberta', 'xlnet', 'albert']:
                 self.vectors_1, self.vectors_2 = self._create_pretrained_word_embeddings()
             elif self.vectorizer in ['smpnet', 'st5', 'sent_glove', 'sdistilroberta', 'sminilm']:
                 self.vectors_1, self.vectors_2 = self._create_pretrained_sentence_embeddings()
             else:
                 raise AttributeError("Not available vectorizer")
             
         if save_embeddings:
-            print("Saving embeddings...")
+            if verbose: print("Saving embeddings...")
             
             if self._applied_to_subset:
-                print("Cannot save embeddings, subset embeddings storing not supported.")
+                if verbose: print("Cannot save embeddings, subset embeddings storing not supported.")
             else:
                 if not self._d1_loaded:
                     p1 = os.path.join(EMBEDDINGS_DIR, self.vectorizer + '_' + (self.data.dataset_name_1 \
                                                             if self.data.dataset_name_1 is not None else "d1") +'.npy')
-                    print("Saving file: ", p1)
+                    if verbose: print("Saving file: ", p1)
                     np.save(p1, self.vectors_1)
                 
-                if not self._d2_loaded:
+                if not data.is_dirty_er and not self._d2_loaded:
                     p2 = os.path.join(EMBEDDINGS_DIR, self.vectorizer + '_' + (self.data.dataset_name_2 \
                                                             if self.data.dataset_name_2 is not None else "d2") +'.npy')
-                    print("Saving file: ", p2)
+                    if verbose: print("Saving file: ", p2)
                     np.save(p2, self.vectors_2)
 
         if return_vectors:
             return (self.vectors_1, _) if data.is_dirty_er else (self.vectors_1, self.vectors_2)
 
         if self.similarity_search == 'faiss':
+            if verbose: print("Starting similarity search with FAISS...")
             self._faiss_metric_type = faiss.METRIC_L2
             self._similarity_search_with_FAISS()
-        elif self.similarity_search == 'falconn':
-            self._similarity_search_with_FALCONN()
-        elif self.similarity_search == 'scann':
-            self._similarity_search_with_SCANN()
+            if verbose: print("Similarity search with FAISS is done.")
         else:
             raise AttributeError("Not available method")
         self._progress_bar.close()        
         self.execution_time = time() - _start_time
         
         if self.with_entity_matching:
             return self.blocks, self.graph
@@ -368,48 +374,58 @@
                 self._progress_bar.update(1)
             self.vector_size = len(vectors_2[0])
             vectors_2 = np.vstack(vectors_2).astype('float32')
             
         return vectors_1, vectors_2 
 
     def _similarity_search_with_FAISS(self):
+        if self.verbose:
+            print("Creating index...")
         index = faiss.IndexFlatL2(self.vectors_1.shape[1])
         
         if self.similarity_distance == 'cosine' or self.similarity_distance == 'cosine_without_normalization':
             index.metric_type = faiss.METRIC_INNER_PRODUCT
         elif self.similarity_distance == 'euclidean':
             index.metric_type = faiss.METRIC_L2
         else:
             raise ValueError("Invalid similarity distance: ", self.similarity_distance)
 
         if self.similarity_distance == 'cosine':
             faiss.normalize_L2(self.vectors_1)
             if not self.data.is_dirty_er: faiss.normalize_L2(self.vectors_2)
-            
+        
+        if self.verbose:
+            print("Training index...")
         index.train(self.vectors_1)  # train on the vectors of dataset 1
 
+
         if self.similarity_distance == 'cosine':
             faiss.normalize_L2(self.vectors_1)
             if not self.data.is_dirty_er: faiss.normalize_L2(self.vectors_2)
 
+        if self.verbose:
+            print("Adding vectors to index...")
         index.add(self.vectors_1)   # add the vectors and update the index
 
         if self.similarity_distance == 'cosine':
             faiss.normalize_L2(self.vectors_1)
             if not self.data.is_dirty_er: faiss.normalize_L2(self.vectors_2)
-        
-        self.distances, self.neighbors = index.search(self.vectors_1 if self.data.is_dirty_er else self.vectors_2,
-                                    self.top_k)
+
+        if self.verbose:
+            print("Searching for neighbors...")
+        self.distances, self.neighbors = index.search(self.vectors_1 if self.data.is_dirty_er else self.vectors_2, self.top_k)
 
         if self.similarity_distance == 'euclidean':
             self.distances = 1/(1 + self.distances)
 
         self.blocks = dict()
-        
-        for _entity in range(0, self.neighbors.shape[0]):
+        if self.verbose:
+            print("Building blocks...")
+        print("disable", not self.verbose)
+        for _entity in tqdm(range(0, self.neighbors.shape[0]), desc="Building blocks", disable=not self.verbose):
             
             _entity_id = self._si.d1_retained_ids[_entity] if self.data.is_dirty_er else self._si.d2_retained_ids[_entity]
             
             # if _entity_id not in self.blocks:
             #     self.blocks[_entity_id] = set()
             
             for _neighbor_index, _neighbor in enumerate(self.neighbors[_entity]):
@@ -424,111 +440,14 @@
 
                 self.blocks[_neighbor_id].add(_entity_id)
                 # self.blocks[_entity_id].add(_neighbor_id)
                 
                 if self.with_entity_matching:
                     self.graph.add_edge(_entity_id, _neighbor_id, weight=self.distances[_entity][_neighbor_index])
 
-    def _similarity_search_with_FALCONN(self):
-        _falconn_parameters = falconn.LSHConstructionParameters()
-        _falconn_parameters.distance_function = falconn.DistanceFunction.NegativeInnerProduct \
-                                                if (self.similarity_distance == 'cosine') \
-                                                else falconn.DistanceFunction.EuclideanSquared
-                                                
-        _normalized_source_vectors = self.vectors_1 / np.linalg.norm(self.vectors_1, axis=1)[:, np.newaxis]
-        _normalized_target_vectors = _normalized_source_vectors \
-                                    if self.data.is_dirty_er \
-                                    else self.vectors_2 / np.linalg.norm(self.vectors_2, axis=1)[:, np.newaxis]                                 
-              
-              
-        _normalized_source_vectors = - _normalized_source_vectors
-        _normalized_target_vectors = -_normalized_target_vectors      
-                                
-        _falconn_parameters.dimension = _normalized_source_vectors.shape[1]
-        _falconn_parameters.lsh_family = falconn.LSHFamily.CrossPolytope
-        _falconn_parameters.storage_hash_table = falconn.StorageHashTable.FlatHashTable
-        _falconn_parameters.num_setup_threads = 0     
-        _falconn_parameters.l = 50
-        _falconn_parameters.num_rotations = 1
-        falconn.compute_number_of_hash_functions(int(log(_normalized_source_vectors.shape[0],2)), _falconn_parameters)
-        _normalized_source_vectors = _normalized_source_vectors.astype(np.float32)
-        _normalized_target_vectors = _normalized_target_vectors.astype(np.float32)
-        
-        index = falconn.LSHIndex(_falconn_parameters)
-        index.setup(_normalized_source_vectors)
-        query_object = index.construct_query_object()
-                
-        self.blocks = dict()
-        
-        for _taget_entity_index, _normalized_target_vector in enumerate(_normalized_target_vectors):            
-            _target_entity_id = self._si.d1_retained_ids[_taget_entity_index] \
-                                if self.data.is_dirty_er \
-                                else self._si.d2_retained_ids[_taget_entity_index]
-            _source_entity_ids = query_object.find_k_nearest_neighbors(query=_normalized_target_vector, k=self.top_k)
-            # if _target_entity_id not in self.blocks:
-            #     self.blocks[_target_entity_id] = set()
-            
-            for id in _source_entity_ids:
-                
-                _source_entity_id = self._si.d1_retained_ids[id]
-                
-                if _source_entity_id not in self.blocks:
-                    self.blocks[_source_entity_id] = set()
-
-                self.blocks[_source_entity_id].add(_target_entity_id)
-                
-                if self.with_entity_matching:
-                    self.graph.add_edge(_source_entity_id, _target_entity_id)
-
-    def _similarity_search_with_SCANN(self):
-        
-        if RUNNING_OS == "Windows":
-            raise NotImplementedError("SCANN is not implemented yet for Windows.")
-        
-        _scann_distance_metric : str = "dot_product" if (self.similarity_distance == 'cosine') else "squared_l2"
-        _normalized_source_vectors = self.vectors_1 / np.linalg.norm(self.vectors_1, axis=1)[:, np.newaxis]
-        _normalized_target_vectors = _normalized_source_vectors \
-                                    if self.data.is_dirty_er \
-                                    else self.vectors_2 / np.linalg.norm(self.vectors_2, axis=1)[:, np.newaxis]
-        _k : int = int(sqrt(self.data.num_of_entities_1))
-        
-        searcher = scann.scann_ops_pybind.builder(_normalized_source_vectors, self.top_k, _scann_distance_metric) \
-                        .tree(num_leaves=_k,
-                              num_leaves_to_search=int(_k),
-                              training_sample_size=int(self.data.num_of_entities_1/2)) \
-                        .score_ah(2, anisotropic_quantization_threshold=0.2) \
-                        .reorder(int(_k)) \
-                        .build()
-
-        self.neighbors, self.distances = searcher.search_batched(_normalized_target_vectors, final_num_neighbors=self.top_k)
-
-        if self.similarity_distance == 'euclidean':
-            self.distances = 1/(1 + np.sqrt(self.distances))
-
-        self.blocks = dict()
-        
-        for _entity in range(0, self.neighbors.shape[0]):
-            
-            _entity_id = self._si.d1_retained_ids[_entity] if self.data.is_dirty_er else self._si.d2_retained_ids[_entity]       
-            
-            for _neighbor_index, _neighbor in enumerate(self.neighbors[_entity]):
-
-                if _neighbor == -1:
-                    continue
-                
-                _neighbor_id = self._si.d1_retained_ids[_neighbor]
-                
-                if _neighbor_id not in self.blocks:
-                    self.blocks[_neighbor_id] = set()
-
-                self.blocks[_neighbor_id].add(_entity_id)
-                                
-                if self.with_entity_matching:
-                    self.graph.add_edge(_entity_id, _neighbor_id, weight=self.distances[_entity][_neighbor_index])
-
     def _create_vector(self, tokens: List[str], vocabulary) -> np.array:
         num_of_tokens = 0
         vector = np.zeros(self.vector_size)
         for token in tokens.split():
             if token in vocabulary:
                 vector += vocabulary[token]
                 num_of_tokens += 1
@@ -584,22 +503,16 @@
             "Vector size": self.vector_size
         }
     
     def stats(self) -> None:
         print("Statistics:")
         if self.similarity_search == 'faiss':
             print(" FAISS:" +
-                # "\n\tNumber of entries in each list:  " + str(self._faiss_num_lists) + 
                 "\n\tIndices shape returned after search: " + str(self.neighbors.shape)
             )
-        elif self.similarity_search == 'falconn':           
-            pass
-        elif self.similarity_search == 'scann'  and LINUX_ENV:
-            pass
-        
         print(u'\u2500' * 123)
         
     
     def export_to_df(self, prediction: dict) -> pd.DataFrame:
         """creates a dataframe with the predicted pairs
 
         Args:
```

### Comparing `pyjedai-0.1.6/src/pyjedai/visualization.py` & `pyjedai-0.1.7/src/pyjedai/visualization.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.1.6/src/pyjedai/workflow.py` & `pyjedai-0.1.7/src/pyjedai/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from itertools import count
 from time import time
 from typing import Callable, List, Tuple
 
 import matplotlib.pyplot as plt
 import os
 import json
-import optuna
 import pandas as pd
 from networkx import Graph
 from tqdm.autonotebook import tqdm
 
 from .datamodel import Data
 from .evaluation import Evaluation
 from .block_building import StandardBlocking
@@ -518,114 +517,14 @@
         axs[1, 0].bar(workflow_df['Name'], workflow_df['F1'], color='orange')
         axs[1, 1].bar(workflow_df['Name'], workflow_df['Runtime (sec)'], color='r')
     fig.autofmt_xdate()
     plt.show()
 
     return workflow_df
 
-class OptimizeWorkflow:
-    """Optuna Framework for GridSearch/RandomSearch/Prunning in a given pyjedai workflow.
-    """
-
-    _id = count()
-
-    def __init__(
-            self,
-            block_building: Callable, # Mandatory: one method
-            entity_matching: Callable, # Mandatory: one method
-            block_cleaning: List[Callable] = None, # Optional: multiple methods
-            comparison_cleaning: List[Callable] = None, # Optional: multiple methods
-            clustering: Callable = None, # Optional: One method
-            joins: Callable = None, # Optional: One method
-            name: str = None
-    ) -> None:
-        self.block_cleaning, self.block_building, self.comparison_cleaning, \
-            self.clustering, self.joins, self.entity_matching = \
-            block_cleaning, block_building, comparison_cleaning, clustering, joins, entity_matching
-        self.f1: float
-        self.recall: float
-        self.precision: float
-        self.runtime: float
-        self.configurations: float
-        self.workflow_exec_time: float
-        self._id: int = next(self._id)
-        self.name: str = name if name else "OptWorkflow-" + str(self._id)
-        self._workflow_bar: tqdm
-
-    def objective(self, target_score: str = 'f1') -> any:
-        """Optuna objective function
-
-            Returns:
-                 One or more from F1,Recall,Precision
-        """
-        pass
-        # if target_score  == 'f1':
-        #     return f1
-        # elif target_score  == 'recall':
-        #     return recall
-        # else:
-        #     return precision
-
-    def run(
-            self,
-            data: Data,
-            num_of_trials = 30,
-            pruner: optuna.pruners = optuna.pruners.NopPruner,
-            sampler: optuna.samplers = optuna.samplers.BaseSampler,
-            study_name = "pyjedai_study",
-            storage_name = "pyjedai_storage_trials",
-            target_score = "f1",
-            load_if_exists=True,
-            verbose=False,
-            tqdm_disable=False,
-            workflow_tqdm_enable=False,
-            optuna_tqdm_enable=True
-    ) -> pd.DataFrame:
-        """Executes the experiments based on a workflow
-
-        Args:
-            data (Data): _description_
-            num_of_trials (int, optional): _description_. Defaults to 30.
-            pruner (optuna.pruners, optional): _description_. Defaults to optuna.pruners.NopPruner.
-            sampler (optuna.samplers, optional): _description_. Defaults to optuna.samplers.BaseSampler.
-            study_name (str, optional): _description_. Defaults to "pyjedai_study".
-            storage_name (str, optional): _description_. Defaults to "pyjedai_storage_trials".
-            target_score (str, optional): _description_. Defaults to "f1".
-            load_if_exists (bool, optional): _description_. Defaults to True.
-            verbose (bool, optional): _description_. Defaults to False.
-            tqdm_disable (bool, optional): _description_. Defaults to False.
-            workflow_tqdm_enable (bool, optional): _description_. Defaults to False.
-            optuna_tqdm_enable (bool, optional): _description_. Defaults to True.
-
-        Returns:
-            pd.DataFrame: _description_
-        """
-        study = optuna.create_study(
-            directions=["maximize"],
-            study_name=study_name,
-            storage=storage_name,
-            load_if_exists=load_if_exists
-        )
-        print("Optuna trials starting")
-        study.optimize(
-            self.objective, 
-            n_trials=num_of_trials, 
-            show_progress_bar=optuna_tqdm_enable
-        )
-        print("Optuna trials finished")
-
-    def visualize(self, with_plotly=True):
-        pass
-    
-    def get_best_trial(self):
-        pass
-    
-    def to_df():
-        pass
-
 class BlockingBasedWorkFlow(PYJEDAIWorkFlow):
     """Blocking-based workflow.
     """
 
     def __init__(
             self,
             block_building: dict = None,
```

### Comparing `pyjedai-0.1.6/src/pyjedai.egg-info/PKG-INFO` & `pyjedai-0.1.7/src/pyjedai.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 6a65  : 2.1.Name: pyje
 00000020: 6461 690a 5665 7273 696f 6e3a 2030 2e31  dai.Version: 0.1
-00000030: 2e36 0a53 756d 6d61 7279 3a20 416e 206f  .6.Summary: An o
+00000030: 2e37 0a53 756d 6d61 7279 3a20 416e 206f  .7.Summary: An o
 00000040: 7065 6e2d 736f 7572 6365 206c 6962 7261  pen-source libra
 00000050: 7279 2074 6861 7420 6275 696c 6473 2070  ry that builds p
 00000060: 6f77 6572 6675 6c20 656e 642d 746f 2d65  owerful end-to-e
 00000070: 6e64 2045 6e74 6974 7920 5265 736f 6c75  nd Entity Resolu
 00000080: 7469 6f6e 2077 6f72 6b66 6c6f 7773 2e0a  tion workflows..
 00000090: 4175 7468 6f72 2d65 6d61 696c 3a20 4b6f  Author-email: Ko
 000000a0: 6e73 7461 6e74 696e 6f73 204e 696b 6f6c  nstantinos Nikol
@@ -100,561 +100,561 @@
 00000630: 4d6f 6475 6c65 730a 5265 7175 6972 6573  Modules.Requires
 00000640: 2d50 7974 686f 6e3a 203e 3d33 2e38 0a44  -Python: >=3.8.D
 00000650: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
 00000660: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
 00000670: 726b 646f 776e 0a4c 6963 656e 7365 2d46  rkdown.License-F
 00000680: 696c 653a 204c 4943 454e 5345 0a52 6571  ile: LICENSE.Req
 00000690: 7569 7265 732d 4469 7374 3a20 6765 6e73  uires-Dist: gens
-000006a0: 696d 3e3d 342e 322e 300a 5265 7175 6972  im>=4.2.0.Requir
-000006b0: 6573 2d44 6973 743a 206d 6174 706c 6f74  es-Dist: matplot
-000006c0: 6c69 623e 3d33 2e31 2e33 0a52 6571 7569  lib>=3.1.3.Requi
-000006d0: 7265 732d 4469 7374 3a20 6d61 7470 6c6f  res-Dist: matplo
-000006e0: 746c 6962 2d69 6e6c 696e 653e 3d30 2e31  tlib-inline>=0.1
-000006f0: 2e33 0a52 6571 7569 7265 732d 4469 7374  .3.Requires-Dist
-00000700: 3a20 6e65 7477 6f72 6b78 3e3d 322e 330a  : networkx>=2.3.
-00000710: 5265 7175 6972 6573 2d44 6973 743a 206e  Requires-Dist: n
-00000720: 6c74 6b3e 3d33 2e37 0a52 6571 7569 7265  ltk>=3.7.Require
-00000730: 732d 4469 7374 3a20 6e75 6d70 793e 3d31  s-Dist: numpy>=1
-00000740: 2e32 310a 5265 7175 6972 6573 2d44 6973  .21.Requires-Dis
-00000750: 743a 2070 616e 6461 733e 3d30 2e32 352e  t: pandas>=0.25.
-00000760: 330a 5265 7175 6972 6573 2d44 6973 743a  3.Requires-Dist:
-00000770: 2070 616e 6461 732d 7072 6f66 696c 696e   pandas-profilin
-00000780: 673e 3d33 2e32 0a52 6571 7569 7265 732d  g>=3.2.Requires-
-00000790: 4469 7374 3a20 7061 6e64 6f63 6669 6c74  Dist: pandocfilt
-000007a0: 6572 733e 3d31 2e35 0a52 6571 7569 7265  ers>=1.5.Require
-000007b0: 732d 4469 7374 3a20 5079 5941 4d4c 3e3d  s-Dist: PyYAML>=
-000007c0: 362e 300a 5265 7175 6972 6573 2d44 6973  6.0.Requires-Dis
-000007d0: 743a 2072 6466 6c69 623e 3d36 2e31 2e31  t: rdflib>=6.1.1
-000007e0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000007f0: 7264 6670 616e 6461 733e 3d31 2e31 2e35  rdfpandas>=1.1.5
-00000800: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000810: 7265 6765 783e 3d32 3032 322e 362e 320a  regex>=2022.6.2.
-00000820: 5265 7175 6972 6573 2d44 6973 743a 2073  Requires-Dist: s
-00000830: 6369 7079 3e3d 312e 370a 5265 7175 6972  cipy>=1.7.Requir
-00000840: 6573 2d44 6973 743a 2073 6561 626f 726e  es-Dist: seaborn
-00000850: 3e3d 302e 3131 0a52 6571 7569 7265 732d  >=0.11.Requires-
-00000860: 4469 7374 3a20 7374 7273 696d 3e3d 302e  Dist: strsim>=0.
-00000870: 302e 330a 5265 7175 6972 6573 2d44 6973  0.3.Requires-Dis
-00000880: 743a 2073 7472 7369 6d70 793e 3d30 2e32  t: strsimpy>=0.2
-00000890: 2e31 0a52 6571 7569 7265 732d 4469 7374  .1.Requires-Dist
-000008a0: 3a20 7471 646d 3e3d 342e 3634 0a52 6571  : tqdm>=4.64.Req
-000008b0: 7569 7265 732d 4469 7374 3a20 7472 616e  uires-Dist: tran
-000008c0: 7366 6f72 6d65 7273 3e3d 342e 3231 0a52  sformers>=4.21.R
-000008d0: 6571 7569 7265 732d 4469 7374 3a20 7365  equires-Dist: se
-000008e0: 6e74 656e 6365 2d74 7261 6e73 666f 726d  ntence-transform
-000008f0: 6572 733e 3d32 2e32 0a52 6571 7569 7265  ers>=2.2.Require
-00000900: 732d 4469 7374 3a20 6661 6973 732d 6370  s-Dist: faiss-cp
-00000910: 753e 3d31 2e37 0a52 6571 7569 7265 732d  u>=1.7.Requires-
-00000920: 4469 7374 3a20 6f70 7475 6e61 3e3d 332e  Dist: optuna>=3.
-00000930: 300a 5265 7175 6972 6573 2d44 6973 743a  0.Requires-Dist:
-00000940: 2074 6f6d 6c69 3b20 7079 7468 6f6e 5f76   tomli; python_v
-00000950: 6572 7369 6f6e 203c 2022 332e 3131 220a  ersion < "3.11".
-00000960: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
-00000970: 792d 7374 7269 6e67 6d61 7463 6869 6e67  y-stringmatching
-00000980: 3e3d 302e 340a 5265 7175 6972 6573 2d44  >=0.4.Requires-D
-00000990: 6973 743a 2076 616c 656e 7469 6e65 3e3d  ist: valentine>=
-000009a0: 302e 313b 2070 7974 686f 6e5f 7665 7273  0.1; python_vers
-000009b0: 696f 6e20 3e20 2233 2e37 220a 5265 7175  ion > "3.7".Requ
-000009c0: 6972 6573 2d44 6973 743a 206f 7264 6572  ires-Dist: order
-000009d0: 6564 2d73 6574 3e3d 342e 300a 5265 7175  ed-set>=4.0.Requ
-000009e0: 6972 6573 2d44 6973 743a 2070 6c6f 746c  ires-Dist: plotl
-000009f0: 793e 3d35 2e31 362e 300a 5265 7175 6972  y>=5.16.0.Requir
-00000a00: 6573 2d44 6973 743a 2073 6861 7065 6c79  es-Dist: shapely
-00000a10: 3e3d 322e 300a 5265 7175 6972 6573 2d44  >=2.0.Requires-D
-00000a20: 6973 743a 2073 6361 6e6e 3b20 706c 6174  ist: scann; plat
-00000a30: 666f 726d 5f73 7973 7465 6d20 3d3d 2022  form_system == "
-00000a40: 4c69 6e75 7822 0a52 6571 7569 7265 732d  Linux".Requires-
-00000a50: 4469 7374 3a20 6661 6c63 6f6e 6e3b 2070  Dist: falconn; p
-00000a60: 6c61 7466 6f72 6d5f 7379 7374 656d 203d  latform_system =
-00000a70: 3d20 224c 696e 7578 220a 5072 6f76 6964  = "Linux".Provid
-00000a80: 6573 2d45 7874 7261 3a20 6465 760a 5265  es-Extra: dev.Re
-00000a90: 7175 6972 6573 2d44 6973 743a 2070 6970  quires-Dist: pip
-00000aa0: 2d74 6f6f 6c73 3b20 6578 7472 6120 3d3d  -tools; extra ==
-00000ab0: 2022 6465 7622 0a52 6571 7569 7265 732d   "dev".Requires-
-00000ac0: 4469 7374 3a20 7079 7465 7374 3b20 6578  Dist: pytest; ex
-00000ad0: 7472 6120 3d3d 2022 6465 7622 0a0a 3c64  tra == "dev"..<d
-00000ae0: 6976 2061 6c69 676e 3d22 6365 6e74 6572  iv align="center
-00000af0: 223e 0a20 2020 203c 6272 3e0a 2020 2020  ">.    <br>.    
-00000b00: 3c69 6d67 2061 6c69 676e 3d22 6365 6e74  <img align="cent
-00000b10: 6572 2220 7372 633d 2268 7474 7073 3a2f  er" src="https:/
-00000b20: 2f67 6974 6875 622e 636f 6d2f 4149 2d74  /github.com/AI-t
-00000b30: 6561 6d2d 556f 412f 7079 4a65 6441 492f  eam-UoA/pyJedAI/
-00000b40: 626c 6f62 2f6d 6169 6e2f 646f 6373 2f69  blob/main/docs/i
-00000b50: 6d67 2f70 796a 6564 6169 2e6c 6f67 6f2e  mg/pyjedai.logo.
-00000b60: 6472 6177 696f 2e70 6e67 3f72 6177 3d74  drawio.png?raw=t
-00000b70: 7275 6522 2061 6c74 3d22 7079 4a65 6441  rue" alt="pyJedA
-00000b80: 4922 2077 6964 7468 3d22 3430 3022 2f3e  I" width="400"/>
-00000b90: 0a3c 2f64 6976 3e0a 3c62 723e 0a3c 6272  .</div>.<br>.<br
-00000ba0: 3e0a 3c64 6976 2061 6c69 676e 3d22 6365  >.<div align="ce
-00000bb0: 6e74 6572 223e 0a41 6e20 6f70 656e 2d73  nter">.An open-s
-00000bc0: 6f75 7263 6520 6c69 6272 6172 7920 7468  ource library th
-00000bd0: 6174 206c 6576 6572 6167 6573 2050 7974  at leverages Pyt
-00000be0: 686f 6ee2 8099 7320 6461 7461 2073 6369  hon...s data sci
-00000bf0: 656e 6365 2065 636f 7379 7374 656d 2074  ence ecosystem t
-00000c00: 6f20 6275 696c 6420 3c62 723e 2070 6f77  o build <br> pow
-00000c10: 6572 6675 6c20 656e 642d 746f 2d65 6e64  erful end-to-end
-00000c20: 2045 6e74 6974 7920 5265 736f 6c75 7469   Entity Resoluti
-00000c30: 6f6e 2077 6f72 6b66 6c6f 7773 2e0a 3c2f  on workflows..</
-00000c40: 6469 763e 0a0a 0a2d 2d2d 0a0a 0a23 204f  div>...---...# O
-00000c50: 7665 7276 6965 770a 0a70 794a 6564 4149  verview..pyJedAI
-00000c60: 2069 7320 6120 7079 7468 6f6e 2066 7261   is a python fra
-00000c70: 6d65 776f 726b 2c20 6169 6d69 6e67 2074  mework, aiming t
-00000c80: 6f20 6f66 6665 7220 6578 7065 7274 7320  o offer experts 
-00000c90: 616e 6420 6e6f 7669 6365 2075 7365 7273  and novice users
-00000ca0: 2c20 726f 6275 7374 2061 6e64 2066 6173  , robust and fas
-00000cb0: 7420 736f 6c75 7469 6f6e 7320 666f 7220  t solutions for 
-00000cc0: 6d75 6c74 6970 6c65 2074 7970 6573 206f  multiple types o
-00000cd0: 6620 456e 7469 7479 2052 6573 6f6c 7574  f Entity Resolut
-00000ce0: 696f 6e20 7072 6f62 6c65 6d73 2e20 4974  ion problems. It
-00000cf0: 2069 7320 6275 696c 6465 6420 7573 696e   is builded usin
-00000d00: 6720 7374 6174 652d 6f66 2d74 6865 2d61  g state-of-the-a
-00000d10: 7274 2070 7974 686f 6e20 6672 616d 6577  rt python framew
-00000d20: 6f72 6b73 2e20 7079 4a65 6441 4920 636f  orks. pyJedAI co
-00000d30: 6e73 7469 7475 7465 7320 7468 6520 736f  nstitutes the so
-00000d40: 6c65 206f 7065 6e2d 736f 7572 6365 204c  le open-source L
-00000d50: 696e 6b20 4469 7363 6f76 6572 7920 746f  ink Discovery to
-00000d60: 6f6c 2074 6861 7420 6973 2063 6170 6162  ol that is capab
-00000d70: 6c65 206f 6620 6578 706c 6f69 7469 6e67  le of exploiting
-00000d80: 2074 6865 206c 6174 6573 7420 6272 6561   the latest brea
-00000d90: 6b74 6872 6f75 6768 7320 696e 2044 6565  kthroughs in Dee
-00000da0: 7020 4c65 6172 6e69 6e67 2061 6e64 204e  p Learning and N
-00000db0: 4c50 2074 6563 686e 6971 7565 732c 2077  LP techniques, w
-00000dc0: 6869 6368 2061 7265 2070 7562 6c69 636c  hich are publicl
-00000dd0: 7920 6176 6169 6c61 626c 6520 7468 726f  y available thro
-00000de0: 7567 6820 7468 6520 5079 7468 6f6e 2064  ugh the Python d
-00000df0: 6174 6120 7363 6965 6e63 6520 6563 6f73  ata science ecos
-00000e00: 7973 7465 6d2e 2054 6869 7320 6170 706c  ystem. This appl
-00000e10: 6965 7320 746f 2062 6f74 6820 626c 6f63  ies to both bloc
-00000e20: 6b69 6e67 2061 6e64 206d 6174 6368 696e  king and matchin
-00000e30: 672c 2074 6875 7320 656e 7375 7269 6e67  g, thus ensuring
-00000e40: 2068 6967 6820 7469 6d65 2065 6666 6963   high time effic
-00000e50: 6965 6e63 792c 2068 6967 6820 7363 616c  iency, high scal
-00000e60: 6162 696c 6974 7920 6173 2077 656c 6c20  ability as well 
-00000e70: 6173 2068 6967 6820 6566 6665 6374 6976  as high effectiv
-00000e80: 656e 6573 732c 2077 6974 686f 7574 2072  eness, without r
-00000e90: 6571 7569 7269 6e67 2061 6e79 206c 6162  equiring any lab
-00000ea0: 656c 6c65 6420 696e 7374 616e 6365 7320  elled instances 
-00000eb0: 6672 6f6d 2074 6865 2075 7365 722e 0a0a  from the user...
-00000ec0: 2323 2320 4b65 792d 4665 6174 7572 6573  ### Key-Features
-00000ed0: 0a0a 2d20 496e 7075 7420 6461 7461 2d74  ..- Input data-t
-00000ee0: 7970 6520 696e 6465 7065 6e64 656e 742e  ype independent.
-00000ef0: 2042 6f74 6820 7374 7275 6374 7572 6564   Both structured
-00000f00: 2061 6e64 2073 656d 692d 7374 7275 6374   and semi-struct
-00000f10: 7572 6564 2064 6174 6120 6361 6e20 6265  ured data can be
-00000f20: 2070 726f 6365 7373 6564 2e0a 2d20 5661   processed..- Va
-00000f30: 7269 6f75 7320 696d 706c 656d 656e 7465  rious implemente
-00000f40: 6420 616c 676f 7269 7468 6d73 2e0a 2d20  d algorithms..- 
-00000f50: 4561 7379 2d74 6f2d 7573 652e 0a2d 2055  Easy-to-use..- U
-00000f60: 7469 6c69 7a65 7320 736f 6d65 206f 6620  tilizes some of 
-00000f70: 7468 6520 6661 6d6f 7573 2061 6e64 2063  the famous and c
-00000f80: 7574 7469 6e67 2d65 6467 6520 6d61 6368  utting-edge mach
-00000f90: 696e 6520 6c65 6172 6e69 6e67 2070 6163  ine learning pac
-00000fa0: 6b61 6765 732e 0a2d 204f 6666 6572 7320  kages..- Offers 
-00000fb0: 7375 7065 7276 6973 6564 2061 6e64 2075  supervised and u
-00000fc0: 6e2d 7375 7065 7276 6973 6564 204d 4c20  n-supervised ML 
-00000fd0: 7465 6368 6e69 7175 6573 2e0a 0a5f 5f4f  techniques...__O
-00000fe0: 7065 6e20 6465 6d6f 7320 6172 6520 6176  pen demos are av
-00000ff0: 6169 6c61 626c 6520 696e 3a5f 5f0a 0a3c  ailable in:__..<
-00001000: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
-00001010: 7222 3e0a 2020 2020 3c61 2068 7265 663d  r">.    <a href=
-00001020: 2268 7474 7073 3a2f 2f6e 6276 6965 7765  "https://nbviewe
-00001030: 722e 6f72 672f 6769 7468 7562 2f41 492d  r.org/github/AI-
-00001040: 7465 616d 2d55 6f41 2f70 794a 6564 4149  team-UoA/pyJedAI
-00001050: 2f62 6c6f 622f 6d61 696e 2f64 6f63 732f  /blob/main/docs/
-00001060: 7475 746f 7269 616c 732f 4465 6d6f 2e69  tutorials/Demo.i
-00001070: 7079 6e62 223e 0a20 2020 2020 2020 203c  pynb">.        <
-00001080: 696d 6720 616c 6967 6e3d 2263 656e 7465  img align="cente
-00001090: 7222 2073 7263 3d22 6874 7470 733a 2f2f  r" src="https://
-000010a0: 6e62 7669 6577 6572 2e6f 7267 2f73 7461  nbviewer.org/sta
-000010b0: 7469 632f 696d 672f 6e61 765f 6c6f 676f  tic/img/nav_logo
-000010c0: 2e73 7667 2220 7769 6474 683d 3132 302f  .svg" width=120/
-000010d0: 3e20 0a20 2020 203c 2f61 3e20 2026 6e62  > .    </a>  &nb
-000010e0: 7370 3b26 6e62 7370 3b26 6e62 7370 3b26  sp;&nbsp;&nbsp;&
-000010f0: 6e62 7370 3b26 6e62 7370 3b26 6e62 7370  nbsp;&nbsp;&nbsp
-00001100: 3b26 6e62 7370 3b0a 2020 2020 3c61 2068  ;&nbsp;.    <a h
-00001110: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00001120: 6875 622e 636f 6d2f 4149 2d74 6561 6d2d  hub.com/AI-team-
-00001130: 556f 412f 7079 4a65 6441 492f 626c 6f62  UoA/pyJedAI/blob
-00001140: 2f6d 6169 6e2f 646f 6373 2f74 7574 6f72  /main/docs/tutor
-00001150: 6961 6c73 2f44 656d 6f2e 6970 796e 6222  ials/Demo.ipynb"
-00001160: 3e0a 2020 2020 2020 2020 3c69 6d67 2061  >.        <img a
-00001170: 6c69 676e 3d22 6365 6e74 6572 2220 7372  lign="center" sr
-00001180: 633d 2268 7474 7073 3a2f 2f6d 6972 6f2e  c="https://miro.
-00001190: 6d65 6469 756d 2e63 6f6d 2f6d 6178 2f31  medium.com/max/1
-000011a0: 3430 302f 312a 4564 6e5f 4c70 6253 704c  400/1*Edn_LpbSpL
-000011b0: 654e 4b66 576b 4564 4732 4a67 2e70 6e67  eNKfWkEdG2Jg.png
-000011c0: 2220 7769 6474 683d 3132 302f 3e20 0a20  " width=120/> . 
-000011d0: 2020 203c 2f61 3e0a 3c2f 6469 763e 0a0a     </a>.</div>..
-000011e0: 5f5f 476f 6f67 6c65 2043 6f6c 6162 2048  __Google Colab H
-000011f0: 616e 6473 2d6f 6e20 6465 6d6f 3a5f 5f20  ands-on demo:__ 
-00001200: 0a0a 3c64 6976 2061 6c69 676e 3d22 6365  ..<div align="ce
-00001210: 6e74 6572 223e 0a20 2020 203c 6120 6872  nter">.    <a hr
-00001220: 6566 3d22 6874 7470 733a 2f2f 636f 6c61  ef="https://cola
-00001230: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
-00001240: 652e 636f 6d2f 6472 6976 652f 3138 5667  e.com/drive/18Vg
-00001250: 454f 4b41 6332 4f62 4646 7844 4e62 3273  EOKAc2ObFFxDNb2s
-00001260: 6a68 424c 4b4b 734e 7666 4550 6f3f 7573  jhBLKKsNvfEPo?us
-00001270: 703d 7368 6172 696e 6722 3e0a 2020 2020  p=sharing">.    
-00001280: 2020 2020 3c69 6d67 2061 6c69 676e 3d22      <img align="
-00001290: 6365 6e74 6572 2220 7372 633d 2268 7474  center" src="htt
-000012a0: 7073 3a2f 2f33 2e62 702e 626c 6f67 7370  ps://3.bp.blogsp
-000012b0: 6f74 2e63 6f6d 2f2d 6170 6f42 6557 4679  ot.com/-apoBeWFy
-000012c0: 634b 512f 5868 4b42 3866 4570 7277 492f  cKQ/XhKB8fEprwI/
-000012d0: 4141 4141 4141 4141 434d 342f 536c 3736  AAAAAAAACM4/Sl76
-000012e0: 797a 4e53 4e59 776c 5368 4942 7268 6544  yzNSNYwlShIBrheD
-000012f0: 4175 6d38 4c39 7152 7457 4e64 6743 4c63  Aum8L9qRtWNdgCLc
-00001300: 4247 4173 5948 512f 7331 3630 302f 636f  BGAsYHQ/s1600/co
-00001310: 6c61 622e 706e 6722 2077 6964 7468 3d31  lab.png" width=1
-00001320: 3230 2f3e 200a 2020 2020 3c2f 613e 0a3c  20/> .    </a>.<
-00001330: 2f64 6976 3e0a 0a23 2049 6e73 7461 6c6c  /div>..# Install
-00001340: 0a0a 2323 2320 5079 5049 0a49 6e73 7461  ..### PyPI.Insta
-00001350: 6c6c 2074 6865 206c 6174 6573 7420 7665  ll the latest ve
-00001360: 7273 696f 6e20 6f66 2070 796a 6564 6169  rsion of pyjedai
-00001370: 205f 5f5b 7265 7175 6972 6573 2070 7974   __[requires pyt
-00001380: 686f 6e20 3e3d 2033 2e38 5d5f 5f3a 0a60  hon >= 3.8]__:.`
-00001390: 6060 0a70 6970 2069 6e73 7461 6c6c 2070  ``.pip install p
-000013a0: 796a 6564 6169 0a60 6060 0a4d 6f72 6520  yjedai.```.More 
-000013b0: 6f6e 205b 5079 5049 5d28 6874 7470 733a  on [PyPI](https:
-000013c0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-000013d0: 6374 2f70 796a 6564 6169 292e 0a0a 2323  ct/pyjedai)...##
-000013e0: 2320 4769 740a 0a53 6574 2075 7020 6c6f  # Git..Set up lo
-000013f0: 6361 6c6c 793a 0a60 6060 0a67 6974 2063  cally:.```.git c
-00001400: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
-00001410: 6875 622e 636f 6d2f 4149 2d74 6561 6d2d  hub.com/AI-team-
-00001420: 556f 412f 7079 4a65 6441 492e 6769 740a  UoA/pyJedAI.git.
-00001430: 6060 600a 676f 2074 6f20 7468 6520 726f  ```.go to the ro
-00001440: 6f74 2064 6972 6563 746f 7279 2077 6974  ot directory wit
-00001450: 6820 6063 6420 7079 4a65 6441 4960 2061  h `cd pyJedAI` a
-00001460: 6e64 2074 7970 653a 0a60 6060 0a70 6970  nd type:.```.pip
-00001470: 2069 6e73 7461 6c6c 202e 0a60 6060 0a0a   install ..```..
-00001480: 2323 2320 446f 636b 6572 0a0a 4176 6169  ### Docker..Avai
-00001490: 6c61 626c 6520 6174 205b 446f 636b 6572  lable at [Docker
-000014a0: 2048 7562 5d28 6874 7470 733a 2f2f 6875   Hub](https://hu
-000014b0: 622e 646f 636b 6572 2e63 6f6d 2f72 2f61  b.docker.com/r/a
-000014c0: 6974 6561 6d75 6f61 2f70 796a 6564 6169  iteamuoa/pyjedai
-000014d0: 292c 206f 7220 636c 6f6e 6520 7468 6973  ), or clone this
-000014e0: 2072 6570 6f20 616e 643a 0a60 6060 0a64   repo and:.```.d
-000014f0: 6f63 6b65 7220 6275 696c 6420 2d66 2044  ocker build -f D
-00001500: 6f63 6b65 7266 696c 650a 6060 600a 0a23  ockerfile.```..#
-00001510: 2044 6570 656e 6465 6e63 6965 730a 0a3c   Dependencies..<
-00001520: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
-00001530: 7222 3e0a 2020 2020 3c69 6d67 2061 6c69  r">.    <img ali
-00001540: 676e 3d22 6365 6e74 6572 2220 7372 633d  gn="center" src=
-00001550: 2268 7474 7073 3a2f 2f75 706c 6f61 642e  "https://upload.
-00001560: 7769 6b69 6d65 6469 612e 6f72 672f 7769  wikimedia.org/wi
-00001570: 6b69 7065 6469 612f 636f 6d6d 6f6e 732f  kipedia/commons/
-00001580: 7468 756d 622f 652f 6564 2f50 616e 6461  thumb/e/ed/Panda
-00001590: 735f 6c6f 676f 2e73 7667 2f32 3536 3070  s_logo.svg/2560p
-000015a0: 782d 5061 6e64 6173 5f6c 6f67 6f2e 7376  x-Pandas_logo.sv
-000015b0: 672e 706e 6722 2077 6964 7468 3d31 3230  g.png" width=120
-000015c0: 2f3e 2026 6e62 7370 3b26 6e62 7370 3b0a  /> &nbsp;&nbsp;.
-000015d0: 2020 2020 3c69 6d67 2061 6c69 676e 3d22      <img align="
-000015e0: 6365 6e74 6572 2220 7372 633d 2268 7474  center" src="htt
-000015f0: 7073 3a2f 2f75 706c 6f61 642e 7769 6b69  ps://upload.wiki
-00001600: 6d65 6469 612e 6f72 672f 7769 6b69 7065  media.org/wikipe
-00001610: 6469 612f 636f 6d6d 6f6e 732f 7468 756d  dia/commons/thum
-00001620: 622f 332f 3331 2f4e 756d 5079 5f6c 6f67  b/3/31/NumPy_log
-00001630: 6f5f 3230 3230 2e73 7667 2f31 3238 3070  o_2020.svg/1280p
-00001640: 782d 4e75 6d50 795f 6c6f 676f 5f32 3032  x-NumPy_logo_202
-00001650: 302e 7376 672e 706e 6722 2077 6964 7468  0.svg.png" width
-00001660: 3d31 3230 2f3e 2026 6e62 7370 3b26 6e62  =120/> &nbsp;&nb
-00001670: 7370 3b0a 2020 2020 3c69 6d67 2061 6c69  sp;.    <img ali
-00001680: 676e 3d22 6365 6e74 6572 2220 7372 633d  gn="center" src=
-00001690: 2268 7474 7073 3a2f 2f6c 6f67 6f65 7073  "https://logoeps
-000016a0: 2e63 6f6d 2f77 702d 636f 6e74 656e 742f  .com/wp-content/
-000016b0: 7570 6c6f 6164 732f 3230 3132 2f31 302f  uploads/2012/10/
-000016c0: 7079 7468 6f6e 2d6c 6f67 6f2d 7665 6374  python-logo-vect
-000016d0: 6f72 2e70 6e67 2220 7769 6474 683d 3132  or.png" width=12
-000016e0: 302f 3e20 266e 6273 703b 266e 6273 703b  0/> &nbsp;&nbsp;
-000016f0: 266e 6273 703b 0a20 2020 203c 696d 6720  &nbsp;.    <img 
-00001700: 616c 6967 6e3d 2263 656e 7465 7222 2073  align="center" s
-00001710: 7263 3d22 6874 7470 733a 2f2f 7570 6c6f  rc="https://uplo
-00001720: 6164 2e77 696b 696d 6564 6961 2e6f 7267  ad.wikimedia.org
-00001730: 2f77 696b 6970 6564 6961 2f63 6f6d 6d6f  /wikipedia/commo
-00001740: 6e73 2f74 6875 6d62 2f33 2f33 382f 4a75  ns/thumb/3/38/Ju
-00001750: 7079 7465 725f 6c6f 676f 2e73 7667 2f38  pyter_logo.svg/8
-00001760: 3833 7078 2d4a 7570 7974 6572 5f6c 6f67  83px-Jupyter_log
-00001770: 6f2e 7376 672e 706e 6722 2077 6964 7468  o.svg.png" width
-00001780: 3d37 302f 3e20 203c 6272 3e0a 2020 2020  =70/>  <br>.    
-00001790: 3c69 6d67 2061 6c69 676e 3d22 6365 6e74  <img align="cent
-000017a0: 6572 2220 7372 633d 2268 7474 7073 3a2f  er" src="https:/
-000017b0: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-000017c0: 6f6e 7465 6e74 2e63 6f6d 2f6f 7074 756e  ontent.com/optun
-000017d0: 612f 6f70 7475 6e61 2f6d 6173 7465 722f  a/optuna/master/
-000017e0: 646f 6373 2f69 6d61 6765 2f6f 7074 756e  docs/image/optun
-000017f0: 612d 6c6f 676f 2e70 6e67 2220 7769 6474  a-logo.png" widt
-00001800: 683d 3135 302f 3e0a 2020 2020 3c69 6d67  h=150/>.    <img
-00001810: 2061 6c69 676e 3d22 6365 6e74 6572 2220   align="center" 
-00001820: 7372 633d 2268 7474 7073 3a2f 2f75 706c  src="https://upl
-00001830: 6f61 642e 7769 6b69 6d65 6469 612e 6f72  oad.wikimedia.or
-00001840: 672f 7769 6b69 7065 6469 612f 636f 6d6d  g/wikipedia/comm
-00001850: 6f6e 732f 7468 756d 622f 382f 3861 2f50  ons/thumb/8/8a/P
-00001860: 6c6f 746c 795f 6c6f 676f 5f66 6f72 5f64  lotly_logo_for_d
-00001870: 6967 6974 616c 5f66 696e 616c 5f25 3238  igital_final_%28
-00001880: 3625 3239 2e70 6e67 2f31 3230 3070 782d  6%29.png/1200px-
-00001890: 506c 6f74 6c79 5f6c 6f67 6f5f 666f 725f  Plotly_logo_for_
-000018a0: 6469 6769 7461 6c5f 6669 6e61 6c5f 2532  digital_final_%2
-000018b0: 3836 2532 392e 706e 6722 2077 6964 7468  86%29.png" width
-000018c0: 3d31 3530 2f3e 0a20 2020 203c 696d 6720  =150/>.    <img 
-000018d0: 616c 6967 6e3d 2263 656e 7465 7222 2073  align="center" s
-000018e0: 7263 3d22 6874 7470 733a 2f2f 7079 746f  rc="https://pyto
-000018f0: 7263 682e 6f72 672f 7475 746f 7269 616c  rch.org/tutorial
-00001900: 732f 5f73 7461 7469 632f 696d 672f 7468  s/_static/img/th
-00001910: 756d 626e 6169 6c73 2f63 726f 7070 6564  umbnails/cropped
-00001920: 2f70 726f 6669 6c65 722e 706e 6722 2077  /profiler.png" w
-00001930: 6964 7468 3d31 3630 2f3e 200a 2020 2020  idth=160/> .    
-00001940: 3c69 6d67 2061 6c69 676e 3d22 6365 6e74  <img align="cent
-00001950: 6572 2220 7372 633d 2268 7474 7073 3a2f  er" src="https:/
-00001960: 2f77 7777 2e66 756c 6c73 7461 636b 7079  /www.fullstackpy
-00001970: 7468 6f6e 2e63 6f6d 2f69 6d67 2f6c 6f67  thon.com/img/log
-00001980: 6f73 2f73 6369 7079 2e70 6e67 2220 7769  os/scipy.png" wi
-00001990: 6474 683d 3135 302f 3e20 203c 6272 3e3c  dth=150/>  <br><
-000019a0: 6272 3e0a 2020 2020 3c69 6d67 2061 6c69  br>.    <img ali
-000019b0: 676e 3d22 6365 6e74 6572 2220 7372 633d  gn="center" src=
-000019c0: 2268 7474 7073 3a2f 2f77 7777 2e6b 6f72  "https://www.kor
-000019d0: 6e6f 736b 2e6d 652f 7265 736f 7572 6365  nosk.me/resource
-000019e0: 732f 6c61 6e67 7561 6765 2d6d 6f64 656c  s/language-model
-000019f0: 2f66 6561 7475 7265 642e 706e 6722 2077  /featured.png" w
-00001a00: 6964 7468 3d31 3530 2f3e 2026 6e62 7370  idth=150/> &nbsp
-00001a10: 3b26 6e62 7370 3b26 6e62 7370 3b0a 2020  ;&nbsp;&nbsp;.  
-00001a20: 2020 3c69 6d67 2061 6c69 676e 3d22 6365    <img align="ce
-00001a30: 6e74 6572 2220 7372 633d 2268 7474 7073  nter" src="https
-00001a40: 3a2f 2f72 6570 6f73 6974 6f72 792d 696d  ://repository-im
-00001a50: 6167 6573 2e67 6974 6875 6275 7365 7263  ages.githubuserc
-00001a60: 6f6e 7465 6e74 2e63 6f6d 2f31 3334 3937  ontent.com/13497
-00001a70: 3735 2f32 3032 6334 3638 302d 3866 3763  75/202c4680-8f7c
-00001a80: 2d31 3165 392d 3931 6336 2d37 3435 6664  -11e9-91c6-745fd
-00001a90: 6362 6566 6665 3822 2077 6964 7468 3d31  cbeffe8" width=1
-00001aa0: 3530 2f3e 2026 6e62 7370 3b26 6e62 7370  50/> &nbsp;&nbsp
-00001ab0: 3b26 6e62 7370 3b0a 2020 2020 3c69 6d67  ;&nbsp;.    <img
-00001ac0: 2061 6c69 676e 3d22 6365 6e74 6572 2220   align="center" 
-00001ad0: 7372 633d 2268 7474 7073 3a2f 2f6e 6574  src="https://net
-00001ae0: 776f 726b 782e 6f72 672f 5f73 7461 7469  workx.org/_stati
-00001af0: 632f 6e65 7477 6f72 6b78 5f6c 6f67 6f2e  c/networkx_logo.
-00001b00: 7376 6722 2077 6964 7468 3d31 3530 2f3e  svg" width=150/>
-00001b10: 2026 6e62 7370 3b26 6e62 7370 3b26 6e62   &nbsp;&nbsp;&nb
-00001b20: 7370 3b0a 2020 2020 3c69 6d67 2061 6c69  sp;.    <img ali
-00001b30: 676e 3d22 6365 6e74 6572 2220 7372 633d  gn="center" src=
-00001b40: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
-00001b50: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00001b60: 6f6d 2f52 4446 4c69 622f 4f57 4c2d 524c  om/RDFLib/OWL-RL
-00001b70: 2f6d 6173 7465 722f 4f57 4c2d 524c 2e70  /master/OWL-RL.p
-00001b80: 6e67 2220 7769 6474 683d 3730 2f3e 200a  ng" width=70/> .
-00001b90: 3c2f 6469 763e 0a3c 6272 3e0a 0a53 6565  </div>.<br>..See
-00001ba0: 2074 6865 2066 756c 6c20 6c69 7374 206f   the full list o
-00001bb0: 6620 6465 7065 6e64 656e 6369 6573 2061  f dependencies a
-00001bc0: 6e64 2061 6c6c 2076 6572 7369 6f6e 7320  nd all versions 
-00001bd0: 7573 6564 2c20 696e 2074 6869 7320 5b66  used, in this [f
-00001be0: 696c 655d 2868 7474 7073 3a2f 2f67 6974  ile](https://git
-00001bf0: 6875 622e 636f 6d2f 4149 2d74 6561 6d2d  hub.com/AI-team-
-00001c00: 556f 412f 7079 4a65 6441 492f 626c 6f62  UoA/pyJedAI/blob
-00001c10: 2f6d 6169 6e2f 7079 7072 6f6a 6563 742e  /main/pyproject.
-00001c20: 746f 6d6c 292e 0a0a 5f5f 5374 6174 7573  toml)...__Status
-00001c30: 5f5f 0a0a 5b21 5b54 6573 7473 5d28 6874  __..[![Tests](ht
-00001c40: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001c50: 2f41 492d 7465 616d 2d55 6f41 2f70 794a  /AI-team-UoA/pyJ
-00001c60: 6564 4149 2f61 6374 696f 6e73 2f77 6f72  edAI/actions/wor
-00001c70: 6b66 6c6f 7773 2f74 6573 7473 2e79 6d6c  kflows/tests.yml
-00001c80: 2f62 6164 6765 2e73 7667 3f62 7261 6e63  /badge.svg?branc
-00001c90: 683d 6d61 696e 295d 2868 7474 7073 3a2f  h=main)](https:/
-00001ca0: 2f67 6974 6875 622e 636f 6d2f 4149 2d74  /github.com/AI-t
-00001cb0: 6561 6d2d 556f 412f 7079 4a65 6441 492f  eam-UoA/pyJedAI/
-00001cc0: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-00001cd0: 732f 7465 7374 732e 796d 6c29 0a5b 215b  s/tests.yml).[![
-00001ce0: 5079 5069 5d28 6874 7470 733a 2f2f 6769  PyPi](https://gi
-00001cf0: 7468 7562 2e63 6f6d 2f41 492d 7465 616d  thub.com/AI-team
-00001d00: 2d55 6f41 2f70 794a 6564 4149 2f61 6374  -UoA/pyJedAI/act
-00001d10: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f70  ions/workflows/p
-00001d20: 7970 692d 7075 626c 6973 682e 796d 6c2f  ypi-publish.yml/
-00001d30: 6261 6467 652e 7376 6729 5d28 6874 7470  badge.svg)](http
-00001d40: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
-00001d50: 492d 7465 616d 2d55 6f41 2f70 794a 6564  I-team-UoA/pyJed
-00001d60: 4149 2f61 6374 696f 6e73 2f77 6f72 6b66  AI/actions/workf
-00001d70: 6c6f 7773 2f70 7970 692d 7075 626c 6973  lows/pypi-publis
-00001d80: 682e 796d 6c29 0a5b 215b 6d61 6465 2d77  h.yml).[![made-w
-00001d90: 6974 682d 7079 7468 6f6e 5d28 6874 7470  ith-python](http
-00001da0: 733a 2f2f 7265 6164 7468 6564 6f63 732e  s://readthedocs.
-00001db0: 6f72 672f 7072 6f6a 6563 7473 2f70 796a  org/projects/pyj
-00001dc0: 6564 6169 2f62 6164 6765 2f3f 7665 7273  edai/badge/?vers
-00001dd0: 696f 6e3d 6c61 7465 7374 295d 2868 7474  ion=latest)](htt
-00001de0: 7073 3a2f 2f70 796a 6564 6169 2e72 6561  ps://pyjedai.rea
-00001df0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00001e00: 6174 6573 742f 3f62 6164 6765 3d6c 6174  atest/?badge=lat
-00001e10: 6573 7429 0a5b 215b 636f 6465 636f 765d  est).[![codecov]
-00001e20: 2868 7474 7073 3a2f 2f63 6f64 6563 6f76  (https://codecov
-00001e30: 2e69 6f2f 6768 2f41 492d 7465 616d 2d55  .io/gh/AI-team-U
-00001e40: 6f41 2f70 796a 6564 6169 2f62 7261 6e63  oA/pyjedai/branc
-00001e50: 682f 6d61 7374 6572 2f67 7261 7068 2f62  h/master/graph/b
-00001e60: 6164 6765 2e73 7667 3f74 6f6b 656e 3d34  adge.svg?token=4
-00001e70: 5152 3058 3331 3543 4c29 5d28 6874 7470  QR0X315CL)](http
-00001e80: 733a 2f2f 636f 6465 636f 762e 696f 2f67  s://codecov.io/g
-00001e90: 682f 4149 2d74 6561 6d2d 556f 412f 7079  h/AI-team-UoA/py
-00001ea0: 6a65 6461 6929 0a0a 0a5f 5f53 7461 7469  jedai)...__Stati
-00001eb0: 7374 6963 7320 2620 496e 666f 5f5f 0a0a  stics & Info__..
-00001ec0: 215b 5079 5049 202d 2044 6f77 6e6c 6f61  ![PyPI - Downloa
-00001ed0: 6473 5d28 6874 7470 733a 2f2f 696d 672e  ds](https://img.
-00001ee0: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00001ef0: 646d 2f70 796a 6564 6169 290a 5b21 5b50  dm/pyjedai).[![P
-00001f00: 7950 4920 7665 7273 696f 6e5d 2868 7474  yPI version](htt
-00001f10: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00001f20: 2e69 6f2f 7079 7069 2f76 2f70 796a 6564  .io/pypi/v/pyjed
-00001f30: 6169 2e73 7667 3f6c 6f67 6f3d 7079 7069  ai.svg?logo=pypi
-00001f40: 266c 6f67 6f43 6f6c 6f72 3d46 4645 3837  &logoColor=FFE87
-00001f50: 3329 5d28 6874 7470 733a 2f2f 7079 7069  3)](https://pypi
-00001f60: 2e6f 7267 2f70 726f 6a65 6374 2f70 796a  .org/project/pyj
-00001f70: 6564 6169 2f29 0a0a 0a23 2042 7567 732c  edai/)...# Bugs,
-00001f80: 2044 6973 6375 7373 696f 6e73 2026 204e   Discussions & N
-00001f90: 6577 730a 0a5b 4769 7448 7562 2044 6973  ews..[GitHub Dis
-00001fa0: 6375 7373 696f 6e73 5d28 6874 7470 733a  cussions](https:
-00001fb0: 2f2f 6769 7468 7562 2e63 6f6d 2f41 492d  //github.com/AI-
-00001fc0: 7465 616d 2d55 6f41 2f70 794a 6564 4149  team-UoA/pyJedAI
-00001fd0: 2f64 6973 6375 7373 696f 6e73 2920 6973  /discussions) is
-00001fe0: 2074 6865 2064 6973 6375 7373 696f 6e20   the discussion 
-00001ff0: 666f 7275 6d20 666f 7220 6765 6e65 7261  forum for genera
-00002000: 6c20 7175 6573 7469 6f6e 7320 616e 6420  l questions and 
-00002010: 6469 7363 7573 7369 6f6e 7320 616e 6420  discussions and 
-00002020: 6f75 7220 7265 636f 6d6d 656e 6465 6420  our recommended 
-00002030: 7374 6172 7469 6e67 2070 6f69 6e74 2e20  starting point. 
-00002040: 506c 6561 7365 2072 6570 6f72 7420 616e  Please report an
-00002050: 7920 6275 6773 2074 6861 7420 796f 7520  y bugs that you 
-00002060: 6669 6e64 205b 6865 7265 5d28 6874 7470  find [here](http
-00002070: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
-00002080: 492d 7465 616d 2d55 6f41 2f70 794a 6564  I-team-UoA/pyJed
-00002090: 4149 2f69 7373 7565 7329 2e0a 0a23 204a  AI/issues)...# J
-000020a0: 6176 6120 2d20 5765 6220 4170 706c 6963  ava - Web Applic
-000020b0: 6174 696f 6e20 0a0a 3c69 6d67 2061 6c69  ation ..<img ali
-000020c0: 676e 3d22 6c65 6674 2220 7372 633d 2268  gn="left" src="h
-000020d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000020e0: 6d2f 7363 6966 792f 4a65 6441 4954 6f6f  m/scify/JedAIToo
-000020f0: 6c6b 6974 2f62 6c6f 622f 6d61 7374 6572  lkit/blob/master
-00002100: 2f64 6f63 756d 656e 7461 7469 6f6e 2f4a  /documentation/J
-00002110: 6564 4149 5f6c 6f67 6f2e 706e 673f 7261  edAI_logo.png?ra
-00002120: 773d 7472 7565 2220 616c 743d 2270 794a  w=true" alt="pyJ
-00002130: 6564 4149 2220 7769 6474 683d 2231 3330  edAI" width="130
-00002140: 222f 3e0a 0a46 6f72 204a 6176 6120 7573  "/>..For Java us
-00002150: 6572 7320 6368 6563 6b6f 7574 2074 6865  ers checkout the
-00002160: 2069 6e69 7469 616c 205b 4a65 6441 495d   initial [JedAI]
-00002170: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00002180: 636f 6d2f 7363 6966 792f 4a65 6441 4954  com/scify/JedAIT
-00002190: 6f6f 6c6b 6974 292e 2054 6865 7265 2079  oolkit). There y
-000021a0: 6f75 2063 616e 2066 696e 6420 4a61 7661  ou can find Java
-000021b0: 2062 6173 6564 2063 6f64 6520 616e 6420   based code and 
-000021c0: 6120 5765 6220 4170 706c 6963 6174 696f  a Web Applicatio
-000021d0: 6e20 666f 7220 696e 7465 7261 6374 6976  n for interactiv
-000021e0: 6520 6372 6561 7469 6f6e 206f 6620 4552  e creation of ER
-000021f0: 2077 6f72 6b66 6c6f 7773 2e20 3c62 723e   workflows. <br>
-00002200: 3c62 723e 204a 6564 4149 2063 6f6e 7374  <br> JedAI const
-00002210: 6974 7574 6573 2061 6e20 6f70 656e 2073  itutes an open s
-00002220: 6f75 7263 652c 2068 6967 6820 7363 616c  ource, high scal
-00002230: 6162 696c 6974 7920 746f 6f6c 6b69 7420  ability toolkit 
-00002240: 7468 6174 206f 6666 6572 7320 6f75 742d  that offers out-
-00002250: 6f66 2d74 6865 2d62 6f78 2073 6f6c 7574  of-the-box solut
-00002260: 696f 6e73 2066 6f72 2061 6e79 2064 6174  ions for any dat
-00002270: 6120 696e 7465 6772 6174 696f 6e20 7461  a integration ta
-00002280: 736b 2c20 652e 672e 2c20 5265 636f 7264  sk, e.g., Record
-00002290: 204c 696e 6b61 6765 2c20 456e 7469 7479   Linkage, Entity
-000022a0: 2052 6573 6f6c 7574 696f 6e20 616e 6420   Resolution and 
-000022b0: 4c69 6e6b 2044 6973 636f 7665 7279 2e20  Link Discovery. 
-000022c0: 4174 2069 7473 2063 6f72 6520 6c69 6573  At its core lies
-000022d0: 2061 2073 6574 206f 6620 646f 6d61 696e   a set of domain
-000022e0: 2d69 6e64 6570 656e 6465 6e74 2c20 7374  -independent, st
-000022f0: 6174 652d 6f66 2d74 6865 2d61 7274 2074  ate-of-the-art t
-00002300: 6563 686e 6971 7565 7320 7468 6174 2061  echniques that a
-00002310: 7070 6c79 2074 6f20 626f 7468 2052 4446  pply to both RDF
-00002320: 2061 6e64 2072 656c 6174 696f 6e61 6c20   and relational 
-00002330: 6461 7461 2e0a 0a3c 6272 3e0a 0a23 2054  data...<br>..# T
-00002340: 6561 6d20 2620 4175 7468 6f72 730a 0a3c  eam & Authors..<
-00002350: 696d 6720 616c 6967 6e3d 2272 6967 6874  img align="right
-00002360: 2220 7372 633d 2268 7474 7073 3a2f 2f67  " src="https://g
-00002370: 6974 6875 622e 636f 6d2f 4149 2d74 6561  ithub.com/AI-tea
-00002380: 6d2d 556f 412f 2e67 6974 6875 622f 626c  m-UoA/.github/bl
-00002390: 6f62 2f6d 6169 6e2f 4149 5f4c 4f47 4f2e  ob/main/AI_LOGO.
-000023a0: 706e 673f 7261 773d 7472 7565 2220 616c  png?raw=true" al
-000023b0: 743d 2270 794a 6564 4149 2220 7769 6474  t="pyJedAI" widt
-000023c0: 683d 2232 3030 222f 3e0a 0a2d 205b 4b6f  h="200"/>..- [Ko
-000023d0: 6e73 7461 6e74 696e 6f73 204e 696b 6f6c  nstantinos Nikol
-000023e0: 6574 6f73 5d28 6874 7470 733a 2f2f 6e69  etos](https://ni
-000023f0: 6b6f 6c65 746f 732d 6b2e 6769 7468 7562  koletos-k.github
-00002400: 2e69 6f29 0a2d 204a 616b 7562 204d 6163  .io).- Jakub Mac
-00002410: 6965 6a65 7773 6b69 0a2d 205b 4765 6f72  iejewski.- [Geor
-00002420: 6765 2050 6170 6164 616b 6973 5d28 6874  ge Papadakis](ht
-00002430: 7470 733a 2f2f 6770 6170 6164 6973 2e77  tps://gpapadis.w
-00002440: 6f72 6470 7265 7373 2e63 6f6d 290a 2d20  ordpress.com).- 
-00002450: 5b4d 616e 6f6c 6973 204b 6f75 6261 7261  [Manolis Koubara
-00002460: 6b69 735d 2868 7474 7073 3a2f 2f63 6769  kis](https://cgi
-00002470: 2e64 692e 756f 612e 6772 2f7e 6b6f 7562  .di.uoa.gr/~koub
-00002480: 6172 616b 2f29 0a0a 5265 7365 6172 6368  arak/)..Research
-00002490: 2061 6e64 2064 6576 656c 6f70 6d65 6e74   and development
-000024a0: 2069 7320 6d61 6465 2075 6e64 6572 2074   is made under t
-000024b0: 6865 2073 7570 6572 7669 7369 6f6e 206f  he supervision o
-000024c0: 6620 5072 2e20 4d61 6e6f 6c69 7320 4b6f  f Pr. Manolis Ko
-000024d0: 7562 6172 616b 6973 2e20 5468 6973 2069  ubarakis. This i
-000024e0: 7320 6120 7265 7365 6172 6368 2070 726f  s a research pro
-000024f0: 6a65 6374 2062 7920 7468 6520 5b41 492d  ject by the [AI-
-00002500: 5465 616d 5d28 6874 7470 733a 2f2f 6169  Team](https://ai
-00002510: 2e64 692e 756f 612e 6772 2920 6f66 2074  .di.uoa.gr) of t
-00002520: 6865 2044 6570 6172 746d 656e 7420 6f66  he Department of
-00002530: 2049 6e66 6f72 6d61 7469 6373 2061 6e64   Informatics and
-00002540: 2054 656c 6563 6f6d 6d75 6e69 6361 7469   Telecommunicati
-00002550: 6f6e 7320 6174 2074 6865 2055 6e69 7665  ons at the Unive
-00002560: 7273 6974 7920 6f66 2041 7468 656e 732e  rsity of Athens.
-00002570: 0a0a 2320 4c69 6365 6e73 650a 0a52 656c  ..# License..Rel
-00002580: 6561 7365 6420 756e 6465 7220 7468 6520  eased under the 
-00002590: 4170 6163 6865 2d32 2e30 206c 6963 656e  Apache-2.0 licen
-000025a0: 7365 2028 7365 6520 5b4c 4943 454e 5345  se (see [LICENSE
-000025b0: 2e74 7874 5d28 6874 7470 733a 2f2f 6769  .txt](https://gi
-000025c0: 7468 7562 2e63 6f6d 2f41 492d 7465 616d  thub.com/AI-team
-000025d0: 2d55 6f41 2f70 794a 6564 4149 2f62 6c6f  -UoA/pyJedAI/blo
-000025e0: 622f 6d61 696e 2f4c 4943 454e 5345 2929  b/main/LICENSE))
-000025f0: 2e0a 0a43 6f70 7972 6967 6874 20c2 a920  ...Copyright .. 
-00002600: 3230 3233 2041 492d 5465 616d 2c20 556e  2023 AI-Team, Un
-00002610: 6976 6572 7369 7479 206f 6620 4174 6865  iversity of Athe
-00002620: 6e73 0a0a 3c64 6976 2061 6c69 676e 3d22  ns..<div align="
-00002630: 6365 6e74 6572 223e 0a20 2020 203c 6872  center">.    <hr
-00002640: 3e0a 2020 2020 3c62 723e 0a20 2020 203c  >.    <br>.    <
-00002650: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00002660: 7374 656c 6172 2d70 726f 6a65 6374 2e65  stelar-project.e
-00002670: 7522 3e0a 2020 2020 2020 2020 3c69 6d67  u">.        <img
-00002680: 2061 6c69 676e 3d22 6365 6e74 6572 2220   align="center" 
-00002690: 7372 633d 2268 7474 7073 3a2f 2f73 7465  src="https://ste
-000026a0: 6c61 722d 7072 6f6a 6563 742e 6575 2f77  lar-project.eu/w
-000026b0: 702d 636f 6e74 656e 742f 7570 6c6f 6164  p-content/upload
-000026c0: 732f 3230 3232 2f30 382f 4c6f 676f 2d53  s/2022/08/Logo-S
-000026d0: 7465 6c61 722d 312d 662e 706e 6722 2077  telar-1-f.png" w
-000026e0: 6964 7468 3d31 3830 2f3e 0a20 2020 203c  idth=180/>.    <
-000026f0: 2f61 3e20 266e 6273 703b 266e 6273 703b  /a> &nbsp;&nbsp;
-00002700: 266e 6273 703b 266e 6273 703b 266e 6273  &nbsp;&nbsp;&nbs
-00002710: 703b 266e 6273 703b 266e 6273 703b 0a20  p;&nbsp;&nbsp;. 
-00002720: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
-00002730: 733a 2f2f 6563 2e65 7572 6f70 612e 6575  s://ec.europa.eu
-00002740: 2f69 6e66 6f2f 696e 6465 785f 656e 223e  /info/index_en">
-00002750: 0a20 2020 2020 2020 203c 696d 6720 616c  .        <img al
-00002760: 6967 6e3d 2263 656e 7465 7222 2073 7263  ign="center" src
-00002770: 3d22 6874 7470 733a 2f2f 7570 6c6f 6164  ="https://upload
-00002780: 2e77 696b 696d 6564 6961 2e6f 7267 2f77  .wikimedia.org/w
-00002790: 696b 6970 6564 6961 2f63 6f6d 6d6f 6e73  ikipedia/commons
-000027a0: 2f74 6875 6d62 2f62 2f62 372f 466c 6167  /thumb/b/b7/Flag
-000027b0: 5f6f 665f 4575 726f 7065 2e73 7667 2f31  _of_Europe.svg/1
-000027c0: 3230 3070 782d 466c 6167 5f6f 665f 4575  200px-Flag_of_Eu
-000027d0: 726f 7065 2e73 7667 2e70 6e67 2220 7769  rope.svg.png" wi
-000027e0: 6474 683d 3134 302f 3e0a 2020 2020 3c2f  dth=140/>.    </
-000027f0: 613e 0a20 2020 203c 6272 3e0a 2020 2020  a>.    <br>.    
-00002800: 3c62 723e 0a20 2020 2020 2020 203c 623e  <br>.        <b>
-00002810: 5468 6973 2070 726f 6a65 6374 2069 7320  This project is 
-00002820: 6265 696e 6720 6675 6e64 6564 2069 6e20  being funded in 
-00002830: 7468 6520 636f 6e74 6578 7420 6f66 203c  the context of <
-00002840: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00002850: 7374 656c 6172 2d70 726f 6a65 6374 2e65  stelar-project.e
-00002860: 7522 3e53 5445 4c41 523c 2f61 3e20 7468  u">STELAR</a> th
-00002870: 6174 2069 7320 616e 203c 6120 6872 6566  at is an <a href
-00002880: 3d22 6874 7470 733a 2f2f 7265 7365 6172  ="https://resear
-00002890: 6368 2d61 6e64 2d69 6e6e 6f76 6174 696f  ch-and-innovatio
-000028a0: 6e2e 6563 2e65 7572 6f70 612e 6575 2f66  n.ec.europa.eu/f
-000028b0: 756e 6469 6e67 2f66 756e 6469 6e67 2d6f  unding/funding-o
-000028c0: 7070 6f72 7475 6e69 7469 6573 2f66 756e  pportunities/fun
-000028d0: 6469 6e67 2d70 726f 6772 616d 6d65 732d  ding-programmes-
-000028e0: 616e 642d 6f70 656e 2d63 616c 6c73 2f68  and-open-calls/h
-000028f0: 6f72 697a 6f6e 2d65 7572 6f70 655f 656e  orizon-europe_en
-00002900: 223e 484f 5249 5a4f 4e2d 4575 726f 7065  ">HORIZON-Europe
-00002910: 3c2f 613e 2070 726f 6a65 6374 2e0a 2020  </a> project..  
-00002920: 2020 2020 2020 3c2f 623e 0a20 2020 203c        </b>.    <
-00002930: 6272 3e0a 3c2f 6469 763e 0a              br>.</div>.
+000006a0: 696d 0a52 6571 7569 7265 732d 4469 7374  im.Requires-Dist
+000006b0: 3a20 6d61 7470 6c6f 746c 6962 0a52 6571  : matplotlib.Req
+000006c0: 7569 7265 732d 4469 7374 3a20 6e65 7477  uires-Dist: netw
+000006d0: 6f72 6b78 0a52 6571 7569 7265 732d 4469  orkx.Requires-Di
+000006e0: 7374 3a20 6e6c 746b 0a52 6571 7569 7265  st: nltk.Require
+000006f0: 732d 4469 7374 3a20 6e75 6d70 790a 5265  s-Dist: numpy.Re
+00000700: 7175 6972 6573 2d44 6973 743a 2070 616e  quires-Dist: pan
+00000710: 6461 730a 5265 7175 6972 6573 2d44 6973  das.Requires-Dis
+00000720: 743a 2073 6369 7079 3d3d 312e 3132 0a52  t: scipy==1.12.R
+00000730: 6571 7569 7265 732d 4469 7374 3a20 7365  equires-Dist: se
+00000740: 6162 6f72 6e0a 5265 7175 6972 6573 2d44  aborn.Requires-D
+00000750: 6973 743a 2074 7164 6d0a 5265 7175 6972  ist: tqdm.Requir
+00000760: 6573 2d44 6973 743a 2074 7261 6e73 666f  es-Dist: transfo
+00000770: 726d 6572 730a 5265 7175 6972 6573 2d44  rmers.Requires-D
+00000780: 6973 743a 2073 656e 7465 6e63 652d 7472  ist: sentence-tr
+00000790: 616e 7366 6f72 6d65 7273 0a52 6571 7569  ansformers.Requi
+000007a0: 7265 732d 4469 7374 3a20 6661 6973 732d  res-Dist: faiss-
+000007b0: 6370 750a 5265 7175 6972 6573 2d44 6973  cpu.Requires-Dis
+000007c0: 743a 2070 792d 7374 7269 6e67 6d61 7463  t: py-stringmatc
+000007d0: 6869 6e67 0a52 6571 7569 7265 732d 4469  hing.Requires-Di
+000007e0: 7374 3a20 7661 6c65 6e74 696e 653b 2070  st: valentine; p
+000007f0: 7974 686f 6e5f 7665 7273 696f 6e20 3e20  ython_version > 
+00000800: 2233 2e37 220a 5265 7175 6972 6573 2d44  "3.7".Requires-D
+00000810: 6973 743a 206f 7264 6572 6564 2d73 6574  ist: ordered-set
+00000820: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000830: 7368 6170 656c 790a 5072 6f76 6964 6573  shapely.Provides
+00000840: 2d45 7874 7261 3a20 6465 760a 5265 7175  -Extra: dev.Requ
+00000850: 6972 6573 2d44 6973 743a 2070 6970 2d74  ires-Dist: pip-t
+00000860: 6f6f 6c73 3b20 6578 7472 6120 3d3d 2022  ools; extra == "
+00000870: 6465 7622 0a52 6571 7569 7265 732d 4469  dev".Requires-Di
+00000880: 7374 3a20 7079 7465 7374 3b20 6578 7472  st: pytest; extr
+00000890: 6120 3d3d 2022 6465 7622 0a0a 3c64 6976  a == "dev"..<div
+000008a0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+000008b0: 0a20 2020 203c 6272 3e0a 2020 2020 3c69  .    <br>.    <i
+000008c0: 6d67 2061 6c69 676e 3d22 6365 6e74 6572  mg align="center
+000008d0: 2220 7372 633d 2268 7474 7073 3a2f 2f67  " src="https://g
+000008e0: 6974 6875 622e 636f 6d2f 4149 2d74 6561  ithub.com/AI-tea
+000008f0: 6d2d 556f 412f 7079 4a65 6441 492f 626c  m-UoA/pyJedAI/bl
+00000900: 6f62 2f6d 6169 6e2f 646f 6373 2f69 6d67  ob/main/docs/img
+00000910: 2f70 796a 6564 6169 2e6c 6f67 6f2e 6472  /pyjedai.logo.dr
+00000920: 6177 696f 2e70 6e67 3f72 6177 3d74 7275  awio.png?raw=tru
+00000930: 6522 2061 6c74 3d22 7079 4a65 6441 4922  e" alt="pyJedAI"
+00000940: 2077 6964 7468 3d22 3430 3022 2f3e 0a3c   width="400"/>.<
+00000950: 2f64 6976 3e0a 3c62 723e 0a3c 6272 3e0a  /div>.<br>.<br>.
+00000960: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00000970: 6572 223e 0a41 6e20 6f70 656e 2d73 6f75  er">.An open-sou
+00000980: 7263 6520 6c69 6272 6172 7920 7468 6174  rce library that
+00000990: 206c 6576 6572 6167 6573 2050 7974 686f   leverages Pytho
+000009a0: 6ee2 8099 7320 6461 7461 2073 6369 656e  n...s data scien
+000009b0: 6365 2065 636f 7379 7374 656d 2074 6f20  ce ecosystem to 
+000009c0: 6275 696c 6420 3c62 723e 2070 6f77 6572  build <br> power
+000009d0: 6675 6c20 656e 642d 746f 2d65 6e64 2045  ful end-to-end E
+000009e0: 6e74 6974 7920 5265 736f 6c75 7469 6f6e  ntity Resolution
+000009f0: 2077 6f72 6b66 6c6f 7773 2e0a 3c2f 6469   workflows..</di
+00000a00: 763e 0a0a 0a2d 2d2d 0a0a 0a23 204f 7665  v>...---...# Ove
+00000a10: 7276 6965 770a 0a70 794a 6564 4149 2069  rview..pyJedAI i
+00000a20: 7320 6120 7079 7468 6f6e 2066 7261 6d65  s a python frame
+00000a30: 776f 726b 2c20 6169 6d69 6e67 2074 6f20  work, aiming to 
+00000a40: 6f66 6665 7220 6578 7065 7274 7320 616e  offer experts an
+00000a50: 6420 6e6f 7669 6365 2075 7365 7273 2c20  d novice users, 
+00000a60: 726f 6275 7374 2061 6e64 2066 6173 7420  robust and fast 
+00000a70: 736f 6c75 7469 6f6e 7320 666f 7220 6d75  solutions for mu
+00000a80: 6c74 6970 6c65 2074 7970 6573 206f 6620  ltiple types of 
+00000a90: 456e 7469 7479 2052 6573 6f6c 7574 696f  Entity Resolutio
+00000aa0: 6e20 7072 6f62 6c65 6d73 2e20 4974 2069  n problems. It i
+00000ab0: 7320 6275 696c 6465 6420 7573 696e 6720  s builded using 
+00000ac0: 7374 6174 652d 6f66 2d74 6865 2d61 7274  state-of-the-art
+00000ad0: 2070 7974 686f 6e20 6672 616d 6577 6f72   python framewor
+00000ae0: 6b73 2e20 7079 4a65 6441 4920 636f 6e73  ks. pyJedAI cons
+00000af0: 7469 7475 7465 7320 7468 6520 736f 6c65  titutes the sole
+00000b00: 206f 7065 6e2d 736f 7572 6365 204c 696e   open-source Lin
+00000b10: 6b20 4469 7363 6f76 6572 7920 746f 6f6c  k Discovery tool
+00000b20: 2074 6861 7420 6973 2063 6170 6162 6c65   that is capable
+00000b30: 206f 6620 6578 706c 6f69 7469 6e67 2074   of exploiting t
+00000b40: 6865 206c 6174 6573 7420 6272 6561 6b74  he latest breakt
+00000b50: 6872 6f75 6768 7320 696e 2044 6565 7020  hroughs in Deep 
+00000b60: 4c65 6172 6e69 6e67 2061 6e64 204e 4c50  Learning and NLP
+00000b70: 2074 6563 686e 6971 7565 732c 2077 6869   techniques, whi
+00000b80: 6368 2061 7265 2070 7562 6c69 636c 7920  ch are publicly 
+00000b90: 6176 6169 6c61 626c 6520 7468 726f 7567  available throug
+00000ba0: 6820 7468 6520 5079 7468 6f6e 2064 6174  h the Python dat
+00000bb0: 6120 7363 6965 6e63 6520 6563 6f73 7973  a science ecosys
+00000bc0: 7465 6d2e 2054 6869 7320 6170 706c 6965  tem. This applie
+00000bd0: 7320 746f 2062 6f74 6820 626c 6f63 6b69  s to both blocki
+00000be0: 6e67 2061 6e64 206d 6174 6368 696e 672c  ng and matching,
+00000bf0: 2074 6875 7320 656e 7375 7269 6e67 2068   thus ensuring h
+00000c00: 6967 6820 7469 6d65 2065 6666 6963 6965  igh time efficie
+00000c10: 6e63 792c 2068 6967 6820 7363 616c 6162  ncy, high scalab
+00000c20: 696c 6974 7920 6173 2077 656c 6c20 6173  ility as well as
+00000c30: 2068 6967 6820 6566 6665 6374 6976 656e   high effectiven
+00000c40: 6573 732c 2077 6974 686f 7574 2072 6571  ess, without req
+00000c50: 7569 7269 6e67 2061 6e79 206c 6162 656c  uiring any label
+00000c60: 6c65 6420 696e 7374 616e 6365 7320 6672  led instances fr
+00000c70: 6f6d 2074 6865 2075 7365 722e 0a0a 2323  om the user...##
+00000c80: 2320 4b65 792d 4665 6174 7572 6573 0a0a  # Key-Features..
+00000c90: 2d20 496e 7075 7420 6461 7461 2d74 7970  - Input data-typ
+00000ca0: 6520 696e 6465 7065 6e64 656e 742e 2042  e independent. B
+00000cb0: 6f74 6820 7374 7275 6374 7572 6564 2061  oth structured a
+00000cc0: 6e64 2073 656d 692d 7374 7275 6374 7572  nd semi-structur
+00000cd0: 6564 2064 6174 6120 6361 6e20 6265 2070  ed data can be p
+00000ce0: 726f 6365 7373 6564 2e0a 2d20 5661 7269  rocessed..- Vari
+00000cf0: 6f75 7320 696d 706c 656d 656e 7465 6420  ous implemented 
+00000d00: 616c 676f 7269 7468 6d73 2e0a 2d20 4561  algorithms..- Ea
+00000d10: 7379 2d74 6f2d 7573 652e 0a2d 2055 7469  sy-to-use..- Uti
+00000d20: 6c69 7a65 7320 736f 6d65 206f 6620 7468  lizes some of th
+00000d30: 6520 6661 6d6f 7573 2061 6e64 2063 7574  e famous and cut
+00000d40: 7469 6e67 2d65 6467 6520 6d61 6368 696e  ting-edge machin
+00000d50: 6520 6c65 6172 6e69 6e67 2070 6163 6b61  e learning packa
+00000d60: 6765 732e 0a2d 204f 6666 6572 7320 7375  ges..- Offers su
+00000d70: 7065 7276 6973 6564 2061 6e64 2075 6e2d  pervised and un-
+00000d80: 7375 7065 7276 6973 6564 204d 4c20 7465  supervised ML te
+00000d90: 6368 6e69 7175 6573 2e0a 0a5f 5f4f 7065  chniques...__Ope
+00000da0: 6e20 6465 6d6f 7320 6172 6520 6176 6169  n demos are avai
+00000db0: 6c61 626c 6520 696e 3a5f 5f0a 0a3c 6469  lable in:__..<di
+00000dc0: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
+00000dd0: 3e0a 2020 2020 3c61 2068 7265 663d 2268  >.    <a href="h
+00000de0: 7474 7073 3a2f 2f6e 6276 6965 7765 722e  ttps://nbviewer.
+00000df0: 6f72 672f 6769 7468 7562 2f41 492d 7465  org/github/AI-te
+00000e00: 616d 2d55 6f41 2f70 794a 6564 4149 2f62  am-UoA/pyJedAI/b
+00000e10: 6c6f 622f 6d61 696e 2f64 6f63 732f 7475  lob/main/docs/tu
+00000e20: 746f 7269 616c 732f 4465 6d6f 2e69 7079  torials/Demo.ipy
+00000e30: 6e62 223e 0a20 2020 2020 2020 203c 696d  nb">.        <im
+00000e40: 6720 616c 6967 6e3d 2263 656e 7465 7222  g align="center"
+00000e50: 2073 7263 3d22 6874 7470 733a 2f2f 6e62   src="https://nb
+00000e60: 7669 6577 6572 2e6f 7267 2f73 7461 7469  viewer.org/stati
+00000e70: 632f 696d 672f 6e61 765f 6c6f 676f 2e73  c/img/nav_logo.s
+00000e80: 7667 2220 7769 6474 683d 3132 302f 3e20  vg" width=120/> 
+00000e90: 0a20 2020 203c 2f61 3e20 2026 6e62 7370  .    </a>  &nbsp
+00000ea0: 3b26 6e62 7370 3b26 6e62 7370 3b26 6e62  ;&nbsp;&nbsp;&nb
+00000eb0: 7370 3b26 6e62 7370 3b26 6e62 7370 3b26  sp;&nbsp;&nbsp;&
+00000ec0: 6e62 7370 3b0a 2020 2020 3c61 2068 7265  nbsp;.    <a hre
+00000ed0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00000ee0: 622e 636f 6d2f 4149 2d74 6561 6d2d 556f  b.com/AI-team-Uo
+00000ef0: 412f 7079 4a65 6441 492f 626c 6f62 2f6d  A/pyJedAI/blob/m
+00000f00: 6169 6e2f 646f 6373 2f74 7574 6f72 6961  ain/docs/tutoria
+00000f10: 6c73 2f44 656d 6f2e 6970 796e 6222 3e0a  ls/Demo.ipynb">.
+00000f20: 2020 2020 2020 2020 3c69 6d67 2061 6c69          <img ali
+00000f30: 676e 3d22 6365 6e74 6572 2220 7372 633d  gn="center" src=
+00000f40: 2268 7474 7073 3a2f 2f6d 6972 6f2e 6d65  "https://miro.me
+00000f50: 6469 756d 2e63 6f6d 2f6d 6178 2f31 3430  dium.com/max/140
+00000f60: 302f 312a 4564 6e5f 4c70 6253 704c 654e  0/1*Edn_LpbSpLeN
+00000f70: 4b66 576b 4564 4732 4a67 2e70 6e67 2220  KfWkEdG2Jg.png" 
+00000f80: 7769 6474 683d 3132 302f 3e20 0a20 2020  width=120/> .   
+00000f90: 203c 2f61 3e0a 3c2f 6469 763e 0a0a 5f5f   </a>.</div>..__
+00000fa0: 476f 6f67 6c65 2043 6f6c 6162 2048 616e  Google Colab Han
+00000fb0: 6473 2d6f 6e20 6465 6d6f 3a5f 5f20 0a0a  ds-on demo:__ ..
+00000fc0: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00000fd0: 6572 223e 0a20 2020 203c 6120 6872 6566  er">.    <a href
+00000fe0: 3d22 6874 7470 733a 2f2f 636f 6c61 622e  ="https://colab.
+00000ff0: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
+00001000: 636f 6d2f 6472 6976 652f 3138 5667 454f  com/drive/18VgEO
+00001010: 4b41 6332 4f62 4646 7844 4e62 3273 6a68  KAc2ObFFxDNb2sjh
+00001020: 424c 4b4b 734e 7666 4550 6f3f 7573 703d  BLKKsNvfEPo?usp=
+00001030: 7368 6172 696e 6722 3e0a 2020 2020 2020  sharing">.      
+00001040: 2020 3c69 6d67 2061 6c69 676e 3d22 6365    <img align="ce
+00001050: 6e74 6572 2220 7372 633d 2268 7474 7073  nter" src="https
+00001060: 3a2f 2f33 2e62 702e 626c 6f67 7370 6f74  ://3.bp.blogspot
+00001070: 2e63 6f6d 2f2d 6170 6f42 6557 4679 634b  .com/-apoBeWFycK
+00001080: 512f 5868 4b42 3866 4570 7277 492f 4141  Q/XhKB8fEprwI/AA
+00001090: 4141 4141 4141 434d 342f 536c 3736 797a  AAAAAACM4/Sl76yz
+000010a0: 4e53 4e59 776c 5368 4942 7268 6544 4175  NSNYwlShIBrheDAu
+000010b0: 6d38 4c39 7152 7457 4e64 6743 4c63 4247  m8L9qRtWNdgCLcBG
+000010c0: 4173 5948 512f 7331 3630 302f 636f 6c61  AsYHQ/s1600/cola
+000010d0: 622e 706e 6722 2077 6964 7468 3d31 3230  b.png" width=120
+000010e0: 2f3e 200a 2020 2020 3c2f 613e 0a3c 2f64  /> .    </a>.</d
+000010f0: 6976 3e0a 0a23 2049 6e73 7461 6c6c 0a0a  iv>..# Install..
+00001100: 7079 4a65 6441 4920 6861 7320 6265 656e  pyJedAI has been
+00001110: 2074 6573 7465 6420 696e 2057 696e 646f   tested in Windo
+00001120: 7773 2061 6e64 204c 696e 7578 204f 532e  ws and Linux OS.
+00001130: 200a 0a5f 5f42 6173 6963 2072 6571 7569   ..__Basic requi
+00001140: 7265 6d65 6e74 733a 5f5f 0a0a 2d20 5079  rements:__..- Py
+00001150: 7468 6f6e 2076 6572 7369 6f6e 2067 7265  thon version gre
+00001160: 6174 6572 206f 7220 6571 7561 6c20 746f  ater or equal to
+00001170: 202a 2a33 2e38 2a2a 2e0a 2d20 466f 7220   **3.8**..- For 
+00001180: 5769 6e64 6f77 732c 204d 6963 726f 736f  Windows, Microso
+00001190: 6674 2056 6973 7561 6c20 432b 2b20 3134  ft Visual C++ 14
+000011a0: 2e30 2069 7320 7265 7175 6972 6564 2e20  .0 is required. 
+000011b0: 446f 776e 6c6f 6164 2069 7420 6672 6f6d  Download it from
+000011c0: 205b 4d69 6372 6f73 6f66 7420 4f66 6669   [Microsoft Offi
+000011d0: 6369 616c 2073 6974 655d 2868 7474 7073  cial site](https
+000011e0: 3a2f 2f76 6973 7561 6c73 7475 6469 6f2e  ://visualstudio.
+000011f0: 6d69 6372 6f73 6f66 742e 636f 6d2f 7669  microsoft.com/vi
+00001200: 7375 616c 2d63 7070 2d62 7569 6c64 2d74  sual-cpp-build-t
+00001210: 6f6f 6c73 2f29 2e0a 0a23 2323 2050 7950  ools/)...### PyP
+00001220: 490a 496e 7374 616c 6c20 7468 6520 6c61  I.Install the la
+00001230: 7465 7374 2076 6572 7369 6f6e 206f 6620  test version of 
+00001240: 7079 6a65 6461 693a 0a60 6060 0a70 6970  pyjedai:.```.pip
+00001250: 2069 6e73 7461 6c6c 2070 796a 6564 6169   install pyjedai
+00001260: 0a60 6060 0a4d 6f72 6520 6f6e 205b 5079  .```.More on [Py
+00001270: 5049 5d28 6874 7470 733a 2f2f 7079 7069  PI](https://pypi
+00001280: 2e6f 7267 2f70 726f 6a65 6374 2f70 796a  .org/project/pyj
+00001290: 6564 6169 292e 0a0a 2323 2320 4769 740a  edai)...### Git.
+000012a0: 0a53 6574 2075 7020 6c6f 6361 6c6c 793a  .Set up locally:
+000012b0: 0a60 6060 0a67 6974 2063 6c6f 6e65 2068  .```.git clone h
+000012c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000012d0: 6d2f 4149 2d74 6561 6d2d 556f 412f 7079  m/AI-team-UoA/py
+000012e0: 4a65 6441 492e 6769 740a 6060 600a 676f  JedAI.git.```.go
+000012f0: 2074 6f20 7468 6520 726f 6f74 2064 6972   to the root dir
+00001300: 6563 746f 7279 2077 6974 6820 6063 6420  ectory with `cd 
+00001310: 7079 4a65 6441 4960 2061 6e64 2074 7970  pyJedAI` and typ
+00001320: 653a 0a60 6060 0a70 6970 2069 6e73 7461  e:.```.pip insta
+00001330: 6c6c 202e 0a60 6060 0a0a 2323 2320 446f  ll ..```..### Do
+00001340: 636b 6572 0a0a 4176 6169 6c61 626c 6520  cker..Available 
+00001350: 6174 205b 446f 636b 6572 2048 7562 5d28  at [Docker Hub](
+00001360: 6874 7470 733a 2f2f 6875 622e 646f 636b  https://hub.dock
+00001370: 6572 2e63 6f6d 2f72 2f61 6974 6561 6d75  er.com/r/aiteamu
+00001380: 6f61 2f70 796a 6564 6169 292c 206f 7220  oa/pyjedai), or 
+00001390: 636c 6f6e 6520 7468 6973 2072 6570 6f20  clone this repo 
+000013a0: 616e 643a 0a60 6060 0a64 6f63 6b65 7220  and:.```.docker 
+000013b0: 6275 696c 6420 2d66 2044 6f63 6b65 7266  build -f Dockerf
+000013c0: 696c 650a 6060 600a 0a23 2044 6570 656e  ile.```..# Depen
+000013d0: 6465 6e63 6965 730a 0a3c 6469 7620 616c  dencies..<div al
+000013e0: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+000013f0: 2020 3c69 6d67 2061 6c69 676e 3d22 6365    <img align="ce
+00001400: 6e74 6572 2220 7372 633d 2268 7474 7073  nter" src="https
+00001410: 3a2f 2f75 706c 6f61 642e 7769 6b69 6d65  ://upload.wikime
+00001420: 6469 612e 6f72 672f 7769 6b69 7065 6469  dia.org/wikipedi
+00001430: 612f 636f 6d6d 6f6e 732f 7468 756d 622f  a/commons/thumb/
+00001440: 652f 6564 2f50 616e 6461 735f 6c6f 676f  e/ed/Pandas_logo
+00001450: 2e73 7667 2f32 3536 3070 782d 5061 6e64  .svg/2560px-Pand
+00001460: 6173 5f6c 6f67 6f2e 7376 672e 706e 6722  as_logo.svg.png"
+00001470: 2077 6964 7468 3d31 3230 2f3e 2026 6e62   width=120/> &nb
+00001480: 7370 3b26 6e62 7370 3b0a 2020 2020 3c69  sp;&nbsp;.    <i
+00001490: 6d67 2061 6c69 676e 3d22 6365 6e74 6572  mg align="center
+000014a0: 2220 7372 633d 2268 7474 7073 3a2f 2f75  " src="https://u
+000014b0: 706c 6f61 642e 7769 6b69 6d65 6469 612e  pload.wikimedia.
+000014c0: 6f72 672f 7769 6b69 7065 6469 612f 636f  org/wikipedia/co
+000014d0: 6d6d 6f6e 732f 7468 756d 622f 332f 3331  mmons/thumb/3/31
+000014e0: 2f4e 756d 5079 5f6c 6f67 6f5f 3230 3230  /NumPy_logo_2020
+000014f0: 2e73 7667 2f31 3238 3070 782d 4e75 6d50  .svg/1280px-NumP
+00001500: 795f 6c6f 676f 5f32 3032 302e 7376 672e  y_logo_2020.svg.
+00001510: 706e 6722 2077 6964 7468 3d31 3230 2f3e  png" width=120/>
+00001520: 2026 6e62 7370 3b26 6e62 7370 3b0a 2020   &nbsp;&nbsp;.  
+00001530: 2020 3c69 6d67 2061 6c69 676e 3d22 6365    <img align="ce
+00001540: 6e74 6572 2220 7372 633d 2268 7474 7073  nter" src="https
+00001550: 3a2f 2f6c 6f67 6f65 7073 2e63 6f6d 2f77  ://logoeps.com/w
+00001560: 702d 636f 6e74 656e 742f 7570 6c6f 6164  p-content/upload
+00001570: 732f 3230 3132 2f31 302f 7079 7468 6f6e  s/2012/10/python
+00001580: 2d6c 6f67 6f2d 7665 6374 6f72 2e70 6e67  -logo-vector.png
+00001590: 2220 7769 6474 683d 3132 302f 3e20 266e  " width=120/> &n
+000015a0: 6273 703b 266e 6273 703b 266e 6273 703b  bsp;&nbsp;&nbsp;
+000015b0: 0a20 2020 203c 696d 6720 616c 6967 6e3d  .    <img align=
+000015c0: 2263 656e 7465 7222 2073 7263 3d22 6874  "center" src="ht
+000015d0: 7470 733a 2f2f 7570 6c6f 6164 2e77 696b  tps://upload.wik
+000015e0: 696d 6564 6961 2e6f 7267 2f77 696b 6970  imedia.org/wikip
+000015f0: 6564 6961 2f63 6f6d 6d6f 6e73 2f74 6875  edia/commons/thu
+00001600: 6d62 2f33 2f33 382f 4a75 7079 7465 725f  mb/3/38/Jupyter_
+00001610: 6c6f 676f 2e73 7667 2f38 3833 7078 2d4a  logo.svg/883px-J
+00001620: 7570 7974 6572 5f6c 6f67 6f2e 7376 672e  upyter_logo.svg.
+00001630: 706e 6722 2077 6964 7468 3d37 302f 3e20  png" width=70/> 
+00001640: 203c 6272 3e0a 2020 2020 3c69 6d67 2061   <br>.    <img a
+00001650: 6c69 676e 3d22 6365 6e74 6572 2220 7372  lign="center" sr
+00001660: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00001670: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00001680: 2e63 6f6d 2f6f 7074 756e 612f 6f70 7475  .com/optuna/optu
+00001690: 6e61 2f6d 6173 7465 722f 646f 6373 2f69  na/master/docs/i
+000016a0: 6d61 6765 2f6f 7074 756e 612d 6c6f 676f  mage/optuna-logo
+000016b0: 2e70 6e67 2220 7769 6474 683d 3135 302f  .png" width=150/
+000016c0: 3e0a 2020 2020 3c69 6d67 2061 6c69 676e  >.    <img align
+000016d0: 3d22 6365 6e74 6572 2220 7372 633d 2268  ="center" src="h
+000016e0: 7474 7073 3a2f 2f75 706c 6f61 642e 7769  ttps://upload.wi
+000016f0: 6b69 6d65 6469 612e 6f72 672f 7769 6b69  kimedia.org/wiki
+00001700: 7065 6469 612f 636f 6d6d 6f6e 732f 7468  pedia/commons/th
+00001710: 756d 622f 382f 3861 2f50 6c6f 746c 795f  umb/8/8a/Plotly_
+00001720: 6c6f 676f 5f66 6f72 5f64 6967 6974 616c  logo_for_digital
+00001730: 5f66 696e 616c 5f25 3238 3625 3239 2e70  _final_%286%29.p
+00001740: 6e67 2f31 3230 3070 782d 506c 6f74 6c79  ng/1200px-Plotly
+00001750: 5f6c 6f67 6f5f 666f 725f 6469 6769 7461  _logo_for_digita
+00001760: 6c5f 6669 6e61 6c5f 2532 3836 2532 392e  l_final_%286%29.
+00001770: 706e 6722 2077 6964 7468 3d31 3530 2f3e  png" width=150/>
+00001780: 0a20 2020 203c 696d 6720 616c 6967 6e3d  .    <img align=
+00001790: 2263 656e 7465 7222 2073 7263 3d22 6874  "center" src="ht
+000017a0: 7470 733a 2f2f 7079 746f 7263 682e 6f72  tps://pytorch.or
+000017b0: 672f 7475 746f 7269 616c 732f 5f73 7461  g/tutorials/_sta
+000017c0: 7469 632f 696d 672f 7468 756d 626e 6169  tic/img/thumbnai
+000017d0: 6c73 2f63 726f 7070 6564 2f70 726f 6669  ls/cropped/profi
+000017e0: 6c65 722e 706e 6722 2077 6964 7468 3d31  ler.png" width=1
+000017f0: 3630 2f3e 200a 2020 2020 3c69 6d67 2061  60/> .    <img a
+00001800: 6c69 676e 3d22 6365 6e74 6572 2220 7372  lign="center" sr
+00001810: 633d 2268 7474 7073 3a2f 2f77 7777 2e66  c="https://www.f
+00001820: 756c 6c73 7461 636b 7079 7468 6f6e 2e63  ullstackpython.c
+00001830: 6f6d 2f69 6d67 2f6c 6f67 6f73 2f73 6369  om/img/logos/sci
+00001840: 7079 2e70 6e67 2220 7769 6474 683d 3135  py.png" width=15
+00001850: 302f 3e20 203c 6272 3e3c 6272 3e0a 2020  0/>  <br><br>.  
+00001860: 2020 3c69 6d67 2061 6c69 676e 3d22 6365    <img align="ce
+00001870: 6e74 6572 2220 7372 633d 2268 7474 7073  nter" src="https
+00001880: 3a2f 2f77 7777 2e6b 6f72 6e6f 736b 2e6d  ://www.kornosk.m
+00001890: 652f 7265 736f 7572 6365 732f 6c61 6e67  e/resources/lang
+000018a0: 7561 6765 2d6d 6f64 656c 2f66 6561 7475  uage-model/featu
+000018b0: 7265 642e 706e 6722 2077 6964 7468 3d31  red.png" width=1
+000018c0: 3530 2f3e 2026 6e62 7370 3b26 6e62 7370  50/> &nbsp;&nbsp
+000018d0: 3b26 6e62 7370 3b0a 2020 2020 3c69 6d67  ;&nbsp;.    <img
+000018e0: 2061 6c69 676e 3d22 6365 6e74 6572 2220   align="center" 
+000018f0: 7372 633d 2268 7474 7073 3a2f 2f72 6570  src="https://rep
+00001900: 6f73 6974 6f72 792d 696d 6167 6573 2e67  ository-images.g
+00001910: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00001920: 2e63 6f6d 2f31 3334 3937 3735 2f32 3032  .com/1349775/202
+00001930: 6334 3638 302d 3866 3763 2d31 3165 392d  c4680-8f7c-11e9-
+00001940: 3931 6336 2d37 3435 6664 6362 6566 6665  91c6-745fdcbeffe
+00001950: 3822 2077 6964 7468 3d31 3530 2f3e 2026  8" width=150/> &
+00001960: 6e62 7370 3b26 6e62 7370 3b26 6e62 7370  nbsp;&nbsp;&nbsp
+00001970: 3b0a 2020 2020 3c69 6d67 2061 6c69 676e  ;.    <img align
+00001980: 3d22 6365 6e74 6572 2220 7372 633d 2268  ="center" src="h
+00001990: 7474 7073 3a2f 2f6e 6574 776f 726b 782e  ttps://networkx.
+000019a0: 6f72 672f 5f73 7461 7469 632f 6e65 7477  org/_static/netw
+000019b0: 6f72 6b78 5f6c 6f67 6f2e 7376 6722 2077  orkx_logo.svg" w
+000019c0: 6964 7468 3d31 3530 2f3e 2026 6e62 7370  idth=150/> &nbsp
+000019d0: 3b26 6e62 7370 3b26 6e62 7370 3b0a 2020  ;&nbsp;&nbsp;.  
+000019e0: 2020 3c69 6d67 2061 6c69 676e 3d22 6365    <img align="ce
+000019f0: 6e74 6572 2220 7372 633d 2268 7474 7073  nter" src="https
+00001a00: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00001a10: 7263 6f6e 7465 6e74 2e63 6f6d 2f52 4446  rcontent.com/RDF
+00001a20: 4c69 622f 4f57 4c2d 524c 2f6d 6173 7465  Lib/OWL-RL/maste
+00001a30: 722f 4f57 4c2d 524c 2e70 6e67 2220 7769  r/OWL-RL.png" wi
+00001a40: 6474 683d 3730 2f3e 200a 3c2f 6469 763e  dth=70/> .</div>
+00001a50: 0a3c 6272 3e0a 0a53 6565 2074 6865 2066  .<br>..See the f
+00001a60: 756c 6c20 6c69 7374 206f 6620 6465 7065  ull list of depe
+00001a70: 6e64 656e 6369 6573 2061 6e64 2061 6c6c  ndencies and all
+00001a80: 2076 6572 7369 6f6e 7320 7573 6564 2c20   versions used, 
+00001a90: 696e 2074 6869 7320 5b66 696c 655d 2868  in this [file](h
+00001aa0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001ab0: 6d2f 4149 2d74 6561 6d2d 556f 412f 7079  m/AI-team-UoA/py
+00001ac0: 4a65 6441 492f 626c 6f62 2f6d 6169 6e2f  JedAI/blob/main/
+00001ad0: 7079 7072 6f6a 6563 742e 746f 6d6c 292e  pyproject.toml).
+00001ae0: 0a0a 5f5f 5374 6174 7573 5f5f 0a0a 5b21  ..__Status__..[!
+00001af0: 5b54 6573 7473 5d28 6874 7470 733a 2f2f  [Tests](https://
+00001b00: 6769 7468 7562 2e63 6f6d 2f41 492d 7465  github.com/AI-te
+00001b10: 616d 2d55 6f41 2f70 794a 6564 4149 2f61  am-UoA/pyJedAI/a
+00001b20: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+00001b30: 2f74 6573 7473 2e79 6d6c 2f62 6164 6765  /tests.yml/badge
+00001b40: 2e73 7667 3f62 7261 6e63 683d 6d61 696e  .svg?branch=main
+00001b50: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00001b60: 622e 636f 6d2f 4149 2d74 6561 6d2d 556f  b.com/AI-team-Uo
+00001b70: 412f 7079 4a65 6441 492f 6163 7469 6f6e  A/pyJedAI/action
+00001b80: 732f 776f 726b 666c 6f77 732f 7465 7374  s/workflows/test
+00001b90: 732e 796d 6c29 0a5b 215b 5079 5069 5d28  s.yml).[![PyPi](
+00001ba0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001bb0: 6f6d 2f41 492d 7465 616d 2d55 6f41 2f70  om/AI-team-UoA/p
+00001bc0: 794a 6564 4149 2f61 6374 696f 6e73 2f77  yJedAI/actions/w
+00001bd0: 6f72 6b66 6c6f 7773 2f70 7970 692d 7075  orkflows/pypi-pu
+00001be0: 626c 6973 682e 796d 6c2f 6261 6467 652e  blish.yml/badge.
+00001bf0: 7376 6729 5d28 6874 7470 733a 2f2f 6769  svg)](https://gi
+00001c00: 7468 7562 2e63 6f6d 2f41 492d 7465 616d  thub.com/AI-team
+00001c10: 2d55 6f41 2f70 794a 6564 4149 2f61 6374  -UoA/pyJedAI/act
+00001c20: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f70  ions/workflows/p
+00001c30: 7970 692d 7075 626c 6973 682e 796d 6c29  ypi-publish.yml)
+00001c40: 0a5b 215b 6d61 6465 2d77 6974 682d 7079  .[![made-with-py
+00001c50: 7468 6f6e 5d28 6874 7470 733a 2f2f 7265  thon](https://re
+00001c60: 6164 7468 6564 6f63 732e 6f72 672f 7072  adthedocs.org/pr
+00001c70: 6f6a 6563 7473 2f70 796a 6564 6169 2f62  ojects/pyjedai/b
+00001c80: 6164 6765 2f3f 7665 7273 696f 6e3d 6c61  adge/?version=la
+00001c90: 7465 7374 295d 2868 7474 7073 3a2f 2f70  test)](https://p
+00001ca0: 796a 6564 6169 2e72 6561 6474 6865 646f  yjedai.readthedo
+00001cb0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00001cc0: 3f62 6164 6765 3d6c 6174 6573 7429 0a5b  ?badge=latest).[
+00001cd0: 215b 636f 6465 636f 765d 2868 7474 7073  ![codecov](https
+00001ce0: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
+00001cf0: 2f41 492d 7465 616d 2d55 6f41 2f70 796a  /AI-team-UoA/pyj
+00001d00: 6564 6169 2f62 7261 6e63 682f 6d61 7374  edai/branch/mast
+00001d10: 6572 2f67 7261 7068 2f62 6164 6765 2e73  er/graph/badge.s
+00001d20: 7667 3f74 6f6b 656e 3d34 5152 3058 3331  vg?token=4QR0X31
+00001d30: 3543 4c29 5d28 6874 7470 733a 2f2f 636f  5CL)](https://co
+00001d40: 6465 636f 762e 696f 2f67 682f 4149 2d74  decov.io/gh/AI-t
+00001d50: 6561 6d2d 556f 412f 7079 6a65 6461 6929  eam-UoA/pyjedai)
+00001d60: 0a0a 0a5f 5f53 7461 7469 7374 6963 7320  ...__Statistics 
+00001d70: 2620 496e 666f 5f5f 0a0a 215b 5079 5049  & Info__..![PyPI
+00001d80: 202d 2044 6f77 6e6c 6f61 6473 5d28 6874   - Downloads](ht
+00001d90: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00001da0: 732e 696f 2f70 7970 692f 646d 2f70 796a  s.io/pypi/dm/pyj
+00001db0: 6564 6169 290a 5b21 5b50 7950 4920 7665  edai).[![PyPI ve
+00001dc0: 7273 696f 6e5d 2868 7474 7073 3a2f 2f69  rsion](https://i
+00001dd0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00001de0: 7069 2f76 2f70 796a 6564 6169 2e73 7667  pi/v/pyjedai.svg
+00001df0: 3f6c 6f67 6f3d 7079 7069 266c 6f67 6f43  ?logo=pypi&logoC
+00001e00: 6f6c 6f72 3d46 4645 3837 3329 5d28 6874  olor=FFE873)](ht
+00001e10: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00001e20: 726f 6a65 6374 2f70 796a 6564 6169 2f29  roject/pyjedai/)
+00001e30: 0a0a 0a23 2042 7567 732c 2044 6973 6375  ...# Bugs, Discu
+00001e40: 7373 696f 6e73 2026 204e 6577 730a 0a5b  ssions & News..[
+00001e50: 4769 7448 7562 2044 6973 6375 7373 696f  GitHub Discussio
+00001e60: 6e73 5d28 6874 7470 733a 2f2f 6769 7468  ns](https://gith
+00001e70: 7562 2e63 6f6d 2f41 492d 7465 616d 2d55  ub.com/AI-team-U
+00001e80: 6f41 2f70 794a 6564 4149 2f64 6973 6375  oA/pyJedAI/discu
+00001e90: 7373 696f 6e73 2920 6973 2074 6865 2064  ssions) is the d
+00001ea0: 6973 6375 7373 696f 6e20 666f 7275 6d20  iscussion forum 
+00001eb0: 666f 7220 6765 6e65 7261 6c20 7175 6573  for general ques
+00001ec0: 7469 6f6e 7320 616e 6420 6469 7363 7573  tions and discus
+00001ed0: 7369 6f6e 7320 616e 6420 6f75 7220 7265  sions and our re
+00001ee0: 636f 6d6d 656e 6465 6420 7374 6172 7469  commended starti
+00001ef0: 6e67 2070 6f69 6e74 2e20 506c 6561 7365  ng point. Please
+00001f00: 2072 6570 6f72 7420 616e 7920 6275 6773   report any bugs
+00001f10: 2074 6861 7420 796f 7520 6669 6e64 205b   that you find [
+00001f20: 6865 7265 5d28 6874 7470 733a 2f2f 6769  here](https://gi
+00001f30: 7468 7562 2e63 6f6d 2f41 492d 7465 616d  thub.com/AI-team
+00001f40: 2d55 6f41 2f70 794a 6564 4149 2f69 7373  -UoA/pyJedAI/iss
+00001f50: 7565 7329 2e0a 0a23 204a 6176 6120 2d20  ues)...# Java - 
+00001f60: 5765 6220 4170 706c 6963 6174 696f 6e20  Web Application 
+00001f70: 0a0a 3c69 6d67 2061 6c69 676e 3d22 6c65  ..<img align="le
+00001f80: 6674 2220 7372 633d 2268 7474 7073 3a2f  ft" src="https:/
+00001f90: 2f67 6974 6875 622e 636f 6d2f 7363 6966  /github.com/scif
+00001fa0: 792f 4a65 6441 4954 6f6f 6c6b 6974 2f62  y/JedAIToolkit/b
+00001fb0: 6c6f 622f 6d61 7374 6572 2f64 6f63 756d  lob/master/docum
+00001fc0: 656e 7461 7469 6f6e 2f4a 6564 4149 5f6c  entation/JedAI_l
+00001fd0: 6f67 6f2e 706e 673f 7261 773d 7472 7565  ogo.png?raw=true
+00001fe0: 2220 616c 743d 2270 794a 6564 4149 2220  " alt="pyJedAI" 
+00001ff0: 7769 6474 683d 2231 3330 222f 3e0a 0a46  width="130"/>..F
+00002000: 6f72 204a 6176 6120 7573 6572 7320 6368  or Java users ch
+00002010: 6563 6b6f 7574 2074 6865 2069 6e69 7469  eckout the initi
+00002020: 616c 205b 4a65 6441 495d 2868 7474 7073  al [JedAI](https
+00002030: 3a2f 2f67 6974 6875 622e 636f 6d2f 7363  ://github.com/sc
+00002040: 6966 792f 4a65 6441 4954 6f6f 6c6b 6974  ify/JedAIToolkit
+00002050: 292e 2054 6865 7265 2079 6f75 2063 616e  ). There you can
+00002060: 2066 696e 6420 4a61 7661 2062 6173 6564   find Java based
+00002070: 2063 6f64 6520 616e 6420 6120 5765 6220   code and a Web 
+00002080: 4170 706c 6963 6174 696f 6e20 666f 7220  Application for 
+00002090: 696e 7465 7261 6374 6976 6520 6372 6561  interactive crea
+000020a0: 7469 6f6e 206f 6620 4552 2077 6f72 6b66  tion of ER workf
+000020b0: 6c6f 7773 2e20 3c62 723e 3c62 723e 204a  lows. <br><br> J
+000020c0: 6564 4149 2063 6f6e 7374 6974 7574 6573  edAI constitutes
+000020d0: 2061 6e20 6f70 656e 2073 6f75 7263 652c   an open source,
+000020e0: 2068 6967 6820 7363 616c 6162 696c 6974   high scalabilit
+000020f0: 7920 746f 6f6c 6b69 7420 7468 6174 206f  y toolkit that o
+00002100: 6666 6572 7320 6f75 742d 6f66 2d74 6865  ffers out-of-the
+00002110: 2d62 6f78 2073 6f6c 7574 696f 6e73 2066  -box solutions f
+00002120: 6f72 2061 6e79 2064 6174 6120 696e 7465  or any data inte
+00002130: 6772 6174 696f 6e20 7461 736b 2c20 652e  gration task, e.
+00002140: 672e 2c20 5265 636f 7264 204c 696e 6b61  g., Record Linka
+00002150: 6765 2c20 456e 7469 7479 2052 6573 6f6c  ge, Entity Resol
+00002160: 7574 696f 6e20 616e 6420 4c69 6e6b 2044  ution and Link D
+00002170: 6973 636f 7665 7279 2e20 4174 2069 7473  iscovery. At its
+00002180: 2063 6f72 6520 6c69 6573 2061 2073 6574   core lies a set
+00002190: 206f 6620 646f 6d61 696e 2d69 6e64 6570   of domain-indep
+000021a0: 656e 6465 6e74 2c20 7374 6174 652d 6f66  endent, state-of
+000021b0: 2d74 6865 2d61 7274 2074 6563 686e 6971  -the-art techniq
+000021c0: 7565 7320 7468 6174 2061 7070 6c79 2074  ues that apply t
+000021d0: 6f20 626f 7468 2052 4446 2061 6e64 2072  o both RDF and r
+000021e0: 656c 6174 696f 6e61 6c20 6461 7461 2e0a  elational data..
+000021f0: 0a3c 6272 3e0a 0a23 2054 6561 6d20 2620  .<br>..# Team & 
+00002200: 4175 7468 6f72 730a 0a3c 696d 6720 616c  Authors..<img al
+00002210: 6967 6e3d 2272 6967 6874 2220 7372 633d  ign="right" src=
+00002220: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00002230: 636f 6d2f 4149 2d74 6561 6d2d 556f 412f  com/AI-team-UoA/
+00002240: 2e67 6974 6875 622f 626c 6f62 2f6d 6169  .github/blob/mai
+00002250: 6e2f 4149 5f4c 4f47 4f2e 706e 673f 7261  n/AI_LOGO.png?ra
+00002260: 773d 7472 7565 2220 616c 743d 2270 794a  w=true" alt="pyJ
+00002270: 6564 4149 2220 7769 6474 683d 2232 3030  edAI" width="200
+00002280: 222f 3e0a 0a2d 205b 4b6f 6e73 7461 6e74  "/>..- [Konstant
+00002290: 696e 6f73 204e 696b 6f6c 6574 6f73 5d28  inos Nikoletos](
+000022a0: 6874 7470 733a 2f2f 6e69 6b6f 6c65 746f  https://nikoleto
+000022b0: 732d 6b2e 6769 7468 7562 2e69 6f29 2c20  s-k.github.io), 
+000022c0: 5265 7365 6172 6368 2041 7373 6f63 6961  Research Associa
+000022d0: 7465 2061 7420 556e 6976 6572 7369 7479  te at University
+000022e0: 206f 6620 4174 6865 6e73 2c20 4772 6565   of Athens, Gree
+000022f0: 6365 0a2d 205b 4a61 6b75 6220 4d61 6369  ce.- [Jakub Maci
+00002300: 656a 6577 736b 695d 2868 7474 7073 3a2f  ejewski](https:/
+00002310: 2f77 7777 2e6c 696e 6b65 6469 6e2e 636f  /www.linkedin.co
+00002320: 6d2f 696e 2f6a 616b 7562 2d6d 6163 6965  m/in/jakub-macie
+00002330: 6a65 7773 6b69 2d30 3237 3032 3931 6237  jewski-0270291b7
+00002340: 2f29 2c20 5265 7365 6172 6368 2041 7373  /), Research Ass
+00002350: 6f63 6961 7465 2061 7420 556e 6976 6572  ociate at Univer
+00002360: 7369 7479 206f 6620 4174 6865 6e73 2c20  sity of Athens, 
+00002370: 4772 6565 6365 0a2d 205b 4765 6f72 6765  Greece.- [George
+00002380: 2050 6170 6164 616b 6973 5d28 6874 7470   Papadakis](http
+00002390: 733a 2f2f 6770 6170 6164 6973 2e77 6f72  s://gpapadis.wor
+000023a0: 6470 7265 7373 2e63 6f6d 292c 2053 656e  dpress.com), Sen
+000023b0: 696f 7220 5265 7365 6172 6368 6572 2061  ior Researcher a
+000023c0: 7420 556e 6976 6572 7369 7479 206f 6620  t University of 
+000023d0: 4174 6865 6e73 2c20 4772 6565 6365 0a2d  Athens, Greece.-
+000023e0: 205b 456b 6174 6572 696e 6920 496f 616e   [Ekaterini Ioan
+000023f0: 6e6f 755d 2868 7474 7073 3a2f 2f77 7777  nou](https://www
+00002400: 2e74 696c 6275 7267 756e 6976 6572 7369  .tilburguniversi
+00002410: 7479 2e65 6475 2f73 7461 6666 2f65 6b61  ty.edu/staff/eka
+00002420: 7465 7269 6e69 2d69 6f61 6e6e 6f75 292c  terini-ioannou),
+00002430: 2041 7373 6973 7461 6e74 2050 726f 6665   Assistant Profe
+00002440: 7373 6f72 2061 7420 5469 6c62 7572 6720  ssor at Tilburg 
+00002450: 556e 6976 6572 7369 7479 2c20 5468 6520  University, The 
+00002460: 4e65 7468 6572 6c61 6e64 7320 0a2d 205b  Netherlands .- [
+00002470: 4d61 6e6f 6c69 7320 4b6f 7562 6172 616b  Manolis Koubarak
+00002480: 6973 5d28 6874 7470 733a 2f2f 6367 692e  is](https://cgi.
+00002490: 6469 2e75 6f61 2e67 722f 7e6b 6f75 6261  di.uoa.gr/~kouba
+000024a0: 7261 6b2f 292c 2050 726f 6665 7373 6f72  rak/), Professor
+000024b0: 2061 7420 556e 6976 6572 7369 7479 206f   at University o
+000024c0: 6620 4174 6865 6e73 2c20 4772 6565 6365  f Athens, Greece
+000024d0: 0a0a 5468 6973 2069 7320 6120 7265 7365  ..This is a rese
+000024e0: 6172 6368 2070 726f 6a65 6374 2062 7920  arch project by 
+000024f0: 7468 6520 5b41 492d 5465 616d 5d28 6874  the [AI-Team](ht
+00002500: 7470 733a 2f2f 6169 2e64 692e 756f 612e  tps://ai.di.uoa.
+00002510: 6772 2920 6f66 2074 6865 2044 6570 6172  gr) of the Depar
+00002520: 746d 656e 7420 6f66 2049 6e66 6f72 6d61  tment of Informa
+00002530: 7469 6373 2061 6e64 2054 656c 6563 6f6d  tics and Telecom
+00002540: 6d75 6e69 6361 7469 6f6e 7320 6174 2074  munications at t
+00002550: 6865 2055 6e69 7665 7273 6974 7920 6f66  he University of
+00002560: 2041 7468 656e 732e 0a0a 2320 4c69 6365   Athens...# Lice
+00002570: 6e73 650a 0a52 656c 6561 7365 6420 756e  nse..Released un
+00002580: 6465 7220 7468 6520 4170 6163 6865 2d32  der the Apache-2
+00002590: 2e30 206c 6963 656e 7365 2028 7365 6520  .0 license (see 
+000025a0: 5b4c 4943 454e 5345 2e74 7874 5d28 6874  [LICENSE.txt](ht
+000025b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000025c0: 2f41 492d 7465 616d 2d55 6f41 2f70 794a  /AI-team-UoA/pyJ
+000025d0: 6564 4149 2f62 6c6f 622f 6d61 696e 2f4c  edAI/blob/main/L
+000025e0: 4943 454e 5345 2929 2e0a 0a43 6f70 7972  ICENSE))...Copyr
+000025f0: 6967 6874 20c2 a920 3230 3234 2041 492d  ight .. 2024 AI-
+00002600: 5465 616d 2c20 556e 6976 6572 7369 7479  Team, University
+00002610: 206f 6620 4174 6865 6e73 0a0a 3c64 6976   of Athens..<div
+00002620: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00002630: 0a20 2020 203c 6872 3e0a 2020 2020 3c62  .    <hr>.    <b
+00002640: 723e 0a20 2020 203c 6120 6872 6566 3d22  r>.    <a href="
+00002650: 6874 7470 733a 2f2f 7374 656c 6172 2d70  https://stelar-p
+00002660: 726f 6a65 6374 2e65 7522 3e0a 2020 2020  roject.eu">.    
+00002670: 2020 2020 3c69 6d67 2061 6c69 676e 3d22      <img align="
+00002680: 6365 6e74 6572 2220 7372 633d 2268 7474  center" src="htt
+00002690: 7073 3a2f 2f73 7465 6c61 722d 7072 6f6a  ps://stelar-proj
+000026a0: 6563 742e 6575 2f77 702d 636f 6e74 656e  ect.eu/wp-conten
+000026b0: 742f 7570 6c6f 6164 732f 3230 3232 2f30  t/uploads/2022/0
+000026c0: 382f 4c6f 676f 2d53 7465 6c61 722d 312d  8/Logo-Stelar-1-
+000026d0: 662e 706e 6722 2077 6964 7468 3d31 3830  f.png" width=180
+000026e0: 2f3e 0a20 2020 203c 2f61 3e20 266e 6273  />.    </a> &nbs
+000026f0: 703b 266e 6273 703b 266e 6273 703b 266e  p;&nbsp;&nbsp;&n
+00002700: 6273 703b 266e 6273 703b 266e 6273 703b  bsp;&nbsp;&nbsp;
+00002710: 266e 6273 703b 0a20 2020 203c 6120 6872  &nbsp;.    <a hr
+00002720: 6566 3d22 6874 7470 733a 2f2f 6563 2e65  ef="https://ec.e
+00002730: 7572 6f70 612e 6575 2f69 6e66 6f2f 696e  uropa.eu/info/in
+00002740: 6465 785f 656e 223e 0a20 2020 2020 2020  dex_en">.       
+00002750: 203c 696d 6720 616c 6967 6e3d 2263 656e   <img align="cen
+00002760: 7465 7222 2073 7263 3d22 6874 7470 733a  ter" src="https:
+00002770: 2f2f 7570 6c6f 6164 2e77 696b 696d 6564  //upload.wikimed
+00002780: 6961 2e6f 7267 2f77 696b 6970 6564 6961  ia.org/wikipedia
+00002790: 2f63 6f6d 6d6f 6e73 2f74 6875 6d62 2f62  /commons/thumb/b
+000027a0: 2f62 372f 466c 6167 5f6f 665f 4575 726f  /b7/Flag_of_Euro
+000027b0: 7065 2e73 7667 2f31 3230 3070 782d 466c  pe.svg/1200px-Fl
+000027c0: 6167 5f6f 665f 4575 726f 7065 2e73 7667  ag_of_Europe.svg
+000027d0: 2e70 6e67 2220 7769 6474 683d 3134 302f  .png" width=140/
+000027e0: 3e0a 2020 2020 3c2f 613e 0a20 2020 203c  >.    </a>.    <
+000027f0: 6272 3e0a 2020 2020 3c62 723e 0a20 2020  br>.    <br>.   
+00002800: 2020 2020 203c 623e 5468 6973 2070 726f       <b>This pro
+00002810: 6a65 6374 2069 7320 6265 696e 6720 6675  ject is being fu
+00002820: 6e64 6564 2069 6e20 7468 6520 636f 6e74  nded in the cont
+00002830: 6578 7420 6f66 203c 6120 6872 6566 3d22  ext of <a href="
+00002840: 6874 7470 733a 2f2f 7374 656c 6172 2d70  https://stelar-p
+00002850: 726f 6a65 6374 2e65 7522 3e53 5445 4c41  roject.eu">STELA
+00002860: 523c 2f61 3e20 7468 6174 2069 7320 616e  R</a> that is an
+00002870: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00002880: 2f2f 7265 7365 6172 6368 2d61 6e64 2d69  //research-and-i
+00002890: 6e6e 6f76 6174 696f 6e2e 6563 2e65 7572  nnovation.ec.eur
+000028a0: 6f70 612e 6575 2f66 756e 6469 6e67 2f66  opa.eu/funding/f
+000028b0: 756e 6469 6e67 2d6f 7070 6f72 7475 6e69  unding-opportuni
+000028c0: 7469 6573 2f66 756e 6469 6e67 2d70 726f  ties/funding-pro
+000028d0: 6772 616d 6d65 732d 616e 642d 6f70 656e  grammes-and-open
+000028e0: 2d63 616c 6c73 2f68 6f72 697a 6f6e 2d65  -calls/horizon-e
+000028f0: 7572 6f70 655f 656e 223e 484f 5249 5a4f  urope_en">HORIZO
+00002900: 4e2d 4575 726f 7065 3c2f 613e 2070 726f  N-Europe</a> pro
+00002910: 6a65 6374 2e0a 2020 2020 2020 2020 3c2f  ject..        </
+00002920: 623e 0a20 2020 203c 6272 3e0a 3c2f 6469  b>.    <br>.</di
+00002930: 763e 0a                                  v>.
```

### Comparing `pyjedai-0.1.6/src/pyjedai.egg-info/SOURCES.txt` & `pyjedai-0.1.7/src/pyjedai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjedai-0.1.6/tests/test_block_building.py` & `pyjedai-0.1.7/tests/test_block_building.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.1.6/tests/test_block_cleaning.py` & `pyjedai-0.1.7/tests/test_block_cleaning.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.1.6/tests/test_clustering.py` & `pyjedai-0.1.7/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.1.6/tests/test_comparison_cleaning.py` & `pyjedai-0.1.7/tests/test_comparison_cleaning.py`

 * *Files identical despite different names*

