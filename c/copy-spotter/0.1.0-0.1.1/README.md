# Comparing `tmp/copy-spotter-0.1.0.tar.gz` & `tmp/copy-spotter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copy-spotter-0.1.0.tar", last modified: Sun Apr 21 09:49:29 2024, max compression
+gzip compressed data, was "copy-spotter-0.1.1.tar", last modified: Wed Apr 24 20:04:14 2024, max compression
```

## Comparing `copy-spotter-0.1.0.tar` & `copy-spotter-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:49:29.341783 copy-spotter-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-21 09:49:14.000000 copy-spotter-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-21 09:49:29.341783 copy-spotter-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-21 09:49:14.000000 copy-spotter-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:49:29.341783 copy-spotter-0.1.0/copy_spotter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-21 09:49:29.000000 copy-spotter-0.1.0/copy_spotter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-21 09:49:29.000000 copy-spotter-0.1.0/copy_spotter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 09:49:29.000000 copy-spotter-0.1.0/copy_spotter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-21 09:49:29.000000 copy-spotter-0.1.0/copy_spotter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 09:49:29.000000 copy-spotter-0.1.0/copy_spotter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 09:49:14.000000 copy-spotter-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:49:29.341783 copy-spotter-0.1.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 09:49:14.000000 copy-spotter-0.1.0/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-21 09:49:14.000000 copy-spotter-0.1.0/scripts/html_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-21 09:49:14.000000 copy-spotter-0.1.0/scripts/html_writing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-21 09:49:14.000000 copy-spotter-0.1.0/scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-21 09:49:14.000000 copy-spotter-0.1.0/scripts/processing_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-21 09:49:14.000000 copy-spotter-0.1.0/scripts/similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-21 09:49:14.000000 copy-spotter-0.1.0/scripts/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-21 09:49:29.341783 copy-spotter-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-21 09:49:14.000000 copy-spotter-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:49:29.341783 copy-spotter-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 09:49:14.000000 copy-spotter-0.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:49:29.341783 copy-spotter-0.1.0/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 09:49:14.000000 copy-spotter-0.1.0/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 09:49:14.000000 copy-spotter-0.1.0/tests/scripts/test_html_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 09:49:14.000000 copy-spotter-0.1.0/tests/scripts/test_html_writing.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 09:49:14.000000 copy-spotter-0.1.0/tests/scripts/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 09:49:14.000000 copy-spotter-0.1.0/tests/scripts/test_processing_files.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 09:49:14.000000 copy-spotter-0.1.0/tests/scripts/test_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-21 09:49:14.000000 copy-spotter-0.1.0/tests/scripts/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:04:14.825332 copy-spotter-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-24 20:03:53.000000 copy-spotter-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-24 20:04:14.825332 copy-spotter-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-24 20:03:53.000000 copy-spotter-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:04:14.825332 copy-spotter-0.1.1/copy_spotter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-24 20:04:14.000000 copy-spotter-0.1.1/copy_spotter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-24 20:04:14.000000 copy-spotter-0.1.1/copy_spotter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:04:14.000000 copy-spotter-0.1.1/copy_spotter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 20:04:14.000000 copy-spotter-0.1.1/copy_spotter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-24 20:04:14.000000 copy-spotter-0.1.1/copy_spotter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 20:04:14.000000 copy-spotter-0.1.1/copy_spotter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:03:53.000000 copy-spotter-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:04:14.825332 copy-spotter-0.1.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:03:53.000000 copy-spotter-0.1.1/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-24 20:03:53.000000 copy-spotter-0.1.1/scripts/html_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-24 20:03:53.000000 copy-spotter-0.1.1/scripts/html_writing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-24 20:03:53.000000 copy-spotter-0.1.1/scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-24 20:03:53.000000 copy-spotter-0.1.1/scripts/processing_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-24 20:03:53.000000 copy-spotter-0.1.1/scripts/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-24 20:03:53.000000 copy-spotter-0.1.1/scripts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-24 20:04:14.829331 copy-spotter-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-24 20:03:53.000000 copy-spotter-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:04:14.825332 copy-spotter-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:03:53.000000 copy-spotter-0.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:04:14.825332 copy-spotter-0.1.1/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:03:53.000000 copy-spotter-0.1.1/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:03:53.000000 copy-spotter-0.1.1/tests/scripts/test_html_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:03:53.000000 copy-spotter-0.1.1/tests/scripts/test_html_writing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:03:53.000000 copy-spotter-0.1.1/tests/scripts/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:03:53.000000 copy-spotter-0.1.1/tests/scripts/test_processing_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:03:53.000000 copy-spotter-0.1.1/tests/scripts/test_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-24 20:03:53.000000 copy-spotter-0.1.1/tests/scripts/test_utils.py
```

### Comparing `copy-spotter-0.1.0/LICENSE` & `copy-spotter-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.0/PKG-INFO` & `copy-spotter-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copy-spotter
-Version: 0.1.0
+Version: 0.1.1
 Summary: Make plagiarism detection easier. This package will find similar sentences between given files and highlight them in a side by side comparison.
 Home-page: https://github.com/Wazzabeee/copy-spotter
 Author: Clément Delteil
 Author-email: clement45.delteil45@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `copy-spotter-0.1.0/README.md` & `copy-spotter-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.0/copy_spotter.egg-info/PKG-INFO` & `copy-spotter-0.1.1/copy_spotter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copy-spotter
-Version: 0.1.0
+Version: 0.1.1
 Summary: Make plagiarism detection easier. This package will find similar sentences between given files and highlight them in a side by side comparison.
 Home-page: https://github.com/Wazzabeee/copy-spotter
 Author: Clément Delteil
 Author-email: clement45.delteil45@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `copy-spotter-0.1.0/copy_spotter.egg-info/SOURCES.txt` & `copy-spotter-0.1.1/copy_spotter.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 copy_spotter.egg-info/PKG-INFO
 copy_spotter.egg-info/SOURCES.txt
 copy_spotter.egg-info/dependency_links.txt
+copy_spotter.egg-info/entry_points.txt
 copy_spotter.egg-info/requires.txt
 copy_spotter.egg-info/top_level.txt
 scripts/__init__.py
 scripts/html_utils.py
 scripts/html_writing.py
 scripts/main.py
 scripts/processing_files.py
```

### Comparing `copy-spotter-0.1.0/scripts/html_utils.py` & `copy-spotter-0.1.1/scripts/html_utils.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.0/scripts/html_writing.py` & `copy-spotter-0.1.1/scripts/html_writing.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.0/scripts/main.py` & `copy-spotter-0.1.1/scripts/main.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.0/scripts/processing_files.py` & `copy-spotter-0.1.1/scripts/processing_files.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.0/scripts/similarity.py` & `copy-spotter-0.1.1/scripts/similarity.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.0/scripts/utils.py` & `copy-spotter-0.1.1/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.0/tests/scripts/test_utils.py` & `copy-spotter-0.1.1/tests/scripts/test_utils.py`

 * *Files identical despite different names*

