# Comparing `tmp/manteia_qa_pylinac-1.2.0.tar.gz` & `tmp/manteia_qa_pylinac-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manteia_qa_pylinac-1.2.0.tar", last modified: Thu Apr 18 07:39:27 2024, max compression
+gzip compressed data, was "manteia_qa_pylinac-1.2.1.tar", last modified: Wed Apr 24 07:53:22 2024, max compression
```

## Comparing `manteia_qa_pylinac-1.2.0.tar` & `manteia_qa_pylinac-1.2.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 07:39:27.377226 manteia_qa_pylinac-1.2.0/
--rw-rw-rw-   0        0        0     1060 2024-01-04 20:28:42.000000 manteia_qa_pylinac-1.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0    25897 2024-04-18 07:39:27.376229 manteia_qa_pylinac-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    24650 2024-01-04 20:28:42.000000 manteia_qa_pylinac-1.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-18 07:39:27.374234 manteia_qa_pylinac-1.2.0/manteia_qa_pylinac.egg-info/
--rw-rw-rw-   0        0        0    25897 2024-04-18 07:39:26.000000 manteia_qa_pylinac-1.2.0/manteia_qa_pylinac.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1345 2024-04-18 07:39:26.000000 manteia_qa_pylinac-1.2.0/manteia_qa_pylinac.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 07:39:26.000000 manteia_qa_pylinac-1.2.0/manteia_qa_pylinac.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 07:39:26.000000 manteia_qa_pylinac-1.2.0/manteia_qa_pylinac.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-18 07:39:27.333343 manteia_qa_pylinac-1.2.0/pylinac/
--rw-rw-rw-   0        0        0     1458 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/__init__.py
--rw-rw-rw-   0        0        0    49437 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/acr.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:39:27.338329 manteia_qa_pylinac-1.2.0/pylinac/calibration/
--rw-rw-rw-   0        0        0        0 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/calibration/__init__.py
--rw-rw-rw-   0        0        0    46451 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/calibration/tg51.py
--rw-rw-rw-   0        0        0    31948 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/calibration/trs398.py
--rw-rw-rw-   0        0        0    21333 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/cheese.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:39:27.361269 manteia_qa_pylinac-1.2.0/pylinac/core/
--rw-rw-rw-   0        0        0        0 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/core/__init__.py
--rw-rw-rw-   0        0        0    11596 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/core/array_utils.py
--rw-rw-rw-   0        0        0     6335 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/core/contrast.py
--rw-rw-rw-   0        0        0     1912 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/core/decorators.py
--rw-rw-rw-   0        0        0       40 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/core/exceptions.py
--rw-rw-rw-   0        0        0    18332 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/core/geometry.py
--rw-rw-rw-   0        0        0     2514 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/core/hill.py
--rw-rw-rw-   0        0        0    73436 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/core/image.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:39:27.366255 manteia_qa_pylinac-1.2.0/pylinac/core/image_generator/
--rw-rw-rw-   0        0        0      492 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/core/image_generator/__init__.py
--rw-rw-rw-   0        0        0    12133 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/core/image_generator/layers.py
--rw-rw-rw-   0        0        0    11121 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/core/image_generator/simulators.py
--rw-rw-rw-   0        0        0    23115 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/core/image_generator/utils.py
--rw-rw-rw-   0        0        0    10344 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/core/io.py
--rw-rw-rw-   0        0        0      419 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/core/mask.py
--rw-rw-rw-   0        0        0      285 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/core/metrics.py
--rw-rw-rw-   0        0        0     8825 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/core/mtf.py
--rw-rw-rw-   0        0        0     4425 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/core/pdf.py
--rw-rw-rw-   0        0        0    96866 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/core/profile.py
--rw-rw-rw-   0        0        0    14267 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/core/roi.py
--rw-rw-rw-   0        0        0     2980 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/core/scale.py
--rw-rw-rw-   0        0        0      166 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/core/typing.py
--rw-rw-rw-   0        0        0     6054 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/core/utilities.py
--rw-rw-rw-   0        0        0      664 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/core/validators.py
--rw-rw-rw-   0        0        0    96750 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/ct.py
--rw-rw-rw-   0        0        0     5093 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/dlg.py
--rw-rw-rw-   0        0        0    63156 2024-04-18 07:38:47.000000 manteia_qa_pylinac-1.2.0/pylinac/field_analysis.py
--rw-rw-rw-   0        0        0   108765 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/log_analyzer.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:39:27.373237 manteia_qa_pylinac-1.2.0/pylinac/metrics/
--rw-rw-rw-   0        0        0        0 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/metrics/__init__.py
--rw-rw-rw-   0        0        0     4939 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/metrics/features.py
--rw-rw-rw-   0        0        0    27943 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/metrics/image.py
--rw-rw-rw-   0        0        0    19376 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/metrics/profile.py
--rw-rw-rw-   0        0        0     2285 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/metrics/utils.py
--rw-rw-rw-   0        0        0    61146 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/nuclear.py
--rw-rw-rw-   0        0        0    63654 2024-04-18 07:37:51.000000 manteia_qa_pylinac-1.2.0/pylinac/picketfence.py
--rw-rw-rw-   0        0        0   105868 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/planar_imaging.py
--rw-rw-rw-   0        0        0    22613 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/quart.py
--rw-rw-rw-   0        0        0      624 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/settings.py
--rw-rw-rw-   0        0        0    27535 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/starshot.py
--rw-rw-rw-   0        0        0       23 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/version.py
--rw-rw-rw-   0        0        0    22457 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/vmat.py
--rw-rw-rw-   0        0        0    89252 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.0/pylinac/winston_lutz.py
--rw-rw-rw-   0        0        0       42 2024-04-18 07:39:27.377226 manteia_qa_pylinac-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      916 2024-04-18 07:36:47.000000 manteia_qa_pylinac-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 07:53:22.568267 manteia_qa_pylinac-1.2.1/
+-rw-rw-rw-   0        0        0     1060 2024-01-04 20:28:42.000000 manteia_qa_pylinac-1.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0    25897 2024-04-24 07:53:22.567269 manteia_qa_pylinac-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    24650 2024-01-04 20:28:42.000000 manteia_qa_pylinac-1.2.1/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-24 07:53:22.565276 manteia_qa_pylinac-1.2.1/manteia_qa_pylinac.egg-info/
+-rw-rw-rw-   0        0        0    25897 2024-04-24 07:53:21.000000 manteia_qa_pylinac-1.2.1/manteia_qa_pylinac.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1345 2024-04-24 07:53:21.000000 manteia_qa_pylinac-1.2.1/manteia_qa_pylinac.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 07:53:21.000000 manteia_qa_pylinac-1.2.1/manteia_qa_pylinac.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-24 07:53:21.000000 manteia_qa_pylinac-1.2.1/manteia_qa_pylinac.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 07:53:22.524384 manteia_qa_pylinac-1.2.1/pylinac/
+-rw-rw-rw-   0        0        0     1458 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/__init__.py
+-rw-rw-rw-   0        0        0    49437 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/acr.py
+drwxrwxrwx   0        0        0        0 2024-04-24 07:53:22.529371 manteia_qa_pylinac-1.2.1/pylinac/calibration/
+-rw-rw-rw-   0        0        0        0 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/calibration/__init__.py
+-rw-rw-rw-   0        0        0    46451 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/calibration/tg51.py
+-rw-rw-rw-   0        0        0    31948 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/calibration/trs398.py
+-rw-rw-rw-   0        0        0    21333 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/cheese.py
+drwxrwxrwx   0        0        0        0 2024-04-24 07:53:22.551312 manteia_qa_pylinac-1.2.1/pylinac/core/
+-rw-rw-rw-   0        0        0        0 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/core/__init__.py
+-rw-rw-rw-   0        0        0    11596 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/core/array_utils.py
+-rw-rw-rw-   0        0        0     6335 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/core/contrast.py
+-rw-rw-rw-   0        0        0     1912 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/core/decorators.py
+-rw-rw-rw-   0        0        0       40 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/core/exceptions.py
+-rw-rw-rw-   0        0        0    18332 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/core/geometry.py
+-rw-rw-rw-   0        0        0     2514 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/core/hill.py
+-rw-rw-rw-   0        0        0    73436 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/core/image.py
+drwxrwxrwx   0        0        0        0 2024-04-24 07:53:22.556300 manteia_qa_pylinac-1.2.1/pylinac/core/image_generator/
+-rw-rw-rw-   0        0        0      492 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/core/image_generator/__init__.py
+-rw-rw-rw-   0        0        0    12133 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/core/image_generator/layers.py
+-rw-rw-rw-   0        0        0    11121 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/core/image_generator/simulators.py
+-rw-rw-rw-   0        0        0    23115 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/core/image_generator/utils.py
+-rw-rw-rw-   0        0        0    10344 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/core/io.py
+-rw-rw-rw-   0        0        0      419 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/core/mask.py
+-rw-rw-rw-   0        0        0      285 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/core/metrics.py
+-rw-rw-rw-   0        0        0     8825 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/core/mtf.py
+-rw-rw-rw-   0        0        0     4425 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/core/pdf.py
+-rw-rw-rw-   0        0        0    96866 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/core/profile.py
+-rw-rw-rw-   0        0        0    14267 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/core/roi.py
+-rw-rw-rw-   0        0        0     2980 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/core/scale.py
+-rw-rw-rw-   0        0        0      166 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/core/typing.py
+-rw-rw-rw-   0        0        0     6054 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/core/utilities.py
+-rw-rw-rw-   0        0        0      664 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/core/validators.py
+-rw-rw-rw-   0        0        0    96777 2024-04-24 07:52:07.000000 manteia_qa_pylinac-1.2.1/pylinac/ct.py
+-rw-rw-rw-   0        0        0     5093 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/dlg.py
+-rw-rw-rw-   0        0        0    63156 2024-04-18 07:38:47.000000 manteia_qa_pylinac-1.2.1/pylinac/field_analysis.py
+-rw-rw-rw-   0        0        0   108765 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/log_analyzer.py
+drwxrwxrwx   0        0        0        0 2024-04-24 07:53:22.564279 manteia_qa_pylinac-1.2.1/pylinac/metrics/
+-rw-rw-rw-   0        0        0        0 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/metrics/__init__.py
+-rw-rw-rw-   0        0        0     4939 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/metrics/features.py
+-rw-rw-rw-   0        0        0    27943 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/metrics/image.py
+-rw-rw-rw-   0        0        0    19376 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/metrics/profile.py
+-rw-rw-rw-   0        0        0     2285 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/metrics/utils.py
+-rw-rw-rw-   0        0        0    61146 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/nuclear.py
+-rw-rw-rw-   0        0        0    63654 2024-04-18 07:37:51.000000 manteia_qa_pylinac-1.2.1/pylinac/picketfence.py
+-rw-rw-rw-   0        0        0   105868 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/planar_imaging.py
+-rw-rw-rw-   0        0        0    22613 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/quart.py
+-rw-rw-rw-   0        0        0      624 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/settings.py
+-rw-rw-rw-   0        0        0    27535 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/starshot.py
+-rw-rw-rw-   0        0        0       23 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/version.py
+-rw-rw-rw-   0        0        0    22457 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/vmat.py
+-rw-rw-rw-   0        0        0    89252 2024-02-13 17:57:53.000000 manteia_qa_pylinac-1.2.1/pylinac/winston_lutz.py
+-rw-rw-rw-   0        0        0       42 2024-04-24 07:53:22.568267 manteia_qa_pylinac-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      916 2024-04-24 07:53:03.000000 manteia_qa_pylinac-1.2.1/setup.py
```

### Comparing `manteia_qa_pylinac-1.2.0/LICENSE.txt` & `manteia_qa_pylinac-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/PKG-INFO` & `manteia_qa_pylinac-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manteia_qa_pylinac
-Version: 1.2.0
+Version: 1.2.1
 Summary: pylinac custom made by manteia
 Home-page: 
 Author: dengjianping
 Author-email: 1601246283@qq.com
 License: BSD License
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `manteia_qa_pylinac-1.2.0/README.rst` & `manteia_qa_pylinac-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/manteia_qa_pylinac.egg-info/PKG-INFO` & `manteia_qa_pylinac-1.2.1/manteia_qa_pylinac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manteia_qa_pylinac
-Version: 1.2.0
+Version: 1.2.1
 Summary: pylinac custom made by manteia
 Home-page: 
 Author: dengjianping
 Author-email: 1601246283@qq.com
 License: BSD License
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `manteia_qa_pylinac-1.2.0/manteia_qa_pylinac.egg-info/SOURCES.txt` & `manteia_qa_pylinac-1.2.1/manteia_qa_pylinac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/__init__.py` & `manteia_qa_pylinac-1.2.1/pylinac/__init__.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/acr.py` & `manteia_qa_pylinac-1.2.1/pylinac/acr.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/calibration/tg51.py` & `manteia_qa_pylinac-1.2.1/pylinac/calibration/tg51.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/calibration/trs398.py` & `manteia_qa_pylinac-1.2.1/pylinac/calibration/trs398.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/cheese.py` & `manteia_qa_pylinac-1.2.1/pylinac/cheese.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/core/array_utils.py` & `manteia_qa_pylinac-1.2.1/pylinac/core/array_utils.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/core/contrast.py` & `manteia_qa_pylinac-1.2.1/pylinac/core/contrast.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/core/decorators.py` & `manteia_qa_pylinac-1.2.1/pylinac/core/decorators.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/core/geometry.py` & `manteia_qa_pylinac-1.2.1/pylinac/core/geometry.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/core/hill.py` & `manteia_qa_pylinac-1.2.1/pylinac/core/hill.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/core/image.py` & `manteia_qa_pylinac-1.2.1/pylinac/core/image.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/core/image_generator/layers.py` & `manteia_qa_pylinac-1.2.1/pylinac/core/image_generator/layers.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/core/image_generator/simulators.py` & `manteia_qa_pylinac-1.2.1/pylinac/core/image_generator/simulators.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/core/image_generator/utils.py` & `manteia_qa_pylinac-1.2.1/pylinac/core/image_generator/utils.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/core/io.py` & `manteia_qa_pylinac-1.2.1/pylinac/core/io.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/core/mtf.py` & `manteia_qa_pylinac-1.2.1/pylinac/core/mtf.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/core/pdf.py` & `manteia_qa_pylinac-1.2.1/pylinac/core/pdf.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/core/profile.py` & `manteia_qa_pylinac-1.2.1/pylinac/core/profile.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/core/roi.py` & `manteia_qa_pylinac-1.2.1/pylinac/core/roi.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/core/scale.py` & `manteia_qa_pylinac-1.2.1/pylinac/core/scale.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/core/utilities.py` & `manteia_qa_pylinac-1.2.1/pylinac/core/utilities.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/core/validators.py` & `manteia_qa_pylinac-1.2.1/pylinac/core/validators.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/ct.py` & `manteia_qa_pylinac-1.2.1/pylinac/ct.py`

 * *Files 0% similar despite different names*

```diff
@@ -2226,14 +2226,15 @@
                 offset=offset,
                 contrast_method=contrast_method,
                 visibility_threshold=visibility_threshold,
                 clear_borders=self.clear_borders,
             )
         if zip_after and not self.was_from_zip:
             self._zip_images()
+        return self.ctp486
 
     def _has_module(self, module_of_interest: type[CatPhanModule]) -> bool:
         return any(
             issubclass(module, module_of_interest) for module in self.modules.keys()
         )
 
     def _get_module(
```

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/dlg.py` & `manteia_qa_pylinac-1.2.1/pylinac/dlg.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/field_analysis.py` & `manteia_qa_pylinac-1.2.1/pylinac/field_analysis.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/log_analyzer.py` & `manteia_qa_pylinac-1.2.1/pylinac/log_analyzer.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/metrics/features.py` & `manteia_qa_pylinac-1.2.1/pylinac/metrics/features.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/metrics/image.py` & `manteia_qa_pylinac-1.2.1/pylinac/metrics/image.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/metrics/profile.py` & `manteia_qa_pylinac-1.2.1/pylinac/metrics/profile.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/metrics/utils.py` & `manteia_qa_pylinac-1.2.1/pylinac/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/nuclear.py` & `manteia_qa_pylinac-1.2.1/pylinac/nuclear.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/picketfence.py` & `manteia_qa_pylinac-1.2.1/pylinac/picketfence.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/planar_imaging.py` & `manteia_qa_pylinac-1.2.1/pylinac/planar_imaging.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/quart.py` & `manteia_qa_pylinac-1.2.1/pylinac/quart.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/settings.py` & `manteia_qa_pylinac-1.2.1/pylinac/settings.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/starshot.py` & `manteia_qa_pylinac-1.2.1/pylinac/starshot.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/vmat.py` & `manteia_qa_pylinac-1.2.1/pylinac/vmat.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/pylinac/winston_lutz.py` & `manteia_qa_pylinac-1.2.1/pylinac/winston_lutz.py`

 * *Files identical despite different names*

### Comparing `manteia_qa_pylinac-1.2.0/setup.py` & `manteia_qa_pylinac-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open("README.rst", "r") as f:
   long_description = f.read()
 
 setup(name='manteia_qa_pylinac',  # 包名
-      version='1.2.0',  # 版本号
+      version='1.2.1',  # 版本号
       description='pylinac custom made by manteia',
       long_description=long_description,
       author='dengjianping',
       author_email='1601246283@qq.com',
       url='',
       install_requires=[],
       license='BSD License',
```

