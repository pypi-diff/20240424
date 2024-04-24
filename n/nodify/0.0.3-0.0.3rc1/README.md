# Comparing `tmp/nodify-0.0.3.tar.gz` & `tmp/nodify-0.0.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodify-0.0.3.tar", last modified: Wed Apr 24 10:47:06 2024, max compression
+gzip compressed data, was "nodify-0.0.3rc1.tar", last modified: Wed Apr 24 10:39:09 2024, max compression
```

## Comparing `nodify-0.0.3.tar` & `nodify-0.0.3rc1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:06.836716 nodify-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-24 10:47:06.836716 nodify-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 10:46:56.000000 nodify-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-24 10:46:56.000000 nodify-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 10:47:06.836716 nodify-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:06.828716 nodify-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:06.832716 nodify-0.0.3/src/nodify/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-24 10:46:56.000000 nodify-0.0.3/src/nodify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-24 10:46:56.000000 nodify-0.0.3/src/nodify/_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-24 10:46:56.000000 nodify-0.0.3/src/nodify/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-04-24 10:46:56.000000 nodify-0.0.3/src/nodify/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-24 10:46:56.000000 nodify-0.0.3/src/nodify/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-24 10:46:56.000000 nodify-0.0.3/src/nodify/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-24 10:46:56.000000 nodify-0.0.3/src/nodify/file_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    26644 2024-04-24 10:46:56.000000 nodify-0.0.3/src/nodify/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-24 10:46:56.000000 nodify-0.0.3/src/nodify/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-04-24 10:46:56.000000 nodify-0.0.3/src/nodify/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-24 10:46:56.000000 nodify-0.0.3/src/nodify/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-24 10:46:56.000000 nodify-0.0.3/src/nodify/syntax_nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:06.832716 nodify-0.0.3/src/nodify/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:46:56.000000 nodify-0.0.3/src/nodify/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-24 10:46:56.000000 nodify-0.0.3/src/nodify/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-24 10:46:56.000000 nodify-0.0.3/src/nodify/tests/test_file_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-04-24 10:46:56.000000 nodify-0.0.3/src/nodify/tests/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-24 10:46:56.000000 nodify-0.0.3/src/nodify/tests/test_pythonscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-24 10:46:56.000000 nodify-0.0.3/src/nodify/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-24 10:46:56.000000 nodify-0.0.3/src/nodify/tests/test_syntax_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-24 10:46:56.000000 nodify-0.0.3/src/nodify/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-24 10:46:56.000000 nodify-0.0.3/src/nodify/tests/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-04-24 10:46:56.000000 nodify-0.0.3/src/nodify/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    37802 2024-04-24 10:46:56.000000 nodify-0.0.3/src/nodify/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:06.832716 nodify-0.0.3/src/nodify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-24 10:47:06.000000 nodify-0.0.3/src/nodify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-24 10:47:06.000000 nodify-0.0.3/src/nodify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:47:06.000000 nodify-0.0.3/src/nodify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 10:47:06.000000 nodify-0.0.3/src/nodify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 10:47:06.000000 nodify-0.0.3/src/nodify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:09.692509 nodify-0.0.3rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-24 10:39:09.692509 nodify-0.0.3rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 10:39:09.692509 nodify-0.0.3rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:09.688509 nodify-0.0.3rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:09.688509 nodify-0.0.3rc1/src/nodify/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/src/nodify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/src/nodify/_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/src/nodify/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/src/nodify/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/src/nodify/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/src/nodify/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/src/nodify/file_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26644 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/src/nodify/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/src/nodify/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/src/nodify/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/src/nodify/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/src/nodify/syntax_nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:09.692509 nodify-0.0.3rc1/src/nodify/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/src/nodify/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/src/nodify/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/src/nodify/tests/test_file_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/src/nodify/tests/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/src/nodify/tests/test_pythonscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/src/nodify/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/src/nodify/tests/test_syntax_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/src/nodify/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/src/nodify/tests/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/src/nodify/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37802 2024-04-24 10:39:02.000000 nodify-0.0.3rc1/src/nodify/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:39:09.692509 nodify-0.0.3rc1/src/nodify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-24 10:39:09.000000 nodify-0.0.3rc1/src/nodify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-24 10:39:09.000000 nodify-0.0.3rc1/src/nodify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:39:09.000000 nodify-0.0.3rc1/src/nodify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 10:39:09.000000 nodify-0.0.3rc1/src/nodify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 10:39:09.000000 nodify-0.0.3rc1/src/nodify.egg-info/top_level.txt
```

### Comparing `nodify-0.0.3/PKG-INFO` & `nodify-0.0.3rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: nodify
-Version: 0.0.3
+Version: 0.0.3rc1
 Summary: Supercharge your functional application with a powerful node system.
 Author-email: Pol Febrer <pfebrer96@gmail.com>
 Maintainer: Pol Febrer
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Requires-Dist: numpy
 Provides-Extra: scripting
 Requires-Dist: black; extra == "scripting"
 Requires-Dist: isort; extra == "scripting"
 Provides-Extra: files
 Requires-Dist: watchdog; extra == "files"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
```

### Comparing `nodify-0.0.3/pyproject.toml` & `nodify-0.0.3rc1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 [project]
 requires-python = ">=3.9"
 
 name = "nodify"
 description = "Supercharge your functional application with a powerful node system."
 readme = "README.md"
 license = {text = "MIT"}
-version = "0.0.3"
+version = "0.0.3rc1"
 
-dependencies = []
+dependencies = [
+    "numpy",
+]
 
 authors = [
     {name = "Pol Febrer", email = "pfebrer96@gmail.com"}
 ]
 maintainers = [{name="Pol Febrer"}]
 
 classifiers = [
```

### Comparing `nodify-0.0.3/src/nodify/_env.py` & `nodify-0.0.3rc1/src/nodify/_env.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.3/src/nodify/context.py` & `nodify-0.0.3rc1/src/nodify/context.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.3/src/nodify/conversions.py` & `nodify-0.0.3rc1/src/nodify/conversions.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.3/src/nodify/dispatcher.py` & `nodify-0.0.3rc1/src/nodify/dispatcher.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.3/src/nodify/errors.py` & `nodify-0.0.3rc1/src/nodify/errors.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.3/src/nodify/file_nodes.py` & `nodify-0.0.3rc1/src/nodify/file_nodes.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.3/src/nodify/node.py` & `nodify-0.0.3rc1/src/nodify/node.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.3/src/nodify/operators.py` & `nodify-0.0.3rc1/src/nodify/operators.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.3/src/nodify/parse.py` & `nodify-0.0.3rc1/src/nodify/parse.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.3/src/nodify/registry.py` & `nodify-0.0.3rc1/src/nodify/registry.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.3/src/nodify/syntax_nodes.py` & `nodify-0.0.3rc1/src/nodify/syntax_nodes.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.3/src/nodify/tests/test_context.py` & `nodify-0.0.3rc1/src/nodify/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.3/src/nodify/tests/test_file_nodes.py` & `nodify-0.0.3rc1/src/nodify/tests/test_file_nodes.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.3/src/nodify/tests/test_node.py` & `nodify-0.0.3rc1/src/nodify/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.3/src/nodify/tests/test_pythonscript.py` & `nodify-0.0.3rc1/src/nodify/tests/test_pythonscript.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.3/src/nodify/tests/test_registry.py` & `nodify-0.0.3rc1/src/nodify/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.3/src/nodify/tests/test_syntax_nodes.py` & `nodify-0.0.3rc1/src/nodify/tests/test_syntax_nodes.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.3/src/nodify/tests/test_utils.py` & `nodify-0.0.3rc1/src/nodify/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.3/src/nodify/tests/test_workflow.py` & `nodify-0.0.3rc1/src/nodify/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.3/src/nodify/utils.py` & `nodify-0.0.3rc1/src/nodify/utils.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.3/src/nodify/workflow.py` & `nodify-0.0.3rc1/src/nodify/workflow.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.3/src/nodify.egg-info/PKG-INFO` & `nodify-0.0.3rc1/src/nodify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: nodify
-Version: 0.0.3
+Version: 0.0.3rc1
 Summary: Supercharge your functional application with a powerful node system.
 Author-email: Pol Febrer <pfebrer96@gmail.com>
 Maintainer: Pol Febrer
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Requires-Dist: numpy
 Provides-Extra: scripting
 Requires-Dist: black; extra == "scripting"
 Requires-Dist: isort; extra == "scripting"
 Provides-Extra: files
 Requires-Dist: watchdog; extra == "files"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
```

### Comparing `nodify-0.0.3/src/nodify.egg-info/SOURCES.txt` & `nodify-0.0.3rc1/src/nodify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

