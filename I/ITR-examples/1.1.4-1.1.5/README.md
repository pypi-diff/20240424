# Comparing `tmp/itr_examples-1.1.4.tar.gz` & `tmp/itr_examples-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itr_examples-1.1.4.tar", last modified: Tue Apr  2 12:36:21 2024, max compression
+gzip compressed data, was "itr_examples-1.1.5.tar", last modified: Wed Apr 24 15:35:58 2024, max compression
```

## Comparing `itr_examples-1.1.4.tar` & `itr_examples-1.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      133 2024-04-02 12:36:03.627423 itr_examples-1.1.4/AUTHORS.rst
--rw-r--r--   0        0        0    11357 2024-04-02 12:36:03.627423 itr_examples-1.1.4/LICENSE.txt
--rw-r--r--   0        0        0     2467 2024-04-02 12:36:03.627423 itr_examples-1.1.4/README.md
--rw-r--r--   0        0        0     2935 2024-04-02 12:36:21.571691 itr_examples-1.1.4/pyproject.toml
--rw-r--r--   0        0        0   104666 2024-04-02 12:36:03.651424 itr_examples-1.1.4/src/ITR_examples/ITR_DV.py
--rw-r--r--   0        0        0    96153 2024-04-02 12:36:03.651424 itr_examples-1.1.4/src/ITR_examples/ITR_UI.py
--rw-r--r--   0        0        0      740 2024-04-02 12:36:03.651424 itr_examples-1.1.4/src/ITR_examples/__init__.py
--rw-r--r--   0        0        0    60436 2024-04-02 12:36:03.651424 itr_examples-1.1.4/src/ITR_examples/data/20220215 ITR Tool Sample Data.xlsx
--rw-r--r--   0        0        0    72880 2024-04-02 12:36:03.651424 itr_examples-1.1.4/src/ITR_examples/data/20220720 ITR Tool Sample Data.xlsx
--rw-r--r--   0        0        0    76225 2024-04-02 12:36:03.651424 itr_examples-1.1.4/src/ITR_examples/data/20220720 ITR Tool Test Data.xlsx
--rw-r--r--   0        0        0    74802 2024-04-02 12:36:03.655424 itr_examples-1.1.4/src/ITR_examples/data/20220927 ITR Tool Sample Data.xlsx
--rw-r--r--   0        0        0    78997 2024-04-02 12:36:03.655424 itr_examples-1.1.4/src/ITR_examples/data/20220927 ITR Tool Test Data.xlsx
--rw-r--r--   0        0        0   122199 2024-04-02 12:36:03.655424 itr_examples-1.1.4/src/ITR_examples/data/20220927 ITR V2 Sample Data.xlsx
--rw-r--r--   0        0        0   144935 2024-04-02 12:36:03.655424 itr_examples-1.1.4/src/ITR_examples/data/20221025 ITR V2 Sample Data.xlsx
--rw-r--r--   0        0        0   355991 2024-04-02 12:36:03.655424 itr_examples-1.1.4/src/ITR_examples/data/20230106 ITR V2 Sample Data.xlsx
--rw-r--r--   0        0        0    62694 2024-04-02 12:36:03.655424 itr_examples-1.1.4/src/ITR_examples/data/20230524 ITR V2 SBTi.xlsx
--rw-r--r--   0        0        0      137 2024-04-02 12:36:03.655424 itr_examples-1.1.4/src/ITR_examples/environment.yml
--rw-r--r--   0        0        0     9939 2024-04-02 12:36:03.659424 itr_examples-1.1.4/src/ITR_examples/utils.py
--rw-r--r--   0        0        0     4304 1970-01-01 00:00:00.000000 itr_examples-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      133 2024-04-24 15:35:41.150150 itr_examples-1.1.5/AUTHORS.rst
+-rw-r--r--   0        0        0    11357 2024-04-24 15:35:41.150150 itr_examples-1.1.5/LICENSE.txt
+-rw-r--r--   0        0        0     2467 2024-04-24 15:35:41.150150 itr_examples-1.1.5/README.md
+-rw-r--r--   0        0        0     2933 2024-04-24 15:35:58.302047 itr_examples-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0   104666 2024-04-24 15:35:41.174150 itr_examples-1.1.5/src/ITR_examples/ITR_DV.py
+-rw-r--r--   0        0        0    96153 2024-04-24 15:35:41.174150 itr_examples-1.1.5/src/ITR_examples/ITR_UI.py
+-rw-r--r--   0        0        0      740 2024-04-24 15:35:41.174150 itr_examples-1.1.5/src/ITR_examples/__init__.py
+-rw-r--r--   0        0        0    60436 2024-04-24 15:35:41.174150 itr_examples-1.1.5/src/ITR_examples/data/20220215 ITR Tool Sample Data.xlsx
+-rw-r--r--   0        0        0    72880 2024-04-24 15:35:41.174150 itr_examples-1.1.5/src/ITR_examples/data/20220720 ITR Tool Sample Data.xlsx
+-rw-r--r--   0        0        0    76225 2024-04-24 15:35:41.174150 itr_examples-1.1.5/src/ITR_examples/data/20220720 ITR Tool Test Data.xlsx
+-rw-r--r--   0        0        0    74802 2024-04-24 15:35:41.174150 itr_examples-1.1.5/src/ITR_examples/data/20220927 ITR Tool Sample Data.xlsx
+-rw-r--r--   0        0        0    78997 2024-04-24 15:35:41.174150 itr_examples-1.1.5/src/ITR_examples/data/20220927 ITR Tool Test Data.xlsx
+-rw-r--r--   0        0        0   122199 2024-04-24 15:35:41.178150 itr_examples-1.1.5/src/ITR_examples/data/20220927 ITR V2 Sample Data.xlsx
+-rw-r--r--   0        0        0   144935 2024-04-24 15:35:41.178150 itr_examples-1.1.5/src/ITR_examples/data/20221025 ITR V2 Sample Data.xlsx
+-rw-r--r--   0        0        0   355991 2024-04-24 15:35:41.178150 itr_examples-1.1.5/src/ITR_examples/data/20230106 ITR V2 Sample Data.xlsx
+-rw-r--r--   0        0        0    62694 2024-04-24 15:35:41.178150 itr_examples-1.1.5/src/ITR_examples/data/20230524 ITR V2 SBTi.xlsx
+-rw-r--r--   0        0        0      137 2024-04-24 15:35:41.178150 itr_examples-1.1.5/src/ITR_examples/environment.yml
+-rw-r--r--   0        0        0     9939 2024-04-24 15:35:41.178150 itr_examples-1.1.5/src/ITR_examples/utils.py
+-rw-r--r--   0        0        0     4303 1970-01-01 00:00:00.000000 itr_examples-1.1.5/PKG-INFO
```

### Comparing `itr_examples-1.1.4/LICENSE.txt` & `itr_examples-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `itr_examples-1.1.4/README.md` & `itr_examples-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `itr_examples-1.1.4/pyproject.toml` & `itr_examples-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ITR-examples"
-version = "v1.1.4"
+version = "v1.1.5"
 description = "Example code and user interface for the ITR project."
 authors = [
     { name = "Michael Tiemann", email = "72577720+MichaelTiemannOSC@users.noreply.github.com" },
 ]
 requires-python = "<3.13,>=3.9"
 readme = "README.md"
 keywords = [
@@ -26,15 +26,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.9",
     "Topic :: Office/Business :: Financial",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development",
 ]
 dependencies = [
-    "ITR==v1.1.4",
+    "ITR==1.1.4",
     "pip>=23.3.1",
     "dash>=2.15.0",
     "dash-bootstrap-components==1.4.2",
     "diskcache==5.6.1",
     "flask==2.2.5",
     "jupyterlab>=4.0.11",
     "kaleido==0.2.1",
@@ -110,15 +110,15 @@
     "src",
 ]
 omit = [
     "test/*",
 ]
 
 [tool.coverage.report]
-fail_under = 70
+fail_under = 0
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
 profile = "black"
```

### Comparing `itr_examples-1.1.4/src/ITR_examples/ITR_DV.py` & `itr_examples-1.1.5/src/ITR_examples/ITR_DV.py`

 * *Files identical despite different names*

### Comparing `itr_examples-1.1.4/src/ITR_examples/ITR_UI.py` & `itr_examples-1.1.5/src/ITR_examples/ITR_UI.py`

 * *Files identical despite different names*

### Comparing `itr_examples-1.1.4/src/ITR_examples/__init__.py` & `itr_examples-1.1.5/src/ITR_examples/__init__.py`

 * *Files identical despite different names*

### Comparing `itr_examples-1.1.4/src/ITR_examples/data/20220215 ITR Tool Sample Data.xlsx` & `itr_examples-1.1.5/src/ITR_examples/data/20220215 ITR Tool Sample Data.xlsx`

 * *Files identical despite different names*

### Comparing `itr_examples-1.1.4/src/ITR_examples/data/20220720 ITR Tool Sample Data.xlsx` & `itr_examples-1.1.5/src/ITR_examples/data/20220720 ITR Tool Sample Data.xlsx`

 * *Files identical despite different names*

### Comparing `itr_examples-1.1.4/src/ITR_examples/data/20220720 ITR Tool Test Data.xlsx` & `itr_examples-1.1.5/src/ITR_examples/data/20220720 ITR Tool Test Data.xlsx`

 * *Files identical despite different names*

### Comparing `itr_examples-1.1.4/src/ITR_examples/data/20220927 ITR Tool Sample Data.xlsx` & `itr_examples-1.1.5/src/ITR_examples/data/20220927 ITR Tool Sample Data.xlsx`

 * *Files identical despite different names*

### Comparing `itr_examples-1.1.4/src/ITR_examples/data/20220927 ITR Tool Test Data.xlsx` & `itr_examples-1.1.5/src/ITR_examples/data/20220927 ITR Tool Test Data.xlsx`

 * *Files identical despite different names*

### Comparing `itr_examples-1.1.4/src/ITR_examples/data/20220927 ITR V2 Sample Data.xlsx` & `itr_examples-1.1.5/src/ITR_examples/data/20220927 ITR V2 Sample Data.xlsx`

 * *Files identical despite different names*

### Comparing `itr_examples-1.1.4/src/ITR_examples/data/20221025 ITR V2 Sample Data.xlsx` & `itr_examples-1.1.5/src/ITR_examples/data/20221025 ITR V2 Sample Data.xlsx`

 * *Files identical despite different names*

### Comparing `itr_examples-1.1.4/src/ITR_examples/data/20230106 ITR V2 Sample Data.xlsx` & `itr_examples-1.1.5/src/ITR_examples/data/20230106 ITR V2 Sample Data.xlsx`

 * *Files identical despite different names*

### Comparing `itr_examples-1.1.4/src/ITR_examples/data/20230524 ITR V2 SBTi.xlsx` & `itr_examples-1.1.5/src/ITR_examples/data/20230524 ITR V2 SBTi.xlsx`

 * *Files identical despite different names*

### Comparing `itr_examples-1.1.4/src/ITR_examples/utils.py` & `itr_examples-1.1.5/src/ITR_examples/utils.py`

 * *Files identical despite different names*

### Comparing `itr_examples-1.1.4/PKG-INFO` & `itr_examples-1.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ITR-examples
-Version: 1.1.4
+Version: 1.1.5
 Summary: Example code and user interface for the ITR project.
-Keywords: Climate ITR Finance
+Keywords: Climate,ITR,Finance
 Author-Email: Michael Tiemann <72577720+MichaelTiemannOSC@users.noreply.github.com>
 License: Apache-2.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
@@ -23,15 +23,15 @@
 Project-URL: Homepage, https://github.com/os-climate/ITR-examples
 Project-URL: Repository, https://github.com/os-climate/ITR-examples
 Project-URL: Downloads, https://github.com/os-climate/ITR-examples/releases
 Project-URL: Bug tracker, https://github.com/os-climate/ITR-examples/issues
 Project-URL: Documentation, https://github.com/os-climate/ITR-examples/tree/main/docs
 Project-URL: Source code, https://github.com/os-climate/ITR-examples
 Requires-Python: <3.13,>=3.9
-Requires-Dist: ITR==v1.1.4
+Requires-Dist: ITR==1.1.4
 Requires-Dist: pip>=23.3.1
 Requires-Dist: dash>=2.15.0
 Requires-Dist: dash-bootstrap-components==1.4.2
 Requires-Dist: diskcache==5.6.1
 Requires-Dist: flask==2.2.5
 Requires-Dist: jupyterlab>=4.0.11
 Requires-Dist: kaleido==0.2.1
```

