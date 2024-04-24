# Comparing `tmp/fixinventoryworker-4.0.2.tar.gz` & `tmp/fixinventoryworker-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventoryworker-4.0.2.tar", last modified: Fri Apr 12 12:17:07 2024, max compression
+gzip compressed data, was "fixinventoryworker-4.0.3.tar", last modified: Wed Apr 24 10:33:10 2024, max compression
```

## Comparing `fixinventoryworker-4.0.2.tar` & `fixinventoryworker-4.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:07.908364 fixinventoryworker-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:12:52.000000 fixinventoryworker-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-12 12:17:07.908364 fixinventoryworker-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-12 12:12:52.000000 fixinventoryworker-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:07.908364 fixinventoryworker-4.0.2/fixinventoryworker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-12 12:17:07.000000 fixinventoryworker-4.0.2/fixinventoryworker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-12 12:17:07.000000 fixinventoryworker-4.0.2/fixinventoryworker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:17:07.000000 fixinventoryworker-4.0.2/fixinventoryworker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-12 12:17:07.000000 fixinventoryworker-4.0.2/fixinventoryworker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:14:21.000000 fixinventoryworker-4.0.2/fixinventoryworker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-12 12:17:07.000000 fixinventoryworker-4.0.2/fixinventoryworker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 12:17:07.000000 fixinventoryworker-4.0.2/fixinventoryworker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:07.908364 fixinventoryworker-4.0.2/fixworker/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 12:12:52.000000 fixinventoryworker-4.0.2/fixworker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13357 2024-04-12 12:12:52.000000 fixinventoryworker-4.0.2/fixworker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-04-12 12:12:52.000000 fixinventoryworker-4.0.2/fixworker/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-04-12 12:12:52.000000 fixinventoryworker-4.0.2/fixworker/collect.py
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-12 12:12:52.000000 fixinventoryworker-4.0.2/fixworker/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-12 12:12:52.000000 fixinventoryworker-4.0.2/fixworker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-04-12 12:12:52.000000 fixinventoryworker-4.0.2/fixworker/fixcore.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-04-12 12:12:52.000000 fixinventoryworker-4.0.2/fixworker/pluginloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-12 12:12:52.000000 fixinventoryworker-4.0.2/fixworker/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-12 12:12:52.000000 fixinventoryworker-4.0.2/fixworker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-12 12:12:52.000000 fixinventoryworker-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 12:17:07.908364 fixinventoryworker-4.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:07.908364 fixinventoryworker-4.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:12:52.000000 fixinventoryworker-4.0.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-12 12:12:52.000000 fixinventoryworker-4.0.2/test/fakeconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-12 12:12:52.000000 fixinventoryworker-4.0.2/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-12 12:12:52.000000 fixinventoryworker-4.0.2/test/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-12 12:12:52.000000 fixinventoryworker-4.0.2/test/test_fixcore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-12 12:12:52.000000 fixinventoryworker-4.0.2/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:10.149128 fixinventoryworker-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 10:29:14.000000 fixinventoryworker-4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-24 10:33:10.149128 fixinventoryworker-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-24 10:29:14.000000 fixinventoryworker-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:10.149128 fixinventoryworker-4.0.3/fixinventoryworker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-24 10:33:10.000000 fixinventoryworker-4.0.3/fixinventoryworker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-24 10:33:10.000000 fixinventoryworker-4.0.3/fixinventoryworker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:33:10.000000 fixinventoryworker-4.0.3/fixinventoryworker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 10:33:10.000000 fixinventoryworker-4.0.3/fixinventoryworker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:30:23.000000 fixinventoryworker-4.0.3/fixinventoryworker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-24 10:33:10.000000 fixinventoryworker-4.0.3/fixinventoryworker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 10:33:10.000000 fixinventoryworker-4.0.3/fixinventoryworker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:10.149128 fixinventoryworker-4.0.3/fixworker/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 10:29:14.000000 fixinventoryworker-4.0.3/fixworker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13357 2024-04-24 10:29:14.000000 fixinventoryworker-4.0.3/fixworker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-04-24 10:29:14.000000 fixinventoryworker-4.0.3/fixworker/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-04-24 10:29:14.000000 fixinventoryworker-4.0.3/fixworker/collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-24 10:29:14.000000 fixinventoryworker-4.0.3/fixworker/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-24 10:29:14.000000 fixinventoryworker-4.0.3/fixworker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-04-24 10:29:14.000000 fixinventoryworker-4.0.3/fixworker/fixcore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-04-24 10:29:14.000000 fixinventoryworker-4.0.3/fixworker/pluginloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-24 10:29:14.000000 fixinventoryworker-4.0.3/fixworker/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-24 10:29:14.000000 fixinventoryworker-4.0.3/fixworker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-24 10:29:14.000000 fixinventoryworker-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 10:33:10.149128 fixinventoryworker-4.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:10.149128 fixinventoryworker-4.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:29:14.000000 fixinventoryworker-4.0.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-24 10:29:14.000000 fixinventoryworker-4.0.3/test/fakeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-24 10:29:14.000000 fixinventoryworker-4.0.3/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-24 10:29:14.000000 fixinventoryworker-4.0.3/test/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-24 10:29:14.000000 fixinventoryworker-4.0.3/test/test_fixcore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-24 10:29:14.000000 fixinventoryworker-4.0.3/test/test_utils.py
```

### Comparing `fixinventoryworker-4.0.2/PKG-INFO` & `fixinventoryworker-4.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: fixinventoryworker
-Version: 4.0.2
+Version: 4.0.3
 Summary: Runs collector plugins and sends the result to fixcore.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/fixworker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.2
+Requires-Dist: fixinventorylib==4.0.3
 Requires-Dist: tenacity
 Requires-Dist: CherryPy
 
 # `fixworker`
 Fix worker daemon
```

### Comparing `fixinventoryworker-4.0.2/README.md` & `fixinventoryworker-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.2/fixinventoryworker.egg-info/PKG-INFO` & `fixinventoryworker-4.0.3/fixinventoryworker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: fixinventoryworker
-Version: 4.0.2
+Version: 4.0.3
 Summary: Runs collector plugins and sends the result to fixcore.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/fixworker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.2
+Requires-Dist: fixinventorylib==4.0.3
 Requires-Dist: tenacity
 Requires-Dist: CherryPy
 
 # `fixworker`
 Fix worker daemon
```

### Comparing `fixinventoryworker-4.0.2/fixinventoryworker.egg-info/SOURCES.txt` & `fixinventoryworker-4.0.3/fixinventoryworker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.2/fixworker/__main__.py` & `fixinventoryworker-4.0.3/fixworker/__main__.py`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.2/fixworker/cleanup.py` & `fixinventoryworker-4.0.3/fixworker/cleanup.py`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.2/fixworker/collect.py` & `fixinventoryworker-4.0.3/fixworker/collect.py`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.2/fixworker/config.py` & `fixinventoryworker-4.0.3/fixworker/config.py`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.2/fixworker/fixcore.py` & `fixinventoryworker-4.0.3/fixworker/fixcore.py`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.2/fixworker/pluginloader.py` & `fixinventoryworker-4.0.3/fixworker/pluginloader.py`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.2/fixworker/tag.py` & `fixinventoryworker-4.0.3/fixworker/tag.py`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.2/fixworker/utils.py` & `fixinventoryworker-4.0.3/fixworker/utils.py`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.2/pyproject.toml` & `fixinventoryworker-4.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "fixinventoryworker"
-version = "4.0.2"
+version = "4.0.3"
 authors = [{ name = "Some Engineering Inc." }]
 description = "Runs collector plugins and sends the result to fixcore."
 license = { text="AGPLv3" }
 requires-python = ">=3.11"
 classifiers = ["Programming Language :: Python :: 3"]
 readme = { file = "README.md", content-type = "text/markdown" }
 
 dependencies = [
-    "fixinventorylib==4.0.2",
+    "fixinventorylib==4.0.3",
     "tenacity",
     "CherryPy",
 ]
 
 [project.scripts]
 fixworker = "fixworker.__main__:main"
 resotoworker = "fixworker.__main__:main"
```

### Comparing `fixinventoryworker-4.0.2/test/test_args.py` & `fixinventoryworker-4.0.3/test/test_args.py`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.2/test/test_collect.py` & `fixinventoryworker-4.0.3/test/test_collect.py`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.2/test/test_fixcore.py` & `fixinventoryworker-4.0.3/test/test_fixcore.py`

 * *Files identical despite different names*

### Comparing `fixinventoryworker-4.0.2/test/test_utils.py` & `fixinventoryworker-4.0.3/test/test_utils.py`

 * *Files identical despite different names*

