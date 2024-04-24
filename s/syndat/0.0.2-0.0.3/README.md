# Comparing `tmp/syndat-0.0.2.tar.gz` & `tmp/syndat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syndat-0.0.2.tar", last modified: Mon Jan 29 12:30:33 2024, max compression
+gzip compressed data, was "syndat-0.0.3.tar", last modified: Wed Apr 24 13:58:36 2024, max compression
```

## Comparing `syndat-0.0.2.tar` & `syndat-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 12:30:33.767135 syndat-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-01-29 12:30:23.000000 syndat-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-01-29 12:30:33.767135 syndat-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-01-29 12:30:23.000000 syndat-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 12:30:33.767135 syndat-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-01-29 12:30:27.000000 syndat-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 12:30:33.767135 syndat-0.0.2/syndat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 12:30:23.000000 syndat-0.0.2/syndat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-01-29 12:30:23.000000 syndat-0.0.2/syndat/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-01-29 12:30:23.000000 syndat-0.0.2/syndat/quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-01-29 12:30:23.000000 syndat-0.0.2/syndat/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 12:30:33.767135 syndat-0.0.2/syndat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-01-29 12:30:33.000000 syndat-0.0.2/syndat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-29 12:30:33.000000 syndat-0.0.2/syndat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 12:30:33.000000 syndat-0.0.2/syndat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-29 12:30:33.000000 syndat-0.0.2/syndat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 12:30:33.767135 syndat-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-01-29 12:30:23.000000 syndat-0.0.2/tests/test_jsd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:58:36.793765 syndat-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-24 13:58:28.000000 syndat-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-24 13:58:36.793765 syndat-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-24 13:58:28.000000 syndat-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:58:36.793765 syndat-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-24 13:58:34.000000 syndat-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:58:36.793765 syndat-0.0.3/syndat/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 13:58:28.000000 syndat-0.0.3/syndat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-24 13:58:28.000000 syndat-0.0.3/syndat/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-24 13:58:28.000000 syndat-0.0.3/syndat/quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-24 13:58:28.000000 syndat-0.0.3/syndat/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:58:36.793765 syndat-0.0.3/syndat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-24 13:58:36.000000 syndat-0.0.3/syndat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-24 13:58:36.000000 syndat-0.0.3/syndat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:58:36.000000 syndat-0.0.3/syndat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 13:58:36.000000 syndat-0.0.3/syndat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:58:36.793765 syndat-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-24 13:58:28.000000 syndat-0.0.3/tests/test_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-24 13:58:28.000000 syndat-0.0.3/tests/test_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-24 13:58:28.000000 syndat-0.0.3/tests/test_jsd.py
```

### Comparing `syndat-0.0.2/LICENSE` & `syndat-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `syndat-0.0.2/README.md` & `syndat-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -14,31 +14,29 @@
 ## Quality metrics
 
 Compute data quality metrics by comparing real and synthetic data in terms of their separation complexity, 
 distribution similarity or pairwise feature correlations:
 
 ```python
 import pandas as pd
-from syndat import quality
-
+import syndat
 real = pd.read_csv("real.csv")
 synthetic = pd.read_csv("synthetic.csv")
 
-jsd = quality.get_jsd(real, synthetic)
-auc = quality.get_auc(real, synthetic)
-norm = quality.get_correlation_quotient(real, synthetic)
+jsd = syndat.quality.jsd(real, synthetic)
+auc = syndat.quality.auc(real, synthetic)
+norm = syndat.quality.correlation(real, synthetic)
 ```
 
 ## Visualization
 
 Visualize real vs. synthetic data distributions and summary statistics for each feature:
 
 ```python
 import pandas as pd
-from syndat import visualization
-
+import syndat
 real = pd.read_csv("real.csv")
 synthetic = pd.read_csv("synthetic.csv")
 
-visualization.plot_distributions(real, synthetic, store_destination="results/plots")
+syndat.visualization.plot_distributions(real, synthetic, store_destination="results/plots")
 ```
```

### Comparing `syndat-0.0.2/setup.py` & `syndat-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 setup(
     name='syndat',
-    version='v0.0.2',
+    version='v0.0.3',
     packages=['syndat'],
     url='https://github.com/SCAI-BIO/syndat',
     license='CC BY-NC-ND 4.0.',
     author='Tim Adams',
     author_email='tim.adams@scai.fraunhofer.de',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
```

