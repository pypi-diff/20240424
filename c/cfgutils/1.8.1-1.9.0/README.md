# Comparing `tmp/cfgutils-1.8.1.tar.gz` & `tmp/cfgutils-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfgutils-1.8.1.tar", last modified: Thu Feb  8 00:17:38 2024, max compression
+gzip compressed data, was "cfgutils-1.9.0.tar", last modified: Wed Mar 13 21:47:57 2024, max compression
```

## Comparing `cfgutils-1.8.1.tar` & `cfgutils-1.9.0.tar`

### file list

```diff
@@ -1,41 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 00:17:38.645846 cfgutils-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-02-08 00:17:30.000000 cfgutils-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-02-08 00:17:38.645846 cfgutils-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-02-08 00:17:30.000000 cfgutils-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 00:17:38.641845 cfgutils-1.8.1/cfgutils/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-08 00:17:30.000000 cfgutils-1.8.1/cfgutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 00:17:38.641845 cfgutils-1.8.1/cfgutils/angr_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-08 00:17:30.000000 cfgutils-1.8.1/cfgutils/angr_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-02-08 00:17:30.000000 cfgutils-1.8.1/cfgutils/angr_utils/ail_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-02-08 00:17:30.000000 cfgutils-1.8.1/cfgutils/angr_utils/prettyify_ail.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 00:17:38.641845 cfgutils-1.8.1/cfgutils/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-02-08 00:17:30.000000 cfgutils-1.8.1/cfgutils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-02-08 00:17:30.000000 cfgutils-1.8.1/cfgutils/data/generic_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    17506 2024-02-08 00:17:30.000000 cfgutils-1.8.1/cfgutils/dominator.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-02-08 00:17:30.000000 cfgutils-1.8.1/cfgutils/file_formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 00:17:38.641845 cfgutils-1.8.1/cfgutils/matrix/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 00:17:30.000000 cfgutils-1.8.1/cfgutils/matrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23556 2024-02-08 00:17:30.000000 cfgutils-1.8.1/cfgutils/matrix/munkres.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-02-08 00:17:30.000000 cfgutils-1.8.1/cfgutils/os_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 00:17:38.641845 cfgutils-1.8.1/cfgutils/regions/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-08 00:17:30.000000 cfgutils-1.8.1/cfgutils/regions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-02-08 00:17:30.000000 cfgutils-1.8.1/cfgutils/regions/graph_region.py
--rw-r--r--   0 runner    (1001) docker     (127)    35694 2024-02-08 00:17:30.000000 cfgutils-1.8.1/cfgutils/regions/region_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-02-08 00:17:30.000000 cfgutils-1.8.1/cfgutils/regions/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 00:17:38.641845 cfgutils-1.8.1/cfgutils/similarity/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-08 00:17:30.000000 cfgutils-1.8.1/cfgutils/similarity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 00:17:38.645846 cfgutils-1.8.1/cfgutils/similarity/ged/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-08 00:17:30.000000 cfgutils-1.8.1/cfgutils/similarity/ged/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-02-08 00:17:30.000000 cfgutils-1.8.1/cfgutils/similarity/ged/abu_aisheh_ged.py
--rw-r--r--   0 runner    (1001) docker     (127)    26655 2024-02-08 00:17:30.000000 cfgutils-1.8.1/cfgutils/similarity/ged/basque_cfged.py
--rw-r--r--   0 runner    (1001) docker     (127)    13268 2024-02-08 00:17:30.000000 cfgutils-1.8.1/cfgutils/similarity/ged/hu_cfged.py
--rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-02-08 00:17:30.000000 cfgutils-1.8.1/cfgutils/sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-02-08 00:17:30.000000 cfgutils-1.8.1/cfgutils/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 00:17:38.645846 cfgutils-1.8.1/cfgutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-02-08 00:17:38.000000 cfgutils-1.8.1/cfgutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-02-08 00:17:38.000000 cfgutils-1.8.1/cfgutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 00:17:38.000000 cfgutils-1.8.1/cfgutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-08 00:17:38.000000 cfgutils-1.8.1/cfgutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-08 00:17:38.000000 cfgutils-1.8.1/cfgutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-02-08 00:17:38.645846 cfgutils-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 00:17:30.000000 cfgutils-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 21:47:57.803854 cfgutils-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-03-13 21:47:45.000000 cfgutils-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-03-13 21:47:57.803854 cfgutils-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-03-13 21:47:45.000000 cfgutils-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 21:47:57.795854 cfgutils-1.9.0/cfgutils/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 21:47:57.799854 cfgutils-1.9.0/cfgutils/angr_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/angr_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6038 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/angr_utils/ail_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/angr_utils/block_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/angr_utils/feat_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/angr_utils/prettyify_ail.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 21:47:57.799854 cfgutils-1.9.0/cfgutils/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/data/generic_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17506 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/dominator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/file_formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 21:47:57.799854 cfgutils-1.9.0/cfgutils/matrix/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/matrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23556 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/matrix/munkres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/os_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 21:47:57.799854 cfgutils-1.9.0/cfgutils/regions/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/regions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/regions/graph_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35694 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/regions/region_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/regions/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 21:47:57.799854 cfgutils-1.9.0/cfgutils/similarity/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/similarity/block_matcher_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 21:47:57.803854 cfgutils-1.9.0/cfgutils/similarity/ged/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/similarity/ged/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/similarity/ged/abu_aisheh_ged.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26655 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/similarity/ged/basque_cfged.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13268 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/similarity/ged/hu_cfged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-03-13 21:47:45.000000 cfgutils-1.9.0/cfgutils/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 21:47:57.803854 cfgutils-1.9.0/cfgutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-03-13 21:47:57.000000 cfgutils-1.9.0/cfgutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-13 21:47:57.000000 cfgutils-1.9.0/cfgutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 21:47:57.000000 cfgutils-1.9.0/cfgutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-13 21:47:57.000000 cfgutils-1.9.0/cfgutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-13 21:47:57.000000 cfgutils-1.9.0/cfgutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-13 21:47:57.803854 cfgutils-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 21:47:45.000000 cfgutils-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 21:47:57.803854 cfgutils-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-03-13 21:47:45.000000 cfgutils-1.9.0/tests/test_angr_cfg_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-03-13 21:47:45.000000 cfgutils-1.9.0/tests/test_ged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-03-13 21:47:45.000000 cfgutils-1.9.0/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-03-13 21:47:45.000000 cfgutils-1.9.0/tests/test_region_identifier.py
```

### Comparing `cfgutils-1.8.1/LICENSE` & `cfgutils-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cfgutils-1.8.1/PKG-INFO` & `cfgutils-1.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: cfgutils
-Version: 1.8.1
+Version: 1.9.0
 Summary: A CFG utility library
 Home-page: https://github.com/mahaloz/cfgutils
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: networkx
 Requires-Dist: graphviz
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pygraphviz
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: sailreval; extra == "tests"
 
 # CFGUtils 
 A Utility library for working with Control Flow Graphs (CFGs) in Python. This library implements previous academic 
 and industrial research in the field of CFGs. It is also the home of the CFGED algorithm, refered to as Basque-CFGED, created in the USENIX Security
 2024 Paper ["Ahoy SAILR! There is No Need to DREAM of C: A Compiler-Aware Structuring Algorithm for Binary Decompilation"](https://www.zionbasque.com/files/publications/sailr_usenix24.pdf).
 
 If you use this library in your research, please cite the SAILR paper. 
@@ -29,15 +32,15 @@
 pip3 install cfgutils
 ```
 
 ## Usage
 CFGUtils is used on Networkx DiGraphs. Most analysis assumes the graph is composed of [GenericBlock](cfgutils/data/generic_block.py) nodes. 
 The nodes a very simple and can be subclassed to represent different kinds of blocks.
 
-All algorithms in this library have a testcase, which can be found in the [tests.py](tests.py) file.
+All algorithms in this library have a testcase, which can be found in the [tests.py](tests/test_ged.py) file.
 
 ### Region Identification
 Regions here are defined as [Single-Entry Single-Exit (SESE)](https://iss.oden.utexas.edu/Publications/Papers/PLDI1994.pdf) subgraphs of the CFG.
 These regions are mostly used in the context of control flow recovery and decompilation. 
 
 ```python
 from cfgutils.data.generic_block import GenericBlock
```

### Comparing `cfgutils-1.8.1/README.md` & `cfgutils-1.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 pip3 install cfgutils
 ```
 
 ## Usage
 CFGUtils is used on Networkx DiGraphs. Most analysis assumes the graph is composed of [GenericBlock](cfgutils/data/generic_block.py) nodes. 
 The nodes a very simple and can be subclassed to represent different kinds of blocks.
 
-All algorithms in this library have a testcase, which can be found in the [tests.py](tests.py) file.
+All algorithms in this library have a testcase, which can be found in the [tests.py](tests/test_ged.py) file.
 
 ### Region Identification
 Regions here are defined as [Single-Entry Single-Exit (SESE)](https://iss.oden.utexas.edu/Publications/Papers/PLDI1994.pdf) subgraphs of the CFG.
 These regions are mostly used in the context of control flow recovery and decompilation. 
 
 ```python
 from cfgutils.data.generic_block import GenericBlock
```

### Comparing `cfgutils-1.8.1/cfgutils/angr_utils/prettyify_ail.py` & `cfgutils-1.9.0/cfgutils/angr_utils/prettyify_ail.py`

 * *Files identical despite different names*

### Comparing `cfgutils-1.8.1/cfgutils/data/__init__.py` & `cfgutils-1.9.0/cfgutils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `cfgutils-1.8.1/cfgutils/data/generic_block.py` & `cfgutils-1.9.0/cfgutils/data/generic_block.py`

 * *Files identical despite different names*

### Comparing `cfgutils-1.8.1/cfgutils/dominator.py` & `cfgutils-1.9.0/cfgutils/dominator.py`

 * *Files identical despite different names*

### Comparing `cfgutils-1.8.1/cfgutils/matrix/munkres.py` & `cfgutils-1.9.0/cfgutils/matrix/munkres.py`

 * *Files identical despite different names*

### Comparing `cfgutils-1.8.1/cfgutils/os_utils.py` & `cfgutils-1.9.0/cfgutils/os_utils.py`

 * *Files identical despite different names*

### Comparing `cfgutils-1.8.1/cfgutils/regions/graph_region.py` & `cfgutils-1.9.0/cfgutils/regions/graph_region.py`

 * *Files identical despite different names*

### Comparing `cfgutils-1.8.1/cfgutils/regions/region_identifier.py` & `cfgutils-1.9.0/cfgutils/regions/region_identifier.py`

 * *Files identical despite different names*

### Comparing `cfgutils-1.8.1/cfgutils/regions/utils.py` & `cfgutils-1.9.0/cfgutils/regions/utils.py`

 * *Files identical despite different names*

### Comparing `cfgutils-1.8.1/cfgutils/similarity/ged/__init__.py` & `cfgutils-1.9.0/cfgutils/similarity/ged/__init__.py`

 * *Files identical despite different names*

### Comparing `cfgutils-1.8.1/cfgutils/similarity/ged/abu_aisheh_ged.py` & `cfgutils-1.9.0/cfgutils/similarity/ged/abu_aisheh_ged.py`

 * *Files identical despite different names*

### Comparing `cfgutils-1.8.1/cfgutils/similarity/ged/basque_cfged.py` & `cfgutils-1.9.0/cfgutils/similarity/ged/basque_cfged.py`

 * *Files identical despite different names*

### Comparing `cfgutils-1.8.1/cfgutils/similarity/ged/hu_cfged.py` & `cfgutils-1.9.0/cfgutils/similarity/ged/hu_cfged.py`

 * *Files identical despite different names*

### Comparing `cfgutils-1.8.1/cfgutils/sorting.py` & `cfgutils-1.9.0/cfgutils/sorting.py`

 * *Files identical despite different names*

### Comparing `cfgutils-1.8.1/cfgutils/transformations.py` & `cfgutils-1.9.0/cfgutils/transformations.py`

 * *Files identical despite different names*

### Comparing `cfgutils-1.8.1/cfgutils.egg-info/PKG-INFO` & `cfgutils-1.9.0/cfgutils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: cfgutils
-Version: 1.8.1
+Version: 1.9.0
 Summary: A CFG utility library
 Home-page: https://github.com/mahaloz/cfgutils
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: networkx
 Requires-Dist: graphviz
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pygraphviz
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: sailreval; extra == "tests"
 
 # CFGUtils 
 A Utility library for working with Control Flow Graphs (CFGs) in Python. This library implements previous academic 
 and industrial research in the field of CFGs. It is also the home of the CFGED algorithm, refered to as Basque-CFGED, created in the USENIX Security
 2024 Paper ["Ahoy SAILR! There is No Need to DREAM of C: A Compiler-Aware Structuring Algorithm for Binary Decompilation"](https://www.zionbasque.com/files/publications/sailr_usenix24.pdf).
 
 If you use this library in your research, please cite the SAILR paper. 
@@ -29,15 +32,15 @@
 pip3 install cfgutils
 ```
 
 ## Usage
 CFGUtils is used on Networkx DiGraphs. Most analysis assumes the graph is composed of [GenericBlock](cfgutils/data/generic_block.py) nodes. 
 The nodes a very simple and can be subclassed to represent different kinds of blocks.
 
-All algorithms in this library have a testcase, which can be found in the [tests.py](tests.py) file.
+All algorithms in this library have a testcase, which can be found in the [tests.py](tests/test_ged.py) file.
 
 ### Region Identification
 Regions here are defined as [Single-Entry Single-Exit (SESE)](https://iss.oden.utexas.edu/Publications/Papers/PLDI1994.pdf) subgraphs of the CFG.
 These regions are mostly used in the context of control flow recovery and decompilation. 
 
 ```python
 from cfgutils.data.generic_block import GenericBlock
```

### Comparing `cfgutils-1.8.1/cfgutils.egg-info/SOURCES.txt` & `cfgutils-1.9.0/cfgutils.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -11,21 +11,28 @@
 cfgutils.egg-info/PKG-INFO
 cfgutils.egg-info/SOURCES.txt
 cfgutils.egg-info/dependency_links.txt
 cfgutils.egg-info/requires.txt
 cfgutils.egg-info/top_level.txt
 cfgutils/angr_utils/__init__.py
 cfgutils/angr_utils/ail_converter.py
+cfgutils/angr_utils/block_matcher.py
+cfgutils/angr_utils/feat_extractor.py
 cfgutils/angr_utils/prettyify_ail.py
 cfgutils/data/__init__.py
 cfgutils/data/generic_block.py
 cfgutils/matrix/__init__.py
 cfgutils/matrix/munkres.py
 cfgutils/regions/__init__.py
 cfgutils/regions/graph_region.py
 cfgutils/regions/region_identifier.py
 cfgutils/regions/utils.py
 cfgutils/similarity/__init__.py
+cfgutils/similarity/block_matcher_base.py
 cfgutils/similarity/ged/__init__.py
 cfgutils/similarity/ged/abu_aisheh_ged.py
 cfgutils/similarity/ged/basque_cfged.py
-cfgutils/similarity/ged/hu_cfged.py
+cfgutils/similarity/ged/hu_cfged.py
+tests/test_angr_cfg_tools.py
+tests/test_ged.py
+tests/test_math.py
+tests/test_region_identifier.py
```

### Comparing `cfgutils-1.8.1/setup.cfg` & `cfgutils-1.9.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -18,11 +18,16 @@
 	graphviz
 	numpy
 	scipy
 	pygraphviz
 python_requires = >= 3.8
 packages = find:
 
+[options.extras_require]
+tests = 
+	pytest
+	sailreval
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

