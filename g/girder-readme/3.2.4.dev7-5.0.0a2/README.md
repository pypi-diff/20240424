# Comparing `tmp/girder-readme-3.2.4.dev7.tar.gz` & `tmp/girder-readme-5.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-readme-3.2.4.dev7.tar", last modified: Wed Apr 24 19:13:42 2024, max compression
+gzip compressed data, was "girder-readme-5.0.0a2.tar", last modified: Fri Apr 12 16:32:04 2024, max compression
```

## Comparing `girder-readme-3.2.4.dev7.tar` & `girder-readme-5.0.0a2.tar`

### file list

```diff
@@ -1,29 +1,21 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:42.978452 girder-readme-3.2.4.dev7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2024-04-24 19:13:42.978452 girder-readme-3.2.4.dev7/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:42.974452 girder-readme-3.2.4.dev7/girder_readme/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      284 2024-04-24 19:11:47.000000 girder-readme-3.2.4.dev7/girder_readme/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      991 2024-04-24 19:11:47.000000 girder-readme-3.2.4.dev7/girder_readme/rest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:42.974452 girder-readme-3.2.4.dev7/girder_readme/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2024-04-24 19:11:47.000000 girder-readme-3.2.4.dev7/girder_readme/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      470 2024-04-24 19:11:47.000000 girder-readme-3.2.4.dev7/girder_readme/web_client/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:42.978452 girder-readme-3.2.4.dev7/girder_readme/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2024-04-24 19:11:47.000000 girder-readme-3.2.4.dev7/girder_readme/web_client/stylesheets/readmeWidget.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:42.978452 girder-readme-3.2.4.dev7/girder_readme/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      101 2024-04-24 19:11:47.000000 girder-readme-3.2.4.dev7/girder_readme/web_client/templates/readmeWidget.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:42.978452 girder-readme-3.2.4.dev7/girder_readme/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      997 2024-04-24 19:11:47.000000 girder-readme-3.2.4.dev7/girder_readme/web_client/views/HierarchyWidget.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:42.978452 girder-readme-3.2.4.dev7/girder_readme.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2024-04-24 19:13:42.000000 girder-readme-3.2.4.dev7/girder_readme.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      612 2024-04-24 19:13:42.000000 girder-readme-3.2.4.dev7/girder_readme.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:13:42.000000 girder-readme-3.2.4.dev7/girder_readme.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2024-04-24 19:13:42.000000 girder-readme-3.2.4.dev7/girder_readme.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:13:42.000000 girder-readme-3.2.4.dev7/girder_readme.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-24 19:13:42.000000 girder-readme-3.2.4.dev7/girder_readme.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-04-24 19:13:42.000000 girder-readme-3.2.4.dev7/girder_readme.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       51 2024-04-24 19:11:47.000000 girder-readme-3.2.4.dev7/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:42.978452 girder-readme-3.2.4.dev7/plugin_tests/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:42.978452 girder-readme-3.2.4.dev7/plugin_tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-04-24 19:11:47.000000 girder-readme-3.2.4.dev7/plugin_tests/data/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2024-04-24 19:11:47.000000 girder-readme-3.2.4.dev7/plugin_tests/readmeSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-24 19:13:42.978452 girder-readme-3.2.4.dev7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1543 2024-04-24 19:11:47.000000 girder-readme-3.2.4.dev7/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:04.053178 girder-readme-5.0.0a2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      146 2024-04-12 16:27:18.000000 girder-readme-5.0.0a2/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      515 2024-04-12 16:32:04.049178 girder-readme-5.0.0a2/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:04.045178 girder-readme-5.0.0a2/girder_readme/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      566 2024-04-12 16:27:18.000000 girder-readme-5.0.0a2/girder_readme/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      991 2024-04-12 16:27:18.000000 girder-readme-5.0.0a2/girder_readme/rest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:04.045178 girder-readme-5.0.0a2/girder_readme/web_client/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:04.049178 girder-readme-5.0.0a2/girder_readme/web_client/dist/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1852 2024-04-12 16:28:42.000000 girder-readme-5.0.0a2/girder_readme/web_client/dist/girder-plugin-readme.umd.cjs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      270 2024-04-12 16:28:42.000000 girder-readme-5.0.0a2/girder_readme/web_client/dist/style.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:04.049178 girder-readme-5.0.0a2/girder_readme.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      515 2024-04-12 16:32:03.000000 girder-readme-5.0.0a2/girder_readme.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      440 2024-04-12 16:32:04.000000 girder-readme-5.0.0a2/girder_readme.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:32:03.000000 girder-readme-5.0.0a2/girder_readme.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2024-04-12 16:32:03.000000 girder-readme-5.0.0a2/girder_readme.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:32:03.000000 girder-readme-5.0.0a2/girder_readme.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-12 16:32:03.000000 girder-readme-5.0.0a2/girder_readme.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-04-12 16:32:03.000000 girder-readme-5.0.0a2/girder_readme.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       51 2024-04-12 16:27:18.000000 girder-readme-5.0.0a2/plugin.cmake
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 16:32:04.053178 girder-readme-5.0.0a2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1543 2024-04-12 16:27:18.000000 girder-readme-5.0.0a2/setup.py
```

### Comparing `girder-readme-3.2.4.dev7/PKG-INFO` & `girder-readme-5.0.0a2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-readme
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Render READMEs from the folder view
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-readme-3.2.4.dev7/girder_readme/rest.py` & `girder-readme-5.0.0a2/girder_readme/rest.py`

 * *Files identical despite different names*

### Comparing `girder-readme-3.2.4.dev7/girder_readme.egg-info/PKG-INFO` & `girder-readme-5.0.0a2/girder_readme.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-readme
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Render READMEs from the folder view
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-readme-3.2.4.dev7/setup.py` & `girder-readme-5.0.0a2/setup.py`

 * *Files identical despite different names*

