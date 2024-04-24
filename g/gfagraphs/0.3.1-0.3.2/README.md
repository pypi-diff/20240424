# Comparing `tmp/gfagraphs-0.3.1.tar.gz` & `tmp/gfagraphs-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfagraphs-0.3.1.tar", last modified: Tue Apr 23 16:25:03 2024, max compression
+gzip compressed data, was "gfagraphs-0.3.2.tar", last modified: Wed Apr 24 08:12:17 2024, max compression
```

## Comparing `gfagraphs-0.3.1.tar` & `gfagraphs-0.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-23 16:25:03.309799 gfagraphs-0.3.1/
--rw-r--r--   0 sidubois (669136) genscale (35005)    34521 2023-11-29 09:58:07.000000 gfagraphs-0.3.1/LICENSE
--rw-r--r--   0 sidubois (669136) genscale (35005)     2114 2024-04-23 16:25:03.308799 gfagraphs-0.3.1/PKG-INFO
--rw-r--r--   0 sidubois (669136) genscale (35005)     1491 2024-04-19 14:44:53.000000 gfagraphs-0.3.1/README.md
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-23 16:25:03.308799 gfagraphs-0.3.1/gfagraphs/
--rw-r--r--   0 sidubois (669136) genscale (35005)       58 2024-04-19 08:22:28.000000 gfagraphs-0.3.1/gfagraphs/__init__.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    39616 2024-03-07 16:32:34.000000 gfagraphs-0.3.1/gfagraphs/gfagraphs.py
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-23 16:25:03.308799 gfagraphs-0.3.1/gfagraphs.egg-info/
--rw-r--r--   0 sidubois (669136) genscale (35005)     2114 2024-04-23 16:25:03.000000 gfagraphs-0.3.1/gfagraphs.egg-info/PKG-INFO
--rw-r--r--   0 sidubois (669136) genscale (35005)      357 2024-04-23 16:25:03.000000 gfagraphs-0.3.1/gfagraphs.egg-info/SOURCES.txt
--rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-23 16:25:03.000000 gfagraphs-0.3.1/gfagraphs.egg-info/dependency_links.txt
--rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-19 08:24:53.000000 gfagraphs-0.3.1/gfagraphs.egg-info/not-zip-safe
--rw-r--r--   0 sidubois (669136) genscale (35005)       19 2024-04-23 16:25:03.000000 gfagraphs-0.3.1/gfagraphs.egg-info/top_level.txt
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-23 16:25:03.308799 gfagraphs-0.3.1/pgGraphs/
--rw-r--r--   0 sidubois (669136) genscale (35005)      184 2024-01-25 14:21:38.000000 gfagraphs-0.3.1/pgGraphs/__init__.py
--rw-r--r--   0 sidubois (669136) genscale (35005)     2079 2024-04-23 15:21:03.000000 gfagraphs-0.3.1/pgGraphs/abstractions.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    16717 2024-04-23 16:16:09.000000 gfagraphs-0.3.1/pgGraphs/gfaparser.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    30506 2024-04-23 16:17:02.000000 gfagraphs-0.3.1/pgGraphs/graph.py
--rw-r--r--   0 sidubois (669136) genscale (35005)     6217 2024-04-19 09:42:36.000000 gfagraphs-0.3.1/pgGraphs/networkx.py
--rw-r--r--   0 sidubois (669136) genscale (35005)      695 2024-04-23 16:25:03.000000 gfagraphs-0.3.1/pyproject.toml
--rw-r--r--   0 sidubois (669136) genscale (35005)       38 2024-04-23 16:25:03.309799 gfagraphs-0.3.1/setup.cfg
--rw-r--r--   0 sidubois (669136) genscale (35005)     2482 2024-04-23 16:06:05.000000 gfagraphs-0.3.1/setup.py
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 08:12:17.086707 gfagraphs-0.3.2/
+-rw-r--r--   0 sidubois (669136) genscale (35005)    34521 2023-11-29 09:58:07.000000 gfagraphs-0.3.2/LICENSE
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2114 2024-04-24 08:12:17.085707 gfagraphs-0.3.2/PKG-INFO
+-rw-r--r--   0 sidubois (669136) genscale (35005)     1491 2024-04-19 14:44:53.000000 gfagraphs-0.3.2/README.md
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 08:12:17.085707 gfagraphs-0.3.2/gfagraphs/
+-rw-r--r--   0 sidubois (669136) genscale (35005)       58 2024-04-19 08:22:28.000000 gfagraphs-0.3.2/gfagraphs/__init__.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    39616 2024-03-07 16:32:34.000000 gfagraphs-0.3.2/gfagraphs/gfagraphs.py
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 08:12:17.085707 gfagraphs-0.3.2/gfagraphs.egg-info/
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2114 2024-04-24 08:12:17.000000 gfagraphs-0.3.2/gfagraphs.egg-info/PKG-INFO
+-rw-r--r--   0 sidubois (669136) genscale (35005)      351 2024-04-24 08:12:17.000000 gfagraphs-0.3.2/gfagraphs.egg-info/SOURCES.txt
+-rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-24 08:12:17.000000 gfagraphs-0.3.2/gfagraphs.egg-info/dependency_links.txt
+-rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-19 08:24:53.000000 gfagraphs-0.3.2/gfagraphs.egg-info/not-zip-safe
+-rw-r--r--   0 sidubois (669136) genscale (35005)       19 2024-04-24 08:12:17.000000 gfagraphs-0.3.2/gfagraphs.egg-info/top_level.txt
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 08:12:17.085707 gfagraphs-0.3.2/pgGraphs/
+-rw-r--r--   0 sidubois (669136) genscale (35005)      178 2024-04-23 16:35:16.000000 gfagraphs-0.3.2/pgGraphs/__init__.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2079 2024-04-23 15:21:03.000000 gfagraphs-0.3.2/pgGraphs/abstractions.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    16717 2024-04-23 16:16:09.000000 gfagraphs-0.3.2/pgGraphs/gfaparser.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    30506 2024-04-23 16:17:02.000000 gfagraphs-0.3.2/pgGraphs/graph.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)     6217 2024-04-19 09:42:36.000000 gfagraphs-0.3.2/pgGraphs/nx.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)      695 2024-04-24 08:12:17.000000 gfagraphs-0.3.2/pyproject.toml
+-rw-r--r--   0 sidubois (669136) genscale (35005)       38 2024-04-24 08:12:17.086707 gfagraphs-0.3.2/setup.cfg
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2482 2024-04-24 08:12:00.000000 gfagraphs-0.3.2/setup.py
```

### Comparing `gfagraphs-0.3.1/LICENSE` & `gfagraphs-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.1/PKG-INFO` & `gfagraphs-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfagraphs
-Version: 0.3.1
+Version: 0.3.2
 Summary: Library to parse, edit and handle in memory GFA graphs
 Home-page: https://github.com/Tharos-ux/gfagraphs
 Author: ('Siegfried Dubois',)
 Author-email: Siegfried Dubois <siegfried.dubois@inria.fr>
 Project-URL: Homepage, https://github.com/Tharos-ux/gfagraphs
 Project-URL: Bug Tracker, https://github.com/Tharos-ux/gfagraphs/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gfagraphs-0.3.1/README.md` & `gfagraphs-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.1/gfagraphs/gfagraphs.py` & `gfagraphs-0.3.2/gfagraphs/gfagraphs.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.1/gfagraphs.egg-info/PKG-INFO` & `gfagraphs-0.3.2/gfagraphs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfagraphs
-Version: 0.3.1
+Version: 0.3.2
 Summary: Library to parse, edit and handle in memory GFA graphs
 Home-page: https://github.com/Tharos-ux/gfagraphs
 Author: ('Siegfried Dubois',)
 Author-email: Siegfried Dubois <siegfried.dubois@inria.fr>
 Project-URL: Homepage, https://github.com/Tharos-ux/gfagraphs
 Project-URL: Bug Tracker, https://github.com/Tharos-ux/gfagraphs/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gfagraphs-0.3.1/pgGraphs/abstractions.py` & `gfagraphs-0.3.2/pgGraphs/abstractions.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.1/pgGraphs/gfaparser.py` & `gfagraphs-0.3.2/pgGraphs/gfaparser.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.1/pgGraphs/graph.py` & `gfagraphs-0.3.2/pgGraphs/graph.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.1/pgGraphs/networkx.py` & `gfagraphs-0.3.2/pgGraphs/nx.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.1/pyproject.toml` & `gfagraphs-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["setuptools>=61.0"]
     build-backend = "setuptools.build_meta"
 
     [project]
     name = "gfagraphs"
-    version = "0.3.1"
+    version = "0.3.2"
     authors = [
     { name="Siegfried Dubois", email="siegfried.dubois@inria.fr" },
     ]
     description = "Library to parse, edit and handle in memory GFA graphs"
     readme = "README.md"
     requires-python = ">=3.10"
     classifiers = [
```

### Comparing `gfagraphs-0.3.1/setup.py` & `gfagraphs-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 NAME: str = "gfagraphs"
 AUTHOR: str = "Siegfried Dubois",
 AUTHOR_EMAIL: str = "siegfried.dubois@inria.fr",
 LICENCE: str = "LICENCE"
 DESCRIPTION: str = "Library to parse, edit and handle in memory GFA graphs"
 REQUIRED_PYTHON: tuple = (3, 10)
 OVERRIDE_VN: bool = True
-VN: str = "0.3.1"
+VN: str = "0.3.2"
 URL: str = "https://github.com/Tharos-ux/gfagraphs"
 REQUIREMENTS: list[str] = [
     'networkx',
     'tharos-pytools',
     'matplotlib',
     'mycolorpy',
 ]
```

