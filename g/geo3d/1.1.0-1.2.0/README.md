# Comparing `tmp/geo3d-1.1.0.tar.gz` & `tmp/geo3d-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo3d-1.1.0.tar", last modified: Sun Apr  3 10:46:28 2022, max compression
+gzip compressed data, was "geo3d-1.2.0.tar", last modified: Wed Apr 24 13:29:00 2024, max compression
```

## Comparing `geo3d-1.1.0.tar` & `geo3d-1.2.0.tar`

### file list

```diff
@@ -1,60 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 10:46:28.254901 geo3d-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-04-03 10:46:14.000000 geo3d-1.1.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 10:46:28.250901 geo3d-1.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-04-03 10:46:14.000000 geo3d-1.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 10:46:28.250901 geo3d-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2079 2022-04-03 10:46:14.000000 geo3d-1.1.0/.github/workflows/build_docs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2361 2022-04-03 10:46:14.000000 geo3d-1.1.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-04-03 10:46:14.000000 geo3d-1.1.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-04-03 10:46:14.000000 geo3d-1.1.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-04-03 10:46:14.000000 geo3d-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     3342 2022-04-03 10:46:14.000000 geo3d-1.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-04-03 10:46:14.000000 geo3d-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-04-03 10:46:28.254901 geo3d-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-04-03 10:46:14.000000 geo3d-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-04-03 10:46:14.000000 geo3d-1.1.0/_pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 10:46:28.250901 geo3d-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-04-03 10:46:14.000000 geo3d-1.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)    14988 2022-04-03 10:46:14.000000 geo3d-1.1.0/docs/basic_usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     1908 2022-04-03 10:46:14.000000 geo3d-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2220 2022-04-03 10:46:14.000000 geo3d-1.1.0/docs/fit.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-04-03 10:46:14.000000 geo3d-1.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-04-03 10:46:14.000000 geo3d-1.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)     4435 2022-04-03 10:46:14.000000 geo3d-1.1.0/docs/queries.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 10:46:28.250901 geo3d-1.1.0/geo3d/
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-04-03 10:46:14.000000 geo3d-1.1.0/geo3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-04-03 10:46:14.000000 geo3d-1.1.0/geo3d/auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (121)     1711 2022-04-03 10:46:14.000000 geo3d-1.1.0/geo3d/fit.py
--rw-r--r--   0 runner    (1001) docker     (121)    16367 2022-04-03 10:46:14.000000 geo3d-1.1.0/geo3d/frame.py
--rw-r--r--   0 runner    (1001) docker     (121)     1268 2022-04-03 10:46:14.000000 geo3d-1.1.0/geo3d/linalg.py
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-04-03 10:46:14.000000 geo3d-1.1.0/geo3d/plane.py
--rw-r--r--   0 runner    (1001) docker     (121)     7170 2022-04-03 10:46:14.000000 geo3d-1.1.0/geo3d/point.py
--rw-r--r--   0 runner    (1001) docker     (121)     7132 2022-04-03 10:46:14.000000 geo3d-1.1.0/geo3d/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (121)     3228 2022-04-03 10:46:14.000000 geo3d-1.1.0/geo3d/query.py
--rw-r--r--   0 runner    (1001) docker     (121)     3090 2022-04-03 10:46:14.000000 geo3d-1.1.0/geo3d/rotation.py
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-04-03 10:46:14.000000 geo3d-1.1.0/geo3d/types.py
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-04-03 10:46:14.000000 geo3d-1.1.0/geo3d/units.py
--rw-r--r--   0 runner    (1001) docker     (121)     7731 2022-04-03 10:46:14.000000 geo3d-1.1.0/geo3d/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 10:46:28.250901 geo3d-1.1.0/geo3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-04-03 10:46:28.000000 geo3d-1.1.0/geo3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      975 2022-04-03 10:46:28.000000 geo3d-1.1.0/geo3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-03 10:46:28.000000 geo3d-1.1.0/geo3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-04-03 10:46:28.000000 geo3d-1.1.0/geo3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-04-03 10:46:28.000000 geo3d-1.1.0/geo3d.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 10:46:28.254901 geo3d-1.1.0/profiling/
--rw-r--r--   0 runner    (1001) docker     (121)    25441 2022-04-03 10:46:14.000000 geo3d-1.1.0/profiling/speed_tests.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-04-03 10:46:14.000000 geo3d-1.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-04-03 10:46:14.000000 geo3d-1.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-04-03 10:46:14.000000 geo3d-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-03 10:46:28.254901 geo3d-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2195 2022-04-03 10:46:14.000000 geo3d-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 10:46:28.254901 geo3d-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-04-03 10:46:14.000000 geo3d-1.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-04-03 10:46:14.000000 geo3d-1.1.0/tests/test_fit.py
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-04-03 10:46:14.000000 geo3d-1.1.0/tests/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-04-03 10:46:14.000000 geo3d-1.1.0/tests/test_plane.py
--rw-r--r--   0 runner    (1001) docker     (121)     1813 2022-04-03 10:46:14.000000 geo3d-1.1.0/tests/test_point.py
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-04-03 10:46:14.000000 geo3d-1.1.0/tests/test_quat_algs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-04-03 10:46:14.000000 geo3d-1.1.0/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-04-03 10:46:14.000000 geo3d-1.1.0/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-04-03 10:46:14.000000 geo3d-1.1.0/tests/test_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:00.852776 geo3d-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 13:28:45.000000 geo3d-1.2.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:00.844776 geo3d-1.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-24 13:28:45.000000 geo3d-1.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:00.844776 geo3d-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-24 13:28:45.000000 geo3d-1.2.0/.github/workflows/build_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-24 13:28:45.000000 geo3d-1.2.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-24 13:28:45.000000 geo3d-1.2.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-24 13:28:45.000000 geo3d-1.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-24 13:28:45.000000 geo3d-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-24 13:28:45.000000 geo3d-1.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-24 13:28:45.000000 geo3d-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-24 13:29:00.852776 geo3d-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-24 13:28:45.000000 geo3d-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:00.848776 geo3d-1.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-24 13:28:45.000000 geo3d-1.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    14988 2024-04-24 13:28:45.000000 geo3d-1.2.0/docs/basic_usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-24 13:28:45.000000 geo3d-1.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-24 13:28:45.000000 geo3d-1.2.0/docs/fit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-24 13:28:45.000000 geo3d-1.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-24 13:28:45.000000 geo3d-1.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-24 13:28:45.000000 geo3d-1.2.0/docs/queries.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:00.848776 geo3d-1.2.0/geo3d/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16367 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7132 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-04-24 13:28:45.000000 geo3d-1.2.0/geo3d/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:00.852776 geo3d-1.2.0/geo3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-24 13:29:00.000000 geo3d-1.2.0/geo3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-24 13:29:00.000000 geo3d-1.2.0/geo3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:29:00.000000 geo3d-1.2.0/geo3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-24 13:29:00.000000 geo3d-1.2.0/geo3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 13:29:00.000000 geo3d-1.2.0/geo3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:00.852776 geo3d-1.2.0/profiling/
+-rw-r--r--   0 runner    (1001) docker     (127)    25441 2024-04-24 13:28:45.000000 geo3d-1.2.0/profiling/speed_tests.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-24 13:28:45.000000 geo3d-1.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-24 13:28:45.000000 geo3d-1.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-24 13:28:45.000000 geo3d-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:29:00.852776 geo3d-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-24 13:28:45.000000 geo3d-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:00.852776 geo3d-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-24 13:28:45.000000 geo3d-1.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-24 13:28:45.000000 geo3d-1.2.0/tests/test_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-24 13:28:45.000000 geo3d-1.2.0/tests/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-24 13:28:45.000000 geo3d-1.2.0/tests/test_plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-24 13:28:45.000000 geo3d-1.2.0/tests/test_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-24 13:28:45.000000 geo3d-1.2.0/tests/test_quat_algs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-24 13:28:45.000000 geo3d-1.2.0/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-24 13:28:45.000000 geo3d-1.2.0/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-24 13:28:45.000000 geo3d-1.2.0/tests/test_vector.py
```

### Comparing `geo3d-1.1.0/.github/workflows/build_docs.yml` & `geo3d-1.2.0/.github/workflows/build_docs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     steps:
       # Checks-out your repository under $GITHUB_WORKSPACE, so your job can access it
       - uses: actions/checkout@v2
       
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
-          python-version: "3.8"
+          python-version: "3.11"
         
       # Runs a single command using the runners shell
       - name: Build the Sphinx Docs
         run: |
           python -m pip install -U pip
           python -m pip install -r requirements-dev.txt
           sudo apt-get install pandoc
```

### Comparing `geo3d-1.1.0/.github/workflows/codeql-analysis.yml` & `geo3d-1.2.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/.github/workflows/pypi-publish.yml` & `geo3d-1.2.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/CODE_OF_CONDUCT.md` & `geo3d-1.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/LICENSE.txt` & `geo3d-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/README.md` & `geo3d-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Release on PyPI](https://github.com/himbeles/geo3d/workflows/Publish%20on%20PyPI/badge.svg)](https://pypi.org/project/geo3d/)
+[![pypi](https://img.shields.io/pypi/v/geo3d.svg)](https://pypi.python.org/pypi/geo3d)
 [![Test package](https://github.com/himbeles/geo3d/workflows/Test%20package/badge.svg)](https://github.com/himbeles/geo3d/actions?query=workflow%3A%22Test+package%22)
 
 # geo3d
 
 A python package for performing geometric calculations in 3D.
 It allows to 
   - find coordinate system transformations between frames
```

### Comparing `geo3d-1.1.0/docs/Makefile` & `geo3d-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/docs/basic_usage.ipynb` & `geo3d-1.2.0/docs/basic_usage.ipynb`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/docs/conf.py` & `geo3d-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/docs/fit.ipynb` & `geo3d-1.2.0/docs/fit.ipynb`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/docs/make.bat` & `geo3d-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/docs/queries.ipynb` & `geo3d-1.2.0/docs/queries.ipynb`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/geo3d/auxiliary.py` & `geo3d-1.2.0/geo3d/auxiliary.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/geo3d/fit.py` & `geo3d-1.2.0/geo3d/fit.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/geo3d/frame.py` & `geo3d-1.2.0/geo3d/frame.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/geo3d/linalg.py` & `geo3d-1.2.0/geo3d/linalg.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/geo3d/plane.py` & `geo3d-1.2.0/geo3d/plane.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/geo3d/point.py` & `geo3d-1.2.0/geo3d/point.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/geo3d/quaternion.py` & `geo3d-1.2.0/geo3d/quaternion.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/geo3d/query.py` & `geo3d-1.2.0/geo3d/query.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/geo3d/rotation.py` & `geo3d-1.2.0/geo3d/rotation.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/geo3d/vector.py` & `geo3d-1.2.0/geo3d/vector.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/geo3d.egg-info/SOURCES.txt` & `geo3d-1.2.0/geo3d.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 .coveragerc
 .gitignore
 CODE_OF_CONDUCT.md
 LICENSE.txt
 README.md
-_pyproject.toml
 pytest.ini
 requirements-dev.txt
 requirements.txt
 setup.py
 .github/dependabot.yml
 .github/workflows/build_docs.yml
 .github/workflows/codeql-analysis.yml
```

### Comparing `geo3d-1.1.0/profiling/speed_tests.ipynb` & `geo3d-1.2.0/profiling/speed_tests.ipynb`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/setup.py` & `geo3d-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/tests/test_frame.py` & `geo3d-1.2.0/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/tests/test_point.py` & `geo3d-1.2.0/tests/test_point.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/tests/test_quat_algs.py` & `geo3d-1.2.0/tests/test_quat_algs.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/tests/test_queries.py` & `geo3d-1.2.0/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/tests/test_transform.py` & `geo3d-1.2.0/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `geo3d-1.1.0/tests/test_vector.py` & `geo3d-1.2.0/tests/test_vector.py`

 * *Files identical despite different names*

