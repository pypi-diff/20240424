# Comparing `tmp/cefeste-1.2.1.tar.gz` & `tmp/cefeste-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cefeste-1.2.1.tar", last modified: Tue Apr  9 07:42:51 2024, max compression
+gzip compressed data, was "cefeste-1.2.2.tar", last modified: Wed Apr 24 07:27:10 2024, max compression
```

## Comparing `cefeste-1.2.1.tar` & `cefeste-1.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2024-04-09 07:42:51.901525 cefeste-1.2.1/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1073 2023-05-05 08:25:33.000000 cefeste-1.2.1/LICENCE
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3012 2024-04-09 07:42:51.897525 cefeste-1.2.1/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2321 2023-05-22 20:53:27.000000 cefeste-1.2.1/README.md
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      708 2024-04-09 07:01:51.000000 cefeste-1.2.1/pyproject.toml
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2024-04-09 07:42:51.901525 cefeste-1.2.1/setup.cfg
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      944 2024-04-09 07:01:39.000000 cefeste-1.2.1/setup.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2024-04-09 07:42:51.873525 cefeste-1.2.1/src/
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2024-04-09 07:42:51.881525 cefeste-1.2.1/src/cefeste/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3364 2023-05-05 08:25:33.000000 cefeste-1.2.1/src/cefeste/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      444 2023-05-05 08:25:33.000000 cefeste-1.2.1/src/cefeste/config.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2024-04-09 07:42:51.889525 cefeste-1.2.1/src/cefeste/elimination/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    15460 2023-10-03 14:22:59.000000 cefeste-1.2.1/src/cefeste/elimination/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    25917 2024-03-22 15:43:43.000000 cefeste-1.2.1/src/cefeste/elimination/shap_rfe.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2024-04-09 07:42:51.893525 cefeste-1.2.1/src/cefeste/selection/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    27806 2023-07-03 11:01:49.000000 cefeste-1.2.1/src/cefeste/selection/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10633 2023-10-03 14:22:59.000000 cefeste-1.2.1/src/cefeste/selection/explanatory.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    22536 2024-03-22 15:43:43.000000 cefeste-1.2.1/src/cefeste/selection/multivariate.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10439 2023-10-03 14:22:59.000000 cefeste-1.2.1/src/cefeste/selection/univariate.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2024-04-09 07:42:51.897525 cefeste-1.2.1/src/cefeste/transform/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     6330 2024-03-22 15:43:43.000000 cefeste-1.2.1/src/cefeste/transform/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3403 2024-03-22 15:43:43.000000 cefeste-1.2.1/src/cefeste/utils.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2024-04-09 07:42:51.897525 cefeste-1.2.1/src/cefeste.egg-info/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3012 2024-04-09 07:42:51.000000 cefeste-1.2.1/src/cefeste.egg-info/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      533 2024-04-09 07:42:51.000000 cefeste-1.2.1/src/cefeste.egg-info/SOURCES.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2024-04-09 07:42:51.000000 cefeste-1.2.1/src/cefeste.egg-info/dependency_links.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      131 2024-04-09 07:42:51.000000 cefeste-1.2.1/src/cefeste.egg-info/requires.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        8 2024-04-09 07:42:51.000000 cefeste-1.2.1/src/cefeste.egg-info/top_level.txt
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2024-04-24 07:27:10.784833 cefeste-1.2.2/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1073 2024-04-24 07:14:28.000000 cefeste-1.2.2/LICENCE
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3012 2024-04-24 07:27:10.780833 cefeste-1.2.2/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2321 2024-04-24 07:14:28.000000 cefeste-1.2.2/README.md
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      708 2024-04-24 07:26:02.000000 cefeste-1.2.2/pyproject.toml
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2024-04-24 07:27:10.784833 cefeste-1.2.2/setup.cfg
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      944 2024-04-24 07:25:48.000000 cefeste-1.2.2/setup.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2024-04-24 07:27:10.776832 cefeste-1.2.2/src/
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2024-04-24 07:27:10.776832 cefeste-1.2.2/src/cefeste/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3364 2024-04-24 07:14:28.000000 cefeste-1.2.2/src/cefeste/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      444 2024-04-24 07:14:28.000000 cefeste-1.2.2/src/cefeste/config.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2024-04-24 07:27:10.780833 cefeste-1.2.2/src/cefeste/elimination/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    15460 2024-04-24 07:14:28.000000 cefeste-1.2.2/src/cefeste/elimination/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    25917 2024-04-24 07:14:28.000000 cefeste-1.2.2/src/cefeste/elimination/shap_rfe.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2024-04-24 07:27:10.780833 cefeste-1.2.2/src/cefeste/selection/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    27806 2024-04-24 07:14:28.000000 cefeste-1.2.2/src/cefeste/selection/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10633 2024-04-24 07:14:28.000000 cefeste-1.2.2/src/cefeste/selection/explanatory.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    22536 2024-04-24 07:14:28.000000 cefeste-1.2.2/src/cefeste/selection/multivariate.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10439 2024-04-24 07:14:28.000000 cefeste-1.2.2/src/cefeste/selection/univariate.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2024-04-24 07:27:10.780833 cefeste-1.2.2/src/cefeste/transform/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     6330 2024-04-24 07:14:28.000000 cefeste-1.2.2/src/cefeste/transform/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3403 2024-04-24 07:14:28.000000 cefeste-1.2.2/src/cefeste/utils.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2024-04-24 07:27:10.780833 cefeste-1.2.2/src/cefeste.egg-info/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3012 2024-04-24 07:27:10.000000 cefeste-1.2.2/src/cefeste.egg-info/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      533 2024-04-24 07:27:10.000000 cefeste-1.2.2/src/cefeste.egg-info/SOURCES.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2024-04-24 07:27:10.000000 cefeste-1.2.2/src/cefeste.egg-info/dependency_links.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      131 2024-04-24 07:27:10.000000 cefeste-1.2.2/src/cefeste.egg-info/requires.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        8 2024-04-24 07:27:10.000000 cefeste-1.2.2/src/cefeste.egg-info/top_level.txt
```

### Comparing `cefeste-1.2.1/LICENCE` & `cefeste-1.2.2/LICENCE`

 * *Files identical despite different names*

### Comparing `cefeste-1.2.1/PKG-INFO` & `cefeste-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cefeste
-Version: 1.2.1
+Version: 1.2.2
 Summary: Feature Selection and Elimination
 Home-page: https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Author: DAT Team
 Project-URL: Homepage, https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENCE
-Requires-Dist: typed-ast==1.5.4
+Requires-Dist: typed-ast>=1.5.4
 Requires-Dist: numpy==1.22.4
-Requires-Dist: pandas==1.4.2
+Requires-Dist: pandas>=1.4.2
 Requires-Dist: scikit-learn>=1.1.1
 Requires-Dist: scipy>=1.8.1
 Requires-Dist: statsmodels>=0.13.2
 Requires-Dist: PyYAML>=6.0
 Requires-Dist: shap==0.41.0
 Requires-Dist: ipython
```

### Comparing `cefeste-1.2.1/README.md` & `cefeste-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cefeste-1.2.1/pyproject.toml` & `cefeste-1.2.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cefeste"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
   { name="DAT Team" },
 ]
 description = "Feature Selection and Elimination"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies=[
-    "typed-ast==1.5.4",
+    "typed-ast>=1.5.4",
     "numpy==1.22.4",
-    "pandas==1.4.2",
+    "pandas>=1.4.2",
     "scikit-learn>=1.1.1",
     "scipy>=1.8.1",
     "statsmodels>=0.13.2",
     "PyYAML>=6.0",
     "shap==0.41.0",
     "ipython",
 ]
```

### Comparing `cefeste-1.2.1/setup.py` & `cefeste-1.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ce-feste",
-    version="1.2.0",
+    version="1.2.2",
     description="Package for Feature Selection, Transformation, Elimination",
     author="DAT Team",
     url="https://dev.azure.com/credem-data/DAT/_git/ce-feste",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
@@ -14,17 +14,17 @@
         "Programming Language :: Python :: 3 :: Only",
     ],
     packages=find_packages(where="src", exclude=["test"]),
     package_dir={"": "src"},
     # Usato solo con 3.9 e 3.10
     python_requires=">=3.9, <4",
     install_requires=[
-        "typed-ast==1.5.4",
+        "typed-ast>=1.5.4",
         "numpy==1.22.4",
-        "pandas==1.4.2",
+        "pandas>=1.4.2",
         "scikit-learn>=1.1.1",
         "scipy>=1.8.1",
         "statsmodels>=0.13.2",
         "PyYAML>=6.0",
         "shap==0.41.0",
         "ipython",
     ],
```

### Comparing `cefeste-1.2.1/src/cefeste/__init__.py` & `cefeste-1.2.2/src/cefeste/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.2.1/src/cefeste/elimination/__init__.py` & `cefeste-1.2.2/src/cefeste/elimination/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.2.1/src/cefeste/elimination/shap_rfe.py` & `cefeste-1.2.2/src/cefeste/elimination/shap_rfe.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.2.1/src/cefeste/selection/__init__.py` & `cefeste-1.2.2/src/cefeste/selection/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.2.1/src/cefeste/selection/explanatory.py` & `cefeste-1.2.2/src/cefeste/selection/explanatory.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.2.1/src/cefeste/selection/multivariate.py` & `cefeste-1.2.2/src/cefeste/selection/multivariate.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.2.1/src/cefeste/selection/univariate.py` & `cefeste-1.2.2/src/cefeste/selection/univariate.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.2.1/src/cefeste/transform/__init__.py` & `cefeste-1.2.2/src/cefeste/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.2.1/src/cefeste/utils.py` & `cefeste-1.2.2/src/cefeste/utils.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.2.1/src/cefeste.egg-info/PKG-INFO` & `cefeste-1.2.2/src/cefeste.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cefeste
-Version: 1.2.1
+Version: 1.2.2
 Summary: Feature Selection and Elimination
 Home-page: https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Author: DAT Team
 Project-URL: Homepage, https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENCE
-Requires-Dist: typed-ast==1.5.4
+Requires-Dist: typed-ast>=1.5.4
 Requires-Dist: numpy==1.22.4
-Requires-Dist: pandas==1.4.2
+Requires-Dist: pandas>=1.4.2
 Requires-Dist: scikit-learn>=1.1.1
 Requires-Dist: scipy>=1.8.1
 Requires-Dist: statsmodels>=0.13.2
 Requires-Dist: PyYAML>=6.0
 Requires-Dist: shap==0.41.0
 Requires-Dist: ipython
```

### Comparing `cefeste-1.2.1/src/cefeste.egg-info/SOURCES.txt` & `cefeste-1.2.2/src/cefeste.egg-info/SOURCES.txt`

 * *Files identical despite different names*

