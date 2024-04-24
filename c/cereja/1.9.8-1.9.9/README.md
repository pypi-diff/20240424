# Comparing `tmp/cereja-1.9.8.tar.gz` & `tmp/cereja-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cereja-1.9.8.tar", last modified: Sun Mar 17 21:45:13 2024, max compression
+gzip compressed data, was "cereja-1.9.9.tar", last modified: Wed Apr 24 07:41:01 2024, max compression
```

## Comparing `cereja-1.9.8.tar` & `cereja-1.9.9.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:45:13.269238 cereja-1.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-17 21:45:02.000000 cereja-1.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12633 2024-03-17 21:45:13.269238 cereja-1.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-03-17 21:45:02.000000 cereja-1.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:45:13.261238 cereja-1.9.8/cereja/
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:45:13.261238 cereja-1.9.8/cereja/_requests/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9236 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/_requests/_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/_requests/request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:45:13.261238 cereja-1.9.8/cereja/array/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19895 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/array/_array.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:45:13.261238 cereja-1.9.8/cereja/concurrently/
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/concurrently/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9957 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/concurrently/_concurrence.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/concurrently/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:45:13.265238 cereja-1.9.8/cereja/config/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7974 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/config/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/config/cj_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/config/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:45:13.265238 cereja-1.9.8/cereja/date/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/date/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/date/_datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:45:13.265238 cereja-1.9.8/cereja/display/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35095 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/display/_display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:45:13.265238 cereja-1.9.8/cereja/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/experimental/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:45:13.265238 cereja-1.9.8/cereja/file/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32679 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/file/_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:45:13.265238 cereja-1.9.8/cereja/geolinear/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/geolinear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14813 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/geolinear/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/geolinear/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:45:13.265238 cereja-1.9.8/cereja/hashtools/
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/hashtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/hashtools/_hash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:45:13.265238 cereja-1.9.8/cereja/mathtools/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/mathtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/mathtools/_op.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:45:13.265238 cereja-1.9.8/cereja/mltools/
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/mltools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20700 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/mltools/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/mltools/pln.py
--rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/mltools/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    15584 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/mltools/split_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:45:13.269238 cereja-1.9.8/cereja/system/
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16560 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/system/_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    25789 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/system/_win32.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/system/commons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/system/unicode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:45:13.269238 cereja-1.9.8/cereja/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46253 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/utils/colab.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-03-17 21:45:02.000000 cereja-1.9.8/cereja/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:45:13.269238 cereja-1.9.8/cereja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12633 2024-03-17 21:45:13.000000 cereja-1.9.8/cereja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-03-17 21:45:13.000000 cereja-1.9.8/cereja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 21:45:13.000000 cereja-1.9.8/cereja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-17 21:45:13.000000 cereja-1.9.8/cereja.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-17 21:45:02.000000 cereja-1.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-17 21:45:13.269238 cereja-1.9.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:45:13.269238 cereja-1.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-17 21:45:02.000000 cereja-1.9.8/tests/testhashtools.py
--rw-r--r--   0 runner    (1001) docker     (127)    13336 2024-03-17 21:45:02.000000 cereja-1.9.8/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-03-17 21:45:02.000000 cereja-1.9.8/tests/testsfiletools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-03-17 21:45:02.000000 cereja-1.9.8/tests/testsgeolinear.py
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-03-17 21:45:02.000000 cereja-1.9.8/tests/testsmltools.py
--rw-r--r--   0 runner    (1001) docker     (127)    17091 2024-03-17 21:45:02.000000 cereja-1.9.8/tests/testsutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:41:01.877065 cereja-1.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-24 07:40:49.000000 cereja-1.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12633 2024-04-24 07:41:01.877065 cereja-1.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-04-24 07:40:49.000000 cereja-1.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:41:01.865064 cereja-1.9.9/cereja/
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:41:01.869064 cereja-1.9.9/cereja/_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9236 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/_requests/_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/_requests/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:41:01.869064 cereja-1.9.9/cereja/array/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19895 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/array/_array.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:41:01.869064 cereja-1.9.9/cereja/concurrently/
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/concurrently/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9957 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/concurrently/_concurrence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8429 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/concurrently/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:41:01.869064 cereja-1.9.9/cereja/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7974 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/config/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/config/cj_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/config/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:41:01.869064 cereja-1.9.9/cereja/date/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/date/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/date/_datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:41:01.869064 cereja-1.9.9/cereja/display/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35095 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/display/_display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:41:01.869064 cereja-1.9.9/cereja/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/experimental/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:41:01.869064 cereja-1.9.9/cereja/file/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32679 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/file/_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:41:01.869064 cereja-1.9.9/cereja/geolinear/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/geolinear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14813 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/geolinear/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/geolinear/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:41:01.869064 cereja-1.9.9/cereja/hashtools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/hashtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/hashtools/_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:41:01.873065 cereja-1.9.9/cereja/mathtools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/mathtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/mathtools/_op.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:41:01.873065 cereja-1.9.9/cereja/mltools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/mltools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20700 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/mltools/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/mltools/pln.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/mltools/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15584 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/mltools/split_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:41:01.873065 cereja-1.9.9/cereja/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16560 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/system/_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26284 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/system/_win32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/system/commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/system/unicode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:41:01.873065 cereja-1.9.9/cereja/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45482 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/utils/colab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-24 07:40:49.000000 cereja-1.9.9/cereja/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:41:01.873065 cereja-1.9.9/cereja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12633 2024-04-24 07:41:01.000000 cereja-1.9.9/cereja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-24 07:41:01.000000 cereja-1.9.9/cereja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 07:41:01.000000 cereja-1.9.9/cereja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 07:41:01.000000 cereja-1.9.9/cereja.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-24 07:40:49.000000 cereja-1.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 07:41:01.877065 cereja-1.9.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:41:01.873065 cereja-1.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-24 07:40:49.000000 cereja-1.9.9/tests/testhashtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13336 2024-04-24 07:40:49.000000 cereja-1.9.9/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-24 07:40:49.000000 cereja-1.9.9/tests/testsfiletools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-24 07:40:49.000000 cereja-1.9.9/tests/testsgeolinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-04-24 07:40:49.000000 cereja-1.9.9/tests/testsmltools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17091 2024-04-24 07:40:49.000000 cereja-1.9.9/tests/testsutils.py
```

### Comparing `cereja-1.9.8/LICENSE` & `cereja-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/PKG-INFO` & `cereja-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cereja
-Version: 1.9.8
+Version: 1.9.9
 Summary: Cereja is a bundle of useful functions that I don't want to rewrite.
 Author-email: Joab Leite <leitejoab@gmail.com>
 License: Copyright (c) 2019 The Cereja Project
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `cereja-1.9.8/README.md` & `cereja-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/__init__.py` & `cereja-1.9.9/cereja/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from .date import *
 from . import hashtools
 from . import mathtools
 from .mathtools import *
 from . import experimental
 from ._requests import request
 
-VERSION = "1.9.8.final.0"
+VERSION = "1.9.9.final.0"
 __version__ = get_version_pep440_compliant(VERSION)
 
 
 def print_cereja_version():
     # This is important, as there may be an exception if the terminal does not support unicode bmp
     try:
         unicode_ = f"\033[31m\U0001F352\033[0;0m"
```

### Comparing `cereja-1.9.8/cereja/__main__.py` & `cereja-1.9.9/cereja/__main__.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/_requests/__init__.py` & `cereja-1.9.9/cereja/_requests/__init__.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/_requests/_http.py` & `cereja-1.9.9/cereja/_requests/_http.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/_requests/request.py` & `cereja-1.9.9/cereja/_requests/request.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/array/__init__.py` & `cereja-1.9.9/cereja/array/__init__.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/array/_array.py` & `cereja-1.9.9/cereja/array/_array.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/concurrently/__init__.py` & `cereja-1.9.9/cereja/concurrently/__init__.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/concurrently/_concurrence.py` & `cereja-1.9.9/cereja/concurrently/_concurrence.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/config/_constants.py` & `cereja-1.9.9/cereja/config/_constants.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/config/cj_types.py` & `cereja-1.9.9/cereja/config/cj_types.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/config/conf.py` & `cereja-1.9.9/cereja/config/conf.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/date/_datetime.py` & `cereja-1.9.9/cereja/date/_datetime.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/display/__init__.py` & `cereja-1.9.9/cereja/display/__init__.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/display/_display.py` & `cereja-1.9.9/cereja/display/_display.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/experimental/commons.py` & `cereja-1.9.9/cereja/experimental/commons.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/file/__init__.py` & `cereja-1.9.9/cereja/file/__init__.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/file/_io.py` & `cereja-1.9.9/cereja/file/_io.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/geolinear/point.py` & `cereja-1.9.9/cereja/geolinear/point.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/geolinear/utils.py` & `cereja-1.9.9/cereja/geolinear/utils.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/hashtools/__init__.py` & `cereja-1.9.9/cereja/hashtools/__init__.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/hashtools/_hash.py` & `cereja-1.9.9/cereja/hashtools/_hash.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/mathtools/__init__.py` & `cereja-1.9.9/cereja/mathtools/__init__.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/mathtools/_op.py` & `cereja-1.9.9/cereja/mathtools/_op.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/mltools/__init__.py` & `cereja-1.9.9/cereja/mltools/__init__.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/mltools/data.py` & `cereja-1.9.9/cereja/mltools/data.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/mltools/pln.py` & `cereja-1.9.9/cereja/mltools/pln.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/mltools/preprocess.py` & `cereja-1.9.9/cereja/mltools/preprocess.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/mltools/split_data.py` & `cereja-1.9.9/cereja/mltools/split_data.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/system/__init__.py` & `cereja-1.9.9/cereja/system/__init__.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/system/_path.py` & `cereja-1.9.9/cereja/system/_path.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/system/_win32.py` & `cereja-1.9.9/cereja/system/_win32.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 EnumWindowsProc = ctypes.WINFUNCTYPE(BOOL, HWND, LPARAM)
 user32 = ctypes.windll.user32
 GetWindowRect = user32.GetWindowRect
 SetWindowPos = user32.SetWindowPos
 IsIconic = user32.IsIconic
 IsZoomed = user32.IsZoomed
 GetWindowDC = user32.GetWindowDC
+GetDC = user32.GetDC
 GetForegroundWindow = user32.GetForegroundWindow
 ReleaseDC = user32.ReleaseDC
 PrintWindow = user32.PrintWindow
 CreateCompatibleDC = ctypes.windll.gdi32.CreateCompatibleDC
 CreateCompatibleBitmap = ctypes.windll.gdi32.CreateCompatibleBitmap
 SelectObject = ctypes.windll.gdi32.SelectObject
 BitBlt = ctypes.windll.gdi32.BitBlt
@@ -181,15 +182,14 @@
         self._is_async = is_async
         self.user32 = ctypes.windll.user32
         self._stop_listen = True
         self._hwnd = hwnd
         self._max_time_simule_key_press = self.MAX_TIME_SIMULE_KEY_PRESS
         self._key_press_callbacks = None
 
-
     @property
     def is_async(self):
         return self._is_async
 
     @is_async.setter
     def is_async(self, v):
         self._is_async = bool(v)
@@ -610,19 +610,20 @@
             return "Minimized"
         elif IsZoomed(self.hwnd):
             return "Maximized"
         else:
             return "Normal"
 
     def capture_image_bmp(self, filepath=None, only_window_content=True):
+        if not user32.IsZoomed(self.hwnd):
+            ctypes.windll.user32.ShowWindow(self.hwnd, 4)
         # Obtenha o DC da janela e crie um DC compatível
-        window_dc = GetWindowDC(self.hwnd)
+        window_dc = GetWindowDC(self.hwnd) if only_window_content else GetDC(self.hwnd)
         mem_dc = CreateCompatibleDC(window_dc)
 
-
         if only_window_content:
             width, height = self.size_window_content
         else:
             # Obtenha as dimensões
             left, top, right, bottom = self.dimensions
             width = right - left
             height = bottom - top
@@ -640,15 +641,16 @@
         bitmap_info.bmiHeader.biWidth = width
         bitmap_info.bmiHeader.biHeight = -height  # Negativo para origem no topo
         bitmap_info.bmiHeader.biPlanes = 1
         bitmap_info.bmiHeader.biBitCount = 32
         bitmap_info.bmiHeader.biCompression = BI_RGB
 
         # Cria buffer para os dados da imagem
-        bitmap_data = ctypes.create_string_buffer(abs(bitmap_info.bmiHeader.biWidth * bitmap_info.bmiHeader.biHeight * 4))
+        bitmap_data = ctypes.create_string_buffer(
+            abs(bitmap_info.bmiHeader.biWidth * bitmap_info.bmiHeader.biHeight * 4))
         # Obtém os dados da imagem
         GetDIBits(mem_dc, screenshot, 0, height, bitmap_data, ctypes.byref(bitmap_info), DIB_RGB_COLORS)
 
         # Se um filepath foi fornecido, salva a imagem como um arquivo BMP
         if filepath:
             with open(filepath, 'wb') as bmp_file:
                 # Escreve o cabeçalho do arquivo BMP
@@ -665,15 +667,14 @@
         # Limpeza
         DeleteObject(screenshot)
         DeleteDC(mem_dc)
         ReleaseDC(self.hwnd, window_dc)
 
         return bitmap_data.raw
 
-
     # SHOW implements
     def hide(self):
         """
         Oculta a janela e ativa outra janela.
 
         Este comando remove completamente a janela da área de trabalho e da barra de tarefas, tornando-a inacessível
         até que seja programaticamente reexibida.
@@ -715,7 +716,15 @@
     def restore(self):
         """Restaura a janela para seu tamanho e posição originais."""
         ShowWindow(self.hwnd, 9)
 
     def show_default(self):
         """Define o estado de exibição com base no valor SW_ especificado no STARTUPINFO."""
         ShowWindow(self.hwnd, 10)
+
+    def set_foreground(self):
+        """Tenta trazer a janela para o primeiro plano."""
+        ctypes.windll.user32.SetForegroundWindow(self.hwnd)
+
+    def bring_to_top(self):
+        """Move a janela para o topo do Z-Order sem necessariamente ativá-la."""
+        ctypes.windll.user32.BringWindowToTop(self.hwnd)
```

### Comparing `cereja-1.9.8/cereja/system/commons.py` & `cereja-1.9.9/cereja/system/commons.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/system/unicode.py` & `cereja-1.9.9/cereja/system/unicode.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/utils/__init__.py` & `cereja-1.9.9/cereja/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/utils/_utils.py` & `cereja-1.9.9/cereja/utils/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,30 +16,29 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 import ast
 import ctypes
 import gc
 import math
-import threading
 import time
 from collections import OrderedDict, defaultdict
 from importlib import import_module
 import importlib
 import sys
 import types
 import random
 from typing import Any, Union, List, Tuple, Sequence, Iterable, Dict, MappingView, Optional, Callable
 import logging
 import itertools
 from copy import copy
 import inspect
 from pprint import PrettyPrinter
 
-from .decorators import time_exec, depreciation
+from .decorators import depreciation
 # Needed init configs
 from ..config.cj_types import ClassType, FunctionType, Number
 from itertools import combinations as itertools_combinations
 
 __all__ = [
     "CjTest",
     "camel_to_snake",
@@ -81,15 +80,14 @@
     "group_by",
     "dict_values_len",
     "dict_max_value",
     "dict_min_value",
     "dict_filter_value",
     "get_zero_mask",
     "get_batch_strides",
-    "Thread",
     "prune_values",
     "split_sequence",
     "has_length",
     "combinations",
     "combinations_sizes",
     "value_from_memory"
 ]
@@ -110,36 +108,14 @@
                 super()._format(object, *args)
             finally:
                 self._width = width
         else:
             super()._format(object, *args)
 
 
-# TODO: Remove Thread class, check cereja.concurrently.process.MultiProcess implementation
-class Thread(threading.Thread):
-    def __init__(
-            self, target, args=None, kwargs=None, name=None, daemon=None, callback=None
-    ):
-        # while threading.active_count() > os.cpu_count() * 2:
-        #    time.sleep(0.1)
-        super().__init__(daemon=daemon, name=name)
-        if args is None:
-            args = ()
-        if kwargs is None:
-            kwargs = {}
-        self._func = target
-        self._args = args
-        self._kwargs = kwargs
-        self._callback = callback
-
-    def run(self):
-        res = self._func(*self._args, **self._kwargs)
-        if self._callback:
-            self._callback(res)
-
 
 def is_indexable(v):
     return hasattr(v, "__getitem__")
 
 
 def split_sequence(seq, is_break_fn):
     """
```

### Comparing `cereja-1.9.8/cereja/utils/colab.py` & `cereja-1.9.9/cereja/utils/colab.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/utils/decorators.py` & `cereja-1.9.9/cereja/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja/utils/version.py` & `cereja-1.9.9/cereja/utils/version.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/cereja.egg-info/PKG-INFO` & `cereja-1.9.9/cereja.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cereja
-Version: 1.9.8
+Version: 1.9.9
 Summary: Cereja is a bundle of useful functions that I don't want to rewrite.
 Author-email: Joab Leite <leitejoab@gmail.com>
 License: Copyright (c) 2019 The Cereja Project
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `cereja-1.9.8/cereja.egg-info/SOURCES.txt` & `cereja-1.9.9/cereja.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/pyproject.toml` & `cereja-1.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/tests/testhashtools.py` & `cereja-1.9.9/tests/testhashtools.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/tests/tests.py` & `cereja-1.9.9/tests/tests.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/tests/testsfiletools.py` & `cereja-1.9.9/tests/testsfiletools.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/tests/testsgeolinear.py` & `cereja-1.9.9/tests/testsgeolinear.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/tests/testsmltools.py` & `cereja-1.9.9/tests/testsmltools.py`

 * *Files identical despite different names*

### Comparing `cereja-1.9.8/tests/testsutils.py` & `cereja-1.9.9/tests/testsutils.py`

 * *Files identical despite different names*

