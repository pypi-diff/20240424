# Comparing `tmp/xee-0.0.8.tar.gz` & `tmp/xee-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xee-0.0.8.tar", last modified: Thu Feb  1 17:34:57 2024, max compression
+gzip compressed data, was "xee-0.0.9.tar", last modified: Wed Feb 14 21:44:42 2024, max compression
```

## Comparing `xee-0.0.8.tar` & `xee-0.0.9.tar`

### file list

```diff
@@ -1,43 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 17:34:57.842594 xee-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 17:34:57.834594 xee-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 17:34:57.834594 xee-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-02-01 17:34:43.000000 xee-0.0.8/.github/workflows/ci-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-02-01 17:34:43.000000 xee-0.0.8/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-02-01 17:34:43.000000 xee-0.0.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-01 17:34:43.000000 xee-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-01 17:34:43.000000 xee-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-02-01 17:34:57.842594 xee-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-02-01 17:34:43.000000 xee-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-02-01 17:34:43.000000 xee-0.0.8/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 17:34:57.838594 xee-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-01 17:34:43.000000 xee-0.0.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-02-01 17:34:43.000000 xee-0.0.8/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-01 17:34:43.000000 xee-0.0.8/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-02-01 17:34:43.000000 xee-0.0.8/docs/code-of-conduct.md
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-02-01 17:34:43.000000 xee-0.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-01 17:34:43.000000 xee-0.0.8/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-02-01 17:34:43.000000 xee-0.0.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-01 17:34:43.000000 xee-0.0.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-01 17:34:43.000000 xee-0.0.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-02-01 17:34:43.000000 xee-0.0.8/docs/why-xee.md
--rw-r--r--   0 runner    (1001) docker     (127)    11803 2024-02-01 17:34:43.000000 xee-0.0.8/docs/xee-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 17:34:57.838594 xee-0.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-02-01 17:34:43.000000 xee-0.0.8/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-02-01 17:34:43.000000 xee-0.0.8/examples/ee_to_zarr.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-01 17:34:43.000000 xee-0.0.8/examples/ee_to_zarr_reqs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-02-01 17:34:43.000000 xee-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-01 17:34:57.842594 xee-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 17:34:57.838594 xee-0.0.8/xee/
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-02-01 17:34:43.000000 xee-0.0.8/xee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37659 2024-02-01 17:34:43.000000 xee-0.0.8/xee/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)    17150 2024-02-01 17:34:43.000000 xee-0.0.8/xee/ext_integration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-02-01 17:34:43.000000 xee-0.0.8/xee/ext_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-02-01 17:34:43.000000 xee-0.0.8/xee/micro_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-02-01 17:34:43.000000 xee-0.0.8/xee/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 17:34:57.842594 xee-0.0.8/xee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-02-01 17:34:57.000000 xee-0.0.8/xee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-02-01 17:34:57.000000 xee-0.0.8/xee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 17:34:57.000000 xee-0.0.8/xee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-01 17:34:57.000000 xee-0.0.8/xee.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-01 17:34:57.000000 xee-0.0.8/xee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-01 17:34:57.000000 xee-0.0.8/xee.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:44:42.476083 xee-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:44:42.468083 xee-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:44:42.472083 xee-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-02-14 21:44:26.000000 xee-0.0.9/.github/workflows/ci-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-02-14 21:44:26.000000 xee-0.0.9/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-02-14 21:44:26.000000 xee-0.0.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-14 21:44:26.000000 xee-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-14 21:44:26.000000 xee-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-02-14 21:44:42.476083 xee-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-02-14 21:44:26.000000 xee-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-02-14 21:44:26.000000 xee-0.0.9/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:44:42.472083 xee-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-14 21:44:26.000000 xee-0.0.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-02-14 21:44:26.000000 xee-0.0.9/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-14 21:44:26.000000 xee-0.0.9/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-02-14 21:44:26.000000 xee-0.0.9/docs/code-of-conduct.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-02-14 21:44:26.000000 xee-0.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-14 21:44:26.000000 xee-0.0.9/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-02-14 21:44:26.000000 xee-0.0.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-14 21:44:26.000000 xee-0.0.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-14 21:44:26.000000 xee-0.0.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-02-14 21:44:26.000000 xee-0.0.9/docs/why-xee.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11803 2024-02-14 21:44:26.000000 xee-0.0.9/docs/xee-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:44:42.472083 xee-0.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-02-14 21:44:26.000000 xee-0.0.9/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:44:42.472083 xee-0.0.9/examples/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-14 21:44:26.000000 xee-0.0.9/examples/dataflow/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-02-14 21:44:26.000000 xee-0.0.9/examples/dataflow/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-14 21:44:26.000000 xee-0.0.9/examples/dataflow/cloudbuild.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-02-14 21:44:26.000000 xee-0.0.9/examples/dataflow/ee_to_zarr_dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-14 21:44:26.000000 xee-0.0.9/examples/dataflow/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-02-14 21:44:26.000000 xee-0.0.9/examples/ee_to_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-14 21:44:26.000000 xee-0.0.9/examples/ee_to_zarr_reqs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-02-14 21:44:26.000000 xee-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 21:44:42.476083 xee-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:44:42.476083 xee-0.0.9/xee/
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-02-14 21:44:26.000000 xee-0.0.9/xee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38869 2024-02-14 21:44:26.000000 xee-0.0.9/xee/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17150 2024-02-14 21:44:26.000000 xee-0.0.9/xee/ext_integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-02-14 21:44:26.000000 xee-0.0.9/xee/ext_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-02-14 21:44:26.000000 xee-0.0.9/xee/micro_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-02-14 21:44:26.000000 xee-0.0.9/xee/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:44:42.476083 xee-0.0.9/xee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-02-14 21:44:42.000000 xee-0.0.9/xee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-02-14 21:44:42.000000 xee-0.0.9/xee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 21:44:42.000000 xee-0.0.9/xee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-14 21:44:42.000000 xee-0.0.9/xee.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-14 21:44:42.000000 xee-0.0.9/xee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-14 21:44:42.000000 xee-0.0.9/xee.egg-info/top_level.txt
```

### Comparing `xee-0.0.8/.github/workflows/ci-build.yml` & `xee-0.0.9/.github/workflows/ci-build.yml`

 * *Files identical despite different names*

### Comparing `xee-0.0.8/.github/workflows/lint.yml` & `xee-0.0.9/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `xee-0.0.8/.github/workflows/publish.yml` & `xee-0.0.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `xee-0.0.8/LICENSE` & `xee-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xee-0.0.8/PKG-INFO` & `xee-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xee
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Google Earth Engine extension for Xarray.
 Author-email: Google LLC <noreply@google.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/google/xee
 Project-URL: Issues, https://github.com/google/Xee/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -28,19 +28,21 @@
 Requires-Dist: affine
 Provides-Extra: tests
 Requires-Dist: absl-py; extra == "tests"
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pyink; extra == "tests"
 Requires-Dist: rasterio; extra == "tests"
 Requires-Dist: rioxarray; extra == "tests"
+Provides-Extra: dataflow
+Requires-Dist: absl-py; extra == "dataflow"
+Requires-Dist: apache-beam[gcp]; extra == "dataflow"
+Requires-Dist: gcsfs; extra == "dataflow"
+Requires-Dist: xarray-beam; extra == "dataflow"
 Provides-Extra: examples
-Requires-Dist: apache_beam[gcp]; extra == "examples"
-Requires-Dist: xarray-beam; extra == "examples"
-Requires-Dist: absl-py; extra == "examples"
-Requires-Dist: gcsfs; extra == "examples"
+Requires-Dist: xee[dataflow]; extra == "examples"
 
 # Xee: Xarray + Google Earth Engine
 
 ![Xee Logo](https://raw.githubusercontent.com/google/Xee/main/docs/xee-logo.png)
 
 _An Xarray extension for Google Earth Engine._
 
@@ -126,15 +128,15 @@
 Open a single Image by passing it to an ImageCollection:
 
 ```python
 i = ee.ImageCollection(ee.Image("LANDSAT/LC08/C02/T1_TOA/LC08_044034_20140318"))
 ds = xarray.open_dataset(i, engine='ee')
 ```
 
-See [examples](examples/) or [docs](docs/) for more uses and integrations.
+See [examples](https://github.com/google/Xee/tree/main/examples) or [docs](https://github.com/google/Xee/tree/main/docs) for more uses and integrations.
 
 ## License
 
 This is not an official Google product.
 
 ```
 Copyright 2023 Google LLC
```

### Comparing `xee-0.0.8/README.md` & `xee-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 Open a single Image by passing it to an ImageCollection:
 
 ```python
 i = ee.ImageCollection(ee.Image("LANDSAT/LC08/C02/T1_TOA/LC08_044034_20140318"))
 ds = xarray.open_dataset(i, engine='ee')
 ```
 
-See [examples](examples/) or [docs](docs/) for more uses and integrations.
+See [examples](https://github.com/google/Xee/tree/main/examples) or [docs](https://github.com/google/Xee/tree/main/docs) for more uses and integrations.
 
 ## License
 
 This is not an official Google product.
 
 ```
 Copyright 2023 Google LLC
```

### Comparing `xee-0.0.8/conftest.py` & `xee-0.0.9/conftest.py`

 * *Files identical despite different names*

### Comparing `xee-0.0.8/docs/Makefile` & `xee-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xee-0.0.8/docs/README.md` & `xee-0.0.9/docs/README.md`

 * *Files identical despite different names*

### Comparing `xee-0.0.8/docs/code-of-conduct.md` & `xee-0.0.9/docs/code-of-conduct.md`

 * *Files identical despite different names*

### Comparing `xee-0.0.8/docs/conf.py` & `xee-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xee-0.0.8/docs/contributing.md` & `xee-0.0.9/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `xee-0.0.8/docs/index.md` & `xee-0.0.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `xee-0.0.8/docs/make.bat` & `xee-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xee-0.0.8/docs/why-xee.md` & `xee-0.0.9/docs/why-xee.md`

 * *Files identical despite different names*

### Comparing `xee-0.0.8/docs/xee-logo.png` & `xee-0.0.9/docs/xee-logo.png`

 * *Files identical despite different names*

### Comparing `xee-0.0.8/examples/README.md` & `xee-0.0.9/examples/README.md`

 * *Files identical despite different names*

### Comparing `xee-0.0.8/examples/ee_to_zarr.py` & `xee-0.0.9/examples/ee_to_zarr.py`

 * *Files identical despite different names*

### Comparing `xee-0.0.8/pyproject.toml` & `xee-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -37,19 +37,22 @@
 tests = [
   "absl-py",
   "pytest",
   "pyink",
   "rasterio",
   "rioxarray",
 ]
-examples = [
-  "apache_beam[gcp]",
-  "xarray-beam",
+dataflow = [
   "absl-py",
+  "apache-beam[gcp]",
   "gcsfs",
+  "xarray-beam",
+]
+examples = [
+  "xee[dataflow]",
 ]
 
 [project.urls]
 Homepage = "https://github.com/google/xee"
 Issues = "https://github.com/google/Xee/issues"
 
 [build-system]
```

### Comparing `xee-0.0.8/xee/__init__.py` & `xee-0.0.9/xee/__init__.py`

 * *Files identical despite different names*

### Comparing `xee-0.0.8/xee/ext.py` & `xee-0.0.9/xee/ext.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,14 +140,16 @@
       scale: Optional[float] = None,
       projection: Optional[ee.Projection] = None,
       geometry: Optional[ee.Geometry] = None,
       primary_dim_name: Optional[str] = None,
       primary_dim_property: Optional[str] = None,
       mask_value: Optional[float] = None,
       request_byte_limit: int = REQUEST_BYTE_LIMIT,
+      ee_init_kwargs: Optional[Dict[str, Any]] = None,
+      ee_init_if_necessary: bool = False,
   ) -> 'EarthEngineStore':
     if mode != 'r':
       raise ValueError(
           f'mode {mode!r} is invalid: data can only be read from Earth Engine.'
       )
 
     return cls(
@@ -158,14 +160,16 @@
         scale=scale,
         projection=projection,
         geometry=geometry,
         primary_dim_name=primary_dim_name,
         primary_dim_property=primary_dim_property,
         mask_value=mask_value,
         request_byte_limit=request_byte_limit,
+        ee_init_kwargs=ee_init_kwargs,
+        ee_init_if_necessary=ee_init_if_necessary,
     )
 
   def __init__(
       self,
       image_collection: ee.ImageCollection,
       chunks: Chunks = None,
       n_images: int = -1,
@@ -173,15 +177,20 @@
       scale: Union[float, int, None] = None,
       projection: Optional[ee.Projection] = None,
       geometry: Optional[ee.Geometry] = None,
       primary_dim_name: Optional[str] = None,
       primary_dim_property: Optional[str] = None,
       mask_value: Optional[float] = None,
       request_byte_limit: int = REQUEST_BYTE_LIMIT,
+      ee_init_kwargs: Optional[Dict[str, Any]] = None,
+      ee_init_if_necessary: bool = False,
   ):
+    self.ee_init_kwargs = ee_init_kwargs
+    self.ee_init_if_necessary = ee_init_if_necessary
+
     self.image_collection = image_collection
     if n_images != -1:
       self.image_collection = image_collection.limit(n_images)
 
     self.projection = projection
     self.geometry = geometry
     self.primary_dim_name = primary_dim_name or 'time'
@@ -718,14 +727,23 @@
     y_size = max(1, int(np.round((y_max - y_min) / np.abs(self.store.scale_y))))
 
     self.shape = (ee_store.n_images, x_size, y_size)
     self._apparent_chunks = {k: 1 for k in self.store.PREFERRED_CHUNKS.keys()}
     if isinstance(self.store.chunks, dict):
       self._apparent_chunks = self.store.chunks.copy()
 
+  def _ee_init_check(self):
+    if not ee.data.is_initialized() and self.store.ee_init_if_necessary:
+      warnings.warn(
+          'Earth Engine is not initialized on worker. '
+          'Attempting to initialize using application default credentials.'
+      )
+
+      ee.Initialize(**(self.store.ee_init_kwargs or {}))
+
   def __getitem__(self, key: indexing.ExplicitIndexer) -> np.typing.ArrayLike:
     return indexing.explicit_indexing_adapter(
         key,
         self.shape,
         indexing.IndexingSupport.BASIC,
         self._raw_indexing_method,
     )
@@ -757,14 +775,15 @@
 
     return tuple(key_new), tuple(squeeze_axes)
 
   def _slice_collection(self, image_slice: slice) -> ee.Image:
     """Reduce the ImageCollection into an Image with bands as index slices."""
     # Get the right range of Images in the collection, either a single image or
     # a range of images...
+    self._ee_init_check()
     start, stop, stride = image_slice.indices(self.shape[0])
 
     # If the input images have IDs, just slice them. Otherwise, we need to do
     # an expensive `toList()` operation.
     if self.store.image_ids:
       imgs = self.store.image_ids[start:stop:stride]
     else:
@@ -926,14 +945,16 @@
       scale: Union[float, int, None] = None,
       projection: Optional[ee.Projection] = None,
       geometry: Optional[ee.Geometry] = None,
       primary_dim_name: Optional[str] = None,
       primary_dim_property: Optional[str] = None,
       ee_mask_value: Optional[float] = None,
       request_byte_limit: int = REQUEST_BYTE_LIMIT,
+      ee_init_if_necessary: bool = False,
+      ee_init_kwargs: Optional[Dict[str, Any]] = None,
   ) -> xarray.Dataset:  # type: ignore
     """Open an Earth Engine ImageCollection as an Xarray Dataset.
 
     Args:
       filename_or_obj: An asset ID for an ImageCollection, or an
         ee.ImageCollection object.
       drop_variables (optional): Variables or bands to drop before opening.
@@ -990,14 +1011,19 @@
       primary_dim_property (optional): Override the `ee.Image` property for
         which to derive the values of the primary dimension. By default, this is
         'system:time_start'.
       ee_mask_value (optional): Value to mask to EE nodata values. By default,
         this is 'np.iinfo(np.int32).max' i.e. 2147483647.
       request_byte_limit: the max allowed bytes to request at a time from Earth
         Engine. By default, it is 48MBs.
+      ee_init_if_necessary: boolean flag to set if auto initialize for Earth
+        Engine should be attempted. Set to True if using distributed compute
+        frameworks.
+      ee_init_kwargs: keywords to pass to Earth Engine Initialize when
+        attempting to auto init for remote workers.
 
     Returns:
       An xarray.Dataset that streams in remote data from Earth Engine.
     """
 
     user_agent = f'Xee/{__version__}'
     if ee.data.getUserAgent() != user_agent:
@@ -1017,14 +1043,16 @@
         scale=scale,
         projection=projection,
         geometry=geometry,
         primary_dim_name=primary_dim_name,
         primary_dim_property=primary_dim_property,
         mask_value=ee_mask_value,
         request_byte_limit=request_byte_limit,
+        ee_init_kwargs=ee_init_kwargs,
+        ee_init_if_necessary=ee_init_if_necessary,
     )
 
     store_entrypoint = backends_store.StoreBackendEntrypoint()
 
     with utils.close_on_error(store):
       ds = store_entrypoint.open_dataset(
           store,
```

### Comparing `xee-0.0.8/xee/ext_integration_test.py` & `xee-0.0.9/xee/ext_integration_test.py`

 * *Files identical despite different names*

### Comparing `xee-0.0.8/xee/ext_test.py` & `xee-0.0.9/xee/ext_test.py`

 * *Files identical despite different names*

### Comparing `xee-0.0.8/xee/micro_benchmarks.py` & `xee-0.0.9/xee/micro_benchmarks.py`

 * *Files identical despite different names*

### Comparing `xee-0.0.8/xee/types.py` & `xee-0.0.9/xee/types.py`

 * *Files identical despite different names*

### Comparing `xee-0.0.8/xee.egg-info/PKG-INFO` & `xee-0.0.9/xee.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xee
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Google Earth Engine extension for Xarray.
 Author-email: Google LLC <noreply@google.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/google/xee
 Project-URL: Issues, https://github.com/google/Xee/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -28,19 +28,21 @@
 Requires-Dist: affine
 Provides-Extra: tests
 Requires-Dist: absl-py; extra == "tests"
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pyink; extra == "tests"
 Requires-Dist: rasterio; extra == "tests"
 Requires-Dist: rioxarray; extra == "tests"
+Provides-Extra: dataflow
+Requires-Dist: absl-py; extra == "dataflow"
+Requires-Dist: apache-beam[gcp]; extra == "dataflow"
+Requires-Dist: gcsfs; extra == "dataflow"
+Requires-Dist: xarray-beam; extra == "dataflow"
 Provides-Extra: examples
-Requires-Dist: apache_beam[gcp]; extra == "examples"
-Requires-Dist: xarray-beam; extra == "examples"
-Requires-Dist: absl-py; extra == "examples"
-Requires-Dist: gcsfs; extra == "examples"
+Requires-Dist: xee[dataflow]; extra == "examples"
 
 # Xee: Xarray + Google Earth Engine
 
 ![Xee Logo](https://raw.githubusercontent.com/google/Xee/main/docs/xee-logo.png)
 
 _An Xarray extension for Google Earth Engine._
 
@@ -126,15 +128,15 @@
 Open a single Image by passing it to an ImageCollection:
 
 ```python
 i = ee.ImageCollection(ee.Image("LANDSAT/LC08/C02/T1_TOA/LC08_044034_20140318"))
 ds = xarray.open_dataset(i, engine='ee')
 ```
 
-See [examples](examples/) or [docs](docs/) for more uses and integrations.
+See [examples](https://github.com/google/Xee/tree/main/examples) or [docs](https://github.com/google/Xee/tree/main/docs) for more uses and integrations.
 
 ## License
 
 This is not an official Google product.
 
 ```
 Copyright 2023 Google LLC
```

