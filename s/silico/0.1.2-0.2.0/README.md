# Comparing `tmp/silico-0.1.2.tar.gz` & `tmp/silico-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silico-0.1.2.tar", last modified: Mon Mar  7 17:24:56 2022, max compression
+gzip compressed data, was "silico-0.2.0.tar", last modified: Wed Apr 24 09:38:45 2024, max compression
```

## Comparing `silico-0.1.2.tar` & `silico-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 17:24:56.748844 silico-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-03-07 17:24:44.000000 silico-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2022-03-07 17:24:56.748844 silico-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-03-07 17:24:44.000000 silico-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-03-07 17:24:56.748844 silico-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1540 2022-03-07 17:24:44.000000 silico-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 17:24:56.748844 silico-0.1.2/silico/
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-03-07 17:24:44.000000 silico-0.1.2/silico/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-03-07 17:24:44.000000 silico-0.1.2/silico/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3803 2022-03-07 17:24:44.000000 silico-0.1.2/silico/analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)    13468 2022-03-07 17:24:44.000000 silico-0.1.2/silico/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3554 2022-03-07 17:24:44.000000 silico-0.1.2/silico/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      888 2022-03-07 17:24:44.000000 silico-0.1.2/silico/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     4121 2022-03-07 17:24:44.000000 silico-0.1.2/silico/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     1957 2022-03-07 17:24:44.000000 silico-0.1.2/silico/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 17:24:56.748844 silico-0.1.2/silico.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2022-03-07 17:24:56.000000 silico-0.1.2/silico.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      325 2022-03-07 17:24:56.000000 silico-0.1.2/silico.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-07 17:24:56.000000 silico-0.1.2/silico.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-03-07 17:24:56.000000 silico-0.1.2/silico.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-03-07 17:24:56.000000 silico-0.1.2/silico.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:38:45.195422 silico-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-24 09:38:34.000000 silico-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-24 09:38:45.195422 silico-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-24 09:38:34.000000 silico-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-24 09:38:45.195422 silico-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-24 09:38:34.000000 silico-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:38:45.195422 silico-0.2.0/silico/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-24 09:38:34.000000 silico-0.2.0/silico/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-24 09:38:34.000000 silico-0.2.0/silico/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-24 09:38:34.000000 silico-0.2.0/silico/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13593 2024-04-24 09:38:34.000000 silico-0.2.0/silico/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-24 09:38:34.000000 silico-0.2.0/silico/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-24 09:38:34.000000 silico-0.2.0/silico/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-24 09:38:34.000000 silico-0.2.0/silico/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-24 09:38:34.000000 silico-0.2.0/silico/ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-24 09:38:34.000000 silico-0.2.0/silico/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-24 09:38:34.000000 silico-0.2.0/silico/urinal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:38:45.195422 silico-0.2.0/silico.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-24 09:38:45.000000 silico-0.2.0/silico.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-24 09:38:45.000000 silico-0.2.0/silico.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 09:38:45.000000 silico-0.2.0/silico.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-24 09:38:45.000000 silico-0.2.0/silico.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-24 09:38:45.000000 silico-0.2.0/silico.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 09:38:45.000000 silico-0.2.0/silico.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:38:45.195422 silico-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-24 09:38:34.000000 silico-0.2.0/tests/test_root.py
```

### Comparing `silico-0.1.2/LICENSE.txt` & `silico-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `silico-0.1.2/setup.py` & `silico-0.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,22 +22,28 @@
           'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
       ],
       description='Python package to handle in silico experiments',
+      entry_points={
+          'console_scripts': [
+              'silico=silico.cli:cli',
+          ],
+
+      },
       extras_require={
           "docs": ["nbsphinx", "sphinx-rtd-theme", "IPython"],
           "test": ["pytest"],
           "progress": ["tqdm"]
       },
       keywords=[],
       long_description=long_description,
       long_description_content_type='text/markdown',
       name='silico',
       packages=find_packages(include=['silico'], exclude=["demos", "tests", "docs"]),
       install_requires=["numpy", "pandas", "scipy", "scikit-learn", "click", "tqdm"],
       url='https://github.com/Dih5/silico',
-      version='0.1.2',
+      version='0.2.0',
 
       )
```

### Comparing `silico-0.1.2/silico/analysis.py` & `silico-0.2.0/silico/analysis.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 import numpy as np
 from scipy.stats import ttest_rel
 import pandas as pd
 
 
 def paired_t_test(df, col_left, col_right, common_col="seed"):
     """
+    Perform and summarize unilateral t-test to decide a difference between columns is significant.
 
-    Considered calling .round(5) on output for clearer reading.
+    Considered calling .round(5) or alike on output for clearer reading.
 
     Args:
         df (pd.DataFrame): The results of the experiment.
-        col_left: Identifier of the column
-        col_right:
-        common_col: Identifier of the column indexing the repetitions of the experiments.
+        col_left (str): Name of the "left" column to compare
+        col_right (str): Name of the "left" column to compare
+        common_col (str): Identifier of the column indexing the repetitions of the experiments.
 
     Returns:
-        pd.Dataframe: Dataframe with the mean values of the left and right column, as well as p-values of unilateral
-                      tests.
+        pd.Dataframe: Dataframe with the mean values of the left and right column, as well as the p-values of unilateral
+                      tests. p-value-less corresponds to the test with alternative hypothesis col_left < col_right.
 
     """
     # TODO: Single level not considered
     group_cols = [level.name for level in df.index.levels]
     if common_col not in group_cols:
         raise ValueError("Common column %s not found." % common_col)
     for c in [col_left, col_right]:
@@ -30,15 +31,15 @@
             raise ValueError("Column %s not found" % c)
     group_cols.remove(common_col)
 
     df_eval = df.groupby(group_cols).agg(list)
 
     df_out = pd.concat(
         (
-            df.groupby(group_cols).agg("mean"),
+            df.groupby(group_cols)[[col_left, col_right]].agg("mean"),
             pd.Series(
                 df_eval.apply(
                     lambda row: ttest_rel(
                         row[col_left], row[col_right], alternative="less"
                     ).pvalue,
                     axis=1,
                 ),
```

### Comparing `silico-0.1.2/silico/base.py` & `silico-0.2.0/silico/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,38 +6,28 @@
 import os
 import pickle
 from glob import glob
 from datetime import datetime
 from multiprocessing import Pool
 import traceback
 
-from functools import reduce
-
 try:
     import pandas as pd
 except ImportError:
     pd = None
 
-from .common import is_notebook
-
 try:
-    if not is_notebook():
-        from tqdm import tqdm
-    else:
-        from tqdm.notebook import tqdm
+    from tqdm.auto import tqdm
 except ImportError:
     def tqdm(*args, **kwargs):
         if args:
             return args[0]
         return kwargs["iterable"]
 
-
-def prod(i):
-    """Product of a list of numbers"""
-    return reduce(lambda x, y: x * y, i, 1)
+from .common import prod, set_kwargs
 
 
 def _hash_function(w):
     """Hash function to provide a unique (negligible collision) string identifier from a dict of parameters"""
     h = hashlib.md5(w)
     return base64.b64encode(h.digest())[:12].decode("utf-8").replace("/", "_")
 
@@ -179,14 +169,16 @@
             f (callable): A function which maps variables names into results, which should be a dict.
             store (str): A path to store the results.
             base_name (str): Prefix for the file name. If None, a name will be extracted from f.
             add_stats (bool): Whether to add running information to the results. If f's output is not a dict, this
                               will fail.
             strategy (str): A method defining how the parameter space is explore. Available options are:
                             - "grid": Explore a grid in order (cartesian product)
+                            - "urinal": Explore the grid picking point with the urinal convention (as far as possible
+                                        from already explored points).
                             - "star": Consider only variations of each of the parameters. The "standard" point can
                                       be defined with the mid_point parameter.
             mid_point (dict of str): A mapping of parameters to their "default" values. Used if strategy is "star". The
                                      mid_point must be in the grid.
 
         """
         self.variables = [implicit_variable_cast(v) for v in variables]
@@ -194,25 +186,27 @@
         self.store = store
 
         self.base_name = base_name
         self.add_stats = add_stats
 
         self.strategy = strategy
 
-        if strategy == "grid":
+        if strategy in ["grid", "urinal"]:
             self._len = prod(len(v) for v in self.variables)
         elif strategy == "star":
             if mid_point is not None:
                 self.mid_point = mid_point
             else:
                 warnings.warn("Not specifying a mid_point uses the median if available. ")
                 self.mid_point = {v.name: v.get_standard() for v in self.variables}
 
             # Sum of lengths, but do not repeat the mid_point
             self._len = sum(len(v) for v in self.variables) - len(self.variables) + 1
+        else:
+            raise ValueError("Invalid strategy")
 
         ensure_dir_exists(store)
 
     def __len__(self):
         return self._len
 
     def iter_values(self):
@@ -224,14 +218,21 @@
         elif self.strategy == "star":
             mid_point = self.mid_point if self.mid_point is not None else {}
             yield mid_point
             for v in self.variables:
                 for value in v.iter_values():
                     if value != mid_point[v.name]:  # Do not repeat mid point
                         yield {**mid_point, **{v.name: value}}
+        elif self.strategy == "urinal":
+            from .urinal import urinal_iteration
+            items = [list(v.iter_values()) for v in self.variables]
+
+            for indices in urinal_iteration([len(l) for l in items]):
+                yield {name: values[i] for name, values, i in zip(names, items, indices)}
+
 
         else:
             raise ValueError("Invalid value for parameter strategy.")
 
     def _run_kwargs(self, **kwargs):
         """Helper pickleable function"""
         try:
@@ -355,33 +356,23 @@
             for file in glob(os.path.join(self.store, "*.pkl")):
                 try:
                     os.remove(file)
                 except FileNotFoundError:
                     pass
 
 
-def _set_kwarg(f, fixed_kwargs):
-    """Closure of a function fixing a kwarg"""
-
-    def f2(*args, **kwargs):
-        fixed_kwargs2 = {k: v for k, v in fixed_kwargs.items() if k not in kwargs}
-        return f(*args, **fixed_kwargs2, **kwargs)
-
-    return f2
-
-
 class SubExperiment(Experiment):
     """An restriction of an experiment, where some of its variables are fixed"""
 
     def __init__(self, original, fixed):
         """
 
         Args:
             original (Experiment): The original experiment.
             fixed (callable): A mapping from variable names to their fixed values.
 
         """
 
         variables = [a for a in original.variables if a.name not in fixed]
-        f = _set_kwarg(original.f, fixed)
+        f = set_kwargs(original.f, fixed)
         store = original.store
         super().__init__(variables, f, store)
```

### Comparing `silico-0.1.2/silico/cli.py` & `silico-0.2.0/silico/cli.py`

 * *Files identical despite different names*

### Comparing `silico-0.1.2/silico/common.py` & `silico-0.2.0/silico/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 import warnings
 
+# prod
+try:
+    from math import prod
+except ImportError:
+    from functools import reduce
+    from operator import mul
+
+
+    def prod(i):
+        """Product of a list of numbers"""
+        return reduce(mul, i, 1)
+
 
 def is_notebook():
     """Detect if running in a notebook"""
     # Not sure this covers
     try:
         ipython_module = get_ipython().__module__
         if ipython_module in ['ipykernel.zmqshell', 'google.colab._shell']:
```

### Comparing `silico-0.1.2/silico/metrics.py` & `silico-0.2.0/silico/metrics.py`

 * *Files identical despite different names*

### Comparing `silico-0.1.2/silico/plot.py` & `silico-0.2.0/silico/plot.py`

 * *Files identical despite different names*

