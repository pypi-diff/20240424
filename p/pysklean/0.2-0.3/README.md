# Comparing `tmp/pysklean-0.2.tar.gz` & `tmp/pysklean-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysklean-0.2.tar", last modified: Wed Apr 24 16:00:49 2024, max compression
+gzip compressed data, was "pysklean-0.3.tar", last modified: Wed Apr 24 16:06:01 2024, max compression
```

## Comparing `pysklean-0.2.tar` & `pysklean-0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 16:00:49.627369 pysklean-0.2/
--rw-rw-rw-   0        0        0      113 2024-04-24 16:00:49.626366 pysklean-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 16:00:49.577959 pysklean-0.2/py_viking/
--rw-rw-rw-   0        0        0       46 2024-04-24 15:52:27.000000 pysklean-0.2/py_viking/__init__.py
--rw-rw-rw-   0        0        0    27125 2024-04-24 16:00:41.000000 pysklean-0.2/py_viking/main.py
-drwxrwxrwx   0        0        0        0 2024-04-24 16:00:49.617352 pysklean-0.2/pysklean.egg-info/
--rw-rw-rw-   0        0        0      113 2024-04-24 16:00:48.000000 pysklean-0.2/pysklean.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2024-04-24 16:00:49.000000 pysklean-0.2/pysklean.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 16:00:48.000000 pysklean-0.2/pysklean.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-24 16:00:48.000000 pysklean-0.2/pysklean.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 16:00:49.628366 pysklean-0.2/setup.cfg
--rw-rw-rw-   0        0        0      225 2024-04-24 16:00:38.000000 pysklean-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:06:01.624848 pysklean-0.3/
+-rw-rw-rw-   0        0        0      113 2024-04-24 16:06:01.620847 pysklean-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 16:06:01.543276 pysklean-0.3/pysklean/
+-rw-rw-rw-   0        0        0       46 2024-04-24 15:52:27.000000 pysklean-0.3/pysklean/__init__.py
+-rw-rw-rw-   0        0        0    27125 2024-04-24 16:00:41.000000 pysklean-0.3/pysklean/main.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:06:01.613828 pysklean-0.3/pysklean.egg-info/
+-rw-rw-rw-   0        0        0      113 2024-04-24 16:06:01.000000 pysklean-0.3/pysklean.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2024-04-24 16:06:01.000000 pysklean-0.3/pysklean.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 16:06:01.000000 pysklean-0.3/pysklean.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-24 16:06:01.000000 pysklean-0.3/pysklean.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 16:06:01.625847 pysklean-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      225 2024-04-24 16:05:56.000000 pysklean-0.3/setup.py
```

### Comparing `pysklean-0.2/py_viking/main.py` & `pysklean-0.3/pysklean/main.py`

 * *Files identical despite different names*

