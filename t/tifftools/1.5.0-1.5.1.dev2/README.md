# Comparing `tmp/tifftools-1.5.0.tar.gz` & `tmp/tifftools-1.5.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tifftools-1.5.0.tar", last modified: Tue Apr 23 12:29:46 2024, max compression
+gzip compressed data, was "tifftools-1.5.1.dev2.tar", last modified: Wed Apr 24 19:10:27 2024, max compression
```

## Comparing `tifftools-1.5.0.tar` & `tifftools-1.5.1.dev2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:29:46.285854 tifftools-1.5.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:29:46.277854 tifftools-1.5.0/.circleci/
--rw-r--r--   0 root         (0) root         (0)     4029 2024-04-23 12:29:22.000000 tifftools-1.5.0/.circleci/config.yml
--rw-r--r--   0 root         (0) root         (0)      303 2024-04-23 12:29:22.000000 tifftools-1.5.0/.editorconfig
--rw-r--r--   0 root         (0) root         (0)      596 2024-04-23 12:29:22.000000 tifftools-1.5.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1633 2024-04-23 12:29:22.000000 tifftools-1.5.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     3672 2024-04-23 12:29:22.000000 tifftools-1.5.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)      549 2024-04-23 12:29:22.000000 tifftools-1.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      148 2024-04-23 12:29:22.000000 tifftools-1.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8825 2024-04-23 12:29:46.281854 tifftools-1.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7969 2024-04-23 12:29:22.000000 tifftools-1.5.0/README.rst
--rw-r--r--   0 root         (0) root         (0)      424 2024-04-23 12:29:22.000000 tifftools-1.5.0/codecov.yml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 12:29:46.285854 tifftools-1.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1958 2024-04-23 12:29:22.000000 tifftools-1.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:29:46.277854 tifftools-1.5.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:29:46.281854 tifftools-1.5.0/tests/data/
--rw-r--r--   0 root         (0) root         (0)      630 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/data/bad_datatype.tif
--rw-r--r--   0 root         (0) root         (0)     1261 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/data/bad_double_reference.tif
--rw-r--r--   0 root         (0) root         (0)      653 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/data/bad_header1.tif
--rw-r--r--   0 root         (0) root         (0)      815 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/data/bad_header2.tif
--rw-r--r--   0 root         (0) root         (0)      453 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/data/bad_ifd_offset.tif
--rw-r--r--   0 root         (0) root         (0)      360 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/data/bad_jpeg.tif
--rw-r--r--   0 root         (0) root         (0)      616 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/data/bad_jpeg2.tif
--rw-r--r--   0 root         (0) root         (0)      453 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/data/bad_strip_offset.tif
--rw-r--r--   0 root         (0) root         (0)     1261 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/data/bad_subifd_offset.tif
--rw-r--r--   0 root         (0) root         (0)      653 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/data/bad_tag_offset.tif
--rw-r--r--   0 root         (0) root         (0)      641 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/data/bad_unicode.tif
--rw-r--r--   0 root         (0) root         (0)      616 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/data/good_jpeg.tif
--rw-r--r--   0 root         (0) root         (0)      453 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/data/good_single.tif
--rw-r--r--   0 root         (0) root         (0)     2114 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/datastore.py
--rw-r--r--   0 root         (0) root         (0)     3059 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/test_constants.py
--rw-r--r--   0 root         (0) root         (0)     4616 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/test_dump.py
--rw-r--r--   0 root         (0) root         (0)     2608 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/test_main.py
--rw-r--r--   0 root         (0) root         (0)      848 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/test_options.py
--rw-r--r--   0 root         (0) root         (0)     1603 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/test_path_or_fobj.py
--rw-r--r--   0 root         (0) root         (0)     1943 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/test_read_tiff.py
--rw-r--r--   0 root         (0) root         (0)      687 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/test_readme.py
--rw-r--r--   0 root         (0) root         (0)     5557 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/test_set.py
--rw-r--r--   0 root         (0) root         (0)     3992 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/test_split.py
--rw-r--r--   0 root         (0) root         (0)     9822 2024-04-23 12:29:22.000000 tifftools-1.5.0/tests/test_write_tiff.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:29:46.281854 tifftools-1.5.0/tifftools/
--rw-r--r--   0 root         (0) root         (0)     1049 2024-04-23 12:29:22.000000 tifftools-1.5.0/tifftools/__init__.py
--rw-r--r--   0 root         (0) root         (0)       94 2024-04-23 12:29:22.000000 tifftools-1.5.0/tifftools/__main__.py
--rw-r--r--   0 root         (0) root         (0)    31419 2024-04-23 12:29:22.000000 tifftools-1.5.0/tifftools/commands.py
--rw-r--r--   0 root         (0) root         (0)    67608 2024-04-23 12:29:22.000000 tifftools-1.5.0/tifftools/constants.py
--rw-r--r--   0 root         (0) root         (0)      265 2024-04-23 12:29:22.000000 tifftools-1.5.0/tifftools/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2062 2024-04-23 12:29:22.000000 tifftools-1.5.0/tifftools/path_or_fobj.py
--rwxr-xr-x   0 root         (0) root         (0)    33259 2024-04-23 12:29:22.000000 tifftools-1.5.0/tifftools/tifftools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:29:46.281854 tifftools-1.5.0/tifftools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8825 2024-04-23 12:29:46.000000 tifftools-1.5.0/tifftools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1131 2024-04-23 12:29:46.000000 tifftools-1.5.0/tifftools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 12:29:46.000000 tifftools-1.5.0/tifftools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-04-23 12:29:46.000000 tifftools-1.5.0/tifftools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 12:29:38.000000 tifftools-1.5.0/tifftools.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-23 12:29:46.000000 tifftools-1.5.0/tifftools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1595 2024-04-23 12:29:22.000000 tifftools-1.5.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:10:27.748515 tifftools-1.5.1.dev2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:10:27.740515 tifftools-1.5.1.dev2/.circleci/
+-rw-r--r--   0 root         (0) root         (0)     4029 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/.circleci/config.yml
+-rw-r--r--   0 root         (0) root         (0)      303 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/.editorconfig
+-rw-r--r--   0 root         (0) root         (0)      596 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1633 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     3764 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)      549 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      148 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8830 2024-04-24 19:10:27.748515 tifftools-1.5.1.dev2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7969 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/README.rst
+-rw-r--r--   0 root         (0) root         (0)      424 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/codecov.yml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 19:10:27.748515 tifftools-1.5.1.dev2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1958 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:10:27.744515 tifftools-1.5.1.dev2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:10:27.744515 tifftools-1.5.1.dev2/tests/data/
+-rw-r--r--   0 root         (0) root         (0)      630 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/bad_datatype.tif
+-rw-r--r--   0 root         (0) root         (0)     1261 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/bad_double_reference.tif
+-rw-r--r--   0 root         (0) root         (0)      653 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/bad_header1.tif
+-rw-r--r--   0 root         (0) root         (0)      815 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/bad_header2.tif
+-rw-r--r--   0 root         (0) root         (0)      453 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/bad_ifd_offset.tif
+-rw-r--r--   0 root         (0) root         (0)      360 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/bad_jpeg.tif
+-rw-r--r--   0 root         (0) root         (0)      616 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/bad_jpeg2.tif
+-rw-r--r--   0 root         (0) root         (0)      453 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/bad_strip_offset.tif
+-rw-r--r--   0 root         (0) root         (0)     1261 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/bad_subifd_offset.tif
+-rw-r--r--   0 root         (0) root         (0)      653 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/bad_tag_offset.tif
+-rw-r--r--   0 root         (0) root         (0)      641 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/bad_unicode.tif
+-rw-r--r--   0 root         (0) root         (0)      616 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/good_jpeg.tif
+-rw-r--r--   0 root         (0) root         (0)      453 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/good_single.tif
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/datastore.py
+-rw-r--r--   0 root         (0) root         (0)     3059 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/test_constants.py
+-rw-r--r--   0 root         (0) root         (0)     4616 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/test_dump.py
+-rw-r--r--   0 root         (0) root         (0)     2608 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/test_main.py
+-rw-r--r--   0 root         (0) root         (0)      848 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/test_options.py
+-rw-r--r--   0 root         (0) root         (0)     1603 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/test_path_or_fobj.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/test_read_tiff.py
+-rw-r--r--   0 root         (0) root         (0)      687 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/test_readme.py
+-rw-r--r--   0 root         (0) root         (0)     5557 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/test_set.py
+-rw-r--r--   0 root         (0) root         (0)     3992 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/test_split.py
+-rw-r--r--   0 root         (0) root         (0)     9822 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/test_write_tiff.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:10:27.744515 tifftools-1.5.1.dev2/tifftools/
+-rw-r--r--   0 root         (0) root         (0)     1049 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tifftools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       94 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tifftools/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    31419 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tifftools/commands.py
+-rw-r--r--   0 root         (0) root         (0)    67608 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tifftools/constants.py
+-rw-r--r--   0 root         (0) root         (0)      265 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tifftools/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tifftools/path_or_fobj.py
+-rwxr-xr-x   0 root         (0) root         (0)    33650 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tifftools/tifftools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:10:27.744515 tifftools-1.5.1.dev2/tifftools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8830 2024-04-24 19:10:27.000000 tifftools-1.5.1.dev2/tifftools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-24 19:10:27.000000 tifftools-1.5.1.dev2/tifftools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 19:10:27.000000 tifftools-1.5.1.dev2/tifftools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-04-24 19:10:27.000000 tifftools-1.5.1.dev2/tifftools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 19:10:22.000000 tifftools-1.5.1.dev2/tifftools.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-24 19:10:27.000000 tifftools-1.5.1.dev2/tifftools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1595 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tox.ini
```

### Comparing `tifftools-1.5.0/.circleci/config.yml` & `tifftools-1.5.1.dev2/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/.gitignore` & `tifftools-1.5.1.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/.pre-commit-config.yaml` & `tifftools-1.5.1.dev2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/CHANGELOG.md` & `tifftools-1.5.1.dev2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Change Log
 
+## Version 1.5.1
+
+### Improvements
+- Speed up deduplication process ([#93](../../pull/93))
+
 ## Version 1.5.0
 
 ### Features
 - Add a deduplicate option to avoid writing all identical data blocks ([#92](../../pull/92))
 
 ### Improvements
 - Refactor how ifds-first option emits data so it is closer to the COGs standard ([#92](../../pull/92))
```

### Comparing `tifftools-1.5.0/LICENSE` & `tifftools-1.5.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/PKG-INFO` & `tifftools-1.5.1.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tifftools
-Version: 1.5.0
+Version: 1.5.1.dev2
 Summary: Pure python tiff tools to handle all tags and IFDs.
 Home-page: https://github.com/DigitalSlideArchive/tifftools
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: tiff
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tifftools-1.5.0/README.rst` & `tifftools-1.5.1.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/setup.py` & `tifftools-1.5.1.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tests/data/bad_datatype.tif` & `tifftools-1.5.1.dev2/tests/data/bad_datatype.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tests/data/bad_double_reference.tif` & `tifftools-1.5.1.dev2/tests/data/bad_double_reference.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tests/data/bad_header1.tif` & `tifftools-1.5.1.dev2/tests/data/bad_header1.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tests/data/bad_header2.tif` & `tifftools-1.5.1.dev2/tests/data/bad_header2.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tests/data/bad_jpeg2.tif` & `tifftools-1.5.1.dev2/tests/data/bad_jpeg2.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tests/data/bad_subifd_offset.tif` & `tifftools-1.5.1.dev2/tests/data/bad_subifd_offset.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tests/data/bad_tag_offset.tif` & `tifftools-1.5.1.dev2/tests/data/bad_tag_offset.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tests/data/bad_unicode.tif` & `tifftools-1.5.1.dev2/tests/data/bad_unicode.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tests/data/good_jpeg.tif` & `tifftools-1.5.1.dev2/tests/data/good_jpeg.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tests/datastore.py` & `tifftools-1.5.1.dev2/tests/datastore.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tests/test_constants.py` & `tifftools-1.5.1.dev2/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tests/test_dump.py` & `tifftools-1.5.1.dev2/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tests/test_main.py` & `tifftools-1.5.1.dev2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tests/test_options.py` & `tifftools-1.5.1.dev2/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tests/test_path_or_fobj.py` & `tifftools-1.5.1.dev2/tests/test_path_or_fobj.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tests/test_read_tiff.py` & `tifftools-1.5.1.dev2/tests/test_read_tiff.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tests/test_readme.py` & `tifftools-1.5.1.dev2/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tests/test_set.py` & `tifftools-1.5.1.dev2/tests/test_set.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tests/test_split.py` & `tifftools-1.5.1.dev2/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tests/test_write_tiff.py` & `tifftools-1.5.1.dev2/tests/test_write_tiff.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tifftools/__init__.py` & `tifftools-1.5.1.dev2/tifftools/__init__.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tifftools/commands.py` & `tifftools-1.5.1.dev2/tifftools/commands.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tifftools/constants.py` & `tifftools-1.5.1.dev2/tifftools/constants.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tifftools/path_or_fobj.py` & `tifftools-1.5.1.dev2/tifftools/path_or_fobj.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tifftools/tifftools.py` & `tifftools-1.5.1.dev2/tifftools/tifftools.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from .constants import Datatype, Tag, get_or_create_tag
 from .exceptions import MustBeBigTiffError, TifftoolsError
 from .path_or_fobj import OpenPathOrFobj, is_filelike_object
 
 logger = logging.getLogger(__name__)
 
-_DEDUP_HASH_METHOD = 'sha256'
+_DEDUP_HASH_METHOD = 'sha1'
 
 
 def check_offset(filelen, offset, length):
     """
     Check if a specific number of bytes can be read from a file at a given
     offset.
 
@@ -320,47 +320,47 @@
     finalpath = path
     if not is_filelike_object(path) and os.path.exists(path):
         if not allowExisting:
             raise TifftoolsError('File already exists')
         with tempfile.NamedTemporaryFile(
                 prefix=os.path.basename(path), dir=os.path.dirname(path)) as temppath:
             path = temppath.name
-    rewriteBigtiff = False
     try:
         with OpenPathOrFobj(path, 'wb') as dest:
             bom = '>' if bigEndian else '<'
             header = b'II' if not bigEndian else b'MM'
             if bigtiff:
                 header += struct.pack(bom + 'HHHQ', 0x2B, 8, 0, 0)
                 ifdPtr = len(header) - 8
             else:
                 header += struct.pack(bom + 'HL', 0x2A, 0)
                 ifdPtr = len(header) - 4
             dest.write(header)
             origifdPtr = ifdPtr
-            for datadest, ifddest in _ifdsPass(ifdsFirst, dest):
-                ifdPtr = origifdPtr
-                if bool(dedup):
-                    dedup = {'hashes': {}, 'reused': 0}
-                for ifd in ifds:
-                    try:
+            try:
+                for datadest, ifddest in _ifdsPass(ifdsFirst, dest):
+                    ifdPtr = origifdPtr
+                    if bool(dedup):
+                        dedup = {
+                            'hashes': {}, 'reused': 0,
+                            'hashlog': {} if not isinstance(dedup, dict) else
+                            dedup.get('hashlog', {})}
+                    for ifd in ifds:
                         ifdPtr = write_ifd(
                             datadest, ifddest, bom, bigtiff, ifd, ifdPtr,
                             ifdsFirst=ifdsFirst, dedup=dedup)
-                    except MustBeBigTiffError:
-                        # This can only be raised if bigtiff is false
-                        rewriteBigtiff = True
-                        break
-            if rewriteBigtiff:
+            except MustBeBigTiffError:
+                # This can only be raised if bigtiff is false
                 dest.seek(0)
                 dest.truncate(0)
                 write_tiff(ifds, dest, bigEndian, True, ifdsFirst=ifdsFirst, dedup=bool(dedup))
-            elif dedup and dedup['reused']:
-                logger.info('Deduplication reused %d block(s)', dedup['reused'])
-    except Exception:
+            else:
+                if dedup and dedup['reused']:
+                    logger.info('Deduplication reused %d block(s)', dedup['reused'])
+    except BaseException:
         if path != finalpath:
             os.unlink(path)
         raise
     else:
         if path != finalpath:
             # By copying the tempfile to the existing destination, the target
             # path keeps its inode
@@ -489,15 +489,15 @@
             opos = dest.tell()
             dest.seek(ddata['offset'])
             dest.write(data)
             dest.seek(opos)
     return ifdrecord
 
 
-def write_ifd(datadest, ifddest, bom, bigtiff, ifd, ifdPtr, tagSet=Tag,
+def write_ifd(datadest, ifddest, bom, bigtiff, ifd, ifdPtr, tagSet=Tag,  # noqa
               ifdsFirst=False, dedup=False):
     """
     Write an IFD to a TIFF file.  This copies image data from other tiff files.
 
     :param datadest: the open file handle to write offset data.
     :param ifddest: the open file handle to write ids and tag data.
     :param bom: either '<' or '>' for using struct to encode values based on
@@ -515,17 +515,14 @@
         hashed data that have been written and values of the offsets where it
         was written, and 'reused' is a count of data blocks that were
         deduplicated.
     :return: the ifdPtr for the next ifd that could be written.
     """
     ptrpack = 'Q' if bigtiff else 'L'
     tagdatalen = 8 if bigtiff else 4
-    # dest.seek(0, os.SEEK_END)
-    # origPos = dest.tell()
-    # origdest = ifddest = dest
     nextifdPtr = None
     ifdrecord = struct.pack(bom + ('Q' if bigtiff else 'H'), len(ifd['tags']))
     subifdPtrs = {}
     deferredData = {}
     ifdpos = ifddest.tell()
     if ifdsFirst:
         ifdlen = (
@@ -594,15 +591,20 @@
                 if ifddest.tell() % 2:
                     ifddest.write(b'\x00')
                 h = None
                 tpos = ifddest.tell()
                 if tag.isIFD() or taginfo.get('datatype') in (Datatype.IFD, Datatype.IFD8):
                     subifdPtrs[tag] = tpos
                 elif dedup:
-                    h = hashlib.new(_DEDUP_HASH_METHOD, data).digest()
+                    hashkey = hash(data)
+                    if hashkey in dedup['hashlog']:
+                        h = dedup['hashlog'][hashkey]
+                    else:
+                        h = hashlib.new(_DEDUP_HASH_METHOD, data).digest()
+                        dedup['hashlog'][hashkey] = h
                     if h in dedup['hashes']:
                         tpos = dedup['hashes'][h]
                     else:
                         dedup['hashes'][h] = tpos
                         h = None
                 _checkDataForNonBigtiff(bigtiff, [tpos])
                 tagrecord += struct.pack(bom + ptrpack, tpos)
@@ -724,27 +726,31 @@
                                 lengths[offsetList[olidx + 1][1]])):
                 destOffsets[offsetList[olidx + 1][1]] = destOffsets[idx] + lengths[idx]
                 tells['idx'].append(offsetList[olidx + 1][1])
                 olidx += 1
                 offset, idx = offsetList[olidx]
                 length += lengths[idx]
             if dedup:
-                readlen = length
-                h = hashlib.new(_DEDUP_HASH_METHOD)
-                while readlen:
-                    data = src.read(min(readlen, COPY_CHUNKSIZE))
-                    h.update(data)
-                    readlen -= len(data)
-                h = h.digest()
+                hashkey = (hash(getattr(src, 'name', src)), offset)
+                if hashkey in dedup['hashlog']:
+                    h = dedup['hashlog'][hashkey]
+                else:
+                    readlen = length
+                    h = hashlib.new(_DEDUP_HASH_METHOD)
+                    while readlen:
+                        data = src.read(min(readlen, COPY_CHUNKSIZE))
+                        h.update(data)
+                        readlen -= len(data)
+                    h = h.digest()
+                    dedup['hashlog'][hashkey] = h
                 if h in dedup['hashes']:
                     hpos = dedup['hashes'][h]
                     for tidx in tells['idx']:
                         destOffsets[tidx] = destOffsets[tidx] - tells['pos'] + hpos
                     dedup['reused'] += 1
-                    logger.debug('Deduplication: %d', dedup['reused'])
                     length = 0
                 else:
                     dedup['hashes'][h] = tells['pos']
                     src.seek(tells['offset'])
             while length:
                 data = src.read(min(length, COPY_CHUNKSIZE))
                 dest.write(data)
```

### Comparing `tifftools-1.5.0/tifftools.egg-info/PKG-INFO` & `tifftools-1.5.1.dev2/tifftools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tifftools
-Version: 1.5.0
+Version: 1.5.1.dev2
 Summary: Pure python tiff tools to handle all tags and IFDs.
 Home-page: https://github.com/DigitalSlideArchive/tifftools
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: tiff
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tifftools-1.5.0/tifftools.egg-info/SOURCES.txt` & `tifftools-1.5.1.dev2/tifftools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.0/tox.ini` & `tifftools-1.5.1.dev2/tox.ini`

 * *Files identical despite different names*

