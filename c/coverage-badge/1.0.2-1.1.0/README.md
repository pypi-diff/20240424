# Comparing `tmp/coverage-badge-1.0.2.tar.gz` & `tmp/coverage-badge-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coverage-badge-1.0.2.tar", last modified: Tue Oct  5 10:55:22 2021, max compression
+gzip compressed data, was "coverage-badge-1.1.0.tar", last modified: Fri Nov 12 22:39:22 2021, max compression
```

## Comparing `coverage-badge-1.0.2.tar` & `coverage-badge-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 danilo    (1000) danilo    (1000)        0 2021-10-05 10:55:22.401690 coverage-badge-1.0.2/
--rw-r--r--   0 danilo    (1000) danilo    (1000)     1062 2020-06-24 12:32:37.000000 coverage-badge-1.0.2/LICENSE.txt
--rw-r--r--   0 danilo    (1000) danilo    (1000)       70 2020-06-24 12:33:04.000000 coverage-badge-1.0.2/MANIFEST.in
--rw-r--r--   0 danilo    (1000) danilo    (1000)     3164 2021-10-05 10:55:22.401690 coverage-badge-1.0.2/PKG-INFO
--rw-r--r--   0 danilo    (1000) danilo    (1000)     2572 2021-10-05 10:51:24.000000 coverage-badge-1.0.2/README.rst
-drwxr-xr-x   0 danilo    (1000) danilo    (1000)        0 2021-10-05 10:55:22.401690 coverage-badge-1.0.2/coverage_badge/
--rw-r--r--   0 danilo    (1000) danilo    (1000)     4412 2021-10-05 10:54:26.000000 coverage-badge-1.0.2/coverage_badge/__main__.py
-drwxr-xr-x   0 danilo    (1000) danilo    (1000)        0 2021-10-05 10:55:22.401690 coverage-badge-1.0.2/coverage_badge/templates/
--rw-r--r--   0 danilo    (1000) danilo    (1000)      926 2020-06-24 12:31:50.000000 coverage-badge-1.0.2/coverage_badge/templates/flat.svg
-drwxr-xr-x   0 danilo    (1000) danilo    (1000)        0 2021-10-05 10:55:22.401690 coverage-badge-1.0.2/coverage_badge.egg-info/
--rw-r--r--   0 danilo    (1000) danilo    (1000)     3164 2021-10-05 10:55:22.000000 coverage-badge-1.0.2/coverage_badge.egg-info/PKG-INFO
--rw-r--r--   0 danilo    (1000) danilo    (1000)      377 2021-10-05 10:55:22.000000 coverage-badge-1.0.2/coverage_badge.egg-info/SOURCES.txt
--rw-r--r--   0 danilo    (1000) danilo    (1000)        1 2021-10-05 10:55:22.000000 coverage-badge-1.0.2/coverage_badge.egg-info/dependency_links.txt
--rw-r--r--   0 danilo    (1000) danilo    (1000)       65 2021-10-05 10:55:22.000000 coverage-badge-1.0.2/coverage_badge.egg-info/entry_points.txt
--rw-r--r--   0 danilo    (1000) danilo    (1000)       14 2021-10-05 10:55:22.000000 coverage-badge-1.0.2/coverage_badge.egg-info/requires.txt
--rw-r--r--   0 danilo    (1000) danilo    (1000)       15 2021-10-05 10:55:22.000000 coverage-badge-1.0.2/coverage_badge.egg-info/top_level.txt
--rw-r--r--   0 danilo    (1000) danilo    (1000)        1 2021-10-05 10:55:22.000000 coverage-badge-1.0.2/coverage_badge.egg-info/zip-safe
--rw-r--r--   0 danilo    (1000) danilo    (1000)       67 2021-10-05 10:55:22.405024 coverage-badge-1.0.2/setup.cfg
--rw-r--r--   0 danilo    (1000) danilo    (1000)      986 2021-10-05 10:53:43.000000 coverage-badge-1.0.2/setup.py
+drwxr-xr-x   0 danilo    (1000) danilo    (1000)        0 2021-11-12 22:39:22.861975 coverage-badge-1.1.0/
+-rw-r--r--   0 danilo    (1000) danilo    (1000)     1062 2021-05-17 16:08:45.000000 coverage-badge-1.1.0/LICENSE.txt
+-rw-r--r--   0 danilo    (1000) danilo    (1000)       70 2021-05-17 16:08:45.000000 coverage-badge-1.1.0/MANIFEST.in
+-rw-r--r--   0 danilo    (1000) danilo    (1000)     3148 2021-11-12 22:39:22.861975 coverage-badge-1.1.0/PKG-INFO
+-rw-r--r--   0 danilo    (1000) danilo    (1000)     2556 2021-10-08 07:09:15.000000 coverage-badge-1.1.0/README.rst
+drwxr-xr-x   0 danilo    (1000) danilo    (1000)        0 2021-11-12 22:39:22.861975 coverage-badge-1.1.0/coverage_badge/
+-rw-r--r--   0 danilo    (1000) danilo    (1000)     4993 2021-11-12 22:37:05.000000 coverage-badge-1.1.0/coverage_badge/__main__.py
+drwxr-xr-x   0 danilo    (1000) danilo    (1000)        0 2021-11-12 22:39:22.861975 coverage-badge-1.1.0/coverage_badge/templates/
+-rw-r--r--   0 danilo    (1000) danilo    (1000)      926 2016-11-29 19:23:57.000000 coverage-badge-1.1.0/coverage_badge/templates/flat.svg
+drwxr-xr-x   0 danilo    (1000) danilo    (1000)        0 2021-11-12 22:39:22.861975 coverage-badge-1.1.0/coverage_badge.egg-info/
+-rw-r--r--   0 danilo    (1000) danilo    (1000)     3148 2021-11-12 22:39:22.000000 coverage-badge-1.1.0/coverage_badge.egg-info/PKG-INFO
+-rw-r--r--   0 danilo    (1000) danilo    (1000)      377 2021-11-12 22:39:22.000000 coverage-badge-1.1.0/coverage_badge.egg-info/SOURCES.txt
+-rw-r--r--   0 danilo    (1000) danilo    (1000)        1 2021-11-12 22:39:22.000000 coverage-badge-1.1.0/coverage_badge.egg-info/dependency_links.txt
+-rw-r--r--   0 danilo    (1000) danilo    (1000)       65 2021-11-12 22:39:22.000000 coverage-badge-1.1.0/coverage_badge.egg-info/entry_points.txt
+-rw-r--r--   0 danilo    (1000) danilo    (1000)        9 2021-11-12 22:39:22.000000 coverage-badge-1.1.0/coverage_badge.egg-info/requires.txt
+-rw-r--r--   0 danilo    (1000) danilo    (1000)       15 2021-11-12 22:39:22.000000 coverage-badge-1.1.0/coverage_badge.egg-info/top_level.txt
+-rw-r--r--   0 danilo    (1000) danilo    (1000)        1 2016-11-29 19:28:34.000000 coverage-badge-1.1.0/coverage_badge.egg-info/zip-safe
+-rw-r--r--   0 danilo    (1000) danilo    (1000)       67 2021-11-12 22:39:22.861975 coverage-badge-1.1.0/setup.cfg
+-rw-r--r--   0 danilo    (1000) danilo    (1000)      981 2021-11-12 22:36:59.000000 coverage-badge-1.1.0/setup.py
```

### Comparing `coverage-badge-1.0.2/LICENSE.txt` & `coverage-badge-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coverage-badge-1.0.2/PKG-INFO` & `coverage-badge-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coverage-badge
-Version: 1.0.2
+Version: 1.1.0
 Summary: Generate coverage badges for Coverage.py.
 Home-page: https://github.com/dbrgn/coverage-badge
 Author: Danilo Bargen
 Author-email: mail@dbrgn.ch
 License: MIT
 Keywords: coverage badge shield
 Platform: UNKNOWN
@@ -17,23 +17,23 @@
 License-File: LICENSE.txt
 
 Coverage.py Badge
 ==================
 
 .. image:: https://github.com/dbrgn/coverage-badge/workflows/CI/badge.svg
     :alt: Build status
-    :target: https://github.com/dbrgn/coverage-badge/actions?query=branch%3Amaster
+    :target: https://github.com/dbrgn/coverage-badge/actions?query=branch%3Amain
 
 .. image:: https://img.shields.io/pypi/dm/coverage-badge.svg
     :alt: PyPI Downloads
     :target: https://pypi.python.org/pypi/coverage-badge
 
 A small script to generate coverage badges using Coverage.py. Example of a generated badge:
 
-.. image:: https://cdn.rawgit.com/dbrgn/coverage-badge/master/example.svg
+.. image:: https://cdn.rawgit.com/dbrgn/coverage-badge/main/example.svg
     :alt: Example coverage badge
 
 The badge template has been taken from shields.io_, therefore it should look
 mostly good. (The spec is a bit stricter on the margins, but I can't easily do
 text width calculations in Python so the margins might not always be 4px.)
 
 **:arrow_right: Note:** If you need a script with a few more features
@@ -64,30 +64,30 @@
     $ coverage-badge -o coverage.svg
 
 It's important that you run ``coverage-badge`` from the directory where the
 ``.coverage`` data file is located.
 
 Different colors for cover ranges:
 
-.. image:: https://cdn.rawgit.com/samael500/coverage-badge/master/media/15.svg
+.. image:: https://cdn.rawgit.com/samael500/coverage-badge/main/media/15.svg
     :alt: 15%
 
-.. image:: https://cdn.rawgit.com/samael500/coverage-badge/master/media/45.svg
+.. image:: https://cdn.rawgit.com/samael500/coverage-badge/main/media/45.svg
     :alt: 45%
 
-.. image:: https://cdn.rawgit.com/samael500/coverage-badge/master/media/65.svg
+.. image:: https://cdn.rawgit.com/samael500/coverage-badge/main/media/65.svg
     :alt: 65%
 
-.. image:: https://cdn.rawgit.com/samael500/coverage-badge/master/media/80.svg
+.. image:: https://cdn.rawgit.com/samael500/coverage-badge/main/media/80.svg
     :alt: 80%
 
-.. image:: https://cdn.rawgit.com/samael500/coverage-badge/master/media/93.svg
+.. image:: https://cdn.rawgit.com/samael500/coverage-badge/main/media/93.svg
     :alt: 93%
 
-.. image:: https://cdn.rawgit.com/samael500/coverage-badge/master/media/97.svg
+.. image:: https://cdn.rawgit.com/samael500/coverage-badge/main/media/97.svg
     :alt: 97%
 
 ----
 
 The full usage text::
 
     usage: __main__.py [-h] [-o FILEPATH] [-p] [-f] [-q] [-v]
```

### Comparing `coverage-badge-1.0.2/README.rst` & `coverage-badge-1.1.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Coverage.py Badge
 ==================
 
 .. image:: https://github.com/dbrgn/coverage-badge/workflows/CI/badge.svg
     :alt: Build status
-    :target: https://github.com/dbrgn/coverage-badge/actions?query=branch%3Amaster
+    :target: https://github.com/dbrgn/coverage-badge/actions?query=branch%3Amain
 
 .. image:: https://img.shields.io/pypi/dm/coverage-badge.svg
     :alt: PyPI Downloads
     :target: https://pypi.python.org/pypi/coverage-badge
 
 A small script to generate coverage badges using Coverage.py. Example of a generated badge:
 
-.. image:: https://cdn.rawgit.com/dbrgn/coverage-badge/master/example.svg
+.. image:: https://cdn.rawgit.com/dbrgn/coverage-badge/main/example.svg
     :alt: Example coverage badge
 
 The badge template has been taken from shields.io_, therefore it should look
 mostly good. (The spec is a bit stricter on the margins, but I can't easily do
 text width calculations in Python so the margins might not always be 4px.)
 
 **:arrow_right: Note:** If you need a script with a few more features
@@ -46,30 +46,30 @@
     $ coverage-badge -o coverage.svg
 
 It's important that you run ``coverage-badge`` from the directory where the
 ``.coverage`` data file is located.
 
 Different colors for cover ranges:
 
-.. image:: https://cdn.rawgit.com/samael500/coverage-badge/master/media/15.svg
+.. image:: https://cdn.rawgit.com/samael500/coverage-badge/main/media/15.svg
     :alt: 15%
 
-.. image:: https://cdn.rawgit.com/samael500/coverage-badge/master/media/45.svg
+.. image:: https://cdn.rawgit.com/samael500/coverage-badge/main/media/45.svg
     :alt: 45%
 
-.. image:: https://cdn.rawgit.com/samael500/coverage-badge/master/media/65.svg
+.. image:: https://cdn.rawgit.com/samael500/coverage-badge/main/media/65.svg
     :alt: 65%
 
-.. image:: https://cdn.rawgit.com/samael500/coverage-badge/master/media/80.svg
+.. image:: https://cdn.rawgit.com/samael500/coverage-badge/main/media/80.svg
     :alt: 80%
 
-.. image:: https://cdn.rawgit.com/samael500/coverage-badge/master/media/93.svg
+.. image:: https://cdn.rawgit.com/samael500/coverage-badge/main/media/93.svg
     :alt: 93%
 
-.. image:: https://cdn.rawgit.com/samael500/coverage-badge/master/media/97.svg
+.. image:: https://cdn.rawgit.com/samael500/coverage-badge/main/media/97.svg
     :alt: 97%
 
 ----
 
 The full usage text::
 
     usage: __main__.py [-h] [-o FILEPATH] [-p] [-f] [-q] [-v]
```

### Comparing `coverage-badge-1.0.2/coverage_badge/__main__.py` & `coverage-badge-1.1.0/coverage_badge/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 import argparse
 import pkg_resources
 
 import coverage
 
 
-__version__ = '1.0.2'
+__version__ = '1.1.0'
 
 
 DEFAULT_COLOR = '#a4a61d'
 COLORS = {
     'brightgreen': '#4c1',
     'green': '#97CA00',
     'yellowgreen': '#a4a61d',
@@ -45,31 +45,39 @@
     """
     Return the rounded total as properly rounded string.
     """
     cov = coverage.Coverage()
     cov.load()
     total = cov.report(file=Devnull())
 
-    class Precision(coverage.results.Numbers):
-        """
-        A class for using the percentage rounding of the main coverage package,
-        with any percentage.
-
-        To get the string format of the percentage, use the ``pc_covered_str``
-        property.
-
-        """
-        def __init__(self, percent):
-            self.percent = percent
-
-        @property
-        def pc_covered(self):
-            return self.percent
-
-    return Precision(total).pc_covered_str
+    if hasattr(coverage.results.Numbers, 'set_precision'):  # Coverage <= 5
+        class Precision(coverage.results.Numbers):
+            """
+            A class for using the percentage rounding of the main coverage package,
+            with any percentage.
+
+            To get the string format of the percentage, use the ``pc_covered_str``
+            property.
+
+            """
+            def __init__(self, percent):
+                self.percent = percent
+
+            @property
+            def pc_covered(self):
+                return self.percent
+
+        return Precision(total).pc_covered_str
+    else:  # Coverage 6.x
+        # NOTE: Precision is no longer set globally in the
+        # `coverage.results.Numbers` class. Instead the precision must be
+        # passed in as the first argument. We pull the precision from the
+        # `coverage.Coverage` object because it should pull the correct
+        # precision from the local .coveragerc file.
+        return coverage.results.Numbers(precision=cov.config.precision).display_covered(total)
 
 
 def get_color(total):
     """
     Return color for current coverage precent
     """
     try:
```

### Comparing `coverage-badge-1.0.2/coverage_badge/templates/flat.svg` & `coverage-badge-1.1.0/coverage_badge/templates/flat.svg`

 * *Files identical despite different names*

### Comparing `coverage-badge-1.0.2/coverage_badge.egg-info/PKG-INFO` & `coverage-badge-1.1.0/coverage_badge.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coverage-badge
-Version: 1.0.2
+Version: 1.1.0
 Summary: Generate coverage badges for Coverage.py.
 Home-page: https://github.com/dbrgn/coverage-badge
 Author: Danilo Bargen
 Author-email: mail@dbrgn.ch
 License: MIT
 Keywords: coverage badge shield
 Platform: UNKNOWN
@@ -17,23 +17,23 @@
 License-File: LICENSE.txt
 
 Coverage.py Badge
 ==================
 
 .. image:: https://github.com/dbrgn/coverage-badge/workflows/CI/badge.svg
     :alt: Build status
-    :target: https://github.com/dbrgn/coverage-badge/actions?query=branch%3Amaster
+    :target: https://github.com/dbrgn/coverage-badge/actions?query=branch%3Amain
 
 .. image:: https://img.shields.io/pypi/dm/coverage-badge.svg
     :alt: PyPI Downloads
     :target: https://pypi.python.org/pypi/coverage-badge
 
 A small script to generate coverage badges using Coverage.py. Example of a generated badge:
 
-.. image:: https://cdn.rawgit.com/dbrgn/coverage-badge/master/example.svg
+.. image:: https://cdn.rawgit.com/dbrgn/coverage-badge/main/example.svg
     :alt: Example coverage badge
 
 The badge template has been taken from shields.io_, therefore it should look
 mostly good. (The spec is a bit stricter on the margins, but I can't easily do
 text width calculations in Python so the margins might not always be 4px.)
 
 **:arrow_right: Note:** If you need a script with a few more features
@@ -64,30 +64,30 @@
     $ coverage-badge -o coverage.svg
 
 It's important that you run ``coverage-badge`` from the directory where the
 ``.coverage`` data file is located.
 
 Different colors for cover ranges:
 
-.. image:: https://cdn.rawgit.com/samael500/coverage-badge/master/media/15.svg
+.. image:: https://cdn.rawgit.com/samael500/coverage-badge/main/media/15.svg
     :alt: 15%
 
-.. image:: https://cdn.rawgit.com/samael500/coverage-badge/master/media/45.svg
+.. image:: https://cdn.rawgit.com/samael500/coverage-badge/main/media/45.svg
     :alt: 45%
 
-.. image:: https://cdn.rawgit.com/samael500/coverage-badge/master/media/65.svg
+.. image:: https://cdn.rawgit.com/samael500/coverage-badge/main/media/65.svg
     :alt: 65%
 
-.. image:: https://cdn.rawgit.com/samael500/coverage-badge/master/media/80.svg
+.. image:: https://cdn.rawgit.com/samael500/coverage-badge/main/media/80.svg
     :alt: 80%
 
-.. image:: https://cdn.rawgit.com/samael500/coverage-badge/master/media/93.svg
+.. image:: https://cdn.rawgit.com/samael500/coverage-badge/main/media/93.svg
     :alt: 93%
 
-.. image:: https://cdn.rawgit.com/samael500/coverage-badge/master/media/97.svg
+.. image:: https://cdn.rawgit.com/samael500/coverage-badge/main/media/97.svg
     :alt: 97%
 
 ----
 
 The full usage text::
 
     usage: __main__.py [-h] [-o FILEPATH] [-p] [-f] [-q] [-v]
```

### Comparing `coverage-badge-1.0.2/setup.py` & `coverage-badge-1.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
 readme = open('README.rst').read()
 
 setup(name='coverage-badge',
-      version='1.0.2',
+      version='1.1.0',
       description='Generate coverage badges for Coverage.py.',
       author='Danilo Bargen',
       author_email='mail@dbrgn.ch',
       url='https://github.com/dbrgn/coverage-badge',
-      install_requires=['coverage==5.*'],
+      install_requires=['coverage'],
       packages=['coverage_badge'],
       zip_safe=True,
       include_package_data=True,
       license='MIT',
       keywords='coverage badge shield',
       long_description=readme,
       entry_points={
```

