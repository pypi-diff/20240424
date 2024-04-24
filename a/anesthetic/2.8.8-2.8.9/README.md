# Comparing `tmp/anesthetic-2.8.8.tar.gz` & `tmp/anesthetic-2.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anesthetic-2.8.8.tar", last modified: Tue Apr  9 18:03:31 2024, max compression
+gzip compressed data, was "anesthetic-2.8.9.tar", last modified: Tue Apr  9 18:44:20 2024, max compression
```

## Comparing `anesthetic-2.8.8.tar` & `anesthetic-2.8.9.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:03:31.101401 anesthetic-2.8.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-09 18:03:27.000000 anesthetic-2.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-04-09 18:03:31.101401 anesthetic-2.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-04-09 18:03:27.000000 anesthetic-2.8.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:03:31.093401 anesthetic-2.8.8/anesthetic/
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/_code_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/_format.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/boundary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:03:31.097401 anesthetic-2.8.8/anesthetic/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/examples/_matplotlib_agg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/examples/perfect_ns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/examples/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:03:31.097401 anesthetic-2.8.8/anesthetic/gui/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9584 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/gui/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/gui/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/kde.py
--rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/labelled_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    58734 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:03:31.097401 anesthetic-2.8.8/anesthetic/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/plotting/_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:03:31.097401 anesthetic-2.8.8/anesthetic/plotting/_matplotlib/
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/plotting/_matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/plotting/_matplotlib/boxplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/plotting/_matplotlib/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/plotting/_matplotlib/hist.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/plotting/_matplotlib/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:03:31.097401 anesthetic-2.8.8/anesthetic/read/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/read/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/read/cobaya.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/read/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/read/getdist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/read/hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/read/multinest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/read/nestedfit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/read/polychord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/read/ultranest.py
--rw-r--r--   0 runner    (1001) docker     (127)    53464 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/samples.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)    21306 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/weighted_labelled_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-04-09 18:03:27.000000 anesthetic-2.8.8/anesthetic/weighted_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:03:31.101401 anesthetic-2.8.8/anesthetic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-04-09 18:03:31.000000 anesthetic-2.8.8/anesthetic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-09 18:03:31.000000 anesthetic-2.8.8/anesthetic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:03:31.000000 anesthetic-2.8.8/anesthetic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 18:03:31.000000 anesthetic-2.8.8/anesthetic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-09 18:03:31.000000 anesthetic-2.8.8/anesthetic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 18:03:31.000000 anesthetic-2.8.8/anesthetic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-09 18:03:27.000000 anesthetic-2.8.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-09 18:03:31.101401 anesthetic-2.8.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:03:31.101401 anesthetic-2.8.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-09 18:03:27.000000 anesthetic-2.8.8/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-09 18:03:27.000000 anesthetic-2.8.8/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-09 18:03:27.000000 anesthetic-2.8.8/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)    19493 2024-04-09 18:03:27.000000 anesthetic-2.8.8/tests/test_labelled_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    35940 2024-04-09 18:03:27.000000 anesthetic-2.8.8/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-04-09 18:03:27.000000 anesthetic-2.8.8/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    73424 2024-04-09 18:03:27.000000 anesthetic-2.8.8/tests/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-09 18:03:27.000000 anesthetic-2.8.8/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-09 18:03:27.000000 anesthetic-2.8.8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-09 18:03:27.000000 anesthetic-2.8.8/tests/test_weighted_labelled_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    35211 2024-04-09 18:03:27.000000 anesthetic-2.8.8/tests/test_weighted_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:44:20.178899 anesthetic-2.8.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-09 18:44:13.000000 anesthetic-2.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-04-09 18:44:20.178899 anesthetic-2.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-04-09 18:44:13.000000 anesthetic-2.8.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:44:20.170899 anesthetic-2.8.9/anesthetic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/_code_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/boundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:44:20.174899 anesthetic-2.8.9/anesthetic/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/examples/_matplotlib_agg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/examples/perfect_ns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/examples/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:44:20.174899 anesthetic-2.8.9/anesthetic/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9584 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/gui/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/gui/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/kde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/labelled_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58734 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:44:20.174899 anesthetic-2.8.9/anesthetic/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/plotting/_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:44:20.174899 anesthetic-2.8.9/anesthetic/plotting/_matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/plotting/_matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/plotting/_matplotlib/boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/plotting/_matplotlib/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/plotting/_matplotlib/hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/plotting/_matplotlib/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:44:20.178899 anesthetic-2.8.9/anesthetic/read/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/read/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/read/cobaya.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/read/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/read/getdist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/read/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/read/multinest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/read/nestedfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/read/polychord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/read/ultranest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54451 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21306 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/weighted_labelled_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-04-09 18:44:13.000000 anesthetic-2.8.9/anesthetic/weighted_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:44:20.178899 anesthetic-2.8.9/anesthetic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-04-09 18:44:20.000000 anesthetic-2.8.9/anesthetic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-09 18:44:20.000000 anesthetic-2.8.9/anesthetic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:44:20.000000 anesthetic-2.8.9/anesthetic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 18:44:20.000000 anesthetic-2.8.9/anesthetic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-09 18:44:20.000000 anesthetic-2.8.9/anesthetic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 18:44:20.000000 anesthetic-2.8.9/anesthetic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-09 18:44:13.000000 anesthetic-2.8.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-09 18:44:20.182900 anesthetic-2.8.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:44:20.178899 anesthetic-2.8.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-09 18:44:13.000000 anesthetic-2.8.9/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-09 18:44:13.000000 anesthetic-2.8.9/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-09 18:44:13.000000 anesthetic-2.8.9/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19493 2024-04-09 18:44:13.000000 anesthetic-2.8.9/tests/test_labelled_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35940 2024-04-09 18:44:13.000000 anesthetic-2.8.9/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-04-09 18:44:13.000000 anesthetic-2.8.9/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73257 2024-04-09 18:44:13.000000 anesthetic-2.8.9/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-09 18:44:13.000000 anesthetic-2.8.9/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-09 18:44:13.000000 anesthetic-2.8.9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-09 18:44:13.000000 anesthetic-2.8.9/tests/test_weighted_labelled_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35211 2024-04-09 18:44:13.000000 anesthetic-2.8.9/tests/test_weighted_pandas.py
```

### Comparing `anesthetic-2.8.8/LICENSE` & `anesthetic-2.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/PKG-INFO` & `anesthetic-2.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anesthetic
-Version: 2.8.8
+Version: 2.8.9
 Summary: nested sampling post-processing
 Author-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>, Adam Ormondroyd <ano23@cam.ac.uk>, Harry Bevins <htjb2@cam.ac.uk>, Johannes Buchner <jbuchner@mpe.mpg.de>, Ethan Carragher <ethan.carragher@adelaide.edu.au>, Andrew Fowlie <andrew.j.fowlie@googlemail.com>, Thomas Gessey-Jones <tg400@cam.ac.uk>, Stefan Heimersheim <sh2061@ast.cam.ac.uk>, Pablo Lemos <plemos91@gmail.com>, Toby Lovick <tcl44@cam.ac.uk>, Deborah Odunuyi <debbieodunuyi@gmail.com>, Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>, Liangliang Su <liangliangsu@njnu.edu.cn>, David Yallup <david.yallup@gmail.com>, Dily Ong <dlo26@cam.ac.uk>
 Maintainer-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>
 License: MIT License
         
         Copyright (c) 2019 Will Handley
         
@@ -80,15 +80,15 @@
 Requires-Dist: getdist; extra == "all"
 Requires-Dist: tables==3.8.0; extra == "all"
 
 ===========================================
 anesthetic: nested sampling post-processing
 ===========================================
 :Authors: Will Handley and Lukas Hergt
-:Version: 2.8.8
+:Version: 2.8.9
 :Homepage: https://github.com/handley-lab/anesthetic
 :Documentation: http://anesthetic.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/anesthetic/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/anesthetic/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/anesthetic/branch/master/graph/badge.svg
```

### Comparing `anesthetic-2.8.8/README.rst` & `anesthetic-2.8.9/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ===========================================
 anesthetic: nested sampling post-processing
 ===========================================
 :Authors: Will Handley and Lukas Hergt
-:Version: 2.8.8
+:Version: 2.8.9
 :Homepage: https://github.com/handley-lab/anesthetic
 :Documentation: http://anesthetic.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/anesthetic/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/anesthetic/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/anesthetic/branch/master/graph/badge.svg
```

### Comparing `anesthetic-2.8.8/anesthetic/__init__.py` & `anesthetic-2.8.9/anesthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/_code_utils.py` & `anesthetic-2.8.9/anesthetic/_code_utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/_format.py` & `anesthetic-2.8.9/anesthetic/_format.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/boundary.py` & `anesthetic-2.8.9/anesthetic/boundary.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/convert.py` & `anesthetic-2.8.9/anesthetic/convert.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/examples/perfect_ns.py` & `anesthetic-2.8.9/anesthetic/examples/perfect_ns.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/examples/utils.py` & `anesthetic-2.8.9/anesthetic/examples/utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/gui/plot.py` & `anesthetic-2.8.9/anesthetic/gui/plot.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/gui/widgets.py` & `anesthetic-2.8.9/anesthetic/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/kde.py` & `anesthetic-2.8.9/anesthetic/kde.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/labelled_pandas.py` & `anesthetic-2.8.9/anesthetic/labelled_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/plot.py` & `anesthetic-2.8.9/anesthetic/plot.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/plotting/_core.py` & `anesthetic-2.8.9/anesthetic/plotting/_core.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/plotting/_matplotlib/__init__.py` & `anesthetic-2.8.9/anesthetic/plotting/_matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/plotting/_matplotlib/boxplot.py` & `anesthetic-2.8.9/anesthetic/plotting/_matplotlib/boxplot.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/plotting/_matplotlib/core.py` & `anesthetic-2.8.9/anesthetic/plotting/_matplotlib/core.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/plotting/_matplotlib/hist.py` & `anesthetic-2.8.9/anesthetic/plotting/_matplotlib/hist.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/read/chain.py` & `anesthetic-2.8.9/anesthetic/read/chain.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/read/cobaya.py` & `anesthetic-2.8.9/anesthetic/read/cobaya.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/read/csv.py` & `anesthetic-2.8.9/anesthetic/read/csv.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/read/getdist.py` & `anesthetic-2.8.9/anesthetic/read/getdist.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/read/hdf.py` & `anesthetic-2.8.9/anesthetic/read/hdf.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/read/multinest.py` & `anesthetic-2.8.9/anesthetic/read/multinest.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/read/nestedfit.py` & `anesthetic-2.8.9/anesthetic/read/nestedfit.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/read/polychord.py` & `anesthetic-2.8.9/anesthetic/read/polychord.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/read/ultranest.py` & `anesthetic-2.8.9/anesthetic/read/ultranest.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/samples.py` & `anesthetic-2.8.9/anesthetic/samples.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,16 +170,19 @@
                 "\'hist_1d\' is the appropriate keyword for anesthetic. "
                 "Your plots may look odd if you use this argument."
                 )
 
         for x, ax in axes.items():
             if x in self and kwargs['kind'] is not None:
                 xlabel = self.get_label(x)
-                self[x].plot(ax=ax, xlabel=xlabel, logx=x in logx,
-                             *args, **kwargs)
+                if np.isinf(self[x]).any():
+                    warnings.warn(f"column {x} has inf values.")
+                selfx = self[x].replace([-np.inf, np.inf], np.nan)
+                selfx.plot(ax=ax, xlabel=xlabel, logx=x in logx,
+                           *args, **kwargs)
                 ax.set_xlabel(xlabel)
             else:
                 ax.plot([], [])
 
         return axes
 
     def plot_2d(self, axes=None, *args, **kwargs):
@@ -235,14 +238,17 @@
 
                 - 'kde_1d': 1d kde plots down the diagonal
                 - 'kde_2d': 2d kde plots in lower triangle
                 - 'kde': 1d & 2d kde plots in lower & diagonal
                 - 'hist_1d': 1d histograms down the diagonal
                 - 'hist_2d': 2d histograms in lower triangle
                 - 'hist': 1d & 2d histograms in lower & diagonal
+                - 'scatter_2d': 2d scatter in lower triangle
+                - 'scatter': 1d histograms down diagonal
+                             & 2d scatter in lower triangle
 
             Feel free to add your own to this list!
             Default:
             {'diagonal': 'kde_1d', 'lower': 'kde_2d', 'upper':'scatter_2d'}
 
         diagonal_kwargs, lower_kwargs, upper_kwargs : dict, optional
             kwargs for the diagonal (1D)/lower or upper (2D) plots. This is
@@ -333,24 +339,32 @@
                             "\'hist_1d\' and \'hist_2d\' are the appropriate "
                             "keywords for anesthetic. Your plots may look "
                             "odd if you use this argument."
                             )
                     if x in self and y in self and lkwargs['kind'] is not None:
                         xlabel = self.get_label(x)
                         ylabel = self.get_label(y)
+                        if np.isinf(self[x]).any():
+                            warnings.warn(f"column {x} has inf values.")
                         if x == y:
-                            self[x].plot(ax=ax.twin, xlabel=xlabel,
-                                         logx=x in logx,
-                                         *args, **lkwargs)
+                            selfx = self[x].replace([-np.inf, np.inf], np.nan)
+                            selfx.plot(ax=ax.twin, xlabel=xlabel,
+                                       logx=x in logx,
+                                       *args, **lkwargs)
                             ax.set_xlabel(xlabel)
                             ax.set_ylabel(ylabel)
                         else:
-                            self.plot(x, y, ax=ax, xlabel=xlabel,
-                                      logx=x in logx, logy=y in logy,
-                                      ylabel=ylabel, *args, **lkwargs)
+                            if np.isinf(self[x]).any():
+                                warnings.warn(f"column {y} has inf values.")
+                            selfxy = self[[x, y]]
+                            selfxy = self.replace([-np.inf, np.inf], np.nan)
+                            selfxy = selfxy.dropna(axis=0)
+                            selfxy.plot(x, y, ax=ax, xlabel=xlabel,
+                                        logx=x in logx, logy=y in logy,
+                                        ylabel=ylabel, *args, **lkwargs)
                             ax.set_xlabel(xlabel)
                             ax.set_ylabel(ylabel)
                     else:
                         if x == y:
                             ax.twin.plot([], [])
                         else:
                             ax.plot([], [])
@@ -366,14 +380,16 @@
         'kde': {'diagonal': 'kde_1d', 'lower': 'kde_2d'},
         'kde_1d': {'diagonal': 'kde_1d'},
         'kde_2d': {'lower': 'kde_2d'},
         'fastkde': {'diagonal': 'fastkde_1d', 'lower': 'fastkde_2d'},
         'hist': {'diagonal': 'hist_1d', 'lower': 'hist_2d'},
         'hist_1d': {'diagonal': 'hist_1d'},
         'hist_2d': {'lower': 'hist_2d'},
+        'scatter': {'diagonal': 'hist_1d', 'lower': 'scatter_2d'},
+        'scatter_2d': {'lower': 'scatter_2d'},
     }
 
     def importance_sample(self, logL_new, action='add', inplace=False):
         """Perform importance re-weighting on the log-likelihood.
 
         Parameters
         ----------
```

### Comparing `anesthetic-2.8.8/anesthetic/scripts.py` & `anesthetic-2.8.9/anesthetic/scripts.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/utils.py` & `anesthetic-2.8.9/anesthetic/utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/weighted_labelled_pandas.py` & `anesthetic-2.8.9/anesthetic/weighted_labelled_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic/weighted_pandas.py` & `anesthetic-2.8.9/anesthetic/weighted_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/anesthetic.egg-info/PKG-INFO` & `anesthetic-2.8.9/anesthetic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anesthetic
-Version: 2.8.8
+Version: 2.8.9
 Summary: nested sampling post-processing
 Author-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>, Adam Ormondroyd <ano23@cam.ac.uk>, Harry Bevins <htjb2@cam.ac.uk>, Johannes Buchner <jbuchner@mpe.mpg.de>, Ethan Carragher <ethan.carragher@adelaide.edu.au>, Andrew Fowlie <andrew.j.fowlie@googlemail.com>, Thomas Gessey-Jones <tg400@cam.ac.uk>, Stefan Heimersheim <sh2061@ast.cam.ac.uk>, Pablo Lemos <plemos91@gmail.com>, Toby Lovick <tcl44@cam.ac.uk>, Deborah Odunuyi <debbieodunuyi@gmail.com>, Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>, Liangliang Su <liangliangsu@njnu.edu.cn>, David Yallup <david.yallup@gmail.com>, Dily Ong <dlo26@cam.ac.uk>
 Maintainer-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>
 License: MIT License
         
         Copyright (c) 2019 Will Handley
         
@@ -80,15 +80,15 @@
 Requires-Dist: getdist; extra == "all"
 Requires-Dist: tables==3.8.0; extra == "all"
 
 ===========================================
 anesthetic: nested sampling post-processing
 ===========================================
 :Authors: Will Handley and Lukas Hergt
-:Version: 2.8.8
+:Version: 2.8.9
 :Homepage: https://github.com/handley-lab/anesthetic
 :Documentation: http://anesthetic.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/anesthetic/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/anesthetic/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/anesthetic/branch/master/graph/badge.svg
```

### Comparing `anesthetic-2.8.8/anesthetic.egg-info/SOURCES.txt` & `anesthetic-2.8.9/anesthetic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/pyproject.toml` & `anesthetic-2.8.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/tests/test_convert.py` & `anesthetic-2.8.9/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/tests/test_examples.py` & `anesthetic-2.8.9/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/tests/test_gui.py` & `anesthetic-2.8.9/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/tests/test_labelled_pandas.py` & `anesthetic-2.8.9/tests/test_labelled_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/tests/test_plot.py` & `anesthetic-2.8.9/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/tests/test_reader.py` & `anesthetic-2.8.9/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/tests/test_samples.py` & `anesthetic-2.8.9/tests/test_samples.py`

 * *Files 2% similar despite different names*

```diff
@@ -414,27 +414,36 @@
     assert axes.iloc[-1, 2].get_xlabel() == '$x_2$'
 
     axes = ns[['x0', 'x1', 'x2']].drop_labels().plot_2d()
     assert axes.iloc[-1, 0].get_xlabel() == 'x0'
     assert axes.iloc[-1, 1].get_xlabel() == 'x1'
     assert axes.iloc[-1, 2].get_xlabel() == 'x2'
 
+    with pytest.warns(UserWarning):
+        axes = ns[['x0', 'logL_birth']].plot_2d()
+        axes = ns.drop_labels()[['x0', 'logL_birth']].plot_2d()
+
 
 def test_plot_1d_no_axes():
     np.random.seed(3)
     ns = read_chains('./tests/example_data/pc')
     axes = ns[['x0', 'x1', 'x2']].plot_1d()
     assert axes.iloc[0].get_xlabel() == '$x_0$'
     assert axes.iloc[1].get_xlabel() == '$x_1$'
     assert axes.iloc[2].get_xlabel() == '$x_2$'
     axes = ns[['x0', 'x1', 'x2']].drop_labels().plot_1d()
     assert axes.iloc[0].get_xlabel() == 'x0'
     assert axes.iloc[1].get_xlabel() == 'x1'
     assert axes.iloc[2].get_xlabel() == 'x2'
 
+    with pytest.warns(UserWarning):
+        axes = ns.plot_1d()
+        axes = ns[['x0', 'logL_birth']].plot_1d()
+        axes = ns.drop_labels()[['x0', 'logL_birth']].plot_1d()
+
 
 @pytest.mark.parametrize('kind', ['kde', 'hist', skipif_no_fastkde('fastkde')])
 def test_plot_logscale_1d(kind):
     ns = read_chains('./tests/example_data/pc')
     params = ['x0', 'x1', 'x2', 'x3', 'x4']
 
     # 1d
@@ -1209,30 +1218,14 @@
     assert x2 < +1
     ax = ns.plot_1d('x0', kind='hist_1d', bins=np.linspace(-1, 1, 11))
     x1, x2 = ax['x0'].get_xlim()
     assert x1 <= -1
     assert x2 >= +1
 
 
-def test_contour_plot_2d_nan():
-    """Contour plots with nans arising from issue #96"""
-    np.random.seed(3)
-    ns = read_chains('./tests/example_data/pc')
-
-    ns.loc[:9, ('x0', '$x_0$')] = np.nan
-    with pytest.raises((np.linalg.LinAlgError, RuntimeError, ValueError)):
-        ns.plot_2d(['x0', 'x1'])
-
-    # Check this error is removed in the case of zero weights
-    weights = ns.get_weights()
-    weights[:10] = 0
-    ns.set_weights(weights, inplace=True)
-    ns.plot_2d(['x0', 'x1'])
-
-
 def test_compute_insertion():
     np.random.seed(3)
     ns = read_chains('./tests/example_data/pc')
     assert 'insertion' not in ns
     ns._compute_insertion_indexes()
     assert 'insertion' in ns
```

### Comparing `anesthetic-2.8.8/tests/test_scripts.py` & `anesthetic-2.8.9/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/tests/test_utils.py` & `anesthetic-2.8.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/tests/test_weighted_labelled_pandas.py` & `anesthetic-2.8.9/tests/test_weighted_labelled_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.8/tests/test_weighted_pandas.py` & `anesthetic-2.8.9/tests/test_weighted_pandas.py`

 * *Files identical despite different names*

