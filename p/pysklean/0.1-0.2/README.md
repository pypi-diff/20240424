# Comparing `tmp/pysklean-0.1.tar.gz` & `tmp/pysklean-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysklean-0.1.tar", last modified: Wed Apr 24 15:55:03 2024, max compression
+gzip compressed data, was "pysklean-0.2.tar", last modified: Wed Apr 24 16:00:49 2024, max compression
```

## Comparing `pysklean-0.1.tar` & `pysklean-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 15:55:03.431440 pysklean-0.1/
--rw-rw-rw-   0        0        0      113 2024-04-24 15:55:03.430439 pysklean-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 15:55:03.333046 pysklean-0.1/py_viking/
--rw-rw-rw-   0        0        0       46 2024-04-24 15:52:27.000000 pysklean-0.1/py_viking/__init__.py
--rw-rw-rw-   0        0        0    27139 2024-04-24 15:52:38.000000 pysklean-0.1/py_viking/main.py
-drwxrwxrwx   0        0        0        0 2024-04-24 15:55:03.421890 pysklean-0.1/pysklean.egg-info/
--rw-rw-rw-   0        0        0      113 2024-04-24 15:55:02.000000 pysklean-0.1/pysklean.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2024-04-24 15:55:02.000000 pysklean-0.1/pysklean.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 15:55:02.000000 pysklean-0.1/pysklean.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-24 15:55:02.000000 pysklean-0.1/pysklean.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 15:55:03.432445 pysklean-0.1/setup.cfg
--rw-rw-rw-   0        0        0      225 2024-04-24 15:53:45.000000 pysklean-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:00:49.627369 pysklean-0.2/
+-rw-rw-rw-   0        0        0      113 2024-04-24 16:00:49.626366 pysklean-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 16:00:49.577959 pysklean-0.2/py_viking/
+-rw-rw-rw-   0        0        0       46 2024-04-24 15:52:27.000000 pysklean-0.2/py_viking/__init__.py
+-rw-rw-rw-   0        0        0    27125 2024-04-24 16:00:41.000000 pysklean-0.2/py_viking/main.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:00:49.617352 pysklean-0.2/pysklean.egg-info/
+-rw-rw-rw-   0        0        0      113 2024-04-24 16:00:48.000000 pysklean-0.2/pysklean.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2024-04-24 16:00:49.000000 pysklean-0.2/pysklean.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 16:00:48.000000 pysklean-0.2/pysklean.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-24 16:00:48.000000 pysklean-0.2/pysklean.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 16:00:49.628366 pysklean-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      225 2024-04-24 16:00:38.000000 pysklean-0.2/setup.py
```

### Comparing `pysklean-0.1/py_viking/main.py` & `pysklean-0.2/py_viking/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-def update_graph():
-    names = input()
+def update_graph(names):
+
     if(names == 'mlp'):
         print(
             '''
     from math import exp 
 from random import seed 
 from random import random
```

