# Comparing `tmp/somacore-1.0.8.tar.gz` & `tmp/somacore-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somacore-1.0.8.tar", last modified: Mon Feb 26 20:39:46 2024, max compression
+gzip compressed data, was "somacore-1.0.9.tar", last modified: Mon Mar 11 20:24:03 2024, max compression
```

## Comparing `somacore-1.0.8.tar` & `somacore-1.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:39:46.755416 somacore-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-02-26 20:39:34.000000 somacore-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-26 20:39:34.000000 somacore-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-02-26 20:39:46.755416 somacore-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-02-26 20:39:34.000000 somacore-1.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:39:46.751416 somacore-1.0.8/python-spec/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-02-26 20:39:34.000000 somacore-1.0.8/python-spec/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:39:46.751416 somacore-1.0.8/python-spec/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:39:46.751416 somacore-1.0.8/python-spec/src/somacore/
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-02-26 20:39:34.000000 somacore-1.0.8/python-spec/src/somacore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-02-26 20:39:34.000000 somacore-1.0.8/python-spec/src/somacore/_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-26 20:39:46.000000 somacore-1.0.8/python-spec/src/somacore/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-02-26 20:39:34.000000 somacore-1.0.8/python-spec/src/somacore/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-02-26 20:39:34.000000 somacore-1.0.8/python-spec/src/somacore/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    19708 2024-02-26 20:39:34.000000 somacore-1.0.8/python-spec/src/somacore/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:39:46.755416 somacore-1.0.8/python-spec/src/somacore/ephemeral/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-26 20:39:34.000000 somacore-1.0.8/python-spec/src/somacore/ephemeral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-02-26 20:39:34.000000 somacore-1.0.8/python-spec/src/somacore/ephemeral/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-02-26 20:39:34.000000 somacore-1.0.8/python-spec/src/somacore/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-02-26 20:39:34.000000 somacore-1.0.8/python-spec/src/somacore/measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-02-26 20:39:34.000000 somacore-1.0.8/python-spec/src/somacore/options.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-26 20:39:34.000000 somacore-1.0.8/python-spec/src/somacore/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:39:46.755416 somacore-1.0.8/python-spec/src/somacore/query/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-26 20:39:34.000000 somacore-1.0.8/python-spec/src/somacore/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-02-26 20:39:34.000000 somacore-1.0.8/python-spec/src/somacore/query/_eager_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-02-26 20:39:34.000000 somacore-1.0.8/python-spec/src/somacore/query/_fast_csr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-02-26 20:39:34.000000 somacore-1.0.8/python-spec/src/somacore/query/axis.py
--rw-r--r--   0 runner    (1001) docker     (127)    26540 2024-02-26 20:39:34.000000 somacore-1.0.8/python-spec/src/somacore/query/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-02-26 20:39:34.000000 somacore-1.0.8/python-spec/src/somacore/query/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-02-26 20:39:34.000000 somacore-1.0.8/python-spec/src/somacore/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 20:39:46.755416 somacore-1.0.8/python-spec/src/somacore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-02-26 20:39:46.000000 somacore-1.0.8/python-spec/src/somacore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 20:39:46.755416 somacore-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:24:03.346314 somacore-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-11 20:23:54.000000 somacore-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-11 20:23:54.000000 somacore-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-11 20:24:03.346314 somacore-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-03-11 20:23:54.000000 somacore-1.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:24:03.342314 somacore-1.0.9/python-spec/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-11 20:23:54.000000 somacore-1.0.9/python-spec/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:24:03.338314 somacore-1.0.9/python-spec/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:24:03.342314 somacore-1.0.9/python-spec/src/somacore/
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-03-11 20:23:54.000000 somacore-1.0.9/python-spec/src/somacore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-03-11 20:23:54.000000 somacore-1.0.9/python-spec/src/somacore/_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-11 20:24:03.000000 somacore-1.0.9/python-spec/src/somacore/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-03-11 20:23:54.000000 somacore-1.0.9/python-spec/src/somacore/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-03-11 20:23:54.000000 somacore-1.0.9/python-spec/src/somacore/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19708 2024-03-11 20:23:54.000000 somacore-1.0.9/python-spec/src/somacore/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:24:03.342314 somacore-1.0.9/python-spec/src/somacore/ephemeral/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-11 20:23:54.000000 somacore-1.0.9/python-spec/src/somacore/ephemeral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-03-11 20:23:54.000000 somacore-1.0.9/python-spec/src/somacore/ephemeral/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-03-11 20:23:54.000000 somacore-1.0.9/python-spec/src/somacore/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-03-11 20:23:54.000000 somacore-1.0.9/python-spec/src/somacore/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-03-11 20:23:54.000000 somacore-1.0.9/python-spec/src/somacore/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-11 20:23:54.000000 somacore-1.0.9/python-spec/src/somacore/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:24:03.342314 somacore-1.0.9/python-spec/src/somacore/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-11 20:23:54.000000 somacore-1.0.9/python-spec/src/somacore/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-03-11 20:23:54.000000 somacore-1.0.9/python-spec/src/somacore/query/_eager_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-03-11 20:23:54.000000 somacore-1.0.9/python-spec/src/somacore/query/_fast_csr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-03-11 20:23:54.000000 somacore-1.0.9/python-spec/src/somacore/query/axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26540 2024-03-11 20:23:54.000000 somacore-1.0.9/python-spec/src/somacore/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-03-11 20:23:54.000000 somacore-1.0.9/python-spec/src/somacore/query/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-03-11 20:23:54.000000 somacore-1.0.9/python-spec/src/somacore/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:24:03.346314 somacore-1.0.9/python-spec/src/somacore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-11 20:24:03.000000 somacore-1.0.9/python-spec/src/somacore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 20:24:03.346314 somacore-1.0.9/setup.cfg
```

### Comparing `somacore-1.0.8/LICENSE` & `somacore-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `somacore-1.0.8/PKG-INFO` & `somacore-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somacore
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python-language API specification and base utilities for implementation of the SOMA system.
 Project-URL: repository, https://github.com/single-cell-data/SOMA.git
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: anndata
```

### Comparing `somacore-1.0.8/pyproject.toml` & `somacore-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `somacore-1.0.8/python-spec/README.md` & `somacore-1.0.9/python-spec/README.md`

 * *Files identical despite different names*

### Comparing `somacore-1.0.8/python-spec/src/somacore/__init__.py` & `somacore-1.0.9/python-spec/src/somacore/__init__.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.8/python-spec/src/somacore/_mixin.py` & `somacore-1.0.9/python-spec/src/somacore/_mixin.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.8/python-spec/src/somacore/base.py` & `somacore-1.0.9/python-spec/src/somacore/base.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.8/python-spec/src/somacore/collection.py` & `somacore-1.0.9/python-spec/src/somacore/collection.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.8/python-spec/src/somacore/data.py` & `somacore-1.0.9/python-spec/src/somacore/data.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.8/python-spec/src/somacore/ephemeral/collections.py` & `somacore-1.0.9/python-spec/src/somacore/ephemeral/collections.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.8/python-spec/src/somacore/experiment.py` & `somacore-1.0.9/python-spec/src/somacore/experiment.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.8/python-spec/src/somacore/measurement.py` & `somacore-1.0.9/python-spec/src/somacore/measurement.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.8/python-spec/src/somacore/options.py` & `somacore-1.0.9/python-spec/src/somacore/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,11 +170,12 @@
 """A sequence of coordinate ranges for reading dense dataframes."""
 
 SparseNDCoord = Union[
     None,
     ValSliceOrSequence[int],
     npt.NDArray[np.integer],
     pa.IntegerArray,
+    pa.ChunkedArray,
 ]
 """A single coordinate range for one dimension of a sparse nd-array."""
 SparseNDCoords = Sequence[SparseNDCoord]
 """A sequence of coordinate ranges for reading sparse ndarrays."""
```

### Comparing `somacore-1.0.8/python-spec/src/somacore/query/_eager_iter.py` & `somacore-1.0.9/python-spec/src/somacore/query/_eager_iter.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.8/python-spec/src/somacore/query/_fast_csr.py` & `somacore-1.0.9/python-spec/src/somacore/query/_fast_csr.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.8/python-spec/src/somacore/query/axis.py` & `somacore-1.0.9/python-spec/src/somacore/query/axis.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.8/python-spec/src/somacore/query/query.py` & `somacore-1.0.9/python-spec/src/somacore/query/query.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.8/python-spec/src/somacore/query/types.py` & `somacore-1.0.9/python-spec/src/somacore/query/types.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.8/python-spec/src/somacore/types.py` & `somacore-1.0.9/python-spec/src/somacore/types.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.8/python-spec/src/somacore.egg-info/SOURCES.txt` & `somacore-1.0.9/python-spec/src/somacore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

