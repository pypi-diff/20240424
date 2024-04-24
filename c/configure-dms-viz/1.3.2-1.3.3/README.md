# Comparing `tmp/configure_dms_viz-1.3.2.tar.gz` & `tmp/configure_dms_viz-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configure_dms_viz-1.3.2.tar", max compression
+gzip compressed data, was "configure_dms_viz-1.3.3.tar", max compression
```

## Comparing `configure_dms_viz-1.3.2.tar` & `configure_dms_viz-1.3.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1095 2024-04-05 20:19:22.027565 configure_dms_viz-1.3.2/LICENSE
--rw-r--r--   0        0        0      621 2024-04-05 20:19:22.027565 configure_dms_viz-1.3.2/README.md
--rw-r--r--   0        0        0        0 2024-04-05 20:19:22.027565 configure_dms_viz-1.3.2/configure_dms_viz/__init__.py
--rwxr-xr-x   0        0        0    38645 2024-04-05 20:19:22.027565 configure_dms_viz-1.3.2/configure_dms_viz/configure_dms_viz.py
--rw-r--r--   0        0        0     8500 2024-04-05 20:19:22.027565 configure_dms_viz-1.3.2/configure_dms_viz/pdb_utils.py
--rw-r--r--   0        0        0     1120 2024-04-05 20:19:22.027565 configure_dms_viz-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 configure_dms_viz-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-04-24 21:35:20.863707 configure_dms_viz-1.3.3/LICENSE
+-rw-r--r--   0        0        0     9172 2024-04-24 21:35:20.863707 configure_dms_viz-1.3.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-24 21:35:20.863707 configure_dms_viz-1.3.3/configure_dms_viz/__init__.py
+-rwxr-xr-x   0        0        0    38948 2024-04-24 21:35:20.863707 configure_dms_viz-1.3.3/configure_dms_viz/configure_dms_viz.py
+-rw-r--r--   0        0        0     8500 2024-04-24 21:35:20.863707 configure_dms_viz-1.3.3/configure_dms_viz/pdb_utils.py
+-rw-r--r--   0        0        0     1454 2024-04-24 21:35:20.867707 configure_dms_viz-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0    10199 1970-01-01 00:00:00.000000 configure_dms_viz-1.3.3/PKG-INFO
```

### Comparing `configure_dms_viz-1.3.2/LICENSE` & `configure_dms_viz-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `configure_dms_viz-1.3.2/configure_dms_viz/configure_dms_viz.py` & `configure_dms_viz-1.3.3/configure_dms_viz/configure_dms_viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -425,14 +425,20 @@
 
     # Make sure the chain names are valid and not just whitespace
     if not included_chains.strip():
         included_chains = "polymer"
     if not excluded_chains.strip():
         excluded_chains = "none"
 
+    # Make sure that there is no overlap between the included and excluded chains
+    if set(included_chains.split(" ")) & set(excluded_chains.split(" ")):
+        raise ValueError(
+            "The included and excluded chains cannot have any overlap. Please remove the overlapping chains."
+        )
+
     # Check that the necessary columns are present in the mut_metric dataframe and format
     mut_metric_df = format_mutation_data(
         mut_metric_df, metric_col, condition_col, alphabet
     )
 
     # If there is no sitemap dataframe, create a default one
     if sitemap_df is None:
```

### Comparing `configure_dms_viz-1.3.2/configure_dms_viz/pdb_utils.py` & `configure_dms_viz-1.3.3/configure_dms_viz/pdb_utils.py`

 * *Files identical despite different names*

### Comparing `configure_dms_viz-1.3.2/pyproject.toml` & `configure_dms_viz-1.3.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 [tool.poetry]
 name = "configure-dms-viz"
-version = "1.3.2"
+version = "1.3.3"
 description = "Configure your data for visualization with dms-viz.github.io"
 authors = ["Will Hannon <hannonww@gmail.com>"]
+maintainers = ["Will Hannon <hannonww@gmail.com>"]
 license = "MIT"
 readme = "README.md"
+homepage = "https://github.com/dms-viz"
+repository = "https://github.com/dms-viz/configure_dms_viz"
+documentation = "https://dms-viz.github.io/dms-viz-docs/"
+keywords = [
+    "deep mutational scanning",
+    "interactive protein structure",
+    "dms-viz",
+    "dms",
+    "protein",
+]
 packages = [{ include = "configure_dms_viz" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.1.6"
 pandas = ">=2.0.0"
 biopython = ">=1.0"
```

