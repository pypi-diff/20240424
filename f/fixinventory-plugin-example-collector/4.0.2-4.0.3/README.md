# Comparing `tmp/fixinventory-plugin-example-collector-4.0.2.tar.gz` & `tmp/fixinventory_plugin_example_collector-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory-plugin-example-collector-4.0.2.tar", last modified: Fri Apr 12 12:13:54 2024, max compression
+gzip compressed data, was "fixinventory_plugin_example_collector-4.0.3.tar", last modified: Wed Apr 24 10:32:11 2024, max compression
```

## Comparing `fixinventory-plugin-example-collector-4.0.2.tar` & `fixinventory_plugin_example_collector-4.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:54.376283 fixinventory-plugin-example-collector-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:10:59.000000 fixinventory-plugin-example-collector-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-12 12:13:54.376283 fixinventory-plugin-example-collector-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-12 12:10:59.000000 fixinventory-plugin-example-collector-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:54.376283 fixinventory-plugin-example-collector-4.0.2/fix_plugin_example_collector/
--rw-r--r--   0 runner    (1001) docker     (127)     8244 2024-04-12 12:10:59.000000 fixinventory-plugin-example-collector-4.0.2/fix_plugin_example_collector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:54.376283 fixinventory-plugin-example-collector-4.0.2/fixinventory_plugin_example_collector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-12 12:13:54.000000 fixinventory-plugin-example-collector-4.0.2/fixinventory_plugin_example_collector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-12 12:13:54.000000 fixinventory-plugin-example-collector-4.0.2/fixinventory_plugin_example_collector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:13:54.000000 fixinventory-plugin-example-collector-4.0.2/fixinventory_plugin_example_collector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-12 12:13:54.000000 fixinventory-plugin-example-collector-4.0.2/fixinventory_plugin_example_collector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:12:09.000000 fixinventory-plugin-example-collector-4.0.2/fixinventory_plugin_example_collector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 12:13:54.000000 fixinventory-plugin-example-collector-4.0.2/fixinventory_plugin_example_collector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 12:13:54.000000 fixinventory-plugin-example-collector-4.0.2/fixinventory_plugin_example_collector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-12 12:10:59.000000 fixinventory-plugin-example-collector-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 12:13:54.380282 fixinventory-plugin-example-collector-4.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:54.376283 fixinventory-plugin-example-collector-4.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-12 12:10:59.000000 fixinventory-plugin-example-collector-4.0.2/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-12 12:10:59.000000 fixinventory-plugin-example-collector-4.0.2/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:11.704620 fixinventory_plugin_example_collector-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 10:29:14.000000 fixinventory_plugin_example_collector-4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-24 10:32:11.704620 fixinventory_plugin_example_collector-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-24 10:29:14.000000 fixinventory_plugin_example_collector-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:11.700620 fixinventory_plugin_example_collector-4.0.3/fix_plugin_example_collector/
+-rw-r--r--   0 runner    (1001) docker     (127)     8244 2024-04-24 10:29:14.000000 fixinventory_plugin_example_collector-4.0.3/fix_plugin_example_collector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:11.704620 fixinventory_plugin_example_collector-4.0.3/fixinventory_plugin_example_collector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-24 10:32:11.000000 fixinventory_plugin_example_collector-4.0.3/fixinventory_plugin_example_collector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-24 10:32:11.000000 fixinventory_plugin_example_collector-4.0.3/fixinventory_plugin_example_collector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:32:11.000000 fixinventory_plugin_example_collector-4.0.3/fixinventory_plugin_example_collector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-24 10:32:11.000000 fixinventory_plugin_example_collector-4.0.3/fixinventory_plugin_example_collector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:30:23.000000 fixinventory_plugin_example_collector-4.0.3/fixinventory_plugin_example_collector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-24 10:32:11.000000 fixinventory_plugin_example_collector-4.0.3/fixinventory_plugin_example_collector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-24 10:32:11.000000 fixinventory_plugin_example_collector-4.0.3/fixinventory_plugin_example_collector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-24 10:29:14.000000 fixinventory_plugin_example_collector-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 10:32:11.704620 fixinventory_plugin_example_collector-4.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:11.704620 fixinventory_plugin_example_collector-4.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-24 10:29:14.000000 fixinventory_plugin_example_collector-4.0.3/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-24 10:29:14.000000 fixinventory_plugin_example_collector-4.0.3/test/test_config.py
```

### Comparing `fixinventory-plugin-example-collector-4.0.2/PKG-INFO` & `fixinventory_plugin_example_collector-4.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-example-collector
-Version: 4.0.2
+Version: 4.0.3
 Summary: Fix Example Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/example_collector
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
@@ -15,14 +15,14 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.2
+Requires-Dist: fixinventorylib==4.0.3
 
 # fix-plugin-example-collector
 Example Collector Plugin for Fix
 
 ## License
 See [LICENSE](../../LICENSE) for details.
```

### Comparing `fixinventory-plugin-example-collector-4.0.2/fix_plugin_example_collector/__init__.py` & `fixinventory_plugin_example_collector-4.0.3/fix_plugin_example_collector/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-example-collector-4.0.2/fixinventory_plugin_example_collector.egg-info/PKG-INFO` & `fixinventory_plugin_example_collector-4.0.3/fixinventory_plugin_example_collector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-example-collector
-Version: 4.0.2
+Version: 4.0.3
 Summary: Fix Example Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/example_collector
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
@@ -15,14 +15,14 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.2
+Requires-Dist: fixinventorylib==4.0.3
 
 # fix-plugin-example-collector
 Example Collector Plugin for Fix
 
 ## License
 See [LICENSE](../../LICENSE) for details.
```

### Comparing `fixinventory-plugin-example-collector-4.0.2/fixinventory_plugin_example_collector.egg-info/SOURCES.txt` & `fixinventory_plugin_example_collector-4.0.3/fixinventory_plugin_example_collector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-example-collector-4.0.2/pyproject.toml` & `fixinventory_plugin_example_collector-4.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fixinventory-plugin-example-collector"
 description = "Fix Example Collector Plugin"
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
 example_collector = "fix_plugin_example_collector:ExampleCollectorPlugin"
 
 [project.urls]
 Documentation = "https://inventory.fix.security"
```

