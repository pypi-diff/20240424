# Comparing `tmp/fixinventory_plugin_k8s-4.0.3.tar.gz` & `tmp/fixinventory_plugin_k8s-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory_plugin_k8s-4.0.3.tar", last modified: Wed Apr 24 10:36:59 2024, max compression
+gzip compressed data, was "fixinventory_plugin_k8s-4.0.4.tar", last modified: Wed Apr 24 19:34:38 2024, max compression
```

## Comparing `fixinventory_plugin_k8s-4.0.3.tar` & `fixinventory_plugin_k8s-4.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:59.443378 fixinventory_plugin_k8s-4.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 10:33:00.000000 fixinventory_plugin_k8s-4.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-24 10:36:59.443378 fixinventory_plugin_k8s-4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-24 10:33:00.000000 fixinventory_plugin_k8s-4.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:59.443378 fixinventory_plugin_k8s-4.0.3/fix_plugin_k8s/
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-24 10:33:00.000000 fixinventory_plugin_k8s-4.0.3/fix_plugin_k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19414 2024-04-24 10:33:00.000000 fixinventory_plugin_k8s-4.0.3/fix_plugin_k8s/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-24 10:33:00.000000 fixinventory_plugin_k8s-4.0.3/fix_plugin_k8s/collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:59.443378 fixinventory_plugin_k8s-4.0.3/fix_plugin_k8s/deferred_edges/
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-24 10:33:00.000000 fixinventory_plugin_k8s-4.0.3/fix_plugin_k8s/deferred_edges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-24 10:33:00.000000 fixinventory_plugin_k8s-4.0.3/fix_plugin_k8s/deferred_edges/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-24 10:33:00.000000 fixinventory_plugin_k8s-4.0.3/fix_plugin_k8s/deferred_edges/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-24 10:33:00.000000 fixinventory_plugin_k8s-4.0.3/fix_plugin_k8s/deferred_edges/digitalocean.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-24 10:33:00.000000 fixinventory_plugin_k8s-4.0.3/fix_plugin_k8s/deferred_edges/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   150075 2024-04-24 10:33:00.000000 fixinventory_plugin_k8s-4.0.3/fix_plugin_k8s/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:59.443378 fixinventory_plugin_k8s-4.0.3/fixinventory_plugin_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-24 10:36:59.000000 fixinventory_plugin_k8s-4.0.3/fixinventory_plugin_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-24 10:36:59.000000 fixinventory_plugin_k8s-4.0.3/fixinventory_plugin_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:36:59.000000 fixinventory_plugin_k8s-4.0.3/fixinventory_plugin_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 10:36:59.000000 fixinventory_plugin_k8s-4.0.3/fixinventory_plugin_k8s.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:34:12.000000 fixinventory_plugin_k8s-4.0.3/fixinventory_plugin_k8s.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-24 10:36:59.000000 fixinventory_plugin_k8s-4.0.3/fixinventory_plugin_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 10:36:59.000000 fixinventory_plugin_k8s-4.0.3/fixinventory_plugin_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-24 10:33:00.000000 fixinventory_plugin_k8s-4.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-24 10:36:59.443378 fixinventory_plugin_k8s-4.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:34:38.567369 fixinventory_plugin_k8s-4.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 19:30:49.000000 fixinventory_plugin_k8s-4.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-24 19:34:38.567369 fixinventory_plugin_k8s-4.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-24 19:30:49.000000 fixinventory_plugin_k8s-4.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:34:38.563369 fixinventory_plugin_k8s-4.0.4/fix_plugin_k8s/
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-24 19:30:49.000000 fixinventory_plugin_k8s-4.0.4/fix_plugin_k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19414 2024-04-24 19:30:49.000000 fixinventory_plugin_k8s-4.0.4/fix_plugin_k8s/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-24 19:30:49.000000 fixinventory_plugin_k8s-4.0.4/fix_plugin_k8s/collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:34:38.567369 fixinventory_plugin_k8s-4.0.4/fix_plugin_k8s/deferred_edges/
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-24 19:30:49.000000 fixinventory_plugin_k8s-4.0.4/fix_plugin_k8s/deferred_edges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-24 19:30:49.000000 fixinventory_plugin_k8s-4.0.4/fix_plugin_k8s/deferred_edges/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-24 19:30:49.000000 fixinventory_plugin_k8s-4.0.4/fix_plugin_k8s/deferred_edges/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-24 19:30:49.000000 fixinventory_plugin_k8s-4.0.4/fix_plugin_k8s/deferred_edges/digitalocean.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-24 19:30:49.000000 fixinventory_plugin_k8s-4.0.4/fix_plugin_k8s/deferred_edges/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   150075 2024-04-24 19:30:49.000000 fixinventory_plugin_k8s-4.0.4/fix_plugin_k8s/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:34:38.567369 fixinventory_plugin_k8s-4.0.4/fixinventory_plugin_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-24 19:34:38.000000 fixinventory_plugin_k8s-4.0.4/fixinventory_plugin_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-24 19:34:38.000000 fixinventory_plugin_k8s-4.0.4/fixinventory_plugin_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:34:38.000000 fixinventory_plugin_k8s-4.0.4/fixinventory_plugin_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 19:34:38.000000 fixinventory_plugin_k8s-4.0.4/fixinventory_plugin_k8s.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:31:52.000000 fixinventory_plugin_k8s-4.0.4/fixinventory_plugin_k8s.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-24 19:34:38.000000 fixinventory_plugin_k8s-4.0.4/fixinventory_plugin_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 19:34:38.000000 fixinventory_plugin_k8s-4.0.4/fixinventory_plugin_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-24 19:30:49.000000 fixinventory_plugin_k8s-4.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-24 19:34:38.567369 fixinventory_plugin_k8s-4.0.4/setup.cfg
```

### Comparing `fixinventory_plugin_k8s-4.0.3/PKG-INFO` & `fixinventory_plugin_k8s-4.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-k8s
-Version: 4.0.3
+Version: 4.0.4
 Summary: Fix Kubernetes Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/k8s
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
-Requires-Dist: fixinventorylib==4.0.3
+Requires-Dist: fixinventorylib==4.0.4
 Requires-Dist: kubernetes
 
 # fix-plugin-k8s
 
 Kubernetes plugin for Fix.
 See [Getting Started](https://inventory.fix.security/docs/getting-started) for more information.
```

### Comparing `fixinventory_plugin_k8s-4.0.3/fix_plugin_k8s/__init__.py` & `fixinventory_plugin_k8s-4.0.4/fix_plugin_k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_k8s-4.0.3/fix_plugin_k8s/base.py` & `fixinventory_plugin_k8s-4.0.4/fix_plugin_k8s/base.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_k8s-4.0.3/fix_plugin_k8s/collector.py` & `fixinventory_plugin_k8s-4.0.4/fix_plugin_k8s/collector.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_k8s-4.0.3/fix_plugin_k8s/deferred_edges/__init__.py` & `fixinventory_plugin_k8s-4.0.4/fix_plugin_k8s/deferred_edges/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_k8s-4.0.3/fix_plugin_k8s/deferred_edges/aws.py` & `fixinventory_plugin_k8s-4.0.4/fix_plugin_k8s/deferred_edges/aws.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_k8s-4.0.3/fix_plugin_k8s/deferred_edges/azure.py` & `fixinventory_plugin_k8s-4.0.4/fix_plugin_k8s/deferred_edges/azure.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_k8s-4.0.3/fix_plugin_k8s/deferred_edges/digitalocean.py` & `fixinventory_plugin_k8s-4.0.4/fix_plugin_k8s/deferred_edges/digitalocean.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_k8s-4.0.3/fix_plugin_k8s/resources.py` & `fixinventory_plugin_k8s-4.0.4/fix_plugin_k8s/resources.py`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_k8s-4.0.3/fixinventory_plugin_k8s.egg-info/PKG-INFO` & `fixinventory_plugin_k8s-4.0.4/fixinventory_plugin_k8s.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-k8s
-Version: 4.0.3
+Version: 4.0.4
 Summary: Fix Kubernetes Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/k8s
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
-Requires-Dist: fixinventorylib==4.0.3
+Requires-Dist: fixinventorylib==4.0.4
 Requires-Dist: kubernetes
 
 # fix-plugin-k8s
 
 Kubernetes plugin for Fix.
 See [Getting Started](https://inventory.fix.security/docs/getting-started) for more information.
```

### Comparing `fixinventory_plugin_k8s-4.0.3/fixinventory_plugin_k8s.egg-info/SOURCES.txt` & `fixinventory_plugin_k8s-4.0.4/fixinventory_plugin_k8s.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventory_plugin_k8s-4.0.3/pyproject.toml` & `fixinventory_plugin_k8s-4.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fixinventory-plugin-k8s"
 description = "Fix Kubernetes Collector Plugin"
-version = "4.0.3"
+version = "4.0.4"
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
-    "fixinventorylib==4.0.3",
+    "fixinventorylib==4.0.4",
     "kubernetes",
 ]
 
 [project.entry-points."fix.plugins"]
 k8s_collector = "fix_plugin_k8s:KubernetesCollectorPlugin"
 
 [project.urls]
```

