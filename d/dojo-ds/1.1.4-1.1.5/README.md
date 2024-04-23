# Comparing `tmp/dojo_ds-1.1.4.tar.gz` & `tmp/dojo_ds-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dojo_ds-1.1.4.tar", last modified: Thu Apr 18 23:51:14 2024, max compression
+gzip compressed data, was "dojo_ds-1.1.5.tar", last modified: Tue Apr 23 23:06:04 2024, max compression
```

## Comparing `dojo_ds-1.1.4.tar` & `dojo_ds-1.1.5.tar`

### file list

```diff
@@ -1,55 +1,50 @@
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 23:51:14.667725 dojo_ds-1.1.4/
--rw-r--r--   0 codingdojo   (502) staff       (20)      195 2024-01-24 00:23:27.000000 dojo_ds-1.1.4/AUTHORS.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)     3530 2023-02-15 01:14:18.000000 dojo_ds-1.1.4/CONTRIBUTING.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       89 2023-02-15 01:14:18.000000 dojo_ds-1.1.4/HISTORY.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)    35129 2023-02-15 01:14:37.000000 dojo_ds-1.1.4/LICENSE
--rw-r--r--   0 codingdojo   (502) staff       (20)      262 2023-02-15 01:14:18.000000 dojo_ds-1.1.4/MANIFEST.in
--rw-r--r--   0 codingdojo   (502) staff       (20)     1706 2024-04-18 23:51:14.667412 dojo_ds-1.1.4/PKG-INFO
--rw-r--r--   0 codingdojo   (502) staff       (20)      607 2023-05-19 01:08:02.000000 dojo_ds-1.1.4/README.rst
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 23:51:14.640011 dojo_ds-1.1.4/docs/
--rw-r--r--   0 codingdojo   (502) staff       (20)      608 2024-01-24 01:18:29.000000 dojo_ds-1.1.4/docs/Makefile
--rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-1.1.4/docs/authors.rst
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 23:51:14.625108 dojo_ds-1.1.4/docs/build/
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 23:51:14.625234 dojo_ds-1.1.4/docs/build/html/
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 23:51:14.641454 dojo_ds-1.1.4/docs/build/html/_static/
--rw-r--r--   0 codingdojo   (502) staff       (20)      286 2024-01-23 23:54:56.000000 dojo_ds-1.1.4/docs/build/html/_static/file.png
--rw-r--r--   0 codingdojo   (502) staff       (20)       90 2024-01-23 23:54:56.000000 dojo_ds-1.1.4/docs/build/html/_static/minus.png
--rw-r--r--   0 codingdojo   (502) staff       (20)       90 2024-01-23 23:54:56.000000 dojo_ds-1.1.4/docs/build/html/_static/plus.png
--rwxr-xr-x   0 codingdojo   (502) staff       (20)     6020 2024-01-24 01:33:23.000000 dojo_ds-1.1.4/docs/conf.py
--rw-r--r--   0 codingdojo   (502) staff       (20)       33 2023-02-15 01:14:18.000000 dojo_ds-1.1.4/docs/contributing.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)     1512 2024-01-24 01:04:56.000000 dojo_ds-1.1.4/docs/dojo_ds.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-1.1.4/docs/history.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)      384 2024-01-24 01:32:59.000000 dojo_ds-1.1.4/docs/index.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)      542 2024-01-24 01:23:15.000000 dojo_ds-1.1.4/docs/installation.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)      805 2023-02-15 01:14:18.000000 dojo_ds-1.1.4/docs/make.bat
--rw-r--r--   0 codingdojo   (502) staff       (20)       58 2024-01-24 01:14:29.000000 dojo_ds-1.1.4/docs/modules.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       58 2024-01-24 00:26:33.000000 dojo_ds-1.1.4/docs/old_modules.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       27 2023-02-15 01:14:18.000000 dojo_ds-1.1.4/docs/readme.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       75 2023-05-17 14:09:11.000000 dojo_ds-1.1.4/docs/usage.rst
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 23:51:14.652716 dojo_ds-1.1.4/dojo_ds/
--rw-r--r--   0 codingdojo   (502) staff       (20)      969 2024-04-18 23:51:08.000000 dojo_ds-1.1.4/dojo_ds/__init__.py
--rw-r--r--   0 codingdojo   (502) staff       (20)     7851 2024-02-23 02:05:37.000000 dojo_ds-1.1.4/dojo_ds/_eda_functions_plotly.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      399 2024-01-23 02:13:03.000000 dojo_ds-1.1.4/dojo_ds/cli.py
--rw-r--r--   0 codingdojo   (502) staff       (20)     4721 2024-02-23 02:07:09.000000 dojo_ds-1.1.4/dojo_ds/data_enrichment.py
--rw-r--r--   0 codingdojo   (502) staff       (20)     2047 2024-02-23 02:12:32.000000 dojo_ds-1.1.4/dojo_ds/deploy.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    12923 2024-02-23 02:03:18.000000 dojo_ds-1.1.4/dojo_ds/eda.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    24080 2024-02-23 02:01:30.000000 dojo_ds-1.1.4/dojo_ds/evaluate.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      245 2024-01-23 02:14:45.000000 dojo_ds-1.1.4/dojo_ds/imports.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    22135 2024-02-23 01:54:13.000000 dojo_ds-1.1.4/dojo_ds/insights.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      293 2024-01-23 02:11:38.000000 dojo_ds-1.1.4/dojo_ds/matplotlib_style.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    13103 2024-02-23 02:09:27.000000 dojo_ds-1.1.4/dojo_ds/nlp.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    20617 2024-04-18 23:50:24.000000 dojo_ds-1.1.4/dojo_ds/time_series.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    19491 2024-02-23 02:13:34.000000 dojo_ds-1.1.4/dojo_ds/utils.py
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 23:51:14.666360 dojo_ds-1.1.4/dojo_ds.egg-info/
--rw-r--r--   0 codingdojo   (502) staff       (20)     1706 2024-04-18 23:51:14.000000 dojo_ds-1.1.4/dojo_ds.egg-info/PKG-INFO
--rw-r--r--   0 codingdojo   (502) staff       (20)      938 2024-04-18 23:51:14.000000 dojo_ds-1.1.4/dojo_ds.egg-info/SOURCES.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)        1 2024-04-18 23:51:14.000000 dojo_ds-1.1.4/dojo_ds.egg-info/dependency_links.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)       45 2024-04-18 23:51:14.000000 dojo_ds-1.1.4/dojo_ds.egg-info/entry_points.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)        1 2023-02-15 01:30:10.000000 dojo_ds-1.1.4/dojo_ds.egg-info/not-zip-safe
--rw-r--r--   0 codingdojo   (502) staff       (20)      121 2024-04-18 23:51:14.000000 dojo_ds-1.1.4/dojo_ds.egg-info/requires.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)        8 2024-04-18 23:51:14.000000 dojo_ds-1.1.4/dojo_ds.egg-info/top_level.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)      379 2024-04-18 23:51:14.668295 dojo_ds-1.1.4/setup.cfg
--rw-r--r--   0 codingdojo   (502) staff       (20)     2602 2024-04-18 23:51:08.000000 dojo_ds-1.1.4/setup.py
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 23:51:14.665479 dojo_ds-1.1.4/tests/
--rw-r--r--   0 codingdojo   (502) staff       (20)       37 2023-02-15 01:14:18.000000 dojo_ds-1.1.4/tests/__init__.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      862 2024-01-23 02:15:25.000000 dojo_ds-1.1.4/tests/test_dojo_ds.py
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-23 23:06:04.941912 dojo_ds-1.1.5/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      195 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/AUTHORS.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)     3530 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/CONTRIBUTING.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       89 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/HISTORY.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)    35129 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/LICENSE
+-rw-r--r--   0 codingdojo   (502) staff       (20)      262 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/MANIFEST.in
+-rw-r--r--   0 codingdojo   (502) staff       (20)     1706 2024-04-23 23:06:04.941839 dojo_ds-1.1.5/PKG-INFO
+-rw-r--r--   0 codingdojo   (502) staff       (20)      607 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/README.rst
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-23 23:06:04.935685 dojo_ds-1.1.5/docs/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      608 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/docs/Makefile
+-rw-r--r--   0 codingdojo   (502) staff       (20)       28 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/docs/authors.rst
+-rwxr-xr-x   0 codingdojo   (502) staff       (20)     6020 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/docs/conf.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)       33 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/docs/contributing.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)     1512 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/docs/dojo_ds.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       28 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/docs/history.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)      384 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/docs/index.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)      542 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/docs/installation.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)      769 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/docs/make.bat
+-rw-r--r--   0 codingdojo   (502) staff       (20)       58 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/docs/modules.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       58 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/docs/old_modules.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       27 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/docs/readme.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       75 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/docs/usage.rst
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-23 23:06:04.940106 dojo_ds-1.1.5/dojo_ds/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      992 2024-04-23 23:05:56.000000 dojo_ds-1.1.5/dojo_ds/__init__.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)     7851 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/dojo_ds/_eda_functions_plotly.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      399 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/dojo_ds/cli.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)     4721 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/dojo_ds/data_enrichment.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    14909 2024-04-23 23:00:20.000000 dojo_ds-1.1.5/dojo_ds/datasets.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)     2047 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/dojo_ds/deploy.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    12923 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/dojo_ds/eda.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    24080 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/dojo_ds/evaluate.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)     8550 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/dojo_ds/imports.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    22135 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/dojo_ds/insights.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      293 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/dojo_ds/matplotlib_style.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    13103 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/dojo_ds/nlp.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    20617 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/dojo_ds/time_series.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    19491 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/dojo_ds/utils.py
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-23 23:06:04.941525 dojo_ds-1.1.5/dojo_ds.egg-info/
+-rw-r--r--   0 codingdojo   (502) staff       (20)     1706 2024-04-23 23:06:04.000000 dojo_ds-1.1.5/dojo_ds.egg-info/PKG-INFO
+-rw-r--r--   0 codingdojo   (502) staff       (20)      858 2024-04-23 23:06:04.000000 dojo_ds-1.1.5/dojo_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)        1 2024-04-23 23:06:04.000000 dojo_ds-1.1.5/dojo_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)       45 2024-04-23 23:06:04.000000 dojo_ds-1.1.5/dojo_ds.egg-info/entry_points.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)        1 2024-04-23 23:06:04.000000 dojo_ds-1.1.5/dojo_ds.egg-info/not-zip-safe
+-rw-r--r--   0 codingdojo   (502) staff       (20)      121 2024-04-23 23:06:04.000000 dojo_ds-1.1.5/dojo_ds.egg-info/requires.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)        8 2024-04-23 23:06:04.000000 dojo_ds-1.1.5/dojo_ds.egg-info/top_level.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)      379 2024-04-23 23:06:04.942266 dojo_ds-1.1.5/setup.cfg
+-rw-r--r--   0 codingdojo   (502) staff       (20)     2602 2024-04-23 23:05:56.000000 dojo_ds-1.1.5/setup.py
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-23 23:06:04.941321 dojo_ds-1.1.5/tests/
+-rw-r--r--   0 codingdojo   (502) staff       (20)       37 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/tests/__init__.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      862 2024-04-23 23:00:04.000000 dojo_ds-1.1.5/tests/test_dojo_ds.py
```

### Comparing `dojo_ds-1.1.4/CONTRIBUTING.rst` & `dojo_ds-1.1.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.4/LICENSE` & `dojo_ds-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.4/PKG-INFO` & `dojo_ds-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo_ds
-Version: 1.1.4
+Version: 1.1.5
 Summary: Code from Coding Dojo's Online Part-Time Data Science boot camp
 Home-page: https://github.com/coding-dojo-data-science/dojo_ds
 Author: James Irving
 Author-email: jirving@codingdojo.com
 License: GNU General Public License v3
 Keywords: dojo_ds
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `dojo_ds-1.1.4/README.rst` & `dojo_ds-1.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.4/docs/Makefile` & `dojo_ds-1.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.4/docs/conf.py` & `dojo_ds-1.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.4/docs/dojo_ds.rst` & `dojo_ds-1.1.5/docs/dojo_ds.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.4/docs/installation.rst` & `dojo_ds-1.1.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.4/dojo_ds/__init__.py` & `dojo_ds-1.1.5/dojo_ds/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 Custom Functions the Data Science Program
 __author__ = James Irving, Brenda Hungerford
 """
 __author__ = """James Irving"""
 __email__ = 'james.irving.phd@gmail.com'
-__version__ = '1.1.4'
+__version__ = '1.1.5'
 from . import data_enrichment as data
 from . import eda 
 from . import evaluate
 from . import insights 
 from . import nlp
 from . import time_series
+from . import datasets
 
 # from . import deployment_functions as deploy
 
 from . import utils as utils
 
 
 # from . import _eda_functions_plotly as eda_plotly
```

### Comparing `dojo_ds-1.1.4/dojo_ds/_eda_functions_plotly.py` & `dojo_ds-1.1.5/dojo_ds/_eda_functions_plotly.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.4/dojo_ds/data_enrichment.py` & `dojo_ds-1.1.5/dojo_ds/data_enrichment.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.4/dojo_ds/deploy.py` & `dojo_ds-1.1.5/dojo_ds/deploy.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.4/dojo_ds/eda.py` & `dojo_ds-1.1.5/dojo_ds/eda.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.4/dojo_ds/evaluate.py` & `dojo_ds-1.1.5/dojo_ds/evaluate.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.4/dojo_ds/insights.py` & `dojo_ds-1.1.5/dojo_ds/insights.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.4/dojo_ds/nlp.py` & `dojo_ds-1.1.5/dojo_ds/nlp.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.4/dojo_ds/time_series.py` & `dojo_ds-1.1.5/dojo_ds/time_series.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.4/dojo_ds/utils.py` & `dojo_ds-1.1.5/dojo_ds/utils.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.4/dojo_ds.egg-info/PKG-INFO` & `dojo_ds-1.1.5/dojo_ds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo_ds
-Version: 1.1.4
+Version: 1.1.5
 Summary: Code from Coding Dojo's Online Part-Time Data Science boot camp
 Home-page: https://github.com/coding-dojo-data-science/dojo_ds
 Author: James Irving
 Author-email: jirving@codingdojo.com
 License: GNU General Public License v3
 Keywords: dojo_ds
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `dojo_ds-1.1.4/dojo_ds.egg-info/SOURCES.txt` & `dojo_ds-1.1.5/dojo_ds.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,21 +15,19 @@
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/modules.rst
 docs/old_modules.rst
 docs/readme.rst
 docs/usage.rst
-docs/build/html/_static/file.png
-docs/build/html/_static/minus.png
-docs/build/html/_static/plus.png
 dojo_ds/__init__.py
 dojo_ds/_eda_functions_plotly.py
 dojo_ds/cli.py
 dojo_ds/data_enrichment.py
+dojo_ds/datasets.py
 dojo_ds/deploy.py
 dojo_ds/eda.py
 dojo_ds/evaluate.py
 dojo_ds/imports.py
 dojo_ds/insights.py
 dojo_ds/matplotlib_style.py
 dojo_ds/nlp.py
```

### Comparing `dojo_ds-1.1.4/setup.py` & `dojo_ds-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,10 +69,10 @@
     include_package_data=True,
     keywords='dojo_ds',
     name='dojo_ds',
     packages=find_packages(include=['dojo_ds', 'dojo_ds.*']),
     test_suite='tests',
     tests_require=load_requirements("./requirements.txt") + test_requirements,
     url='https://github.com/coding-dojo-data-science/dojo_ds',
-    version='1.1.4',
+    version='1.1.5',
     zip_safe=False,
 )
```

### Comparing `dojo_ds-1.1.4/tests/test_dojo_ds.py` & `dojo_ds-1.1.5/tests/test_dojo_ds.py`

 * *Files identical despite different names*

