# Comparing `tmp/geohub-0.0.3.tar.gz` & `tmp/geohub-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geohub-0.0.3.tar", last modified: Thu Mar 28 21:35:05 2024, max compression
+gzip compressed data, was "geohub-0.0.5.tar", last modified: Wed Apr 24 20:39:20 2024, max compression
```

## Comparing `geohub-0.0.3.tar` & `geohub-0.0.5.tar`

### file list

```diff
@@ -1,62 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:35:05.254146 geohub-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-28 21:34:53.000000 geohub-0.0.3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:35:05.246147 geohub-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:35:05.246147 geohub-0.0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-28 21:34:53.000000 geohub-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-28 21:34:53.000000 geohub-0.0.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-28 21:34:53.000000 geohub-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:35:05.250146 geohub-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-03-28 21:34:53.000000 geohub-0.0.3/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-28 21:34:53.000000 geohub-0.0.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-28 21:34:53.000000 geohub-0.0.3/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-28 21:34:53.000000 geohub-0.0.3/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-28 21:34:53.000000 geohub-0.0.3/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-03-28 21:34:53.000000 geohub-0.0.3/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-28 21:34:53.000000 geohub-0.0.3/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-28 21:34:53.000000 geohub-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 21:34:53.000000 geohub-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-28 21:34:53.000000 geohub-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-03-28 21:35:05.254146 geohub-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-28 21:34:53.000000 geohub-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:35:05.250146 geohub-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-28 21:34:53.000000 geohub-0.0.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-28 21:34:53.000000 geohub-0.0.3/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-03-28 21:34:53.000000 geohub-0.0.3/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:35:05.250146 geohub-0.0.3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-28 21:34:53.000000 geohub-0.0.3/docs/examples/cats.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-28 21:34:53.000000 geohub-0.0.3/docs/examples/dogs.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-28 21:34:53.000000 geohub-0.0.3/docs/examples/guest.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-28 21:34:53.000000 geohub-0.0.3/docs/examples/guest_book.txt
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-28 21:34:53.000000 geohub-0.0.3/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12272 2024-03-28 21:34:53.000000 geohub-0.0.3/docs/examples/ipyleaflet.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    28734 2024-03-28 21:34:53.000000 geohub-0.0.3/docs/examples/lab_4.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    46254 2024-03-28 21:34:53.000000 geohub-0.0.3/docs/examples/lab_5.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-28 21:34:53.000000 geohub-0.0.3/docs/examples/learning_python.txt
--rw-r--r--   0 runner    (1001) docker     (127)   186383 2024-03-28 21:34:53.000000 geohub-0.0.3/docs/examples/moral_teachings.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-28 21:34:53.000000 geohub-0.0.3/docs/examples/user_response.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-28 21:34:53.000000 geohub-0.0.3/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-28 21:34:53.000000 geohub-0.0.3/docs/geohub.md
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-28 21:34:53.000000 geohub-0.0.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-28 21:34:53.000000 geohub-0.0.3/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:35:05.250146 geohub-0.0.3/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-28 21:34:53.000000 geohub-0.0.3/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-28 21:34:53.000000 geohub-0.0.3/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:35:05.254146 geohub-0.0.3/geohub/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-28 21:34:53.000000 geohub-0.0.3/geohub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-28 21:34:53.000000 geohub-0.0.3/geohub/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-03-28 21:34:53.000000 geohub-0.0.3/geohub/geohub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:35:05.254146 geohub-0.0.3/geohub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-03-28 21:35:05.000000 geohub-0.0.3/geohub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-28 21:35:05.000000 geohub-0.0.3/geohub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 21:35:05.000000 geohub-0.0.3/geohub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-28 21:35:05.000000 geohub-0.0.3/geohub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-28 21:35:05.000000 geohub-0.0.3/geohub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-28 21:35:05.000000 geohub-0.0.3/geohub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-03-28 21:34:53.000000 geohub-0.0.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-28 21:34:53.000000 geohub-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-28 21:34:53.000000 geohub-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-28 21:34:53.000000 geohub-0.0.3/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 21:35:05.254146 geohub-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:35:05.254146 geohub-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-28 21:34:53.000000 geohub-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-28 21:34:53.000000 geohub-0.0.3/tests/test_geohub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:20.225843 geohub-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-24 20:39:08.000000 geohub-0.0.5/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:20.213843 geohub-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:20.217843 geohub-0.0.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-24 20:39:08.000000 geohub-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-24 20:39:08.000000 geohub-0.0.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-24 20:39:08.000000 geohub-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:20.217843 geohub-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-24 20:39:08.000000 geohub-0.0.5/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-24 20:39:08.000000 geohub-0.0.5/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-24 20:39:08.000000 geohub-0.0.5/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-24 20:39:08.000000 geohub-0.0.5/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-24 20:39:08.000000 geohub-0.0.5/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-24 20:39:08.000000 geohub-0.0.5/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-24 20:39:08.000000 geohub-0.0.5/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-24 20:39:08.000000 geohub-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:39:08.000000 geohub-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-24 20:39:08.000000 geohub-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-24 20:39:20.225843 geohub-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-24 20:39:08.000000 geohub-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:20.217843 geohub-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:20.221843 geohub-0.0.5/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/examples/cats.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/examples/dogs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   117900 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/examples/europe_110.geo.json
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/examples/guest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/examples/guest_book.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15573 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/examples/ipyleaflet.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    74174 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/examples/ipywidget.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    28246 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/examples/lab_4.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    46254 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/examples/lab_5.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/examples/lab_9.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/examples/learning_python.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   186383 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/examples/moral_teachings.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10984 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/examples/raster.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/examples/toolbar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/examples/user_response.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/geohub.md
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:20.221843 geohub-0.0.5/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:20.221843 geohub-0.0.5/docs/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/python/get_started.md
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-24 20:39:08.000000 geohub-0.0.5/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:20.221843 geohub-0.0.5/geohub/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-24 20:39:08.000000 geohub-0.0.5/geohub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-24 20:39:08.000000 geohub-0.0.5/geohub/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10728 2024-04-24 20:39:08.000000 geohub-0.0.5/geohub/geohub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:20.225843 geohub-0.0.5/geohub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-24 20:39:20.000000 geohub-0.0.5/geohub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-24 20:39:20.000000 geohub-0.0.5/geohub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:39:20.000000 geohub-0.0.5/geohub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-24 20:39:20.000000 geohub-0.0.5/geohub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-24 20:39:20.000000 geohub-0.0.5/geohub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 20:39:20.000000 geohub-0.0.5/geohub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-24 20:39:08.000000 geohub-0.0.5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-24 20:39:08.000000 geohub-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-24 20:39:08.000000 geohub-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-24 20:39:08.000000 geohub-0.0.5/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 20:39:20.225843 geohub-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:20.225843 geohub-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-24 20:39:08.000000 geohub-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-24 20:39:08.000000 geohub-0.0.5/tests/test_geohub.py
```

### Comparing `geohub-0.0.3/.github/workflows/docs-build.yml` & `geohub-0.0.5/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `geohub-0.0.3/.github/workflows/docs.yml` & `geohub-0.0.5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `geohub-0.0.3/.github/workflows/installation.yml` & `geohub-0.0.5/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `geohub-0.0.3/.github/workflows/macos.yml` & `geohub-0.0.5/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `geohub-0.0.3/.github/workflows/pypi.yml` & `geohub-0.0.5/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `geohub-0.0.3/.github/workflows/ubuntu.yml` & `geohub-0.0.5/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `geohub-0.0.3/.github/workflows/windows.yml` & `geohub-0.0.5/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `geohub-0.0.3/.gitignore` & `geohub-0.0.5/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 private/
 *.py[cod]
 *$py.class
+*.geo.json
 
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 env/
```

### Comparing `geohub-0.0.3/PKG-INFO` & `geohub-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geohub
-Version: 0.0.3
+Version: 0.0.5
 Summary: A python package created with some data and geospatial analysis skills
 Author-email: Mahnaz Meem <mahnazsarkermeem@gmail.com>
 License: BSD License
 Project-URL: Homepage, https://github.com/mahnaz-meem/geohub
 Keywords: geohub
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -15,14 +15,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: ipyleaflet
+Requires-Dist: geopandas
+Requires-Dist: pandas
+Requires-Dist: localtileserver
+Requires-Dist: rasterio
+Requires-Dist: matplotlib
 Provides-Extra: all
 Requires-Dist: geohub[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # geohub
```

### Comparing `geohub-0.0.3/docs/contributing.md` & `geohub-0.0.5/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `geohub-0.0.3/docs/examples/ipyleaflet.ipynb` & `geohub-0.0.5/docs/examples/raster.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9502354497354497%*

 * *Differences: {"'cells'": "{1: {'execution_count': None, 'outputs': [], 'source': ['# pip install geohub']}, 2: "*

 * *            "{'execution_count': 1, 'outputs': [OrderedDict([('data', "*

 * *            "OrderedDict([('application/vnd.jupyter.widget-view+json', OrderedDict([('model_id', "*

 * *            "'d3d6f4341ca54bb99b2ad14a39aa4ecb'), ('version_major', 2), ('version_minor', 0)])), "*

 * *            '(\'text/plain\', ["Map(center=[25, -115], '*

 * *            "controls=(ZoomControl(options=['position', 'zoom_in_text', 'zoom_in_titl […]*

```diff
@@ -1,412 +1,360 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Raster Analysis and Add Image or GIF\n",
+                "\n",
+                "[![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Mahnaz-Meem/geohub/blob/main/docs/examples/raster.ipynb)"
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# pip install geohub"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "4bee9113495b4d358ba6b489e1172dc0",
+                            "model_id": "d3d6f4341ca54bb99b2ad14a39aa4ecb",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
-                            "Map(center=[52.204793, 360.121558], controls=(ZoomControl(options=['position', 'zoom_in_text', 'zoom_in_title'\u2026"
+                            "Map(center=[25, -115], controls=(ZoomControl(options=['position', 'zoom_in_text', 'zoom_in_title', 'zoom_out_t\u2026"
                         ]
                     },
+                    "execution_count": 1,
                     "metadata": {},
-                    "output_type": "display_data"
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
-                "from ipyleaflet import Map, Marker\n",
-                "\n",
-                "center = (52.204793, 360.121558)\n",
+                "from ipyleaflet import Map, ImageOverlay\n",
                 "\n",
-                "m = Map(center=center, zoom=15)\n",
+                "m = Map(center=(25, -115), zoom=4)\n",
                 "\n",
-                "marker = Marker(location=center, draggable=True)\n",
-                "m.add(marker)\n",
+                "image = ImageOverlay(\n",
+                "    url=\"https://i.imgur.com/06Q1fSz.png\",\n",
+                "    # url='../06Q1fSz.png',\n",
+                "    bounds=((13, -130), (32, -100))\n",
+                ")\n",
                 "\n",
-                "display(m)\n",
-                "\n",
-                "# Now that the marker is on the Map, you can drag it with your mouse,\n",
-                "# it will automatically update the `marker.location` attribute in Python\n",
-                "\n",
-                "# You can also update the marker location from Python, that will update the\n",
-                "# marker location on the Map:\n",
-                "# marker.location = (50, 356)"
+                "m.add(image)\n",
+                "m"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 2,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "3bc2e53f1a7843d0837546b591f3dcab",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
+                        "text/plain": [
+                            "Map(center=[20, 0], controls=(ZoomControl(options=['position', 'zoom_in_text', 'zoom_in_title', 'zoom_out_text\u2026"
+                        ]
+                    },
+                    "execution_count": 2,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
-                "import ipyleaflet"
+                "import geohub\n",
+                "m = geohub.Map()\n",
+                "url=\"https://i.imgur.com/06Q1fSz.png\"\n",
+                "    # url='../06Q1fSz.png',\n",
+                "bounds=((13, -130), (32, -100))\n",
+                "m.add_image(url, bounds)\n",
+                "m.add_layers_control()\n",
+                "m.scroll_wheel_zoom = True\n",
+                "m"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "e9ce42e9cfca401db42cbe90fa09b706",
+                            "model_id": "6fbf248e579a43e58218eb3d79c47855",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
-                            "Map(center=[40, -100], controls=(ZoomControl(options=['position', 'zoom_in_text', 'zoom_in_title', 'zoom_out_t\u2026"
+                            "Map(center=[20, 0], controls=(ZoomControl(options=['position', 'zoom_in_text', 'zoom_in_title', 'zoom_out_text\u2026"
                         ]
                     },
-                    "execution_count": 18,
+                    "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "m = ipyleaflet.Map(center=(40, -100), zoom=4)\n",
+                "# Add gif\n",
+                "m = geohub.Map()\n",
+                "url=\"https://www.reactiongifs.com/r/cheering_minions.gif\"\n",
+                "    # url='../06Q1fSz.png',\n",
+                "bounds=((3, -100), (32, 10))\n",
+                "m.add_image(url, bounds)\n",
+                "m.add_layers_control()\n",
                 "m"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# pip install localtileserver"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "7eb1805f53b740feb6308624a2d67365",
+                            "model_id": "2dca057a44f941c38a0123c44feff1fe",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
-                            "Map(center=[40, -100], controls=(ZoomControl(options=['position', 'zoom_in_text', 'zoom_in_title', 'zoom_out_t\u2026"
+                            "Map(center=[37.752215, -122.418776], controls=(ZoomControl(options=['position', 'zoom_in_text', 'zoom_in_title\u2026"
                         ]
                     },
-                    "execution_count": 20,
+                    "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "m = ipyleaflet.Map(center=(40, -100), zoom=4)\n",
-                "m.scroll_wheel_zoom = True\n",
-                "m.add_control(ipyleaflet.FullScreenControl())\n",
+                "from localtileserver import TileClient, get_leaflet_tile_layer, examples\n",
+                "from ipyleaflet import Map\n",
+                "\n",
+                "# Create a TileClient from a raster file\n",
+                "# client = TileClient('path/to/geo.tif')\n",
+                "client = examples.get_san_francisco()  # use example data\n",
                 "\n",
+                "# Create ipyleaflet TileLayer from that server\n",
+                "t = get_leaflet_tile_layer(client)\n",
+                "# Create ipyleaflet map, add tile layer, and display\n",
+                "m = Map(center=client.center(), zoom=client.default_zoom)\n",
+                "m.add(t)\n",
                 "m"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 5,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "(TileLayer(attribution='&copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors', base=True, max_zoom=19, min_zoom=1, name='OpenStreetMap.Mapnik', options=['attribution', 'bounds', 'detect_retina', 'max_native_zoom', 'max_zoom', 'min_native_zoom', 'min_zoom', 'no_wrap', 'tile_size', 'tms', 'zoom_offset'], url='https://tile.openstreetmap.org/{z}/{x}/{y}.png'),\n",
+                            " BoundTileLayer(attribution=\"Raster file served by <a href='https://github.com/banesullivan/localtileserver' target='_blank'>localtileserver</a>.\", bounds=((37.452199, -122.718792), (38.052231, -122.11876)), loading=True, max_native_zoom=30, max_zoom=30, options=['attribution', 'bounds', 'detect_retina', 'max_native_zoom', 'max_zoom', 'min_native_zoom', 'min_zoom', 'no_wrap', 'tile_size', 'tms', 'zoom_offset'], show_loading=True, url='http://localhost:50624/api/tiles/{z}/{x}/{y}.png?&filename=%2Fvsicurl%3Furl%3Dhttps%253A%252F%252Fdata.kitware.com%252Fapi%252Fv1%252Ffile%252F626854a14acac99f42126a74%252Fdownload%26use_head%3Dno%26list_dir%3Dno'))"
+                        ]
+                    },
+                    "execution_count": 5,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
-                "import geohub"
+                "m.layers"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from geohub.geohub import Map"
+                "import matplotlib.pyplot as plt\n",
+                "from ipyleaflet import Map, ImageOverlay"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "f9c7259d25f84ca880ba3e5f3b7a9146",
+                            "model_id": "da28193f20e242d494554c4a12c07368",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
-                            "Map(center=[20, 0], controls=(ZoomControl(options=['position', 'zoom_in_text', 'zoom_in_title', 'zoom_out_text\u2026"
+                            "Map(center=[37.630466999999996, -119.03021849999999], controls=(ZoomControl(options=['position', 'zoom_in_text\u2026"
                         ]
                     },
-                    "execution_count": 24,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "m=geohub.Map()\n",
+                "import geohub\n",
+                "m = geohub.Map()\n",
+                "data = 'https://github.com/opengeos/datasets/releases/download/raster/srtm90.tif'\n",
+                "m.add_raster(data, name = 'DEM')\n",
+                "# m.add_layers_control()\n",
                 "m"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "990f923e7254475a86aada3d2f2fccc6",
+                            "model_id": "d4a9cbb10010464e8a90e57d57c97825",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
-                            "Map(center=[20, 0], controls=(ZoomControl(options=['position', 'zoom_in_text', 'zoom_in_title', 'zoom_out_text\u2026"
+                            "Map(center=[37.630466999999996, -119.03021849999999], controls=(ZoomControl(options=['position', 'zoom_in_text\u2026"
                         ]
                     },
-                    "execution_count": 26,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "m=geohub.Map()\n",
-                "m.add_basemap('OpenTopoMap')\n",
-                "m.add_layers_control()\n",
+                "from localtileserver import get_leaflet_tile_layer, TileClient\n",
+                "from ipyleaflet import Map\n",
+                "\n",
+                "# First, create a tile server from local raster file\n",
+                "client = TileClient('https://github.com/opengeos/datasets/releases/download/raster/srtm90.tif')\n",
+                "\n",
+                "# Create ipyleaflet tile layer from that server\n",
+                "t = get_leaflet_tile_layer(client, colormap = 'terrain')\n",
+                "\n",
+                "m = Map(center=client.center(), zoom=client.default_zoom)\n",
+                "m.add(t)\n",
                 "m"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "df908df785b747589453805401509fd1",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
                         "text/plain": [
-                            "Map(center=[52.204793, 360.121558], controls=(ZoomControl(options=['position', 'zoom_in_text', 'zoom_in_title'\u2026"
+                            "(TileLayer(attribution='&copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors', base=True, max_zoom=19, min_zoom=1, name='OpenStreetMap.Mapnik', options=['attribution', 'bounds', 'detect_retina', 'max_native_zoom', 'max_zoom', 'min_native_zoom', 'min_zoom', 'no_wrap', 'tile_size', 'tms', 'zoom_offset'], url='https://tile.openstreetmap.org/{z}/{x}/{y}.png'),\n",
+                            " BoundTileLayer(attribution=\"Raster file served by <a href='https://github.com/banesullivan/localtileserver' target='_blank'>localtileserver</a>.\", bounds=((36.634011, -120.755927), (38.626923, -117.30451)), max_native_zoom=30, max_zoom=30, options=['attribution', 'bounds', 'detect_retina', 'max_native_zoom', 'max_zoom', 'min_native_zoom', 'min_zoom', 'no_wrap', 'tile_size', 'tms', 'zoom_offset'], show_loading=True, url='http://localhost:50624/api/tiles/{z}/{x}/{y}.png?&filename=%2Fvsicurl%3Furl%3Dhttps%253A%252F%252Fgithub.com%252Fopengeos%252Fdatasets%252Freleases%252Fdownload%252Fraster%252Fsrtm90.tif%26use_head%3Dno%26list_dir%3Dno&colormap=terrain'))"
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "from ipyleaflet import Map, basemaps\n",
-                "\n",
-                "center = (52.204793, 360.121558)    \n",
-                "zoom = 5\n",
-                "\n",
-                "Map(basemap=basemaps.NASAGIBS.ViirsEarthAtNight2012, center=center, zoom=zoom)"
+                "m.layers"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "(TileLayer(attribution='&copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors', base=True, max_zoom=19, min_zoom=1, name='OpenStreetMap.Mapnik', options=['attribution', 'bounds', 'detect_retina', 'max_native_zoom', 'max_zoom', 'min_native_zoom', 'min_zoom', 'no_wrap', 'tile_size', 'tms', 'zoom_offset'], url='https://tile.openstreetmap.org/{z}/{x}/{y}.png'),)"
+                            "(37.630466999999996, -119.03021849999999)"
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "m.layers"
+                "client.center()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "(ZoomControl(options=['position', 'zoom_in_text', 'zoom_in_title', 'zoom_out_text', 'zoom_out_title']),\n",
-                            " AttributionControl(options=['position', 'prefix'], position='bottomright'))"
+                            "7"
                         ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "m.controls"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 21,
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/html": [
-                            "\n",
-                            "        <div>\n",
-                            "        <style>\n",
-                            "/* CSS stylesheet for displaying xyzservices objects in Jupyter.*/\n",
-                            ".xyz-wrap {\n",
-                            "    --xyz-border-color: var(--jp-border-color2, #ddd);\n",
-                            "    --xyz-font-color2: var(--jp-content-font-color2, rgba(128, 128, 128, 1));\n",
-                            "    --xyz-background-color-white: var(--jp-layout-color1, white);\n",
-                            "    --xyz-background-color: var(--jp-layout-color2, rgba(128, 128, 128, 0.1));\n",
-                            "}\n",
-                            "\n",
-                            "html[theme=dark] .xyz-wrap,\n",
-                            "body.vscode-dark .xyz-wrap,\n",
-                            "body.vscode-high-contrast .xyz-wrap {\n",
-                            "    --xyz-border-color: #222;\n",
-                            "    --xyz-font-color2: rgba(255, 255, 255, 0.54);\n",
-                            "    --xyz-background-color-white: rgba(255, 255, 255, 1);\n",
-                            "    --xyz-background-color: rgba(255, 255, 255, 0.05);\n",
-                            "\n",
-                            "}\n",
-                            "\n",
-                            ".xyz-header {\n",
-                            "    padding-top: 6px;\n",
-                            "    padding-bottom: 6px;\n",
-                            "    margin-bottom: 4px;\n",
-                            "    border-bottom: solid 1px var(--xyz-border-color);\n",
-                            "}\n",
-                            "\n",
-                            ".xyz-header>div {\n",
-                            "    display: inline;\n",
-                            "    margin-top: 0;\n",
-                            "    margin-bottom: 0;\n",
-                            "}\n",
-                            "\n",
-                            ".xyz-obj,\n",
-                            ".xyz-name {\n",
-                            "    margin-left: 2px;\n",
-                            "    margin-right: 10px;\n",
-                            "}\n",
-                            "\n",
-                            ".xyz-obj {\n",
-                            "    color: var(--xyz-font-color2);\n",
-                            "}\n",
-                            "\n",
-                            ".xyz-attrs {\n",
-                            "    grid-column: 1 / -1;\n",
-                            "}\n",
-                            "\n",
-                            "dl.xyz-attrs {\n",
-                            "    padding: 0 5px 0 5px;\n",
-                            "    margin: 0;\n",
-                            "    display: grid;\n",
-                            "    grid-template-columns: 135px auto;\n",
-                            "    background-color: var(--xyz-background-color);\n",
-                            "}\n",
-                            "\n",
-                            ".xyz-attrs dt,\n",
-                            "dd {\n",
-                            "    padding: 0;\n",
-                            "    margin: 0;\n",
-                            "    float: left;\n",
-                            "    padding-right: 10px;\n",
-                            "    width: auto;\n",
-                            "}\n",
-                            "\n",
-                            ".xyz-attrs dt {\n",
-                            "    font-weight: normal;\n",
-                            "    grid-column: 1;\n",
-                            "}\n",
-                            "\n",
-                            ".xyz-attrs dd {\n",
-                            "    grid-column: 2;\n",
-                            "    white-space: pre-wrap;\n",
-                            "    word-break: break-all;\n",
-                            "}\n",
-                            "\n",
-                            ".xyz-details ul>li>label>span {\n",
-                            "    color: var(--xyz-font-color2);\n",
-                            "    padding-left: 10px;\n",
-                            "}\n",
-                            "\n",
-                            ".xyz-inside {\n",
-                            "    display: none;\n",
-                            "}\n",
-                            "\n",
-                            ".xyz-checkbox:checked~.xyz-inside {\n",
-                            "    display: contents;\n",
-                            "}\n",
-                            "\n",
-                            ".xyz-collapsible li>input {\n",
-                            "    display: none;\n",
-                            "}\n",
-                            "\n",
-                            ".xyz-collapsible>li>label {\n",
-                            "    cursor: pointer;\n",
-                            "}\n",
-                            "\n",
-                            ".xyz-collapsible>li>label:hover {\n",
-                            "    color: var(--xyz-font-color2);\n",
-                            "}\n",
-                            "\n",
-                            "ul.xyz-collapsible {\n",
-                            "    list-style: none!important;\n",
-                            "    padding-left: 20px!important;\n",
-                            "}\n",
-                            "\n",
-                            ".xyz-checkbox+label:before {\n",
-                            "    content: '\u25ba';\n",
-                            "    font-size: 11px;\n",
-                            "}\n",
-                            "\n",
-                            ".xyz-checkbox:checked+label:before {\n",
-                            "    content: '\u25bc';\n",
-                            "}\n",
-                            "\n",
-                            ".xyz-wrap {\n",
-                            "    margin-bottom: 10px;\n",
-                            "}\n",
-                            "</style>\n",
-                            "            <div class=\"xyz-wrap\">\n",
-                            "                <div class=\"xyz-header\">\n",
-                            "                    <div class=\"xyz-obj\">xyzservices.TileProvider</div>\n",
-                            "                    <div class=\"xyz-name\">OpenTopoMap</div>\n",
-                            "                </div>\n",
-                            "                <div class=\"xyz-details\">\n",
-                            "                    <dl class=\"xyz-attrs\">\n",
-                            "                        <dt><span>url</span></dt><dd>https://{s}.tile.opentopomap.org/{z}/{x}/{y}.png</dd><dt><span>max_zoom</span></dt><dd>17</dd><dt><span>html_attribution</span></dt><dd>Map data: &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors, <a href=\"http://viewfinderpanoramas.org\">SRTM</a> | Map style: &copy; <a href=\"https://opentopomap.org\">OpenTopoMap</a> (<a href=\"https://creativecommons.org/licenses/by-sa/3.0/\">CC-BY-SA</a>)</dd><dt><span>attribution</span></dt><dd>Map data: (C) OpenStreetMap contributors, SRTM | Map style: (C) OpenTopoMap (CC-BY-SA)</dd>\n",
-                            "                    </dl>\n",
-                            "                </div>\n",
-                            "            </div>\n",
-                            "        </div>\n",
-                            "        "
-                        ],
-                        "text/plain": [
-                            "{'url': 'https://{s}.tile.opentopomap.org/{z}/{x}/{y}.png',\n",
-                            " 'max_zoom': 17,\n",
-                            " 'html_attribution': 'Map data: &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors, <a href=\"http://viewfinderpanoramas.org\">SRTM</a> | Map style: &copy; <a href=\"https://opentopomap.org\">OpenTopoMap</a> (<a href=\"https://creativecommons.org/licenses/by-sa/3.0/\">CC-BY-SA</a>)',\n",
-                            " 'attribution': 'Map data: (C) OpenStreetMap contributors, SRTM | Map style: (C) OpenTopoMap (CC-BY-SA)',\n",
-                            " 'name': 'OpenTopoMap'}"
+                "client.default_zoom"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 12,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "80f17c92099f4b3f8555d7e17f2d6b03",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
+                        "text/plain": [
+                            "Map(center=[37.630466999999996, -119.03021849999999], controls=(ZoomControl(options=['position', 'zoom_in_text\u2026"
                         ]
                     },
-                    "execution_count": 21,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "eval(\"basemaps.OpenTopoMap\")"
+                "import geohub\n",
+                "m = geohub.Map()\n",
+                "data = 'https://github.com/opengeos/datasets/releases/download/raster/srtm90.tif'\n",
+                "m.add_raster(data, name = 'DEM', colormap = 'terrain')\n",
+                "# m.add_layers_control()\n",
+                "m"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "geo",
             "language": "python",
@@ -418,13 +366,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.7"
+            "version": "3.11.8"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `geohub-0.0.3/docs/examples/lab_4.ipynb` & `geohub-0.0.5/docs/examples/lab_4.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997457470414202%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, "*

 * *            "'[![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Mahnaz-Meem/geohub/blob/main/docs/examples/lab_4.ipynb)')], "*

 * *            'delete: [11, 10, 9, 8, 7, 6, 4, 3, 2, 1]}}}'}*

```diff
@@ -3,24 +3,15 @@
         {
             "cell_type": "markdown",
             "id": "0",
             "metadata": {},
             "source": [
                 "# Lab 4\n",
                 "\n",
-                "[![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Mahnaz-Meem/geohub/blob/main/docs/examples/lab_4.ipynb)\n",
-                "\n",
-                "## Submission instructions\n",
-                "\n",
-                "1. Download the notebook from https://geohey.gishub.org/labs/lab4\n",
-                "2. Complete the lab questions\n",
-                "3. Restart Kernel and Run All Cells\n",
-                "4. Upload the notebook to your GitHub repository\n",
-                "5. Make sure the notebook has an `Open In Colab` badge. Click on the badge to make sure your notebook can be opened in Colab.\n",
-                "6. Submit the link to the notebook on your GitHub repository to Canvas"
+                "[![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Mahnaz-Meem/geohub/blob/main/docs/examples/lab_4.ipynb)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 26,
             "id": "1",
             "metadata": {
```

### Comparing `geohub-0.0.3/docs/examples/lab_5.ipynb` & `geohub-0.0.5/docs/examples/lab_5.ipynb`

 * *Files identical despite different names*

### Comparing `geohub-0.0.3/docs/examples/moral_teachings.txt` & `geohub-0.0.5/docs/examples/moral_teachings.txt`

 * *Files identical despite different names*

### Comparing `geohub-0.0.3/docs/installation.md` & `geohub-0.0.5/docs/installation.md`

 * *Files identical despite different names*

### Comparing `geohub-0.0.3/geohub.egg-info/PKG-INFO` & `geohub-0.0.5/geohub.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geohub
-Version: 0.0.3
+Version: 0.0.5
 Summary: A python package created with some data and geospatial analysis skills
 Author-email: Mahnaz Meem <mahnazsarkermeem@gmail.com>
 License: BSD License
 Project-URL: Homepage, https://github.com/mahnaz-meem/geohub
 Keywords: geohub
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -15,14 +15,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: ipyleaflet
+Requires-Dist: geopandas
+Requires-Dist: pandas
+Requires-Dist: localtileserver
+Requires-Dist: rasterio
+Requires-Dist: matplotlib
 Provides-Extra: all
 Requires-Dist: geohub[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # geohub
```

### Comparing `geohub-0.0.3/geohub.egg-info/SOURCES.txt` & `geohub-0.0.5/geohub.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -23,24 +23,30 @@
 docs/faq.md
 docs/geohub.md
 docs/index.md
 docs/installation.md
 docs/usage.md
 docs/examples/cats.txt
 docs/examples/dogs.txt
+docs/examples/europe_110.geo.json
 docs/examples/guest.txt
 docs/examples/guest_book.txt
 docs/examples/intro.ipynb
 docs/examples/ipyleaflet.ipynb
+docs/examples/ipywidget.ipynb
 docs/examples/lab_4.ipynb
 docs/examples/lab_5.ipynb
+docs/examples/lab_9.ipynb
 docs/examples/learning_python.txt
 docs/examples/moral_teachings.txt
+docs/examples/raster.ipynb
+docs/examples/toolbar.ipynb
 docs/examples/user_response.txt
 docs/overrides/main.html
+docs/python/get_started.md
 geohub/__init__.py
 geohub/common.py
 geohub/geohub.py
 geohub.egg-info/PKG-INFO
 geohub.egg-info/SOURCES.txt
 geohub.egg-info/dependency_links.txt
 geohub.egg-info/entry_points.txt
```

### Comparing `geohub-0.0.3/mkdocs.yml` & `geohub-0.0.5/mkdocs.yml`

 * *Files 15% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     # - pdf-export
     - mkdocs-jupyter:
           include_source: True
           ignore_h1_titles: True
           execute: True
           allow_errors: false
           ignore: ["conf.py"]
-          execute_ignore: ["examples/lab_4.ipynb", "examples/lab_5.ipynb"]
+          execute_ignore: ["examples/lab_4.ipynb", "examples/lab_5.ipynb", "examples/ipyleaflet.ipynb"]
           
 markdown_extensions:
     - admonition
     - abbr
     - attr_list
     - def_list
     - footnotes
@@ -71,22 +71,27 @@
 #         provider: google
 #         property: UA-XXXXXXXXX-X
 
 nav:
     - Home: index.md
     - Installation: installation.md
     - Usage: usage.md
+    - Get Started: get_started.md
     - Contributing: contributing.md
     - FAQ: faq.md
     - Changelog: changelog.md
     - Report Issues: https://github.com/mahnaz-meem/geohub/issues
     - Examples:
         - examples/intro.ipynb
-        - examples/lab_4.ipynb
-        - examples/lab_5.ipynb
+        - examples/ipyleaflet.ipynb
+        - examples/ipywidget.ipynb
+        - examples/raster.ipynb
+        - examples/toolbar.ipynb
 
     - API Reference:
           - geohub module: geohub.md
           - common module: common.md
     - Labs:
         - examples/lab_4.ipynb
         - examples/lab_5.ipynb
+        - examples/lab_9.ipynb
+
```

### Comparing `geohub-0.0.3/pyproject.toml` & `geohub-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "geohub"
-version = "0.0.3"
+version = "0.0.5"
 dynamic = [
     "dependencies",
 ]
 description = "A python package created with some data and geospatial analysis skills"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.3"
+current_version = "0.0.5"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

