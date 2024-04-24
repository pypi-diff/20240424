# Comparing `tmp/waylay_ml_adapter_sklearn-0.0.2.tar.gz` & `tmp/waylay_ml_adapter_sklearn-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_ml_adapter_sklearn-0.0.2.tar", last modified: Wed Apr 17 09:14:51 2024, max compression
+gzip compressed data, was "waylay_ml_adapter_sklearn-0.0.3.tar", last modified: Wed Apr 24 15:25:43 2024, max compression
```

## Comparing `waylay_ml_adapter_sklearn-0.0.2.tar` & `waylay_ml_adapter_sklearn-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:51.709236 waylay_ml_adapter_sklearn-0.0.2/
--rw-r--r--   0 thomas     (502) staff       (20)      355 2024-04-17 09:14:51.708830 waylay_ml_adapter_sklearn-0.0.2/PKG-INFO
--rw-r--r--   0 thomas     (502) staff       (20)       60 2024-01-25 17:01:42.000000 waylay_ml_adapter_sklearn-0.0.2/README.md
--rw-r--r--   0 thomas     (502) staff       (20)     1001 2024-04-17 08:27:35.000000 waylay_ml_adapter_sklearn-0.0.2/pyproject.toml
--rw-r--r--   0 thomas     (502) staff       (20)       38 2024-04-17 09:14:51.709282 waylay_ml_adapter_sklearn-0.0.2/setup.cfg
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:51.703077 waylay_ml_adapter_sklearn-0.0.2/src/
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:51.702836 waylay_ml_adapter_sklearn-0.0.2/src/ml_adapter/
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:51.704696 waylay_ml_adapter_sklearn-0.0.2/src/ml_adapter/sklearn/
--rw-r--r--   0 thomas     (502) staff       (20)     1475 2024-04-17 08:27:35.000000 waylay_ml_adapter_sklearn-0.0.2/src/ml_adapter/sklearn/__init__.py
--rw-r--r--   0 thomas     (502) staff       (20)        0 2024-01-25 17:02:04.000000 waylay_ml_adapter_sklearn-0.0.2/src/ml_adapter/sklearn/py.typed
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-17 09:14:51.708418 waylay_ml_adapter_sklearn-0.0.2/src/waylay_ml_adapter_sklearn.egg-info/
--rw-r--r--   0 thomas     (502) staff       (20)      355 2024-04-17 09:14:51.000000 waylay_ml_adapter_sklearn-0.0.2/src/waylay_ml_adapter_sklearn.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (502) staff       (20)      355 2024-04-17 09:14:51.000000 waylay_ml_adapter_sklearn-0.0.2/src/waylay_ml_adapter_sklearn.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (502) staff       (20)        1 2024-04-17 09:14:51.000000 waylay_ml_adapter_sklearn-0.0.2/src/waylay_ml_adapter_sklearn.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (502) staff       (20)       94 2024-04-17 09:14:51.000000 waylay_ml_adapter_sklearn-0.0.2/src/waylay_ml_adapter_sklearn.egg-info/requires.txt
--rw-r--r--   0 thomas     (502) staff       (20)       11 2024-04-17 09:14:51.000000 waylay_ml_adapter_sklearn-0.0.2/src/waylay_ml_adapter_sklearn.egg-info/top_level.txt
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:25:43.568720 waylay_ml_adapter_sklearn-0.0.3/
+-rw-r--r--   0 thomas     (502) staff       (20)      746 2024-04-24 15:21:52.000000 waylay_ml_adapter_sklearn-0.0.3/LICENCE.txt
+-rw-r--r--   0 thomas     (502) staff       (20)     1724 2024-04-24 15:25:43.568373 waylay_ml_adapter_sklearn-0.0.3/PKG-INFO
+-rw-r--r--   0 thomas     (502) staff       (20)     1278 2024-04-24 11:51:39.000000 waylay_ml_adapter_sklearn-0.0.3/README.md
+-rw-r--r--   0 thomas     (502) staff       (20)     1081 2024-04-24 15:21:52.000000 waylay_ml_adapter_sklearn-0.0.3/pyproject.toml
+-rw-r--r--   0 thomas     (502) staff       (20)       38 2024-04-24 15:25:43.568767 waylay_ml_adapter_sklearn-0.0.3/setup.cfg
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:25:43.562903 waylay_ml_adapter_sklearn-0.0.3/src/
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:25:43.562713 waylay_ml_adapter_sklearn-0.0.3/src/ml_adapter/
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:25:43.564282 waylay_ml_adapter_sklearn-0.0.3/src/ml_adapter/sklearn/
+-rw-r--r--   0 thomas     (502) staff       (20)     1044 2024-04-24 10:44:07.000000 waylay_ml_adapter_sklearn-0.0.3/src/ml_adapter/sklearn/__init__.py
+-rw-r--r--   0 thomas     (502) staff       (20)        0 2024-01-25 17:02:04.000000 waylay_ml_adapter_sklearn-0.0.3/src/ml_adapter/sklearn/py.typed
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-24 15:25:43.567810 waylay_ml_adapter_sklearn-0.0.3/src/waylay_ml_adapter_sklearn.egg-info/
+-rw-r--r--   0 thomas     (502) staff       (20)     1724 2024-04-24 15:25:43.000000 waylay_ml_adapter_sklearn-0.0.3/src/waylay_ml_adapter_sklearn.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (502) staff       (20)      367 2024-04-24 15:25:43.000000 waylay_ml_adapter_sklearn-0.0.3/src/waylay_ml_adapter_sklearn.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (502) staff       (20)        1 2024-04-24 15:25:43.000000 waylay_ml_adapter_sklearn-0.0.3/src/waylay_ml_adapter_sklearn.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (502) staff       (20)       94 2024-04-24 15:25:43.000000 waylay_ml_adapter_sklearn-0.0.3/src/waylay_ml_adapter_sklearn.egg-info/requires.txt
+-rw-r--r--   0 thomas     (502) staff       (20)       11 2024-04-24 15:25:43.000000 waylay_ml_adapter_sklearn-0.0.3/src/waylay_ml_adapter_sklearn.egg-info/top_level.txt
```

### Comparing `waylay_ml_adapter_sklearn-0.0.2/pyproject.toml` & `waylay_ml_adapter_sklearn-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 
 [tool.setuptools-git-versioning]
 enabled = true
 
 [project]
 name = "waylay-ml-adapter-sklearn"
 description = "ML_adapter for sklearn."
-requires-python = ">=3.9"
-authors = [{name = "Waylay"}]
+requires-python = ">=3.11"
+authors = [{name = "Waylay", email = "info@waylay.io"}]
+license={file = "LICENSE.txt"}
+readme = "README.md"
 dependencies = [
   "waylay-ml-adapter-numpy",
 ]
 dynamic = ["version"]
 
 
 [project.optional-dependencies]
@@ -28,15 +30,15 @@
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 markers = [
-    "exclude_ci: marks tests to exlude for ci (unstable or requires additional config)"
+    "exclude_ci: marks tests to exclude for ci (unstable or requires additional config)"
 ]
 
 [tool.ruff]
 include = ["pyproject.toml", "src/**/*.py", "test/**/*.py"]
 
 [tool.ruff.lint]
 select = ["E", "F", "UP",  "B", "SIM", "I", "D1", "D4"]
```

