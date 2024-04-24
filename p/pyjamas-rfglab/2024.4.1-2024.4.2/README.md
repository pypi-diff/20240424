# Comparing `tmp/pyjamas-rfglab-2024.4.1.tar.gz` & `tmp/pyjamas-rfglab-2024.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjamas-rfglab-2024.4.1.tar", last modified: Wed Apr 17 16:35:19 2024, max compression
+gzip compressed data, was "pyjamas-rfglab-2024.4.2.tar", last modified: Wed Apr 24 16:49:57 2024, max compression
```

## Comparing `pyjamas-rfglab-2024.4.1.tar` & `pyjamas-rfglab-2024.4.2.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-17 16:35:19.504043 pyjamas-rfglab-2024.4.1/
--rw-r--r--   0 rodrigo    (501) staff       (20)      265 2023-01-17 21:44:31.000000 pyjamas-rfglab-2024.4.1/MANIFEST.in
--rw-r--r--   0 rodrigo    (501) staff       (20)     1686 2024-04-17 16:35:19.503467 pyjamas-rfglab-2024.4.1/PKG-INFO
--rw-r--r--   0 rodrigo    (501) staff       (20)     1202 2023-07-11 19:12:22.000000 pyjamas-rfglab-2024.4.1/README.md
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-17 16:35:19.442757 pyjamas-rfglab-2024.4.1/pyjamas/
--rw-r--r--   0 rodrigo    (501) staff       (20)    33144 2020-02-04 05:51:32.000000 pyjamas-rfglab-2024.4.1/pyjamas/LICENSE
--rw-r--r--   0 rodrigo    (501) staff       (20)     1088 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.4.1/pyjamas/__init__.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-17 16:35:19.460320 pyjamas-rfglab-2024.4.1/pyjamas/dialogs/
--rw-r--r--   0 rodrigo    (501) staff       (20)     1645 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.1/pyjamas/dialogs/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    17593 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/dialogs/adjustcontrast.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    31465 2024-03-22 23:06:04.000000 pyjamas-rfglab-2024.4.1/pyjamas/dialogs/batchanalysis.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    12069 2024-04-16 14:02:15.000000 pyjamas-rfglab-2024.4.1/pyjamas/dialogs/batchflatfield.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     5509 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/dialogs/batchprojectconcat.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     6823 2024-04-16 14:02:15.000000 pyjamas-rfglab-2024.4.1/pyjamas/dialogs/batchresize.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2980 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/dialogs/classifierdialogABC.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3199 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/dialogs/classifiertype.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     6437 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/dialogs/expandnpropagateseeds.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     5227 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/dialogs/expandseeds.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    13000 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/dialogs/findseeds.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    11361 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/dialogs/logregression.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3453 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/dialogs/matplotlibdialog.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     8858 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/dialogs/measurepoly.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    13277 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/dialogs/neuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     8699 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.4.1/pyjamas/dialogs/nonmax_suppr.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     5533 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/dialogs/propagateseeds.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    14588 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/dialogs/rescuneuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    12510 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/dialogs/svm.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2243 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/dialogs/textdialog.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2817 2023-12-27 20:45:04.000000 pyjamas-rfglab-2024.4.1/pyjamas/dialogs/texteditdialog.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     4082 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/dialogs/timepoints.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1806 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/dragdropmainwindow.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-17 16:35:19.461493 pyjamas-rfglab-2024.4.1/pyjamas/external/
--rw-r--r--   0 rodrigo    (501) staff       (20)      899 2021-05-09 22:07:44.000000 pyjamas-rfglab-2024.4.1/pyjamas/external/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     6852 2020-07-11 20:09:58.000000 pyjamas-rfglab-2024.4.1/pyjamas/external/pascal_voc_io.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     4930 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/orthogonalviewswindow.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    52457 2024-04-17 16:34:42.000000 pyjamas-rfglab-2024.4.1/pyjamas/pjscore.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    33519 2023-11-22 14:41:28.000000 pyjamas-rfglab-2024.4.1/pyjamas/pjseventfilter.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2123 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/pjsthreads.py
--rw-r--r--   0 rodrigo    (501) staff       (20)  2950837 2023-06-21 15:47:44.000000 pyjamas-rfglab-2024.4.1/pyjamas/pyjamas.tif
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-17 16:35:19.464967 pyjamas-rfglab-2024.4.1/pyjamas/rannotations/
--rw-r--r--   0 rodrigo    (501) staff       (20)      924 2022-06-20 21:44:00.000000 pyjamas-rfglab-2024.4.1/pyjamas/rannotations/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)      856 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.4.1/pyjamas/rannotations/rannotation.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    16818 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/rannotations/rpolyline.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2288 2022-08-14 20:59:38.000000 pyjamas-rfglab-2024.4.1/pyjamas/rannotations/rvector2d.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-17 16:35:19.477719 pyjamas-rfglab-2024.4.1/pyjamas/rcallbacks/
--rw-r--r--   0 rodrigo    (501) staff       (20)     1257 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.4.1/pyjamas/rcallbacks/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     7690 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/rcallbacks/rcallback.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1658 2023-02-07 15:13:59.000000 pyjamas-rfglab-2024.4.1/pyjamas/rcallbacks/rcbabout.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    14800 2023-11-02 21:21:06.000000 pyjamas-rfglab-2024.4.1/pyjamas/rcallbacks/rcbannotations.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    82102 2024-04-16 14:02:15.000000 pyjamas-rfglab-2024.4.1/pyjamas/rcallbacks/rcbbatchprocess.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    66584 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/rcallbacks/rcbclassifiers.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    77584 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.4.1/pyjamas/rcallbacks/rcbimage.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    50542 2024-03-01 22:58:24.000000 pyjamas-rfglab-2024.4.1/pyjamas/rcallbacks/rcbio.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    11360 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.4.1/pyjamas/rcallbacks/rcbmeasure.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    13844 2023-11-22 14:41:28.000000 pyjamas-rfglab-2024.4.1/pyjamas/rcallbacks/rcboptions.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3617 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/rcallbacks/rcbplugins.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-17 16:35:19.480905 pyjamas-rfglab-2024.4.1/pyjamas/rimage/
--rw-r--r--   0 rodrigo    (501) staff       (20)      913 2020-05-28 03:02:49.000000 pyjamas-rfglab-2024.4.1/pyjamas/rimage/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3091 2021-08-22 22:13:16.000000 pyjamas-rfglab-2024.4.1/pyjamas/rimage/csgraph.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3774 2024-03-01 22:58:24.000000 pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimcore.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-17 16:35:19.495320 pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/
--rw-r--r--   0 rodrigo    (501) staff       (20)     1484 2021-02-14 22:27:21.000000 pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3557 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/batchclassifier.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1585 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/batchml.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2740 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/batchneuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     7409 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/batchrecurrentneuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)      275 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/classifier_types.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1173 2020-08-28 21:52:01.000000 pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/featurecalculator.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1387 2020-12-27 23:49:18.000000 pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/featurecalculator_rawimage.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1289 2020-12-27 23:49:18.000000 pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/featurecalculator_rowofpixels.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3104 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/featurecalculator_sog.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    17339 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/rimclassifier.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1824 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/rimlr.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1382 2021-10-27 20:01:04.000000 pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/rimml.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1857 2021-10-27 20:01:04.000000 pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/rimneuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1960 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/rimrecurrentneuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    20979 2023-07-11 19:12:22.000000 pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/rimrescunet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2084 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/rimsvm.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    15508 2023-07-11 19:12:22.000000 pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/rimunet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    69198 2024-03-01 22:58:24.000000 pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimutils.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-17 16:35:19.496885 pyjamas-rfglab-2024.4.1/pyjamas/rplugins/
--rw-r--r--   0 rodrigo    (501) staff       (20)      847 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.4.1/pyjamas/rplugins/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1249 2023-02-19 02:47:05.000000 pyjamas-rfglab-2024.4.1/pyjamas/rplugins/base.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    28427 2024-03-14 22:30:31.000000 pyjamas-rfglab-2024.4.1/pyjamas/rutils.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-17 16:35:19.498806 pyjamas-rfglab-2024.4.1/pyjamas/tests/
--rw-r--r--   0 rodrigo    (501) staff       (20)      796 2023-01-02 00:28:47.000000 pyjamas-rfglab-2024.4.1/pyjamas/tests/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)      857 2023-01-19 20:27:03.000000 pyjamas-rfglab-2024.4.1/pyjamas/tests/conftest.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-17 16:35:19.502047 pyjamas-rfglab-2024.4.1/pyjamas/tests/unit/
--rw-r--r--   0 rodrigo    (501) staff       (20)        0 2022-12-25 02:03:19.000000 pyjamas-rfglab-2024.4.1/pyjamas/tests/unit/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     7461 2024-04-16 14:02:15.000000 pyjamas-rfglab-2024.4.1/pyjamas/tests/unit/pjsfixtures.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    12484 2023-11-22 14:41:28.000000 pyjamas-rfglab-2024.4.1/pyjamas/tests/unit/test_image.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    16029 2023-12-07 19:48:58.000000 pyjamas-rfglab-2024.4.1/pyjamas/tests/unit/test_io.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-17 16:35:19.503110 pyjamas-rfglab-2024.4.1/pyjamas_rfglab.egg-info/
--rw-r--r--   0 rodrigo    (501) staff       (20)     2562 2024-04-17 16:35:18.000000 pyjamas-rfglab-2024.4.1/pyjamas_rfglab.egg-info/SOURCES.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)       38 2024-04-17 16:35:19.504147 pyjamas-rfglab-2024.4.1/setup.cfg
--rw-r--r--   0 rodrigo    (501) staff       (20)     3061 2024-04-17 16:34:42.000000 pyjamas-rfglab-2024.4.1/setup.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.937870 pyjamas-rfglab-2024.4.2/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      265 2023-01-17 21:44:31.000000 pyjamas-rfglab-2024.4.2/MANIFEST.in
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1686 2024-04-24 16:49:57.936980 pyjamas-rfglab-2024.4.2/PKG-INFO
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1202 2023-07-11 19:12:22.000000 pyjamas-rfglab-2024.4.2/README.md
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.865958 pyjamas-rfglab-2024.4.2/pyjamas/
+-rw-r--r--   0 rodrigo    (501) staff       (20)    33144 2020-02-04 05:51:32.000000 pyjamas-rfglab-2024.4.2/pyjamas/LICENSE
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1088 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.4.2/pyjamas/__init__.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.890367 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1645 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    17593 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/adjustcontrast.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    31465 2024-03-22 23:06:04.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/batchanalysis.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    12069 2024-04-16 14:02:15.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/batchflatfield.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     5509 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/batchprojectconcat.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     6823 2024-04-16 14:02:15.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/batchresize.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2980 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/classifierdialogABC.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3199 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/classifiertype.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     6437 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/expandnpropagateseeds.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     5227 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/expandseeds.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    13000 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/findseeds.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    11361 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/logregression.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3453 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/matplotlibdialog.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     8858 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/measurepoly.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    13277 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/neuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     8699 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/nonmax_suppr.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     5533 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/propagateseeds.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    14588 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/rescuneuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    12510 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/svm.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2243 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/textdialog.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2817 2023-12-27 20:45:04.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/texteditdialog.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     4082 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dialogs/timepoints.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1806 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/dragdropmainwindow.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.892195 pyjamas-rfglab-2024.4.2/pyjamas/external/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      899 2021-05-09 22:07:44.000000 pyjamas-rfglab-2024.4.2/pyjamas/external/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     6852 2020-07-11 20:09:58.000000 pyjamas-rfglab-2024.4.2/pyjamas/external/pascal_voc_io.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     4930 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/orthogonalviewswindow.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    52457 2024-04-24 16:48:36.000000 pyjamas-rfglab-2024.4.2/pyjamas/pjscore.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    33519 2023-11-22 14:41:28.000000 pyjamas-rfglab-2024.4.2/pyjamas/pjseventfilter.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2123 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/pjsthreads.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)  2950837 2023-06-21 15:47:44.000000 pyjamas-rfglab-2024.4.2/pyjamas/pyjamas.tif
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.896294 pyjamas-rfglab-2024.4.2/pyjamas/rannotations/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      924 2022-06-20 21:44:00.000000 pyjamas-rfglab-2024.4.2/pyjamas/rannotations/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)      856 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.4.2/pyjamas/rannotations/rannotation.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    16818 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/rannotations/rpolyline.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2288 2022-08-14 20:59:38.000000 pyjamas-rfglab-2024.4.2/pyjamas/rannotations/rvector2d.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.910721 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1257 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     7690 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcallback.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1658 2023-02-07 15:13:59.000000 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbabout.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    14800 2023-11-02 21:21:06.000000 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbannotations.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    82216 2024-04-24 16:48:36.000000 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbbatchprocess.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    66584 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbclassifiers.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    77584 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbimage.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    52357 2024-04-24 16:48:36.000000 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbio.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    11360 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbmeasure.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    13844 2023-11-22 14:41:28.000000 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcboptions.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3617 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbplugins.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.913529 pyjamas-rfglab-2024.4.2/pyjamas/rimage/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      913 2020-05-28 03:02:49.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3091 2021-08-22 22:13:16.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/csgraph.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3774 2024-03-01 22:58:24.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimcore.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.928825 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1484 2021-02-14 22:27:21.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3557 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/batchclassifier.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1585 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/batchml.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2740 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/batchneuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     7409 2023-08-11 20:09:20.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/batchrecurrentneuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)      275 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/classifier_types.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1173 2020-08-28 21:52:01.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/featurecalculator.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1387 2020-12-27 23:49:18.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/featurecalculator_rawimage.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1289 2020-12-27 23:49:18.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/featurecalculator_rowofpixels.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3104 2024-03-12 21:08:54.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/featurecalculator_sog.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    17339 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimclassifier.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1824 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimlr.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1382 2021-10-27 20:01:04.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimml.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1857 2021-10-27 20:01:04.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimneuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1960 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimrecurrentneuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    20979 2023-07-11 19:12:22.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimrescunet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2084 2023-04-12 16:40:46.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimsvm.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    15508 2023-07-11 19:12:22.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimunet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    69198 2024-03-01 22:58:24.000000 pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimutils.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.930957 pyjamas-rfglab-2024.4.2/pyjamas/rplugins/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      847 2020-01-17 04:15:16.000000 pyjamas-rfglab-2024.4.2/pyjamas/rplugins/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1249 2023-02-19 02:47:05.000000 pyjamas-rfglab-2024.4.2/pyjamas/rplugins/base.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    28427 2024-03-14 22:30:31.000000 pyjamas-rfglab-2024.4.2/pyjamas/rutils.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.932304 pyjamas-rfglab-2024.4.2/pyjamas/tests/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      796 2023-01-02 00:28:47.000000 pyjamas-rfglab-2024.4.2/pyjamas/tests/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)      857 2023-01-19 20:27:03.000000 pyjamas-rfglab-2024.4.2/pyjamas/tests/conftest.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.935326 pyjamas-rfglab-2024.4.2/pyjamas/tests/unit/
+-rw-r--r--   0 rodrigo    (501) staff       (20)        0 2022-12-25 02:03:19.000000 pyjamas-rfglab-2024.4.2/pyjamas/tests/unit/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     7505 2024-04-24 16:48:36.000000 pyjamas-rfglab-2024.4.2/pyjamas/tests/unit/pjsfixtures.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    12484 2023-11-22 14:41:28.000000 pyjamas-rfglab-2024.4.2/pyjamas/tests/unit/test_image.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    16118 2024-04-24 16:48:36.000000 pyjamas-rfglab-2024.4.2/pyjamas/tests/unit/test_io.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2024-04-24 16:49:57.936321 pyjamas-rfglab-2024.4.2/pyjamas_rfglab.egg-info/
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2562 2024-04-24 16:49:57.000000 pyjamas-rfglab-2024.4.2/pyjamas_rfglab.egg-info/SOURCES.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)       38 2024-04-24 16:49:57.938007 pyjamas-rfglab-2024.4.2/setup.cfg
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3061 2024-04-17 16:34:42.000000 pyjamas-rfglab-2024.4.2/setup.py
```

### Comparing `pyjamas-rfglab-2024.4.1/PKG-INFO` & `pyjamas-rfglab-2024.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjamas-rfglab
-Version: 2024.4.1
+Version: 2024.4.2
 Summary: PyJAMAS is Just A More Awesome SIESTA
 Home-page: https://bitbucket.org/rfg_lab/pyjamas
 Author: Rodrigo Fernandez-Gonzalez
 Author-email: rodrigo.fernandez.gonzalez@utoronto.ca
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `pyjamas-rfglab-2024.4.1/README.md` & `pyjamas-rfglab-2024.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/LICENSE` & `pyjamas-rfglab-2024.4.2/pyjamas/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/__init__.py` & `pyjamas-rfglab-2024.4.2/pyjamas/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/dialogs/__init__.py` & `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/dialogs/adjustcontrast.py` & `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/adjustcontrast.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/dialogs/batchanalysis.py` & `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/batchanalysis.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/dialogs/batchflatfield.py` & `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/batchflatfield.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/dialogs/batchprojectconcat.py` & `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/batchprojectconcat.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/dialogs/batchresize.py` & `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/batchresize.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/dialogs/classifierdialogABC.py` & `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/classifierdialogABC.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/dialogs/classifiertype.py` & `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/classifiertype.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/dialogs/expandnpropagateseeds.py` & `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/expandnpropagateseeds.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/dialogs/expandseeds.py` & `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/expandseeds.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/dialogs/findseeds.py` & `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/findseeds.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/dialogs/logregression.py` & `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/logregression.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/dialogs/matplotlibdialog.py` & `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/matplotlibdialog.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/dialogs/measurepoly.py` & `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/measurepoly.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/dialogs/neuralnet.py` & `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/neuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/dialogs/nonmax_suppr.py` & `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/nonmax_suppr.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/dialogs/propagateseeds.py` & `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/propagateseeds.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/dialogs/rescuneuralnet.py` & `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/rescuneuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/dialogs/svm.py` & `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/svm.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/dialogs/textdialog.py` & `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/textdialog.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/dialogs/texteditdialog.py` & `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/texteditdialog.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/dialogs/timepoints.py` & `pyjamas-rfglab-2024.4.2/pyjamas/dialogs/timepoints.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/dragdropmainwindow.py` & `pyjamas-rfglab-2024.4.2/pyjamas/dragdropmainwindow.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/external/__init__.py` & `pyjamas-rfglab-2024.4.2/pyjamas/external/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/external/pascal_voc_io.py` & `pyjamas-rfglab-2024.4.2/pyjamas/external/pascal_voc_io.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/orthogonalviewswindow.py` & `pyjamas-rfglab-2024.4.2/pyjamas/orthogonalviewswindow.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/pjscore.py` & `pyjamas-rfglab-2024.4.2/pyjamas/pjscore.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     livewire_gaussian_sigma: float = 0.
     balloon_crop_size: int = 50  # crop size used to inflate balloons
     livewire_shortest_path_fn = tuple(rimcore.rimage.livewire_shortest_path_fns.values())[0]  # fn to calculate shortest path between two pixels
 
     undo_stack_size: int = 500
 
     # Read version.
-    __version__: str = '2024.4.1'
+    __version__: str = '2024.4.2'
 
     def __init__(self):
         self.initData()  # Initialize object variables.
         self.setupUI()  # Build the GUI.
 
     def setupUI(self):
         self.app = QtWidgets.QApplication(sys.argv)
```

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/pjseventfilter.py` & `pyjamas-rfglab-2024.4.2/pyjamas/pjseventfilter.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/pjsthreads.py` & `pyjamas-rfglab-2024.4.2/pyjamas/pjsthreads.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/pyjamas.tif` & `pyjamas-rfglab-2024.4.2/pyjamas/pyjamas.tif`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rannotations/__init__.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rannotations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rannotations/rannotation.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rannotations/rannotation.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rannotations/rpolyline.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rannotations/rpolyline.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rannotations/rvector2d.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rannotations/rvector2d.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rcallbacks/__init__.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rcallbacks/rcallback.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcallback.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rcallbacks/rcbabout.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbabout.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rcallbacks/rcbannotations.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbannotations.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rcallbacks/rcbbatchprocess.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbbatchprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,23 +256,30 @@
 
     def cbBatchFlatFieldCorrection(self, parameters: Optional[dict] = None) -> bool:
         """
         Flat field correction of all images within a given folder or folder tree.
 
         :param parameters: dictionary with parameters, a dialog will open if the value is none.
 
-            ``input_folder``: absolute path to the folder containing all images to be resized.
-            ``darkfield_file``: path to the file containing the image to correct for darkfield, '' or None of no darkfield correction.
-            ``flatfield_file``: path to the file containing the image to correct for flatfield, '' or None of no flatfield correction.
-            ``crop_dims``: tuple with (row, col) dimensions to crop the images before applying any corrections, None for no cropping.
-            ``bg_mode``: background subtraction, None if no background subtraction, 'mode' if the background is the volume mode.
-            ``input_substr``: substring to refine input files corrected, '' to correct all images.
-            ``file_suffix``: suffix to add to the file name of the corrected images.
+            ``input_folder``:
+                absolute path to the folder containing all images to be resized.
+            ``darkfield_file``:
+                path to the file containing the image to correct for darkfield, '' or None of no darkfield correction.
+            ``flatfield_file``:
+                path to the file containing the image to correct for flatfield, '' or None of no flatfield correction.
+            ``crop_dims``:
+                tuple with (row, col) dimensions to crop the images before applying any corrections, None for no cropping.
+            ``bg_mode``:
+                background subtraction, None if no background subtraction, 'mode' if the background is the volume mode.
+            ``input_substr``:
+                substring to refine input files corrected, '' to correct all images.
+            ``file_suffix``:
+                suffix to add to the file name of the corrected images.
 
-        :return: True if resizing complete, False otherwise.
+        :return: True if correction complete, False otherwise.
         """
         # Get folder name.
         continue_flag: bool = True
 
         if parameters is None or parameters is False:
             dialog = QtWidgets.QDialog()
             ui = BatchFlatFieldCorrectionDialog()
```

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rcallbacks/rcbclassifiers.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbclassifiers.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rcallbacks/rcbimage.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbimage.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rcallbacks/rcbio.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbio.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from pyjamas.rimage.rimutils import rimutils
 from pyjamas.rimage.rimml.rimlr import lr
 from pyjamas.rimage.rimml.rimsvm import svm
 from pyjamas.rimage.rimml.rimunet import UNet
 from pyjamas.rutils import RUtils
 from pyjamas.rimage.rimml.classifier_types import classifier_types
 from pyjamas.dialogs.classifiertype import ClassifierTypeDialog
+from pyjamas.dialogs.timepoints import TimePointsDialog
 from pyjamas.rimage.rimml.batchrecurrentneuralnet import BatchRecurrentNeuralNet
 from pyjamas.rimage.rimml.rimrescunet import ReSCUNet
 
 
 class RCBIO(RCallback):
     FILENAME_BASE: str = "cell_"
     FILENAME_FIDUCIAL_LENGTH: int = 5
@@ -320,15 +321,16 @@
         path_to_mask: str = os.path.join(self.pjs.cwd, filename, "mask", filenameext)
         cwd = self.pjs.cwd
 
         # Save image.
         self.pjs.io.cbSaveROI(path_to_image, (minx, maxx), (miny, maxy), (self.pjs.curslice, self.pjs.curslice))
 
         # Export mask.
-        self.pjs.io.cbExportCurrentAnnotationsBinaryImage(path_to_mask, numpy.array([[minx, miny], [maxx, maxy]]))
+        self.pjs.io.cbExportCurrentAnnotationsBinaryImage(path_to_mask, numpy.array([[minx, miny], [maxx, maxy]]),
+                                                          firstSlice=self.pjs.curslice + 1, lastSlice=self.pjs.curslice + 1)
 
         # Important, as cbSaveROI and cbExportCurrentAnnotationsBinaryImage may affect the cwd.
         self.pjs.cwd = cwd
 
         return True
 
     def cbSaveROI(self, filename: Optional[str] = None, x_range: Tuple[int, int] = False,
@@ -567,20 +569,23 @@
 
         self.pjs.statusbar.showMessage(f"Saved {filename}.")
 
         return True
 
     def cbExportCurrentAnnotationsBinaryImage(self, filename: Optional[str] = None,
                                               polyline: Optional[numpy.ndarray] = None,
+                                              firstSlice: Optional[int] = None, lastSlice: Optional[int] = None,
                                               message: str = "Save annotations ...") -> bool:
         """
         Save current slice annotations as a binary image displaying one mask per object.
 
         :param filename: '' for automated naming based on the current image name (pjs.filename). If not provided, a dialog will open.
         :param polyline: ndarray with two columns containing the x, y coordinates of the ROI; if None or empty array, use the entire image as ROI.
+        :param firstSlice: slice number for the first slice to use (minimum is 1); a dialog will open if this parameter is None.
+        :param lastSlice: slice number for the last slice to use; a dialog will open if this parameter is None.
         :param message: string to display as the dialog box title.
         :return:
         """
         # Get file name.
         if filename is None or filename is False:  # When the menu option is clicked on, for some reason that I do not understand, the function is called with filename = False, which causes a bunch of problems.
             fname = QtWidgets.QFileDialog.getSaveFileName(None, message,
                                                           self.pjs.cwd,
@@ -596,15 +601,33 @@
             filename = os.path.join(self.pjs.cwd, fname)
 
         self.pjs.cwd = os.path.dirname(filename)
 
         if filename[-4:] not in PyJAMAS.image_extensions:
             filename = RUtils.set_extension(filename, PyJAMAS.image_extensions[0])
 
-        if (polyline is None) | (polyline == []):
+        # Get the slices to use.
+        if (firstSlice is False or firstSlice is None or lastSlice is False or lastSlice is None) and self.pjs is not None:
+            dialog = QtWidgets.QDialog()
+            ui = TimePointsDialog()
+
+            lastSlice = 1 if self.pjs.n_frames == 1 else self.pjs.slices.shape[0]
+            ui.setupUi(dialog, firstslice=self.pjs.curslice + 1, lastslice=lastSlice)
+
+            dialog.exec()
+            dialog.show()
+            # If the dialog was closed by pressing OK, then run the measurements.
+            continue_flag = dialog.result() == QtWidgets.QDialog.DialogCode.Accepted
+            firstSlice, lastSlice = ui.parameters()
+
+            dialog.close()
+        else:
+            continue_flag = True
+
+        if (polyline is None) | (polyline == []) | (polyline is False):
             minx = 0
             miny = 0
             maxx = self.pjs.width - 1
             maxy = self.pjs.height - 1
         else:
             minx, miny, maxx, maxy = self.get_coordinate_bounds(coordinates=polyline)
 
@@ -612,17 +635,27 @@
         transform = QtGui.QTransform()
         transform.translate(-minx, -miny)
 
         # Transform using a one pixel less wide and less tall size such that the polyline that determines the ROI
         # (if there was one) is not included in the regions within the image.
         _, new_polylines, _ = self.transform_annotations(transform, (maxx - minx - 1, maxy - miny - 1))
 
-        thepolylines = new_polylines[self.pjs.curslice]
+        if continue_flag:
+            if firstSlice <= lastSlice:
+                thepolylines = new_polylines[firstSlice - 1:lastSlice]
+            else:
+                thepolylines = new_polylines[lastSlice:firstSlice]
+        else:
+            return False
 
-        mask_image = rimutils.mask_from_polylines((maxy - miny + 1, maxx - minx + 1), thepolylines, self.pjs.brush_size)
+        mask_image = numpy.zeros((len(thepolylines), maxy - miny + 1, maxx - minx + 1), dtype=bool)
+        for t, these_polylines in enumerate(thepolylines):
+            mask_image[t] = rimutils.mask_from_polylines((maxy - miny + 1, maxx - minx + 1), these_polylines, self.pjs.brush_size)
+        if firstSlice == lastSlice:  # Reduce dimensions if the mask should only be one slice
+            mask_image = mask_image[0]
         rimutils.write_stack(filename, mask_image)
 
         self.pjs.statusbar.showMessage(f"Saved {filename}.")
 
         return True
 
     def cbSaveClassifier(self, filename: Optional[str] = None,
```

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rcallbacks/rcbmeasure.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbmeasure.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rcallbacks/rcboptions.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcboptions.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rcallbacks/rcbplugins.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rcallbacks/rcbplugins.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rimage/__init__.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rimage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rimage/csgraph.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rimage/csgraph.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimcore.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimcore.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/__init__.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/batchclassifier.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/batchclassifier.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/batchml.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/batchml.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/batchneuralnet.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/batchneuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/batchrecurrentneuralnet.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/batchrecurrentneuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/featurecalculator.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/featurecalculator.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/featurecalculator_rawimage.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/featurecalculator_rawimage.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/featurecalculator_rowofpixels.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/featurecalculator_rowofpixels.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/featurecalculator_sog.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/featurecalculator_sog.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/rimclassifier.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimclassifier.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/rimlr.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimlr.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/rimml.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimml.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/rimneuralnet.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimneuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/rimrecurrentneuralnet.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimrecurrentneuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/rimrescunet.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimrescunet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/rimsvm.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimsvm.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimml/rimunet.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimml/rimunet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rimage/rimutils.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rimage/rimutils.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rplugins/__init__.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rplugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rplugins/base.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rplugins/base.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/rutils.py` & `pyjamas-rfglab-2024.4.2/pyjamas/rutils.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/tests/__init__.py` & `pyjamas-rfglab-2024.4.2/pyjamas/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/tests/conftest.py` & `pyjamas-rfglab-2024.4.2/pyjamas/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/tests/unit/pjsfixtures.py` & `pyjamas-rfglab-2024.4.2/pyjamas/tests/unit/pjsfixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os.path
 from typing import List, Tuple
 
+import pyjamas
 import cv2
 import numpy
 import pytest
 import skimage
 
-FIXTURE_DIR: str = '/Users/rodrigo/src/pyjamas_dev/pyjamas/tests/unit/fixtures/'
+FIXTURE_DIR: str = os.path.join(os.path.split(pyjamas.__file__)[0], "tests", "unit", "fixtures")
 LOGO_FIXTURE: str = 'original_logo.tif'
 IMAGE_FIXTURE: str = 'image.tif'
 CLASSIFIER_FIXTURE: Tuple[str, str] = ('classifier_lr.cfr', 'classifier_svm.cfr')
 DISPLAY_FIXTURE: str = 'display.tif'
 BINMASKS_FIXTURE: str = 'binmasks.tif'
 MOVIE_FIXTURE: str = 'movie.avi'
 PJSANNOTATIONS_FIXTURE: str = 'annotations.pjs'
@@ -24,15 +25,15 @@
 FLIPPED_LR_FIXTURE: str = 'flipped_lr.tif'
 FLIPPED_UD_FIXTURE: str = 'flipped_ud.tif'
 INVERTED_FIXTURE: str = 'inverted.tif'
 GRADIENT_FIXTURE: str = 'gradient.tif'
 KYMOGRAPH_FIXTURE: str = 'kymograph.tif'
 REGISTERED_FIXTURE: str = 'registered.tif'
 TMP_IMG_FILE: str = 'image.tif'
-TMP_DIR: str = '/Users/rodrigo/src/pyjamas_dev/pyjamas/tests/tmp/'
+TMP_DIR: str = os.path.join(os.path.split(pyjamas.__file__)[0], "tests", "tmp")
 TMP_DISP_FILE: str = 'display.tif'
 TMP_BINMASKS_FILE: str = 'binmasks.tif'
 TMP_MOVIE_FILE: str = 'movie.avi'
 TMP_PJS_FILE: str = 'annotations.pjs'
 TMP_MAT_FILE: str = 'annotations.mat'
 TMP_SINGLE_CELL_PJS_FILE: str = 'cell_00001.pjs'
 PIX_PERCENTILE_LIMITS: Tuple[int, int] = (10, 90)
@@ -53,14 +54,15 @@
 BATCH_FLATFIELD_DIR: str = 'batch_ffc/images_for_correction'
 BATCH_FLATFIELD_OUTPUTDIR: str = 'batch_ffc/corrected_images'
 BATCH_FLATFIELD_FLATFIELDIMAGEPATH: str = 'batch_ffc/ffc_image.tif'
 BATCH_FLATFIELD_DARKIMAGEPATH: str = 'batch_ffc/dark_field_image.tif'
 BATCH_FLATFIELD_SUBSTR: str = ''
 BATCH_FLATFIELD_FILESUFFIX: str = '_ffc_corrected'
 BATCH_FLATFIELD_CROPDIMS: Tuple[int, int] = (512, 512)
+
 @pytest.fixture
 def image_fixture():
     return skimage.io.imread(os.path.join(FIXTURE_DIR, IMAGE_FIXTURE))
 
 
 @pytest.fixture
 def display_fixture():
@@ -243,8 +245,7 @@
             'darkfield_file': os.path.join(FIXTURE_DIR, BATCH_FLATFIELD_DARKIMAGEPATH),
             'flatfield_file': os.path.join(FIXTURE_DIR, BATCH_FLATFIELD_FLATFIELDIMAGEPATH),
             'crop_dims': BATCH_FLATFIELD_CROPDIMS,
             'file_suffix': BATCH_FLATFIELD_FILESUFFIX,
             'input_substr': BATCH_FLATFIELD_SUBSTR,
             'output_folder': os.path.join(FIXTURE_DIR, BATCH_FLATFIELD_OUTPUTDIR)
             }
-
```

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/tests/unit/test_image.py` & `pyjamas-rfglab-2024.4.2/pyjamas/tests/unit/test_image.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas/tests/unit/test_io.py` & `pyjamas-rfglab-2024.4.2/pyjamas/tests/unit/test_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -341,14 +341,15 @@
     PyJAMAS_FIXTURE.image.cbExpandSeeds(1, 1, sigma=2.0,
                                         wait_for_thread=True)  # you need to wait, otherwise the test fails!!!
     PyJAMAS_FIXTURE.removePolylineByIndex(0, 0)
 
     PyJAMAS_FIXTURE.io.cbExportCurrentAnnotationsBinaryImage(
         os.path.join(pjsfixtures.TMP_DIR, pjsfixtures.TMP_BINMASKS_FILE),
         numpy.array([[0, 0], [PyJAMAS_FIXTURE.width - 1,
-                              PyJAMAS_FIXTURE.height - 1]]))
+                              PyJAMAS_FIXTURE.height - 1]]),
+        firstSlice=PyJAMAS_FIXTURE.curslice + 1, lastSlice=PyJAMAS_FIXTURE.curslice + 1)
 
     assert numpy.array_equal(binmasks_fixture,
                              skimage.io.imread(os.path.join(pjsfixtures.TMP_DIR, pjsfixtures.TMP_BINMASKS_FILE)))
 
 
 PyJAMAS_FIXTURE.app.quit()
```

### Comparing `pyjamas-rfglab-2024.4.1/pyjamas_rfglab.egg-info/SOURCES.txt` & `pyjamas-rfglab-2024.4.2/pyjamas_rfglab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2024.4.1/setup.py` & `pyjamas-rfglab-2024.4.2/setup.py`

 * *Files identical despite different names*

