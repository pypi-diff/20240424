# Comparing `tmp/pyEDAA.Reports-0.4.1.tar.gz` & `tmp/pyedaa_reports-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyEDAA.Reports-0.4.1.tar", last modified: Sun Mar 17 00:35:55 2024, max compression
+gzip compressed data, was "pyedaa_reports-0.5.0.tar", last modified: Wed Apr 24 21:46:30 2024, max compression
```

## Comparing `pyEDAA.Reports-0.4.1.tar` & `pyedaa_reports-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 00:35:55.276815 pyEDAA.Reports-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-03-17 00:35:42.000000 pyEDAA.Reports-0.4.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-03-17 00:35:55.276815 pyEDAA.Reports-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-03-17 00:35:42.000000 pyEDAA.Reports-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 00:35:55.264814 pyEDAA.Reports-0.4.1/pyEDAA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 00:35:55.268815 pyEDAA.Reports-0.4.1/pyEDAA/Reports/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 00:35:55.268815 pyEDAA.Reports-0.4.1/pyEDAA/Reports/DocumentationCoverage/
--rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-03-17 00:35:42.000000 pyEDAA.Reports-0.4.1/pyEDAA/Reports/DocumentationCoverage/Python.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-03-17 00:35:42.000000 pyEDAA.Reports-0.4.1/pyEDAA/Reports/DocumentationCoverage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 00:35:55.268815 pyEDAA.Reports-0.4.1/pyEDAA/Reports/Unittesting/
--rw-r--r--   0 runner    (1001) docker     (127)    13651 2024-03-17 00:35:42.000000 pyEDAA.Reports-0.4.1/pyEDAA/Reports/Unittesting/JUnit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-03-17 00:35:42.000000 pyEDAA.Reports-0.4.1/pyEDAA/Reports/Unittesting/OSVVM.py
--rw-r--r--   0 runner    (1001) docker     (127)    34727 2024-03-17 00:35:42.000000 pyEDAA.Reports-0.4.1/pyEDAA/Reports/Unittesting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-03-17 00:35:42.000000 pyEDAA.Reports-0.4.1/pyEDAA/Reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 00:35:42.000000 pyEDAA.Reports-0.4.1/pyEDAA/Reports/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 00:35:55.268815 pyEDAA.Reports-0.4.1/pyEDAA/Reports/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-03-17 00:35:42.000000 pyEDAA.Reports-0.4.1/pyEDAA/Reports/resources/Unittesting.xsd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 00:35:42.000000 pyEDAA.Reports-0.4.1/pyEDAA/Reports/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 00:35:55.268815 pyEDAA.Reports-0.4.1/pyEDAA.Reports.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-03-17 00:35:55.000000 pyEDAA.Reports-0.4.1/pyEDAA.Reports.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-17 00:35:55.000000 pyEDAA.Reports-0.4.1/pyEDAA.Reports.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 00:35:55.000000 pyEDAA.Reports-0.4.1/pyEDAA.Reports.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-17 00:35:55.000000 pyEDAA.Reports-0.4.1/pyEDAA.Reports.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-17 00:35:55.000000 pyEDAA.Reports-0.4.1/pyEDAA.Reports.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-17 00:35:42.000000 pyEDAA.Reports-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-17 00:35:55.276815 pyEDAA.Reports-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-03-17 00:35:42.000000 pyEDAA.Reports-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:30.908217 pyedaa_reports-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8957 2024-04-24 21:46:30.908217 pyedaa_reports-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:30.896217 pyedaa_reports-0.5.0/pyEDAA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:30.900217 pyedaa_reports-0.5.0/pyEDAA/Reports/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:30.900217 pyedaa_reports-0.5.0/pyEDAA/Reports/CLI/
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/CLI/Unittesting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/CLI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:30.900217 pyedaa_reports-0.5.0/pyEDAA/Reports/Dependency/
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/Dependency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:30.900217 pyedaa_reports-0.5.0/pyEDAA/Reports/DocumentationCoverage/
+-rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/DocumentationCoverage/Python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/DocumentationCoverage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:30.900217 pyedaa_reports-0.5.0/pyEDAA/Reports/Requirement/
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/Requirement/Python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/Requirement/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:30.900217 pyedaa_reports-0.5.0/pyEDAA/Reports/Unittesting/
+-rw-r--r--   0 runner    (1001) docker     (127)    13651 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/Unittesting/JUnit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/Unittesting/OSVVM.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34747 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/Unittesting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:30.900217 pyedaa_reports-0.5.0/pyEDAA/Reports/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/resources/Unittesting.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:30.900217 pyedaa_reports-0.5.0/pyEDAA.Reports.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8957 2024-04-24 21:46:30.000000 pyedaa_reports-0.5.0/pyEDAA.Reports.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-24 21:46:30.000000 pyedaa_reports-0.5.0/pyEDAA.Reports.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 21:46:30.000000 pyedaa_reports-0.5.0/pyEDAA.Reports.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-24 21:46:30.000000 pyedaa_reports-0.5.0/pyEDAA.Reports.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-24 21:46:30.000000 pyedaa_reports-0.5.0/pyEDAA.Reports.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 21:46:30.000000 pyedaa_reports-0.5.0/pyEDAA.Reports.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 21:46:30.908217 pyedaa_reports-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/setup.py
```

### Comparing `pyEDAA.Reports-0.4.1/LICENSE.md` & `pyedaa_reports-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyEDAA.Reports-0.4.1/PKG-INFO` & `pyedaa_reports-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEDAA.Reports
-Version: 0.4.1
+Version: 0.5.0
 Summary: Various report abstract data models and report format converters.
 Home-page: https://GitHub.com/pyEDAA/pyEDAA.Reports
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyEDAA.GitHub.io/pyEDAA.Reports
 Project-URL: Source Code, https://GitHub.com/pyEDAA/pyEDAA.Reports
@@ -18,65 +18,61 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: pyTooling~=6.0.0
-Requires-Dist: lxml>=4.9
-Requires-Dist: ruamel.yaml>=0.17
+Requires-Dist: lxml~=5.1
+Requires-Dist: pyTooling~=6.1
+Requires-Dist: ruamel.yaml~=0.18.6
 Provides-Extra: doc
-Requires-Dist: pyTooling~=6.0.0; extra == "doc"
-Requires-Dist: pyTooling~=6.0; extra == "doc"
-Requires-Dist: sphinx<8.0,>=7.2; extra == "doc"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "doc"
+Requires-Dist: sphinx_reports~=0.6; extra == "doc"
+Requires-Dist: autoapi>=2.0.1; extra == "doc"
+Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
+Requires-Dist: pyTooling~=6.1; extra == "doc"
+Requires-Dist: docutils~=0.18.1; extra == "doc"
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
-Requires-Dist: sphinx_reports>=0.5.0; extra == "doc"
+Requires-Dist: lxml~=5.1; extra == "doc"
+Requires-Dist: setuptools~=69.5; extra == "doc"
+Requires-Dist: sphinx~=7.3; extra == "doc"
+Requires-Dist: colorama>=0.4.6; extra == "doc"
 Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
-Requires-Dist: setuptools>=69.0.0; extra == "doc"
-Requires-Dist: sphinx_autodoc_typehints>=1.25.2; extra == "doc"
-Requires-Dist: lxml>=4.9; extra == "doc"
-Requires-Dist: docutils<0.19.0,>=0.18.0; extra == "doc"
 Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
-Requires-Dist: autoapi>=2.0.1; extra == "doc"
-Requires-Dist: ruamel.yaml>=0.17; extra == "doc"
-Requires-Dist: colorama>=0.4.6; extra == "doc"
-Requires-Dist: ruamel.yaml>=0.18.5; extra == "doc"
-Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
+Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
 Provides-Extra: test
-Requires-Dist: pyTooling~=6.0.0; extra == "test"
-Requires-Dist: pytest-cov>=4.1.0; extra == "test"
-Requires-Dist: mypy>=1.5; extra == "test"
-Requires-Dist: Coverage>=7.3; extra == "test"
-Requires-Dist: lxml>=4.9; extra == "test"
-Requires-Dist: typing_extensions>=4.7.1; extra == "test"
-Requires-Dist: pytest>=7.4.0; extra == "test"
-Requires-Dist: ruamel.yaml>=0.17; extra == "test"
+Requires-Dist: pytest-cov~=5.0; extra == "test"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
+Requires-Dist: mypy~=1.10; extra == "test"
+Requires-Dist: pytest~=8.1; extra == "test"
+Requires-Dist: Coverage~=7.5; extra == "test"
+Requires-Dist: pyTooling~=6.1; extra == "test"
+Requires-Dist: lxml~=5.1; extra == "test"
+Requires-Dist: typing_extensions~=4.11; extra == "test"
 Provides-Extra: all
-Requires-Dist: sphinx_reports>=0.5.0; extra == "all"
-Requires-Dist: mypy>=1.5; extra == "all"
-Requires-Dist: lxml>=4.9; extra == "all"
+Requires-Dist: autoapi>=2.0.1; extra == "all"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
+Requires-Dist: lxml~=5.1; extra == "all"
+Requires-Dist: typing_extensions~=4.11; extra == "all"
 Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
+Requires-Dist: pyTooling~=6.1; extra == "all"
+Requires-Dist: setuptools~=69.5; extra == "all"
 Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
-Requires-Dist: colorama>=0.4.6; extra == "all"
-Requires-Dist: ruamel.yaml>=0.18.5; extra == "all"
-Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
+Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "all"
+Requires-Dist: pytest-cov~=5.0; extra == "all"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "all"
+Requires-Dist: pytest~=8.1; extra == "all"
 Requires-Dist: sphinx_design>=0.5.0; extra == "all"
-Requires-Dist: sphinx_autodoc_typehints>=1.25.2; extra == "all"
-Requires-Dist: pyTooling~=6.0; extra == "all"
-Requires-Dist: typing_extensions>=4.7.1; extra == "all"
-Requires-Dist: ruamel.yaml>=0.17; extra == "all"
-Requires-Dist: autoapi>=2.0.1; extra == "all"
-Requires-Dist: pyTooling~=6.0.0; extra == "all"
-Requires-Dist: pytest-cov>=4.1.0; extra == "all"
-Requires-Dist: sphinx<8.0,>=7.2; extra == "all"
-Requires-Dist: Coverage>=7.3; extra == "all"
-Requires-Dist: setuptools>=69.0.0; extra == "all"
-Requires-Dist: docutils<0.19.0,>=0.18.0; extra == "all"
-Requires-Dist: pytest>=7.4.0; extra == "all"
+Requires-Dist: sphinx~=7.3; extra == "all"
+Requires-Dist: sphinx_reports~=0.6; extra == "all"
+Requires-Dist: mypy~=1.10; extra == "all"
+Requires-Dist: docutils~=0.18.1; extra == "all"
+Requires-Dist: Coverage~=7.5; extra == "all"
+Requires-Dist: colorama>=0.4.6; extra == "all"
 
 <p align="center">
   <a title="edaa-org.github.io/pyEDAA.Reports" href="https://edaa-org.github.io/pyEDAA.Reports"><img height="80px" src="doc/_static/logo.svg"/></a>
 </p>
 
 [![Sourcecode on GitHub](https://img.shields.io/badge/pyEDAA-Reports-29b6f6.svg?longCache=true&style=flat-square&logo=GitHub&labelColor=0277bd)](https://GitHub.com/edaa-org/pyEDAA.Reports)
 [![Documentation](https://img.shields.io/website?longCache=true&style=flat-square&label=edaa-org.github.io%2FpyEDAA.Reports&logo=GitHub&logoColor=fff&up_color=blueviolet&up_message=Read%20now%20%E2%9E%9A&url=https%3A%2F%2Fedaa-org.github.io%2FpyEDAA.Reports%2Findex.html)](https://edaa-org.github.io/pyEDAA.Reports/)
```

### Comparing `pyEDAA.Reports-0.4.1/README.md` & `pyedaa_reports-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyEDAA.Reports-0.4.1/pyEDAA/Reports/DocumentationCoverage/Python.py` & `pyedaa_reports-0.5.0/pyEDAA/Reports/DocumentationCoverage/Python.py`

 * *Files identical despite different names*

### Comparing `pyEDAA.Reports-0.4.1/pyEDAA/Reports/DocumentationCoverage/__init__.py` & `pyedaa_reports-0.5.0/pyEDAA/Reports/DocumentationCoverage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyEDAA.Reports-0.4.1/pyEDAA/Reports/Unittesting/JUnit.py` & `pyedaa_reports-0.5.0/pyEDAA/Reports/Unittesting/JUnit.py`

 * *Files identical despite different names*

### Comparing `pyEDAA.Reports-0.4.1/pyEDAA/Reports/Unittesting/OSVVM.py` & `pyedaa_reports-0.5.0/pyEDAA/Reports/Unittesting/OSVVM.py`

 * *Files identical despite different names*

### Comparing `pyEDAA.Reports-0.4.1/pyEDAA/Reports/Unittesting/__init__.py` & `pyedaa_reports-0.5.0/pyEDAA/Reports/Unittesting/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,14 +395,15 @@
 
 
 @export
 class TestsuiteBase(Base, Generic[TestsuiteType]):
 	_status:     TestsuiteStatus
 	_testsuites: Dict[str, TestsuiteType]
 
+	_tests:        int
 	_inconsistent: int
 	_excluded:     int
 	_skipped:      int
 	_errored:      int
 	_weak:         int
 	_failed:       int
 	_passed:       int
```

### Comparing `pyEDAA.Reports-0.4.1/pyEDAA/Reports/__init__.py` & `pyedaa_reports-0.5.0/pyEDAA/Reports/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 """
 Various report abstract data models and report format converters.
 """
 __author__ =    "Patrick Lehmann"
 __email__ =     "Paebbels@gmail.com"
 __copyright__ = "2021-2024, Electronic Design Automation Abstraction (EDA²)"
 __license__ =   "Apache License, Version 2.0"
-__version__ =   "0.4.1"
+__version__ =   "0.5.0"
 __keywords__ =  ["Reports", "Abstract Model", "Data Model", "Test Case", "Test Suite", "OSVVM", "YAML", "XML"]
 
 from enum                 import Enum
 from importlib.resources  import files
 from pathlib              import Path
 from sys                  import version_info
 from types                import ModuleType
```

### Comparing `pyEDAA.Reports-0.4.1/pyEDAA/Reports/resources/Unittesting.xsd` & `pyedaa_reports-0.5.0/pyEDAA/Reports/resources/Unittesting.xsd`

 * *Files identical despite different names*

### Comparing `pyEDAA.Reports-0.4.1/pyEDAA.Reports.egg-info/PKG-INFO` & `pyedaa_reports-0.5.0/pyEDAA.Reports.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEDAA.Reports
-Version: 0.4.1
+Version: 0.5.0
 Summary: Various report abstract data models and report format converters.
 Home-page: https://GitHub.com/pyEDAA/pyEDAA.Reports
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyEDAA.GitHub.io/pyEDAA.Reports
 Project-URL: Source Code, https://GitHub.com/pyEDAA/pyEDAA.Reports
@@ -18,65 +18,61 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: pyTooling~=6.0.0
-Requires-Dist: lxml>=4.9
-Requires-Dist: ruamel.yaml>=0.17
+Requires-Dist: lxml~=5.1
+Requires-Dist: pyTooling~=6.1
+Requires-Dist: ruamel.yaml~=0.18.6
 Provides-Extra: doc
-Requires-Dist: pyTooling~=6.0.0; extra == "doc"
-Requires-Dist: pyTooling~=6.0; extra == "doc"
-Requires-Dist: sphinx<8.0,>=7.2; extra == "doc"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "doc"
+Requires-Dist: sphinx_reports~=0.6; extra == "doc"
+Requires-Dist: autoapi>=2.0.1; extra == "doc"
+Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
+Requires-Dist: pyTooling~=6.1; extra == "doc"
+Requires-Dist: docutils~=0.18.1; extra == "doc"
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
-Requires-Dist: sphinx_reports>=0.5.0; extra == "doc"
+Requires-Dist: lxml~=5.1; extra == "doc"
+Requires-Dist: setuptools~=69.5; extra == "doc"
+Requires-Dist: sphinx~=7.3; extra == "doc"
+Requires-Dist: colorama>=0.4.6; extra == "doc"
 Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
-Requires-Dist: setuptools>=69.0.0; extra == "doc"
-Requires-Dist: sphinx_autodoc_typehints>=1.25.2; extra == "doc"
-Requires-Dist: lxml>=4.9; extra == "doc"
-Requires-Dist: docutils<0.19.0,>=0.18.0; extra == "doc"
 Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
-Requires-Dist: autoapi>=2.0.1; extra == "doc"
-Requires-Dist: ruamel.yaml>=0.17; extra == "doc"
-Requires-Dist: colorama>=0.4.6; extra == "doc"
-Requires-Dist: ruamel.yaml>=0.18.5; extra == "doc"
-Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
+Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
 Provides-Extra: test
-Requires-Dist: pyTooling~=6.0.0; extra == "test"
-Requires-Dist: pytest-cov>=4.1.0; extra == "test"
-Requires-Dist: mypy>=1.5; extra == "test"
-Requires-Dist: Coverage>=7.3; extra == "test"
-Requires-Dist: lxml>=4.9; extra == "test"
-Requires-Dist: typing_extensions>=4.7.1; extra == "test"
-Requires-Dist: pytest>=7.4.0; extra == "test"
-Requires-Dist: ruamel.yaml>=0.17; extra == "test"
+Requires-Dist: pytest-cov~=5.0; extra == "test"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
+Requires-Dist: mypy~=1.10; extra == "test"
+Requires-Dist: pytest~=8.1; extra == "test"
+Requires-Dist: Coverage~=7.5; extra == "test"
+Requires-Dist: pyTooling~=6.1; extra == "test"
+Requires-Dist: lxml~=5.1; extra == "test"
+Requires-Dist: typing_extensions~=4.11; extra == "test"
 Provides-Extra: all
-Requires-Dist: sphinx_reports>=0.5.0; extra == "all"
-Requires-Dist: mypy>=1.5; extra == "all"
-Requires-Dist: lxml>=4.9; extra == "all"
+Requires-Dist: autoapi>=2.0.1; extra == "all"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
+Requires-Dist: lxml~=5.1; extra == "all"
+Requires-Dist: typing_extensions~=4.11; extra == "all"
 Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
+Requires-Dist: pyTooling~=6.1; extra == "all"
+Requires-Dist: setuptools~=69.5; extra == "all"
 Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
-Requires-Dist: colorama>=0.4.6; extra == "all"
-Requires-Dist: ruamel.yaml>=0.18.5; extra == "all"
-Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
+Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "all"
+Requires-Dist: pytest-cov~=5.0; extra == "all"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "all"
+Requires-Dist: pytest~=8.1; extra == "all"
 Requires-Dist: sphinx_design>=0.5.0; extra == "all"
-Requires-Dist: sphinx_autodoc_typehints>=1.25.2; extra == "all"
-Requires-Dist: pyTooling~=6.0; extra == "all"
-Requires-Dist: typing_extensions>=4.7.1; extra == "all"
-Requires-Dist: ruamel.yaml>=0.17; extra == "all"
-Requires-Dist: autoapi>=2.0.1; extra == "all"
-Requires-Dist: pyTooling~=6.0.0; extra == "all"
-Requires-Dist: pytest-cov>=4.1.0; extra == "all"
-Requires-Dist: sphinx<8.0,>=7.2; extra == "all"
-Requires-Dist: Coverage>=7.3; extra == "all"
-Requires-Dist: setuptools>=69.0.0; extra == "all"
-Requires-Dist: docutils<0.19.0,>=0.18.0; extra == "all"
-Requires-Dist: pytest>=7.4.0; extra == "all"
+Requires-Dist: sphinx~=7.3; extra == "all"
+Requires-Dist: sphinx_reports~=0.6; extra == "all"
+Requires-Dist: mypy~=1.10; extra == "all"
+Requires-Dist: docutils~=0.18.1; extra == "all"
+Requires-Dist: Coverage~=7.5; extra == "all"
+Requires-Dist: colorama>=0.4.6; extra == "all"
 
 <p align="center">
   <a title="edaa-org.github.io/pyEDAA.Reports" href="https://edaa-org.github.io/pyEDAA.Reports"><img height="80px" src="doc/_static/logo.svg"/></a>
 </p>
 
 [![Sourcecode on GitHub](https://img.shields.io/badge/pyEDAA-Reports-29b6f6.svg?longCache=true&style=flat-square&logo=GitHub&labelColor=0277bd)](https://GitHub.com/edaa-org/pyEDAA.Reports)
 [![Documentation](https://img.shields.io/website?longCache=true&style=flat-square&label=edaa-org.github.io%2FpyEDAA.Reports&logo=GitHub&logoColor=fff&up_color=blueviolet&up_message=Read%20now%20%E2%9E%9A&url=https%3A%2F%2Fedaa-org.github.io%2FpyEDAA.Reports%2Findex.html)](https://edaa-org.github.io/pyEDAA.Reports/)
```

### Comparing `pyEDAA.Reports-0.4.1/pyEDAA.Reports.egg-info/SOURCES.txt` & `pyedaa_reports-0.5.0/pyEDAA.Reports.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 LICENSE.md
 README.md
 pyproject.toml
 setup.py
 pyEDAA.Reports.egg-info/PKG-INFO
 pyEDAA.Reports.egg-info/SOURCES.txt
 pyEDAA.Reports.egg-info/dependency_links.txt
+pyEDAA.Reports.egg-info/entry_points.txt
 pyEDAA.Reports.egg-info/requires.txt
 pyEDAA.Reports.egg-info/top_level.txt
 pyEDAA/Reports/__init__.py
 pyEDAA/Reports/py.typed
+pyEDAA/Reports/CLI/Unittesting.py
+pyEDAA/Reports/CLI/__init__.py
+pyEDAA/Reports/Dependency/__init__.py
 pyEDAA/Reports/DocumentationCoverage/Python.py
 pyEDAA/Reports/DocumentationCoverage/__init__.py
+pyEDAA/Reports/Requirement/Python.py
+pyEDAA/Reports/Requirement/__init__.py
 pyEDAA/Reports/Unittesting/JUnit.py
 pyEDAA/Reports/Unittesting/OSVVM.py
 pyEDAA/Reports/Unittesting/__init__.py
 pyEDAA/Reports/resources/Unittesting.xsd
 pyEDAA/Reports/resources/__init__.py
```

### Comparing `pyEDAA.Reports-0.4.1/pyproject.toml` & `pyedaa_reports-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = [
-  "setuptools >= 69.0.0",
-  "wheel >= 0.40.0",
-  "pyTooling ~= 6.0"
+  "setuptools ~= 69.5",
+  "wheel ~= 0.40.0",
+  "pyTooling ~= 6.1"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
 
 [tool.mypy]
```

### Comparing `pyEDAA.Reports-0.4.1/setup.py` & `pyedaa_reports-0.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,9 +50,12 @@
 	],
 	sourceFileWithVersion=packageInformationFile,
 	dataFiles={
 		packageName: [
 			f"py.typed",
 			f"resources/*.xsd"
 		]
+	},
+	consoleScripts={
+		"pyedaa-reports": "pyEDAA.Reports.CLI:main"
 	}
 ))
```

