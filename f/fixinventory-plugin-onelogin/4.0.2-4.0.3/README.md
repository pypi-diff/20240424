# Comparing `tmp/fixinventory-plugin-onelogin-4.0.2.tar.gz` & `tmp/fixinventory_plugin_onelogin-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory-plugin-onelogin-4.0.2.tar", last modified: Fri Apr 12 12:13:49 2024, max compression
+gzip compressed data, was "fixinventory_plugin_onelogin-4.0.3.tar", last modified: Wed Apr 24 10:32:20 2024, max compression
```

## Comparing `fixinventory-plugin-onelogin-4.0.2.tar` & `fixinventory_plugin_onelogin-4.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:49.560401 fixinventory-plugin-onelogin-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:10:50.000000 fixinventory-plugin-onelogin-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-12 12:13:49.560401 fixinventory-plugin-onelogin-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-12 12:10:50.000000 fixinventory-plugin-onelogin-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:49.556401 fixinventory-plugin-onelogin-4.0.2/fix_plugin_onelogin/
--rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-04-12 12:10:50.000000 fixinventory-plugin-onelogin-4.0.2/fix_plugin_onelogin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-12 12:10:50.000000 fixinventory-plugin-onelogin-4.0.2/fix_plugin_onelogin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:49.556401 fixinventory-plugin-onelogin-4.0.2/fixinventory_plugin_onelogin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-12 12:13:49.000000 fixinventory-plugin-onelogin-4.0.2/fixinventory_plugin_onelogin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-12 12:13:49.000000 fixinventory-plugin-onelogin-4.0.2/fixinventory_plugin_onelogin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:13:49.000000 fixinventory-plugin-onelogin-4.0.2/fixinventory_plugin_onelogin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-12 12:13:49.000000 fixinventory-plugin-onelogin-4.0.2/fixinventory_plugin_onelogin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:11:59.000000 fixinventory-plugin-onelogin-4.0.2/fixinventory_plugin_onelogin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-12 12:13:49.000000 fixinventory-plugin-onelogin-4.0.2/fixinventory_plugin_onelogin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 12:13:49.000000 fixinventory-plugin-onelogin-4.0.2/fixinventory_plugin_onelogin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-12 12:10:50.000000 fixinventory-plugin-onelogin-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 12:13:49.560401 fixinventory-plugin-onelogin-4.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:49.556401 fixinventory-plugin-onelogin-4.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-12 12:10:50.000000 fixinventory-plugin-onelogin-4.0.2/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:20.528850 fixinventory_plugin_onelogin-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 10:29:15.000000 fixinventory_plugin_onelogin-4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-24 10:32:20.528850 fixinventory_plugin_onelogin-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-24 10:29:15.000000 fixinventory_plugin_onelogin-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:20.528850 fixinventory_plugin_onelogin-4.0.3/fix_plugin_onelogin/
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-04-24 10:29:15.000000 fixinventory_plugin_onelogin-4.0.3/fix_plugin_onelogin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-24 10:29:15.000000 fixinventory_plugin_onelogin-4.0.3/fix_plugin_onelogin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:20.528850 fixinventory_plugin_onelogin-4.0.3/fixinventory_plugin_onelogin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-24 10:32:20.000000 fixinventory_plugin_onelogin-4.0.3/fixinventory_plugin_onelogin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-24 10:32:20.000000 fixinventory_plugin_onelogin-4.0.3/fixinventory_plugin_onelogin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:32:20.000000 fixinventory_plugin_onelogin-4.0.3/fixinventory_plugin_onelogin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-24 10:32:20.000000 fixinventory_plugin_onelogin-4.0.3/fixinventory_plugin_onelogin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:30:29.000000 fixinventory_plugin_onelogin-4.0.3/fixinventory_plugin_onelogin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-24 10:32:20.000000 fixinventory_plugin_onelogin-4.0.3/fixinventory_plugin_onelogin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 10:32:20.000000 fixinventory_plugin_onelogin-4.0.3/fixinventory_plugin_onelogin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-24 10:29:15.000000 fixinventory_plugin_onelogin-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 10:32:20.528850 fixinventory_plugin_onelogin-4.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:20.528850 fixinventory_plugin_onelogin-4.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-24 10:29:15.000000 fixinventory_plugin_onelogin-4.0.3/test/test_config.py
```

### Comparing `fixinventory-plugin-onelogin-4.0.2/PKG-INFO` & `fixinventory_plugin_onelogin-4.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-onelogin
-Version: 4.0.2
+Version: 4.0.3
 Summary: Fix OneLogin Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/onelogin
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
@@ -15,15 +15,15 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.2
+Requires-Dist: fixinventorylib==4.0.3
 Requires-Dist: onelogin==2.0.4
 
 # fix-plugin-onelogin
 OneLogin collector plugin for Fix
 
 This plugin collects OneLogin users as cloud resources and adds them to the Fix graph for use by other plugins.
```

### Comparing `fixinventory-plugin-onelogin-4.0.2/fix_plugin_onelogin/__init__.py` & `fixinventory_plugin_onelogin-4.0.3/fix_plugin_onelogin/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-onelogin-4.0.2/fixinventory_plugin_onelogin.egg-info/PKG-INFO` & `fixinventory_plugin_onelogin-4.0.3/fixinventory_plugin_onelogin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-onelogin
-Version: 4.0.2
+Version: 4.0.3
 Summary: Fix OneLogin Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/onelogin
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
@@ -15,15 +15,15 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.2
+Requires-Dist: fixinventorylib==4.0.3
 Requires-Dist: onelogin==2.0.4
 
 # fix-plugin-onelogin
 OneLogin collector plugin for Fix
 
 This plugin collects OneLogin users as cloud resources and adds them to the Fix graph for use by other plugins.
```

### Comparing `fixinventory-plugin-onelogin-4.0.2/pyproject.toml` & `fixinventory_plugin_onelogin-4.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fixinventory-plugin-onelogin"
 description = "Fix OneLogin Plugin"
-version = "4.0.2"
+version = "4.0.3"
 authors = [{name="Some Engineering Inc."}]
 license = { text="AGPLv3" }
 requires-python = ">=3.11"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "fixinventorylib==4.0.2",
+    "fixinventorylib==4.0.3",
     "onelogin==2.0.4",
 ]
 
 [project.entry-points."fix.plugins"]
 onelogin = "fix_plugin_onelogin:OneLoginPlugin"
 
 [project.urls]
```

