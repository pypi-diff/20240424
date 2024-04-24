# Comparing `tmp/tesci-1.0.0.tar.gz` & `tmp/tesci-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tesci-1.0.0.tar", last modified: Thu Mar 14 19:46:51 2024, max compression
+gzip compressed data, was "tesci-1.0.1.tar", last modified: Wed Apr 24 13:11:53 2024, max compression
```

## Comparing `tesci-1.0.0.tar` & `tesci-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 19:46:51.811599 tesci-1.0.0/
--rw-rw-rw-   0        0        0    11558 2024-03-09 16:44:12.000000 tesci-1.0.0/LICENSE-APACHE
--rw-rw-rw-   0        0        0     1098 2024-03-09 16:44:12.000000 tesci-1.0.0/LICENSE-MIT
--rw-rw-rw-   0        0        0     4193 2024-03-14 19:46:51.809616 tesci-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3074 2024-03-14 19:34:15.000000 tesci-1.0.0/README.md
--rw-rw-rw-   0        0        0     1199 2024-03-14 19:40:22.000000 tesci-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-14 19:46:51.811599 tesci-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-14 19:46:51.771597 tesci-1.0.0/tesci/
--rw-rw-rw-   0        0        0        0 2023-08-08 16:20:31.000000 tesci-1.0.0/tesci/__init__.py
--rw-rw-rw-   0        0        0     2492 2024-03-14 18:00:55.000000 tesci-1.0.0/tesci/release.py
-drwxrwxrwx   0        0        0        0 2024-03-14 19:46:51.794621 tesci-1.0.0/tesci/scripts/
--rw-rw-rw-   0        0        0        0 2023-08-26 15:16:30.000000 tesci-1.0.0/tesci/scripts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 19:46:51.796618 tesci-1.0.0/tesci/scripts/aggregate/
--rw-rw-rw-   0        0        0     1333 2024-03-14 18:02:00.000000 tesci-1.0.0/tesci/scripts/aggregate/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 19:46:51.798620 tesci-1.0.0/tesci/scripts/apply/
--rw-rw-rw-   0        0        0      546 2024-03-14 18:02:03.000000 tesci-1.0.0/tesci/scripts/apply/__init__.py
--rw-rw-rw-   0        0        0     6505 2024-03-14 19:45:23.000000 tesci-1.0.0/tesci/scripts/context.py
-drwxrwxrwx   0        0        0        0 2024-03-14 19:46:51.800616 tesci-1.0.0/tesci/scripts/include/
--rw-rw-rw-   0        0        0      352 2024-03-14 18:02:05.000000 tesci-1.0.0/tesci/scripts/include/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 19:46:51.801620 tesci-1.0.0/tesci/scripts/join/
--rw-rw-rw-   0        0        0       95 2023-12-04 19:40:35.000000 tesci-1.0.0/tesci/scripts/join/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 19:46:51.803605 tesci-1.0.0/tesci/scripts/preview/
--rw-rw-rw-   0        0        0      201 2024-03-14 18:02:07.000000 tesci-1.0.0/tesci/scripts/preview/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 19:46:51.805596 tesci-1.0.0/tesci/scripts/release/
--rw-rw-rw-   0        0        0      660 2024-03-14 18:02:09.000000 tesci-1.0.0/tesci/scripts/release/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 19:46:51.806607 tesci-1.0.0/tesci/scripts/similarity/
--rw-rw-rw-   0        0        0     1349 2024-03-14 18:03:03.000000 tesci-1.0.0/tesci/scripts/similarity/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 19:46:51.807597 tesci-1.0.0/tesci/scripts/start/
--rw-rw-rw-   0        0        0      406 2024-03-14 18:00:36.000000 tesci-1.0.0/tesci/scripts/start/__init__.py
--rw-rw-rw-   0        0        0      704 2024-03-14 17:59:54.000000 tesci-1.0.0/tesci/scripts/tesci.py
--rw-rw-rw-   0        0        0    12733 2024-03-14 18:00:59.000000 tesci-1.0.0/tesci/similarity.py
--rw-rw-rw-   0        0        0     8724 2024-03-14 18:01:39.000000 tesci-1.0.0/tesci/transformations.py
--rw-rw-rw-   0        0        0      580 2023-12-20 22:44:31.000000 tesci-1.0.0/tesci/types.py
-drwxrwxrwx   0        0        0        0 2024-03-14 19:46:51.809616 tesci-1.0.0/tesci.egg-info/
--rw-rw-rw-   0        0        0     4193 2024-03-14 19:46:51.000000 tesci-1.0.0/tesci.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      666 2024-03-14 19:46:51.000000 tesci-1.0.0/tesci.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 19:46:51.000000 tesci-1.0.0/tesci.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-03-14 19:46:51.000000 tesci-1.0.0/tesci.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      133 2024-03-14 19:46:51.000000 tesci-1.0.0/tesci.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-03-14 19:46:51.000000 tesci-1.0.0/tesci.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 13:11:53.206456 tesci-1.0.1/
+-rw-rw-rw-   0        0        0    11558 2024-03-09 16:44:12.000000 tesci-1.0.1/LICENSE-APACHE
+-rw-rw-rw-   0        0        0     1098 2024-03-09 16:44:12.000000 tesci-1.0.1/LICENSE-MIT
+-rw-rw-rw-   0        0        0     4185 2024-04-24 13:11:53.205460 tesci-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3066 2024-04-14 18:00:51.000000 tesci-1.0.1/README.md
+-rw-rw-rw-   0        0        0     1199 2024-04-24 13:10:13.000000 tesci-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-24 13:11:53.206456 tesci-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 13:11:53.163461 tesci-1.0.1/tesci/
+-rw-rw-rw-   0        0        0        0 2023-08-08 16:20:31.000000 tesci-1.0.1/tesci/__init__.py
+-rw-rw-rw-   0        0        0     2492 2024-04-03 21:41:33.000000 tesci-1.0.1/tesci/release.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:11:53.193464 tesci-1.0.1/tesci/scripts/
+-rw-rw-rw-   0        0        0        0 2023-08-26 15:16:30.000000 tesci-1.0.1/tesci/scripts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:11:53.194455 tesci-1.0.1/tesci/scripts/aggregate/
+-rw-rw-rw-   0        0        0     1333 2024-03-14 18:02:00.000000 tesci-1.0.1/tesci/scripts/aggregate/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:11:53.195462 tesci-1.0.1/tesci/scripts/apply/
+-rw-rw-rw-   0        0        0      546 2024-03-14 18:02:03.000000 tesci-1.0.1/tesci/scripts/apply/__init__.py
+-rw-rw-rw-   0        0        0     6505 2024-03-14 19:45:23.000000 tesci-1.0.1/tesci/scripts/context.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:11:53.197457 tesci-1.0.1/tesci/scripts/include/
+-rw-rw-rw-   0        0        0      352 2024-03-14 18:02:05.000000 tesci-1.0.1/tesci/scripts/include/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:11:53.198457 tesci-1.0.1/tesci/scripts/join/
+-rw-rw-rw-   0        0        0       95 2023-12-04 19:40:35.000000 tesci-1.0.1/tesci/scripts/join/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:11:53.198457 tesci-1.0.1/tesci/scripts/preview/
+-rw-rw-rw-   0        0        0      201 2024-03-14 18:02:07.000000 tesci-1.0.1/tesci/scripts/preview/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:11:53.199455 tesci-1.0.1/tesci/scripts/release/
+-rw-rw-rw-   0        0        0      660 2024-03-14 18:02:09.000000 tesci-1.0.1/tesci/scripts/release/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:11:53.200457 tesci-1.0.1/tesci/scripts/similarity/
+-rw-rw-rw-   0        0        0     1349 2024-03-14 18:03:03.000000 tesci-1.0.1/tesci/scripts/similarity/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:11:53.201457 tesci-1.0.1/tesci/scripts/start/
+-rw-rw-rw-   0        0        0      406 2024-03-14 18:00:36.000000 tesci-1.0.1/tesci/scripts/start/__init__.py
+-rw-rw-rw-   0        0        0      704 2024-03-14 17:59:54.000000 tesci-1.0.1/tesci/scripts/tesci.py
+-rw-rw-rw-   0        0        0    13970 2024-04-24 13:08:08.000000 tesci-1.0.1/tesci/similarity.py
+-rw-rw-rw-   0        0        0     8724 2024-03-14 18:01:39.000000 tesci-1.0.1/tesci/transformations.py
+-rw-rw-rw-   0        0        0      580 2023-12-20 22:44:31.000000 tesci-1.0.1/tesci/types.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:11:53.202458 tesci-1.0.1/tesci.egg-info/
+-rw-rw-rw-   0        0        0     4185 2024-04-24 13:11:53.000000 tesci-1.0.1/tesci.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      666 2024-04-24 13:11:53.000000 tesci-1.0.1/tesci.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 13:11:53.000000 tesci-1.0.1/tesci.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-24 13:11:53.000000 tesci-1.0.1/tesci.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      133 2024-04-24 13:11:53.000000 tesci-1.0.1/tesci.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-24 13:11:53.000000 tesci-1.0.1/tesci.egg-info/top_level.txt
```

### Comparing `tesci-1.0.0/LICENSE-APACHE` & `tesci-1.0.1/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `tesci-1.0.0/LICENSE-MIT` & `tesci-1.0.1/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `tesci-1.0.0/PKG-INFO` & `tesci-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tesci
-Version: 1.0.0
+Version: 1.0.1
 Summary: A toolkit to aid in scientific mapping
 Keywords: scientific mapping,merging data sources
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
@@ -29,15 +29,15 @@
 Requires-Dist: rapidfuzz>=3.5.2
 Requires-Dist: importlib-metadata; python_version < "3.8"
 
 # tesci
 
 ## An interactive toolkit for merging data from multiple citation databases
 
-[![PyPI](https://img.shields.io/pypi/v/tesci.svg)](https://img.shields.io/pypi/v/tesci.svg)
+[![PyPI](https://img.shields.io/pypi/v/tesci.svg)](https://pypi.org/project/tesci/)
 [![License-1]( https://img.shields.io/badge/License-Apache-blue.svg)](https://img.shields.io/badge/License-Apache-blue.svg)
 [![License-2]( https://img.shields.io/badge/License-MIT-green.svg)](https://img.shields.io/badge/License-MIT-green.svg)
 [![Python-Versions](https://img.shields.io/pypi/pyversions/tesci.svg)](https://img.shields.io/pypi/pyversions/tesci.svg)
 
 ## Overview
 
 `TeslaSCIToolkit` (abbrev. `tesci`) is a scientific mapping tool that comes with the following features:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tesci Version: 1.0.0 Summary: A toolkit to aid in
+Metadata-Version: 2.1 Name: tesci Version: 1.0.1 Summary: A toolkit to aid in
 scientific mapping Keywords: scientific mapping,merging data sources
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Science/Research Classifier: Topic :: Scientific/
 Engineering Classifier: License :: OSI Approved :: MIT License Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3.11 Classifier:
@@ -10,16 +10,16 @@
 Independent Requires-Python: >=3.11 Description-Content-Type: text/markdown
 License-File: LICENSE-APACHE License-File: LICENSE-MIT Requires-Dist:
 click>=8.1 Requires-Dist: requests Requires-Dist: pandas Requires-Dist: pyyaml
 Requires-Dist: PyGithub>=2.1.1 Requires-Dist: attrs Requires-Dist: xlrd
 Requires-Dist: openpyxl Requires-Dist: rapidfuzz>=3.5.2 Requires-Dist:
 importlib-metadata; python_version < "3.8" # tesci ## An interactive toolkit
 for merging data from multiple citation databases [![PyPI](https://
-img.shields.io/pypi/v/tesci.svg)](https://img.shields.io/pypi/v/tesci.svg) [!
-[License-1]( https://img.shields.io/badge/License-Apache-blue.svg)](https://
+img.shields.io/pypi/v/tesci.svg)](https://pypi.org/project/tesci/) [![License-
+1]( https://img.shields.io/badge/License-Apache-blue.svg)](https://
 img.shields.io/badge/License-Apache-blue.svg) [![License-2]( https://
 img.shields.io/badge/License-MIT-green.svg)](https://img.shields.io/badge/
 License-MIT-green.svg) [![Python-Versions](https://img.shields.io/pypi/
 pyversions/tesci.svg)](https://img.shields.io/pypi/pyversions/tesci.svg) ##
 Overview `TeslaSCIToolkit` (abbrev. `tesci`) is a scientific mapping tool that
 comes with the following features: 1. Merging data from multiple citation
 databases 2. Restricting access to sensitive columns in data sources with
```

### Comparing `tesci-1.0.0/README.md` & `tesci-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # tesci
 
 ## An interactive toolkit for merging data from multiple citation databases
 
-[![PyPI](https://img.shields.io/pypi/v/tesci.svg)](https://img.shields.io/pypi/v/tesci.svg)
+[![PyPI](https://img.shields.io/pypi/v/tesci.svg)](https://pypi.org/project/tesci/)
 [![License-1]( https://img.shields.io/badge/License-Apache-blue.svg)](https://img.shields.io/badge/License-Apache-blue.svg)
 [![License-2]( https://img.shields.io/badge/License-MIT-green.svg)](https://img.shields.io/badge/License-MIT-green.svg)
 [![Python-Versions](https://img.shields.io/pypi/pyversions/tesci.svg)](https://img.shields.io/pypi/pyversions/tesci.svg)
 
 ## Overview
 
 `TeslaSCIToolkit` (abbrev. `tesci`) is a scientific mapping tool that comes with the following features:
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
 # tesci ## An interactive toolkit for merging data from multiple citation
-databases [![PyPI](https://img.shields.io/pypi/v/tesci.svg)](https://
-img.shields.io/pypi/v/tesci.svg) [![License-1]( https://img.shields.io/badge/
-License-Apache-blue.svg)](https://img.shields.io/badge/License-Apache-blue.svg)
-[![License-2]( https://img.shields.io/badge/License-MIT-green.svg)](https://
-img.shields.io/badge/License-MIT-green.svg) [![Python-Versions](https://
-img.shields.io/pypi/pyversions/tesci.svg)](https://img.shields.io/pypi/
-pyversions/tesci.svg) ## Overview `TeslaSCIToolkit` (abbrev. `tesci`) is a
-scientific mapping tool that comes with the following features: 1. Merging data
-from multiple citation databases 2. Restricting access to sensitive columns in
-data sources with aggregations 3. Exporting transformed data into other
-repositories 4. CI/CD integration, currently GitHub Actions For examples and
-use-cases, see [examples](examples/) directory. ## Quickstart ### Aggregating
-data from a single database source To create an aggregation of [`simple.csv`]
-(examples/simple/simple.csv) based on average `salary` and `age`. #### 1.
-Interactive approach ```properties tesci start -d simple.csv -o exported.csvâ
-tesci aggregate avg -c salary -a avg_salaryâ tesci aggregate avg -c age -
+databases [![PyPI](https://img.shields.io/pypi/v/tesci.svg)](https://pypi.org/
+project/tesci/) [![License-1]( https://img.shields.io/badge/License-Apache-
+blue.svg)](https://img.shields.io/badge/License-Apache-blue.svg) [![License-2]
+( https://img.shields.io/badge/License-MIT-green.svg)](https://img.shields.io/
+badge/License-MIT-green.svg) [![Python-Versions](https://img.shields.io/pypi/
+pyversions/tesci.svg)](https://img.shields.io/pypi/pyversions/tesci.svg) ##
+Overview `TeslaSCIToolkit` (abbrev. `tesci`) is a scientific mapping tool that
+comes with the following features: 1. Merging data from multiple citation
+databases 2. Restricting access to sensitive columns in data sources with
+aggregations 3. Exporting transformed data into other repositories 4. CI/CD
+integration, currently GitHub Actions For examples and use-cases, see
+[examples](examples/) directory. ## Quickstart ### Aggregating data from a
+single database source To create an aggregation of [`simple.csv`](examples/
+simple/simple.csv) based on average `salary` and `age`. #### 1. Interactive
+approach ```properties tesci start -d simple.csv -o exported.csvâ tesci
+aggregate avg -c salary -a avg_salaryâ tesci aggregate avg -c age -
 a avg_ageâ tesci applyâ ``` #### 2. Configuration approach ```yml
 aggregate:â - alias: avg_salaryâ column: salaryâ function: avgâ -
 alias: avg_ageâ column: ageâ function: avgâ data:â dest:
 exported.csvâ src: simple.csv ``` The result is a transformation from
 `simple.csv` to `exported.csv`: | | | | |--|--|--| |
 iidd nnaammee          eemmaaiill              pphhoonnee--nnuummbbeerr aaggee ssaallaarryy
 1  John Doe      john@mail.com      1234567890   33  100000
```

### Comparing `tesci-1.0.0/pyproject.toml` & `tesci-1.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tesci"
-version = "1.0.0"
+version = "1.0.1"
 description = "A toolkit to aid in scientific mapping"
 readme = "README.md"
 keywords = ["scientific mapping", "merging data sources"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
```

### Comparing `tesci-1.0.0/tesci/release.py` & `tesci-1.0.1/tesci/release.py`

 * *Files identical despite different names*

### Comparing `tesci-1.0.0/tesci/scripts/aggregate/__init__.py` & `tesci-1.0.1/tesci/scripts/aggregate/__init__.py`

 * *Files identical despite different names*

### Comparing `tesci-1.0.0/tesci/scripts/apply/__init__.py` & `tesci-1.0.1/tesci/scripts/apply/__init__.py`

 * *Files identical despite different names*

### Comparing `tesci-1.0.0/tesci/scripts/context.py` & `tesci-1.0.1/tesci/scripts/context.py`

 * *Files identical despite different names*

### Comparing `tesci-1.0.0/tesci/scripts/release/__init__.py` & `tesci-1.0.1/tesci/scripts/release/__init__.py`

 * *Files identical despite different names*

### Comparing `tesci-1.0.0/tesci/scripts/similarity/__init__.py` & `tesci-1.0.1/tesci/scripts/similarity/__init__.py`

 * *Files identical despite different names*

### Comparing `tesci-1.0.0/tesci/scripts/tesci.py` & `tesci-1.0.1/tesci/scripts/tesci.py`

 * *Files identical despite different names*

### Comparing `tesci-1.0.0/tesci/similarity.py` & `tesci-1.0.1/tesci/similarity.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,34 +82,61 @@
     if replace is not None:
         df2[from_col] = df2[from_col].replace(replace)
     if truncate_after is not None:
         for truncate_str in truncate_after:
             df2[from_col] = df2[from_col].str.split(truncate_str).str[0]
 
 
+def assert_no_duplicate_columns(from_columns, into_columns):
+    err_msg = ""
+    for col in from_columns:
+        if from_columns.count(col.lower()) > 1:
+            err_msg += f"Duplicate column \"{col.upper()}\" found in 'from' columns.\n"
+    for col in into_columns:
+        if into_columns.count(col.lower()) > 1:
+            err_msg += f"Duplicate column \"{col.upper()}\" found in 'into' columns.\n"
+
+    if len(err_msg) > 0:
+        err_msg += (
+            "\nEnsure that each column in your configuration file is unique in 'from' and 'into'."
+        )
+        raise ValueError(err_msg)
+
+
 def merge(first_src: Path | None, second_src: Path | None, dest: Path | None):
     config = Config()
     if "similarity_config" not in config.content.get("join", {}).keys():
         logging.info(
             "No similarity_config to apply to the dataset. Are you using a config file that has similarity_config?"
         )
         return
 
     columns = config.content["join"]["similarity_config"]["merge"]["columns"]
 
+    from_columns = [col["from_"].lower() for col in columns]
+    into_columns = [col["into_"].lower() for col in columns]
+    assert_no_duplicate_columns(from_columns, into_columns)
+
     if first_src is not None and second_src is not None:
         first_src = Path(first_src)
         second_src = Path(second_src)
         df1 = JoinSource(Reader(first_src).load(), None).df
         df2 = JoinSource(Reader(second_src).load(), None).df
     else:
         data = DataSource.get()
         df1 = data.join_sources.sources[0].df
         df2 = data.join_sources.sources[1].df
 
+    df1.rename(columns=str.lower, inplace=True)
+    df2.rename(columns=str.lower, inplace=True)
+
+    for column in columns:
+        column["from_"] = column["from_"].lower()
+        column["into_"] = column["into_"].lower()
+
     if config.content["join"]["similarity_config"]["merge"].get("drop_duplicates"):
         df1.drop_duplicates(inplace=True)
         df2.drop_duplicates(inplace=True)
 
     for column in columns:
         from_col = column["from_"]
         into_col = column["into_"]
@@ -295,15 +322,17 @@
             row.rename({from_col: into_col}, inplace=True)
 
     exact_matches_df = pd.DataFrame(exact_matches_series)
     suggested_matches_df = pd.DataFrame(suggested_matches_series)
     potential_matches_df = pd.DataFrame(potential_matches_series)
     no_matches_df = pd.DataFrame(no_matches_series)
     no_matches_df = pd.concat([no_matches_df, potential_matches_df])
-
+    final_df = pd.concat(
+        [exact_matches_df, suggested_matches_df, potential_matches_df, no_matches_df]
+    )
     analytics = {
         "exact_matches": len(exact_matches),
         "suggested_matches": len(suggested_matches),
         "potential_matches": len(potential_matches),
         "no_matches": len(no_matches),
         "sum of merged matches": len(exact_matches) + len(suggested_matches),
         "sum of non-merged matches": len(potential_matches) + len(no_matches),
@@ -311,15 +340,15 @@
         + len(suggested_matches)
         + len(potential_matches)
         + len(no_matches),
         "df2 size": len(df2),
         "df1 size": len(df1),
         "merged_df size": len(merged_df),
         "duplicates in merged_df": len(
-            merged_df[merged_df.duplicated(subset="Title", keep="first")]
+            merged_df[merged_df.duplicated(subset="title", keep="first")]
         ),
     }
     import pprint
 
     pp = pprint.PrettyPrinter(indent=4)
     pp.pprint(analytics)
     df = merged_df
@@ -333,7 +362,8 @@
     ):
         DataSource.save_to_file(
             df,
             Config(),
             name_override=f"config-{name}-matches.xls",
             path_override=path_override,
         )
+    DataSource.save_to_file(final_df, Config(), name_override="config-final.xls")
```

### Comparing `tesci-1.0.0/tesci/transformations.py` & `tesci-1.0.1/tesci/transformations.py`

 * *Files identical despite different names*

### Comparing `tesci-1.0.0/tesci/types.py` & `tesci-1.0.1/tesci/types.py`

 * *Files identical despite different names*

### Comparing `tesci-1.0.0/tesci.egg-info/PKG-INFO` & `tesci-1.0.1/tesci.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tesci
-Version: 1.0.0
+Version: 1.0.1
 Summary: A toolkit to aid in scientific mapping
 Keywords: scientific mapping,merging data sources
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
@@ -29,15 +29,15 @@
 Requires-Dist: rapidfuzz>=3.5.2
 Requires-Dist: importlib-metadata; python_version < "3.8"
 
 # tesci
 
 ## An interactive toolkit for merging data from multiple citation databases
 
-[![PyPI](https://img.shields.io/pypi/v/tesci.svg)](https://img.shields.io/pypi/v/tesci.svg)
+[![PyPI](https://img.shields.io/pypi/v/tesci.svg)](https://pypi.org/project/tesci/)
 [![License-1]( https://img.shields.io/badge/License-Apache-blue.svg)](https://img.shields.io/badge/License-Apache-blue.svg)
 [![License-2]( https://img.shields.io/badge/License-MIT-green.svg)](https://img.shields.io/badge/License-MIT-green.svg)
 [![Python-Versions](https://img.shields.io/pypi/pyversions/tesci.svg)](https://img.shields.io/pypi/pyversions/tesci.svg)
 
 ## Overview
 
 `TeslaSCIToolkit` (abbrev. `tesci`) is a scientific mapping tool that comes with the following features:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tesci Version: 1.0.0 Summary: A toolkit to aid in
+Metadata-Version: 2.1 Name: tesci Version: 1.0.1 Summary: A toolkit to aid in
 scientific mapping Keywords: scientific mapping,merging data sources
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Science/Research Classifier: Topic :: Scientific/
 Engineering Classifier: License :: OSI Approved :: MIT License Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3.11 Classifier:
@@ -10,16 +10,16 @@
 Independent Requires-Python: >=3.11 Description-Content-Type: text/markdown
 License-File: LICENSE-APACHE License-File: LICENSE-MIT Requires-Dist:
 click>=8.1 Requires-Dist: requests Requires-Dist: pandas Requires-Dist: pyyaml
 Requires-Dist: PyGithub>=2.1.1 Requires-Dist: attrs Requires-Dist: xlrd
 Requires-Dist: openpyxl Requires-Dist: rapidfuzz>=3.5.2 Requires-Dist:
 importlib-metadata; python_version < "3.8" # tesci ## An interactive toolkit
 for merging data from multiple citation databases [![PyPI](https://
-img.shields.io/pypi/v/tesci.svg)](https://img.shields.io/pypi/v/tesci.svg) [!
-[License-1]( https://img.shields.io/badge/License-Apache-blue.svg)](https://
+img.shields.io/pypi/v/tesci.svg)](https://pypi.org/project/tesci/) [![License-
+1]( https://img.shields.io/badge/License-Apache-blue.svg)](https://
 img.shields.io/badge/License-Apache-blue.svg) [![License-2]( https://
 img.shields.io/badge/License-MIT-green.svg)](https://img.shields.io/badge/
 License-MIT-green.svg) [![Python-Versions](https://img.shields.io/pypi/
 pyversions/tesci.svg)](https://img.shields.io/pypi/pyversions/tesci.svg) ##
 Overview `TeslaSCIToolkit` (abbrev. `tesci`) is a scientific mapping tool that
 comes with the following features: 1. Merging data from multiple citation
 databases 2. Restricting access to sensitive columns in data sources with
```

### Comparing `tesci-1.0.0/tesci.egg-info/SOURCES.txt` & `tesci-1.0.1/tesci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

