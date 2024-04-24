# Comparing `tmp/alida-dataset-0.0.1.tar.gz` & `tmp/alida-dataset-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alida-dataset-0.0.1.tar", last modified: Wed Apr 24 12:26:16 2024, max compression
+gzip compressed data, was "dist/alida-dataset-0.0.2.tar", last modified: Wed Apr 24 13:00:13 2024, max compression
```

## Comparing `alida-dataset-0.0.1.tar` & `alida-dataset-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:26:16.434667 alida-dataset-0.0.1/
--rw-r--r--   0 root         (0) root         (0)      430 2024-04-24 12:26:16.434667 alida-dataset-0.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 12:26:06.000000 alida-dataset-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:26:16.434667 alida-dataset-0.0.1/alida_dataset.egg-info/
--rw-r--r--   0 root         (0) root         (0)      430 2024-04-24 12:26:16.000000 alida-dataset-0.0.1/alida_dataset.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      283 2024-04-24 12:26:16.000000 alida-dataset-0.0.1/alida_dataset.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 12:26:16.000000 alida-dataset-0.0.1/alida_dataset.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2024-04-24 12:26:16.000000 alida-dataset-0.0.1/alida_dataset.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-24 12:26:16.000000 alida-dataset-0.0.1/alida_dataset.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:26:16.434667 alida-dataset-0.0.1/alidadataset/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 12:26:06.000000 alida-dataset-0.0.1/alidadataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      337 2024-04-24 12:26:06.000000 alida-dataset-0.0.1/alidadataset/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2024-04-24 12:26:06.000000 alida-dataset-0.0.1/alidadataset/utils.py
--rw-rw-rw-   0 root         (0) root         (0)       79 2024-04-24 12:26:16.434667 alida-dataset-0.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      667 2024-04-24 12:26:06.000000 alida-dataset-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:00:13.426275 alida-dataset-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)      430 2024-04-24 13:00:13.426275 alida-dataset-0.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 13:00:03.000000 alida-dataset-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:00:13.426275 alida-dataset-0.0.2/alida_dataset.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      430 2024-04-24 13:00:13.000000 alida-dataset-0.0.2/alida_dataset.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      459 2024-04-24 13:00:13.000000 alida-dataset-0.0.2/alida_dataset.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 13:00:13.000000 alida-dataset-0.0.2/alida_dataset.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-24 13:00:13.000000 alida-dataset-0.0.2/alida_dataset.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-24 13:00:13.000000 alida-dataset-0.0.2/alida_dataset.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:00:13.426275 alida-dataset-0.0.2/alidadataset/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 13:00:03.000000 alida-dataset-0.0.2/alidadataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      337 2024-04-24 13:00:03.000000 alida-dataset-0.0.2/alidadataset/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:00:13.426275 alida-dataset-0.0.2/alidadataset/serializations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 13:00:03.000000 alida-dataset-0.0.2/alidadataset/serializations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1352 2024-04-24 13:00:03.000000 alida-dataset-0.0.2/alidadataset/serializations/hugging_face_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)      770 2024-04-24 13:00:03.000000 alida-dataset-0.0.2/alidadataset/serializations/pandas_dataframe.py
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-04-24 13:00:03.000000 alida-dataset-0.0.2/alidadataset/serializations/path.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2024-04-24 13:00:03.000000 alida-dataset-0.0.2/alidadataset/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       79 2024-04-24 13:00:13.427275 alida-dataset-0.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      667 2024-04-24 13:00:03.000000 alida-dataset-0.0.2/setup.py
```

### Comparing `alida-dataset-0.0.1/alidadataset/utils.py` & `alida-dataset-0.0.2/alidadataset/utils.py`

 * *Files identical despite different names*

### Comparing `alida-dataset-0.0.1/setup.py` & `alida-dataset-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="alida-dataset",
-    version="0.0.1",
+    version="0.0.2",
     author="Alida research team",
     author_email="engineering-alida-lab@eng.it",
     description="Utils for loading datasets using alida services.",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

