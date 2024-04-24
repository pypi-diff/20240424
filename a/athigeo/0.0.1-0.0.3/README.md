# Comparing `tmp/athigeo-0.0.1.tar.gz` & `tmp/athigeo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athigeo-0.0.1.tar", last modified: Wed Feb 21 18:40:07 2024, max compression
+gzip compressed data, was "athigeo-0.0.3.tar", last modified: Wed Apr 24 19:59:50 2024, max compression
```

## Comparing `athigeo-0.0.1.tar` & `athigeo-0.0.3.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:40:07.717724 athigeo-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-21 18:39:49.000000 athigeo-0.0.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:40:07.709724 athigeo-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:40:07.713724 athigeo-0.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-02-21 18:39:49.000000 athigeo-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-02-21 18:39:49.000000 athigeo-0.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-21 18:39:49.000000 athigeo-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:40:07.713724 athigeo-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-02-21 18:39:49.000000 athigeo-0.0.1/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-02-21 18:39:49.000000 athigeo-0.0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-02-21 18:39:49.000000 athigeo-0.0.1/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-02-21 18:39:49.000000 athigeo-0.0.1/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-02-21 18:39:49.000000 athigeo-0.0.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-02-21 18:39:49.000000 athigeo-0.0.1/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-02-21 18:39:49.000000 athigeo-0.0.1/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-02-21 18:39:49.000000 athigeo-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 18:39:49.000000 athigeo-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-21 18:39:49.000000 athigeo-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-02-21 18:40:07.717724 athigeo-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-02-21 18:39:49.000000 athigeo-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:40:07.713724 athigeo-0.0.1/athigeo/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-21 18:39:49.000000 athigeo-0.0.1/athigeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-21 18:39:49.000000 athigeo-0.0.1/athigeo/athigeo.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-21 18:39:49.000000 athigeo-0.0.1/athigeo/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:40:07.717724 athigeo-0.0.1/athigeo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-02-21 18:40:07.000000 athigeo-0.0.1/athigeo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-02-21 18:40:07.000000 athigeo-0.0.1/athigeo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 18:40:07.000000 athigeo-0.0.1/athigeo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-21 18:40:07.000000 athigeo-0.0.1/athigeo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-21 18:40:07.000000 athigeo-0.0.1/athigeo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-21 18:40:07.000000 athigeo-0.0.1/athigeo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:40:07.717724 athigeo-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-21 18:39:49.000000 athigeo-0.0.1/docs/athigeo.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-21 18:39:49.000000 athigeo-0.0.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-21 18:39:49.000000 athigeo-0.0.1/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-02-21 18:39:49.000000 athigeo-0.0.1/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:40:07.717724 athigeo-0.0.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-21 18:39:49.000000 athigeo-0.0.1/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-21 18:39:49.000000 athigeo-0.0.1/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-21 18:39:49.000000 athigeo-0.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-02-21 18:39:49.000000 athigeo-0.0.1/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:40:07.717724 athigeo-0.0.1/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-21 18:39:49.000000 athigeo-0.0.1/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-21 18:39:49.000000 athigeo-0.0.1/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-02-21 18:39:49.000000 athigeo-0.0.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-02-21 18:39:49.000000 athigeo-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-21 18:39:49.000000 athigeo-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-21 18:39:49.000000 athigeo-0.0.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 18:40:07.717724 athigeo-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 18:40:07.717724 athigeo-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-21 18:39:49.000000 athigeo-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-21 18:39:49.000000 athigeo-0.0.1/tests/test_athigeo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:59:50.217353 athigeo-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-24 19:59:38.000000 athigeo-0.0.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:59:50.205354 athigeo-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:59:50.209354 athigeo-0.0.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-24 19:59:38.000000 athigeo-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-24 19:59:38.000000 athigeo-0.0.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-24 19:59:38.000000 athigeo-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:59:50.209354 athigeo-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-24 19:59:38.000000 athigeo-0.0.3/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-24 19:59:38.000000 athigeo-0.0.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-24 19:59:38.000000 athigeo-0.0.3/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-24 19:59:38.000000 athigeo-0.0.3/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-24 19:59:38.000000 athigeo-0.0.3/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-24 19:59:38.000000 athigeo-0.0.3/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-24 19:59:38.000000 athigeo-0.0.3/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-24 19:59:38.000000 athigeo-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:59:38.000000 athigeo-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-24 19:59:38.000000 athigeo-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-24 19:59:50.213353 athigeo-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-24 19:59:38.000000 athigeo-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:59:50.209354 athigeo-0.0.3/athigeo/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-24 19:59:38.000000 athigeo-0.0.3/athigeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-24 19:59:38.000000 athigeo-0.0.3/athigeo/athigeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-24 19:59:38.000000 athigeo-0.0.3/athigeo/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:59:50.213353 athigeo-0.0.3/athigeo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-24 19:59:50.000000 athigeo-0.0.3/athigeo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-24 19:59:50.000000 athigeo-0.0.3/athigeo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:59:50.000000 athigeo-0.0.3/athigeo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-24 19:59:50.000000 athigeo-0.0.3/athigeo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 19:59:50.000000 athigeo-0.0.3/athigeo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 19:59:50.000000 athigeo-0.0.3/athigeo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:59:50.213353 athigeo-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 19:59:38.000000 athigeo-0.0.3/docs/CNAME
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-24 19:59:38.000000 athigeo-0.0.3/docs/athigeo.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 19:59:38.000000 athigeo-0.0.3/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-24 19:59:38.000000 athigeo-0.0.3/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-24 19:59:38.000000 athigeo-0.0.3/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:59:50.213353 athigeo-0.0.3/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-24 19:59:38.000000 athigeo-0.0.3/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 19:59:38.000000 athigeo-0.0.3/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-24 19:59:38.000000 athigeo-0.0.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-24 19:59:38.000000 athigeo-0.0.3/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:59:50.213353 athigeo-0.0.3/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-24 19:59:38.000000 athigeo-0.0.3/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-24 19:59:38.000000 athigeo-0.0.3/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-24 19:59:38.000000 athigeo-0.0.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-24 19:59:38.000000 athigeo-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 19:59:38.000000 athigeo-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-24 19:59:38.000000 athigeo-0.0.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:59:50.217353 athigeo-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:59:50.213353 athigeo-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-24 19:59:38.000000 athigeo-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-24 19:59:38.000000 athigeo-0.0.3/tests/test_athigeo.py
```

### Comparing `athigeo-0.0.1/.github/workflows/docs-build.yml` & `athigeo-0.0.3/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.1/.github/workflows/docs.yml` & `athigeo-0.0.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.1/.github/workflows/installation.yml` & `athigeo-0.0.3/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.1/.github/workflows/macos.yml` & `athigeo-0.0.3/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.1/.github/workflows/pypi.yml` & `athigeo-0.0.3/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.1/.github/workflows/ubuntu.yml` & `athigeo-0.0.3/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.1/.github/workflows/windows.yml` & `athigeo-0.0.3/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.1/.gitignore` & `athigeo-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.1/PKG-INFO` & `athigeo-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athigeo
-Version: 0.0.1
+Version: 0.0.3
 Summary: A python package intro
 Author-email: Dennis Mutai <dennis.mutaigeo@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/Dmutai/athigeo
 Keywords: athigeo
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -30,13 +30,16 @@
 [![image](https://img.shields.io/conda/vn/conda-forge/athigeo.svg)](https://anaconda.org/conda-forge/athigeo)
 
 
 **A python package intro**
 
 
 -   Free software: MIT License
--   Documentation: https://Dmutai.github.io/athigeo
+-   Documentation: https://athigeo.xyz/
     
 
 ## Features
 
--   TODO
+-   visualize raster and vector data
+
+- Analyzing raster and vector data
+- Print out useful Message
```

### Comparing `athigeo-0.0.1/athigeo.egg-info/PKG-INFO` & `athigeo-0.0.3/athigeo.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athigeo
-Version: 0.0.1
+Version: 0.0.3
 Summary: A python package intro
 Author-email: Dennis Mutai <dennis.mutaigeo@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/Dmutai/athigeo
 Keywords: athigeo
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -30,13 +30,16 @@
 [![image](https://img.shields.io/conda/vn/conda-forge/athigeo.svg)](https://anaconda.org/conda-forge/athigeo)
 
 
 **A python package intro**
 
 
 -   Free software: MIT License
--   Documentation: https://Dmutai.github.io/athigeo
+-   Documentation: https://athigeo.xyz/
     
 
 ## Features
 
--   TODO
+-   visualize raster and vector data
+
+- Analyzing raster and vector data
+- Print out useful Message
```

### Comparing `athigeo-0.0.1/athigeo.egg-info/SOURCES.txt` & `athigeo-0.0.3/athigeo.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 athigeo/common.py
 athigeo.egg-info/PKG-INFO
 athigeo.egg-info/SOURCES.txt
 athigeo.egg-info/dependency_links.txt
 athigeo.egg-info/entry_points.txt
 athigeo.egg-info/requires.txt
 athigeo.egg-info/top_level.txt
+docs/CNAME
 docs/athigeo.md
 docs/changelog.md
 docs/common.md
 docs/contributing.md
 docs/faq.md
 docs/index.md
 docs/installation.md
```

### Comparing `athigeo-0.0.1/docs/contributing.md` & `athigeo-0.0.3/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.1/docs/installation.md` & `athigeo-0.0.3/docs/installation.md`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.1/mkdocs.yml` & `athigeo-0.0.3/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 site_name: athigeo
 site_description: A python package intro
 site_author: Dmutai
-site_url: https://Dmutai.github.io/athigeo
+site_url: https://athigeo.xyz
 repo_url: https://github.com/Dmutai/athigeo
 
 copyright: "Copyright &copy; 2024 - 2024 Dennis Mutai"
 
 theme:
     palette:
         - scheme: default
```

### Comparing `athigeo-0.0.1/pyproject.toml` & `athigeo-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "athigeo"
-version = "0.0.1"
+version = "0.0.3"
 dynamic = [
     "dependencies",
 ]
 description = "A python package intro"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.1"
+current_version = "0.0.3"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

