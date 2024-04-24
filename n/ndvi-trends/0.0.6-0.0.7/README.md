# Comparing `tmp/ndvi_trends-0.0.6.tar.gz` & `tmp/ndvi_trends-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndvi_trends-0.0.6.tar", last modified: Fri Mar 22 16:21:41 2024, max compression
+gzip compressed data, was "ndvi_trends-0.0.7.tar", last modified: Wed Apr 24 02:41:29 2024, max compression
```

## Comparing `ndvi_trends-0.0.6.tar` & `ndvi_trends-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 brookieguzder-williams   (501) staff       (20)        0 2024-03-22 16:21:41.773676 ndvi_trends-0.0.6/
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)     2193 2024-02-23 18:28:00.000000 ndvi_trends-0.0.6/LICENSE.md
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)     2677 2024-03-22 16:21:41.773608 ndvi_trends-0.0.6/PKG-INFO
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)     2556 2024-03-21 20:23:04.000000 ndvi_trends-0.0.6/README.md
-drwxr-xr-x   0 brookieguzder-williams   (501) staff       (20)        0 2024-03-22 16:21:41.772036 ndvi_trends-0.0.6/ndvi_trends/
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)       14 2024-03-22 16:16:19.000000 ndvi_trends-0.0.6/ndvi_trends/__init__.py
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)      262 2024-03-22 16:16:45.000000 ndvi_trends-0.0.6/ndvi_trends/calc.py
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)    11575 2024-03-22 16:16:40.000000 ndvi_trends-0.0.6/ndvi_trends/data.py
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)    20527 2024-03-22 16:16:49.000000 ndvi_trends-0.0.6/ndvi_trends/smoothing.py
-drwxr-xr-x   0 brookieguzder-williams   (501) staff       (20)        0 2024-03-22 16:21:41.773172 ndvi_trends-0.0.6/ndvi_trends/utils/
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)       14 2024-03-22 16:16:18.000000 ndvi_trends-0.0.6/ndvi_trends/utils/__init__.py
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)     2139 2024-03-22 16:16:54.000000 ndvi_trends-0.0.6/ndvi_trends/utils/ee.py
-drwxr-xr-x   0 brookieguzder-williams   (501) staff       (20)        0 2024-03-22 16:21:41.773385 ndvi_trends-0.0.6/ndvi_trends.egg-info/
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)     2677 2024-03-22 16:21:41.000000 ndvi_trends-0.0.6/ndvi_trends.egg-info/PKG-INFO
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)      328 2024-03-22 16:21:41.000000 ndvi_trends-0.0.6/ndvi_trends.egg-info/SOURCES.txt
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)        1 2024-03-22 16:21:41.000000 ndvi_trends-0.0.6/ndvi_trends.egg-info/dependency_links.txt
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)       12 2024-03-22 16:21:41.000000 ndvi_trends-0.0.6/ndvi_trends.egg-info/top_level.txt
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)      240 2024-03-22 16:19:51.000000 ndvi_trends-0.0.6/pyproject.toml
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)      114 2024-03-22 16:21:41.773944 ndvi_trends-0.0.6/setup.cfg
+drwxr-xr-x   0 brookieguzder-williams   (501) staff       (20)        0 2024-04-24 02:41:29.880318 ndvi_trends-0.0.7/
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)     2193 2024-02-23 18:28:00.000000 ndvi_trends-0.0.7/LICENSE.md
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)     3127 2024-04-24 02:41:29.880264 ndvi_trends-0.0.7/PKG-INFO
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)     3006 2024-03-22 16:26:36.000000 ndvi_trends-0.0.7/README.md
+drwxr-xr-x   0 brookieguzder-williams   (501) staff       (20)        0 2024-04-24 02:41:29.878791 ndvi_trends-0.0.7/ndvi_trends/
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)       14 2024-03-22 16:16:19.000000 ndvi_trends-0.0.7/ndvi_trends/__init__.py
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)      262 2024-03-22 16:16:45.000000 ndvi_trends-0.0.7/ndvi_trends/calc.py
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)    11979 2024-03-31 16:45:05.000000 ndvi_trends-0.0.7/ndvi_trends/data.py
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)    22814 2024-04-24 02:37:00.000000 ndvi_trends-0.0.7/ndvi_trends/smoothing.py
+drwxr-xr-x   0 brookieguzder-williams   (501) staff       (20)        0 2024-04-24 02:41:29.879817 ndvi_trends-0.0.7/ndvi_trends/utils/
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)       14 2024-03-22 16:16:18.000000 ndvi_trends-0.0.7/ndvi_trends/utils/__init__.py
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)     2139 2024-03-22 16:16:54.000000 ndvi_trends-0.0.7/ndvi_trends/utils/ee.py
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)    10757 2024-04-22 18:29:55.000000 ndvi_trends-0.0.7/ndvi_trends/utils/npxr.py
+drwxr-xr-x   0 brookieguzder-williams   (501) staff       (20)        0 2024-04-24 02:41:29.880116 ndvi_trends-0.0.7/ndvi_trends.egg-info/
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)     3127 2024-04-24 02:41:29.000000 ndvi_trends-0.0.7/ndvi_trends.egg-info/PKG-INFO
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)      354 2024-04-24 02:41:29.000000 ndvi_trends-0.0.7/ndvi_trends.egg-info/SOURCES.txt
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)        1 2024-04-24 02:41:29.000000 ndvi_trends-0.0.7/ndvi_trends.egg-info/dependency_links.txt
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)       12 2024-04-24 02:41:29.000000 ndvi_trends-0.0.7/ndvi_trends.egg-info/top_level.txt
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)      240 2024-04-24 02:38:23.000000 ndvi_trends-0.0.7/pyproject.toml
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)      114 2024-04-24 02:41:29.880496 ndvi_trends-0.0.7/setup.cfg
```

### Comparing `ndvi_trends-0.0.6/LICENSE.md` & `ndvi_trends-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ndvi_trends-0.0.6/PKG-INFO` & `ndvi_trends-0.0.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: ndvi_trends
-Version: 0.0.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 #### NDVI TRENDS
 
 A module for studying NDVI Trends (from S2/LSAT) with a particular emphasis on determining or deriving relvant features for cover-cropping.
 
 1. Generate and Save NDVI Series for small Regions
 	a. grab NDVI Series on the fly for any geom
 	b. for a large set of geoms efficiently grab and save all
@@ -70,14 +64,27 @@
 # (optional) need to first remove old distributions or be more selective with * on twine-upload
 rm -rf dist
 # https://packaging.python.org/en/latest/tutorials/packaging-projects/
 python -m build
 python -m twine upload dist/*
 ```
 
+NOTE:  When testing locally the editable environment (`pip install -e .`) might behave differently than the pacakage. For example, the pyproject.toml should explicitly include submodules. In this case:
+
+```toml
+[tool.setuptools]
+packages = [
+	"ndvi_trends",
+	"ndvi_trends.utils"
+]
+```
+
+My original file did not include `ndvi_trends.utils` but behaved correctly locally. However when deployed this lead to problems.  Before deploying drop the `-e`!
+
+
 ###### MODULES:
 
 ├── ndvi_trends
 │		├── calc: extracts features and statistics from NDVI Series
 │		├── data: methods for fetching NDVI data from Harmonized S2-Landsat using GEE
 │		├── smoothing: gap filling and smoothing utilities
 │		└── utils
```

### Comparing `ndvi_trends-0.0.6/README.md` & `ndvi_trends-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1
+Name: ndvi_trends
+Version: 0.0.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 #### NDVI TRENDS
 
 A module for studying NDVI Trends (from S2/LSAT) with a particular emphasis on determining or deriving relvant features for cover-cropping.
 
 1. Generate and Save NDVI Series for small Regions
 	a. grab NDVI Series on the fly for any geom
 	b. for a large set of geoms efficiently grab and save all
@@ -64,14 +70,27 @@
 # (optional) need to first remove old distributions or be more selective with * on twine-upload
 rm -rf dist
 # https://packaging.python.org/en/latest/tutorials/packaging-projects/
 python -m build
 python -m twine upload dist/*
 ```
 
+NOTE:  When testing locally the editable environment (`pip install -e .`) might behave differently than the pacakage. For example, the pyproject.toml should explicitly include submodules. In this case:
+
+```toml
+[tool.setuptools]
+packages = [
+	"ndvi_trends",
+	"ndvi_trends.utils"
+]
+```
+
+My original file did not include `ndvi_trends.utils` but behaved correctly locally. However when deployed this lead to problems.  Before deploying drop the `-e`!
+
+
 ###### MODULES:
 
 ├── ndvi_trends
 │		├── calc: extracts features and statistics from NDVI Series
 │		├── data: methods for fetching NDVI data from Harmonized S2-Landsat using GEE
 │		├── smoothing: gap filling and smoothing utilities
 │		└── utils
```

### Comparing `ndvi_trends-0.0.6/ndvi_trends/data.py` & `ndvi_trends-0.0.7/ndvi_trends/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,21 @@
     ds = get_ee_xrr(ndvi_ic, geom, attrs={'nb_s2': nb_s2, 'nb_landsat': nb_lsat})
     ds['is_sentinel_2'] = 'time', is_s2
     if attrs:
         ds = ds.assign_attrs(attrs)
     return ds
 
 
-def get_ndvi_dataset_for_field(dn, start_date=None, end_date=None, attrs={}, source=None):
+def get_ndvi_dataset_for_field(
+        dn,
+        start_date=None,
+        end_date=None,
+        attrs={},
+        source=None,
+        local_dir=None):
     """ TODO: MANAGE MULTI-GEOM FIELDS
 
     Fetches cloud-masked ndvi xr.dataset from Google Earth Engine for
     a given field, start and end date.
 
     The field geometries/attributes are contained in asset
     projects/yield-predict/assets/KnoxFields
@@ -144,28 +150,36 @@
         end_date (str): end date as string
         attrs (dict): attributes-dict to add to resulting dataset
         source (str): filter data by datasource. one of ['S2','LSAT']
 
     Returns:
         xr.DataSet of ndvi values
     """
-    dn = int(dn)
-    attrs = attrs.copy()
-    attrs['DN'] = dn
-    attrs['data_start_date'] = start_date
-    attrs['data_end_date'] = end_date
-    field = ee.Feature(FIELDS_FC.filter(ee.Filter.eq('DN', dn)).first())
-    geom = field.geometry()
-    attrs.update(field.toDictionary().getInfo())
-    return get_ndvi_dataset(
-        geom,
-        start_date=start_date,
-        end_date=end_date,
-        attrs=attrs,
-        source=source)
+    if local_dir:
+        ds = xr.open_dataset(f'{local_dir}/{dn}', engine='zarr', consolidated=False,)
+        if start_date or end_date:
+            ds = ds.sel(time=slice(start_date, end_date))
+        if attrs:
+            ds = ds.assign_attrs(attrs)
+        return ds
+    else:
+        dn = int(dn)
+        attrs = attrs.copy()
+        attrs['DN'] = dn
+        attrs['data_start_date'] = start_date
+        attrs['data_end_date'] = end_date
+        field = ee.Feature(FIELDS_FC.filter(ee.Filter.eq('DN', dn)).first())
+        geom = field.geometry()
+        attrs.update(field.toDictionary().getInfo())
+        return get_ndvi_dataset(
+            geom,
+            start_date=start_date,
+            end_date=end_date,
+            attrs=attrs,
+            source=source)
 
 
 def get_ndvi_dataset_at_point(
         lon,
         lat,
         radius=DEFAULT_RADIUS,
         start_date=None,
```

### Comparing `ndvi_trends-0.0.6/ndvi_trends/utils/ee.py` & `ndvi_trends-0.0.7/ndvi_trends/utils/ee.py`

 * *Files identical despite different names*

### Comparing `ndvi_trends-0.0.6/ndvi_trends.egg-info/PKG-INFO` & `ndvi_trends-0.0.7/ndvi_trends.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndvi_trends
-Version: 0.0.6
+Version: 0.0.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 #### NDVI TRENDS
 
 A module for studying NDVI Trends (from S2/LSAT) with a particular emphasis on determining or deriving relvant features for cover-cropping.
 
@@ -70,14 +70,27 @@
 # (optional) need to first remove old distributions or be more selective with * on twine-upload
 rm -rf dist
 # https://packaging.python.org/en/latest/tutorials/packaging-projects/
 python -m build
 python -m twine upload dist/*
 ```
 
+NOTE:  When testing locally the editable environment (`pip install -e .`) might behave differently than the pacakage. For example, the pyproject.toml should explicitly include submodules. In this case:
+
+```toml
+[tool.setuptools]
+packages = [
+	"ndvi_trends",
+	"ndvi_trends.utils"
+]
+```
+
+My original file did not include `ndvi_trends.utils` but behaved correctly locally. However when deployed this lead to problems.  Before deploying drop the `-e`!
+
+
 ###### MODULES:
 
 ├── ndvi_trends
 │		├── calc: extracts features and statistics from NDVI Series
 │		├── data: methods for fetching NDVI data from Harmonized S2-Landsat using GEE
 │		├── smoothing: gap filling and smoothing utilities
 │		└── utils
```

