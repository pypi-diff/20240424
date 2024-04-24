# Comparing `tmp/cnspy_spatial_csv_formats-0.1.1.tar.gz` & `tmp/cnspy_spatial_csv_formats-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jungr/workspace/CNS/VIO_Evaluation_Framework/py3_pkgs/cnspy_eco_system_test/pkgs/b_spatial_csv_formats/dist/tmp_rc6felh/c", last modified: Sat Mar 20 14:23:25 2021, max compression
+gzip compressed data, was "cnspy_spatial_csv_formats-0.2.0.tar", last modified: Wed Apr 24 12:16:32 2024, max compression
```

## Comparing `cnspy_spatial_csv_formats-0.1.1.tar` & `cnspy_spatial_csv_formats-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:23:25.645449 cnspy_spatial_csv_formats-0.1.1/
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     3126 2021-03-20 14:23:25.645449 cnspy_spatial_csv_formats-0.1.1/PKG-INFO
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     2114 2021-03-20 14:21:27.000000 cnspy_spatial_csv_formats-0.1.1/README.md
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:23:25.645449 cnspy_spatial_csv_formats-0.1.1/cnspy_spatial_csv_formats/
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     4897 2021-03-20 12:20:48.000000 cnspy_spatial_csv_formats-0.1.1/cnspy_spatial_csv_formats/CSVFormatPose.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     3460 2021-03-20 12:20:48.000000 cnspy_spatial_csv_formats-0.1.1/cnspy_spatial_csv_formats/PoseStructs.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 12:20:48.000000 cnspy_spatial_csv_formats-0.1.1/cnspy_spatial_csv_formats/__init__.py
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:23:25.645449 cnspy_spatial_csv_formats-0.1.1/cnspy_spatial_csv_formats.egg-info/
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     3126 2021-03-20 14:23:25.000000 cnspy_spatial_csv_formats-0.1.1/cnspy_spatial_csv_formats.egg-info/PKG-INFO
--rw-rw-r--   0 jungr     (1000) jungr     (1000)      428 2021-03-20 14:23:25.000000 cnspy_spatial_csv_formats-0.1.1/cnspy_spatial_csv_formats.egg-info/SOURCES.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)        1 2021-03-20 14:23:25.000000 cnspy_spatial_csv_formats-0.1.1/cnspy_spatial_csv_formats.egg-info/dependency_links.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)        6 2021-03-20 14:23:25.000000 cnspy_spatial_csv_formats-0.1.1/cnspy_spatial_csv_formats.egg-info/requires.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)       31 2021-03-20 14:23:25.000000 cnspy_spatial_csv_formats-0.1.1/cnspy_spatial_csv_formats.egg-info/top_level.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)       38 2021-03-20 14:23:25.645449 cnspy_spatial_csv_formats-0.1.1/setup.cfg
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     1257 2021-03-20 14:21:27.000000 cnspy_spatial_csv_formats-0.1.1/setup.py
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:23:25.645449 cnspy_spatial_csv_formats-0.1.1/test/
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 12:20:48.000000 cnspy_spatial_csv_formats-0.1.1/test/__init__.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     2641 2021-03-20 12:20:48.000000 cnspy_spatial_csv_formats-0.1.1/test/test_CSVFormatPose.py
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:16:32.329202 cnspy_spatial_csv_formats-0.2.0/
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)    35149 2022-05-30 14:10:28.000000 cnspy_spatial_csv_formats-0.2.0/LICENCE
+-rw-r--r--   0 jungr     (1000) jungr     (1000)     4489 2024-04-24 12:16:32.329202 cnspy_spatial_csv_formats-0.2.0/PKG-INFO
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     3810 2024-04-24 11:44:10.000000 cnspy_spatial_csv_formats-0.2.0/README.md
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:16:32.329202 cnspy_spatial_csv_formats-0.2.0/cnspy_spatial_csv_formats/
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     2296 2024-04-24 11:44:10.000000 cnspy_spatial_csv_formats-0.2.0/cnspy_spatial_csv_formats/CSVSpatialFormat.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)     9288 2024-04-24 11:44:10.000000 cnspy_spatial_csv_formats-0.2.0/cnspy_spatial_csv_formats/CSVSpatialFormatType.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     2268 2024-04-24 11:44:10.000000 cnspy_spatial_csv_formats-0.2.0/cnspy_spatial_csv_formats/ErrorRepresentationType.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     3165 2024-04-24 11:44:10.000000 cnspy_spatial_csv_formats-0.2.0/cnspy_spatial_csv_formats/EstimationErrorType.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     6228 2024-04-24 11:44:10.000000 cnspy_spatial_csv_formats-0.2.0/cnspy_spatial_csv_formats/PoseStructs.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2022-05-30 14:10:28.000000 cnspy_spatial_csv_formats-0.2.0/cnspy_spatial_csv_formats/__init__.py
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:16:32.329202 cnspy_spatial_csv_formats-0.2.0/cnspy_spatial_csv_formats.egg-info/
+-rw-r--r--   0 jungr     (1000) jungr     (1000)     4489 2024-04-24 12:16:32.000000 cnspy_spatial_csv_formats-0.2.0/cnspy_spatial_csv_formats.egg-info/PKG-INFO
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)      631 2024-04-24 12:16:32.000000 cnspy_spatial_csv_formats-0.2.0/cnspy_spatial_csv_formats.egg-info/SOURCES.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)        1 2024-04-24 12:16:32.000000 cnspy_spatial_csv_formats-0.2.0/cnspy_spatial_csv_formats.egg-info/dependency_links.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)        6 2024-04-24 12:16:32.000000 cnspy_spatial_csv_formats-0.2.0/cnspy_spatial_csv_formats.egg-info/requires.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)       31 2024-04-24 12:16:32.000000 cnspy_spatial_csv_formats-0.2.0/cnspy_spatial_csv_formats.egg-info/top_level.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)       38 2024-04-24 12:16:32.329202 cnspy_spatial_csv_formats-0.2.0/setup.cfg
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     1257 2022-05-30 14:10:28.000000 cnspy_spatial_csv_formats-0.2.0/setup.py
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:16:32.329202 cnspy_spatial_csv_formats-0.2.0/test/
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2022-05-30 14:10:28.000000 cnspy_spatial_csv_formats-0.2.0/test/__init__.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     4988 2024-04-24 11:44:10.000000 cnspy_spatial_csv_formats-0.2.0/test/test_CSVSpatialFormatType.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     1443 2024-04-24 11:44:10.000000 cnspy_spatial_csv_formats-0.2.0/test/test_EstimationErrorType.py
```

### Comparing `cnspy_spatial_csv_formats-0.1.1/setup.py` & `cnspy_spatial_csv_formats-0.2.0/setup.py`

 * *Files identical despite different names*

