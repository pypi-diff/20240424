# Comparing `tmp/pandas_geojson-2.0.1.tar.gz` & `tmp/pandas_geojson-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_geojson-2.0.1.tar", last modified: Tue Apr  2 03:02:39 2024, max compression
+gzip compressed data, was "pandas_geojson-2.1.0.tar", last modified: Wed Apr 24 03:11:20 2024, max compression
```

## Comparing `pandas_geojson-2.0.1.tar` & `pandas_geojson-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 03:02:39.262102 pandas_geojson-2.0.1/
--rw-rw-rw-   0        0        0     1097 2024-03-18 19:56:01.000000 pandas_geojson-2.0.1/LICENSE
--rw-rw-rw-   0        0        0    53377 2024-04-02 03:02:39.261104 pandas_geojson-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    52944 2024-03-27 02:11:25.000000 pandas_geojson-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 03:02:39.227433 pandas_geojson-2.0.1/pandas_geojson/
--rw-rw-rw-   0        0        0      280 2024-04-02 03:02:09.000000 pandas_geojson-2.0.1/pandas_geojson/__init__.py
--rw-rw-rw-   0        0        0     3347 2024-04-02 02:59:27.000000 pandas_geojson-2.0.1/pandas_geojson/core.py
--rw-rw-rw-   0        0        0      645 2024-03-18 19:56:01.000000 pandas_geojson-2.0.1/pandas_geojson/io.py
-drwxrwxrwx   0        0        0        0 2024-04-02 03:02:39.259104 pandas_geojson-2.0.1/pandas_geojson.egg-info/
--rw-rw-rw-   0        0        0    53377 2024-04-02 03:02:39.000000 pandas_geojson-2.0.1/pandas_geojson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2024-04-02 03:02:39.000000 pandas_geojson-2.0.1/pandas_geojson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 03:02:39.000000 pandas_geojson-2.0.1/pandas_geojson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-02 03:02:39.000000 pandas_geojson-2.0.1/pandas_geojson.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-02 03:02:39.000000 pandas_geojson-2.0.1/pandas_geojson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 03:02:39.262102 pandas_geojson-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      823 2024-04-02 03:01:31.000000 pandas_geojson-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:11:20.221367 pandas_geojson-2.1.0/
+-rw-rw-rw-   0        0        0     1097 2024-03-18 19:56:01.000000 pandas_geojson-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0    53354 2024-04-24 03:11:20.219366 pandas_geojson-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    52944 2024-03-27 02:11:25.000000 pandas_geojson-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 03:11:20.194786 pandas_geojson-2.1.0/pandas_geojson/
+-rw-rw-rw-   0        0        0      491 2024-04-22 22:20:20.000000 pandas_geojson-2.1.0/pandas_geojson/__init__.py
+-rw-rw-rw-   0        0        0    10534 2024-04-23 02:53:14.000000 pandas_geojson-2.1.0/pandas_geojson/core.py
+-rw-rw-rw-   0        0        0      645 2024-03-18 19:56:01.000000 pandas_geojson-2.1.0/pandas_geojson/io.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:11:20.218367 pandas_geojson-2.1.0/pandas_geojson.egg-info/
+-rw-rw-rw-   0        0        0    53354 2024-04-24 03:11:20.000000 pandas_geojson-2.1.0/pandas_geojson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-04-24 03:11:20.000000 pandas_geojson-2.1.0/pandas_geojson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 03:11:20.000000 pandas_geojson-2.1.0/pandas_geojson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-24 03:11:20.000000 pandas_geojson-2.1.0/pandas_geojson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 03:11:20.221367 pandas_geojson-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      815 2024-04-22 23:35:36.000000 pandas_geojson-2.1.0/setup.py
```

### Comparing `pandas_geojson-2.0.1/LICENSE` & `pandas_geojson-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_geojson-2.0.1/PKG-INFO` & `pandas_geojson-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: pandas_geojson
-Version: 2.0.1
+Version: 2.1.0
 Summary: Convert Pandas Dataframe to GeoJSON
 Home-page: https://github.com/jrasband-dev/pandas-geojson
 Author: Jayden Rasband
 Author-email: jayden.rasband@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pandas
 
 ![](https://raw.githubusercontent.com/jrasband-dev/pandas-geojson/master/static/pandasgeojson.png)
 
 ---
 ![PyPI - Version](https://img.shields.io/pypi/v/pandas-geojson)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pandas-geojson)
 ![PyPI - License](https://img.shields.io/pypi/l/pandas-geojson)
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 2.1 Name: pandas_geojson Version: 2.0.1 Summary: Convert
+Metadata-Version: 2.1 Name: pandas_geojson Version: 2.1.0 Summary: Convert
 Pandas Dataframe to GeoJSON Home-page: https://github.com/jrasband-dev/pandas-
 geojson Author: Jayden Rasband Author-email: jayden.rasband@gmail.com License:
 MIT Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: pandas ![](https://raw.githubusercontent.com/jrasband-
-dev/pandas-geojson/master/static/pandasgeojson.png) --- ![PyPI - Version]
-(https://img.shields.io/pypi/v/pandas-geojson) ![PyPI - Downloads](https://
-img.shields.io/pypi/dm/pandas-geojson) ![PyPI - License](https://
-img.shields.io/pypi/l/pandas-geojson) ![Libraries.io SourceRank](https://
-img.shields.io/librariesio/sourcerank/pypi/pandas-geojson) # Getting Started
-Install the latest version of pandas-geojson using pip. ``` pip install pandas-
-geojson ``` ## Open GeoJSON Files Using the `read_geojson` function, you can
-easily read in GeoJSON data int the GeoJSON object. ```python import
-pandas_geojson as pdg geojson = pdg.read_geojson('datasets/
-National_Obesity_By_State.geojson') type(geojson) ```
+LICENSE ![](https://raw.githubusercontent.com/jrasband-dev/pandas-geojson/
+master/static/pandasgeojson.png) --- ![PyPI - Version](https://img.shields.io/
+pypi/v/pandas-geojson) ![PyPI - Downloads](https://img.shields.io/pypi/dm/
+pandas-geojson) ![PyPI - License](https://img.shields.io/pypi/l/pandas-geojson)
+![Libraries.io SourceRank](https://img.shields.io/librariesio/sourcerank/pypi/
+pandas-geojson) # Getting Started Install the latest version of pandas-geojson
+using pip. ``` pip install pandas-geojson ``` ## Open GeoJSON Files Using the
+`read_geojson` function, you can easily read in GeoJSON data int the GeoJSON
+object. ```python import pandas_geojson as pdg geojson = pdg.read_geojson
+('datasets/National_Obesity_By_State.geojson') type(geojson) ```
 pandas_geojson.core.GeoJSON ## List Properties Pandas-GeoJSON utilizes
 properties to filter large geojson files. This functionallity helps you
 identify all of the properties in the geojson file so that you can choose a
 filter criteria. For more on filtering see [filter_geojson](#filter-geojson)
 ```python geojson.get_properties() ``` ['FID', 'NAME', 'Obesity',
 'SHAPE_Length', 'SHAPE_Area'] ## DataFrame to GeoJSON Pandas-GeoJSON makes it
 easy to convert a dataframe with coordinates into a GeoJSON object. Your
```

### Comparing `pandas_geojson-2.0.1/README.md` & `pandas_geojson-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pandas_geojson-2.0.1/pandas_geojson/io.py` & `pandas_geojson-2.1.0/pandas_geojson/io.py`

 * *Files identical despite different names*

### Comparing `pandas_geojson-2.0.1/pandas_geojson.egg-info/PKG-INFO` & `pandas_geojson-2.1.0/pandas_geojson.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: pandas_geojson
-Version: 2.0.1
+Version: 2.1.0
 Summary: Convert Pandas Dataframe to GeoJSON
 Home-page: https://github.com/jrasband-dev/pandas-geojson
 Author: Jayden Rasband
 Author-email: jayden.rasband@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pandas
 
 ![](https://raw.githubusercontent.com/jrasband-dev/pandas-geojson/master/static/pandasgeojson.png)
 
 ---
 ![PyPI - Version](https://img.shields.io/pypi/v/pandas-geojson)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pandas-geojson)
 ![PyPI - License](https://img.shields.io/pypi/l/pandas-geojson)
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 2.1 Name: pandas_geojson Version: 2.0.1 Summary: Convert
+Metadata-Version: 2.1 Name: pandas_geojson Version: 2.1.0 Summary: Convert
 Pandas Dataframe to GeoJSON Home-page: https://github.com/jrasband-dev/pandas-
 geojson Author: Jayden Rasband Author-email: jayden.rasband@gmail.com License:
 MIT Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: pandas ![](https://raw.githubusercontent.com/jrasband-
-dev/pandas-geojson/master/static/pandasgeojson.png) --- ![PyPI - Version]
-(https://img.shields.io/pypi/v/pandas-geojson) ![PyPI - Downloads](https://
-img.shields.io/pypi/dm/pandas-geojson) ![PyPI - License](https://
-img.shields.io/pypi/l/pandas-geojson) ![Libraries.io SourceRank](https://
-img.shields.io/librariesio/sourcerank/pypi/pandas-geojson) # Getting Started
-Install the latest version of pandas-geojson using pip. ``` pip install pandas-
-geojson ``` ## Open GeoJSON Files Using the `read_geojson` function, you can
-easily read in GeoJSON data int the GeoJSON object. ```python import
-pandas_geojson as pdg geojson = pdg.read_geojson('datasets/
-National_Obesity_By_State.geojson') type(geojson) ```
+LICENSE ![](https://raw.githubusercontent.com/jrasband-dev/pandas-geojson/
+master/static/pandasgeojson.png) --- ![PyPI - Version](https://img.shields.io/
+pypi/v/pandas-geojson) ![PyPI - Downloads](https://img.shields.io/pypi/dm/
+pandas-geojson) ![PyPI - License](https://img.shields.io/pypi/l/pandas-geojson)
+![Libraries.io SourceRank](https://img.shields.io/librariesio/sourcerank/pypi/
+pandas-geojson) # Getting Started Install the latest version of pandas-geojson
+using pip. ``` pip install pandas-geojson ``` ## Open GeoJSON Files Using the
+`read_geojson` function, you can easily read in GeoJSON data int the GeoJSON
+object. ```python import pandas_geojson as pdg geojson = pdg.read_geojson
+('datasets/National_Obesity_By_State.geojson') type(geojson) ```
 pandas_geojson.core.GeoJSON ## List Properties Pandas-GeoJSON utilizes
 properties to filter large geojson files. This functionallity helps you
 identify all of the properties in the geojson file so that you can choose a
 filter criteria. For more on filtering see [filter_geojson](#filter-geojson)
 ```python geojson.get_properties() ``` ['FID', 'NAME', 'Obesity',
 'SHAPE_Length', 'SHAPE_Area'] ## DataFrame to GeoJSON Pandas-GeoJSON makes it
 easy to convert a dataframe with coordinates into a GeoJSON object. Your
```

### Comparing `pandas_geojson-2.0.1/setup.py` & `pandas_geojson-2.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="pandas_geojson",
-    version="2.0.1",
+    version="2.1.0",
     description="Convert Pandas Dataframe to GeoJSON",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/jrasband-dev/pandas-geojson",
     author="Jayden Rasband",
     author_email="jayden.rasband@gmail.com",
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
     ],
     packages=["pandas_geojson"],
     include_package_data=True,
-    install_requires=["pandas"],
+    install_requires=[],
 )
```

