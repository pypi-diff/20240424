# Comparing `tmp/girder-sentry-3.2.4.dev7.tar.gz` & `tmp/girder-sentry-5.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-sentry-3.2.4.dev7.tar", last modified: Wed Apr 24 19:13:46 2024, max compression
+gzip compressed data, was "girder-sentry-5.0.0a2.tar", last modified: Fri Apr 12 16:32:16 2024, max compression
```

## Comparing `girder-sentry-3.2.4.dev7.tar` & `girder-sentry-5.0.0a2.tar`

### file list

```diff
@@ -1,27 +1,22 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:46.018448 girder-sentry-3.2.4.dev7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      569 2024-04-24 19:13:46.018448 girder-sentry-3.2.4.dev7/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:46.014449 girder-sentry-3.2.4.dev7/girder_sentry/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2024-04-24 19:11:47.000000 girder-sentry-3.2.4.dev7/girder_sentry/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2024-04-24 19:11:47.000000 girder-sentry-3.2.4.dev7/girder_sentry/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      579 2024-04-24 19:11:47.000000 girder-sentry-3.2.4.dev7/girder_sentry/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:46.018448 girder-sentry-3.2.4.dev7/girder_sentry/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-04-24 19:11:47.000000 girder-sentry-3.2.4.dev7/girder_sentry/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2024-04-24 19:11:47.000000 girder-sentry-3.2.4.dev7/girder_sentry/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      414 2024-04-24 19:11:47.000000 girder-sentry-3.2.4.dev7/girder_sentry/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:46.018448 girder-sentry-3.2.4.dev7/girder_sentry/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2024-04-24 19:11:47.000000 girder-sentry-3.2.4.dev7/girder_sentry/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:46.018448 girder-sentry-3.2.4.dev7/girder_sentry/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      809 2024-04-24 19:11:47.000000 girder-sentry-3.2.4.dev7/girder_sentry/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:46.018448 girder-sentry-3.2.4.dev7/girder_sentry/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2728 2024-04-24 19:11:47.000000 girder-sentry-3.2.4.dev7/girder_sentry/web_client/views/ConfigView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:46.018448 girder-sentry-3.2.4.dev7/girder_sentry.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      569 2024-04-24 19:13:45.000000 girder-sentry-3.2.4.dev7/girder_sentry.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      609 2024-04-24 19:13:45.000000 girder-sentry-3.2.4.dev7/girder_sentry.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:13:45.000000 girder-sentry-3.2.4.dev7/girder_sentry.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2024-04-24 19:13:45.000000 girder-sentry-3.2.4.dev7/girder_sentry.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:13:45.000000 girder-sentry-3.2.4.dev7/girder_sentry.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2024-04-24 19:13:45.000000 girder-sentry-3.2.4.dev7/girder_sentry.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-04-24 19:13:45.000000 girder-sentry-3.2.4.dev7/girder_sentry.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       51 2024-04-24 19:11:47.000000 girder-sentry-3.2.4.dev7/plugin.cmake
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-24 19:13:46.018448 girder-sentry-3.2.4.dev7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1639 2024-04-24 19:11:47.000000 girder-sentry-3.2.4.dev7/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:16.817269 girder-sentry-5.0.0a2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      146 2024-04-12 16:27:18.000000 girder-sentry-5.0.0a2/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      566 2024-04-12 16:32:16.817269 girder-sentry-5.0.0a2/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:16.817269 girder-sentry-5.0.0a2/girder_sentry/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      686 2024-04-12 16:27:18.000000 girder-sentry-5.0.0a2/girder_sentry/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2024-04-12 16:27:18.000000 girder-sentry-5.0.0a2/girder_sentry/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      579 2024-04-12 16:27:18.000000 girder-sentry-5.0.0a2/girder_sentry/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:16.817269 girder-sentry-5.0.0a2/girder_sentry/web_client/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:16.817269 girder-sentry-5.0.0a2/girder_sentry/web_client/dist/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74123 2024-04-12 16:28:46.000000 girder-sentry-5.0.0a2/girder_sentry/web_client/dist/girder-plugin-sentry.umd.cjs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      206 2024-04-12 16:28:46.000000 girder-sentry-5.0.0a2/girder_sentry/web_client/dist/style.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:16.817269 girder-sentry-5.0.0a2/girder_sentry.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      566 2024-04-12 16:32:16.000000 girder-sentry-5.0.0a2/girder_sentry.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      466 2024-04-12 16:32:16.000000 girder-sentry-5.0.0a2/girder_sentry.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:32:16.000000 girder-sentry-5.0.0a2/girder_sentry.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2024-04-12 16:32:16.000000 girder-sentry-5.0.0a2/girder_sentry.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:32:16.000000 girder-sentry-5.0.0a2/girder_sentry.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2024-04-12 16:32:16.000000 girder-sentry-5.0.0a2/girder_sentry.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-04-12 16:32:16.000000 girder-sentry-5.0.0a2/girder_sentry.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       51 2024-04-12 16:27:18.000000 girder-sentry-5.0.0a2/plugin.cmake
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 16:32:16.817269 girder-sentry-5.0.0a2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1639 2024-04-12 16:27:18.000000 girder-sentry-5.0.0a2/setup.py
```

### Comparing `girder-sentry-3.2.4.dev7/PKG-INFO` & `girder-sentry-5.0.0a2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-sentry
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Allow the automatic tracking of issues using Sentry.
 Maintainer: Kitware, Inc.
 Maintainer-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-sentry-3.2.4.dev7/girder_sentry/rest.py` & `girder-sentry-5.0.0a2/girder_sentry/rest.py`

 * *Files identical despite different names*

### Comparing `girder-sentry-3.2.4.dev7/girder_sentry/settings.py` & `girder-sentry-5.0.0a2/girder_sentry/settings.py`

 * *Files identical despite different names*

### Comparing `girder-sentry-3.2.4.dev7/girder_sentry.egg-info/PKG-INFO` & `girder-sentry-5.0.0a2/girder_sentry.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-sentry
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Allow the automatic tracking of issues using Sentry.
 Maintainer: Kitware, Inc.
 Maintainer-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-sentry-3.2.4.dev7/setup.py` & `girder-sentry-5.0.0a2/setup.py`

 * *Files identical despite different names*

