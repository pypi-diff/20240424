# Comparing `tmp/schedula_core-1.5.7.tar.gz` & `tmp/schedula_core-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schedula_core-1.5.7.tar", last modified: Fri Apr 19 10:49:42 2024, max compression
+gzip compressed data, was "schedula_core-1.5.8.tar", last modified: Fri Apr 19 12:14:57 2024, max compression
```

## Comparing `schedula_core-1.5.7.tar` & `schedula_core-1.5.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:49:42.277184 schedula_core-1.5.7/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       67 2024-04-12 16:17:27.000000 schedula_core-1.5.7/AUTHORS.rst
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13141 2024-04-12 16:17:27.000000 schedula_core-1.5.7/LICENSE.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4233 2024-04-19 10:49:42.277094 schedula_core-1.5.7/PKG-INFO
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    21979 2024-04-19 10:36:00.000000 schedula_core-1.5.7/README.rst
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:49:42.269435 schedula_core-1.5.7/schedula/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4309 2024-04-17 14:10:45.000000 schedula_core-1.5.7/schedula/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      777 2024-04-19 10:36:00.000000 schedula_core-1.5.7/schedula/_version.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1267 2024-04-17 14:10:45.000000 schedula_core-1.5.7/schedula/cli.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    68892 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/dispatcher.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:49:42.273668 schedula_core-1.5.7/schedula/utils/
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1446 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/__init__.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    13251 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/alg.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:49:42.274514 schedula_core-1.5.7/schedula/utils/asy/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11064 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/asy/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8126 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/asy/executors.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3284 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/asy/factory.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16000 2024-04-17 16:28:10.000000 schedula_core-1.5.7/schedula/utils/base.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    24001 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/blue.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2009 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/cst.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    56461 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/dsp.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1392 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/exc.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2194 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/gen.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4332 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/graph.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      692 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/imp.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    40509 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/sol.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1630 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/utl.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:49:42.276847 schedula_core-1.5.7/schedula_core.egg-info/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4233 2024-04-19 10:49:42.000000 schedula_core-1.5.7/schedula_core.egg-info/PKG-INFO
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      761 2024-04-19 10:49:42.000000 schedula_core-1.5.7/schedula_core.egg-info/SOURCES.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        1 2024-04-19 10:49:42.000000 schedula_core-1.5.7/schedula_core.egg-info/dependency_links.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        9 2024-04-19 10:49:42.000000 schedula_core-1.5.7/schedula_core.egg-info/top_level.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      162 2024-04-19 10:49:42.277574 schedula_core-1.5.7/setup.cfg
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     7344 2024-04-19 10:12:23.000000 schedula_core-1.5.7/setup.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:49:42.276578 schedula_core-1.5.7/tests/
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    89504 2024-04-12 16:17:27.000000 schedula_core-1.5.7/tests/test_dispatcher.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1020 2024-04-12 16:17:27.000000 schedula_core-1.5.7/tests/test_import.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1164 2024-04-12 16:17:27.000000 schedula_core-1.5.7/tests/test_micropython.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)      872 2024-04-12 16:17:27.000000 schedula_core-1.5.7/tests/test_readme.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1028 2024-04-12 16:17:27.000000 schedula_core-1.5.7/tests/test_setup.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:14:57.746957 schedula_core-1.5.8/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       67 2024-04-12 16:17:27.000000 schedula_core-1.5.8/AUTHORS.rst
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13141 2024-04-12 16:17:27.000000 schedula_core-1.5.8/LICENSE.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4233 2024-04-19 12:14:57.746896 schedula_core-1.5.8/PKG-INFO
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    21979 2024-04-19 12:06:22.000000 schedula_core-1.5.8/README.rst
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:14:57.739318 schedula_core-1.5.8/schedula/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4309 2024-04-17 14:10:45.000000 schedula_core-1.5.8/schedula/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      777 2024-04-19 12:06:22.000000 schedula_core-1.5.8/schedula/_version.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1267 2024-04-17 14:10:45.000000 schedula_core-1.5.8/schedula/cli.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    68892 2024-04-12 16:17:27.000000 schedula_core-1.5.8/schedula/dispatcher.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:14:57.744025 schedula_core-1.5.8/schedula/utils/
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1446 2024-04-12 16:17:27.000000 schedula_core-1.5.8/schedula/utils/__init__.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    13251 2024-04-12 16:17:27.000000 schedula_core-1.5.8/schedula/utils/alg.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:14:57.744852 schedula_core-1.5.8/schedula/utils/asy/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11064 2024-04-12 16:17:27.000000 schedula_core-1.5.8/schedula/utils/asy/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8126 2024-04-12 16:17:27.000000 schedula_core-1.5.8/schedula/utils/asy/executors.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3284 2024-04-12 16:17:27.000000 schedula_core-1.5.8/schedula/utils/asy/factory.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16000 2024-04-17 16:28:10.000000 schedula_core-1.5.8/schedula/utils/base.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    24001 2024-04-12 16:17:27.000000 schedula_core-1.5.8/schedula/utils/blue.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2009 2024-04-12 16:17:27.000000 schedula_core-1.5.8/schedula/utils/cst.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    56461 2024-04-12 16:17:27.000000 schedula_core-1.5.8/schedula/utils/dsp.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1392 2024-04-12 16:17:27.000000 schedula_core-1.5.8/schedula/utils/exc.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2194 2024-04-12 16:17:27.000000 schedula_core-1.5.8/schedula/utils/gen.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4332 2024-04-12 16:17:27.000000 schedula_core-1.5.8/schedula/utils/graph.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      692 2024-04-12 16:17:27.000000 schedula_core-1.5.8/schedula/utils/imp.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    40509 2024-04-12 16:17:27.000000 schedula_core-1.5.8/schedula/utils/sol.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1630 2024-04-12 16:17:27.000000 schedula_core-1.5.8/schedula/utils/utl.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:14:57.746667 schedula_core-1.5.8/schedula_core.egg-info/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4233 2024-04-19 12:14:57.000000 schedula_core-1.5.8/schedula_core.egg-info/PKG-INFO
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      761 2024-04-19 12:14:57.000000 schedula_core-1.5.8/schedula_core.egg-info/SOURCES.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        1 2024-04-19 12:14:57.000000 schedula_core-1.5.8/schedula_core.egg-info/dependency_links.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        9 2024-04-19 12:14:57.000000 schedula_core-1.5.8/schedula_core.egg-info/top_level.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      162 2024-04-19 12:14:57.747193 schedula_core-1.5.8/setup.cfg
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     7360 2024-04-19 12:06:22.000000 schedula_core-1.5.8/setup.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:14:57.746481 schedula_core-1.5.8/tests/
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    89504 2024-04-12 16:17:27.000000 schedula_core-1.5.8/tests/test_dispatcher.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1020 2024-04-12 16:17:27.000000 schedula_core-1.5.8/tests/test_import.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1164 2024-04-12 16:17:27.000000 schedula_core-1.5.8/tests/test_micropython.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)      872 2024-04-12 16:17:27.000000 schedula_core-1.5.8/tests/test_readme.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1028 2024-04-12 16:17:27.000000 schedula_core-1.5.8/tests/test_setup.py
```

### Comparing `schedula_core-1.5.7/LICENSE.txt` & `schedula_core-1.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/PKG-INFO` & `schedula_core-1.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: schedula-core
-Version: 1.5.7
+Version: 1.5.8
 Summary: Produce a plan that dispatches calls based on a graph of functions, satisfying data dependencies.
 Home-page: https://github.com/vinci1it2000/schedula
-Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.7
+Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.8
 Author: Vincenzo Arcidiacono
 Author-email: vinci1it2000@gmail.com
 License: EUPL 1.1+
 Project-URL: Documentation, https://schedula.readthedocs.io
 Project-URL: Issue tracker, https://github.com/vinci1it2000/schedula/issues
 Keywords: flow-based programming,dataflow,parallel,asynchronous,async,scheduling,dispatch,functional programming,dataflow programming
 Classifier: Programming Language :: Python
```

### Comparing `schedula_core-1.5.7/README.rst` & `schedula_core-1.5.8/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 #######################################################################
 schedula: A smart function scheduler for dynamic flow-based programming
 #######################################################################
 |pypi_ver| |test_status| |cover_status| |docs_status| |downloads|
 |month_downloads| |github_issues| |python_ver| |proj_license| |binder|
 
-:release:       1.5.7
-:date:          2024-04-19 12:30:00
+:release:       1.5.8
+:date:          2024-04-20 00:00:00
 :repository:    https://github.com/vinci1it2000/schedula
 :pypi-repo:     https://pypi.org/project/schedula/
 :docs:          https://schedula.readthedocs.io/
 :wiki:          https://github.com/vinci1it2000/schedula/wiki/
 :download:      https://github.com/vinci1it2000/schedula/releases/
 :keywords:      flow-based programming, dataflow, parallel, async, scheduling,
                 dispatch, functional programming, dataflow programming
```

### Comparing `schedula_core-1.5.7/schedula/__init__.py` & `schedula_core-1.5.8/schedula/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/schedula/_version.py` & `schedula_core-1.5.8/schedula/_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 # You may not use this work except in compliance with the Licence.
 # You may obtain a copy of the Licence at: http://ec.europa.eu/idabc/eupl
 
 __all__ = ['__version__', '__updated__', '__title__', '__author__',
            '__license__', '__copyright__']
 
 #: Authoritative project's PEP 440 version.
-__version__ = version = "1.5.7"  # Also update README.rst
+__version__ = version = "1.5.8"  # Also update README.rst
 
 # Please UPDATE TIMESTAMP WHEN BUMPING VERSIONS AND BEFORE RELEASE.
 #: Release date.
-__updated__ = "2024-04-19 12:30:00"
+__updated__ = "2024-04-20 00:00:00"
 
 __title__ = 'schedula'
 
 __author__ = 'Vincenzo Arcidiacono <vinci1it2000@gmail.com>'
 
 __license__ = 'EUPL, see LICENSE.txt'
```

### Comparing `schedula_core-1.5.7/schedula/cli.py` & `schedula_core-1.5.8/schedula/cli.py`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/schedula/dispatcher.py` & `schedula_core-1.5.8/schedula/dispatcher.py`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/schedula/utils/__init__.py` & `schedula_core-1.5.8/schedula/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/schedula/utils/alg.py` & `schedula_core-1.5.8/schedula/utils/alg.py`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/schedula/utils/asy/__init__.py` & `schedula_core-1.5.8/schedula/utils/asy/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/schedula/utils/asy/executors.py` & `schedula_core-1.5.8/schedula/utils/asy/executors.py`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/schedula/utils/asy/factory.py` & `schedula_core-1.5.8/schedula/utils/asy/factory.py`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/schedula/utils/base.py` & `schedula_core-1.5.8/schedula/utils/base.py`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/schedula/utils/blue.py` & `schedula_core-1.5.8/schedula/utils/blue.py`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/schedula/utils/cst.py` & `schedula_core-1.5.8/schedula/utils/cst.py`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/schedula/utils/dsp.py` & `schedula_core-1.5.8/schedula/utils/dsp.py`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/schedula/utils/exc.py` & `schedula_core-1.5.8/schedula/utils/exc.py`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/schedula/utils/gen.py` & `schedula_core-1.5.8/schedula/utils/gen.py`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/schedula/utils/graph.py` & `schedula_core-1.5.8/schedula/utils/graph.py`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/schedula/utils/imp.py` & `schedula_core-1.5.8/schedula/utils/imp.py`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/schedula/utils/sol.py` & `schedula_core-1.5.8/schedula/utils/sol.py`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/schedula/utils/utl.py` & `schedula_core-1.5.8/schedula/utils/utl.py`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/schedula_core.egg-info/PKG-INFO` & `schedula_core-1.5.8/schedula_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: schedula-core
-Version: 1.5.7
+Version: 1.5.8
 Summary: Produce a plan that dispatches calls based on a graph of functions, satisfying data dependencies.
 Home-page: https://github.com/vinci1it2000/schedula
-Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.7
+Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.8
 Author: Vincenzo Arcidiacono
 Author-email: vinci1it2000@gmail.com
 License: EUPL 1.1+
 Project-URL: Documentation, https://schedula.readthedocs.io
 Project-URL: Issue tracker, https://github.com/vinci1it2000/schedula/issues
 Keywords: flow-based programming,dataflow,parallel,asynchronous,async,scheduling,dispatch,functional programming,dataflow programming
 Classifier: Programming Language :: Python
```

### Comparing `schedula_core-1.5.7/schedula_core.egg-info/SOURCES.txt` & `schedula_core-1.5.8/schedula_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/setup.py` & `schedula_core-1.5.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,17 +180,19 @@
         extras_require=extras,
         tests_require=['requests', 'cryptography', 'ddt'],
         package_data={
             'schedula.utils.drw': [
                 'templates/*', 'index/js/*', 'index/css/*', 'viz/*'
             ],
             'schedula.utils.form': [
-                'templates/schedula/*', 'static/schedula/js/*.js.gz',
-                'static/schedula/css/*.css.gz',
-                'static/schedula/media/*.gz',
                 'static/schedula/forms/*',
-                'templates/schedula/*',
-                'templates/schedula/email/*'
+                'static/schedula/**/*.gz',
+                'static/schedula/**/*.LICENSE.txt',
+                'templates/**/*',
+                'sample/.babelrc',
+                'sample/*.*',
+                'sample/src/**/*',
+                'translations/**/*'
             ]
         },
         **kw
     )
```

### Comparing `schedula_core-1.5.7/tests/test_dispatcher.py` & `schedula_core-1.5.8/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/tests/test_import.py` & `schedula_core-1.5.8/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/tests/test_micropython.py` & `schedula_core-1.5.8/tests/test_micropython.py`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/tests/test_readme.py` & `schedula_core-1.5.8/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `schedula_core-1.5.7/tests/test_setup.py` & `schedula_core-1.5.8/tests/test_setup.py`

 * *Files identical despite different names*

