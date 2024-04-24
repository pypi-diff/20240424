# Comparing `tmp/fixinventory-plugin-random-4.0.2.tar.gz` & `tmp/fixinventory_plugin_random-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory-plugin-random-4.0.2.tar", last modified: Fri Apr 12 12:13:48 2024, max compression
+gzip compressed data, was "fixinventory_plugin_random-4.0.3.tar", last modified: Wed Apr 24 10:32:12 2024, max compression
```

## Comparing `fixinventory-plugin-random-4.0.2.tar` & `fixinventory_plugin_random-4.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:48.001354 fixinventory-plugin-random-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:10:58.000000 fixinventory-plugin-random-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-12 12:13:48.001354 fixinventory-plugin-random-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-12 12:10:58.000000 fixinventory-plugin-random-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:48.001354 fixinventory-plugin-random-4.0.2/fix_plugin_random/
--rw-r--r--   0 runner    (1001) docker     (127)    11001 2024-04-12 12:10:58.000000 fixinventory-plugin-random-4.0.2/fix_plugin_random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-12 12:10:58.000000 fixinventory-plugin-random-4.0.2/fix_plugin_random/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-12 12:10:58.000000 fixinventory-plugin-random-4.0.2/fix_plugin_random/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:48.001354 fixinventory-plugin-random-4.0.2/fixinventory_plugin_random.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-12 12:13:47.000000 fixinventory-plugin-random-4.0.2/fixinventory_plugin_random.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-12 12:13:47.000000 fixinventory-plugin-random-4.0.2/fixinventory_plugin_random.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:13:47.000000 fixinventory-plugin-random-4.0.2/fixinventory_plugin_random.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-12 12:13:47.000000 fixinventory-plugin-random-4.0.2/fixinventory_plugin_random.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:12:03.000000 fixinventory-plugin-random-4.0.2/fixinventory_plugin_random.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 12:13:47.000000 fixinventory-plugin-random-4.0.2/fixinventory_plugin_random.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:13:47.000000 fixinventory-plugin-random-4.0.2/fixinventory_plugin_random.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-12 12:10:58.000000 fixinventory-plugin-random-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 12:13:48.001354 fixinventory-plugin-random-4.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:48.001354 fixinventory-plugin-random-4.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-12 12:10:58.000000 fixinventory-plugin-random-4.0.2/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:12.827545 fixinventory_plugin_random-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 10:29:13.000000 fixinventory_plugin_random-4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-24 10:32:12.827545 fixinventory_plugin_random-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-24 10:29:13.000000 fixinventory_plugin_random-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:12.827545 fixinventory_plugin_random-4.0.3/fix_plugin_random/
+-rw-r--r--   0 runner    (1001) docker     (127)    11001 2024-04-24 10:29:13.000000 fixinventory_plugin_random-4.0.3/fix_plugin_random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-24 10:29:13.000000 fixinventory_plugin_random-4.0.3/fix_plugin_random/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-24 10:29:13.000000 fixinventory_plugin_random-4.0.3/fix_plugin_random/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:12.827545 fixinventory_plugin_random-4.0.3/fixinventory_plugin_random.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-24 10:32:12.000000 fixinventory_plugin_random-4.0.3/fixinventory_plugin_random.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-24 10:32:12.000000 fixinventory_plugin_random-4.0.3/fixinventory_plugin_random.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:32:12.000000 fixinventory_plugin_random-4.0.3/fixinventory_plugin_random.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-24 10:32:12.000000 fixinventory_plugin_random-4.0.3/fixinventory_plugin_random.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:30:21.000000 fixinventory_plugin_random-4.0.3/fixinventory_plugin_random.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-24 10:32:12.000000 fixinventory_plugin_random-4.0.3/fixinventory_plugin_random.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 10:32:12.000000 fixinventory_plugin_random-4.0.3/fixinventory_plugin_random.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-24 10:29:13.000000 fixinventory_plugin_random-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 10:32:12.831544 fixinventory_plugin_random-4.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:12.827545 fixinventory_plugin_random-4.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-24 10:29:13.000000 fixinventory_plugin_random-4.0.3/test/test_config.py
```

### Comparing `fixinventory-plugin-random-4.0.2/PKG-INFO` & `fixinventory_plugin_random-4.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-random
-Version: 4.0.2
+Version: 4.0.3
 Summary: Fix Random Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/random
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
 
 # fix-plugin-random
 Random Cloud Collector for Fix
 
 Creates a plausible pseudo-random cloud based on a configurable seed.
 
 The base infrastructure stays the same, but the number of instances vary slightly from run to run so that metrics show some more interesting up/down lines.
```

### Comparing `fixinventory-plugin-random-4.0.2/README.md` & `fixinventory_plugin_random-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-random-4.0.2/fix_plugin_random/__init__.py` & `fixinventory_plugin_random-4.0.3/fix_plugin_random/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-random-4.0.2/fix_plugin_random/resources.py` & `fixinventory_plugin_random-4.0.3/fix_plugin_random/resources.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-random-4.0.2/fixinventory_plugin_random.egg-info/PKG-INFO` & `fixinventory_plugin_random-4.0.3/fixinventory_plugin_random.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-random
-Version: 4.0.2
+Version: 4.0.3
 Summary: Fix Random Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/random
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
 
 # fix-plugin-random
 Random Cloud Collector for Fix
 
 Creates a plausible pseudo-random cloud based on a configurable seed.
 
 The base infrastructure stays the same, but the number of instances vary slightly from run to run so that metrics show some more interesting up/down lines.
```

### Comparing `fixinventory-plugin-random-4.0.2/pyproject.toml` & `fixinventory_plugin_random-4.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fixinventory-plugin-random"
 description = "Fix Random Collector Plugin"
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
 ]
 
 [project.entry-points."fix.plugins"]
 random = "fix_plugin_random:RandomCollectorPlugin"
 
 [project.urls]
 Documentation = "https://inventory.fix.security"
```

